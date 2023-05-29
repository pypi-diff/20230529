# Comparing `tmp/alacorder-80.8.4.tar.gz` & `tmp/alacorder-80.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.4.tar", max compression
+gzip compressed data, was "alacorder-80.8.5.tar", max compression
```

## Comparing `alacorder-80.8.4.tar` & `alacorder-80.8.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.4/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.4/README.md
--rw-r--r--   0        0        0      746 2023-05-27 19:48:40.042778 alacorder-80.8.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-27 17:58:28.272608 alacorder-80.8.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.4/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   279759 2023-05-27 19:48:11.877769 alacorder-80.8.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   279759 2023-05-27 19:48:07.702290 alacorder-80.8.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 alacorder-80.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.5/LICENSE
+-rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.5/README.md
+-rw-r--r--   0        0        0      746 2023-05-29 15:57:01.593196 alacorder-80.8.5/pyproject.toml
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   281427 2023-05-29 15:56:03.618301 alacorder-80.8.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   281427 2023-05-29 15:55:57.780550 alacorder-80.8.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 alacorder-80.8.5/PKG-INFO
```

### Comparing `alacorder-80.8.4/LICENSE` & `alacorder-80.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.4/README.md` & `alacorder-80.8.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.4/pyproject.toml` & `alacorder-80.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.4"
+version = "80.8.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.8.4/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.5/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.4/src/alacorder/__main__.py` & `alacorder-80.8.5/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.4"
+version = "80.8.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1218,14 +1218,15 @@
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DOB"),
             pl.col("AllPagesTextNoNewLine")
             .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
@@ -3177,14 +3178,59 @@
             .alias("VictimDOB"),
         ]
     )
     sent = sent.drop_nulls("Number")
     sent = sent.fill_null("")
     return sent
 
+def autopair(pairs_template, adoc_pairs):
+    adoc_pairs = adoc_pairs.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name"),
+            pl.concat_str(
+                [
+                    pl.col("Name").str.extract(r'^([A-Z]+)'), # last name
+                    pl.lit(" "),
+                    pl.col("Name").str.extract(r', ([A-Z]+)'), # first name
+                    pl.lit(" "),
+                    pl.col("YOB").cast(pl.Utf8)
+                ]
+            )
+            .alias("LastFirstYOB")
+        ]
+    )
+    if pl.Date in pairs_template.select("DOB").dtypes:
+        pairs_template = pairs_template.with_columns(pl.col("DOB").dt.strftime('%m/%d/%Y'))
+    pairs_template = pairs_template.with_columns(
+        pl.concat_str(
+            [
+                pl.col("Name").str.extract(r'^([A-Z]+)'), # last name
+                pl.lit(" "),
+                pl.col("Name").str.extract(r'^[A-Z]+ ([A-Z]+)'), # first name
+                pl.lit(" "),
+                pl.col("DOB").str.extract(r'\d\d/\d\d/(\d\d\d\d)') # yob
+            ]
+        )
+        .alias("LastFirstYOB")
+    )
+    pairs_template = pairs_template.join(adoc_pairs, on="LastFirstYOB", how="left")
+    pairs_template = pairs_template.drop("LastFirstYOB","Name_right","AIS / Unique ID")
+    pairs_template = pairs_template.select(
+        [
+            pl.col("AIS").alias("AIS / Unique ID"),
+            pl.col("Name"),
+            pl.col("Alias"),
+            pl.col("DOB"),
+            pl.col("CaseCount"),
+            pl.col("Cases")
+        ]
+    )
+    return pairs_template
+
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
 def read_query(path, window=None):
     if isinstance(path, dict):
         cf = path
@@ -4857,14 +4903,15 @@
             window["MT"].update(disabled=True)
         elif event == "ADOC-FETCH-NEWQUERY":
             if window["ADOC-FETCH-INPUTPATH"].get() == '':
                 sg.popup("Enter valid path and try again.")
                 continue
             out = pl.DataFrame({'AIS': [], 'FirstName': [], 'LastName': []})
             write(out, sheet_names=["adoc-fetch-template"], path=window["ADOC-FETCH-INPUTPATH"].get())
+            sg.popup("Template created.")
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
```

### Comparing `alacorder-80.8.4/src/alacorder/alac.py` & `alacorder-80.8.5/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.4"
+version = "80.8.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1218,14 +1218,15 @@
             .str.replace(r"C$", "")
             .str.strip()
             .alias("Name"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace_all(r"[^\d/]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DOB"),
             pl.col("AllPagesTextNoNewLine")
             .str.extract(r"(SSN\:)(.{0,100})(Alias 1)", group_index=2)
             .str.replace(r"(SSN)", "")
             .str.replace(r"Alias", "")
             .str.replace(r"\:", "")
             .str.strip()
@@ -3177,14 +3178,59 @@
             .alias("VictimDOB"),
         ]
     )
     sent = sent.drop_nulls("Number")
     sent = sent.fill_null("")
     return sent
 
+def autopair(pairs_template, adoc_pairs):
+    adoc_pairs = adoc_pairs.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name"),
+            pl.concat_str(
+                [
+                    pl.col("Name").str.extract(r'^([A-Z]+)'), # last name
+                    pl.lit(" "),
+                    pl.col("Name").str.extract(r', ([A-Z]+)'), # first name
+                    pl.lit(" "),
+                    pl.col("YOB").cast(pl.Utf8)
+                ]
+            )
+            .alias("LastFirstYOB")
+        ]
+    )
+    if pl.Date in pairs_template.select("DOB").dtypes:
+        pairs_template = pairs_template.with_columns(pl.col("DOB").dt.strftime('%m/%d/%Y'))
+    pairs_template = pairs_template.with_columns(
+        pl.concat_str(
+            [
+                pl.col("Name").str.extract(r'^([A-Z]+)'), # last name
+                pl.lit(" "),
+                pl.col("Name").str.extract(r'^[A-Z]+ ([A-Z]+)'), # first name
+                pl.lit(" "),
+                pl.col("DOB").str.extract(r'\d\d/\d\d/(\d\d\d\d)') # yob
+            ]
+        )
+        .alias("LastFirstYOB")
+    )
+    pairs_template = pairs_template.join(adoc_pairs, on="LastFirstYOB", how="left")
+    pairs_template = pairs_template.drop("LastFirstYOB","Name_right","AIS / Unique ID")
+    pairs_template = pairs_template.select(
+        [
+            pl.col("AIS").alias("AIS / Unique ID"),
+            pl.col("Name"),
+            pl.col("Alias"),
+            pl.col("DOB"),
+            pl.col("CaseCount"),
+            pl.col("Cases")
+        ]
+    )
+    return pairs_template
+
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
 def read_query(path, window=None):
     if isinstance(path, dict):
         cf = path
@@ -4857,14 +4903,15 @@
             window["MT"].update(disabled=True)
         elif event == "ADOC-FETCH-NEWQUERY":
             if window["ADOC-FETCH-INPUTPATH"].get() == '':
                 sg.popup("Enter valid path and try again.")
                 continue
             out = pl.DataFrame({'AIS': [], 'FirstName': [], 'LastName': []})
             write(out, sheet_names=["adoc-fetch-template"], path=window["ADOC-FETCH-INPUTPATH"].get())
+            sg.popup("Template created.")
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
```

### Comparing `alacorder-80.8.4/PKG-INFO` & `alacorder-80.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.4
+Version: 80.8.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


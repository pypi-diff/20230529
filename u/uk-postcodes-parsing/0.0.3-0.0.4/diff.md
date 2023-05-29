# Comparing `tmp/uk_postcodes_parsing-0.0.3.tar.gz` & `tmp/uk_postcodes_parsing-0.0.4.tar.gz`

## Comparing `uk_postcodes_parsing-0.0.3.tar` & `uk_postcodes_parsing-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/LICENSE
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/README.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.0.3/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.3/.github/workflows/test.yml` & `uk_postcodes_parsing-0.0.4/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Test
 
 on: 
   push:
     paths:
       - 'tests/**'
-      - 'src/ukpostcodes/**'
+      - 'src/uk_postcodes_parsing/**'
   workflow_dispatch:
 
 jobs:
   Quality-checks:
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.3/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
     r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}"
 )
 
 
 def _parse(postcode: str) -> dict:
+    if postcode.upper().startswith("NPT"):  # Edge case logging
+        logger.info("Found 'NPT' Newport postcode discontinued in 1984.")
     if not is_valid(postcode):
         return None
     return {
         "postcode": to_normalised(postcode),
         "incode": to_incode(postcode),
         "outcode": to_outcode(postcode),
         "area": to_area(postcode),
```

### Comparing `uk_postcodes_parsing-0.0.3/tests/test_all.py` & `uk_postcodes_parsing-0.0.4/tests/test_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             district="EH16",
             sub_district=None,
             sector="EH16 5",
             unit="OY",
         ),
     ]
 
+
 def test_parsing_detailed():
     df = pd.read_csv("tests/data/postcode_parse_test.csv")
     df = df.where(pd.notnull(df), None)
 
     parsed_postcodes = df["Postcode"].apply(ukpostcode.parse)
 
     for i, parsed_postcode in enumerate(parsed_postcodes):
```

### Comparing `uk_postcodes_parsing-0.0.3/.gitignore` & `uk_postcodes_parsing-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.3/LICENSE` & `uk_postcodes_parsing-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.3/pyproject.toml` & `uk_postcodes_parsing-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
 description = "A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```


# Comparing `tmp/ietf_reviewtool-0.3.0.tar.gz` & `tmp/ietf_reviewtool-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ietf_reviewtool-0.3.0.tar", max compression
+gzip compressed data, was "ietf_reviewtool-0.3.1.tar", max compression
```

## Comparing `ietf_reviewtool-0.3.0.tar` & `ietf_reviewtool-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    18092 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/LICENSE
--rw-r--r--   0        0        0     6700 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/README.md
--rw-r--r--   0        0        0      285 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/__init__.py
--rw-r--r--   0        0        0      146 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/__main__.py
--rw-r--r--   0        0        0     1183 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/agenda.py
--rw-r--r--   0        0        0    14217 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/boilerplate.py
--rw-r--r--   0        0        0     5144 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/doc.py
--rw-r--r--   0        0        0     4181 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/grammar.py
--rwxr-xr-x   0        0        0    30018 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/ietf_reviewtool.py
--rw-r--r--   0        0        0     2527 2023-05-29 14:33:51.708521 ietf_reviewtool-0.3.0/ietf_reviewtool/inclusive.py
--rw-r--r--   0        0        0     4829 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/metadata.py
--rw-r--r--   0        0        0    10926 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/references.py
--rw-r--r--   0        0        0    10872 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/review.py
--rw-r--r--   0        0        0        0 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/__init__.py
--rw-r--r--   0        0        0     2970 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/docposition.py
--rw-r--r--   0        0        0    11456 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/fetch.py
--rw-r--r--   0        0        0     2936 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/format.py
--rw-r--r--   0        0        0    10522 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/text.py
--rw-r--r--   0        0        0     2033 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/ietf_reviewtool/util/utils.py
--rw-r--r--   0        0        0     1376 2023-05-29 14:33:51.712521 ietf_reviewtool-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 ietf_reviewtool-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6700 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/README.md
+-rw-r--r--   0        0        0      285 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/__main__.py
+-rw-r--r--   0        0        0     1183 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/agenda.py
+-rw-r--r--   0        0        0    14217 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/boilerplate.py
+-rw-r--r--   0        0        0     5144 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/doc.py
+-rw-r--r--   0        0        0     4181 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/grammar.py
+-rwxr-xr-x   0        0        0    30018 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/ietf_reviewtool.py
+-rw-r--r--   0        0        0     2527 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/inclusive.py
+-rw-r--r--   0        0        0     4829 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/metadata.py
+-rw-r--r--   0        0        0    10926 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/references.py
+-rw-r--r--   0        0        0    10872 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/review.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/__init__.py
+-rw-r--r--   0        0        0     2970 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/docposition.py
+-rw-r--r--   0        0        0    11456 2023-05-29 14:45:57.112254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/fetch.py
+-rw-r--r--   0        0        0     2936 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/format.py
+-rw-r--r--   0        0        0    10386 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/text.py
+-rw-r--r--   0        0        0     2033 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/ietf_reviewtool/util/utils.py
+-rw-r--r--   0        0        0     1376 2023-05-29 14:45:57.116254 ietf_reviewtool-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7698 1970-01-01 00:00:00.000000 ietf_reviewtool-0.3.1/PKG-INFO
```

### Comparing `ietf_reviewtool-0.3.0/LICENSE` & `ietf_reviewtool-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/README.md` & `ietf_reviewtool-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/agenda.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/agenda.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/boilerplate.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/boilerplate.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/doc.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/doc.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/grammar.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/grammar.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/ietf_reviewtool.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/ietf_reviewtool.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/inclusive.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/inclusive.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/metadata.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/metadata.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/references.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/references.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/review.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/review.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/util/docposition.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/util/docposition.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/util/fetch.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/util/fetch.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/util/format.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/util/format.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/util/text.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/util/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,14 @@
             )
         except UnicodeDecodeError as err:
             log.warning("Could not extract URLs: %s", err)
             return {}
 
         for url in extracted_urls:
             url = url.rstrip(".\"]'>;,)")
-            if re.match(r"[\d\.:a-f]+", url, flags=re.IGNORECASE):
-                # skip literal IP addresses
-                continue
             try:
                 urllib.parse.urlparse(url).netloc
             except ValueError as err:
                 log.warning("%s: %s", err, url)
                 continue
 
             urls[part].add(url)
```

### Comparing `ietf_reviewtool-0.3.0/ietf_reviewtool/util/utils.py` & `ietf_reviewtool-0.3.1/ietf_reviewtool/util/utils.py`

 * *Files identical despite different names*

### Comparing `ietf_reviewtool-0.3.0/pyproject.toml` & `ietf_reviewtool-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ietf-reviewtool"
-version = "0.3.0"
+version = "0.3.1"
 description = "Review tool for IETF documents"
 authors = ["Lars Eggert <lars@eggert.org>"]
 readme = "README.md"
 homepage = "https://github.com/larseggert/ietf-reviewtool"
 repository = "https://github.com/larseggert/ietf-reviewtool"
 license = "GPL-2.0-only"
```

### Comparing `ietf_reviewtool-0.3.0/PKG-INFO` & `ietf_reviewtool-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ietf-reviewtool
-Version: 0.3.0
+Version: 0.3.1
 Summary: Review tool for IETF documents
 Home-page: https://github.com/larseggert/ietf-reviewtool
 License: GPL-2.0-only
 Author: Lars Eggert
 Author-email: lars@eggert.org
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```


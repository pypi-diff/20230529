# Comparing `tmp/modo_data_science_helpers-0.2.0.tar.gz` & `tmp/modo_data_science_helpers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modo_data_science_helpers-0.2.0.tar", max compression
+gzip compressed data, was "modo_data_science_helpers-0.3.0.tar", max compression
```

## Comparing `modo_data_science_helpers-0.2.0.tar` & `modo_data_science_helpers-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1494 2023-05-12 11:08:38.864353 modo_data_science_helpers-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.2.0/modo_data_science_helpers/__init__.py
--rw-r--r--   0        0        0     4101 2023-05-12 14:52:45.858633 modo_data_science_helpers-0.2.0/modo_data_science_helpers/aws_utils.py
--rw-r--r--   0        0        0      454 2023-05-18 12:34:28.987670 modo_data_science_helpers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1494 2023-05-12 11:08:38.864353 modo_data_science_helpers-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 10:39:55.207198 modo_data_science_helpers-0.3.0/modo_data_science_helpers/__init__.py
+-rw-r--r--   0        0        0     4101 2023-05-12 14:52:45.858633 modo_data_science_helpers-0.3.0/modo_data_science_helpers/aws_utils.py
+-rw-r--r--   0        0        0      454 2023-05-29 17:44:15.642649 modo_data_science_helpers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 modo_data_science_helpers-0.3.0/PKG-INFO
```

### Comparing `modo_data_science_helpers-0.2.0/README.md` & `modo_data_science_helpers-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `modo_data_science_helpers-0.2.0/modo_data_science_helpers/aws_utils.py` & `modo_data_science_helpers-0.3.0/modo_data_science_helpers/aws_utils.py`

 * *Files identical despite different names*

### Comparing `modo_data_science_helpers-0.2.0/PKG-INFO` & `modo_data_science_helpers-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: modo-data-science-helpers
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helpers for AWS most common operations. Includes clipboard auth
 Author: Esteban Elia
 Author-email: esteban.elia@modo.com.ar
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: awswrangler (>=3.1.1,<4.0.0)
 Requires-Dist: boto3 (>=1.26.135,<2.0.0)
 Requires-Dist: clipboard (>=0.0.4,<0.0.5)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
```


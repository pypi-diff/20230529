# Comparing `tmp/paketmutfak-1.1.8.tar.gz` & `tmp/paketmutfak-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paketmutfak-1.1.8.tar", max compression
+gzip compressed data, was "paketmutfak-1.1.9.tar", max compression
```

## Comparing `paketmutfak-1.1.8.tar` & `paketmutfak-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0       22 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/__init__.py
--rw-r--r--   0        0        0     5968 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/db/LogDbBase.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/db/__init__.py
--rw-r--r--   0        0        0     3082 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/db/dynamo_db_base_class.py
--rw-r--r--   0        0        0    16321 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/db/sql_db_base_class.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/mail/__init__.py
--rw-r--r--   0        0        0     3539 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/mail/aws_ses.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/__init__.py
--rw-r--r--   0        0        0     7424 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/PM.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/__init__.py
--rw-r--r--   0        0        0     5305 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/error_codes.py
--rw-r--r--   0        0        0      113 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/log_levels.py
--rw-r--r--   0        0        0      525 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/parameters.py
--rw-r--r--   0        0        0     1101 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/constants/platforms.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/formats/__init__.py
--rw-r--r--   0        0        0     7173 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/formats/order.py
--rw-r--r--   0        0        0        0 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/functions/__init__.py
--rw-r--r--   0        0        0    22794 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/functions/general.py
--rw-r--r--   0        0        0     2785 2023-03-22 08:30:51.148187 paketmutfak-1.1.8/paketmutfak/utils/functions/regions.py
--rw-r--r--   0        0        0     1246 2023-03-22 08:31:18.395857 paketmutfak-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 paketmutfak-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0       22 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/__init__.py
+-rw-r--r--   0        0        0     5968 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/db/LogDbBase.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/db/__init__.py
+-rw-r--r--   0        0        0     3082 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/db/dynamo_db_base_class.py
+-rw-r--r--   0        0        0    16321 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/db/sql_db_base_class.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/mail/__init__.py
+-rw-r--r--   0        0        0     3539 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/mail/aws_ses.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/__init__.py
+-rw-r--r--   0        0        0     7424 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/PM.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/__init__.py
+-rw-r--r--   0        0        0     5305 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/error_codes.py
+-rw-r--r--   0        0        0      113 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/log_levels.py
+-rw-r--r--   0        0        0      525 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/parameters.py
+-rw-r--r--   0        0        0     1101 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/constants/platforms.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/formats/__init__.py
+-rw-r--r--   0        0        0     7173 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/formats/order.py
+-rw-r--r--   0        0        0        0 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/functions/__init__.py
+-rw-r--r--   0        0        0    22794 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/functions/general.py
+-rw-r--r--   0        0        0     2785 2023-03-22 09:08:03.247518 paketmutfak-1.1.9/paketmutfak/utils/functions/regions.py
+-rw-r--r--   0        0        0     1246 2023-03-22 09:08:24.887457 paketmutfak-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 paketmutfak-1.1.9/PKG-INFO
```

### Comparing `paketmutfak-1.1.8/LICENSE.txt` & `paketmutfak-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/db/LogDbBase.py` & `paketmutfak-1.1.9/paketmutfak/db/LogDbBase.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/db/dynamo_db_base_class.py` & `paketmutfak-1.1.9/paketmutfak/db/dynamo_db_base_class.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/db/sql_db_base_class.py` & `paketmutfak-1.1.9/paketmutfak/db/sql_db_base_class.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/mail/aws_ses.py` & `paketmutfak-1.1.9/paketmutfak/mail/aws_ses.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/constants/PM.py` & `paketmutfak-1.1.9/paketmutfak/utils/constants/PM.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/constants/error_codes.py` & `paketmutfak-1.1.9/paketmutfak/utils/constants/error_codes.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/constants/parameters.py` & `paketmutfak-1.1.9/paketmutfak/utils/constants/parameters.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/constants/platforms.py` & `paketmutfak-1.1.9/paketmutfak/utils/constants/platforms.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/formats/order.py` & `paketmutfak-1.1.9/paketmutfak/utils/formats/order.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/functions/general.py` & `paketmutfak-1.1.9/paketmutfak/utils/functions/general.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/paketmutfak/utils/functions/regions.py` & `paketmutfak-1.1.9/paketmutfak/utils/functions/regions.py`

 * *Files identical despite different names*

### Comparing `paketmutfak-1.1.8/pyproject.toml` & `paketmutfak-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paketmutfak"
-version = "1.1.8"
+version = "1.1.9"
 description = "Library of code for working with paket mutfak"
 authors = ["Paket Mutfak <dev@paketmutfak.com.tr>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.1.3"
```

### Comparing `paketmutfak-1.1.8/PKG-INFO` & `paketmutfak-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paketmutfak
-Version: 1.1.8
+Version: 1.1.9
 Summary: Library of code for working with paket mutfak
 Author: Paket Mutfak
 Author-email: dev@paketmutfak.com.tr
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


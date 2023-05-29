# Comparing `tmp/pyheartlib-0.0.7.tar.gz` & `tmp/pyheartlib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartlib-0.0.7.tar", max compression
+gzip compressed data, was "pyheartlib-0.0.8.tar", max compression
```

## Comparing `pyheartlib-0.0.7.tar` & `pyheartlib-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       59 2023-05-29 09:26:57.636241 pyheartlib-0.0.7/LICENSE
--rw-r--r--   0        0        0     2438 2023-05-29 09:26:57.636241 pyheartlib-0.0.7/README.md
--rw-r--r--   0        0        0     1429 2023-05-29 09:28:47.204727 pyheartlib-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/__init__.py
--rw-r--r--   0        0        0       54 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/archs/__init__.py
--rw-r--r--   0        0        0    17957 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/beat_info.py
--rw-r--r--   0        0        0     1160 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/config.yaml
--rw-r--r--   0        0        0     5429 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data.py
--rw-r--r--   0        0        0     9295 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_arrhythmia.py
--rw-r--r--   0        0        0    23957 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_beat.py
--rw-r--r--   0        0        0     9605 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_rpeak.py
--rw-r--r--   0        0        0       39 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/pqrst.py
--rw-r--r--   0        0        0     2827 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/report.py
--rw-r--r--   0        0        0     5887 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/utils.py
--rw-r--r--   0        0        0     6150 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/features.py
--rw-r--r--   0        0        0     2579 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/io.py
--rw-r--r--   0        0        0     5773 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/processing.py
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyheartlib-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-29 11:04:46.307576 pyheartlib-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2438 2023-05-29 11:04:46.307576 pyheartlib-0.0.8/README.md
+-rw-r--r--   0        0        0     1429 2023-05-29 11:06:26.363587 pyheartlib-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/archs/__init__.py
+-rw-r--r--   0        0        0    17957 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/beat_info.py
+-rw-r--r--   0        0        0     1160 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/config.yaml
+-rw-r--r--   0        0        0     5429 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data.py
+-rw-r--r--   0        0        0     9295 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_arrhythmia.py
+-rw-r--r--   0        0        0    23957 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_beat.py
+-rw-r--r--   0        0        0     9605 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/data_rpeak.py
+-rw-r--r--   0        0        0       39 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/pqrst.py
+-rw-r--r--   0        0        0     2827 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/report.py
+-rw-r--r--   0        0        0     5887 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/extra/utils.py
+-rw-r--r--   0        0        0     6150 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/features.py
+-rw-r--r--   0        0        0     2579 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/io.py
+-rw-r--r--   0        0        0     5773 2023-05-29 11:04:46.315576 pyheartlib-0.0.8/src/pyheartlib/processing.py
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyheartlib-0.0.8/PKG-INFO
```

### Comparing `pyheartlib-0.0.7/README.md` & `pyheartlib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/pyproject.toml` & `pyheartlib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyheartlib"
-version = "0.0.7"
+version = "0.0.8"
 description = "A Python package for processing and modeling electrocardiogram signals"
 authors = ["Sadegh Mohammadi"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `pyheartlib-0.0.7/src/pyheartlib/beat_info.py` & `pyheartlib-0.0.8/src/pyheartlib/beat_info.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/config.yaml` & `pyheartlib-0.0.8/src/pyheartlib/config.yaml`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/data.py` & `pyheartlib-0.0.8/src/pyheartlib/data.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/data_arrhythmia.py` & `pyheartlib-0.0.8/src/pyheartlib/data_arrhythmia.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/data_beat.py` & `pyheartlib-0.0.8/src/pyheartlib/data_beat.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/data_rpeak.py` & `pyheartlib-0.0.8/src/pyheartlib/data_rpeak.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/extra/pqrst.py` & `pyheartlib-0.0.8/src/pyheartlib/extra/pqrst.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/extra/report.py` & `pyheartlib-0.0.8/src/pyheartlib/extra/report.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/extra/utils.py` & `pyheartlib-0.0.8/src/pyheartlib/extra/utils.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/features.py` & `pyheartlib-0.0.8/src/pyheartlib/features.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/io.py` & `pyheartlib-0.0.8/src/pyheartlib/io.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/src/pyheartlib/processing.py` & `pyheartlib-0.0.8/src/pyheartlib/processing.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.7/PKG-INFO` & `pyheartlib-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyheartlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python package for processing and modeling electrocardiogram signals
 License: Proprietary
 Author: Sadegh Mohammadi
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


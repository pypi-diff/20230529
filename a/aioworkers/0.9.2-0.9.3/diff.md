# Comparing `tmp/aioworkers-0.9.2.tar.gz` & `tmp/aioworkers-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioworkers-0.9.2.tar", last modified: Sun Dec 17 20:05:33 2017, max compression
+gzip compressed data, was "dist/aioworkers-0.9.3.tar", last modified: Fri Dec 22 15:11:53 2017, max compression
```

## Comparing `aioworkers-0.9.2.tar` & `aioworkers-0.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1321 2017-11-17 06:47:00.000000 aioworkers-0.9.2/setup.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       38 2017-12-17 20:05:33.000000 aioworkers-0.9.2/setup.cfg
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers.egg-info/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1035 2017-12-17 20:05:32.000000 aioworkers-0.9.2/aioworkers.egg-info/SOURCES.txt
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        1 2017-12-17 20:05:32.000000 aioworkers-0.9.2/aioworkers.egg-info/dependency_links.txt
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       11 2017-12-17 20:05:32.000000 aioworkers-0.9.2/aioworkers.egg-info/top_level.txt
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     8663 2017-12-17 20:05:32.000000 aioworkers-0.9.2/aioworkers.egg-info/PKG-INFO
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       62 2017-12-17 20:05:32.000000 aioworkers-0.9.2/aioworkers.egg-info/entry_points.txt
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1426 2017-11-19 23:45:22.000000 aioworkers-0.9.2/aioworkers/app.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5129 2017-11-03 23:09:09.000000 aioworkers-0.9.2/aioworkers/redis.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     4094 2017-11-19 23:45:22.000000 aioworkers-0.9.2/aioworkers/cli.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     3285 2017-11-03 23:09:08.000000 aioworkers-0.9.2/aioworkers/amqp.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       71 2017-06-25 12:58:57.000000 aioworkers-0.9.2/aioworkers/__main__.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      659 2017-11-19 23:45:22.000000 aioworkers-0.9.2/aioworkers/http.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      345 2017-06-25 13:31:37.000000 aioworkers-0.9.2/aioworkers/config.py
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers/core/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1052 2017-10-11 22:49:54.000000 aioworkers-0.9.2/aioworkers/core/interact.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     3635 2017-11-03 23:09:08.000000 aioworkers-0.9.2/aioworkers/core/formatter.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1850 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/core/base.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)    10634 2017-12-11 11:53:12.000000 aioworkers-0.9.2/aioworkers/core/config.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-13 00:24:49.000000 aioworkers-0.9.2/aioworkers/core/__init__.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     9235 2017-12-17 19:29:26.000000 aioworkers-0.9.2/aioworkers/core/context.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2104 2017-11-19 23:45:22.000000 aioworkers-0.9.2/aioworkers/core/plugin.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2293 2017-10-23 09:46:35.000000 aioworkers-0.9.2/aioworkers/core/command.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       22 2017-12-17 20:04:06.000000 aioworkers-0.9.2/aioworkers/__init__.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1954 2017-12-17 19:40:19.000000 aioworkers-0.9.2/aioworkers/utils.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2087 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/humanize.py
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers/queue/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      498 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/queue/csv.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1781 2017-11-19 23:45:22.000000 aioworkers-0.9.2/aioworkers/queue/base.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-13 00:24:50.000000 aioworkers-0.9.2/aioworkers/queue/__init__.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2746 2017-03-10 21:22:20.000000 aioworkers-0.9.2/aioworkers/queue/timeout.py
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers/storage/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)    10676 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/storage/filesystem.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5751 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/storage/http.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2431 2017-09-23 23:04:17.000000 aioworkers-0.9.2/aioworkers/storage/meta.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2061 2017-04-29 10:44:08.000000 aioworkers-0.9.2/aioworkers/storage/base.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       41 2017-02-18 21:13:25.000000 aioworkers-0.9.2/aioworkers/storage/__init__.py
-drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-17 20:05:33.000000 aioworkers-0.9.2/aioworkers/worker/
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2189 2017-09-23 23:04:17.000000 aioworkers-0.9.2/aioworkers/worker/updater.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2966 2017-04-12 08:26:40.000000 aioworkers-0.9.2/aioworkers/worker/subprocess.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5160 2017-11-17 06:47:00.000000 aioworkers-0.9.2/aioworkers/worker/base.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1810 2017-10-23 09:46:35.000000 aioworkers-0.9.2/aioworkers/worker/supervisor.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-25 23:11:20.000000 aioworkers-0.9.2/aioworkers/worker/__init__.py
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1612 2017-03-19 20:18:04.000000 aioworkers-0.9.2/README.rst
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     8663 2017-12-17 20:05:33.000000 aioworkers-0.9.2/PKG-INFO
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      101 2016-11-13 00:24:50.000000 aioworkers-0.9.2/MANIFEST.in
--rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     4391 2017-12-17 20:04:06.000000 aioworkers-0.9.2/HISTORY.rst
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1321 2017-11-17 06:47:00.000000 aioworkers-0.9.3/setup.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       38 2017-12-22 15:11:53.000000 aioworkers-0.9.3/setup.cfg
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers.egg-info/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1035 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers.egg-info/SOURCES.txt
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        1 2017-12-22 15:11:52.000000 aioworkers-0.9.3/aioworkers.egg-info/dependency_links.txt
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       11 2017-12-22 15:11:52.000000 aioworkers-0.9.3/aioworkers.egg-info/top_level.txt
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     8787 2017-12-22 15:11:52.000000 aioworkers-0.9.3/aioworkers.egg-info/PKG-INFO
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       62 2017-12-22 15:11:52.000000 aioworkers-0.9.3/aioworkers.egg-info/entry_points.txt
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1426 2017-11-19 23:45:22.000000 aioworkers-0.9.3/aioworkers/app.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5129 2017-12-19 08:53:54.000000 aioworkers-0.9.3/aioworkers/redis.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     4094 2017-11-19 23:45:22.000000 aioworkers-0.9.3/aioworkers/cli.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     3285 2017-11-03 23:09:08.000000 aioworkers-0.9.3/aioworkers/amqp.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       71 2017-06-25 12:58:57.000000 aioworkers-0.9.3/aioworkers/__main__.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      659 2017-11-19 23:45:22.000000 aioworkers-0.9.3/aioworkers/http.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      345 2017-06-25 13:31:37.000000 aioworkers-0.9.3/aioworkers/config.py
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers/core/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1052 2017-10-11 22:49:54.000000 aioworkers-0.9.3/aioworkers/core/interact.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     3635 2017-11-03 23:09:08.000000 aioworkers-0.9.3/aioworkers/core/formatter.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1850 2017-11-17 06:47:00.000000 aioworkers-0.9.3/aioworkers/core/base.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)    10634 2017-12-11 11:53:12.000000 aioworkers-0.9.3/aioworkers/core/config.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-13 00:24:49.000000 aioworkers-0.9.3/aioworkers/core/__init__.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     9235 2017-12-17 19:29:26.000000 aioworkers-0.9.3/aioworkers/core/context.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2104 2017-11-19 23:45:22.000000 aioworkers-0.9.3/aioworkers/core/plugin.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2293 2017-10-23 09:46:35.000000 aioworkers-0.9.3/aioworkers/core/command.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       22 2017-12-22 14:58:20.000000 aioworkers-0.9.3/aioworkers/__init__.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2029 2017-12-19 18:59:16.000000 aioworkers-0.9.3/aioworkers/utils.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2087 2017-11-17 06:47:00.000000 aioworkers-0.9.3/aioworkers/humanize.py
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers/queue/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      498 2017-11-17 06:47:00.000000 aioworkers-0.9.3/aioworkers/queue/csv.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1781 2017-11-19 23:45:22.000000 aioworkers-0.9.3/aioworkers/queue/base.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-13 00:24:50.000000 aioworkers-0.9.3/aioworkers/queue/__init__.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2746 2017-03-10 21:22:20.000000 aioworkers-0.9.3/aioworkers/queue/timeout.py
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers/storage/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)    10894 2017-12-22 14:54:22.000000 aioworkers-0.9.3/aioworkers/storage/filesystem.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5751 2017-11-17 06:47:00.000000 aioworkers-0.9.3/aioworkers/storage/http.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2431 2017-09-23 23:04:17.000000 aioworkers-0.9.3/aioworkers/storage/meta.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2061 2017-04-29 10:44:08.000000 aioworkers-0.9.3/aioworkers/storage/base.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)       41 2017-02-18 21:13:25.000000 aioworkers-0.9.3/aioworkers/storage/__init__.py
+drwxrwxr-x   0 yttrium   (1000) yttrium   (1000)        0 2017-12-22 15:11:53.000000 aioworkers-0.9.3/aioworkers/worker/
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2189 2017-09-23 23:04:17.000000 aioworkers-0.9.3/aioworkers/worker/updater.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     2966 2017-04-12 08:26:40.000000 aioworkers-0.9.3/aioworkers/worker/subprocess.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     5160 2017-11-17 06:47:00.000000 aioworkers-0.9.3/aioworkers/worker/base.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1810 2017-10-23 09:46:35.000000 aioworkers-0.9.3/aioworkers/worker/supervisor.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)        0 2016-11-25 23:11:20.000000 aioworkers-0.9.3/aioworkers/worker/__init__.py
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     1612 2017-03-19 20:18:04.000000 aioworkers-0.9.3/README.rst
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     8787 2017-12-22 15:11:53.000000 aioworkers-0.9.3/PKG-INFO
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)      101 2016-11-13 00:24:50.000000 aioworkers-0.9.3/MANIFEST.in
+-rw-rw-r--   0 yttrium   (1000) yttrium   (1000)     4493 2017-12-22 14:58:04.000000 aioworkers-0.9.3/HISTORY.rst
```

### Comparing `aioworkers-0.9.2/setup.py` & `aioworkers-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers.egg-info/SOURCES.txt` & `aioworkers-0.9.3/aioworkers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers.egg-info/PKG-INFO` & `aioworkers-0.9.3/aioworkers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: aioworkers
-Version: 0.9.2
+Version: 0.9.3
 Summary: Easy configurable workers based on asyncio
 Home-page: https://github.com/aioworkers/aioworkers
 Author: Alexander Malev
 Author-email: yttrium@somedev.ru
 License: Apache Software License 2.0
-Description-Content-Type: UNKNOWN
 Description: aioworkers
         ==========
         
         
         .. image:: https://img.shields.io/pypi/v/aioworkers.svg
           :target: https://pypi.python.org/pypi/aioworkers
         
@@ -56,14 +55,21 @@
         * Configuration subsystem
         
         
         =======
         History
         =======
         
+        0.9.3 (2017-12-22)
+        ------------------
+        
+        * Fix FileSystemStorage.get_free_space
+        * Improve import_name
+        
+        
         0.9.2 (2017-12-17)
         ------------------
         
         * Fix access to nested element
         * Improve import_name
```

### Comparing `aioworkers-0.9.2/aioworkers/app.py` & `aioworkers-0.9.3/aioworkers/app.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/redis.py` & `aioworkers-0.9.3/aioworkers/redis.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/cli.py` & `aioworkers-0.9.3/aioworkers/cli.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/amqp.py` & `aioworkers-0.9.3/aioworkers/amqp.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/http.py` & `aioworkers-0.9.3/aioworkers/http.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/interact.py` & `aioworkers-0.9.3/aioworkers/core/interact.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/formatter.py` & `aioworkers-0.9.3/aioworkers/core/formatter.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/base.py` & `aioworkers-0.9.3/aioworkers/core/base.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/config.py` & `aioworkers-0.9.3/aioworkers/core/config.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/context.py` & `aioworkers-0.9.3/aioworkers/core/context.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/plugin.py` & `aioworkers-0.9.3/aioworkers/core/plugin.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/core/command.py` & `aioworkers-0.9.3/aioworkers/core/command.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/utils.py` & `aioworkers-0.9.3/aioworkers/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,47 +4,52 @@
 import logging
 import sys
 from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
 
+@functools.lru_cache(None)
 def import_name(stref: str):
     """
     >>> import_name('datetime.datetime.utcnow') is not None
     True
     >>> import_name('aioworkers.utils.import_name') is not None
     True
     """
     h = stref
     p = []
-    while True:
-        try:
-            r = importlib.util.find_spec(h)
-        except (AttributeError, ImportError):
-            r = None
+    m = None
+    try:
+        r = importlib.util.find_spec(stref)
+    except (AttributeError, ImportError):
+        r = None
 
-        if r is not None:
-            break
-        elif '.' not in h:
-            raise ImportError(stref)
+    if r is not None:
+        return importlib.import_module(stref)
 
+    while '.' in h:
         h, t = h.rsplit('.', 1)
         p.append(t)
+        if h in sys.modules:
+            m = sys.modules[h]
+            break
 
-    h = importlib.import_module(h)
+    if m is None:
+        m = importlib.import_module(h)
 
     for i in reversed(p):
-        if not hasattr(h, i):
-            raise ImportError(
-                '{}: Not found {} in {}'.format(stref, i, h))
-        h = getattr(h, i, None)
+        if hasattr(m, i):
+            m = getattr(m, i)
+        else:
+            h += '.' + i
+            m = importlib.import_module(h)
 
     logger.debug('Imported "{}" as {}'.format(stref, h))
-    return h
+    return m
 
 
 def module_path(str_module, return_str=False):
     if str_module in sys.modules:
         m = sys.modules[str_module]
     else:
         m = import_name(str_module)
```

### Comparing `aioworkers-0.9.2/aioworkers/humanize.py` & `aioworkers-0.9.3/aioworkers/humanize.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/queue/base.py` & `aioworkers-0.9.3/aioworkers/queue/base.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/queue/timeout.py` & `aioworkers-0.9.3/aioworkers/queue/timeout.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/storage/filesystem.py` & `aioworkers-0.9.3/aioworkers/storage/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,16 +204,23 @@
 
     def run_in_executor(self, f, *args, **kwargs):
         if kwargs:
             f = partial(f, **kwargs)
         return self.loop.run_in_executor(self._executor, f, *args)
 
     def disk_usage(self):
+        def disk_usage(path):
+            try:
+                return shutil.disk_usage(path)
+            except FileNotFoundError:
+                os.makedirs(path, exist_ok=True)
+            return shutil.disk_usage(path)
+
         return self.loop.run_in_executor(
-            self._executor, shutil.disk_usage, self._config.path)
+            self._executor, disk_usage, self._config.path)
 
     async def get_free_space(self):
         du = await self.disk_usage()
         return du.free
 
     async def wait_free_space(self, size=None):
         if not self._limit:
```

### Comparing `aioworkers-0.9.2/aioworkers/storage/http.py` & `aioworkers-0.9.3/aioworkers/storage/http.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/storage/meta.py` & `aioworkers-0.9.3/aioworkers/storage/meta.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/storage/base.py` & `aioworkers-0.9.3/aioworkers/storage/base.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/worker/updater.py` & `aioworkers-0.9.3/aioworkers/worker/updater.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/worker/subprocess.py` & `aioworkers-0.9.3/aioworkers/worker/subprocess.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/worker/base.py` & `aioworkers-0.9.3/aioworkers/worker/base.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/aioworkers/worker/supervisor.py` & `aioworkers-0.9.3/aioworkers/worker/supervisor.py`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/README.rst` & `aioworkers-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `aioworkers-0.9.2/PKG-INFO` & `aioworkers-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: aioworkers
-Version: 0.9.2
+Version: 0.9.3
 Summary: Easy configurable workers based on asyncio
 Home-page: https://github.com/aioworkers/aioworkers
 Author: Alexander Malev
 Author-email: yttrium@somedev.ru
 License: Apache Software License 2.0
-Description-Content-Type: UNKNOWN
 Description: aioworkers
         ==========
         
         
         .. image:: https://img.shields.io/pypi/v/aioworkers.svg
           :target: https://pypi.python.org/pypi/aioworkers
         
@@ -56,14 +55,21 @@
         * Configuration subsystem
         
         
         =======
         History
         =======
         
+        0.9.3 (2017-12-22)
+        ------------------
+        
+        * Fix FileSystemStorage.get_free_space
+        * Improve import_name
+        
+        
         0.9.2 (2017-12-17)
         ------------------
         
         * Fix access to nested element
         * Improve import_name
```

### Comparing `aioworkers-0.9.2/HISTORY.rst` & `aioworkers-0.9.3/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+0.9.3 (2017-12-22)
+------------------
+
+* Fix FileSystemStorage.get_free_space
+* Improve import_name
+
+
 0.9.2 (2017-12-17)
 ------------------
 
 * Fix access to nested element
 * Improve import_name
```


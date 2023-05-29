# Comparing `tmp/opencan-cand-0.1.0.tar.gz` & `tmp/opencan-cand-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencan-cand-0.1.0.tar", last modified: Sat Feb  4 15:45:08 2023, max compression
+gzip compressed data, was "opencan-cand-0.1.1.tar", last modified: Mon May 29 16:16:54 2023, max compression
```

## Comparing `opencan-cand-0.1.0.tar` & `opencan-cand-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-02-04 15:45:08.855743 opencan-cand-0.1.0/
--rw-r--r--   0 dmezh      (501) staff       (20)    16725 2022-11-07 05:40:35.000000 opencan-cand-0.1.0/LICENSE
--rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-02-04 15:45:08.855623 opencan-cand-0.1.0/PKG-INFO
--rw-r--r--   0 dmezh      (501) staff       (20)     1216 2022-09-20 08:07:41.000000 opencan-cand-0.1.0/README.md
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-02-04 15:45:08.854787 opencan-cand-0.1.0/cand/
--rw-r--r--   0 dmezh      (501) staff       (20)      133 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/__init__.py
--rwxr-xr-x   0 dmezh      (501) staff       (20)     3482 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/cand
--rw-r--r--   0 dmezh      (501) staff       (20)     1760 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/client.py
--rw-r--r--   0 dmezh      (501) staff       (20)      209 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/config.py
--rw-r--r--   0 dmezh      (501) staff       (20)     1889 2023-02-04 01:12:19.000000 opencan-cand-0.1.0/cand/listener.py
--rw-r--r--   0 dmezh      (501) staff       (20)      751 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/serialization.py
--rw-r--r--   0 dmezh      (501) staff       (20)     2414 2023-02-04 01:12:23.000000 opencan-cand-0.1.0/cand/talker.py
--rw-r--r--   0 dmezh      (501) staff       (20)      387 2022-09-20 08:16:39.000000 opencan-cand-0.1.0/cand/util.py
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-02-04 15:45:08.855365 opencan-cand-0.1.0/opencan_cand.egg-info/
--rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-02-04 15:45:08.000000 opencan-cand-0.1.0/opencan_cand.egg-info/PKG-INFO
--rw-r--r--   0 dmezh      (501) staff       (20)      367 2023-02-04 15:45:08.000000 opencan-cand-0.1.0/opencan_cand.egg-info/SOURCES.txt
--rw-r--r--   0 dmezh      (501) staff       (20)        1 2023-02-04 15:45:08.000000 opencan-cand-0.1.0/opencan_cand.egg-info/dependency_links.txt
--rw-r--r--   0 dmezh      (501) staff       (20)       83 2023-02-04 15:45:08.000000 opencan-cand-0.1.0/opencan_cand.egg-info/requires.txt
--rw-r--r--   0 dmezh      (501) staff       (20)        5 2023-02-04 15:45:08.000000 opencan-cand-0.1.0/opencan_cand.egg-info/top_level.txt
--rw-r--r--   0 dmezh      (501) staff       (20)      611 2023-02-04 15:42:27.000000 opencan-cand-0.1.0/pyproject.toml
--rw-r--r--   0 dmezh      (501) staff       (20)       38 2023-02-04 15:45:08.855787 opencan-cand-0.1.0/setup.cfg
--rwxr-xr-x   0 dmezh      (501) staff       (20)      107 2022-09-20 18:17:54.000000 opencan-cand-0.1.0/setup.py
-drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-02-04 15:45:08.855476 opencan-cand-0.1.0/test/
--rw-r--r--   0 dmezh      (501) staff       (20)      533 2022-09-20 08:10:52.000000 opencan-cand-0.1.0/test/test_send_rate.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473917 opencan-cand-0.1.1/
+-rw-r--r--   0 dmezh      (501) staff       (20)    16725 2022-11-07 05:40:35.000000 opencan-cand-0.1.1/LICENSE
+-rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-05-29 16:16:54.473801 opencan-cand-0.1.1/PKG-INFO
+-rw-r--r--   0 dmezh      (501) staff       (20)     1216 2022-09-20 08:07:41.000000 opencan-cand-0.1.1/README.md
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.472912 opencan-cand-0.1.1/cand/
+-rw-r--r--   0 dmezh      (501) staff       (20)      133 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/__init__.py
+-rwxr-xr-x   0 dmezh      (501) staff       (20)     3482 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/cand
+-rw-r--r--   0 dmezh      (501) staff       (20)     1760 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/client.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      209 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/config.py
+-rw-r--r--   0 dmezh      (501) staff       (20)     1889 2023-02-04 01:12:19.000000 opencan-cand-0.1.1/cand/listener.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      751 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/serialization.py
+-rw-r--r--   0 dmezh      (501) staff       (20)     2403 2023-05-29 16:15:35.000000 opencan-cand-0.1.1/cand/talker.py
+-rw-r--r--   0 dmezh      (501) staff       (20)      387 2022-09-20 08:16:39.000000 opencan-cand-0.1.1/cand/util.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473438 opencan-cand-0.1.1/opencan_cand.egg-info/
+-rw-r--r--   0 dmezh      (501) staff       (20)     1585 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/PKG-INFO
+-rw-r--r--   0 dmezh      (501) staff       (20)      367 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)        1 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)       83 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/requires.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)        5 2023-05-29 16:16:54.000000 opencan-cand-0.1.1/opencan_cand.egg-info/top_level.txt
+-rw-r--r--   0 dmezh      (501) staff       (20)      611 2023-05-29 16:15:35.000000 opencan-cand-0.1.1/pyproject.toml
+-rw-r--r--   0 dmezh      (501) staff       (20)       38 2023-05-29 16:16:54.473949 opencan-cand-0.1.1/setup.cfg
+-rwxr-xr-x   0 dmezh      (501) staff       (20)      107 2022-09-20 18:17:54.000000 opencan-cand-0.1.1/setup.py
+drwxr-xr-x   0 dmezh      (501) staff       (20)        0 2023-05-29 16:16:54.473533 opencan-cand-0.1.1/test/
+-rw-r--r--   0 dmezh      (501) staff       (20)      533 2022-09-20 08:10:52.000000 opencan-cand-0.1.1/test/test_send_rate.py
```

### Comparing `opencan-cand-0.1.0/LICENSE` & `opencan-cand-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/PKG-INFO` & `opencan-cand-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencan-cand
-Version: 0.1.0
+Version: 0.1.1
 Summary: A fast and super useful daemon for decoding and encoding CAN messages.
 Author-email: OpenCAN <info@opencan.org>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/opencan/cand
 Keywords: cand,can,canbus,can bus
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opencan-cand-0.1.0/README.md` & `opencan-cand-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/cand/cand` & `opencan-cand-0.1.1/cand/cand`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/cand/client.py` & `opencan-cand-0.1.1/cand/client.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/cand/listener.py` & `opencan-cand-0.1.1/cand/listener.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/cand/serialization.py` & `opencan-cand-0.1.1/cand/serialization.py`

 * *Files identical despite different names*

### Comparing `opencan-cand-0.1.0/cand/talker.py` & `opencan-cand-0.1.1/cand/talker.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,23 @@
             p.execute()
             time_at_flush = time()
 
         elif len(p) > 0 and time() - time_at_flush > MAX_BUFFER_WAIT_TIME_SECONDS:
             p.execute()
             time_at_flush = time()
 
-        _, serial_msgs = cfg.rdb.blmpop(
+        if _ := cfg.rdb.blmpop(
             QUEUE_POP_TIMEOUT,
             1,
             "queue:cansend",
             direction="LEFT",
-            count=MAX_BUFFER_SIZE + 1,
-        ) or None, None
-
-        if serial_msgs is None:
+            count=MAX_BUFFER_SIZE + 1
+        ):
+            serial_msgs = _[1]
+        else:
             continue
 
         if len(serial_msgs) > MAX_BUFFER_SIZE:
             if time() - time_at_last_buffer_warning > 1:
                 log.critical(
                     f"Buffer is saturated ({len(serial_msgs)})! cand may not be keeping up with sent messsages."
                     + f" (suppressed {buffer_warning_suppress_count} times)"
```

### Comparing `opencan-cand-0.1.0/opencan_cand.egg-info/PKG-INFO` & `opencan-cand-0.1.1/opencan_cand.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencan-cand
-Version: 0.1.0
+Version: 0.1.1
 Summary: A fast and super useful daemon for decoding and encoding CAN messages.
 Author-email: OpenCAN <info@opencan.org>
 License: MPL-2.0
 Project-URL: Homepage, https://github.com/opencan/cand
 Keywords: cand,can,canbus,can bus
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opencan-cand-0.1.0/pyproject.toml` & `opencan-cand-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "opencan-cand"
-version = "0.1.0"
+version = "0.1.1"
 description = "A fast and super useful daemon for decoding and encoding CAN messages."
 authors = [
     {name = "OpenCAN", email = "info@opencan.org"},
 ]
 
 readme = "README.md"
 requires-python = ">=3.9"
@@ -16,12 +16,12 @@
 license = {text = "MPL-2.0"}
 
 dependencies = [
     "cantools>=37.0.7",
     "coloredlogs>=15.0.1",
     "msgpack>=1.0.3",
     "python-can>=3.3.4",
-    "redis>=4.3.2",
+    "redis>=4.5.5",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/opencan/cand"
```

### Comparing `opencan-cand-0.1.0/test/test_send_rate.py` & `opencan-cand-0.1.1/test/test_send_rate.py`

 * *Files identical despite different names*


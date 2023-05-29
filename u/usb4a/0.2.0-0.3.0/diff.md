# Comparing `tmp/usb4a-0.2.0.tar.gz` & `tmp/usb4a-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\usb4a-0.2.0.tar", last modified: Sun Nov  8 22:49:24 2020, max compression
+gzip compressed data, was "usb4a-0.3.0.tar", last modified: Mon May 29 00:50:36 2023, max compression
```

## Comparing `usb4a-0.2.0.tar` & `usb4a-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2020-11-08 22:49:24.000000 usb4a-0.2.0/
--rw-rw-rw-   0        0        0      615 2020-11-08 22:49:24.000000 usb4a-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2827 2020-11-08 22:42:31.000000 usb4a-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2020-11-08 22:49:24.000000 usb4a-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      730 2020-11-08 22:42:31.000000 usb4a-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-11-08 22:49:24.000000 usb4a-0.2.0/usb4a/
--rw-rw-rw-   0        0        0      220 2020-11-08 22:42:31.000000 usb4a-0.2.0/usb4a/__init__.py
--rw-rw-rw-   0        0        0     4378 2020-11-08 22:42:31.000000 usb4a-0.2.0/usb4a/usb.py
-drwxrwxrwx   0        0        0        0 2020-11-08 22:49:24.000000 usb4a-0.2.0/usb4a.egg-info/
--rw-rw-rw-   0        0        0      615 2020-11-08 22:49:22.000000 usb4a-0.2.0/usb4a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2020-11-08 22:49:22.000000 usb4a-0.2.0/usb4a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-08 22:49:22.000000 usb4a-0.2.0/usb4a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2020-11-08 22:49:22.000000 usb4a-0.2.0/usb4a.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 00:50:36.278033 usb4a-0.3.0/
+-rw-rw-rw-   0        0        0      585 2023-05-29 00:50:36.253323 usb4a-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-29 00:50:36.278988 usb4a-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-05-28 23:56:43.000000 usb4a-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:50:36.222318 usb4a-0.3.0/usb4a/
+-rw-rw-rw-   0        0        0      220 2023-05-28 23:57:14.000000 usb4a-0.3.0/usb4a/__init__.py
+-rw-rw-rw-   0        0        0     4541 2023-05-29 00:05:55.000000 usb4a-0.3.0/usb4a/usb.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:50:36.248364 usb4a-0.3.0/usb4a.egg-info/
+-rw-rw-rw-   0        0        0      585 2023-05-29 00:50:36.000000 usb4a-0.3.0/usb4a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-05-29 00:50:36.000000 usb4a-0.3.0/usb4a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:50:36.000000 usb4a-0.3.0/usb4a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 00:50:36.000000 usb4a-0.3.0/usb4a.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `usb4a-0.2.0/PKG-INFO` & `usb4a-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: usb4a
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package for Android USB host.
 Home-page: https://github.com/jacklinquan/usb4a
 Author: Quan Lin
 Author-email: jacklinquan@gmail.com
 License: MIT
-Description: https://github.com/jacklinquan/usb4a
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Android
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+https://github.com/jacklinquan/usb4a
```

### Comparing `usb4a-0.2.0/setup.py` & `usb4a-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="usb4a",
-    version="0.2.0",
+    version="0.3.0",
     description="Python package for Android USB host.",
     long_description="https://github.com/jacklinquan/usb4a",
     long_description_content_type="text/markdown",
     url="https://github.com/jacklinquan/usb4a",
     author="Quan Lin",
     author_email="jacklinquan@gmail.com",
     license="MIT",
```

### Comparing `usb4a-0.2.0/usb4a/usb.py` & `usb4a-0.3.0/usb4a/usb.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,20 @@
     
     Parameters:
         usb_device (object): the USB device object. 
     '''
     usb_manager = get_usb_manager()
     ACTION_USB_PERMISSION = "com.access.device.USB_PERMISSION"
     intent = Intent(ACTION_USB_PERMISSION)
-    pintent = PendingIntent.getBroadcast(get_context(), 0, intent, 0)
+    try:
+        pintent = PendingIntent.getBroadcast(get_context(), 0, intent, 0)
+    except Exception:
+        pintent = PendingIntent.getBroadcast(
+            get_context(), 0, intent, PendingIntent.FLAG_IMMUTABLE
+        )
     usb_manager.requestPermission(usb_device, pintent)
     
 def build_usb_control_request_type(direction, usb_type, recipient):
     '''Build USB control request type for USB communication.
     
     Parameters:
         direction (int):
```

### Comparing `usb4a-0.2.0/usb4a.egg-info/PKG-INFO` & `usb4a-0.3.0/usb4a.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: usb4a
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python package for Android USB host.
 Home-page: https://github.com/jacklinquan/usb4a
 Author: Quan Lin
 Author-email: jacklinquan@gmail.com
 License: MIT
-Description: https://github.com/jacklinquan/usb4a
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Android
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+https://github.com/jacklinquan/usb4a
```


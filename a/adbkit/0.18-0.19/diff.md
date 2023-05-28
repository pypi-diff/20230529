# Comparing `tmp/adbkit-0.18.tar.gz` & `tmp/adbkit-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.18.tar", last modified: Sun May 28 07:49:29 2023, max compression
+gzip compressed data, was "adbkit-0.19.tar", last modified: Sun May 28 22:11:18 2023, max compression
```

## Comparing `adbkit-0.18.tar` & `adbkit-0.19.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.310506 adbkit-0.18/
--rw-rw-rw-   0        0        0     1148 2023-05-28 07:48:50.000000 adbkit-0.18/LICENSE.rst
--rw-rw-rw-   0        0        0       89 2023-05-28 07:48:49.000000 adbkit-0.18/MANIFEST.in
--rw-rw-rw-   0        0        0   161921 2023-05-28 07:49:29.311455 adbkit-0.18/PKG-INFO
--rw-rw-rw-   0        0        0   160268 2023-05-28 07:38:39.000000 adbkit-0.18/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.306602 adbkit-0.18/adbkit/
--rw-rw-rw-   0        0        0   160268 2023-05-28 07:38:39.000000 adbkit-0.18/adbkit/README.MD
--rw-rw-rw-   0        0        0   129534 2023-05-28 07:33:33.000000 adbkit-0.18/adbkit/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-28 07:49:28.000000 adbkit-0.18/adbkit/requirements.txt
--rw-rw-rw-   0        0        0   340479 2023-05-28 07:49:28.000000 adbkit-0.18/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.309502 adbkit-0.18/adbkit.egg-info/
--rw-rw-rw-   0        0        0   161921 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      651 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-28 07:49:29.312430 adbkit-0.18/setup.cfg
--rw-rw-rw-   0        0        0     2785 2023-05-28 07:49:28.000000 adbkit-0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.939002 adbkit-0.19/
+-rw-rw-rw-   0        0        0     1148 2023-05-28 22:10:52.000000 adbkit-0.19/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-05-28 22:10:51.000000 adbkit-0.19/MANIFEST.in
+-rw-rw-rw-   0        0        0   161921 2023-05-28 22:11:18.939999 adbkit-0.19/PKG-INFO
+-rw-rw-rw-   0        0        0   160268 2023-05-28 07:54:48.000000 adbkit-0.19/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.935038 adbkit-0.19/adbkit/
+-rw-rw-rw-   0        0        0   160268 2023-05-28 07:54:48.000000 adbkit-0.19/adbkit/README.MD
+-rw-rw-rw-   0        0        0   129748 2023-05-28 22:08:30.000000 adbkit-0.19/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   340479 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.939002 adbkit-0.19/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   161921 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      651 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-28 22:11:18.940997 adbkit-0.19/setup.cfg
+-rw-rw-rw-   0        0        0     2785 2023-05-28 22:11:18.000000 adbkit-0.19/setup.py
```

### Comparing `adbkit-0.18/LICENSE.rst` & `adbkit-0.19/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/PKG-INFO` & `adbkit-0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.18
+Version: 0.19
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.18/README.md` & `adbkit-0.19/README.md`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/adbkit/README.MD` & `adbkit-0.19/adbkit/README.MD`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/adbkit/__init__.py` & `adbkit-0.19/adbkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2482,47 +2482,50 @@
         else:
             print(f"Use {killkeys} to turn imshow on/off")
             self._start_show_screenshot(str(self.deviceserial), killkeys, sleeptime)
 
     def aa_activate_scrcpy_screenshots_usb(
         self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
     ):
+        screenwidth, screenheight = get_screen_height_width(self.adb_path, self.deviceserial)
         self.scrcpy_screenshot_usb = AdbShotUSB(
             device_serial=self.deviceserial,
             adb_path=self.adb_path,
             adb_host_address=adb_host_address,
             adb_host_port=adb_host_port,
             sleep_after_exception=0.05,
             frame_buffer=4,
             lock_video_orientation=lock_video_orientation,
             max_frame_rate=0,
             byte_package_size=131072,
             scrcpy_server_version="2.0",
             log_level="info",
-            max_video_width=0,
+            max_video_width=screenheight,
             start_server=False,
             connect_to_device=False,
         )
 
     def aa_activate_scrcpy_screenshots_tcp(
         self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
     ):
+        screenwidth, screenheight = get_screen_height_width(self.adb_path, self.deviceserial)
+
         self.scrcpy_screenshot_tcp = AdbShotTCP(
             device_serial=self.deviceserial,
             adb_path=self.adb_path,
             ip=adb_host_address,
             port=adb_host_port,
             sleep_after_exception=0.05,
             frame_buffer=4,
             lock_video_orientation=lock_video_orientation,
             max_frame_rate=0,
             byte_package_size=131072,
             scrcpy_server_version="2.0",
             log_level="info",
-            max_video_width=0,
+            max_video_width=screenheight,
             start_server=False,
             connect_to_device=False,
         )
 
     @staticmethod
     def connect_to_all_bluestacks_hyperv_devices(
         adb_path,
```

### Comparing `adbkit-0.18/adbkit/requirements.txt` & `adbkit-0.19/adbkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/adbkit/thirdparty.json` & `adbkit-0.19/adbkit/thirdparty.json`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/adbkit.egg-info/PKG-INFO` & `adbkit-0.19/adbkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.18
+Version: 0.19
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.18/adbkit.egg-info/requires.txt` & `adbkit-0.19/adbkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.18/setup.py` & `adbkit-0.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.18'''
+VERSION = '''0.19'''
 DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
```


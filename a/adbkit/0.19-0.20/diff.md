# Comparing `tmp/adbkit-0.19.tar.gz` & `tmp/adbkit-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.19.tar", last modified: Sun May 28 22:11:18 2023, max compression
+gzip compressed data, was "adbkit-0.20.tar", last modified: Mon May 29 01:30:11 2023, max compression
```

## Comparing `adbkit-0.19.tar` & `adbkit-0.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.939002 adbkit-0.19/
--rw-rw-rw-   0        0        0     1148 2023-05-28 22:10:52.000000 adbkit-0.19/LICENSE.rst
--rw-rw-rw-   0        0        0       89 2023-05-28 22:10:51.000000 adbkit-0.19/MANIFEST.in
--rw-rw-rw-   0        0        0   161921 2023-05-28 22:11:18.939999 adbkit-0.19/PKG-INFO
--rw-rw-rw-   0        0        0   160268 2023-05-28 07:54:48.000000 adbkit-0.19/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.935038 adbkit-0.19/adbkit/
--rw-rw-rw-   0        0        0   160268 2023-05-28 07:54:48.000000 adbkit-0.19/adbkit/README.MD
--rw-rw-rw-   0        0        0   129748 2023-05-28 22:08:30.000000 adbkit-0.19/adbkit/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit/requirements.txt
--rw-rw-rw-   0        0        0   340479 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-28 22:11:18.939002 adbkit-0.19/adbkit.egg-info/
--rw-rw-rw-   0        0        0   161921 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      651 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 22:11:18.000000 adbkit-0.19/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-28 22:11:18.940997 adbkit-0.19/setup.cfg
--rw-rw-rw-   0        0        0     2785 2023-05-28 22:11:18.000000 adbkit-0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:30:11.248019 adbkit-0.20/
+-rw-rw-rw-   0        0        0     1148 2023-05-29 01:29:37.000000 adbkit-0.20/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-05-29 01:29:36.000000 adbkit-0.20/MANIFEST.in
+-rw-rw-rw-   0        0        0   161921 2023-05-29 01:30:11.249017 adbkit-0.20/PKG-INFO
+-rw-rw-rw-   0        0        0   160268 2023-05-28 22:13:52.000000 adbkit-0.20/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:30:11.243032 adbkit-0.20/adbkit/
+-rw-rw-rw-   0        0        0   160268 2023-05-28 22:13:52.000000 adbkit-0.20/adbkit/README.MD
+-rw-rw-rw-   0        0        0   130248 2023-05-29 00:06:17.000000 adbkit-0.20/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-05-29 01:30:10.000000 adbkit-0.20/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   341731 2023-05-29 01:30:10.000000 adbkit-0.20/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-29 01:30:11.247022 adbkit-0.20/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   161921 2023-05-29 01:30:11.000000 adbkit-0.20/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-29 01:30:11.000000 adbkit-0.20/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:30:11.000000 adbkit-0.20/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      667 2023-05-29 01:30:11.000000 adbkit-0.20/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 01:30:11.000000 adbkit-0.20/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-29 01:30:11.250014 adbkit-0.20/setup.cfg
+-rw-rw-rw-   0        0        0     2823 2023-05-29 01:30:10.000000 adbkit-0.20/setup.py
```

### Comparing `adbkit-0.19/LICENSE.rst` & `adbkit-0.20/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.19/PKG-INFO` & `adbkit-0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.19
+Version: 0.20
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.19/README.md` & `adbkit-0.20/README.md`

 * *Files identical despite different names*

### Comparing `adbkit-0.19/adbkit/README.MD` & `adbkit-0.20/adbkit/README.MD`

 * *Files identical despite different names*

### Comparing `adbkit-0.19/adbkit/__init__.py` & `adbkit-0.20/adbkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     get_shapes_using_THRESH_OTSU,
     get_shapes_using_ADAPTIVE_THRESH_MEAN_C,
     get_shapes_using_ADAPTIVE_THRESH_GAUSSIAN_C,
 )
 from a_pandas_ex_adb_execute_activities import pd_add_adb_execute_activities
 
 from a_pandas_ex_image_tools import pd_add_image_tools
+from adb_push_create import push_file, make_folders
 from adbescapes import ADBInputEscaped
 
 from adbdevicechanger import AdbChanger
 from bstconnect import connect_to_all_localhost_devices
 from check_if_nan import is_nan
 from cv2imshow.cv2imshow import cv2_imshow_multi
 from taskkill import taskkill_regex_rearch
@@ -2482,15 +2483,17 @@
         else:
             print(f"Use {killkeys} to turn imshow on/off")
             self._start_show_screenshot(str(self.deviceserial), killkeys, sleeptime)
 
     def aa_activate_scrcpy_screenshots_usb(
         self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
     ):
-        screenwidth, screenheight = get_screen_height_width(self.adb_path, self.deviceserial)
+        screenwidth, screenheight = get_screen_height_width(
+            self.adb_path, self.deviceserial
+        )
         self.scrcpy_screenshot_usb = AdbShotUSB(
             device_serial=self.deviceserial,
             adb_path=self.adb_path,
             adb_host_address=adb_host_address,
             adb_host_port=adb_host_port,
             sleep_after_exception=0.05,
             frame_buffer=4,
@@ -2503,15 +2506,17 @@
             start_server=False,
             connect_to_device=False,
         )
 
     def aa_activate_scrcpy_screenshots_tcp(
         self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
     ):
-        screenwidth, screenheight = get_screen_height_width(self.adb_path, self.deviceserial)
+        screenwidth, screenheight = get_screen_height_width(
+            self.adb_path, self.deviceserial
+        )
 
         self.scrcpy_screenshot_tcp = AdbShotTCP(
             device_serial=self.deviceserial,
             adb_path=self.adb_path,
             ip=adb_host_address,
             port=adb_host_port,
             sleep_after_exception=0.05,
@@ -3237,14 +3242,27 @@
             self.adb_path,
             self.deviceserial,
             exit_keys=exit_keys,
             print_output=print_output,
             timeout=timeout,
         )
 
+    def aa_create_nested_folder_path(self, path):
+        return make_folders(
+            adb_path=self.adb_path, deviceserial=self.deviceserial, path2create=path
+        )
+
+    def aa_push_file_to_path(self, file, dest):
+        return push_file(
+            adb_path=self.adb_path,
+            deviceserial=self.deviceserial,
+            file=file,
+            dest=dest,
+        )
+
     def aa_list_pids_basic(
         self,
         exit_keys="ctrl+x",
         print_output=True,
         timeout=None,
     ):
         return list_pids(
```

### Comparing `adbkit-0.19/adbkit/requirements.txt` & `adbkit-0.20/adbkit/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 a_pandas_ex_adb_to_df
 a_pandas_ex_apply_ignore_exceptions
 a_pandas_ex_csv_plus
 a_pandas_ex_image_tools
 a_pandas_ex_logcat2df
 a_pandas_ex_tesseract_multirow_regex_fuzz
 adb_grep_search
+adb_push_create
 adb_unicode_keyboard
 adbblitz
 adbdevicechanger
 adbescapes
 androdf
 bstconnect
 check_if_nan
```

### Comparing `adbkit-0.19/adbkit/thirdparty.json` & `adbkit-0.20/adbkit/thirdparty.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967948717948718%*

 * *Differences: {'13': "{'LicenseText': '\\n\\n The MIT License (MIT)\\n\\n Copyright (c) 2023 Johannes "*

 * *       'Fischer\\n\\n \\n\\n Permission is hereby granted, free of charge, to any person obtaining '*

 * *       'a copy\\n\\n of this software and associated documentation files (the "Software"), to '*

 * *       'deal\\n\\n in the Software without restriction, including without limitation the '*

 * *       'rights\\n\\n to use, copy, modify, merge, publish, distribute, sublicense, and/or '*

 * *       'sell\\n\\n copies of the Software, […]*

```diff
@@ -69,21 +69,27 @@
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adb-grep-search",
         "Version": "0.12"
     },
     {
         "License": "MIT",
-        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2022 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
-        "Name": "adb-unicode-keyboard",
+        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
+        "Name": "adb-push-create",
         "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
+        "Name": "adb-unicode-keyboard",
+        "Version": "0.11"
+    },
+    {
+        "License": "MIT",
+        "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adbblitz",
         "Version": "0.10"
     },
     {
         "License": "MIT",
         "LicenseText": "\n\n The MIT License (MIT)\n\n Copyright (c) 2023 Johannes Fischer\n\n \n\n Permission is hereby granted, free of charge, to any person obtaining a copy\n\n of this software and associated documentation files (the \"Software\"), to deal\n\n in the Software without restriction, including without limitation the rights\n\n to use, copy, modify, merge, publish, distribute, sublicense, and/or sell\n\n copies of the Software, and to permit persons to whom the Software is\n\n furnished to do so, subject to the following conditions:\n\n \n\n The above copyright notice and this permission notice shall be included in all\n\n copies or substantial portions of the Software.\n\n \n\n THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\n\n EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\n\n MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\n\n IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,\n\n DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n\n OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE\n\n OR OTHER DEALINGS IN THE SOFTWARE.\n\n\n\n",
         "Name": "adbdevicechanger",
```

### Comparing `adbkit-0.19/adbkit.egg-info/PKG-INFO` & `adbkit-0.20/adbkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.19
+Version: 0.20
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.19/adbkit.egg-info/requires.txt` & `adbkit-0.20/adbkit.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 a_pandas_ex_adb_to_df
 a_pandas_ex_apply_ignore_exceptions
 a_pandas_ex_csv_plus
 a_pandas_ex_image_tools
 a_pandas_ex_logcat2df
 a_pandas_ex_tesseract_multirow_regex_fuzz
 adb_grep_search
+adb_push_create
 adb_unicode_keyboard
 adbblitz
 adbdevicechanger
 adbescapes
 androdf
 bstconnect
 check_if_nan
```

### Comparing `adbkit-0.19/setup.py` & `adbkit-0.20/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.19'''
+VERSION = '''0.20'''
 DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/adbkit',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
+    #packages=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_push_create', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
     keywords=['adb', 'android', 'automation', 'shell', 'root'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
+    install_requires=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_push_create', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```


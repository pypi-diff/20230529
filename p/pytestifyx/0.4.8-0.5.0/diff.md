# Comparing `tmp/pytestifyx-0.4.8-py2.py3-none-any.whl.zip` & `tmp/pytestifyx-0.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 56769 bytes, number of entries: 87
--rw-r--r--  2.0 unx      208 b- defN 23-May-25 12:52 pytestifyx/__init__.py
+Zip file size: 59790 bytes, number of entries: 88
+-rw-r--r--  2.0 unx      208 b- defN 23-May-29 13:05 pytestifyx/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 23-May-10 13:55 pytestifyx/chinese_fix.py
--rw-r--r--  2.0 unx      846 b- defN 23-Apr-02 10:19 pytestifyx/cli.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-29 13:01 pytestifyx/cli.py
 -rw-r--r--  2.0 unx     1611 b- defN 23-May-22 23:17 pytestifyx/config.py
 -rw-r--r--  2.0 unx      895 b- defN 23-May-22 23:17 pytestifyx/core.py
+-rw-r--r--  2.0 unx    15403 b- defN 23-May-29 13:04 pytestifyx/parse.py
 -rw-r--r--  2.0 unx     2085 b- defN 23-Apr-02 11:05 pytestifyx/scaffold.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 12:47 pytestifyx/driver/__init__.py
 -rw-r--r--  2.0 unx    15016 b- defN 23-May-22 23:19 pytestifyx/driver/api.py
 -rw-r--r--  2.0 unx     4770 b- defN 23-May-25 12:51 pytestifyx/driver/web.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 13:26 pytestifyx/test_project/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-16 15:20 pytestifyx/test_project/api_test/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-02 10:23 pytestifyx/test_project/api_test/test_application/__init__.py
@@ -76,14 +77,14 @@
 -rw-r--r--  2.0 unx      712 b- defN 23-May-22 23:18 pytestifyx/utils/public/get_project_path.py
 -rw-r--r--  2.0 unx      300 b- defN 23-Feb-23 12:06 pytestifyx/utils/public/img_to_base64.py
 -rw-r--r--  2.0 unx      372 b- defN 23-May-10 13:35 pytestifyx/utils/public/printify_table.py
 -rw-r--r--  2.0 unx      608 b- defN 23-May-10 13:36 pytestifyx/utils/public/trans_param_style.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-19 04:37 pytestifyx/utils/requests/__init__.py
 -rw-r--r--  2.0 unx      464 b- defN 22-Nov-21 14:29 pytestifyx/utils/requests/reload_all.py
 -rw-r--r--  2.0 unx     2485 b- defN 23-May-22 23:17 pytestifyx/utils/requests/requests_config.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1046 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      132 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8923 b- defN 23-May-25 12:52 pytestifyx-0.4.8.dist-info/RECORD
-87 files, 135541 bytes uncompressed, 41829 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1046 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      132 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9001 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/RECORD
+88 files, 151307 bytes uncompressed, 44736 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: pytestifyx/config.py
 Comment: 
 
 Filename: pytestifyx/core.py
 Comment: 
 
+Filename: pytestifyx/parse.py
+Comment: 
+
 Filename: pytestifyx/scaffold.py
 Comment: 
 
 Filename: pytestifyx/driver/__init__.py
 Comment: 
 
 Filename: pytestifyx/driver/api.py
@@ -237,26 +240,26 @@
 
 Filename: pytestifyx/utils/requests/reload_all.py
 Comment: 
 
 Filename: pytestifyx/utils/requests/requests_config.py
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/LICENSE
+Filename: pytestifyx-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/METADATA
+Filename: pytestifyx-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/WHEEL
+Filename: pytestifyx-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/entry_points.txt
+Filename: pytestifyx-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/top_level.txt
+Filename: pytestifyx-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytestifyx-0.4.8.dist-info/RECORD
+Filename: pytestifyx-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytestifyx/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .core import TestCase
 from .utils.logs.core import log
 
 __author__ = "luyh"
 
-__version__ = "0.4.8"
+__version__ = "0.5.0"
 
 __description__ = "pytestifyx is a pytest-based automation testing framework for api, ui, app testing"
```

## pytestifyx/cli.py

```diff
@@ -1,24 +1,29 @@
 from argparse import ArgumentParser
 import sys
 
 from pytestifyx import __description__, __version__
+from pytestifyx.parse import trans_saz_to_test
 from pytestifyx.scaffold import main_scaffold
 
 
 def main():
     # 命令行处理程序入口
     arg_parser = ArgumentParser(description=__description__)
     arg_parser.add_argument("-V", "--version", dest="version", action="store_true", help="show version")
-    arg_parser.add_argument("-P", "--project", dest="version", action="store_true", help="Create an inuyasha test project")
+    arg_parser.add_argument("-P", "--project", dest="project", action="store_true", help="Create an inuyasha test project")
+    arg_parser.add_argument("-T", "--parse", dest="parse", action="store_true", help="fiddler saz file parse to pytestifyx test case")
 
     if sys.argv[1] in ["-V", "--version"]:
         print(f"{__version__}")
     elif sys.argv[1] in ["-h", "--help"]:
         arg_parser.print_help()
     elif sys.argv[1] in ["-P", "--project"]:
         arg_parser.print_help()
         main_scaffold()
+    elif sys.argv[1] in ["-T", "--parse"]:
+        arg_parser.print_help()
+        trans_saz_to_test()
     else:
         print(f"Unknown command: {sys.argv[1]}")
         arg_parser.print_help()
         sys.exit(0)
```

## Comparing `pytestifyx-0.4.8.dist-info/LICENSE` & `pytestifyx-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytestifyx-0.4.8.dist-info/METADATA` & `pytestifyx-0.5.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestifyx
-Version: 0.4.8
+Version: 0.5.0
 Summary: pytestifyx is a pytest-based automation testing framework for api, ui, app testing
 Home-page: https://github.com/jaylu2018/PyTestifyx
 Author: luyh
 Author-email: jaylu1995@outlook.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `pytestifyx-0.4.8.dist-info/RECORD` & `pytestifyx-0.5.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-pytestifyx/__init__.py,sha256=nvzGfa7kRUeG5xzaZfXG6x2d_gmlPNMncv91s6c272M,208
+pytestifyx/__init__.py,sha256=eImb2lTWPLRfb88I1hZV64LLPkCvtBFpEPkAMJUXQBY,208
 pytestifyx/chinese_fix.py,sha256=qFkCAFR4EspSMgeBwuiAZ9zl51SEESgp4wKqEFqzGe8,302
-pytestifyx/cli.py,sha256=VZn72UAbdOG2n5SAZ5Q8OigiukupTPb28jbGsER12Y8,846
+pytestifyx/cli.py,sha256=0nHxXP3NGN7Sdzw3l8p2hGBRIqehO3LWMDCHgSVCD-o,1131
 pytestifyx/config.py,sha256=M9ViILKvF2T4dDjofHDPlCrYlZOlkQ0tExFaNsSN-e0,1611
 pytestifyx/core.py,sha256=XHbqbn2dtB6v40-k4guU449wXhF3W3aCkYa6Wm1hsOA,895
+pytestifyx/parse.py,sha256=SGLFSZ3FWxXs_e8wmc1YWDl4sun_3cHaCYtsk4ctHVY,15403
 pytestifyx/scaffold.py,sha256=c-zhigz3Zqo2zwt3r9H6Wu-6MQPR27-Q4qU6M3-cQGc,2085
 pytestifyx/driver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/driver/api.py,sha256=RoNIw48wkdRQd-d8N26oa-SMQefIEP2AApZSMCMv50o,15016
 pytestifyx/driver/web.py,sha256=cVX0WeZ-plJc96Otwl--p9680CwphPihhN-JxXCJzus,4770
 pytestifyx/test_project/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/test_project/api_test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/test_project/api_test/test_application/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -75,13 +76,13 @@
 pytestifyx/utils/public/get_project_path.py,sha256=JqweA7jeZZc_bUeNOpcm0NnOGoE9WVBCdRIfDKHuq0Q,712
 pytestifyx/utils/public/img_to_base64.py,sha256=IxTLg8b_QINdixlU-HTiWQ57CT4F8Yu3VXIcms2QRHo,300
 pytestifyx/utils/public/printify_table.py,sha256=9fWgPBfsDwnnkFJKi57tHFZtdFARdYoWS-3le4I_Jpk,372
 pytestifyx/utils/public/trans_param_style.py,sha256=lYJR85uWtLPoqpK3N_ja53jqMu3tMasR61PGsUQCZqk,608
 pytestifyx/utils/requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/requests/reload_all.py,sha256=rB3ORnl1cYZ7vkAUitzVNOg2TV2Ao1OlvQqmZVopZ6w,464
 pytestifyx/utils/requests/requests_config.py,sha256=JDJTRBNGEfcemJtR4E0aZc89tnzCvYtX4PcSZzencKo,2485
-pytestifyx-0.4.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytestifyx-0.4.8.dist-info/METADATA,sha256=Xxd3H4XuKbCtGY8XARiweSlg-uBeZP3OU8mXf6WEzc4,1046
-pytestifyx-0.4.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-pytestifyx-0.4.8.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
-pytestifyx-0.4.8.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
-pytestifyx-0.4.8.dist-info/RECORD,,
+pytestifyx-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytestifyx-0.5.0.dist-info/METADATA,sha256=oGJkTJjEp85UBbEfRW84S9Xjh16qpyczsnAMzmVzWIE,1046
+pytestifyx-0.5.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+pytestifyx-0.5.0.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
+pytestifyx-0.5.0.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
+pytestifyx-0.5.0.dist-info/RECORD,,
```


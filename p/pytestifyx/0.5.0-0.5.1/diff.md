# Comparing `tmp/pytestifyx-0.5.0-py2.py3-none-any.whl.zip` & `tmp/pytestifyx-0.5.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 59790 bytes, number of entries: 88
--rw-r--r--  2.0 unx      208 b- defN 23-May-29 13:05 pytestifyx/__init__.py
+Zip file size: 59799 bytes, number of entries: 88
+-rw-r--r--  2.0 unx      208 b- defN 23-May-29 13:08 pytestifyx/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 23-May-10 13:55 pytestifyx/chinese_fix.py
 -rw-r--r--  2.0 unx     1131 b- defN 23-May-29 13:01 pytestifyx/cli.py
 -rw-r--r--  2.0 unx     1611 b- defN 23-May-22 23:17 pytestifyx/config.py
 -rw-r--r--  2.0 unx      895 b- defN 23-May-22 23:17 pytestifyx/core.py
 -rw-r--r--  2.0 unx    15403 b- defN 23-May-29 13:04 pytestifyx/parse.py
 -rw-r--r--  2.0 unx     2085 b- defN 23-Apr-02 11:05 pytestifyx/scaffold.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 12:47 pytestifyx/driver/__init__.py
@@ -77,14 +77,14 @@
 -rw-r--r--  2.0 unx      712 b- defN 23-May-22 23:18 pytestifyx/utils/public/get_project_path.py
 -rw-r--r--  2.0 unx      300 b- defN 23-Feb-23 12:06 pytestifyx/utils/public/img_to_base64.py
 -rw-r--r--  2.0 unx      372 b- defN 23-May-10 13:35 pytestifyx/utils/public/printify_table.py
 -rw-r--r--  2.0 unx      608 b- defN 23-May-10 13:36 pytestifyx/utils/public/trans_param_style.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-19 04:37 pytestifyx/utils/requests/__init__.py
 -rw-r--r--  2.0 unx      464 b- defN 22-Nov-21 14:29 pytestifyx/utils/requests/reload_all.py
 -rw-r--r--  2.0 unx     2485 b- defN 23-May-22 23:17 pytestifyx/utils/requests/requests_config.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1046 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      132 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9001 b- defN 23-May-29 13:05 pytestifyx-0.5.0.dist-info/RECORD
-88 files, 151307 bytes uncompressed, 44736 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1081 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      132 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9001 b- defN 23-May-29 13:09 pytestifyx-0.5.1.dist-info/RECORD
+88 files, 151342 bytes uncompressed, 44745 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -240,26 +240,26 @@
 
 Filename: pytestifyx/utils/requests/reload_all.py
 Comment: 
 
 Filename: pytestifyx/utils/requests/requests_config.py
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/LICENSE
+Filename: pytestifyx-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/METADATA
+Filename: pytestifyx-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/WHEEL
+Filename: pytestifyx-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/entry_points.txt
+Filename: pytestifyx-0.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/top_level.txt
+Filename: pytestifyx-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pytestifyx-0.5.0.dist-info/RECORD
+Filename: pytestifyx-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytestifyx/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .core import TestCase
 from .utils.logs.core import log
 
 __author__ = "luyh"
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 __description__ = "pytestifyx is a pytest-based automation testing framework for api, ui, app testing"
```

## Comparing `pytestifyx-0.5.0.dist-info/LICENSE` & `pytestifyx-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytestifyx-0.5.0.dist-info/METADATA` & `pytestifyx-0.5.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestifyx
-Version: 0.5.0
+Version: 0.5.1
 Summary: pytestifyx is a pytest-based automation testing framework for api, ui, app testing
 Home-page: https://github.com/jaylu2018/PyTestifyx
 Author: luyh
 Author-email: jaylu1995@outlook.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,20 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytest (~=7.2.1)
-Requires-Dist: playwright (~=1.30.0)
-Requires-Dist: pytest-playwright (~=0.3.0)
-Requires-Dist: pytest-cases (~=3.6.13)
-Requires-Dist: loguru (~=0.6.0)
-Requires-Dist: prettytable (~=3.6.0)
-Requires-Dist: deepdiff (~=6.3.0)
+Requires-Dist: pytest (>=7.2.1)
+Requires-Dist: playwright (>=1.30.0)
+Requires-Dist: pytest-playwright (>=0.3.0)
+Requires-Dist: pytest-cases (>=3.6.13)
+Requires-Dist: loguru (>=0.6.0)
+Requires-Dist: prettytable (>=3.6.0)
+Requires-Dist: deepdiff (>=6.3.0)
+Requires-Dist: requests (==2.29.0)
 
 # pytestifyx
 pytestifyx is a pytest-based automation testing framework for api, ui, app testing
```

## Comparing `pytestifyx-0.5.0.dist-info/RECORD` & `pytestifyx-0.5.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pytestifyx/__init__.py,sha256=eImb2lTWPLRfb88I1hZV64LLPkCvtBFpEPkAMJUXQBY,208
+pytestifyx/__init__.py,sha256=0uFOBFyWahMr9D4qdIZgCKEyxtQ8ZnZpsu9dWiryOr8,208
 pytestifyx/chinese_fix.py,sha256=qFkCAFR4EspSMgeBwuiAZ9zl51SEESgp4wKqEFqzGe8,302
 pytestifyx/cli.py,sha256=0nHxXP3NGN7Sdzw3l8p2hGBRIqehO3LWMDCHgSVCD-o,1131
 pytestifyx/config.py,sha256=M9ViILKvF2T4dDjofHDPlCrYlZOlkQ0tExFaNsSN-e0,1611
 pytestifyx/core.py,sha256=XHbqbn2dtB6v40-k4guU449wXhF3W3aCkYa6Wm1hsOA,895
 pytestifyx/parse.py,sha256=SGLFSZ3FWxXs_e8wmc1YWDl4sun_3cHaCYtsk4ctHVY,15403
 pytestifyx/scaffold.py,sha256=c-zhigz3Zqo2zwt3r9H6Wu-6MQPR27-Q4qU6M3-cQGc,2085
 pytestifyx/driver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -76,13 +76,13 @@
 pytestifyx/utils/public/get_project_path.py,sha256=JqweA7jeZZc_bUeNOpcm0NnOGoE9WVBCdRIfDKHuq0Q,712
 pytestifyx/utils/public/img_to_base64.py,sha256=IxTLg8b_QINdixlU-HTiWQ57CT4F8Yu3VXIcms2QRHo,300
 pytestifyx/utils/public/printify_table.py,sha256=9fWgPBfsDwnnkFJKi57tHFZtdFARdYoWS-3le4I_Jpk,372
 pytestifyx/utils/public/trans_param_style.py,sha256=lYJR85uWtLPoqpK3N_ja53jqMu3tMasR61PGsUQCZqk,608
 pytestifyx/utils/requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/requests/reload_all.py,sha256=rB3ORnl1cYZ7vkAUitzVNOg2TV2Ao1OlvQqmZVopZ6w,464
 pytestifyx/utils/requests/requests_config.py,sha256=JDJTRBNGEfcemJtR4E0aZc89tnzCvYtX4PcSZzencKo,2485
-pytestifyx-0.5.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytestifyx-0.5.0.dist-info/METADATA,sha256=oGJkTJjEp85UBbEfRW84S9Xjh16qpyczsnAMzmVzWIE,1046
-pytestifyx-0.5.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-pytestifyx-0.5.0.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
-pytestifyx-0.5.0.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
-pytestifyx-0.5.0.dist-info/RECORD,,
+pytestifyx-0.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytestifyx-0.5.1.dist-info/METADATA,sha256=x1QGkR7yJCArNGA5yTG4zhDmuAJYA5st-lj06xDlck0,1081
+pytestifyx-0.5.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+pytestifyx-0.5.1.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
+pytestifyx-0.5.1.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
+pytestifyx-0.5.1.dist-info/RECORD,,
```


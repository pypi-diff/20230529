# Comparing `tmp/msg2po-1.1.8.tar.gz` & `tmp/msg2po-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg2po-1.1.8.tar", max compression
+gzip compressed data, was "msg2po-1.1.9.tar", max compression
```

## Comparing `msg2po-1.1.8.tar` & `msg2po-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1428 2023-02-18 23:53:40.888630 msg2po-1.1.8/README.md
--rw-r--r--   0        0        0        0 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/__init__.py
--rwxr-xr-x   0        0        0     1617 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/bgforge_config.py
--rw-r--r--   0        0        0      511 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/common.py
--rw-r--r--   0        0        0     2033 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/config.py
--rw-r--r--   0        0        0    31400 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/core.py
--rwxr-xr-x   0        0        0      731 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/diff_male_female_po_to_csv.py
--rwxr-xr-x   0        0        0     4016 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/dir2msgstr.py
--rwxr-xr-x   0        0        0     1144 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/female_csv2po.py
--rwxr-xr-x   0        0        0     1374 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/file2msgstr.py
--rwxr-xr-x   0        0        0      731 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/file2po.py
--rwxr-xr-x   0        0        0     1756 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/lowercase.py
--rwxr-xr-x   0        0        0     2447 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/msgmerge.py
--rwxr-xr-x   0        0        0      892 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/po2file.py
--rwxr-xr-x   0        0        0     4477 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/poify.py
--rwxr-xr-x   0        0        0      662 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/resave_po.py
--rwxr-xr-x   0        0        0     2199 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/unfuzzy.py
--rw-r--r--   0        0        0     1336 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/unfuzzy.yml
--rwxr-xr-x   0        0        0     1122 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/unfuzzy_cassidy.py
--rwxr-xr-x   0        0        0     2272 2023-02-18 23:53:40.888630 msg2po-1.1.8/msg2po/unpoify.py
--rw-r--r--   0        0        0     1155 2023-02-18 23:53:40.888630 msg2po-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 msg2po-1.1.8/setup.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 msg2po-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1428 2023-02-23 18:25:08.757121 msg2po-1.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/__init__.py
+-rwxr-xr-x   0        0        0     1617 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/bgforge_config.py
+-rw-r--r--   0        0        0      511 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/common.py
+-rw-r--r--   0        0        0     2033 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/config.py
+-rw-r--r--   0        0        0    31400 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/core.py
+-rwxr-xr-x   0        0        0      731 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/diff_male_female_po_to_csv.py
+-rwxr-xr-x   0        0        0     4016 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/dir2msgstr.py
+-rwxr-xr-x   0        0        0     1144 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/female_csv2po.py
+-rwxr-xr-x   0        0        0     1374 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/file2msgstr.py
+-rwxr-xr-x   0        0        0      731 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/file2po.py
+-rwxr-xr-x   0        0        0     1756 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/lowercase.py
+-rwxr-xr-x   0        0        0     2447 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/msgmerge.py
+-rwxr-xr-x   0        0        0      892 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/po2file.py
+-rwxr-xr-x   0        0        0     4477 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/poify.py
+-rwxr-xr-x   0        0        0      662 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/resave_po.py
+-rwxr-xr-x   0        0        0     2199 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy.py
+-rw-r--r--   0        0        0     1336 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy.yml
+-rwxr-xr-x   0        0        0     1122 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy_cassidy.py
+-rwxr-xr-x   0        0        0     2272 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unpoify.py
+-rw-r--r--   0        0        0     1155 2023-02-23 18:25:08.757121 msg2po-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 msg2po-1.1.9/setup.py
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 msg2po-1.1.9/PKG-INFO
```

### Comparing `msg2po-1.1.8/README.md` & `msg2po-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/bgforge_config.py` & `msg2po-1.1.9/msg2po/bgforge_config.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/config.py` & `msg2po-1.1.9/msg2po/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ruamel.yaml
 import sys
 import os
 
-VERSION = "1.1.8"
+VERSION = "1.1.9"
 
 
 class Config:
     def __init__(self):
         yml = ".bgforge.yml"
         translation_defaults = {
             "encoding": "cp1252",
```

### Comparing `msg2po-1.1.8/msg2po/core.py` & `msg2po-1.1.9/msg2po/core.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/diff_male_female_po_to_csv.py` & `msg2po-1.1.9/msg2po/diff_male_female_po_to_csv.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/dir2msgstr.py` & `msg2po-1.1.9/msg2po/dir2msgstr.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/female_csv2po.py` & `msg2po-1.1.9/msg2po/female_csv2po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/file2msgstr.py` & `msg2po-1.1.9/msg2po/file2msgstr.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/file2po.py` & `msg2po-1.1.9/msg2po/file2po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/lowercase.py` & `msg2po-1.1.9/msg2po/lowercase.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/msgmerge.py` & `msg2po-1.1.9/msg2po/msgmerge.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/po2file.py` & `msg2po-1.1.9/msg2po/po2file.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/poify.py` & `msg2po-1.1.9/msg2po/poify.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/resave_po.py` & `msg2po-1.1.9/msg2po/resave_po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/unfuzzy.py` & `msg2po-1.1.9/msg2po/unfuzzy.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/unfuzzy.yml` & `msg2po-1.1.9/msg2po/unfuzzy.yml`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/unfuzzy_cassidy.py` & `msg2po-1.1.9/msg2po/unfuzzy_cassidy.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/msg2po/unpoify.py` & `msg2po-1.1.9/msg2po/unpoify.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.8/pyproject.toml` & `msg2po-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msg2po"
-version = "1.1.8"
+version = "1.1.9"
 description = "A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back"
 authors = ["BGforge <dev@bgforge.net>"]
 keywords = ["Fallout", "Fallout 2", "Baldur's Gate", "Infinity Engine", "WeiDU"]
 readme = "README.md"
 homepage = "https://github.com/BGforgeNet/msg2po"
 repository = "https://github.com/BGforgeNet/msg2po"
```

### Comparing `msg2po-1.1.8/setup.py` & `msg2po-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                      'msgmerge-female = msg2po.msgmerge:main',
                      'po2file = msg2po.po2file:main',
                      'resave-po = msg2po.resave_po:main',
                      'unpoify = msg2po.unpoify:main']}
 
 setup_kwargs = {
     'name': 'msg2po',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back',
     'long_description': '# MSG2PO\n\n[![Build status](https://github.com/BGforgeNet/msg2po/workflows/release/badge.svg)](https://github.com/BGforgeNet/msg2po/actions?query=workflow%3Arelease)\n[![Patreon](https://img.shields.io/badge/Patreon-donate-FF424D?logo=Patreon&labelColor=141518)](https://www.patreon.com/BGforge)\n[![Telegram](https://img.shields.io/badge/telegram-join%20%20%20%20%E2%9D%B1%E2%9D%B1%E2%9D%B1-darkorange?logo=telegram)](https://t.me/bgforge)\n[![Discord](https://img.shields.io/discord/420268540700917760?logo=discord&label=discord&color=blue&logoColor=FEE75C)](https://discord.gg/4Yqfggm)\n[![IRC](https://img.shields.io/badge/%23IRC-join%20%20%20%20%E2%9D%B1%E2%9D%B1%E2%9D%B1-darkorange)](https://bgforge.net/irc)\n\nThis is a set of tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back, used in [BGforge Hive](https://hive.bgforge.net/). Ask questions [here](https://forums.bgforge.net/viewforum.php?f=9).\n\n## Installation\n```bash\npip install msg2po\n```\n\n## Usage\n```bash\n$ poify.py -h\n.bgforge.yml not found, assuming defaults\nusage: poify.py [-h] [-e ENC] [DIR]\n\nPoify files in selected directory\n\npositional arguments:\n  DIR         source language directory (default: ./english)\n\noptions:\n  -h, --help  show this help message and exit\n  -e ENC      source encoding (default: cp1252)\n```\n\n## Action\nGithub [action](docs/action.md) is available for automatic processing.\n\n---\n[Changelog](docs/changelog.md)\n',
     'author': 'BGforge',
     'author_email': 'dev@bgforge.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/BGforgeNet/msg2po',
```

### Comparing `msg2po-1.1.8/PKG-INFO` & `msg2po-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msg2po
-Version: 1.1.8
+Version: 1.1.9
 Summary: A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back
 Home-page: https://github.com/BGforgeNet/msg2po
 Keywords: Fallout,Fallout 2,Baldur's Gate,Infinity Engine,WeiDU
 Author: BGforge
 Author-email: dev@bgforge.net
 Requires-Python: >=3.6.2
 Classifier: Programming Language :: Python :: 3
```


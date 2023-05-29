# Comparing `tmp/honkaistarrail-0.0.3.tar.gz` & `tmp/honkaistarrail-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkaistarrail-0.0.3.tar", max compression
+gzip compressed data, was "honkaistarrail-0.0.4.tar", max compression
```

## Comparing `honkaistarrail-0.0.3.tar` & `honkaistarrail-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.3/honkaistarrail/calculator.py
--rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.3/honkaistarrail/modal.py
--rw-r--r--   0        0        0    29135 2023-05-04 13:30:29.205747 honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
--rw-r--r--   0        0        0    38022 2023-05-04 13:30:26.497309 honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/gacha_data.py
--rw-r--r--   0        0        0     6803 2023-05-04 13:50:38.210012 honkaistarrail-0.0.3/honkaistarrail/starrail.py
--rw-r--r--   0        0        0      480 2023-05-04 14:14:45.073560 honkaistarrail-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.3/README.md
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.3/setup.py
--rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-04-30 01:59:37.302415 honkaistarrail-0.0.4/honkaistarrail/calculator.py
+-rw-r--r--   0        0        0     1308 2023-05-04 13:23:46.753489 honkaistarrail-0.0.4/honkaistarrail/modal.py
+-rw-r--r--   0        0        0    29135 2023-05-04 13:30:29.205747 honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc
+-rw-r--r--   0        0        0    38022 2023-05-04 13:30:26.497309 honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/gacha_data.py
+-rw-r--r--   0        0        0     6977 2023-05-29 19:55:18.822822 honkaistarrail-0.0.4/honkaistarrail/starrail.py
+-rw-r--r--   0        0        0      480 2023-05-29 19:56:15.501740 honkaistarrail-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1623 2023-05-04 14:13:03.361305 honkaistarrail-0.0.4/README.md
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 honkaistarrail-0.0.4/setup.py
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 honkaistarrail-0.0.4/PKG-INFO
```

### Comparing `honkaistarrail-0.0.3/honkaistarrail/calculator.py` & `honkaistarrail-0.0.4/honkaistarrail/calculator.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.3/honkaistarrail/modal.py` & `honkaistarrail-0.0.4/honkaistarrail/modal.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc` & `honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/__pycache__/gacha_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.3/honkaistarrail/src/data/gacha/gacha_data.py` & `honkaistarrail-0.0.4/honkaistarrail/src/data/gacha/gacha_data.py`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.3/honkaistarrail/starrail.py` & `honkaistarrail-0.0.4/honkaistarrail/starrail.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,53 +27,54 @@
         examination(lang,banner)
         self.link = link
         if self.link == "":
             self.get_auto_link(reg=reg)
         self.limit = limit
         self.lang = lang
         self.banner = str(banner)
-        data = self.set_parameters()
+        if self.link != "-":
+            data = self.set_parameters()
 
-        if data.authkey == None:
-            raise ValueError(f"Check if the link is correct")
+            if data.authkey == None:
+                raise ValueError(f"Check if the link is correct")
+                
+            if data.lang != self.lang:
+                data.lang = self.lang
             
-        if data.lang != self.lang:
-            data.lang = self.lang
-        
-        if self.banner == "1":
-            #EVENT
-            data.gacha_id = _EVENT
-            data.default_gacha_type = 11
-        elif self.banner == "2":
-            #LIGHT CONE
-            data.gacha_id = _LIGHT_CONE
-            data.default_gacha_type = 12
-        else:
-            #STANDART
-            data.gacha_id = _STANDART
-            data.default_gacha_type = 1
-        self.params = {
-            "authkey_ver": data.authkey_ver,
-            "gacha_id": data.gacha_id,
-            "timestamp": int(datetime.now(timezone.utc).astimezone(timezone.utc).replace(tzinfo=timezone.utc).timestamp()),
-            "region": data.region,
-            "default_gacha_type": data.default_gacha_type ,
-            "lang": data.lang,
-            "authkey": urllib.parse.unquote(data.authkey),
-            "game_biz": data.game_biz,
-            "plat_type": "pc",
-            "page": 1,
-            "size": 20,
-            "gacha_type": data.default_gacha_type,
-            "end_id": 0
-        }
+            if self.banner == "1":
+                #EVENT
+                data.gacha_id = _EVENT
+                data.default_gacha_type = 11
+            elif self.banner == "2":
+                #LIGHT CONE
+                data.gacha_id = _LIGHT_CONE
+                data.default_gacha_type = 12
+            else:
+                #STANDART
+                data.gacha_id = _STANDART
+                data.default_gacha_type = 1
+            self.params = {
+                "authkey_ver": data.authkey_ver,
+                "gacha_id": data.gacha_id,
+                "timestamp": int(datetime.now(timezone.utc).astimezone(timezone.utc).replace(tzinfo=timezone.utc).timestamp()),
+                "region": data.region,
+                "default_gacha_type": data.default_gacha_type ,
+                "lang": data.lang,
+                "authkey": urllib.parse.unquote(data.authkey),
+                "game_biz": data.game_biz,
+                "plat_type": "pc",
+                "page": 1,
+                "size": 20,
+                "gacha_type": data.default_gacha_type,
+                "end_id": 0
+            }
 
 
-        self.history = []
-        self.response = None
+            self.history = []
+            self.response = None
 
     def get_auto_link(self, reg = "os"):
         if reg.lower() == "os":
             cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/d5b77400c5d710e4260474afa5011d17/raw/bd8c200f7906fb005d4d11097a8f95e4feb8823f/HonkaiStarRailJump.ps1")'] 
         elif reg.lower() == "cn":
             cmd = ['powershell', '-Command', 'Invoke-Expression (New-Object Net.WebClient).DownloadString("https://gist.githubusercontent.com/DEViantUA/19d224c9c13e6f6b1cc62a12fc0e8a9d/raw/9dcd08b8033d9e60921e216c7219354e863e13b5/HonkaiStarRailJump_CN.ps1")'] 
         else:
```

### Comparing `honkaistarrail-0.0.3/README.md` & `honkaistarrail-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `honkaistarrail-0.0.3/setup.py` & `honkaistarrail-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['honkaistarrail', 'honkaistarrail.src.data.gacha']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkaistarrail',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Asynchronous module for working with API Honkai: Star Rail',
     'long_description': '<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/HSR-BANNER.png" />\n</p>\n\n# Asynchronous module for working with API Honkai: Star Rail\n\nAt the moment it only supports counting guarantors and getting a jumps \n\n### Installation: \n```\npip install honkaistarrail\n```\nPyPi: [OPEN](https://pypi.org/project/honkaistarrail/)\n\nYou can also see other usage examples here: [OPEN](https://github.com/DEViantUA/starrail.py/tree/main/Examples)\n\nInstructions for getting a link to the history of jumps: [OPEN](https://github.com/DEViantUA/starrail.py/blob/main/Instruction.md)\n\n### ID Banned:\n``1`` - Event Banner\n``2`` - Light Cone\n``3`` - Standart Banner\n\n\n### Launc:\n\n```py\n# Copyright 2023 DEViantUa <t.me/deviant_ua>\n# All rights reserved.\n\n\'\'\'\nThis method returns the full history of jumps for the \nlast 3 months, does not return the results of jumps \nand how much is left before the guarantor.\n\'\'\'\n\nimport asyncio\nfrom honkaistarrail import starrail\n\nasync def get_jump_history():\n    link = ""\n    async with starrail.Jump(link = link,banner = 1,lang = "en") as hist:\n        async for key in hist.get_history():\n            for info in key:\n                print(f\'[{info.type}] Name: {info.name} ({info.rank}*) - {info.time.strftime("%d.%m.%Y %H:%M:%S")}\')\n\n\nasyncio.run(get_jump_history())\n```\n\n\n# In developing:\n\n1. Automatic code redemption.\n2. Automatic collection of daily marks on HoYoLab.\n\n___\n<p align="center">\n  <img src="https://raw.githubusercontent.com/DEViantUA/HonkaiStarRail.py/main/Readme/%D0%91%D0%B5%D0%B7-%D0%B8%D0%BC%D0%B5%D0%BD%D0%B8-1.png" />\n</p>\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiStarRail.py',
```

### Comparing `honkaistarrail-0.0.3/PKG-INFO` & `honkaistarrail-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkaistarrail
-Version: 0.0.3
+Version: 0.0.4
 Summary: Asynchronous module for working with API Honkai: Star Rail
 Home-page: https://github.com/DEViantUA/HonkaiStarRail.py
 Author: None
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


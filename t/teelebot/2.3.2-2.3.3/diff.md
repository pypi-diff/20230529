# Comparing `tmp/teelebot-2.3.2-py3-none-any.whl.zip` & `tmp/teelebot-2.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 40600 bytes, number of entries: 20
+Zip file size: 40622 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat     4241 b- defN 23-May-15 07:38 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    32825 b- defN 23-May-15 08:37 teelebot/bot.py
+-rw-rw-rw-  2.0 fat    33199 b- defN 23-May-29 02:04 teelebot/bot.py
 -rw-rw-rw-  2.0 fat     7128 b- defN 23-May-14 14:32 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat     1581 b- defN 23-May-15 07:43 teelebot/common.py
--rw-rw-rw-  2.0 fat    23796 b- defN 23-May-15 08:39 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    23008 b- defN 23-May-29 01:43 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
 -rw-rw-rw-  2.0 fat     7059 b- defN 23-May-14 18:00 teelebot/metadata.py
 -rw-rw-rw-  2.0 fat      737 b- defN 23-May-14 14:25 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     3824 b- defN 23-May-15 05:04 teelebot/request.py
 -rw-rw-rw-  2.0 fat     4075 b- defN 23-May-14 14:30 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      472 b- defN 23-May-15 02:41 teelebot/version.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-May-29 01:16 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9700 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1558 b- defN 23-May-15 08:51 teelebot-2.3.2.dist-info/RECORD
-20 files, 137602 bytes uncompressed, 38094 bytes compressed:  72.3%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9719 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1558 b- defN 23-May-29 02:26 teelebot-2.3.3.dist-info/RECORD
+20 files, 137218 bytes uncompressed, 38116 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -33,29 +33,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/LICENSE
+Filename: teelebot-2.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/METADATA
+Filename: teelebot-2.3.3.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/WHEEL
+Filename: teelebot-2.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/entry_points.txt
+Filename: teelebot-2.3.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/top_level.txt
+Filename: teelebot-2.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/zip-safe
+Filename: teelebot-2.3.3.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.3.2.dist-info/RECORD
+Filename: teelebot-2.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 """
-@description: A bot framework based on the Telegram Bot API
+@description: A Python-based Telegram Bot framework
 @creation date: 2019-08-13
-@last modification: 2023-05-15
+@last modification: 2023-05-29
 @author: Pluto (github:plutobell)
 """
 import time
 import sys
 import os
 import copy
 import types
@@ -166,16 +166,19 @@
         if fur.exception() is not None:
             _logger.debug(f"EXCEPTION - {str(fur.result())}")
 
     def __import_module(self, plugin_name):
         """
         Dynamic import module
         """
-        sys.path.append(self.path_converter(f'{self.__plugin_dir}{plugin_name}{os.sep}'))
-        Module = importlib.import_module(plugin_name)  # Module Detection
+        if self.__plugin_dir not in sys.path:
+            sys.path.append(self.__plugin_dir)
+        # print(sys.path)
+
+        Module = importlib.import_module(f'{plugin_name}.{plugin_name}')  # Module Detection
 
         return Module
 
     def __update_plugin(self, plugin_name, as_plugin=True):
         """
         Hot update plugin
         """
@@ -454,35 +457,39 @@
         except Exception as e:
             _logger.error(f"Run plugin error: {e}")
             traceback.print_exc()
             return
 
         for plugin, command in plugin_bridge.items():
             try:
-                plugin_requires_version = ""
-                ok, data = self.metadata.read(plugin_name=plugin)
-                # plugin_info = self.get_plugin_info(plugin_name=plugin)
-                if ok:
-                    plugin_requires_version = data.get("Requires-teelebot", {})
-                    plugin_requires_version = plugin_requires_version.replace(">", "").replace("<", "").replace("=", "")
-                    if plugin_requires_version in [None, "", " "]:
-                        _logger.warn(f"Skip run {plugin} plugin: failed to get the version of the plugin")
-                        continue
-                else:
-                    _logger.warn(f"Skip run {plugin} plugin: failed to get information about the plugin (error: {data})")
-                    continue
-                if plugin_requires_version > self.version:
-                    _logger.warn(f"Skip run {plugin} plugin: the plugin requires teelebot version >= {plugin_requires_version}")
-                    continue
-
                 if message_type == "query":
                     if command in ["", " ", None]:
                         continue
 
                 if message.get(message_type)[:len(command)] == command:
+                    plugin_requires_version = ""
+                    ok, data = self.metadata.read(plugin_name=plugin)
+                    if ok:
+                        plugin_requires_version = data.get("Requires-teelebot", {})
+                        plugin_requires_version = plugin_requires_version.replace(">", "").replace("<", "").replace("=", "")
+                        if plugin_requires_version in [None, "", " "]:
+                            _logger.warn(f"Skip run {plugin} plugin: failed to get the version of the plugin")
+                            continue
+                    else:
+                        _logger.warn(f"Skip run {plugin} plugin: failed to get information about the plugin (error: {data})")
+                        continue
+                    if plugin_requires_version > self.version:
+                        _logger.warn(f"Skip run {plugin} plugin: the plugin requires teelebot version >= {plugin_requires_version}")
+                        continue
+
+                    no_plugin_path = f'{self.__plugin_dir}{plugin}.py'
+                    if os.path.exists(no_plugin_path):
+                        _logger.warn(f"Skip run {plugin} plugin: there is a module named '{plugin}.py' under the plugin dir with the same name as plugin {plugin} ({no_plugin_path})")
+                        continue
+
                     try:
                         module = self.__import_module(plugin)
                         pluginFunc = getattr(module, plugin)
                         fur = self.__thread_pool.submit(pluginFunc, bot, message)
                         fur.add_done_callback(self.__threadpool_exception)
                     except Exception as e:
                         _logger.error(f"Run {plugin} plugin error: {str(e)}")
```

## teelebot/handler.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-05-15
+@last modification: 2023-05-29
 '''
 import configparser
 import argparse
 import re
 import os
 import sys
 import copy
@@ -193,28 +193,21 @@
 
     pycache_path = f'{os.path.dirname(os.path.abspath(__file__))}/__pycache__'
     if os.path.exists(str(Path(pycache_path))):
         shutil.rmtree(str(Path(pycache_path)))
 
     if not os.path.isdir(plugin_dir):  # Plugin directory detection
         os.makedirs(plugin_dir)
-        # os.mkdir(plugin_dir)
-        with open(str(Path(f'{plugin_dir}__init__.py')), "w", encoding="utf-8") as f:
-            pass
-    elif not os.path.exists(str(Path(f'{plugin_dir}__init__.py'))):
-        with open(str(Path(f'{plugin_dir}__init__.py')), "w", encoding="utf-8") as f:
-            pass
+    sys.path.append(plugin_dir)
 
     if args.make_plugin and plugin_dir_in_config: # Plugin template creation
         plugin_name = args.make_plugin
         if not os.path.exists(str(Path(plugin_dir + plugin_name))):
             os.mkdir(str(Path(plugin_dir + plugin_name)))
-            if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}__init__.py'))):
-                with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}__init__.py')), "w", encoding="utf-8") as init:
-                    pass
+
             if not os.path.exists(str(Path(f'{plugin_dir}{plugin_name}{os.sep}{plugin_name}.py'))):
                 with open(str(Path(f'{plugin_dir}{plugin_name}{os.sep}{plugin_name}.py')), "w", encoding="utf-8") as enter:
                     enter.writelines([
                         "# -*- coding: utf-8 -*-\n",
                         "\n",
                         "def " + plugin_name + "(bot, message):\n",
                         "\n" + \
@@ -398,16 +391,14 @@
     non_plugin_list = []
     plugin_list = []
     corrupted_plugin_list = []
 
     plugin_lis = os.listdir(plugin_dir)
     for plugi in plugin_lis:
         if os.path.isdir(str(Path(f'{plugin_dir}{plugi}'))) and plugi != "__pycache__" and plugi[0] != '.':
-            if not os.path.exists(Path(f"{plugin_dir}{plugi}{os.sep}__init__.py")):
-                with open(Path(f"{plugin_dir}{plugi}{os.sep}__init__.py"), "w", encoding="utf-8") as init: pass
             
             entrance_exist = False
             entrance_count = 0
             try:
                 with open(str(Path(f"{plugin_dir}{plugi}{os.sep}{plugi}.py")), "r", encoding="utf-8") as e:
                     content = e.read()
                     if f"def {plugi}(bot, message):" in content or \
@@ -427,35 +418,34 @@
 
             metadata_ok = False
             metadata = _Metadata(plugin_dir=plugin_dir)
             ok, metadata_data = metadata.read(plugin_name=plugi)
             if ok:
                 if list(metadata_data.keys()) == list(metadata_template.keys()):
                     metadata_ok = True
+
+                    if metadata_data["Command"] == common_pkg_prefix: # Skip plugin integrity checks
+                        continue
             else:
                 os.system("")
                 print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{str(metadata_data)}")
 
             package_file_list = os.listdir(str(Path(f'{plugin_dir}{plugi}')))
             if plugi + ".py" in package_file_list and \
-                "__init__.py" in package_file_list and \
                 "METADATA" in package_file_list and \
                 entrance_exist and entrance_count == 1 and metadata_ok:
                 plugin_list.append(plugi)
             else:
                 corrupted_plugin_list.append(plugi)
 
                 missing_files_count = 0
                 error = f"plugin missing "
                 if f"{plugi}.py" not in package_file_list:
                     error += f"'{plugi}.py' "
                     missing_files_count += 1
-                if "__init__.py" not in package_file_list:
-                    error += "'__init__.py' "
-                    missing_files_count += 1
                 if "METADATA" not in package_file_list:
                     error += "'METADATA' "
                     missing_files_count += 1
                 if missing_files_count != 0:
                     os.system("")
                     print(f"\033[1;31mThe {plugi} plugin is corrupted: \033[0m{error}")
```

## teelebot/version.py

```diff
@@ -1,17 +1,17 @@
 # -*- coding:utf-8 -*-
 """
-@description: A bot framework based on the Telegram Bot API
+@description: A Python-based Telegram Bot framework
 @creation date: 2019-11-15
-@last modification: 2023-05-15
+@last modification: 2023-05-29
 @author: Pluto (github:plutobell)
 """
 
-__version__ = "2.3.2"
+__version__ = "2.3.3"
 
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
-__description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
+__description__ = "teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading."
```

## Comparing `teelebot-2.3.2.dist-info/LICENSE` & `teelebot-2.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.3.2.dist-info/METADATA` & `teelebot-2.3.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.3.2
-Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
+Version: 2.3.3
+Summary: teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.3.2 Summary: teelebot is a
-robot framework based on Telegram Bot API, with plug-in system, easy to extend.
-Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
-GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
-Programming Language :: Python :: 3 Classifier: Operating System :: OS
-Independent Classifier: License :: OSI Approved :: GNU General Public License
-v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: requests
+Metadata-Version: 2.1 Name: teelebot Version: 2.3.3 Summary: teelebot is a
+Python-based Telegram Bot framework with a plugin system that supports hot
+reload and hot loading. Home-page: https://ojoll.com Author: Pluto Author-
+email: hi@ojoll.com License: GPLv3 Keywords: teelebot telegram bot telegram bot
+api telegram Classifier: Programming Language :: Python :: 3 Classifier:
+Operating System :: OS Independent Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: requests
                                     ******
                                  [./LOGO.png]
                                    teelebot
                                      ******
                           *** Pythonå®ç°çTelegram
 Botæºå¨äººæ¡æ¶ï¼å·ææä»¶ç³»ç»ï¼æä»¶æ¯æç­æ´æ°åç­è£è½½ã
                                       ***
```


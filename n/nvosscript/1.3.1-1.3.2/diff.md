# Comparing `tmp/nvosscript-1.3.1.tar.gz` & `tmp/nvosscript-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.1.tar", last modified: Fri May 19 01:33:14 2023, max compression
+gzip compressed data, was "nvosscript-1.3.2.tar", last modified: Mon May 29 08:51:58 2023, max compression
```

## Comparing `nvosscript-1.3.1.tar` & `nvosscript-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.907871 nvosscript-1.3.1/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.1/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-19 01:33:14.907712 nvosscript-1.3.1/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.1/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.902673 nvosscript-1.3.1/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.1/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13416 2023-05-19 01:32:59.000000 nvosscript-1.3.1/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.3.1/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     9021 2023-05-12 07:47:19.000000 nvosscript-1.3.1/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6172 2023-05-11 08:47:40.000000 nvosscript-1.3.1/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      985 2023-05-04 01:42:28.000000 nvosscript-1.3.1/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.904828 nvosscript-1.3.1/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      500 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-05-19 01:33:14.000000 nvosscript-1.3.1/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-05-19 01:33:14.907981 nvosscript-1.3.1/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-05-19 01:32:59.000000 nvosscript-1.3.1/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.905890 nvosscript-1.3.1/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      712 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/datahandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1797 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      240 2023-05-04 01:42:28.000000 nvosscript-1.3.1/skyeye/skyeyecommand.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.906519 nvosscript-1.3.1/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.1/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      185 2023-05-04 01:42:28.000000 nvosscript-1.3.1/start/commonUtil.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4525 2023-05-19 01:33:05.000000 nvosscript-1.3.1/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.899806 nvosscript-1.3.1/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.906692 nvosscript-1.3.1/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.1/venv/bin/activate_this.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-05-19 01:33:14.907256 nvosscript-1.3.1/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.1/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495911 nvosscript-1.3.2/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.2/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-29 08:51:58.495748 nvosscript-1.3.2/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.2/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.492034 nvosscript-1.3.2/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.2/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    13399 2023-05-29 07:40:29.000000 nvosscript-1.3.2/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8990 2023-05-29 07:40:49.000000 nvosscript-1.3.2/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6143 2023-05-29 07:41:05.000000 nvosscript-1.3.2/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.493141 nvosscript-1.3.2/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-05-29 08:51:58.000000 nvosscript-1.3.2/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-05-29 08:51:58.496017 nvosscript-1.3.2/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-05-29 07:31:27.000000 nvosscript-1.3.2/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.494119 nvosscript-1.3.2/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.2/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.2/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      778 2023-05-29 07:35:56.000000 nvosscript-1.3.2/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     2490 2023-05-29 07:45:23.000000 nvosscript-1.3.2/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495022 nvosscript-1.3.2/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.2/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1663 2023-05-29 07:39:37.000000 nvosscript-1.3.2/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-05-29 08:05:59.000000 nvosscript-1.3.2/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1157 2023-05-29 07:39:37.000000 nvosscript-1.3.2/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-05-29 08:51:58.495351 nvosscript-1.3.2/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.2/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.1/LICENSE` & `nvosscript-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.1/nvos/file.py` & `nvosscript-1.3.2/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import logging
 import json
-from nvos import remote, utils
-from start import commonUtil
+from nvos import remote
+from start import utils
 
 logger = logging.getLogger(__name__)
 
 
 # 初始化工作环境
 def init_work_space(workspace_path):
     if len(workspace_path) == 0:
@@ -31,15 +31,15 @@
     workspace_env = []
     if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
         with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
             for line in f:
                 workspace_env.append(line.strip())
     workspace_env.append(workspace_path)
     workspace_env = list(set(workspace_env))
-    commonUtil.check_local_workspace()
+    utils.check_local_workspace()
     with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'w') as f:
         for item in workspace_env:
             f.write(item + "\n")
 
     return True
```

### Comparing `nvosscript-1.3.1/nvos/login.py` & `nvosscript-1.3.2/start/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ldap3
 import os
 import json
-from nvos import utils
+from start import utils
 
 
 def login_user_check(user_name, password):
     try:
         server = ldap3.Server('ldap.fareast.nevint.com')
         conn = ldap3.Connection(server, user_name, password, client_strategy=ldap3.SAFE_SYNC, auto_bind=True)
         status, result, response, _ = conn.search('o=test', '(objectclass=*)')
```

### Comparing `nvosscript-1.3.1/nvos/remote.py` & `nvosscript-1.3.2/nvos/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import requests
 import hashlib
 import json
 import re
 import concurrent.futures
 import multiprocessing
 from tqdm import tqdm
-from nvos import login
-from start import commonUtil
+from start import utils, login
 import logging
 
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
@@ -95,17 +94,18 @@
                 if matchObj:
                     flag = True
                     break
             if not flag:
                 continue
 
             if project_space["project_space"] in file_path["file_path"]:
-                file_name = "%s/%s/%s" % (login.get_user_id(), md5(project_space["git_branch"], project_space["project_space"]),
+                file_name = "%s/%s/%s" % (
+                    login.get_user_id(), md5(project_space["git_branch"], project_space["project_space"]),
                                             file_path["file_path"][file_path["file_path"]
-                                          .find(os.path.basename(project_space["project_space"])):])
+                .find(os.path.basename(project_space["project_space"])):])
                 file_name = file_name.replace("\\", "/")
                 local_file_path = file_path["file_path"]
                 temp_file = {"local_file_path": local_file_path, "file_name": file_name}
                 upload_list.append(temp_file)
     upload_process(upload_list, bucket)
 
     file_upload_notify(workspace_path, project_space_list)
@@ -217,15 +217,15 @@
 
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
     tip = daemon_network_front_mapping.get(env)
     result = {"cloud":val,"tip":tip,"env":env}
-    commonUtil.check_local_workspace()
+    utils.check_local_workspace()
     with open(os.path.expanduser(os.path.join('~','.ndtcrc' ,'nvos_env')), 'w') as f:
         f.writelines(json.dumps(result))
     print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
```

### Comparing `nvosscript-1.3.1/nvos/run.py` & `nvosscript-1.3.2/nvos/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import subprocess
 import threading
 
-from nvos import login, file, utils, remote
-from start import commonUtil
+from nvos import file, remote
+from start import utils, login
 import os
 import time
 import logging
 import concurrent.futures
 import platform
-import json
 import shutil
 
 # 导入全局日志记录器
 logger = logging.getLogger()
 
 
 def command_init():
@@ -53,15 +52,15 @@
                 all_workspace_list.append(item.strip())
 
     all_workspace_list = set(all_workspace_list)
     if model is None or model == "start".lower():
         all_workspace_list.add(workspace_path)
     elif model == "stop".lower():
         all_workspace_list.remove(workspace_path)
-    commonUtil.check_local_workspace()
+    utils.check_local_workspace()
     with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "aync_workspace")), "w") as f:
         for item in list(all_workspace_list):
             f.write(item + '\n')
 
     if platform.system() == 'Windows':
         return
     # 在运行时执行
```

### Comparing `nvosscript-1.3.1/nvos/utils.py` & `nvosscript-1.3.2/start/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,7 +20,10 @@
             subdirectory_workspace, result = check_subdirectory_workspace_exist(os.path.join(current_path, file_name),
                                                                                 index)
             if result:
                 return subdirectory_workspace, result
     return "", False
 
 
+def check_local_workspace():
+    if not os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc'))):
+        os.mkdir(os.path.expanduser(os.path.join("~", '.ndtcrc')))
```

### Comparing `nvosscript-1.3.1/setup.py` & `nvosscript-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.1',
+    version='1.3.2',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.1/skyeye/datahandler.py` & `nvosscript-1.3.2/skyeye/loghandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import logging
+from skyeye import remote
 
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 def filter_effective_log(path):
     if path is None:
         print("please upload correct path")
         return
@@ -12,16 +13,17 @@
     logger_list = []
     if not os.path.exists(path) or os.path.isdir(path):
         print(f"{path} not exists or this path is directory,please upload a logger file ")
         return
 
     with open(path, 'r') as f:
         for line in f:
-            matchObj = re.match("\d|\d+|\d+|.*", line, re.M | re.I)
+            matchObj = re.search("\d\|\d+\|\d+\|.*", line, re.M | re.I)
             if matchObj:
                 logger_list.append(line)
 
     logger.info(f"filter logger info data is {logger_list}")
+    remote.upload_file(logger_list)
```

### Comparing `nvosscript-1.3.1/start/main.py` & `nvosscript-1.3.2/start/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This is a sample Python script.
 import os.path
 # Press ⌃R to execute it or replace it with your code.
 # Press Double ⇧ to search everywhere for classes, files, tool windows, actions, and settings.
-import sys
 import logging
 import getpass
 import argparse
 import multiprocessing
-from nvos import login, run
-from skyeye import skyeyecommand, datahandler
+from nvos import run
+from start import login
+from skyeye import handler
 
 # 创建全局记录器
 # 配置日志格式化信息
 logging.basicConfig(filename=os.path.expanduser(os.path.join('~', 'ndtc.log')), level=logging.INFO,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 logger = logging.getLogger()
 
@@ -32,19 +32,19 @@
     subparsers.add_parser('push', help='[NVOS]The push command is used upload local new files or folders to the cloud')
     subparsers.add_parser('version', help='[NVOS]The version command will tell you this script really version')
     subparsers.add_parser('path',
                           help='[NVOS]The path command will return windows service register script path, so you can '
                                'install this script for windows like async command.You need execute "pythonw '
                                'win_auto_script.py" and script is this command return path content')
     upload = subparsers.add_parser('upload', help="[NVOS,SkyEye] upload your something to cloud")
-    upload.add_argument("-m", "--module", choices=['nvos', 'skyeye'] , help="choose you want to upload module,if you don't choose, it will default to all")
+    upload.add_argument("-m", "--module", choices=['nvos', 'skyeye'], help="choose you want to upload module,if you don't choose, it will default to all")
     upload.add_argument("-l", '--log', help="input your SkeyEye log path,then we will analysis this log")
     env = subparsers.add_parser('env')
     env.add_argument('module', choices=['nvos', 'skyeye'])
-    env.add_argument('-s', '--switch', choices=['dev', 'stg', 'prod'])
+    env.add_argument('-s', '--switch', choices=['local','dev', 'stg', 'prod'])
 
     args = parser.parse_args()
 
     if args.subcommand == "login":
         username = input("email：")
         password = getpass.getpass("password：")
         status = login.login_user_check(username, password)
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.1")
+        print("1.3.2")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
@@ -75,21 +75,21 @@
             "\n\t if you still have many things you don't understand,you can take a look as https://nio.feishu.cn/wiki/wikcn9L7Di4ILQKaNmDDTrmpLqg ")
 
 
 def switch_command_env(module, switch=None):
     if module == "nvos":
         run.command_env(switch)
     elif module == "skyeye":
-        skyeyecommand.command_env(switch)
+        handler.command_env(switch)
 
 def switch_command_upload(module,log=None):
     if module == "nvos":
         run.command_upload()
     elif module == "skyeye":
-        datahandler.filter_effective_log(log)
+        handler.command_log(log)
     else:
         run.command_upload()
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `nvosscript-1.3.1/win/win_auto_script.py` & `nvosscript-1.3.2/win/win_auto_script.py`

 * *Files identical despite different names*


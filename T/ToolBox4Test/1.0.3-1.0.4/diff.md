# Comparing `tmp/ToolBox4Test-1.0.3.tar.gz` & `tmp/ToolBox4Test-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolBox4Test-1.0.3.tar", last modified: Mon May 15 14:54:11 2023, max compression
+gzip compressed data, was "dist\ToolBox4Test-1.0.4.tar", last modified: Mon May 29 13:56:34 2023, max compression
```

## Comparing `ToolBox4Test-1.0.3.tar` & `ToolBox4Test-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.999469 ToolBox4Test-1.0.3/
--rw-rw-rw-   0        0        0       90 2023-05-14 14:00:29.000000 ToolBox4Test-1.0.3/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       43 2023-05-15 14:21:35.000000 ToolBox4Test-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1397 2023-05-15 14:54:10.998788 ToolBox4Test-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.943222 ToolBox4Test-1.0.3/TestToolBox/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.956156 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/
--rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/__init__.py
--rw-rw-rw-   0        0        0    32884 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/adbShell.py
--rw-rw-rw-   0        0        0     8958 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/dataDriver.py
--rw-rw-rw-   0        0        0    15470 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/iterToolkit.py
--rw-rw-rw-   0        0        0    22709 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.3/TestToolBox/BaseUtility/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.960572 ToolBox4Test-1.0.3/TestToolBox/CaseData/
--rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.3/TestToolBox/CaseData/__init__.py
--rw-rw-rw-   0        0        0    15310 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/CaseData/generateXmind.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.981314 ToolBox4Test-1.0.3/TestToolBox/Common/
--rw-rw-rw-   0        0        0     1322 2023-05-14 12:22:11.000000 ToolBox4Test-1.0.3/TestToolBox/Common/Api_Template_Doc.yml
--rw-rw-rw-   0        0        0     4308 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/CMS_COMMON_ENUM.yml
--rw-rw-rw-   0        0        0     6107 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/CMS_Rules.yml
--rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.3/TestToolBox/Common/__init__.py
--rw-rw-rw-   0        0        0    11847 2023-05-15 14:25:10.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initConfig.py
--rw-rw-rw-   0        0        0    17339 2023-05-14 11:57:25.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initRequest.py
--rw-rw-rw-   0        0        0    11320 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initRule.py
--rw-rw-rw-   0        0        0    15112 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/Common/initUIEnv.py
--rw-rw-rw-   0        0        0      656 2023-05-14 13:12:05.000000 ToolBox4Test-1.0.3/TestToolBox/__init__.py
--rw-rw-rw-   0        0        0     3164 2023-05-14 11:53:55.000000 ToolBox4Test-1.0.3/TestToolBox/invokeFuncTrack.py
--rwxrwxrwx   0        0        0       25 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.3/TestToolBox/toolbox.bat
--rw-rw-rw-   0        0        0    25522 2023-05-14 11:21:50.000000 ToolBox4Test-1.0.3/TestToolBox/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:54:10.996792 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/
--rw-rw-rw-   0        0        0     1397 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      193 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 14:54:10.000000 ToolBox4Test-1.0.3/ToolBox4Test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      223 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 14:54:10.999469 ToolBox4Test-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3635 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/
+-rw-rw-rw-   0        0        0       91 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-05-15 14:21:35.000000 ToolBox4Test-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1397 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.085838 ToolBox4Test-1.0.4/ToolBox4Test/
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.117081 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/__init__.py
+-rw-rw-rw-   0        0        0    32883 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/adbShell.py
+-rw-rw-rw-   0        0        0     8959 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/dataDriver.py
+-rw-rw-rw-   0        0        0    15471 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/iterToolkit.py
+-rw-rw-rw-   0        0        0    22733 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.117081 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/
+-rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/__init__.py
+-rw-rw-rw-   0        0        0    15311 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/generateXmind.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/ToolBox4Test/Common/
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/__init__.py
+-rw-rw-rw-   0        0        0    12085 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initConfig.py
+-rw-rw-rw-   0        0        0    17348 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initRequest.py
+-rw-rw-rw-   0        0        0    11329 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initRule.py
+-rw-rw-rw-   0        0        0    15115 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initUIEnv.py
+-rw-rw-rw-   0        0        0      659 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/invokeFuncTrack.py
+-rw-rw-rw-   0        0        0    25527 2023-05-16 14:24:49.000000 ToolBox4Test-1.0.4/ToolBox4Test/toolbox.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.101461 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/
+-rw-rw-rw-   0        0        0     1397 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      223 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3665 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/setup.py
```

### Comparing `ToolBox4Test-1.0.3/LICENSE` & `ToolBox4Test-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.3/PKG-INFO` & `ToolBox4Test-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.3
+Version: 1.0.4
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.3/README.md` & `ToolBox4Test-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/adbShell.py` & `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/adbShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2020/11/12 10:21
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : adbShell.py
 @Describe  : Common/ 封装adb shell 命令, app操作类
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 11-12
 # 1. 
@@ -47,15 +47,15 @@
 class adbShell:
     def __init__(self, device_id=''):
         self.__system = platform.system()
         self.__find = ''
         self.__command = ''
         self.__device_id = device_id
         self.__get_find()
-        # self.__check_adb()
+        self.__check_adb()
         self.__connection_devices()
 
     def __get_find(self):
         """
         判断系统类型，windows使用findstr，linux使用grep
         :return:
         """
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/dataDriver.py` & `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/dataDriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2021/12/6 16:19
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : dataDriver.py
 @Describe  : 数据库连接
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 2021/12/6
 # 1.
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/iterToolkit.py` & `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/iterToolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2020/10/10 10:30
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : iterToolkit.py
 @Describe  : json数据迭代遍历
 ————————————————————
 @Version   : 2.1
 """
 # update   : 10-10 - ver 0.1
 # 1. 遍历/修改json
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/BaseUtility/toolkit.py` & `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2020/8/29 17:28
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : toolkit.py
 @Describe  : 工具箱 文本 数据处理
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 08-29
 # 1. 封装记录埋点数据方法,便于扩展
@@ -33,22 +33,23 @@
 
 from loguru import logger
 
 from jsonpath import jsonpath
 import yaml
 import json
 import csv
+
 # import xlrd
 # import xlwt
 # import xldate_as_tuple, xlscopy
 
-from pycallgraph import PyCallGraph
-from pycallgraph import Config
-from pycallgraph import GlobbingFilter
-from pycallgraph.output import GraphvizOutput
+# from pycallgraph import PyCallGraph
+# from pycallgraph import Config
+# from pycallgraph import GlobbingFilter
+# from pycallgraph.output import GraphvizOutput
 
 """
 # 索引数据表格
 """
 
 
 # 将变量名转换成字符串实例
@@ -86,14 +87,15 @@
     def __enter__(self):
         self.t0 = time.time()
     
     def __exit__(self, *args, **kwargs):
         print(f'CostTime: @{(time.time() - self.t0):.3f}s')
 
 
+"""
 # 上下文追踪 - with Tracker():
 class Tracker(PyCallGraph):
     def __init__(self, output_file=None):
         config = Config()
         config.trace_filter = GlobbingFilter(exclude=[
             'pycallgraph.*',
             '*.secret_function',
@@ -130,14 +132,15 @@
         file_name = f"funcTracker.{call_func_name}.{func.__name__}.png"
         graphviz = GraphvizOutput(output_file=file_name)
         with PyCallGraph(output=graphviz, config=config):
             result = func(*args, **kwargs)
         return result
     
     return track
+"""
 
 
 # 打印对象/模块所有属性值
 def getAllAttr(_module):
     module_list = dir(_module)
     length = len(module_list)
     result = {
@@ -396,15 +399,15 @@
 csv 文件数据操作
 """
 
 
 # 只在第一行写入标题,不重复
 def csvRecoder(file_name, msg, title=None, _type="w"):
     mkdir(file_name)
-    # file_name = f"{Project_Dir}/TestData/indexValueName.csv"
+    # file_name = f"{_project_dir}/TestData/indexValueName.csv"
     with open(file_name, _type, newline='', encoding="utf-8") as cfile:
         pen = csv.writer(cfile, delimiter=',')
         # 读取文件判断有无内容行
         with open(file_name, 'r', newline='') as rf:
             reader = csv.reader(rf)
             # if not [row for row in reader]:     # 写入标题
             if title:  # 写入标题
@@ -413,15 +416,15 @@
             else:
                 # for d in data:
                 pen.writerows(msg)
 
 
 # 获取数据
 def csvReader(file_name, title=True):
-    # file_name = f"{Project_Dir}/TestData/indexValueName.csv"
+    # file_name = f"{_project_dir}/TestData/indexValueName.csv"
     result = []
     with open(file_name) as cf:
         lines = cf.readlines()
         # if title:
         #     title_line = lines[0]
         #     for t in title_line:
         #         result.append(t)
@@ -495,15 +498,15 @@
     row_num = 0     # 行 cols  # 列
 
     for list_ in list_date:
         for data in list_:
             _sheet.write(row_num, list_.index(data), data)
         row_num += 1
 
-    # book.save(f"{Project_Dir}/TestData/indexValueName.xls")
+    # book.save(f"{_project_dir}/TestData/indexValueName.xls")
     book.save(index_excel)
 
 
 # 写入表格 v2.0 - 重复写入
 def xlsWrite(sheetname, list_date):
     if not os.path.exists(index_excel):
         xlsWrite_v1(sheetname, list_date)
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/CaseData/generateXmind.py` & `ToolBox4Test-1.0.4/ToolBox4Test/CaseData/generateXmind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2021/6/21 16:29
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : json2xmind.py
 @Describe  : 解析成数据格式 xmind <=> data
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 6-21
 # 1. xmind 解析
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/Common/initConfig.py` & `ToolBox4Test-1.0.4/ToolBox4Test/Common/initConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2022/1/8 22:58
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : initConfig
 @Describe  : 初始化配置参数
 ————————————————————
 @Version   : 1.0
 """
 # update   : 2022/1/8
 # 1. 接口文档转换为字典对象
@@ -26,19 +26,20 @@
 # update   :
 # 1.
 # 2.
 # ————————————————————
 import csv
 import itertools
 
-from TestToolBox import Project_Dir
 from loguru import logger
 from faker import Faker
 
-from TestToolBox.BaseUtility.toolkit import loadYaml, lazy, DictObjection, mkdir
+from ToolBox4Test.BaseUtility.toolkit import loadYaml, lazy, DictObjection, mkdir
+
+from ToolBox4Test import _project_dir
 
 
 """
 Pytest 公共配置
 """
 
 
@@ -46,15 +47,16 @@
     # id = f"{item.name}"
     id = f""
     # 判断类型
     if isinstance(fixture_value, dict):
         # 详情参数
         for key, val in fixture_value.items():
             if isinstance(val, str):
-                id = f"{id}#{key}:{val[:7]}-"
+                # id = f"{id}#{key}:{val[:7]}-"
+                id = f"{id}#{val}-"
             else:
                 id = f"{id}#{key}:{val}-"
         # 精简参数 - 仅title标识
         # for key, val in fixture_value.items():
         #     if key == "title":
         #         id = f"{id}#{key}:{val}-"
         #     else:
@@ -284,30 +286,34 @@
 """
 
 
 # demo
 def __generator(args):
     logger.debug(f"Gen start ...")
     count = 0
-    object_attr = GenDemo.api_object
+    # api_doc = f"{_project_dir}/Common/Api_Template_Doc.yml"
+    object_attr = GenDemo().api_object
     # for i in range(2):
     for key in object_attr.keys():
     
         # setattr(GenDemo, f"funcName{count}", GenDemo.getFunc(a, b, c=True))
         setattr(GenDemo, f"{object_attr.get(key).get('DESC')}", args(object_attr, key))
 
         count += 1
 
     logger.debug(f"Gen complete!")
 
 
 class GenDemo:
-    api_doc = f"{Project_Dir}/Common/Api_Template_Doc.yml"
+    api_doc = rf"{_project_dir}/Common/Api_Template_Doc.yml"
     api_object = CommonConfig(api_doc).classData
-
+    
+    # def __init__(self, file_path: str):
+    #     self.api_object = CommonConfig(file_path).classData
+        
     @staticmethod
     def getFunc(*args, **kwargs):
         def func(self):  # self 是类实例化对象
             # self.apiReqs(*args, **kwargs)
             return self.apiReqs(*args, **kwargs)
             # return CMSBasicConfig(*args, **kwargs)
 
@@ -323,17 +329,17 @@
 
 if __name__ == '__main__':
     pass
 
     """
     类属性生成器 generation
     """
-
-    # __generator(GenDemo.getFunc)  # GenApiReqs 类绑定接口方法
-    # logger.debug(dir(GenDemo()))
+    # print("a")
+    __generator(GenDemo.getFunc)  # GenApiReqs 类绑定接口方法
+    logger.debug(dir(GenDemo()))
     #
     # demo = GenDemo()
 
     """
     # 实例化 调试
     """
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/Common/initRequest.py` & `ToolBox4Test-1.0.4/ToolBox4Test/Common/initRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2022/1/10 12:01
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : initRequest.py
 @Describe  : 接口请求数据初始化 规范化
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 2022/1/10
 # 1. get、post 请求数据格式化 - 请求数据类
@@ -48,23 +48,23 @@
 from jsonpath import jsonpath
 from loguru import logger
 import random
 import re
 import requests
 from requests import Response
 
-from TestToolBox.BaseUtility.toolkit import DictObjection, Objectionary, Highlight, prettyData
+from ToolBox4Test.BaseUtility.toolkit import DictObjection, Objectionary, Highlight, prettyData
 # from BaseUtility.iterToolkit import myUpdatePro
-from TestToolBox.Common.initConfig import CommonConfig, CSVFactory
+from ToolBox4Test.Common.initConfig import CommonConfig, CSVFactory
 # flag = 0
-from TestToolBox.Common.initRule import runBizRuleCheck
+from ToolBox4Test.Common.initRule import runBizRuleCheck
 
-from TestToolBox import Project_Dir
+from ToolBox4Test import _project_dir
 
-COMMON_ENUM = CommonConfig(f"{Project_Dir}/Common/CMS_COMMON_ENUM.yml").classData
+COMMON_ENUM = CommonConfig(f"{_project_dir}/Common/CMS_COMMON_ENUM.yml").classData
 
 
 # todo 全部继承 父类 CommonConfig
 class REQS:     # 接口请求类
     
     # todo 加载接口文档后，统一校验必要字段 REQUEST RESPONSE
     # def __init__(self, api_doc: Objectionary, api_target: Union[str, list],
@@ -164,15 +164,15 @@
 
     # @lazy
     @staticmethod
     def __HEADERS(targetReqs):
         return targetReqs.HEADERS
     
     # 缓存登陆 token
-    api_cache_file = f"{Project_Dir}/TestSuite_CMS_Api/cacheData.yml"
+    api_cache_file = f"{__project_dir}/TestSuite_CMS_Api/cacheData.yml"
 
     @staticmethod
     def _updateHeaders(targetReqs, addHeaders):
         # _headers = copy.deepcopy(dict(self._HEADERS()))
         _headers = dict(targetReqs.HEADERS)
         # logger.info(f"REQS.HEADERS: {_headers}")
         if addHeaders:
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/Common/initRule.py` & `ToolBox4Test-1.0.4/ToolBox4Test/Common/initRule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2022/6/13 15:17
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : initRule.py
 @Describe  : business_rules 业务规则引擎
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 2022/6/13
 # 1. business_rules
@@ -31,29 +31,29 @@
 from business_rules.actions import BaseActions, rule_action
 from business_rules.fields import *
 from business_rules.variables import *
 
 from business_rules.engine import run
 from business_rules import run_all
 
-from TestToolBox.BaseUtility.iterToolkit import iterTarget2Keys
-from TestToolBox.BaseUtility.toolkit import DictObjection, loadYaml, get_varsname
-from TestToolBox.Common.initConfig import CSVFactory, CommonConfig
+from ToolBox4Test.BaseUtility.iterToolkit import iterTarget2Keys
+from ToolBox4Test.BaseUtility.toolkit import DictObjection, loadYaml, get_varsname
+from ToolBox4Test.Common.initConfig import CSVFactory, CommonConfig
 
-from TestToolBox import Project_Dir
+from ToolBox4Test import _project_dir
 
 
 """
 06/13 v1.5 业务规则数据筛选逻辑层 -- 随机生成合规生产计划
 """
 
 RuleMode = "Creation"     # 创造/验证模式 Creation / Validation
 
 # COMMON_ENUM = loadYaml("CMS_COMMON_ENUM.yml")
-COMMON_ENUM = CommonConfig(f"{Project_Dir}/Common/CMS_COMMON_ENUM.yml").classData
+COMMON_ENUM = CommonConfig(f"{_project_dir}/Common/CMS_COMMON_ENUM.yml").classData
 
 
 # 自定义请求参数 - 业务规则校验 - 更新接口请求模板
 class CMSContentProduceRule:
     def __init__(self):
         pass
     
@@ -143,16 +143,16 @@
     def add_assistantCoachIds(self, assistantCoachIds, results=None):
         # logger.debug(f"add_assistantCoachIds: {results}")
         # print(results, assistantCoachIds)
         self.vars.update({"assistantCoachIds": random.sample(assistantCoachIds, 1)})
 
 
 # 3 - 业务规则
-CMS_Rules = CommonConfig(f"{Project_Dir}/Common/CMS_Rules.yml").classData
-# producePlan_rule = loadYaml(f"{Project_Dir}/Common/CMS_Rules.yml").get("producePlan_rule")
+CMS_Rules = CommonConfig(f"{_project_dir}/Common/CMS_Rules.yml").classData
+# producePlan_rule = loadYaml(f"{_project_dir}/Common/CMS_Rules.yml").get("producePlan_rule")
 CMS_Content_Rule = CMS_Rules.CMS_Content_Rule
 # producePlan_rule = CMS_Rules.producePlan_rule
 
 
 # 加载枚举值 随机组合
 def genRandomData():
     logger.info("加载枚举值 随机组合")
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/Common/initUIEnv.py` & `ToolBox4Test-1.0.4/ToolBox4Test/Common/initUIEnv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2020/11/11 22:38
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : initUIEnv.py
 @Describe  : 环境准备
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 11-11 基础环境准备
 # 1. todo 测试环境准备
@@ -26,16 +26,16 @@
 # update   :
 # 1.
 # ————————————————————
 
 
 from loguru import logger
 
-from TestToolBox.BaseUtility.adbShell import adbShell
-from TestToolBox.Common.initConfig import CommonConfig
+from ToolBox4Test.BaseUtility.adbShell import adbShell
+from ToolBox4Test.Common.initConfig import CommonConfig
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 
 
 """
 # 原生 selenium remote-debug 调试
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/__init__.py` & `ToolBox4Test-1.0.4/ToolBox4Test/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2021/6/9 09:40
 @Contact   : wen.guo@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : __init__.py.py
 @Describe  : TestToolbox 测试工具箱 | 辅助快速测试与验证
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 
 # 1. 
@@ -20,10 +20,10 @@
 # 2. 
 # ————————————————————
 
 import os
 import sys
 
 
-Project_Dir = os.path.dirname(os.path.abspath(__file__))
-sys.path.append(Project_Dir)
+_project_dir = os.path.dirname(os.path.abspath(__file__))
+sys.path.append(_project_dir)
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/invokeFuncTrack.py` & `ToolBox4Test-1.0.4/ToolBox4Test/invokeFuncTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: UTF-8 -*- 
 """   
 @Author    : Gavin
 @DateTime  : 2020/8/20 11:01
 @Contact   : wen.guo@dmall.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : invokeFuncTrack.py
 @Describe  : 
 ————————————————————
 @Version   : 0.1 
 """
 # update   : 
 # 1.项目内路径使用绝对路径(配置文件中同一调用)
```

### Comparing `ToolBox4Test-1.0.3/TestToolBox/toolbox.py` & `ToolBox4Test-1.0.4/ToolBox4Test/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
 import json
 import yaml
 from jsonpath import jsonpath
 
 
 # 相对路径
-# Project_Dir = os.path.dirname(os.path.abspath(__file__))
-# sys.path.append(Project_Dir)
+# _project_dir = os.path.dirname(os.path.abspath(__file__))
+# sys.path.append(_project_dir)
 
 # globalSetting暂存
 # do 项目全局配置 do 相对路径
-# Project_Dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+# _project_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 #
-# if os.path.relpath(Project_Dir) != ".":
+# if os.path.relpath(_project_dir) != ".":
 #     os.chdir("../")
 
 """
 Base - 基础录入数据处理
 """
 
 
@@ -693,15 +693,15 @@
         tips("未匹配,请重新选择工具模式!")
         main()
 
 
 if __name__ == '__main__':
     pass
     
-    # print(Project_Dir)
+    # print(_project_dir)
     
     # 循环
     # while True:
     #     pprintJson()
     
     # pprintJson()
```

### Comparing `ToolBox4Test-1.0.3/ToolBox4Test.egg-info/PKG-INFO` & `ToolBox4Test-1.0.4/ToolBox4Test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.3
+Version: 1.0.4
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.3/setup.py` & `ToolBox4Test-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 
     Test Toolbox | 测试工具箱 by Gavin
     
 @Author    : Gavin
 @DateTime  : 2021/6/9 09:56
 @Contact   : guowenwhy@foxmail.com
 
-@Project   : TestToolBox
+@Project   : ToolBox4Test
 @File      : setup.py
 @Describe  : TestToolbox 测试工具箱 | 辅助快速测试与验证
 ————————————————————
 @Version   : 1.0.1
 """
 # update   : 0.1 调试
 # 1. python setup.py develop
 # 2. python setup.py sdist bdist_wheel
 # ————————————————————
 # update   : 05/14
-# 1. python setup.py sdist upload
-# 2. 
+# 1. python setup.py sdist upload -- dis
+# 2. twine upload dist/*
 # ————————————————————
 # update   :
 # 1.
 # 2.
 # ————————————————————
 
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ToolBox4Test",
-    version="1.0.3",
+    version="1.0.4",
     author="Gavin",
     author_email="guowenwhy@foxmail.com",
     description="TestToolbox 测试工具箱",
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     # 项目主页
@@ -54,30 +54,30 @@
     
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
     include_package_data=True,
     
     entry_points={
             'console_scripts': [
-                'testbox = TestToolBox.toolbox:main'
+                'testbox = ToolBox4Test.toolbox:main'
             ]
         },
     
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
     ],
     
     install_requires=[
         'pyyaml>=6.0',
         'jsonpath>=0.82',
-        'pycallgraph>=1.0.1',
+        # 'pycallgraph>=1.0.1',
         'pytest>=7.1.2',
         'selenium>=4.9.0',
         'faker>=13.3.2',
         'requests>=2.29.0',
         'xmind>=1.2.0',
         'loguru>=0.5.3',
         'pymysql>=1.0.2',
```


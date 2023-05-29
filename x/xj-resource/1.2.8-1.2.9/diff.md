# Comparing `tmp/xj_resource-1.2.8.tar.gz` & `tmp/xj_resource-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xj_resource-1.2.8.tar", last modified: Fri Sep  2 03:50:47 2022, max compression
+gzip compressed data, was "dist\xj_resource-1.2.9.tar", last modified: Thu Sep  8 09:37:24 2022, max compression
```

## Comparing `xj_resource-1.2.8.tar` & `xj_resource-1.2.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.948836 xj_resource-1.2.8/
--rw-rw-rw-   0        0        0     5199 2022-09-02 03:50:47.945835 xj_resource-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2022-08-02 03:38:20.000000 xj_resource-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2022-09-02 03:50:47.948836 xj_resource-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1965 2022-09-02 03:49:37.000000 xj_resource-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.794827 xj_resource-1.2.8/xj_resource/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/__init__.py
--rw-rw-rw-   0        0        0     3050 2022-09-02 03:49:14.000000 xj_resource-1.2.8/xj_resource/admin.py
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.841830 xj_resource-1.2.8/xj_resource/apis/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/apis/__init__.py
--rw-rw-rw-   0        0        0      884 2022-08-30 09:17:31.000000 xj_resource-1.2.8/xj_resource/apis/resource_image_list.py
--rw-rw-rw-   0        0        0     2578 2022-08-30 09:11:35.000000 xj_resource-1.2.8/xj_resource/apis/resource_upload_file.py
--rw-rw-rw-   0        0        0     2749 2022-08-29 12:52:54.000000 xj_resource-1.2.8/xj_resource/apis/resource_upload_image.py
--rw-rw-rw-   0        0        0     2596 2022-08-30 09:17:31.000000 xj_resource-1.2.8/xj_resource/apis/resource_upload_video.py
--rw-rw-rw-   0        0        0      217 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/apps.py
--rw-rw-rw-   0        0        0     1024 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/config.py
--rw-rw-rw-   0        0        0    10081 2022-09-02 03:49:14.000000 xj_resource-1.2.8/xj_resource/models.py
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.885832 xj_resource-1.2.8/xj_resource/services/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/services/__init__.py
--rw-rw-rw-   0        0        0     2988 2022-08-30 09:17:31.000000 xj_resource-1.2.8/xj_resource/services/resource_file_service.py
--rw-rw-rw-   0        0        0     3289 2022-09-02 03:48:53.000000 xj_resource-1.2.8/xj_resource/services/resource_image_service.py
--rw-rw-rw-   0        0        0    13612 2022-08-30 09:11:35.000000 xj_resource-1.2.8/xj_resource/services/resource_upload_service.py
--rw-rw-rw-   0        0        0     2237 2022-08-30 09:17:31.000000 xj_resource-1.2.8/xj_resource/services/resource_video_service.py
--rw-rw-rw-   0        0        0     5365 2022-08-29 01:20:00.000000 xj_resource-1.2.8/xj_resource/services/upload_file_service [赵向明2022.8.26以前].py
--rw-rw-rw-   0        0        0     4503 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/services/upload_file_service [赵向明7.31以前].py
--rw-rw-rw-   0        0        0     4279 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/services/upload_image_service [赵向明7.31以前].py
--rw-rw-rw-   0        0        0      875 2022-08-30 09:11:35.000000 xj_resource-1.2.8/xj_resource/urls.py
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.939835 xj_resource-1.2.8/xj_resource/utils/
--rw-rw-rw-   0        0        0        0 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/__init__.py
--rw-rw-rw-   0        0        0      450 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/check_type.py
--rw-rw-rw-   0        0        0     1428 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/custom_response.py
--rw-rw-rw-   0        0        0     2063 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/digit_algorithm.py
--rw-rw-rw-   0        0        0     1911 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/excel_operate.py
--rw-rw-rw-   0        0        0      276 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/file_operate.py
--rw-rw-rw-   0        0        0      988 2022-08-29 11:14:18.000000 xj_resource-1.2.8/xj_resource/utils/j_config.py
--rw-rw-rw-   0        0        0      429 2022-08-29 11:14:18.000000 xj_resource-1.2.8/xj_resource/utils/j_dict.py
--rw-rw-rw-   0        0        0     7090 2022-08-25 01:23:30.000000 xj_resource-1.2.8/xj_resource/utils/model_handle.py
--rw-rw-rw-   0        0        0     1360 2022-08-02 03:36:27.000000 xj_resource-1.2.8/xj_resource/utils/validate.py
-drwxrwxrwx   0        0        0        0 2022-09-02 03:50:47.814828 xj_resource-1.2.8/xj_resource.egg-info/
--rw-rw-rw-   0        0        0     5199 2022-09-02 03:50:47.000000 xj_resource-1.2.8/xj_resource.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1233 2022-09-02 03:50:47.000000 xj_resource-1.2.8/xj_resource.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-02 03:50:47.000000 xj_resource-1.2.8/xj_resource.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-09-02 03:50:47.000000 xj_resource-1.2.8/xj_resource.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/
+-rw-rw-rw-   0        0        0     5199 2022-09-08 09:37:24.000000 xj_resource-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2022-08-09 06:45:37.000000 xj_resource-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-08 09:37:24.000000 xj_resource-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1965 2022-09-08 09:36:25.000000 xj_resource-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource/
+-rw-rw-rw-   0        0        0        0 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/__init__.py
+-rw-rw-rw-   0        0        0     3050 2022-09-06 01:56:38.000000 xj_resource-1.2.9/xj_resource/admin.py
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource/apis/
+-rw-rw-rw-   0        0        0        0 2022-07-31 11:32:37.000000 xj_resource-1.2.9/xj_resource/apis/__init__.py
+-rw-rw-rw-   0        0        0      884 2022-08-30 09:05:48.000000 xj_resource-1.2.9/xj_resource/apis/resource_image_list.py
+-rw-rw-rw-   0        0        0     2578 2022-08-30 08:28:32.000000 xj_resource-1.2.9/xj_resource/apis/resource_upload_file.py
+-rw-rw-rw-   0        0        0     2749 2022-08-30 09:15:45.000000 xj_resource-1.2.9/xj_resource/apis/resource_upload_image.py
+-rw-rw-rw-   0        0        0     2596 2022-08-30 08:24:43.000000 xj_resource-1.2.9/xj_resource/apis/resource_upload_video.py
+-rw-rw-rw-   0        0        0      235 2022-09-06 01:56:38.000000 xj_resource-1.2.9/xj_resource/apps.py
+-rw-rw-rw-   0        0        0     1024 2022-07-31 11:32:37.000000 xj_resource-1.2.9/xj_resource/config.py
+-rw-rw-rw-   0        0        0    10081 2022-09-06 01:56:38.000000 xj_resource-1.2.9/xj_resource/models.py
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource/services/
+-rw-rw-rw-   0        0        0        0 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/services/__init__.py
+-rw-rw-rw-   0        0        0     2988 2022-08-30 08:21:02.000000 xj_resource-1.2.9/xj_resource/services/resource_file_service.py
+-rw-rw-rw-   0        0        0     3289 2022-09-06 01:56:38.000000 xj_resource-1.2.9/xj_resource/services/resource_image_service.py
+-rw-rw-rw-   0        0        0    13691 2022-09-08 09:36:12.000000 xj_resource-1.2.9/xj_resource/services/resource_upload_service.py
+-rw-rw-rw-   0        0        0     2237 2022-08-30 08:10:44.000000 xj_resource-1.2.9/xj_resource/services/resource_video_service.py
+-rw-rw-rw-   0        0        0     5365 2022-08-28 03:57:47.000000 xj_resource-1.2.9/xj_resource/services/upload_file_service [赵向明2022.8.26以前].py
+-rw-rw-rw-   0        0        0     4503 2022-07-31 11:32:37.000000 xj_resource-1.2.9/xj_resource/services/upload_file_service [赵向明7.31以前].py
+-rw-rw-rw-   0        0        0     4279 2022-07-31 11:32:37.000000 xj_resource-1.2.9/xj_resource/services/upload_image_service [赵向明7.31以前].py
+-rw-rw-rw-   0        0        0      875 2022-08-30 09:15:45.000000 xj_resource-1.2.9/xj_resource/urls.py
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/utils/__init__.py
+-rw-rw-rw-   0        0        0      450 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/utils/check_type.py
+-rw-rw-rw-   0        0        0     1428 2022-07-19 09:24:10.000000 xj_resource-1.2.9/xj_resource/utils/custom_response.py
+-rw-rw-rw-   0        0        0     2075 2022-09-08 09:31:24.000000 xj_resource-1.2.9/xj_resource/utils/digit_algorithm.py
+-rw-rw-rw-   0        0        0     1911 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/utils/excel_operate.py
+-rw-rw-rw-   0        0        0      276 2022-05-26 09:37:45.000000 xj_resource-1.2.9/xj_resource/utils/file_operate.py
+-rw-rw-rw-   0        0        0      988 2022-08-26 05:29:25.000000 xj_resource-1.2.9/xj_resource/utils/j_config.py
+-rw-rw-rw-   0        0        0      429 2022-08-26 02:38:16.000000 xj_resource-1.2.9/xj_resource/utils/j_dict.py
+-rw-rw-rw-   0        0        0     7090 2022-08-09 06:45:58.000000 xj_resource-1.2.9/xj_resource/utils/model_handle.py
+-rw-rw-rw-   0        0        0     1360 2022-07-06 10:14:59.000000 xj_resource-1.2.9/xj_resource/utils/validate.py
+drwxrwxrwx   0        0        0        0 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource.egg-info/
+-rw-rw-rw-   0        0        0     5199 2022-09-08 09:37:23.000000 xj_resource-1.2.9/xj_resource.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1233 2022-09-08 09:37:24.000000 xj_resource-1.2.9/xj_resource.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-08 09:37:23.000000 xj_resource-1.2.9/xj_resource.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2022-09-08 09:37:23.000000 xj_resource-1.2.9/xj_resource.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `xj_resource-1.2.8/PKG-INFO` & `xj_resource-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_resource
-Version: 1.2.8
+Version: 1.2.9
 Summary: 资源模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # 模块介绍
         
         ## 1.资源上传
```

### Comparing `xj_resource-1.2.8/README.md` & `xj_resource-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/setup.py` & `xj_resource-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_resource',  # 模块名称
-    version='1.2.8',  # 模块版本
+    version='1.2.9',  # 模块版本
     description='资源模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_user'],  # 系指定安装模块
     license="apache 3.0",
```

### Comparing `xj_resource-1.2.8/xj_resource/admin.py` & `xj_resource-1.2.9/xj_resource/admin.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/apis/resource_image_list.py` & `xj_resource-1.2.9/xj_resource/apis/resource_image_list.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/apis/resource_upload_file.py` & `xj_resource-1.2.9/xj_resource/apis/resource_upload_file.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/apis/resource_upload_image.py` & `xj_resource-1.2.9/xj_resource/apis/resource_upload_image.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/apis/resource_upload_video.py` & `xj_resource-1.2.9/xj_resource/apis/resource_upload_video.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/config.py` & `xj_resource-1.2.9/xj_resource/config.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/models.py` & `xj_resource-1.2.9/xj_resource/models.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/resource_file_service.py` & `xj_resource-1.2.9/xj_resource/services/resource_file_service.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/resource_image_service.py` & `xj_resource-1.2.9/xj_resource/services/resource_image_service.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/resource_upload_service.py` & `xj_resource-1.2.9/xj_resource/services/resource_upload_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding=utf-8
 import base64
 import hashlib
 import os
 from pathlib import Path
+import random
 import re
 import time
 
 from main.settings import BASE_DIR
 from ..models import ResourceImageGroup
 from ..utils.digit_algorithm import DigitAlgorithm
 from ..utils.j_config import JConfig
 from ..utils.j_dict import JDict
 
 module_dir = Path(__file__).parent.parent
 root_config = JDict(JConfig.get_section(str(BASE_DIR) + '/config.ini', 'xj_resource', encode='utf-8-sig'))
 module_config = JDict(JConfig.get_section(str(module_dir) + '/config.ini', 'xj_resource', encode='utf-8-sig'))
-
 if not BASE_DIR:
     print("MSA ERROR: BASE_DIR is not find, check setting.py please!")
 
+
 class ResourceUploadService:
     """
     @class 资源上传服务。
     @description 该服务只提供文件上传和生成信息，不提供数据库写入！
     """
     # 公共成员，基本数据
     user_id = None  # 用户ID
@@ -185,32 +186,35 @@
         # 一检查文件名。
         self.origin_filename = self.__input_file.name
         ret = re.search(r'(.*)\.(\w{3,5})$', self.__input_file.name)
         if not ret:
             return None, '上传的文件名错误，格式后辍应为3-5个字符'
         self.origin_title = ret.group(1)
         self.suffix = ret.group(2)
-        self.filename = f"{self.__upload_prefix}{DigitAlgorithm.make_unicode_16()}.{self.suffix}"
+
+        # 三检查文件流
+        self.__file_stream = self.__input_file.read()
+        if not self.__file_stream:
+            return None, '文件流读取失败'
+        self.md5 = self.get_md5()
+
+        # 生成唯一的文件名
+        self.filename = f"{self.__upload_prefix}{DigitAlgorithm.make_unicode_16(self.md5)}.{self.suffix}"
         # 注：添加对多余路径分隔符/\检查
         self.__save_absolute_file_path = re.sub(r"[/\\]{1,3}", "/", f"{str(BASE_DIR)}/{self.save_dir}/{self.filename}")
         if self.__upload_absolute_dir:
             self.__save_absolute_file_path = re.sub(r"[/\\]{1,3}", "/", f"{self.__upload_absolute_dir}/{self.filename}")
         # print("> init_file: save_absolute_dir:", self.save_absolute_dir)
 
         # 二检查文件格式。注：添加多余空格检查
         # print("> init_file __upload_format_list:", self.__upload_formats.replace(' ', '').split(","))
         if self.__upload_formats and self.__upload_formats.strip() != '*' and self.suffix \
                 and self.suffix not in self.__upload_formats.replace(' ', '').split(","):
             return None, '上传文件格式错误，支持：' + self.__upload_formats
 
-        # 三检查文件流
-        self.__file_stream = self.__input_file.read()
-        if not self.__file_stream:
-            return None, '文件流读取失败'
-
         # 四检查文件大小
         self.size = size = len(self.__file_stream)
         # print("> init_file: __file_stream", type(self.__file_stream), size)
         if size == 0:
             return None, "空文件"
         if self.__upload_limit and size > self.__upload_limit:
             return None, f"文件大小超过限制，不应大于{self.__upload_limit}字节。"
@@ -224,15 +228,15 @@
         self.__file_info['user_id'] = self.user_id
         self.__file_info['title'] = self.title = file_title if file_title else self.origin_title
         self.__file_info['filename'] = self.filename
         self.__file_info['url'] = self.url = f"{self.__upload_host}{self.pseudo_dir}{self.filename}"
         self.__file_info['format'] = self.suffix
         self.__file_info['size'] = self.size
         self.__file_info['thumb'] = None
-        self.__file_info['md5'] = self.md5 = self.get_md5()
+        self.__file_info['md5'] = self.md5
         self.__file_info['snapshot'] = {
             'origin_filename': self.origin_filename,
             'upload_host': self.__upload_host,  # 当代码移植后，域名发生变化，可以通过上传主机查找替换为新主机
             'upload_url': self.__upload_url,  # 上传的地址,由配置产生的伪URL，不含文件夹分组的目录
             'pseudo_dir': self.pseudo_dir,  # 当代码移植后，引用伪目录发生变化，可以通过伪目录替换为新伪目录
             'save_dir': self.save_dir,  # TODO 建议不放快照，因为大部分情况下，并不希望用户看到文件存放的真实路径
             'save_absolute_dir': self.__save_absolute_dir,  # TODO 建议不放快照，真实绝对路径
```

### Comparing `xj_resource-1.2.8/xj_resource/services/resource_video_service.py` & `xj_resource-1.2.9/xj_resource/services/resource_video_service.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/upload_file_service [赵向明2022.8.26以前].py` & `xj_resource-1.2.9/xj_resource/services/upload_file_service [赵向明2022.8.26以前].py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/upload_file_service [赵向明7.31以前].py` & `xj_resource-1.2.9/xj_resource/services/upload_file_service [赵向明7.31以前].py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/services/upload_image_service [赵向明7.31以前].py` & `xj_resource-1.2.9/xj_resource/services/upload_image_service [赵向明7.31以前].py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/urls.py` & `xj_resource-1.2.9/xj_resource/urls.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/utils/custom_response.py` & `xj_resource-1.2.9/xj_resource/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/utils/digit_algorithm.py` & `xj_resource-1.2.9/xj_resource/utils/digit_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         # 当前时间戳
         timestamp = str(int(time.time()))
         # 截取第3位到第10位
         timestamp_code = timestamp[2:10]
 
         # 十六进制校验码
-        crc_hex = Jt.crc16(salt) if salt else '0'
+        crc_hex = DigitAlgorithm.crc16(salt) if salt else '0'
         # 十六进制转十进制
         crc_int = int(crc_hex, 16)
         # 头位补0
         crc_code = str('000000' + str(crc_int))[-6:]
         unicode = year_code + timestamp_code + crc_code
 
         return unicode
```

### Comparing `xj_resource-1.2.8/xj_resource/utils/excel_operate.py` & `xj_resource-1.2.9/xj_resource/utils/excel_operate.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/utils/j_config.py` & `xj_resource-1.2.9/xj_resource/utils/j_config.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/utils/model_handle.py` & `xj_resource-1.2.9/xj_resource/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource/utils/validate.py` & `xj_resource-1.2.9/xj_resource/utils/validate.py`

 * *Files identical despite different names*

### Comparing `xj_resource-1.2.8/xj_resource.egg-info/PKG-INFO` & `xj_resource-1.2.9/xj_resource.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-resource
-Version: 1.2.8
+Version: 1.2.9
 Summary: 资源模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # 模块介绍
         
         ## 1.资源上传
```

### Comparing `xj_resource-1.2.8/xj_resource.egg-info/SOURCES.txt` & `xj_resource-1.2.9/xj_resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*


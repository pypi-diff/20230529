# Comparing `tmp/movies-download-0.0.1.tar.gz` & `tmp/movies-download-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\workspace\movies\dist\.tmp-dxoi7aa9\movies-download-0.0.1.tar", last modified: Mon May 29 07:13:18 2023, max compression
+gzip compressed data, was "D:\workspace\movies\dist\.tmp-hjsririk\movies-download-0.0.2.tar", last modified: Mon May 29 07:50:05 2023, max compression
```

## Comparing `movies-download-0.0.1.tar` & `movies-download-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:13:18.827175 movies-download-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-05-29 06:58:59.000000 movies-download-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      874 2023-05-29 07:13:18.827175 movies-download-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-29 07:03:17.000000 movies-download-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:13:18.827175 movies-download-0.0.1/get_it/
--rw-rw-rw-   0        0        0        0 2023-05-29 06:27:46.000000 movies-download-0.0.1/get_it/__init__.py
--rw-rw-rw-   0        0        0    10340 2023-05-29 06:25:23.000000 movies-download-0.0.1/get_it/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:13:18.827175 movies-download-0.0.1/movies_download.egg-info/
--rw-rw-rw-   0        0        0      874 2023-05-29 07:13:18.000000 movies-download-0.0.1/movies_download.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-29 07:13:18.000000 movies-download-0.0.1/movies_download.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:13:18.000000 movies-download-0.0.1/movies_download.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 07:13:18.000000 movies-download-0.0.1/movies_download.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2023-05-29 07:12:58.000000 movies-download-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 07:13:18.827175 movies-download-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      524 2023-05-29 06:44:55.000000 movies-download-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:50:05.754719 movies-download-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-05-29 06:58:59.000000 movies-download-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1065 2023-05-29 07:50:05.754719 movies-download-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-29 07:47:23.000000 movies-download-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 07:50:05.754719 movies-download-0.0.2/movies_download/
+-rw-rw-rw-   0        0        0        0 2023-05-29 06:27:46.000000 movies-download-0.0.2/movies_download/__init__.py
+-rw-rw-rw-   0        0        0    10340 2023-05-29 06:25:23.000000 movies-download-0.0.2/movies_download/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:50:05.754719 movies-download-0.0.2/movies_download.egg-info/
+-rw-rw-rw-   0        0        0     1065 2023-05-29 07:50:05.000000 movies-download-0.0.2/movies_download.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-29 07:50:05.000000 movies-download-0.0.2/movies_download.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:50:05.000000 movies-download-0.0.2/movies_download.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 07:50:05.000000 movies-download-0.0.2/movies_download.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2023-05-29 07:49:55.000000 movies-download-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:50:05.754719 movies-download-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      531 2023-05-29 07:49:55.000000 movies-download-0.0.2/setup.py
```

### Comparing `movies-download-0.0.1/LICENSE` & `movies-download-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `movies-download-0.0.1/PKG-INFO` & `movies-download-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: movies-download
-Version: 0.0.1
+Version: 0.0.2
 Summary: 视频下载助手
-Home-page: https://github.com/gituser/test-tackage
+Home-page: https://gitee.com/cgq/movies-download
 Author: 碧海苍鹰
 Author-email: 碧海苍鹰 <348249063@qq.com>
 License: MIT
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://gitee.com/cgq/movies-download
+Project-URL: Bug Tracker, https://gitee.com/cgq/movies-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 自由行
 一个下载电影的助手。
+方便下载m3u8格式的视频文件。
+
+# 使用方法
+请自行研究。
 
 # 打包程序
+
+## 安装打包工具
 ```shell
 python -m pip install --upgrade build
+```
+## 创建配置文件后, 开始打包，执行下面的命令
+```shell
 python -m build
+```
+
+## 安装上传工具并上传到PyPI，执行下面的命令
+```shell
 python -m pip install --upgrade twine
-python -m twine upload --repository testpypi dist/*
-python -m twine upload --repository pypi dist/*
+python -m twine upload dist/*
 ```
```

### Comparing `movies-download-0.0.1/get_it/main.py` & `movies-download-0.0.2/movies_download/main.py`

 * *Files identical despite different names*

### Comparing `movies-download-0.0.1/movies_download.egg-info/PKG-INFO` & `movies-download-0.0.2/movies_download.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: movies-download
-Version: 0.0.1
+Version: 0.0.2
 Summary: 视频下载助手
-Home-page: https://github.com/gituser/test-tackage
+Home-page: https://gitee.com/cgq/movies-download
 Author: 碧海苍鹰
 Author-email: 碧海苍鹰 <348249063@qq.com>
 License: MIT
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://gitee.com/cgq/movies-download
+Project-URL: Bug Tracker, https://gitee.com/cgq/movies-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 自由行
 一个下载电影的助手。
+方便下载m3u8格式的视频文件。
+
+# 使用方法
+请自行研究。
 
 # 打包程序
+
+## 安装打包工具
 ```shell
 python -m pip install --upgrade build
+```
+## 创建配置文件后, 开始打包，执行下面的命令
+```shell
 python -m build
+```
+
+## 安装上传工具并上传到PyPI，执行下面的命令
+```shell
 python -m pip install --upgrade twine
-python -m twine upload --repository testpypi dist/*
-python -m twine upload --repository pypi dist/*
+python -m twine upload dist/*
 ```
```

### Comparing `movies-download-0.0.1/pyproject.toml` & `movies-download-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "movies-download"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="碧海苍鹰", email="348249063@qq.com" },
 ]
 description = "视频下载助手"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://gitee.com/cgq/movies-download"
+"Bug Tracker" = "https://gitee.com/cgq/movies-download/issues"
```

### Comparing `movies-download-0.0.1/setup.py` & `movies-download-0.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     description = fh.read()
 
 setuptools.setup(
     name="movies-download",
-    version="0.0.1",
+    version="0.0.2",
     author="碧海苍鹰",
     author_email="348249063@qq.com",
-    packages=["get_it"],
+    packages=["movies_download"],
     description="视频下载助手",
     long_description=description,
     long_description_content_type="text/markdown",
-    url="https://github.com/gituser/test-tackage",
+    url="https://gitee.com/cgq/movies-download",
     license='MIT',
     python_requires='>=3.8',
     install_requires=[]
 )
```


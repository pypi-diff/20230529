# Comparing `tmp/pyxbox-0.1.2.tar.gz` & `tmp/pyxbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxbox-0.1.2.tar", last modified: Sun May 28 14:27:13 2023, max compression
+gzip compressed data, was "pyxbox-0.1.3.tar", last modified: Mon May 29 13:59:52 2023, max compression
```

## Comparing `pyxbox-0.1.2.tar` & `pyxbox-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 14:27:13.973424 pyxbox-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-05-28 05:11:25.000000 pyxbox-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1245 2023-05-28 14:27:13.972422 pyxbox-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-05-28 13:53:58.000000 pyxbox-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 14:27:13.951683 pyxbox-0.1.2/pyxbox/
--rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 14:27:13.970726 pyxbox-0.1.2/pyxbox/bilibili_utils/
--rw-rw-rw-   0        0        0      344 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/ApiException.py
--rw-rw-rw-   0        0        0     5113 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/BytesReader.py
--rw-rw-rw-   0        0        0     2218 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/Color.py
--rw-rw-rw-   0        0        0     3382 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/Danmaku.py
--rw-rw-rw-   0        0        0      337 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/DanmakuClosedException.py
--rw-rw-rw-   0        0        0      378 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/ResponseException.py
--rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/__init__.py
--rw-rw-rw-   0        0        0     3667 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/utils.py
--rw-rw-rw-   0        0        0      598 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/bilibili_utils/varint.py
--rw-rw-rw-   0        0        0     4127 2023-05-28 14:18:31.000000 pyxbox-0.1.2/pyxbox/media.py
--rw-rw-rw-   0        0        0    10266 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/proxies.py
--rw-rw-rw-   0        0        0    79745 2023-05-28 07:23:35.000000 pyxbox-0.1.2/pyxbox/tools.py
--rw-rw-rw-   0        0        0    42825 2023-05-28 05:11:25.000000 pyxbox-0.1.2/pyxbox/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-05-28 14:27:13.958115 pyxbox-0.1.2/pyxbox.egg-info/
--rw-rw-rw-   0        0        0     1245 2023-05-28 14:27:13.000000 pyxbox-0.1.2/pyxbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-05-28 14:27:13.000000 pyxbox-0.1.2/pyxbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 14:27:13.000000 pyxbox-0.1.2/pyxbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-28 14:27:13.000000 pyxbox-0.1.2/pyxbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 14:27:13.000000 pyxbox-0.1.2/pyxbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 14:27:13.973424 pyxbox-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-05-28 13:46:43.000000 pyxbox-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:59:52.782684 pyxbox-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-28 05:11:25.000000 pyxbox-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1392 2023-05-29 13:59:52.770871 pyxbox-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1136 2023-05-29 13:58:49.000000 pyxbox-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 13:59:52.751086 pyxbox-0.1.3/pyxbox/
+-rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:59:52.769874 pyxbox-0.1.3/pyxbox/bilibili_utils/
+-rw-rw-rw-   0        0        0      344 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/ApiException.py
+-rw-rw-rw-   0        0        0     5113 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/BytesReader.py
+-rw-rw-rw-   0        0        0     2218 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/Color.py
+-rw-rw-rw-   0        0        0     3382 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/Danmaku.py
+-rw-rw-rw-   0        0        0      337 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/DanmakuClosedException.py
+-rw-rw-rw-   0        0        0      378 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/ResponseException.py
+-rw-rw-rw-   0        0        0      232 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/utils.py
+-rw-rw-rw-   0        0        0      598 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/bilibili_utils/varint.py
+-rw-rw-rw-   0        0        0     2963 2023-05-29 13:28:13.000000 pyxbox-0.1.3/pyxbox/mail.py
+-rw-rw-rw-   0        0        0     4127 2023-05-28 14:18:31.000000 pyxbox-0.1.3/pyxbox/media.py
+-rw-rw-rw-   0        0        0    10266 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/proxies.py
+-rw-rw-rw-   0        0        0    79745 2023-05-28 07:23:35.000000 pyxbox-0.1.3/pyxbox/tools.py
+-rw-rw-rw-   0        0        0    42825 2023-05-28 05:11:25.000000 pyxbox-0.1.3/pyxbox/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:59:52.758899 pyxbox-0.1.3/pyxbox.egg-info/
+-rw-rw-rw-   0        0        0     1392 2023-05-29 13:59:52.000000 pyxbox-0.1.3/pyxbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-05-29 13:59:52.000000 pyxbox-0.1.3/pyxbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 13:59:52.000000 pyxbox-0.1.3/pyxbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-29 13:59:52.000000 pyxbox-0.1.3/pyxbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 13:59:52.000000 pyxbox-0.1.3/pyxbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 13:59:52.782684 pyxbox-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-05-29 01:31:55.000000 pyxbox-0.1.3/setup.py
```

### Comparing `pyxbox-0.1.2/LICENSE` & `pyxbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/PKG-INFO` & `pyxbox-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbox
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://gitee.com/spider-x/pyxbox
 Author: BruceLong
 Author-email: 18656170559@163.com
 License: MIT Licence
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,14 +47,18 @@
 
 #### user_agent
 - 请求头：user-agent库
 
 #### proxies
 - 代理相关模块封装
 
+#### mail
+##### EmailSender
+> 邮件发送工具，不用再写太多冗余的代码只需要简单的几行代码即可批量发送内容。
+
 ## 安装教程
 
 1. 安装：`pip install pyxbox`
 2. 更新：`pip install -U pyxbox`
 3. 卸载：`pip uninstall pyxbox`
 
 ## 使用说明
```

### Comparing `pyxbox-0.1.2/README.md` & `pyxbox-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 
 #### user_agent
 - 请求头：user-agent库
 
 #### proxies
 - 代理相关模块封装
 
+#### mail
+##### EmailSender
+> 邮件发送工具，不用再写太多冗余的代码只需要简单的几行代码即可批量发送内容。
+
 ## 安装教程
 
 1. 安装：`pip install pyxbox`
 2. 更新：`pip install -U pyxbox`
 3. 卸载：`pip uninstall pyxbox`
 
 ## 使用说明
```

### Comparing `pyxbox-0.1.2/pyxbox/bilibili_utils/BytesReader.py` & `pyxbox-0.1.3/pyxbox/bilibili_utils/BytesReader.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/bilibili_utils/Color.py` & `pyxbox-0.1.3/pyxbox/bilibili_utils/Color.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/bilibili_utils/Danmaku.py` & `pyxbox-0.1.3/pyxbox/bilibili_utils/Danmaku.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/bilibili_utils/utils.py` & `pyxbox-0.1.3/pyxbox/bilibili_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/bilibili_utils/varint.py` & `pyxbox-0.1.3/pyxbox/bilibili_utils/varint.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/media.py` & `pyxbox-0.1.3/pyxbox/media.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/proxies.py` & `pyxbox-0.1.3/pyxbox/proxies.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/tools.py` & `pyxbox-0.1.3/pyxbox/tools.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox/user_agent.py` & `pyxbox-0.1.3/pyxbox/user_agent.py`

 * *Files identical despite different names*

### Comparing `pyxbox-0.1.2/pyxbox.egg-info/PKG-INFO` & `pyxbox-0.1.3/pyxbox.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxbox
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://gitee.com/spider-x/pyxbox
 Author: BruceLong
 Author-email: 18656170559@163.com
 License: MIT Licence
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -47,14 +47,18 @@
 
 #### user_agent
 - 请求头：user-agent库
 
 #### proxies
 - 代理相关模块封装
 
+#### mail
+##### EmailSender
+> 邮件发送工具，不用再写太多冗余的代码只需要简单的几行代码即可批量发送内容。
+
 ## 安装教程
 
 1. 安装：`pip install pyxbox`
 2. 更新：`pip install -U pyxbox`
 3. 卸载：`pip uninstall pyxbox`
 
 ## 使用说明
```

### Comparing `pyxbox-0.1.2/pyxbox.egg-info/SOURCES.txt` & `pyxbox-0.1.3/pyxbox.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 pyxbox/__init__.py
+pyxbox/mail.py
 pyxbox/media.py
 pyxbox/proxies.py
 pyxbox/tools.py
 pyxbox/user_agent.py
 pyxbox.egg-info/PKG-INFO
 pyxbox.egg-info/SOURCES.txt
 pyxbox.egg-info/dependency_links.txt
```

### Comparing `pyxbox-0.1.2/setup.py` & `pyxbox-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     README = readme.read()
 
 # 允许setup.py在任何路径下执行
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="pyxbox",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     long_description=README,  # 详细描述（一般会写在README.md中）
     long_description_content_type="text/markdown",  # README.md中描述的语法（一般为markdown）
     url="https://gitee.com/spider-x/pyxbox",
     author="BruceLong",
     license="MIT Licence",
     author_email="18656170559@163.com",
     include_package_data=True,
     platforms="any",
-    install_requires=['wheel', 'w3lib', 'requests', 'demjson==1.6', 'ffmpeg-python', 'tqdm']
+    install_requires=['wheel', 'w3lib', 'requests', 'demjson==1.6', 'ffmpeg-python', 'tqdm', 'six']
 )
```


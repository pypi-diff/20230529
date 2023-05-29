# Comparing `tmp/hackcqooc-0.0.8.tar.gz` & `tmp/hackcqooc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hackcqooc-0.0.8.tar", last modified: Thu Nov 24 15:11:25 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hackcqooc-0.0.8.tar` & `hackcqooc-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:11:25.484094 hackcqooc-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2022-11-24 15:11:25.484094 hackcqooc-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:11:25.484094 hackcqooc-0.0.8/hackcqooc/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/api_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     9159 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/msg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/request.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    40828 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/hackcqooc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 15:11:25.484094 hackcqooc-0.0.8/hackcqooc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2022-11-24 15:11:25.000000 hackcqooc-0.0.8/hackcqooc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      355 2022-11-24 15:11:25.000000 hackcqooc-0.0.8/hackcqooc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 15:11:25.000000 hackcqooc-0.0.8/hackcqooc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-24 15:11:25.000000 hackcqooc-0.0.8/hackcqooc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2022-11-24 15:11:25.000000 hackcqooc-0.0.8/hackcqooc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 15:11:25.484094 hackcqooc-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3829 2022-11-24 15:11:11.000000 hackcqooc-0.0.8/setup.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/license
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/requirements-dev.lock
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/requirements.lock
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/sample.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/setup.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/.github/workflows/run_pytest.yaml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/api_url.py
+-rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/core.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/msg.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/processor.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/request.py
+-rwxr-xr-x   0        0        0    40828 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/test.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/hackcqooc/user.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/.coveragerc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_api_url.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_core.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_msg.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_processor.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_request.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/tests/test_user.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 hackcqooc-0.0.9/PKG-INFO
```

### Comparing `hackcqooc-0.0.8/PKG-INFO` & `hackcqooc-0.0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,36 @@
-Metadata-Version: 2.1
-Name: hackcqooc
-Version: 0.0.8
-Summary: Hacking cqooc
-Home-page: https://github.com/Fatpandac/hackcqooc
-Author: Fatpandac
-Author-email: i@Fatpandac.com
-License: MIT
-Description: 
-        <h1 align="center">hackcqooc</h1>
-        
-        ![GitHub](https://img.shields.io/github/license/Fatpandac/hackcqooc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hackcqooc) ![PyPI](https://img.shields.io/pypi/v/hackcqooc) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Fatpandac/hackcqooc/main.svg)](https://results.pre-commit.ci/latest/github/Fatpandac/hackcqooc/main)
-        
-        一个重庆高校在线开放课程平台自动化工具包。
-        
-        ## [Hackcqooc 的使用样例](https://github.com/Fatpandac/hackcqooc/blob/main/sample.py)
-        
-        在终端环境中分别设置变量 `USERS` 和 `PASSWORD`
-        后运行 `python3 sample.py` 它将会告诉你 Hackcqooc 的运行方式。
-        
-        ## 安装
-        
-        ```
-        pip3 install hackcqooc
-        ```
-        
-        ## 功能
-        
-        1. 🔑 使用帐号密码直接登录
-        2. 🍪 使用 Cookie 登陆 ([@omg-xtao](https://github.com/omg-xtao))
-        3. ℹ️ 获取用户信息
-        4. 🏛️ 获取用户选课信息
-        5. 📚 获取用户课程详情
-        6. ⏳ 跳过对应课程
-        7. 📝 获取测验列表 ([@omg-xtao](https://github.com/omg-xtao))
-        8. 💯 获取考试列表 ([@omg-xtao](https://github.com/omg-xtao))
-        9. 📖 获取作业列表 ([@omg-xtao](https://github.com/omg-xtao))
-        10. 🔢 获取章节列表 ([@omg-xtao](https://github.com/omg-xtao))
-        
-        ## 有谁在使用
-        
-        |                      仓库                                    |             简介               |
-        |:--------------------------------------------------------:|:------------------------------:|
-        | [fuck_cqooc](https://github.com/Fatpandac/fuck_cqooc)    | 一个重庆高校在线开放课程平台刷课工具 |
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.0.0
-Description-Content-Type: text/markdown
+<h1 align="center">hackcqooc</h1>
+
+![GitHub](https://img.shields.io/github/license/Fatpandac/hackcqooc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hackcqooc) ![PyPI](https://img.shields.io/pypi/v/hackcqooc) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Fatpandac/hackcqooc/main.svg)](https://results.pre-commit.ci/latest/github/Fatpandac/hackcqooc/main)
+
+一个重庆高校在线开放课程平台自动化工具包。
+
+## [Hackcqooc 的使用样例](https://github.com/Fatpandac/hackcqooc/blob/main/sample.py)
+
+在终端环境中分别设置变量 `USERS` 和 `PASSWORD`
+后运行 `python3 sample.py` 它将会告诉你 Hackcqooc 的运行方式。
+
+## 安装
+
+```
+pip3 install hackcqooc
+```
+
+## 功能
+
+1. 🔑 使用帐号密码直接登录
+2. 🍪 使用 Cookie 登陆 ([@omg-xtao](https://github.com/omg-xtao))
+3. ℹ️ 获取用户信息
+4. 🏛️ 获取用户选课信息
+5. 📚 获取用户课程详情
+6. ⏳ 跳过对应课程
+7. 📝 获取测验列表 ([@omg-xtao](https://github.com/omg-xtao))
+8. 💯 获取考试列表 ([@omg-xtao](https://github.com/omg-xtao))
+9. 📖 获取作业列表 ([@omg-xtao](https://github.com/omg-xtao))
+10. 🔢 获取章节列表 ([@omg-xtao](https://github.com/omg-xtao))
+
+## 有谁在使用
+
+|                      仓库                                 |             简介               |
+|:--------------------------------------------------------:|:------------------------------:|
+| [fuckcqooc](https://github.com/Fatpandac/fuck_cqooc)     | 一个重庆高校在线开放课程平台刷课工具 |
+| [xygxpt](https://github.com/Mrkk1/xygxpt)                | 小鱼高校平台助手                  |
```

### Comparing `hackcqooc-0.0.8/README.md` & `hackcqooc-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: hackcqooc
+Version: 0.0.9
+Summary: 一个重庆高校在线开放课程平台自动化工具包。
+Author-email: Fatpandac <i@fatpandac.com>
+License: MIT
+Requires-Python: >=3.8
+Requires-Dist: js2py~=0.74
+Requires-Dist: requests~=2.30.0
+Description-Content-Type: text/markdown
+
 <h1 align="center">hackcqooc</h1>
 
 ![GitHub](https://img.shields.io/github/license/Fatpandac/hackcqooc) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hackcqooc) ![PyPI](https://img.shields.io/pypi/v/hackcqooc) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Fatpandac/hackcqooc/main.svg)](https://results.pre-commit.ci/latest/github/Fatpandac/hackcqooc/main)
 
 一个重庆高校在线开放课程平台自动化工具包。
 
 ## [Hackcqooc 的使用样例](https://github.com/Fatpandac/hackcqooc/blob/main/sample.py)
@@ -26,10 +37,11 @@
 7. 📝 获取测验列表 ([@omg-xtao](https://github.com/omg-xtao))
 8. 💯 获取考试列表 ([@omg-xtao](https://github.com/omg-xtao))
 9. 📖 获取作业列表 ([@omg-xtao](https://github.com/omg-xtao))
 10. 🔢 获取章节列表 ([@omg-xtao](https://github.com/omg-xtao))
 
 ## 有谁在使用
 
-|                      仓库                                    |             简介               |
+|                      仓库                                 |             简介               |
 |:--------------------------------------------------------:|:------------------------------:|
-| [fuck_cqooc](https://github.com/Fatpandac/fuck_cqooc)    | 一个重庆高校在线开放课程平台刷课工具 |
+| [fuckcqooc](https://github.com/Fatpandac/fuck_cqooc)     | 一个重庆高校在线开放课程平台刷课工具 |
+| [xygxpt](https://github.com/Mrkk1/xygxpt)                | 小鱼高校平台助手                  |
```

### Comparing `hackcqooc-0.0.8/hackcqooc/api_url.py` & `hackcqooc-0.0.9/hackcqooc/api_url.py`

 * *Files identical despite different names*

### Comparing `hackcqooc-0.0.8/hackcqooc/core.py` & `hackcqooc-0.0.9/hackcqooc/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         login_success = data["code"] == 0
         if login_success:
             self.__user.set_xsid(data["xsid"])
             self.__request.set_headers("Cookie", f'xsid={data["xsid"]}')
             self.__process_user_info()
             return Msg().processing("登录成功", 200, data)
         else:
-            return Msg().processing("登录失败，可能需要官网登录后重试", 400, data)
+            # return Msg().processing("登录失败，可能需要官网登录后重试", 400, data)
+            return Msg().processing(data["msg"], 400, data)
 
     def __login_by_cookie(self) -> dict:
         cookie = self.__user.get_cookie()
         # parse cookie to dict
         cookie_dict = dict(
             item.split("=") if "=" in item else ""
             for item in cookie.split(";")
```

### Comparing `hackcqooc-0.0.8/hackcqooc/msg.py` & `hackcqooc-0.0.9/hackcqooc/msg.py`

 * *Files identical despite different names*

### Comparing `hackcqooc-0.0.8/hackcqooc/processor.py` & `hackcqooc-0.0.9/hackcqooc/processor.py`

 * *Files identical despite different names*

### Comparing `hackcqooc-0.0.8/hackcqooc/request.py` & `hackcqooc-0.0.9/hackcqooc/request.py`

 * *Files identical despite different names*

### Comparing `hackcqooc-0.0.8/hackcqooc/test.py` & `hackcqooc-0.0.9/hackcqooc/test.py`

 * *Files identical despite different names*

### Comparing `hackcqooc-0.0.8/hackcqooc/user.py` & `hackcqooc-0.0.9/hackcqooc/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 class User:
-
     __xsid = None
     __sid = None
     __username = None
     __pwd = None
     __name = None
     __course_data = None
     __lessons_data = None
```

### Comparing `hackcqooc-0.0.8/setup.py` & `hackcqooc-0.0.9/setup.py`

 * *Files identical despite different names*


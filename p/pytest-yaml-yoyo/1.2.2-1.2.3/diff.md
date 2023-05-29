# Comparing `tmp/pytest-yaml-yoyo-1.2.2.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.2.tar", last modified: Mon May 22 13:47:58 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.3.tar", last modified: Mon May 29 07:10:43 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.2.tar` & `pytest-yaml-yoyo-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.045463 pytest-yaml-yoyo-1.2.2/
--rw-rw-rw-   0        0        0    23692 2023-05-22 13:47:58.044494 pytest-yaml-yoyo-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    23193 2023-05-20 01:43:47.000000 pytest-yaml-yoyo-1.2.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-22 13:47:58.045463 pytest-yaml-yoyo-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:57.809317 pytest-yaml-yoyo-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.011555 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9329 2023-05-22 13:47:16.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28442 2023-05-19 16:19:35.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:58.042499 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    23692 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 13:47:57.000000 pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.134659 pytest-yaml-yoyo-1.2.3/
+-rw-rw-rw-   0        0        0    23692 2023-05-29 07:10:43.132663 pytest-yaml-yoyo-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    23193 2023-05-20 01:43:47.000000 pytest-yaml-yoyo-1.2.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:10:43.134659 pytest-yaml-yoyo-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:10:42.998644 pytest-yaml-yoyo-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.107729 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9720 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28418 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.130668 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    23692 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.2/PKG-INFO` & `pytest-yaml-yoyo-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.2
+Version: 1.2.3
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
```

### Comparing `pytest-yaml-yoyo-1.2.2/README.rst` & `pytest-yaml-yoyo-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/setup.py` & `pytest-yaml-yoyo-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.2',
+    version='v1.2.3',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,23 @@
         }
     # 添加全局base_url
     s.base_url = request.config.option.base_url
     yield s
     s.close()
 
 
+@pytest.fixture(scope="session", autouse=True)
+def environ(request):
+    """Return a env object"""
+    config = request.config
+    env_name = config.getoption("--env") or config.getini("env")
+    if env_name is not None:
+        return g.get('env')
+
+
 def pytest_collect_file(file_path: Path, parent):  # noqa
     """
         收集测试用例：
         1.测试文件以.yml 或 .yaml 后缀的文件
         2.并且以 test 开头或者 test 结尾
     """
     if file_path.suffix in [".yml", ".yaml"] and (file_path.name.startswith("test") or file_path.name.endswith("test")):
@@ -206,25 +215,29 @@
 def pytest_terminal_summary(terminalreporter, exitstatus, config): # noqa
     """收集测试结果"""
     total = terminalreporter._numcollected  # noqa
     if total > 0:
         passed = len([i for i in terminalreporter.stats.get('passed', []) if i.when != 'teardown'])
         failed = len([i for i in terminalreporter.stats.get('failed', []) if i.when != 'teardown'])
         error = len([i for i in terminalreporter.stats.get('error', []) if i.when != 'teardown'])
-        # skipped = len([i for i in terminalreporter.stats.get('skipped', []) if i.when != 'teardown'])
-        successful = len(terminalreporter.stats.get('passed', [])) / terminalreporter._numcollected * 100  # noqa
+        skipped = len([i for i in terminalreporter.stats.get('skipped', []) if i.when != 'teardown'])
+        if terminalreporter._numcollected- skipped == 0:
+            successful = 0
+        else:
+            successful = len(terminalreporter.stats.get('passed', [])) / terminalreporter._numcollected * 100  # noqa
         duration = time.time() - terminalreporter._sessionstarttime  # noqa
         markdown_text = f"""### 执行结果:
 - 运行环境: {g.get('env_name')}
 - 运行base_url: {g.get('base_url')}
 - 持续时间: {duration: .2f} 秒
 
 ### 本次运行结果:
 - 总用例数: {total}
 - 通过用例：{passed}
+- 跳过用例：{skipped}
 - 失败用例： {failed}
 - 异常用例： {error}
 - 通过率： {successful: .2f} % \n
 """
         if g.get('env'):
             if hasattr(g["env"], 'DING_TALK'):
                 ding_talk = g["env"].DING_TALK
```

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
                 case[case_name] = case_value
             else:
                 case[case_name] = [case_value]
             # 用例参数获取
             if len(case[case_name]) < 1:
                 log.debug('test case not item to run !')
             else:
-                log.info(f'--------{case[case_name]}')
                 if 'fixtures' in case[case_name][0]:
                     case_raw_fixtures = case[case_name][0].get('fixtures', [])
                     case_fixtures = render_template_obj.rend_template_any(case_raw_fixtures, **self.context)
                 if "parameters" in case[case_name][0]:
                     log.info('parameters 参数化执行用例')
                     case_raw_parameters = case[case_name][0].get('parameters', [])
                     # case_raw_fixtures = case[case_name][0].get('fixtures', [])
@@ -403,17 +402,17 @@
             return request_value
         import inspect
         for fun in funcs:
             # 获取函数对象的入参
             ars = [arg_name for arg_name, v in inspect.signature(fun).parameters.items()]
             if 'req' in ars:
                 if context:
-                    fun(context.get('req'))
+                    fun(*[context.get(arg) for arg in ars])
                 else:
-                    fun(self.context.get('req'))
+                    fun(*[self.context.get(arg) for arg in ars])
             else:
                 fun()
         return request_value
 
     def response_hooks(self, config_hooks: dict, request_value: dict) -> dict:
         """ 合并全局config_hooks 和 单个请求 hooks 参数
             config_hooks = {
```

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/validate.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.2
+Version: 1.2.3
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
```

### Comparing `pytest-yaml-yoyo-1.2.2/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


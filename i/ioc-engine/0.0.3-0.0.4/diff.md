# Comparing `tmp/ioc_engine-0.0.3.tar.gz` & `tmp/ioc_engine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioc_engine-0.0.3.tar", last modified: Fri May 26 10:56:59 2023, max compression
+gzip compressed data, was "ioc_engine-0.0.4.tar", last modified: Mon May 29 10:57:14 2023, max compression
```

## Comparing `ioc_engine-0.0.3.tar` & `ioc_engine-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 10:56:59.412179 ioc_engine-0.0.3/
--rw-r--r--   0 zhangzhihua   (501) staff       (20)      332 2023-05-26 10:56:59.412033 ioc_engine-0.0.3/PKG-INFO
--rw-r--r--   0 zhangzhihua   (501) staff       (20)       11 2023-05-26 10:20:03.000000 ioc_engine-0.0.3/README.md
-drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 10:56:59.410210 ioc_engine-0.0.3/ioc_engine.egg-info/
--rw-r--r--   0 zhangzhihua   (501) staff       (20)      332 2023-05-26 10:56:59.000000 ioc_engine-0.0.3/ioc_engine.egg-info/PKG-INFO
--rw-r--r--   0 zhangzhihua   (501) staff       (20)      290 2023-05-26 10:56:59.000000 ioc_engine-0.0.3/ioc_engine.egg-info/SOURCES.txt
--rw-r--r--   0 zhangzhihua   (501) staff       (20)        1 2023-05-26 10:56:59.000000 ioc_engine-0.0.3/ioc_engine.egg-info/dependency_links.txt
--rw-r--r--   0 zhangzhihua   (501) staff       (20)        4 2023-05-26 10:56:59.000000 ioc_engine-0.0.3/ioc_engine.egg-info/top_level.txt
-drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 10:56:59.411502 ioc_engine-0.0.3/lib/
--rw-r--r--   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 07:19:51.000000 ioc_engine-0.0.3/lib/__init__.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)     1689 2023-05-26 09:13:26.000000 ioc_engine-0.0.3/lib/application_context.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)       94 2023-05-26 09:13:26.000000 ioc_engine-0.0.3/lib/exception.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)     1308 2023-05-26 09:08:32.000000 ioc_engine-0.0.3/lib/function_util.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)     3002 2023-05-26 09:27:37.000000 ioc_engine-0.0.3/lib/ioc_engine.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)     1385 2023-05-26 09:08:39.000000 ioc_engine-0.0.3/lib/module_util.py
--rw-r--r--   0 zhangzhihua   (501) staff       (20)       38 2023-05-26 10:56:59.412221 ioc_engine-0.0.3/setup.cfg
--rw-r--r--   0 zhangzhihua   (501) staff       (20)      601 2023-05-26 10:56:27.000000 ioc_engine-0.0.3/setup.py
-drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 10:56:59.411725 ioc_engine-0.0.3/test/
--rw-r--r--   0 zhangzhihua   (501) staff       (20)      735 2023-05-26 09:25:33.000000 ioc_engine-0.0.3/test/test_scan.py
+drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-29 10:57:14.241159 ioc_engine-0.0.4/
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)      332 2023-05-29 10:57:14.241004 ioc_engine-0.0.4/PKG-INFO
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)       11 2023-05-26 10:20:03.000000 ioc_engine-0.0.4/README.md
+drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-29 10:57:14.239732 ioc_engine-0.0.4/ioc_engine/
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)        0 2023-05-26 07:19:51.000000 ioc_engine-0.0.4/ioc_engine/__init__.py
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)     1692 2023-05-29 10:52:14.000000 ioc_engine-0.0.4/ioc_engine/application_context.py
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)       94 2023-05-26 09:13:26.000000 ioc_engine-0.0.4/ioc_engine/exception.py
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)     1308 2023-05-26 09:08:32.000000 ioc_engine-0.0.4/ioc_engine/function_util.py
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)     3024 2023-05-29 10:52:14.000000 ioc_engine-0.0.4/ioc_engine/ioc_engine.py
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)     1385 2023-05-26 09:08:39.000000 ioc_engine-0.0.4/ioc_engine/module_util.py
+drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-29 10:57:14.240511 ioc_engine-0.0.4/ioc_engine.egg-info/
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)      332 2023-05-29 10:57:14.000000 ioc_engine-0.0.4/ioc_engine.egg-info/PKG-INFO
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)      332 2023-05-29 10:57:14.000000 ioc_engine-0.0.4/ioc_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)        1 2023-05-29 10:57:14.000000 ioc_engine-0.0.4/ioc_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)       11 2023-05-29 10:57:14.000000 ioc_engine-0.0.4/ioc_engine.egg-info/top_level.txt
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)       38 2023-05-29 10:57:14.241203 ioc_engine-0.0.4/setup.cfg
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)      590 2023-05-29 10:57:03.000000 ioc_engine-0.0.4/setup.py
+drwxr-xr-x   0 zhangzhihua   (501) staff       (20)        0 2023-05-29 10:57:14.240660 ioc_engine-0.0.4/test/
+-rw-r--r--   0 zhangzhihua   (501) staff       (20)      736 2023-05-29 10:54:00.000000 ioc_engine-0.0.4/test/test_scan.py
```

### Comparing `ioc_engine-0.0.3/lib/application_context.py` & `ioc_engine-0.0.4/ioc_engine/application_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 
     def set_object(self, value: Any):
         bean_define = BeanDefinition.build(value)
         if bean_define.name in self.__context_name_map:
             raise Exception("容器内注入的对象发生冲突")
         self.__context_name_map[bean_define.name] = bean_define
 
-    def get_type_object_first(self, clazz: Type[T]) -> Optional[T]:
+    def get_object_by_type(self, clazz: Type[T]) -> Optional[T]:
         name = BeanDefinition.build_common_name(clazz)
-        element = self.get_name_object(name)
+        element = self.get_object_by_name(name)
         if element is not None:
             return element
         return None
 
-    def get_name_object(self, name: str) -> Optional[T]:
+    def get_object_by_name(self, name: str) -> Optional[T]:
         value: BeanDefinition = self.__context_name_map.get(name)
         if value is None:
             return None
         return value.value
 
     def contain_type(self, clazz: Type[T]):
         return clazz in self.__context_name_map
```

### Comparing `ioc_engine-0.0.3/lib/function_util.py` & `ioc_engine-0.0.4/ioc_engine/function_util.py`

 * *Files identical despite different names*

### Comparing `ioc_engine-0.0.3/lib/ioc_engine.py` & `ioc_engine-0.0.4/ioc_engine/ioc_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 from typing import Type
 
-from lib import function_util
-from lib.application_context import ApplicationContext
-from lib.exception import NoAutoScanException
-from lib.function_util import FunctionParamsMeta
+from ioc_engine import function_util
+from ioc_engine.application_context import ApplicationContext
+from ioc_engine.exception import NoAutoScanException
+from ioc_engine.function_util import FunctionParamsMeta
 
 
 class AutoScan:
     """
     如果需要被自动扫描，需要继承这个类
     """
 
@@ -17,15 +17,15 @@
     def __init__(self):
         self.application_context = ApplicationContext()
 
     def scan(self, clazz: Type):
         # 监测到还依赖于自动注入的类，递归加载依赖的类
         if not issubclass(clazz, AutoScan):
             raise NoAutoScanException(f"无法加载没有开启AutoScan的类, class:{clazz}")
-        value = self.application_context.get_type_object_first(clazz)
+        value = self.application_context.get_object_by_type(clazz)
         if value is not None:
             return value
 
         value = clazz.__new__(clazz)
         try:
             # 检测构造函数是否被重写
             getattr(clazz.__init__, "__annotations__")
@@ -68,14 +68,14 @@
                 if meta.args_type != FunctionParamsMeta.ArgsTypeEnum.NORMAL:
                     continue
                 class_type = meta.args_class
                 value = None
                 if not self.application_context.contain_type(class_type):
                     value = self.scan(class_type)
                 if value is None:
-                    value = application_context.get_type_object_first(class_type)
+                    value = application_context.get_object_by_type(class_type)
                 if meta.args_name not in kwargs:
                     kwargs[meta.args_name] = value
             result = func(*args, **kwargs)
             return result
 
         return inner_wrapper
```

### Comparing `ioc_engine-0.0.3/lib/module_util.py` & `ioc_engine-0.0.4/ioc_engine/module_util.py`

 * *Files identical despite different names*

### Comparing `ioc_engine-0.0.3/setup.py` & `ioc_engine-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 
-import lib
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ioc_engine",
-    version="0.0.3",
+    version="0.0.4",
     author="dawndevil",
     author_email="351987551@qq.com",
     description="ioc容器",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(exclude=["test", "*.test", "test.*"]),
```

### Comparing `ioc_engine-0.0.3/test/test_scan.py` & `ioc_engine-0.0.4/test/test_scan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pytest
 
-from lib.exception import NoAutoScanException
+from ioc_engine.exception import NoAutoScanException
 from test import mock_entry
 from test.mock2_entity import Mock2
 from test.mock_entity import Mock
 from test.mock_entry import engine
 
 
 def test_mock_inject_success():
     mock2 = mock_entry.get_mock2()
 
-    assert mock2 == engine.application_context.get_type_object_first(Mock2)
+    assert mock2 == engine.application_context.get_object_by_type(Mock2)
     print("自动加载mock2成功")
-    assert mock2.get_mock() == engine.application_context.get_type_object_first(Mock)
+    assert mock2.get_mock() == engine.application_context.get_object_by_type(Mock)
     print("自动加载mock2中的mock1成功")
 
 
 def test_mock_inject_failed():
     # mock4 没有设置自动依赖，应该报错
     with pytest.raises(NoAutoScanException):
         mock_entry.get_mock3()
```


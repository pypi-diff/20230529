# Comparing `tmp/python-utils-3.5.2.tar.gz` & `tmp/python-utils-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-utils-3.5.2.tar", last modified: Thu Feb  9 14:41:01 2023, max compression
+gzip compressed data, was "python-utils-3.6.0.tar", last modified: Mon May 29 00:59:15 2023, max compression
```

## Comparing `python-utils-3.5.2.tar` & `python-utils-3.6.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-02-09 14:41:01.926658 python-utils-3.5.2/
--rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.5.2/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.5.2/MANIFEST.in
--rw-r--r--   0 rick       (501) staff       (20)     8814 2023-02-09 14:41:01.926794 python-utils-3.5.2/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     8370 2022-10-26 10:18:43.000000 python-utils-3.5.2/README.rst
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-02-09 14:41:01.918385 python-utils-3.5.2/_python_utils_tests/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-02-09 14:40:50.000000 python-utils-3.5.2/_python_utils_tests/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.5.2/_python_utils_tests/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      592 2023-02-08 16:44:13.000000 python-utils-3.5.2/_python_utils_tests/test_containers.py
--rw-r--r--   0 rick       (501) staff       (20)      897 2022-05-29 21:48:50.000000 python-utils-3.5.2/_python_utils_tests/test_decorators.py
--rw-r--r--   0 rick       (501) staff       (20)     1669 2022-05-30 22:13:21.000000 python-utils-3.5.2/_python_utils_tests/test_generators.py
--rw-r--r--   0 rick       (501) staff       (20)     1431 2022-05-29 21:48:50.000000 python-utils-3.5.2/_python_utils_tests/test_import.py
--rw-r--r--   0 rick       (501) staff       (20)      362 2022-05-29 02:02:55.000000 python-utils-3.5.2/_python_utils_tests/test_logger.py
--rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.5.2/_python_utils_tests/test_python_utils.py
--rw-r--r--   0 rick       (501) staff       (20)     4326 2022-10-29 19:12:20.000000 python-utils-3.5.2/_python_utils_tests/test_time.py
--rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.5.2/coverage.rc
--rw-r--r--   0 rick       (501) staff       (20)      252 2022-06-01 21:21:04.000000 python-utils-3.5.2/pytest.ini
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-02-09 14:41:01.924603 python-utils-3.5.2/python_utils/
--rw-r--r--   0 rick       (501) staff       (20)      385 2023-02-09 14:40:51.000000 python-utils-3.5.2/python_utils/__about__.py
--rw-r--r--   0 rick       (501) staff       (20)     1705 2023-02-09 14:40:51.000000 python-utils-3.5.2/python_utils/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)      502 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/aio.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.5.2/python_utils/compat.py
--rw-r--r--   0 rick       (501) staff       (20)     8321 2023-02-09 14:40:51.000000 python-utils-3.5.2/python_utils/containers.py
--rw-r--r--   0 rick       (501) staff       (20)    11285 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/converters.py
--rw-r--r--   0 rick       (501) staff       (20)     3119 2022-05-29 21:48:50.000000 python-utils-3.5.2/python_utils/decorators.py
--rw-r--r--   0 rick       (501) staff       (20)      610 2022-05-29 02:07:44.000000 python-utils-3.5.2/python_utils/exceptions.py
--rw-r--r--   0 rick       (501) staff       (20)     4926 2022-10-29 18:57:07.000000 python-utils-3.5.2/python_utils/formatters.py
--rw-r--r--   0 rick       (501) staff       (20)     2275 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/generators.py
--rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.5.2/python_utils/import_.py
--rw-r--r--   0 rick       (501) staff       (20)     3053 2022-05-29 21:48:50.000000 python-utils-3.5.2/python_utils/logger.py
--rw-r--r--   0 rick       (501) staff       (20)      320 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/loguru.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/py.typed
--rw-r--r--   0 rick       (501) staff       (20)     4853 2022-10-29 19:12:20.000000 python-utils-3.5.2/python_utils/terminal.py
--rw-r--r--   0 rick       (501) staff       (20)    10122 2022-05-29 21:48:50.000000 python-utils-3.5.2/python_utils/time.py
--rw-r--r--   0 rick       (501) staff       (20)     3118 2023-02-09 13:42:39.000000 python-utils-3.5.2/python_utils/types.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-02-09 14:41:01.926404 python-utils-3.5.2/python_utils.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)     8814 2023-02-09 14:41:01.000000 python-utils-3.5.2/python_utils.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     1022 2023-02-09 14:41:01.000000 python-utils-3.5.2/python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2023-02-09 14:41:01.000000 python-utils-3.5.2/python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)      187 2023-02-09 14:41:01.000000 python-utils-3.5.2/python_utils.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       13 2023-02-09 14:41:01.000000 python-utils-3.5.2/python_utils.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)        2 2021-12-16 15:50:12.000000 python-utils-3.5.2/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      611 2023-02-09 14:41:01.927926 python-utils-3.5.2/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)     1615 2023-02-08 16:44:13.000000 python-utils-3.5.2/setup.py
--rw-r--r--   0 rick       (501) staff       (20)     1488 2023-02-09 14:40:51.000000 python-utils-3.5.2/tox.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.642409 python-utils-3.6.0/
+-rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.6.0/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.6.0/MANIFEST.in
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-05-29 00:59:15.642876 python-utils-3.6.0/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     8642 2023-05-29 00:58:50.000000 python-utils-3.6.0/README.rst
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.605651 python-utils-3.6.0/_python_utils_tests/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-29 00:58:48.000000 python-utils-3.6.0/_python_utils_tests/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.6.0/_python_utils_tests/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      508 2023-05-29 00:58:50.000000 python-utils-3.6.0/_python_utils_tests/test_aio.py
+-rw-r--r--   0 rick       (501) staff       (20)      592 2023-02-08 16:44:13.000000 python-utils-3.6.0/_python_utils_tests/test_containers.py
+-rw-r--r--   0 rick       (501) staff       (20)      897 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1669 2022-05-30 22:13:21.000000 python-utils-3.6.0/_python_utils_tests/test_generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1431 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_import.py
+-rw-r--r--   0 rick       (501) staff       (20)      362 2022-05-29 02:02:55.000000 python-utils-3.6.0/_python_utils_tests/test_logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_python_utils.py
+-rw-r--r--   0 rick       (501) staff       (20)     4326 2022-10-29 19:12:20.000000 python-utils-3.6.0/_python_utils_tests/test_time.py
+-rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.6.0/coverage.rc
+-rw-r--r--   0 rick       (501) staff       (20)      391 2023-05-29 00:58:50.000000 python-utils-3.6.0/pyproject.toml
+-rw-r--r--   0 rick       (501) staff       (20)      253 2023-05-29 00:58:50.000000 python-utils-3.6.0/pytest.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.623605 python-utils-3.6.0/python_utils/
+-rw-r--r--   0 rick       (501) staff       (20)      385 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/__about__.py
+-rw-r--r--   0 rick       (501) staff       (20)     1705 2023-05-29 00:58:48.000000 python-utils-3.6.0/python_utils/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)      544 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/aio.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.6.0/python_utils/compat.py
+-rw-r--r--   0 rick       (501) staff       (20)     9783 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/containers.py
+-rw-r--r--   0 rick       (501) staff       (20)    11404 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/converters.py
+-rw-r--r--   0 rick       (501) staff       (20)     4061 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)      617 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/exceptions.py
+-rw-r--r--   0 rick       (501) staff       (20)     5015 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/formatters.py
+-rw-r--r--   0 rick       (501) staff       (20)     2609 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.6.0/python_utils/import_.py
+-rw-r--r--   0 rick       (501) staff       (20)     3132 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      358 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/loguru.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.6.0/python_utils/py.typed
+-rw-r--r--   0 rick       (501) staff       (20)     4711 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/terminal.py
+-rw-r--r--   0 rick       (501) staff       (20)    11304 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/time.py
+-rw-r--r--   0 rick       (501) staff       (20)     3652 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/types.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.641745 python-utils-3.6.0/python_utils.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     1069 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)      160 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       13 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)        2 2023-02-09 15:13:53.000000 python-utils-3.6.0/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      611 2023-05-29 00:59:15.646852 python-utils-3.6.0/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)     1594 2023-05-29 00:58:50.000000 python-utils-3.6.0/setup.py
+-rw-r--r--   0 rick       (501) staff       (20)     1440 2023-05-29 00:58:50.000000 python-utils-3.6.0/tox.ini
```

### Comparing `python-utils-3.5.2/LICENSE` & `python-utils-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/PKG-INFO` & `python-utils-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.5.2
+Version: 3.6.0
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >3.6.0
+Requires-Python: >3.8.0
 Provides-Extra: loguru
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 Useful Python Utils
 ==============================================================================
@@ -36,14 +36,21 @@
 
  - The source: https://github.com/WoLpH/python-utils
  - Project page: https://pypi.python.org/pypi/python-utils
  - Reporting bugs: https://github.com/WoLpH/python-utils/issues
  - Documentation: https://python-utils.readthedocs.io/en/latest/
  - My blog: https://wol.ph/
 
+Security contact information
+------------------------------------------------------------------------------
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
+
 Requirements for installing:
 ------------------------------------------------------------------------------
 
 For the Python 3+ release (i.e. v3.0.0 or higher) there are no requirements.
 For the Python 2 compatible version (v2.x.x) the `six` package is needed.
 
 Installation:
```

### Comparing `python-utils-3.5.2/README.rst` & `python-utils-3.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
  - The source: https://github.com/WoLpH/python-utils
  - Project page: https://pypi.python.org/pypi/python-utils
  - Reporting bugs: https://github.com/WoLpH/python-utils/issues
  - Documentation: https://python-utils.readthedocs.io/en/latest/
  - My blog: https://wol.ph/
 
+Security contact information
+------------------------------------------------------------------------------
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
+
 Requirements for installing:
 ------------------------------------------------------------------------------
 
 For the Python 3+ release (i.e. v3.0.0 or higher) there are no requirements.
 For the Python 2 compatible version (v2.x.x) the `six` package is needed.
 
 Installation:
```

### Comparing `python-utils-3.5.2/_python_utils_tests/test_containers.py` & `python-utils-3.6.0/_python_utils_tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/_python_utils_tests/test_decorators.py` & `python-utils-3.6.0/_python_utils_tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/_python_utils_tests/test_generators.py` & `python-utils-3.6.0/_python_utils_tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/_python_utils_tests/test_import.py` & `python-utils-3.6.0/_python_utils_tests/test_import.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/_python_utils_tests/test_time.py` & `python-utils-3.6.0/_python_utils_tests/test_time.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/python_utils/__init__.py` & `python-utils-3.6.0/python_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/python_utils/containers.py` & `python-utils-3.6.0/python_utils/containers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,69 @@
+# pyright: reportIncompatibleMethodOverride=false
 import abc
 import typing
-from typing import Any, Generator
+import collections
 
 from . import types
 
 if typing.TYPE_CHECKING:
     import _typeshed  # noqa: F401
 
 #: A type alias for a type that can be used as a key in a dictionary.
 KT = types.TypeVar('KT')
 #: A type alias for a type that can be used as a value in a dictionary.
 VT = types.TypeVar('VT')
 #: A type alias for a dictionary with keys of type KT and values of type VT.
 DT = types.Dict[KT, VT]
 #: A type alias for the casted type of a dictionary key.
-KT_cast = types.Optional[types.Callable[[Any], KT]]
+KT_cast = types.Optional[types.Callable[..., KT]]
 #: A type alias for the casted type of a dictionary value.
-VT_cast = types.Optional[types.Callable[[Any], VT]]
+VT_cast = types.Optional[types.Callable[..., VT]]
 #: A type alias for the hashable values of the `UniqueList`
 HT = types.TypeVar('HT', bound=types.Hashable)
+#: A type alias for a regular generic type
+T = types.TypeVar('T')
 
 # Using types.Union instead of | since Python 3.7 doesn't fully support it
 DictUpdateArgs = types.Union[
-    types.Mapping,
-    types.Iterable[types.Union[types.Tuple[Any, Any], types.Mapping]],
+    types.Mapping[KT, VT],
+    types.Iterable[types.Tuple[KT, VT]],
+    types.Iterable[types.Mapping[KT, VT]],
     '_typeshed.SupportsKeysAndGetItem[KT, VT]',
 ]
 
+OnDuplicate = types.Literal['ignore', 'raise']
+
 
 class CastedDictBase(types.Dict[KT, VT], abc.ABC):
-    _key_cast: KT_cast
-    _value_cast: VT_cast
+    _key_cast: KT_cast[KT]
+    _value_cast: VT_cast[VT]
 
     def __init__(
         self,
-        key_cast: KT_cast = None,
-        value_cast: VT_cast = None,
-        *args: DictUpdateArgs,
+        key_cast: KT_cast[KT] = None,
+        value_cast: VT_cast[VT] = None,
+        *args: DictUpdateArgs[KT, VT],
         **kwargs: VT,
     ) -> None:
         self._value_cast = value_cast
         self._key_cast = key_cast
         self.update(*args, **kwargs)
 
-    def update(self, *args: DictUpdateArgs, **kwargs: VT) -> None:
+    def update(
+        self, *args: DictUpdateArgs[types.Any, types.Any], **kwargs: types.Any
+    ) -> None:
         if args:
             kwargs.update(*args)
 
         if kwargs:
             for key, value in kwargs.items():
                 self[key] = value
 
-    def __setitem__(self, key: Any, value: Any) -> None:
+    def __setitem__(self, key: types.Any, value: types.Any) -> None:
         if self._key_cast is not None:
             key = self._key_cast(key)
 
         return super().__setitem__(key, value)
 
 
 class CastedDict(CastedDictBase[KT, VT]):
@@ -89,15 +97,15 @@
     >>> d['3'] = '4'
     >>> d.update({'5': '6'})
     >>> d.update([('7', '8')])
     >>> d
     {1: 2, '3': '4', '5': '6', '7': '8'}
     '''
 
-    def __setitem__(self, key: Any, value: Any) -> None:
+    def __setitem__(self, key: typing.Any, value: typing.Any) -> None:
         if self._value_cast is not None:
             value = self._value_cast(value)
 
         super().__setitem__(key, value)
 
 
 class LazyCastedDict(CastedDictBase[KT, VT]):
@@ -142,41 +150,41 @@
 
     >>> list(d.items())
     [(1, 2), ('3', '4'), ('5', '6'), ('7', '8')]
     >>> d['3']
     '4'
     '''
 
-    def __setitem__(self, key: Any, value: Any) -> None:
+    def __setitem__(self, key: types.Any, value: types.Any):
         if self._key_cast is not None:
             key = self._key_cast(key)
 
         super().__setitem__(key, value)
 
-    def __getitem__(self, key: Any) -> VT:
+    def __getitem__(self, key: types.Any) -> VT:
         if self._key_cast is not None:
             key = self._key_cast(key)
 
         value = super().__getitem__(key)
 
         if self._value_cast is not None:
             value = self._value_cast(value)
 
         return value
 
     def items(  # type: ignore
         self,
-    ) -> Generator[types.Tuple[KT, VT], None, None]:
+    ) -> types.Generator[types.Tuple[KT, VT], None, None]:
         if self._value_cast is None:
             yield from super().items()
         else:
             for key, value in super().items():
                 yield key, self._value_cast(value)
 
-    def values(self) -> Generator[VT, None, None]:  # type: ignore
+    def values(self) -> types.Generator[VT, None, None]:  # type: ignore
         if self._value_cast is None:
             yield from super().values()
         else:
             for value in super().values():
                 yield self._value_cast(value)
 
 
@@ -215,15 +223,15 @@
     '''
 
     _set: types.Set[HT]
 
     def __init__(
         self,
         *args: HT,
-        on_duplicate: types.Literal['raise', 'ignore'] = 'ignore',
+        on_duplicate: OnDuplicate = 'ignore',
     ):
         self.on_duplicate = on_duplicate
         self._set = set()
         super().__init__()
         for arg in args:
             self.append(arg)
 
@@ -243,58 +251,97 @@
                 raise ValueError('Duplicate value: %s' % value)
             else:
                 return
 
         self._set.add(value)
         super().append(value)
 
-    def __contains__(self, item):
+    def __contains__(self, item: HT) -> bool:  # type: ignore
         return item in self._set
 
     @types.overload
     def __setitem__(self, indices: types.SupportsIndex, values: HT) -> None:
         ...
 
     @types.overload
     def __setitem__(self, indices: slice, values: types.Iterable[HT]) -> None:
         ...
 
-    def __setitem__(self, indices, values) -> None:
+    def __setitem__(
+        self,
+        indices: types.Union[slice, types.SupportsIndex],
+        values: types.Union[types.Iterable[HT], HT],
+    ) -> None:
         if isinstance(indices, slice):
+            values = types.cast(types.Iterable[HT], values)
             if self.on_duplicate == 'ignore':
                 raise RuntimeError(
                     'ignore mode while setting slices introduces ambiguous '
                     'behaviour and is therefore not supported'
                 )
 
-            duplicates = set(values) & self._set
-            if duplicates and values != self[indices]:
-                raise ValueError('Duplicate values: %s' % duplicates)
+            duplicates: types.Set[HT] = set(values) & self._set
+            if duplicates and values != list(self[indices]):
+                raise ValueError(f'Duplicate values: {duplicates}')
 
             self._set.update(values)
-            super().__setitem__(indices, values)
         else:
+            values = types.cast(HT, values)
             if values in self._set and values != self[indices]:
                 if self.on_duplicate == 'raise':
-                    raise ValueError('Duplicate value: %s' % values)
+                    raise ValueError(f'Duplicate value: {values}')
                 else:
                     return
 
             self._set.add(values)
-            super().__setitem__(indices, values)
+
+        super().__setitem__(
+            types.cast(slice, indices), types.cast(types.List[HT], values)
+        )
 
     def __delitem__(
         self, index: types.Union[types.SupportsIndex, slice]
     ) -> None:
         if isinstance(index, slice):
             for value in self[index]:
                 self._set.remove(value)
         else:
             self._set.remove(self[index])
 
         super().__delitem__(index)
 
 
+class SlicableDeque(types.Generic[T], collections.deque):  # type: ignore
+    @types.overload
+    def __getitem__(self, index: types.SupportsIndex) -> T:
+        ...
+
+    @types.overload
+    def __getitem__(self, index: slice) -> 'SlicableDeque[T]':
+        ...
+
+    def __getitem__(
+        self, index: types.Union[types.SupportsIndex, slice]
+    ) -> types.Union[T, 'SlicableDeque[T]']:
+        '''
+        Return the item or slice at the given index.
+
+        >>> d = SlicableDeque[int]([1, 2, 3, 4, 5])
+        >>> d[1:4]
+        SlicableDeque([2, 3, 4])
+
+        >>> d = SlicableDeque[str](['a', 'b', 'c'])
+        >>> d[-2:]
+        SlicableDeque(['b', 'c'])
+
+        '''
+        if isinstance(index, slice):
+            start, stop, step = index.indices(len(self))
+            return self.__class__(self[i] for i in range(start, stop, step))
+        else:
+            return types.cast(T, super().__getitem__(index))
+
+
 if __name__ == '__main__':
     import doctest
 
     doctest.testmod()
```

### Comparing `python-utils-3.5.2/python_utils/converters.py` & `python-utils-3.6.0/python_utils/converters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import decimal
 import math
 import re
 import typing
 
 from . import types
 
+_TN = types.TypeVar('_TN', bound=types.DecimalNumber)
+
 
 def to_int(
     input_: typing.Optional[str] = None,
     default: int = 0,
     exception: types.ExceptionsType = (ValueError, TypeError),
-    regexp: types.Optional[types.Pattern] = None,
+    regexp: types.Optional[types.Pattern[str]] = None,
 ) -> int:
     r'''
     Convert the given input to an integer or return default
 
     When trying to convert the exceptions given in the exception parameter
     are automatically catched and the default will be returned.
 
@@ -80,31 +82,30 @@
     elif hasattr(regexp, 'search'):
         pass
     elif regexp is not None:
         raise TypeError('unknown argument for regexp parameter: %r' % regexp)
 
     try:
         if regexp and input_:
-            match = regexp.search(input_)
-            if match:
+            if match := regexp.search(input_):
                 input_ = match.groups()[-1]
 
         if input_ is None:
             return default
         else:
             return int(input_)
     except exception:  # type: ignore
         return default
 
 
 def to_float(
     input_: str,
     default: int = 0,
     exception: types.ExceptionsType = (ValueError, TypeError),
-    regexp: types.Optional[types.Pattern] = None,
+    regexp: types.Optional[types.Pattern[str]] = None,
 ) -> types.Number:
     r'''
     Convert the given `input_` to an integer or return default
 
     When trying to convert the exceptions given in the exception parameter
     are automatically catched and the default will be returned.
 
@@ -161,16 +162,15 @@
     elif hasattr(regexp, 'search'):
         pass
     elif regexp is not None:
         raise TypeError('unknown argument for regexp parameter')
 
     try:
         if regexp:
-            match = regexp.search(input_)
-            if match:
+            if match := regexp.search(input_):
                 input_ = match.group(1)
         return float(input_)
     except exception:
         return default
 
 
 def to_unicode(
@@ -219,17 +219,15 @@
     b'a'
     >>> class Foo(object): __str__ = lambda s: u'a'
     >>> to_str(Foo())
     'a'
     >>> to_str(Foo)
     "<class 'python_utils.converters.Foo'>"
     '''
-    if isinstance(input_, bytes):
-        pass
-    else:
+    if not isinstance(input_, bytes):
         if not hasattr(input_, 'encode'):
             input_ = str(input_)
 
         input_ = input_.encode(encoding, errors)
     return input_
 
 
@@ -259,20 +257,20 @@
     else:
         power = min(int(math.log(x, 2) / 10), n_prefixes - 1)
     scaled = float(x) / (2 ** (10 * power))
     return scaled, power
 
 
 def remap(
-    value: types.DecimalNumber,
-    old_min: types.DecimalNumber,
-    old_max: types.DecimalNumber,
-    new_min: types.DecimalNumber,
-    new_max: types.DecimalNumber,
-) -> types.DecimalNumber:
+    value: _TN,
+    old_min: _TN,
+    old_max: _TN,
+    new_min: _TN,
+    new_max: _TN,
+) -> _TN:
     '''
     remap a value from one range into another.
 
     >>> remap(500, 0, 1000, 0, 100)
     50
     >>> remap(250.0, 0.0, 1000.0, 0.0, 100.0)
     25.0
@@ -358,36 +356,34 @@
         or isinstance(new_max, float)
     ):
         type_ = float
 
     else:
         type_ = int
 
-    value = type_(value)
-    old_min = type_(old_min)
-    old_max = type_(old_max)
-    new_max = type_(new_max)
-    new_min = type_(new_min)
-
-    old_range = old_max - old_min  # type: ignore
-    new_range = new_max - new_min  # type: ignore
+    value = types.cast(_TN, type_(value))
+    old_min = types.cast(_TN, type_(old_min))
+    old_max = types.cast(_TN, type_(old_max))
+    new_max = types.cast(_TN, type_(new_max))
+    new_min = types.cast(_TN, type_(new_min))
+
+    # These might not be floats but the Python type system doesn't understand
+    # the generic type system in this case
+    old_range = types.cast(float, old_max) - types.cast(float, old_min)
+    new_range = types.cast(float, new_max) - types.cast(float, new_min)
 
     if old_range == 0:
-        raise ValueError(
-            'Input range ({}-{}) is empty'.format(old_min, old_max)
-        )
+        raise ValueError(f'Input range ({old_min}-{old_max}) is empty')
 
     if new_range == 0:
-        raise ValueError(
-            'Output range ({}-{}) is empty'.format(new_min, new_max)
-        )
+        raise ValueError(f'Output range ({new_min}-{new_max}) is empty')
 
     new_value = (value - old_min) * new_range  # type: ignore
 
     if type_ == int:
         new_value //= old_range  # type: ignore
     else:
         new_value /= old_range  # type: ignore
 
     new_value += new_min  # type: ignore
 
-    return new_value
+    return types.cast(_TN, new_value)
```

### Comparing `python-utils-3.5.2/python_utils/formatters.py` & `python-utils-3.6.0/python_utils/formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pyright: reportUnnecessaryIsInstance=false
 import datetime
 
 from python_utils import types
 
 
 def camel_to_underscore(name: str) -> str:
     '''Convert camel case style naming to underscore/snake case style naming
@@ -17,15 +18,15 @@
     >>> camel_to_underscore('Spam_And_Bacon')
     'spam_and_bacon'
     >>> camel_to_underscore('__SpamAndBacon__')
     '__spam_and_bacon__'
     >>> camel_to_underscore('__SpamANDBacon__')
     '__spam_and_bacon__'
     '''
-    output = []
+    output: types.List[str] = []
     for i, c in enumerate(name):
         if i > 0:
             pc = name[i - 1]
             if c.isupper() and not pc.isupper() and pc != '_':
                 # Uppercase and the previous character isn't upper/underscore?
                 # Add the underscore
                 output.append('_')
@@ -40,15 +41,15 @@
 
     return ''.join(output)
 
 
 def apply_recursive(
     function: types.Callable[[str], str],
     data: types.OptionalScope = None,
-    **kwargs
+    **kwargs: types.Any,
 ) -> types.OptionalScope:
     '''
     Apply a function to all keys in a scope recursively
 
     >>> apply_recursive(camel_to_underscore, {'SpamEggsAndBacon': 'spam'})
     {'spam_eggs_and_bacon': 'spam'}
     >>> apply_recursive(camel_to_underscore, {'SpamEggsAndBacon': {
@@ -133,19 +134,19 @@
         (diff.days % 30 / 7, 'week', 'weeks'),
         (diff.days % 7, 'day', 'days'),
         (diff.seconds / 3600, 'hour', 'hours'),
         (diff.seconds % 3600 / 60, 'minute', 'minutes'),
         (diff.seconds % 60, 'second', 'seconds'),
     )
 
-    output = []
+    output: types.List[str] = []
     for period, singular, plural in periods:
         if int(period):
             if int(period) == 1:
                 output.append('%d %s' % (period, singular))
             else:
                 output.append('%d %s' % (period, plural))
 
     if output:
-        return '%s ago' % ' and '.join(output[:2])
+        return f'{" and ".join(output[:2])} ago'
 
     return default
```

### Comparing `python-utils-3.5.2/python_utils/generators.py` & `python-utils-3.6.0/python_utils/generators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 import asyncio
 import time
 
 import python_utils
 from python_utils import types
 
 
+_T = types.TypeVar('_T')
+
+
 async def abatcher(
-    generator: types.AsyncIterator,
+    generator: types.AsyncGenerator[_T, None],
     batch_size: types.Optional[int] = None,
     interval: types.Optional[types.delta_type] = None,
-) -> types.AsyncIterator[list]:
+) -> types.AsyncGenerator[types.List[_T], None]:
     '''
     Asyncio generator wrapper that returns items with a given batch size or
     interval (whichever is reached first).
     '''
-    batch: list = []
+    batch: types.List[_T] = []
 
     assert batch_size or interval, 'Must specify either batch_size or interval'
 
     # If interval is specified, use it to determine when to yield the batch
     # Alternatively set a really long timeout to keep the code simpler
     if interval:
         interval_s = python_utils.delta_to_seconds(interval)
     else:
         # Set the timeout to 10 years
         interval_s = 60 * 60 * 24 * 365 * 10.0
 
-    next_yield = time.perf_counter() + interval_s
+    next_yield: float = time.perf_counter() + interval_s
 
-    pending: types.Set = set()
+    done: types.Set[asyncio.Task[_T]]
+    pending: types.Set[asyncio.Task[_T]] = set()
 
     while True:
         try:
             done, pending = await asyncio.wait(
                 pending
                 or [
-                    asyncio.create_task(generator.__anext__()),  # type: ignore
+                    asyncio.create_task(
+                        types.cast(
+                            types.Coroutine[None, None, _T],
+                            generator.__anext__(),
+                        )
+                    ),
                 ],
                 timeout=interval_s,
                 return_when=asyncio.FIRST_COMPLETED,
             )
 
             if done:
                 for result in done:
@@ -61,20 +70,21 @@
             # Always set the next yield time to the current time. If the
             # loop is running slow due to blocking functions we do not
             # want to burst too much
             next_yield = time.perf_counter() + interval_s
 
 
 def batcher(
-    iterable: types.Iterable, batch_size: int = 10
-) -> types.Iterator[list]:
+    iterable: types.Iterable[_T],
+    batch_size: int = 10,
+) -> types.Generator[types.List[_T], None, None]:
     '''
     Generator wrapper that returns items with a given batch size
     '''
-    batch = []
+    batch: types.List[_T] = []
     for item in iterable:
         batch.append(item)
         if len(batch) == batch_size:
             yield batch
             batch = []
 
     if batch:
```

### Comparing `python-utils-3.5.2/python_utils/import_.py` & `python-utils-3.6.0/python_utils/import_.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/python_utils/logger.py` & `python-utils-3.6.0/python_utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     '''
 
     # Being a tad lazy here and not creating a Protocol.
     # The actual classes define the correct type anyway
     logger: typing.Any
 
     @classmethod
-    def __get_name(cls, *name_parts: str) -> str:
+    def __get_name(  # pyright: ignore[reportUnusedFunction]
+        cls, *name_parts: str
+    ) -> str:
         return '.'.join(n.strip() for n in name_parts if n.strip())
 
     @classmethod
     @functools.wraps(logging.debug)
     def debug(cls, msg: str, *args: typing.Any, **kwargs: typing.Any):
         cls.logger.debug(msg, *args, **kwargs)
 
@@ -91,12 +93,12 @@
 
     logger: logging.Logger  # pragma: no cover
 
     @classmethod
     def __get_name(cls, *name_parts: str) -> str:
         return LoggerBase._LoggerBase__get_name(*name_parts)  # type: ignore
 
-    def __new__(cls, *args, **kwargs):
+    def __new__(cls, *args: typing.Any, **kwargs: typing.Any):
         cls.logger = logging.getLogger(
             cls.__get_name(cls.__module__, cls.__name__)
         )
         return super(Logged, cls).__new__(cls)
```

### Comparing `python-utils-3.5.2/python_utils/terminal.py` & `python-utils-3.6.0/python_utils/terminal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import os
 import typing
 
 from . import converters
 
 Dimensions = typing.Tuple[int, int]
 OptionalDimensions = typing.Optional[Dimensions]
@@ -16,81 +17,63 @@
 
     Returns:
         width, height: Two integers containing width and height
     '''
     w: typing.Optional[int]
     h: typing.Optional[int]
 
-    try:
+    with contextlib.suppress(Exception):
         # Default to 79 characters for IPython notebooks
         from IPython import get_ipython  # type: ignore
 
         ipython = get_ipython()
         from ipykernel import zmqshell  # type: ignore
 
         if isinstance(ipython, zmqshell.ZMQInteractiveShell):
             return 79, 24
-    except Exception:  # pragma: no cover
-        pass
-
-    try:
+    with contextlib.suppress(Exception):
         # This works for Python 3, but not Pypy3. Probably the best method if
         # it's supported so let's always try
         import shutil
 
         w, h = shutil.get_terminal_size()
         if w and h:
             # The off by one is needed due to progressbars in some cases, for
             # safety we'll always substract it.
             return w - 1, h
-    except Exception:  # pragma: no cover
-        pass
-
-    try:
+    with contextlib.suppress(Exception):
         w = converters.to_int(os.environ.get('COLUMNS'))
         h = converters.to_int(os.environ.get('LINES'))
         if w and h:
             return w, h
-    except Exception:  # pragma: no cover
-        pass
-
-    try:
+    with contextlib.suppress(Exception):
         import blessings  # type: ignore
 
         terminal = blessings.Terminal()
         w = terminal.width
         h = terminal.height
         if w and h:
             return w, h
-    except Exception:  # pragma: no cover
-        pass
-
-    try:
+    with contextlib.suppress(Exception):
         # The method can return None so we don't unpack it
         wh = _get_terminal_size_linux()
         if wh is not None and all(wh):
             return wh
-    except Exception:  # pragma: no cover
-        pass
 
-    try:
+    with contextlib.suppress(Exception):
         # Windows detection doesn't always work, let's try anyhow
         wh = _get_terminal_size_windows()
         if wh is not None and all(wh):
             return wh
-    except Exception:  # pragma: no cover
-        pass
 
-    try:
+    with contextlib.suppress(Exception):
         # needed for window's python in cygwin's xterm!
         wh = _get_terminal_size_tput()
         if wh is not None and all(wh):
             return wh
-    except Exception:  # pragma: no cover
-        pass
 
     return 79, 24
 
 
 def _get_terminal_size_windows() -> OptionalDimensions:  # pragma: no cover
     res = None
     try:
@@ -158,20 +141,18 @@
             )
         except Exception:
             return None
 
     size = ioctl_GWINSZ(0) or ioctl_GWINSZ(1) or ioctl_GWINSZ(2)
 
     if not size:
-        try:
-            fd = os.open(os.ctermid(), os.O_RDONLY)
+        with contextlib.suppress(Exception):
+            fd = os.open(os.ctermid(), os.O_RDONLY)  # type: ignore
             size = ioctl_GWINSZ(fd)
             os.close(fd)
-        except Exception:
-            pass
     if not size:
         try:
             size = os.environ['LINES'], os.environ['COLUMNS']
         except Exception:
             return None
 
     return int(size[1]), int(size[0])
```

### Comparing `python-utils-3.5.2/python_utils/time.py` & `python-utils-3.6.0/python_utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+# pyright: reportUnnecessaryIsInstance=false
 import asyncio
 import datetime
 import functools
 import itertools
 import time
 
 import python_utils
 from python_utils import aio, exceptions, types
 
+_T = types.TypeVar('_T')
+_P = types.ParamSpec('_P')
+
+
 # There might be a better way to get the epoch with tzinfo, please create
 # a pull request if you know a better way that functions for Python 2 and 3
 epoch = datetime.datetime(year=1970, month=1, day=1)
 
 
 def timedelta_to_seconds(delta: datetime.timedelta) -> types.Number:
     '''Convert a timedelta to seconds with the microseconds as fraction
@@ -135,15 +140,17 @@
     else:
         raise TypeError('Unknown type %s: %r' % (type(timestamp), timestamp))
 
 
 def timeout_generator(
     timeout: types.delta_type,
     interval: types.delta_type = datetime.timedelta(seconds=1),
-    iterable: types.Union[types.Iterable, types.Callable] = itertools.count,
+    iterable: types.Union[
+        types.Iterable[_T], types.Callable[[], types.Iterable[_T]]
+    ] = itertools.count,  # type: ignore
     interval_multiplier: float = 1.0,
     maximum_interval: types.Optional[types.delta_type] = None,
 ):
     '''
     Generator that walks through the given iterable (a counter by default)
     until the float_timeout is reached with a configurable float_interval
     between items
@@ -175,15 +182,15 @@
     '''
     float_timeout: float = delta_to_seconds(timeout)
     float_interval: float = delta_to_seconds(interval)
     float_maximum_interval: types.Optional[float] = delta_to_seconds_or_none(
         maximum_interval
     )
 
-    iterable_: types.Iterable
+    iterable_: types.Iterable[_T]
     if callable(iterable):
         iterable_ = iterable()
     else:
         iterable_ = iterable
 
     end = float_timeout + time.perf_counter()
     for item in iterable_:
@@ -198,20 +205,22 @@
         if float_maximum_interval:
             float_interval = min(float_interval, float_maximum_interval)
 
 
 async def aio_timeout_generator(
     timeout: types.delta_type,
     interval: types.delta_type = datetime.timedelta(seconds=1),
-    iterable: types.Union[types.AsyncIterable, types.Callable] = aio.acount,
+    iterable: types.Union[
+        types.AsyncIterable[_T], types.Callable[..., types.AsyncIterable[_T]]
+    ] = aio.acount,
     interval_multiplier: float = 1.0,
     maximum_interval: types.Optional[types.delta_type] = None,
-):
+) -> types.AsyncGenerator[_T, None]:
     '''
-    Aync generator that walks through the given iterable (a counter by
+    Async generator that walks through the given async iterable (a counter by
     default) until the float_timeout is reached with a configurable
     float_interval between items
 
     The interval_exponent automatically increases the float_timeout with each
     run. Note that if the float_interval is less than 1, 1/interval_exponent
     will be used so the float_interval is always growing. To double the
     float_interval with each run, specify 2.
@@ -222,15 +231,15 @@
     '''
     float_timeout: float = delta_to_seconds(timeout)
     float_interval: float = delta_to_seconds(interval)
     float_maximum_interval: types.Optional[float] = delta_to_seconds_or_none(
         maximum_interval
     )
 
-    iterable_: types.AsyncIterable
+    iterable_: types.AsyncIterable[_T]
     if callable(iterable):
         iterable_ = iterable()
     else:
         iterable_ = iterable
 
     end = float_timeout + time.perf_counter()
     async for item in iterable_:  # pragma: no branch
@@ -243,20 +252,30 @@
 
         float_interval *= interval_multiplier
         if float_maximum_interval:  # pragma: no branch
             float_interval = min(float_interval, float_maximum_interval)
 
 
 async def aio_generator_timeout_detector(
-    generator: types.AsyncGenerator,
+    generator: types.AsyncGenerator[_T, None],
     timeout: types.Optional[types.delta_type] = None,
     total_timeout: types.Optional[types.delta_type] = None,
-    on_timeout: types.Optional[types.Callable] = exceptions.reraise,
-    **kwargs,
-):
+    on_timeout: types.Optional[
+        types.Callable[
+            [
+                types.AsyncGenerator[_T, None],
+                types.Optional[types.delta_type],
+                types.Optional[types.delta_type],
+                BaseException,
+            ],
+            types.Any,
+        ]
+    ] = exceptions.reraise,
+    **on_timeout_kwargs: types.Mapping[types.Text, types.Any],
+) -> types.AsyncGenerator[_T, None]:
     '''
     This function is used to detect if an asyncio generator has not yielded
     an element for a set amount of time.
 
     The `on_timeout` argument is called with the `generator`, `timeout`,
     `total_timeout`, `exception` and the extra `**kwargs` to this function as
     arguments.
@@ -282,43 +301,61 @@
                 yield await asyncio.wait_for(generator.__anext__(), timeout_s)
             else:
                 yield await generator.__anext__()
 
         except asyncio.TimeoutError as exception:
             if on_timeout is not None:
                 await on_timeout(
-                    generator, timeout, total_timeout, exception, **kwargs
+                    generator,
+                    timeout,
+                    total_timeout,
+                    exception,
+                    **on_timeout_kwargs,
                 )
             break
 
         except StopAsyncIteration:
             break
 
 
 def aio_generator_timeout_detector_decorator(
     timeout: types.Optional[types.delta_type] = None,
     total_timeout: types.Optional[types.delta_type] = None,
-    on_timeout: types.Optional[types.Callable] = exceptions.reraise,
-    **kwargs,
+    on_timeout: types.Optional[
+        types.Callable[
+            [
+                types.AsyncGenerator[types.Any, None],
+                types.Optional[types.delta_type],
+                types.Optional[types.delta_type],
+                BaseException,
+            ],
+            types.Any,
+        ]
+    ] = exceptions.reraise,
+    **on_timeout_kwargs: types.Mapping[types.Text, types.Any],
 ):
     '''
     A decorator wrapper for aio_generator_timeout_detector.
     '''
 
-    def _timeout_detector_decorator(generator: types.Callable):
+    def _timeout_detector_decorator(
+        generator: types.Callable[_P, types.AsyncGenerator[_T, None]]
+    ) -> types.Callable[_P, types.AsyncGenerator[_T, None]]:
         '''
         The decorator itself.
         '''
 
         @functools.wraps(generator)
-        def wrapper(*args, **wrapper_kwargs):
+        def wrapper(
+            *args: _P.args, **kwargs: _P.kwargs
+        ) -> types.AsyncGenerator[_T, None]:
             return aio_generator_timeout_detector(
-                generator(*args, **wrapper_kwargs),
+                generator(*args, **kwargs),
                 timeout,
                 total_timeout,
                 on_timeout,
-                **kwargs,
+                **on_timeout_kwargs,
             )
 
         return wrapper
 
     return _timeout_detector_decorator
```

### Comparing `python-utils-3.5.2/python_utils/types.py` & `python-utils-3.6.0/python_utils/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
+# pyright: reportWildcardImportFromLibrary=false
 import datetime
 import decimal
-import sys
-from typing import *  # type: ignore # pragma: no cover
+from typing_extensions import *  # type: ignore  # noqa: F403
+from typing import *  # type: ignore  # pragma: no cover  # noqa: F403
+from types import *  # type: ignore  # pragma: no cover  # noqa: F403
 
-# import * does not import Pattern
-from typing import Pattern
-
-if sys.version_info >= (3, 8):  # pragma: no cover
-    from typing import Literal, SupportsIndex
-else:  # pragma: no cover
-    from typing_extensions import Literal, SupportsIndex
+# import * does not import these in all Python versions
+from typing import Pattern, BinaryIO, IO, TextIO, Match
 
 # Quickhand for optional because it gets so much use. If only Python had
 # support for an optional type shorthand such as `SomeType?` instead of
 # `Optional[SomeType]`.
 from typing import Optional as O  # noqa
 
 # Since the Union operator is only supported for Python 3.10, we'll create a
@@ -35,18 +32,14 @@
     datetime.datetime,
     str,
     int,
     float,
     None,
 ]
 
-assert Pattern is not None  # type: ignore
-assert Literal is not None
-assert SupportsIndex is not None
-
 __all__ = [
     'OptionalScope',
     'Number',
     'DecimalNumber',
     'delta_type',
     'timestamp_type',
     # The types from the typing module.
@@ -59,21 +52,23 @@
     'Final',
     'ForwardRef',
     'Generic',
     'Literal',
     'SupportsIndex',
     'Optional',
     'ParamSpec',
+    'ParamSpecArgs',
+    'ParamSpecKwargs',
     'Protocol',
     'Tuple',
     'Type',
     'TypeVar',
     'Union',
     # ABCs (from collections.abc).
-    'AbstractSet',  # collections.abc.Set.
+    'AbstractSet',
     'ByteString',
     'Container',
     'ContextManager',
     'Hashable',
     'ItemsView',
     'Iterable',
     'Iterator',
@@ -130,16 +125,40 @@
     'get_type_hints',
     'is_typeddict',
     'NewType',
     'no_type_check',
     'no_type_check_decorator',
     'NoReturn',
     'overload',
-    'ParamSpecArgs',
-    'ParamSpecKwargs',
     'runtime_checkable',
     'Text',
     'TYPE_CHECKING',
     'TypeAlias',
     'TypeGuard',
     'TracebackType',
+    # Types from the `types` module.
+    'FunctionType',
+    'LambdaType',
+    'CodeType',
+    'MappingProxyType',
+    'SimpleNamespace',
+    'GeneratorType',
+    'CoroutineType',
+    'AsyncGeneratorType',
+    'MethodType',
+    'BuiltinFunctionType',
+    'BuiltinMethodType',
+    'WrapperDescriptorType',
+    'MethodWrapperType',
+    'MethodDescriptorType',
+    'ClassMethodDescriptorType',
+    'ModuleType',
+    'TracebackType',
+    'FrameType',
+    'GetSetDescriptorType',
+    'MemberDescriptorType',
+    'new_class',
+    'resolve_bases',
+    'prepare_class',
+    'DynamicClassAttribute',
+    'coroutine',
 ]
```

### Comparing `python-utils-3.5.2/python_utils.egg-info/PKG-INFO` & `python-utils-3.6.0/python_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.5.2
+Version: 3.6.0
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >3.6.0
+Requires-Python: >3.8.0
 Provides-Extra: loguru
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 Useful Python Utils
 ==============================================================================
@@ -36,14 +36,21 @@
 
  - The source: https://github.com/WoLpH/python-utils
  - Project page: https://pypi.python.org/pypi/python-utils
  - Reporting bugs: https://github.com/WoLpH/python-utils/issues
  - Documentation: https://python-utils.readthedocs.io/en/latest/
  - My blog: https://wol.ph/
 
+Security contact information
+------------------------------------------------------------------------------
+
+To report a security vulnerability, please use the
+`Tidelift security contact <https://tidelift.com/security>`_.
+Tidelift will coordinate the fix and disclosure.
+
 Requirements for installing:
 ------------------------------------------------------------------------------
 
 For the Python 3+ release (i.e. v3.0.0 or higher) there are no requirements.
 For the Python 2 compatible version (v2.x.x) the `six` package is needed.
 
 Installation:
```

### Comparing `python-utils-3.5.2/python_utils.egg-info/SOURCES.txt` & `python-utils-3.6.0/python_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 MANIFEST.in
 README.rst
 coverage.rc
+pyproject.toml
 pytest.ini
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 _python_utils_tests/__init__.py
 _python_utils_tests/requirements.txt
+_python_utils_tests/test_aio.py
 _python_utils_tests/test_containers.py
 _python_utils_tests/test_decorators.py
 _python_utils_tests/test_generators.py
 _python_utils_tests/test_import.py
 _python_utils_tests/test_logger.py
 _python_utils_tests/test_python_utils.py
 _python_utils_tests/test_time.py
```

### Comparing `python-utils-3.5.2/setup.cfg` & `python-utils-3.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-utils-3.5.2/setup.py` & `python-utils-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 if os.path.isfile('README.rst'):
     long_description = open('README.rst').read()
 else:
     long_description = 'See http://pypi.python.org/pypi/python-utils/'
 
 if __name__ == '__main__':
     setuptools.setup(
-        python_requires='>3.6.0',
+        python_requires='>3.8.0',
         name='python-utils',
         version=about['__version__'],
         author=about['__author__'],
         author_email=about['__author_email__'],
         description=about['__description__'],
         url=about['__url__'],
         license='BSD',
         packages=setuptools.find_packages(
             exclude=['_python_utils_tests', '*.__pycache__'],
         ),
         package_data={'python_utils': ['py.typed']},
         long_description=long_description,
-        install_requires=['typing_extensions;python_version<"3.8"'],
+        install_requires=['typing_extensions'],
         tests_require=['pytest'],
         extras_require={
             'loguru': [
                 'loguru',
             ],
             'docs': [
                 'mock',
```

### Comparing `python-utils-3.5.2/tox.ini` & `python-utils-3.6.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [tox]
-envlist = black, py37, py38, py39, py310, py311, pypy3, flake8, docs, mypy, pyright
+envlist = black, py38, py39, py310, py311, flake8, docs, mypy, pyright
 skip_missing_interpreters = True
 
 [testenv]
 basepython =
-    py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
     py311: python3.11
-    pypy: pypy
 
 setenv = PY_IGNORE_IMPORTMISMATCH=1
 deps =
     mypy
     pyright
     -r{toxinidir}/_python_utils_tests/requirements.txt
 commands =
```


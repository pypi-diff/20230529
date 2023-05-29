# Comparing `tmp/configration-2.0.1.tar.gz` & `tmp/configration-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.1.tar", last modified: Mon May 29 08:19:27 2023, max compression
+gzip compressed data, was "configration-2.0.2.tar", last modified: Mon May 29 11:34:47 2023, max compression
```

## Comparing `configration-2.0.1.tar` & `configration-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.985494 configration-2.0.1/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.1/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      826 2023-05-29 08:19:27.985494 configration-2.0.1/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.1/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.982161 configration-2.0.1/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.1/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-29 08:18:04.000000 configration-2.0.1/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.985494 configration-2.0.1/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.1/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1695 2023-05-28 08:11:27.000000 configration-2.0.1/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.1/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      952 2023-05-28 09:53:21.000000 configration-2.0.1/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      948 2023-05-28 09:52:59.000000 configration-2.0.1/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.985494 configration-2.0.1/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.1/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1563 2023-05-28 09:59:14.000000 configration-2.0.1/configration/tests/test_json.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1563 2023-05-28 10:00:21.000000 configration-2.0.1/configration/tests/test_toml.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.985494 configration-2.0.1/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      826 2023-05-29 08:19:27.000000 configration-2.0.1/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      498 2023-05-29 08:19:27.000000 configration-2.0.1/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-29 08:19:27.000000 configration-2.0.1/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-05-29 08:19:27.000000 configration-2.0.1/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-29 08:19:27.985494 configration-2.0.1/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.1/setup.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:19:27.985494 configration-2.0.1/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      205 2023-05-26 07:00:53.000000 configration-2.0.1/tests/test_json.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.2/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      882 2023-05-29 11:34:47.261345 configration-2.0.2/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.2/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.258012 configration-2.0.2/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.2/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-29 11:22:41.000000 configration-2.0.2/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.2/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1951 2023-05-29 11:33:46.000000 configration-2.0.2/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.2/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      952 2023-05-28 09:53:21.000000 configration-2.0.2/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      948 2023-05-28 09:52:59.000000 configration-2.0.2/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.2/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1696 2023-05-29 09:29:59.000000 configration-2.0.2/configration/tests/test_json.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1696 2023-05-29 09:31:39.000000 configration-2.0.2/configration/tests/test_toml.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.258012 configration-2.0.2/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      882 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      498 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-05-29 11:34:47.000000 configration-2.0.2/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-29 11:34:47.261345 configration-2.0.2/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.2/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 11:34:47.261345 configration-2.0.2/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      205 2023-05-26 07:00:53.000000 configration-2.0.2/tests/test_json.py
```

### Comparing `configration-2.0.1/LICENSE.txt` & `configration-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.1/PKG-INFO` & `configration-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.1
+Version: 2.0.2
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 1.0.2 29 May 2023
+
+1. Provide __repr__
+
+------
+
 Version 1.0.1 29 May 2023
 
 1. Expose TomlConfig
 
 ------
 
 Version 1.0.0 29 May 2023
```

### Comparing `configration-2.0.1/configration/src/config.py` & `configration-2.0.2/configration/src/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,22 @@
     def __init__(self, path: str, attrs: dict[str, list[type]] = {}):
         self.path = path
         self.attrs = attrs
         self.config = self._get_config()
         for key, item in self.config.items():
             self.__dict__[key] = item
 
+    def __repr__(self):
+        if not self.attrs:
+            return str(self.__dict__)
+        output = ['Config:']
+        for key, item in self.attrs.items():
+            output .append(f'{key}, {self.__dict__[key]}')
+        return '\n'.join(output)
+
     def _get_config(self) -> dict[str, object]:
         # Return config, if contents are valid.
         config = self._read_config()
 
         if not self.attrs:
             return config
```

### Comparing `configration-2.0.1/configration/src/json_config.py` & `configration-2.0.2/configration/src/json_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.1/configration/src/toml_config.py` & `configration-2.0.2/configration/src/toml_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.1/configration/tests/test_json.py` & `configration-2.0.2/configration/tests/test_json.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,46 +4,48 @@
 from ..src.json_config import JsonConfig
 
 CONFIG_ATTRS = {
     'period_start_month': [int],
     'payment_bbo': [int, float],
     'period_months': [int],
 }
+ANSI_COLOR_RED = "\x1b[31m"
+ANSI_COLOR_RESET = "\x1b[0m"
 
 
 def test_config_structure():
     path = Path('tests', 'test_data', 'config.json')
     config = JsonConfig(path)
     assert isinstance(config.config, dict)
     assert len(config.config) == 3
 
 
 def test_config_missing(capsys):
     path = Path('tests', 'test_data', 'not_a_file.json')
     err_msg = f'The config file is not in the expected location: {path}'
     JsonConfig(path)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_invalid_attrs(capsys):
     path = Path('tests', 'test_data', 'config_invalid_attrs.json')
     err_msg = "Corrupt config file. period_start_month not of type [<class 'int'>]"
     JsonConfig(path, CONFIG_ATTRS)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_invalid_json(capsys):
     path = Path('tests', 'test_data', 'config_invalid_json.json')
     err_msg = f"Invalid json format in {path}"
     JsonConfig(path)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_missing_attr(capsys):
     path = Path('tests', 'test_data', 'config_missing_attr.json')
     err_msg = f"Corrupt config file. Missing attribute: payment_bbo"
     JsonConfig(path, CONFIG_ATTRS)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
```

### Comparing `configration-2.0.1/configration/tests/test_toml.py` & `configration-2.0.2/configration/tests/test_toml.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,46 +4,48 @@
 from ..src.toml_config import TomlConfig
 
 CONFIG_ATTRS = {
     'period_start_month': [int],
     'payment_bbo': [int, float],
     'period_months': [int],
 }
+ANSI_COLOR_RED = "\x1b[31m"
+ANSI_COLOR_RESET = "\x1b[0m"
 
 
 def test_config_structure():
     path = Path('tests', 'test_data', 'config.toml')
     config = TomlConfig(path)
     assert isinstance(config.config, dict)
     assert len(config.config) == 3
 
 
 def test_config_missing(capsys):
     path = Path('tests', 'test_data', 'not_a_file.toml')
     err_msg = f'The config file is not in the expected location: {path}'
     TomlConfig(path)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_invalid_attrs(capsys):
     path = Path('tests', 'test_data', 'config_invalid_attrs.toml')
     err_msg = "Corrupt config file. period_start_month not of type [<class 'int'>]"
     TomlConfig(path, CONFIG_ATTRS)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_invalid_json(capsys):
     path = Path('tests', 'test_data', 'config_invalid_toml.toml')
     err_msg = f"Invalid toml format in {path}"
     TomlConfig(path)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
 
 
 def test_config_missing_attr(capsys):
     path = Path('tests', 'test_data', 'config_missing_attr.toml')
     err_msg = f"Corrupt config file. Missing attribute: payment_bbo"
     TomlConfig(path, CONFIG_ATTRS)
     captured = capsys.readouterr()
-    assert captured.out.strip() == f'\x1b[31m{err_msg}\x1b[0m'
+    assert captured.out.strip() == f'{ANSI_COLOR_RED}{err_msg}{ANSI_COLOR_RESET}'
```

### Comparing `configration-2.0.1/configration.egg-info/PKG-INFO` & `configration-2.0.2/configration.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.1
+Version: 2.0.2
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 1.0.2 29 May 2023
+
+1. Provide __repr__
+
+------
+
 Version 1.0.1 29 May 2023
 
 1. Expose TomlConfig
 
 ------
 
 Version 1.0.0 29 May 2023
```

### Comparing `configration-2.0.1/setup.py` & `configration-2.0.2/setup.py`

 * *Files identical despite different names*


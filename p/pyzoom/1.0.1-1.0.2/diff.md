# Comparing `tmp/pyzoom-1.0.1.tar.gz` & `tmp/pyzoom-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzoom-1.0.1.tar", max compression
+gzip compressed data, was "pyzoom-1.0.2.tar", max compression
```

## Comparing `pyzoom-1.0.1.tar` & `pyzoom-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4771 2023-05-28 20:51:01.282510 pyzoom-1.0.1/README.md
--rw-r--r--   0        0        0      567 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       84 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/__init__.py
--rw-r--r--   0        0        0     4534 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/_base.py
--rw-r--r--   0        0        0     7287 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/_client.py
--rw-r--r--   0        0        0      438 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/err.py
--rw-r--r--   0        0        0     1425 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/oauth.py
--rw-r--r--   0        0        0     4856 2023-05-28 20:51:01.282510 pyzoom-1.0.1/pyzoom/schemas.py
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 pyzoom-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5113 2023-05-28 21:03:54.454478 pyzoom-1.0.2/README.md
+-rw-r--r--   0        0        0      567 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/__init__.py
+-rw-r--r--   0        0        0     4534 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/_base.py
+-rw-r--r--   0        0        0     7287 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/_client.py
+-rw-r--r--   0        0        0      438 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/err.py
+-rw-r--r--   0        0        0     2869 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/oauth.py
+-rw-r--r--   0        0        0     4856 2023-05-28 21:03:54.454478 pyzoom-1.0.2/pyzoom/schemas.py
+-rw-r--r--   0        0        0     5963 1970-01-01 00:00:00.000000 pyzoom-1.0.2/PKG-INFO
```

### Comparing `pyzoom-1.0.1/README.md` & `pyzoom-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,24 @@
 Using [poetry](https://python-poetry.org/):
 
 `poetry add pyzoom`
 
 ## OAUTH Authorization
 I have provided some functions to ease the flow of getting all the tokens. You will need your Zoom App's `Client ID` and `Client Secret`.
 
+### Requesting Tokens
+Once your user has accepted integration on the zoom side and you received the code from the redirect:
+
+```python
+from pyzoom import request_tokens
+
+tokens = request_tokens("APP_CLIENT_ID", "APP_CLIENT_SECRET", "APP_REDIRECT_URL", "CALLBACK_CODE"):
+```
+The result of a successful request will be a map with the tokens. 
+
 ### Refreshing tokens
 
 ```python
 from pyzoom import refresh_tokens
 
 tokens = refresh_tokens("APP_CLIEN_ID", "APP_CLIENT_SECRET", "USER_REFRESH_TOKEN")
 ```
```

### Comparing `pyzoom-1.0.1/pyproject.toml` & `pyzoom-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyzoom"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python wrapper for Zoom Video API"
 authors = ["MB <mb@blaster.ai>"]
 license = "MIT"
 readme='README.md'
 homepage='https://github.com/licht1stein/pyzoom'
 
 [tool.poetry.dependencies]
```

### Comparing `pyzoom-1.0.1/pyzoom/_base.py` & `pyzoom-1.0.2/pyzoom/_base.py`

 * *Files identical despite different names*

### Comparing `pyzoom-1.0.1/pyzoom/_client.py` & `pyzoom-1.0.2/pyzoom/_client.py`

 * *Files identical despite different names*

### Comparing `pyzoom-1.0.1/pyzoom/schemas.py` & `pyzoom-1.0.2/pyzoom/schemas.py`

 * *Files identical despite different names*

### Comparing `pyzoom-1.0.1/PKG-INFO` & `pyzoom-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzoom
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper for Zoom Video API
 Home-page: https://github.com/licht1stein/pyzoom
 License: MIT
 Author: MB
 Author-email: mb@blaster.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,14 +53,24 @@
 Using [poetry](https://python-poetry.org/):
 
 `poetry add pyzoom`
 
 ## OAUTH Authorization
 I have provided some functions to ease the flow of getting all the tokens. You will need your Zoom App's `Client ID` and `Client Secret`.
 
+### Requesting Tokens
+Once your user has accepted integration on the zoom side and you received the code from the redirect:
+
+```python
+from pyzoom import request_tokens
+
+tokens = request_tokens("APP_CLIENT_ID", "APP_CLIENT_SECRET", "APP_REDIRECT_URL", "CALLBACK_CODE"):
+```
+The result of a successful request will be a map with the tokens. 
+
 ### Refreshing tokens
 
 ```python
 from pyzoom import refresh_tokens
 
 tokens = refresh_tokens("APP_CLIEN_ID", "APP_CLIENT_SECRET", "USER_REFRESH_TOKEN")
 ```
```


# Comparing `tmp/binance-c2c-sapi-sdk-0.0.3.tar.gz` & `tmp/binance-c2c-sapi-sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-c2c-sapi-sdk-0.0.3.tar", last modified: Sun May 28 21:32:49 2023, max compression
+gzip compressed data, was "binance-c2c-sapi-sdk-0.0.4.tar", last modified: Mon May 29 06:26:22 2023, max compression
```

## Comparing `binance-c2c-sapi-sdk-0.0.3.tar` & `binance-c2c-sapi-sdk-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:32:49.602212 binance-c2c-sapi-sdk-0.0.3/
--rw-rw-rw-   0        0        0      607 2023-05-28 21:32:49.601206 binance-c2c-sapi-sdk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 binance-c2c-sapi-sdk-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:32:49.576205 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi/__init__.py
--rw-rw-rw-   0        0        0     7591 2023-05-28 18:40:23.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi/api.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:32:49.599206 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/
--rw-rw-rw-   0        0        0      607 2023-05-28 21:32:49.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-28 21:32:49.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:32:49.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 21:32:49.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 21:32:49.000000 binance-c2c-sapi-sdk-0.0.3/binance_c2c_sapi_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:32:49.602212 binance-c2c-sapi-sdk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-05-28 21:32:44.000000 binance-c2c-sapi-sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:26:22.060703 binance-c2c-sapi-sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:26:22.060703 binance-c2c-sapi-sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 06:26:07.000000 binance-c2c-sapi-sdk-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:26:22.060703 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 06:26:07.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-29 06:26:07.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:26:22.060703 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:26:22.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 06:26:22.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:26:22.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 06:26:22.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 06:26:22.000000 binance-c2c-sapi-sdk-0.0.4/binance_c2c_sapi_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:26:22.060703 binance-c2c-sapi-sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-29 06:26:07.000000 binance-c2c-sapi-sdk-0.0.4/setup.py
```

### Comparing `binance-c2c-sapi-sdk-0.0.3/README.md` & `binance-c2c-sapi-sdk-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# Binance API Python Wrapper
-
-This is a Python wrapper for the Binance API, providing convenient methods to interact with various endpoints of the Binance API.
-
-## Installation
-
-To use this wrapper, you'll need Python 3.6 or above. Clone the repository and install the required dependencies using pip:
-
-```shell
-git clone https://github.com/your-username/binance-api-python-wrapper.git
-cd binance-api-python-wrapper
-pip install -r requirements.txt
-```
-
-## Usage
-
-1. Import the `BinanceAPI` class:
-
-```python
-from binance_api import BinanceAPI
-```
-
-2. Create an instance of the BinanceAPI class by providing your Binance API key and secret:
-
-```python
-api_key = 'YOUR_API_KEY'
-api_secret = 'YOUR_API_SECRET'
-
-bn = BinanceAPI(api_key, api_secret)
-```
-
-3. Use the available methods to interact with the Binance API. For example, to search for advertisements:
-
-```python
-ads = bn.search_ads("BTC", "GBP", "BUY")
-print(ads)
-```
-
-4. Refer to the docstrings in the code for detailed information about each method, including arguments and return values.
-
-## Disclaimer
-This project is provided as-is and is not affiliated with or endorsed by Binance. Use it at your own risk.
+# Binance API Python Wrapper
+
+This is a Python wrapper for the Binance API, providing convenient methods to interact with various endpoints of the Binance API.
+
+## Installation
+
+To use this wrapper, you'll need Python 3.6 or above. Clone the repository and install the required dependencies using pip:
+
+```shell
+git clone https://github.com/your-username/binance-api-python-wrapper.git
+cd binance-api-python-wrapper
+pip install -r requirements.txt
+```
+
+## Usage
+
+1. Import the `BinanceAPI` class:
+
+```python
+from binance_api import BinanceAPI
+```
+
+2. Create an instance of the BinanceAPI class by providing your Binance API key and secret:
+
+```python
+api_key = 'YOUR_API_KEY'
+api_secret = 'YOUR_API_SECRET'
+
+bn = BinanceAPI(api_key, api_secret)
+```
+
+3. Use the available methods to interact with the Binance API. For example, to search for advertisements:
+
+```python
+ads = bn.search_ads("BTC", "GBP", "BUY")
+print(ads)
+```
+
+4. Refer to the docstrings in the code for detailed information about each method, including arguments and return values.
+
+## Disclaimer
+This project is provided as-is and is not affiliated with or endorsed by Binance. Use it at your own risk.
```

### Comparing `binance-c2c-sapi-sdk-0.0.3/setup.py` & `binance-c2c-sapi-sdk-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.0.3'
-DESCRIPTION = 'Binance C2C SAPI Wrapper'
-LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
-
-# Setting up
-setup(
-    name="binance-c2c-sapi-sdk",
-    version=VERSION,
-    author="Richard",
-    author_email="<rich_swainson@hotmail.co.uk>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    install_requires=['requests'],
-    keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = '0.0.4'
+DESCRIPTION = 'Binance C2C SAPI Wrapper'
+LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
+
+# Setting up
+setup(
+    name="binance-c2c-sapi-sdk",
+    version=VERSION,
+    author="Richard",
+    author_email="<rich_swainson@hotmail.co.uk>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=['requests'],
+    keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```


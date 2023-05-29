# Comparing `tmp/cs-binance-c2c-sapi-0.0.2.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.2.tar", last modified: Mon May 29 06:52:01 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.3.tar", last modified: Mon May 29 09:28:44 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.2.tar` & `cs-binance-c2c-sapi-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.314126 cs-binance-c2c-sapi-0.0.2/
--rw-rw-rw-   0        0        0      606 2023-05-29 06:52:01.307834 cs-binance-c2c-sapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.277746 cs-binance-c2c-sapi-0.0.2/binance_c2c/
--rw-rw-rw-   0        0        0       27 2023-05-29 06:50:57.000000 cs-binance-c2c-sapi-0.0.2/binance_c2c/__init__.py
--rw-rw-rw-   0        0        0     7386 2023-05-29 06:32:10.000000 cs-binance-c2c-sapi-0.0.2/binance_c2c/api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.307834 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      606 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 06:52:01.314126 cs-binance-c2c-sapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-29 06:51:57.000000 cs-binance-c2c-sapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:28:43.997518 cs-binance-c2c-sapi-0.0.3/
+-rw-rw-rw-   0        0        0      606 2023-05-29 09:28:43.996099 cs-binance-c2c-sapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 09:28:43.977224 cs-binance-c2c-sapi-0.0.3/binance_c2c/
+-rw-rw-rw-   0        0        0       27 2023-05-29 06:50:57.000000 cs-binance-c2c-sapi-0.0.3/binance_c2c/__init__.py
+-rw-rw-rw-   0        0        0     7687 2023-05-29 09:28:10.000000 cs-binance-c2c-sapi-0.0.3/binance_c2c/api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 09:28:43.992000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-05-29 09:28:43.000000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-29 09:28:43.000000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 09:28:43.000000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 09:28:43.000000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 09:28:43.000000 cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 09:28:43.998526 cs-binance-c2c-sapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-29 09:28:16.000000 cs-binance-c2c-sapi-0.0.3/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.2/PKG-INFO` & `cs-binance-c2c-sapi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.2/README.md` & `cs-binance-c2c-sapi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.2/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.3/binance_c2c/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         except requests.exceptions.Timeout:
             # Handle timeouts
             print("The request timed out")
         except requests.exceptions.TooManyRedirects:
             # Handle TooManyRedirects
             print("Too many redirects")
         except requests.exceptions.RequestException as e:
-            # Catch any other exceptions
+            print("Status Code: ", response.status_code)
+            print("Response Text: ", response.text)
             print("An error occurred: ", e)
             raise SystemExit(e)
 
         try:
             data = response.json()
         except ValueError:
             print("Error: Unable to parse JSON response")
@@ -214,7 +215,14 @@
         Args:
             file_name (str): File name.
             data (dict): Data to be saved.
         """
         with open(f'./json/{file_name}.json', 'w') as f:
             json.dump(data, f, indent=4)
 
+
+if __name__ == "__main__":
+    import os
+    from dotenv import load_dotenv
+    load_dotenv()
+    bn = BinanceAPI(os.getenv("BINANCE_API_KEY"), os.getenv("BINANCE_API_SECRET"))
+    bn.get_order_details("20495432379774300160")
```

### Comparing `cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.3/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.2/setup.py` & `cs-binance-c2c-sapi-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```


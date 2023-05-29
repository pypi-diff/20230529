# Comparing `tmp/cs-binance-c2c-sapi-0.0.6.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.6.tar", last modified: Mon May 29 11:13:05 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.7.tar", last modified: Mon May 29 17:55:17 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.6.tar` & `cs-binance-c2c-sapi-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:13:05.016173 cs-binance-c2c-sapi-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 11:13:05.016173 cs-binance-c2c-sapi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 11:12:50.000000 cs-binance-c2c-sapi-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:13:05.012173 cs-binance-c2c-sapi-0.0.6/binance_c2c/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 11:12:50.000000 cs-binance-c2c-sapi-0.0.6/binance_c2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-29 11:12:50.000000 cs-binance-c2c-sapi-0.0.6/binance_c2c/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:13:05.012173 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 11:13:05.000000 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-29 11:13:05.000000 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:13:05.000000 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 11:13:05.000000 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 11:13:05.000000 cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:13:05.016173 cs-binance-c2c-sapi-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 11:12:50.000000 cs-binance-c2c-sapi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/binance_c2c/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/binance_c2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/binance_c2c/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:55:17.000000 cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:55:17.296864 cs-binance-c2c-sapi-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 17:55:06.000000 cs-binance-c2c-sapi-0.0.7/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.6/PKG-INFO` & `cs-binance-c2c-sapi-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.6/README.md` & `cs-binance-c2c-sapi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.6/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.7/binance_c2c/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,27 +58,27 @@
             params (dict, optional): Request parameters. Defaults to {}.
             body_params (dict, optional): Request body parameters. Defaults to None.
 
         Returns:
             dict: Response data in JSON format.
         """
         url = f'{self.BASE_URL}{endpoint}'
-        params['timestamp'] = self.get_server_time()
-        params['signature'] = self.create_signature(params)
+        server_time = self.get_server_time()
 
+        params = {
+            'timestamp': server_time
+        }
+
+        signature = self.create_signature(params)
+        params['signature'] = signature
 
         headers = {
             'X-MBX-APIKEY': self.api_key,
             'Content-Type': 'application/json'
         }
-
-        print("URL: ", url)
-        print("Headers: ", headers)
-        print("Request parameters: ", params)
-        print("Body parameters: ", body_params)
         try:
             if method == 'GET':
                 response = requests.get(url, headers=headers, params=params)
             elif method == 'POST':
                 response = requests.post(
                     url, headers=headers, params=params, data=json.dumps(body_params))
             response.raise_for_status()  # Check for successful request
@@ -86,18 +86,14 @@
             # Handle timeouts
             print("The request timed out")
         except requests.exceptions.TooManyRedirects:
             # Handle TooManyRedirects
             print("Too many redirects")
         except requests.exceptions.RequestException as e:
             # If an error occurred during the request, print out some debug information
-            print("URL: ", url)
-            print("Headers: ", headers)
-            print("Params: ", params)
-            print("Body Params: ", body_params)
             print("Status Code: ", response.status_code)
             print("Response Text: ", response.text)
             print("An error occurred: ", e)
             raise SystemExit(e)
 
         try:
             data = response.json()
@@ -226,13 +222,16 @@
             file_name (str): File name.
             data (dict): Data to be saved.
         """
         with open(f'./json/{file_name}.json', 'w') as f:
             json.dump(data, f, indent=4)
 
 
-# if __name__ == "__main__":
-#     import os
-#     from dotenv import load_dotenv
-#     load_dotenv()
-#     bn = BinanceAPI(os.getenv("BINANCE_API_KEY"), os.getenv("BINANCE_API_SECRET"))
-#     print(bn.get_order_details("20495432379774300160"))
+if __name__ == "__main__":
+    import os
+    from dotenv import load_dotenv
+    load_dotenv()
+    bn = BinanceAPI(os.getenv("BINANCE_API_KEY"), os.getenv("BINANCE_API_SECRET"))
+    print(bn.get_order_details("20495432379774300160"))
+    print(bn.get_order_details("20495432379774300160"))
+    print(bn.get_order_details("20495432379774300160"))
+    print(bn.get_order_details("20495432379774300160"))
```

### Comparing `cs-binance-c2c-sapi-0.0.6/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.7/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.6/setup.py` & `cs-binance-c2c-sapi-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```


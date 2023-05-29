# Comparing `tmp/cs-binance-c2c-sapi-0.0.4.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.4.tar", last modified: Mon May 29 09:37:21 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.5.tar", last modified: Mon May 29 10:29:00 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.4.tar` & `cs-binance-c2c-sapi-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:37:21.746793 cs-binance-c2c-sapi-0.0.4/
--rw-rw-rw-   0        0        0      606 2023-05-29 09:37:21.745421 cs-binance-c2c-sapi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 09:37:21.715185 cs-binance-c2c-sapi-0.0.4/binance_c2c/
--rw-rw-rw-   0        0        0       27 2023-05-29 06:50:57.000000 cs-binance-c2c-sapi-0.0.4/binance_c2c/__init__.py
--rw-rw-rw-   0        0        0     8109 2023-05-29 09:36:16.000000 cs-binance-c2c-sapi-0.0.4/binance_c2c/api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:37:21.744288 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      606 2023-05-29 09:37:21.000000 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-29 09:37:21.000000 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:37:21.000000 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 09:37:21.000000 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 09:37:21.000000 cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 09:37:21.746793 cs-binance-c2c-sapi-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-29 09:37:07.000000 cs-binance-c2c-sapi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:29:00.467281 cs-binance-c2c-sapi-0.0.5/
+-rw-rw-rw-   0        0        0      606 2023-05-29 10:29:00.466280 cs-binance-c2c-sapi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 10:29:00.446623 cs-binance-c2c-sapi-0.0.5/binance_c2c/
+-rw-rw-rw-   0        0        0       27 2023-05-29 06:50:57.000000 cs-binance-c2c-sapi-0.0.5/binance_c2c/__init__.py
+-rw-rw-rw-   0        0        0     8960 2023-05-29 10:27:38.000000 cs-binance-c2c-sapi-0.0.5/binance_c2c/api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:29:00.463808 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-05-29 10:29:00.000000 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-29 10:29:00.000000 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:29:00.000000 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 10:29:00.000000 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 10:29:00.000000 cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:29:00.467281 cs-binance-c2c-sapi-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-29 10:28:58.000000 cs-binance-c2c-sapi-0.0.5/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.4/PKG-INFO` & `cs-binance-c2c-sapi-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.4/README.md` & `cs-binance-c2c-sapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.4/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.5/binance_c2c/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import hashlib
 import hmac
 import json
+import datetime
 
 
 class BinanceAPI:
     BASE_URL = 'https://api.binance.com'
 
     def __init__(self, api_key, api_secret):
         """
@@ -25,14 +26,24 @@
         Returns:
             int: Server time in milliseconds.
         """
         url = f'{self.BASE_URL}/api/v3/time'
         response = requests.get(url)
         response.raise_for_status()  # Check for successful request
         return response.json()['serverTime']
+    
+    @staticmethod
+    def get_current_time():
+        """
+        Get the current time in milliseconds.
+        
+        Returns:
+            int: Current time in milliseconds.
+        """
+        return int(datetime.datetime.now().timestamp() * 1000)
 
     def create_signature(self, params):
         """
         Create a signature for API authentication.
 
         Args:
             params (dict): Request parameters.
@@ -43,14 +54,36 @@
         query_string = '&'.join([f'{k}={v}' for k, v in params.items()])
         signature = hmac.new(
             self.api_secret.encode('utf-8'),
             query_string.encode('utf-8'),
             hashlib.sha256
         ).hexdigest()
         return signature
+    
+    def make_c2c_request(self, endpoint, body_params):
+        url = f'https://api.binance.com{endpoint}'
+        server_time = self.get_server_time()
+
+        params = {
+            'timestamp': server_time
+        }
+
+        signature = self.create_signature(params)
+        params['signature'] = signature
+
+        headers = {
+            'X-MBX-APIKEY': self.api_key,
+            'Content-Type': 'application/json'
+        }
+
+        if body_params:
+            response = requests.post(url, headers=headers,
+                                     params=params, data=json.dumps(body_params))
+
+        return response.json()
 
     def make_request(self, method, endpoint, params={}, body_params=None):
         """
         Make a request to the Binance API.
 
         Args:
             method (str): HTTP method ('GET' or 'POST').
@@ -58,27 +91,27 @@
             params (dict, optional): Request parameters. Defaults to {}.
             body_params (dict, optional): Request body parameters. Defaults to None.
 
         Returns:
             dict: Response data in JSON format.
         """
         url = f'{self.BASE_URL}{endpoint}'
-        params['timestamp'] = self.get_server_time()
-        params['signature'] = self.create_signature(params)
 
+        params = {
+            'timestamp': self.get_server_time()
+        }
+
+        signature = self.create_signature(params)
+        params['signature'] = signature
 
         headers = {
             'X-MBX-APIKEY': self.api_key,
             'Content-Type': 'application/json'
         }
 
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
@@ -86,20 +119,14 @@
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
-            print("Status Code: ", response.status_code)
-            print("Response Text: ", response.text)
             print("An error occurred: ", e)
             raise SystemExit(e)
 
         try:
             data = response.json()
         except ValueError:
             print("Error: Unable to parse JSON response")
@@ -231,8 +258,13 @@
 
 
 if __name__ == "__main__":
     import os
     from dotenv import load_dotenv
     load_dotenv()
     bn = BinanceAPI(os.getenv("BINANCE_API_KEY"), os.getenv("BINANCE_API_SECRET"))
-    print(bn.get_order_details("20495432379774300160"))
+    print(bn.get_order_details("20495432379774300160"))
+    print(bn.get_order_details("20495432379774300160"))
+    # msgs = bn.get_messages("20495432379774300160")
+    # msgs = bn.get_messages("20495432379774300160")
+    order_list = bn.get_order_list({"page": 1, "rows": 100})
+    order_list = bn.get_order_list({"page": 1, "rows": 100})
```

### Comparing `cs-binance-c2c-sapi-0.0.4/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.5/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.4/setup.py` & `cs-binance-c2c-sapi-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```


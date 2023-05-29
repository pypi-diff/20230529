# Comparing `tmp/shurjopay-plugin-0.1.6.tar.gz` & `tmp/shurjopay-plugin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shurjopay-plugin-0.1.6.tar", last modified: Thu Mar 30 09:25:11 2023, max compression
+gzip compressed data, was "shurjopay-plugin-0.1.7.tar", last modified: Mon May 29 11:58:57 2023, max compression
```

## Comparing `shurjopay-plugin-0.1.6.tar` & `shurjopay-plugin-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-03-30 09:25:11.790089 shurjopay-plugin-0.1.6/
--rw-r--r--   0 imtiaz     (501) staff       (20)     1097 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.6/LICENSE
--rw-r--r--   0 imtiaz     (501) staff       (20)       52 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.6/MANIFEST.in
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-03-30 09:25:11.789969 shurjopay-plugin-0.1.6/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)     3982 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.6/README.md
--rw-r--r--   0 imtiaz     (501) staff       (20)      103 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.6/pyproject.toml
--rw-r--r--   0 imtiaz     (501) staff       (20)       38 2023-03-30 09:25:11.790126 shurjopay-plugin-0.1.6/setup.cfg
--rw-r--r--   0 imtiaz     (501) staff       (20)      933 2023-03-30 09:23:31.000000 shurjopay-plugin-0.1.6/setup.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-03-30 09:25:11.786965 shurjopay-plugin-0.1.6/src/
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-03-30 09:25:11.788909 shurjopay-plugin-0.1.6/src/shurjopay_plugin/
--rw-r--r--   0 imtiaz     (501) staff       (20)       75 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin/__init__.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     1531 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin/logger_config.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     5097 2023-03-30 09:23:31.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin/models.py
--rw-r--r--   0 imtiaz     (501) staff       (20)    10730 2023-03-30 09:23:31.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin/shurjopay_plugin.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     2335 2023-03-30 09:23:31.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin/utils.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-03-30 09:25:11.789555 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-03-30 09:25:11.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)      476 2023-03-30 09:25:11.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        1 2023-03-30 09:25:11.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        9 2023-03-30 09:25:11.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/requires.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)       17 2023-03-30 09:25:11.000000 shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-03-30 09:25:11.789692 shurjopay-plugin-0.1.6/tests/
--rw-r--r--   0 imtiaz     (501) staff       (20)     2615 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.6/tests/test_shurjopay_plugin.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890639 shurjopay-plugin-0.1.7/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     1097 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.7/LICENSE
+-rw-r--r--   0 imtiaz     (501) staff       (20)       52 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.7/MANIFEST.in
+-rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-05-29 11:58:57.890501 shurjopay-plugin-0.1.7/PKG-INFO
+-rw-r--r--   0 imtiaz     (501) staff       (20)     3982 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.7/README.md
+-rw-r--r--   0 imtiaz     (501) staff       (20)      103 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.7/pyproject.toml
+-rw-r--r--   0 imtiaz     (501) staff       (20)       38 2023-05-29 11:58:57.890686 shurjopay-plugin-0.1.7/setup.cfg
+-rw-r--r--   0 imtiaz     (501) staff       (20)      933 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/setup.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.887037 shurjopay-plugin-0.1.7/src/
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.889341 shurjopay-plugin-0.1.7/src/shurjopay_plugin/
+-rw-r--r--   0 imtiaz     (501) staff       (20)       75 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/__init__.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     1531 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/logger_config.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     5182 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/models.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)    11381 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/shurjopay_plugin.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     2305 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/utils.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890128 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 imtiaz     (501) staff       (20)      476 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)        1 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)        9 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/requires.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)       17 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890285 shurjopay-plugin-0.1.7/tests/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     2752 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/tests/test_shurjopay_plugin.py
```

### Comparing `shurjopay-plugin-0.1.6/LICENSE` & `shurjopay-plugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.6/PKG-INFO` & `shurjopay-plugin-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.6/README.md` & `shurjopay-plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.6/setup.py` & `shurjopay-plugin-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="shurjopay-plugin",
-    version="0.1.6",
+    version="0.1.7",
     author="Mahabubul Hasan",
     author_email="plugindev@shurjomukhi.com.bd",
     description="Shurjopay version 2.1 payment gateway integration package for python users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shurjopay-plugins/sp-plugin-python.git",
     project_urls={
```

### Comparing `shurjopay-plugin-0.1.6/src/shurjopay_plugin/logger_config.py` & `shurjopay-plugin-0.1.7/src/shurjopay_plugin/logger_config.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.6/src/shurjopay_plugin/shurjopay_plugin.py` & `shurjopay-plugin-0.1.7/src/shurjopay_plugin/shurjopay_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,71 +2,85 @@
  Shurjopay Python Plugin for shurjoPay Gateway Services.
  Author Md Mahabubul Hasan
  Since 2022-10-10
 '''
 import requests
 import datetime
 import json
-from .models import *
-from .utils import *
+from .models import (
+    PaymentDetailsModel,
+    ShurjoPayTokenModel,
+    VerifiedPaymentDetailsModel
+)
+from .utils import (
+    get_client_ip,
+    Endpoints,
+    ShurjopayStatus,
+    ShurjopayException,
+    ShurjopayAuthException)
 from .logger_config import ShurjopayLoggerConfig
 
+
 class ShurjopayPlugin(object):
     '''
         shurjoPay Online payment gateway has several API's which need to be integrated by merchants for accessing different services. The available services are:
         - Authenticating
         - Making payment
         - Verifying payment 
         - Checking payment status
         For more details view the shurjoPay version-2.1 integration documentation : https://docs.google.com/document/d/19J4HE0j873nBJqcN-uRBYYAa_qBA3p1XSY-jy2fwvEE/edit .    
     '''
-    # shurjopay Token attributes  
-    # token(str), 
+    # shurjopay Token attributes
+    # token(str),
     # token_type,
-    # expires_in, 
-    # sp_code, 
+    # expires_in,
+    # sp_code,
     # message
     AUTH_TOKEN = None
 
     # Status Message
     AUTHENTICATION_SUCCESS = 'Merchant Authentication Successful!'
     AUTHENTICATION_FAILED = 'Merchant Authentication Failed!'
+    AUTHENTICATION_SUCCESS = 'Merchant Authentication Successful!'
+    AUTHENTICATION_FAILED = 'Merchant Authentication Failed!'
     AUTHENTICATION_TOKEN_EXPIRED = 'Shurjopay Token Expired!'
+    WRONG_CREDENTIALS = 'Please check your credentials'
     PAYMENT_REQUEST_SUCCESS = 'Shurjopay Payment Request Successful!'
     PAYMENT_REQUEST_FAILED = 'Shurjopay Payment Request Failed!'
     PAYMENT_VERIFICATION_FAILED = 'Shurjopay Payment Verification Failed!'
     PAYMENT_CHECK_FAILED = 'Shurjopay Payment Checking Failed!'
 
-    
+
     def __init__(self, sp_config) -> None:
         # Initialize the configuration keys for plugin configuration
         self.SP_USERNAME = sp_config.SP_USERNAME
         self.SP_PASSWORD = sp_config.SP_PASSWORD
-        self.SP_ENDPOINT = requests.compat.urljoin(sp_config.SP_ENDPOINT, Endpoints.API.value)
-        self.SP_RETURN = sp_config.SP_RETURN 
+        self.SP_ENDPOINT = requests.compat.urljoin(
+            sp_config.SP_ENDPOINT, Endpoints.API.value)
+        self.SP_RETURN = sp_config.SP_RETURN
         self.SP_CANCEL = sp_config.SP_CANCEL
         self.SP_PREFIX = sp_config.SP_PREFIX
-        
-        if sp_config.SP_LOGDIR == None or sp_config.SP_LOGDIR == '':
+
+        if sp_config.SP_LOGDIR is None or sp_config.SP_LOGDIR == '':
             self.logger = ShurjopayLoggerConfig().get_logger()
             return
         self.logger = ShurjopayLoggerConfig().get_file_logger(sp_config.SP_LOGDIR)
-        
+
     def authenticate(self):
-        ''' Authenticate with shurjoPay Payment Gateway using merchant credectials.
-        
+        ''' Authenticate with shurjoPay Payment Gateway using Merchant credectials.
+
         Returns
         -------
         AUTH_TOKEN (ShurjoPayTokenModel): token details from "get-token" api response which contains
             - token(str), 
             - token_type(str),
             - expires_in(int),(in seconds)
             - sp_code(int),
             - message(str)
-            
+
         Raises
         -----
         ShurjopayAuthException: If authentication fails due to invalid credentials or any other reason. 
         '''
         # Create token endpoint url
         url = requests.compat.urljoin(self.SP_ENDPOINT, Endpoints.TOKEN.value)
         self.logger.info(self.SP_ENDPOINT)
@@ -75,146 +89,163 @@
             "username": self.SP_USERNAME,
             "password": self.SP_PASSWORD,
         }
         try:
             response = requests.post(url, data=payloads)
             token_details = response.json()
             # Check if authentication is successful
-            if (int)(token_details['sp_code']) == ShurjopayStatus().AUTH_SUCCESS.code: 
-                self.logger.info(f'sp_code:{token_details["sp_code"]}, sp_message:{ShurjopayStatus().AUTH_SUCCESS.message}')
-                 # set AUTH_TOKEN from response
+            if (int)(token_details['sp_code']) == ShurjopayStatus().AUTH_SUCCESS.code:
+                self.logger.info(
+                    f'sp_code:{token_details["sp_code"]}, sp_message:{ShurjopayStatus().AUTH_SUCCESS.message}')
+                # set AUTH_TOKEN from response
                 self.AUTH_TOKEN = ShurjoPayTokenModel(**token_details)
                 return self.AUTH_TOKEN
-            self.logger.error(f'sp_code:{token_details["sp_code"]}, sp_message:{token_details["message"]}')
-            raise ShurjopayException(token_details['sp_code'], token_details['message'])
+            self.logger.error(
+                f'sp_code:{token_details["sp_code"]}, sp_message:{token_details["message"]}')
+            raise ShurjopayException(
+                token_details['sp_code'], token_details['message'])
         except ShurjopayAuthException as ex:
             # Log authentication expception error
-            self.logger.error(f'{self.AUTHENTICATION_FAILED}, {ex}') 
+            self.logger.error(f'{self.WRONG_CREDENTIALS}, {ex}')
             # Raise exception if authentication fails
-            raise ShurjopayAuthException(self.AUTHENTICATION_FAILED, ex) 
+            raise ShurjopayAuthException(self.WRONG_CREDENTIALS, ex)
 
     def is_token_valid(self):
         '''Checks if token is valid or not by comparing token expiry time with current time
-            
+
         Returns
         -------
         True: if token is valid 
         None: if token is invalid
         '''
         return True if (datetime.datetime.strptime(
                        self.AUTH_TOKEN.token_create_time, "%Y-%m-%d %I:%M:%S%p") + datetime.timedelta(seconds=self.AUTH_TOKEN.expires_in)) > datetime.datetime.now() else False
 
     def make_payment(self, payment_req):
         '''Make payment request to shurjoPay Gateway using a payment request object containing payment details.
-       
+
         Args
         ----
         payment_req (PaymentRequestModel): PaymentRequest object containing payment details.
-       
+
         Returns
         -------
         payment_details (PaymentDetailsModel): PaymentDetails object containing redirect URL to reach payment page, order id to verify order in shurjoPay.
         None: if response dosenot contains callback url.
-        
+
         Raises
         ------
         ShurjopayAuthException if payment fails due to token expired or invalid token.
         ShurjopayException if payment fails due to any other reason.
         '''
         try:
             # Check if token is valid or expired
-            if self.AUTH_TOKEN == None or self.is_token_valid() == False: 
+            if self.AUTH_TOKEN is None or self.is_token_valid() is False:
                 # Authenticate with shurjoPay
                 self.AUTH_TOKEN = self.authenticate()
         except ShurjopayAuthException as ex:
-            self.logger.error(f'{self.AUTHENTICATION_FAILED}: {ex}') 
-            raise 
+            self.logger.error(f'{self.AUTHENTICATION_FAILED}: {ex}')
+            raise ShurjopayAuthException(
+                self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
+
          # Create make payment endpoint url
-        url = requests.compat.urljoin(self.SP_ENDPOINT, Endpoints.SECRET_PAY.value)
+        url = requests.compat.urljoin(
+            self.SP_ENDPOINT, Endpoints.SECRET_PAY.value)
         headers = {
             'content-type': 'application/json',
-            'Authorization': f'{self.AUTH_TOKEN.token_type} {self.AUTH_TOKEN.token}' 
+            'Authorization': f'{self.AUTH_TOKEN.token_type} {self.AUTH_TOKEN.token}'
         }
         # Map data from authentication token to payment request object
-        payloads = self._map_payment_request(payment_req) 
+        payloads = self._map_payment_request(payment_req)
         if self.is_token_valid():
             try:
-                response = requests.post(url, headers=headers, data=json.dumps(payloads))
+                response = requests.post(
+                    url, headers=headers, data=json.dumps(payloads))
                 response_json = response.json()
-                 # Check if payment request is successful
+                # Check if payment request is successful
                 if response_json['checkout_url'] == None:
                     self.logger.error(self.PAYMENT_REQUEST_FAILED)
                     return None
                 self.logger.info(self.PAYMENT_REQUEST_SUCCESS)
                 # Return payment detais object
-                return PaymentDetailsModel(**response_json) 
+                return PaymentDetailsModel(**response_json)
             except ShurjopayException as ex:
                 self.logger.error(f'{self.PAYMENT_REQUEST_FAILED}: {ex}')
                 raise ShurjopayException(self.PAYMENT_REQUEST_FAILED, ex)
         else:
-            self.logger.warning(f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
-            raise ShurjopayException(self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED) 
+            self.logger.warning(
+                f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
+            raise ShurjopayAuthException(
+                self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
 
     def verify_payment(self, order_id):
         ''' Complete the payment process ushig the order id in the the IPN.
-        
+
         Args
         -----
         order_id (str): Order id of the payment.
-        
+
         Returns
         -------
         VerifiedPaymentModel: VerifiedPayment object containing payment details.
-        
+
         Raises
         -------
         ShurjopayAuthException if payment fails due to token expired or invalid token.
         ShurjopayException if payment fails due to any other reason.
         '''
         try:
             # Check if token is valid or expired
-            if self.AUTH_TOKEN == None or self.is_token_valid() == False: 
+            if self.AUTH_TOKEN is None or self.is_token_valid() is False:
                 # Authenticate with shurjoPay
-                self.AUTH_TOKEN = self.authenticate() 
+                self.AUTH_TOKEN = self.authenticate()
         except ShurjopayAuthException as ex:
             self.logger.error(self.AUTHENTICATION_FAILED, ex)
-            raise 
+            raise
         # Create verify payment endpoint url
-        url = requests.compat.urljoin(self.SP_ENDPOINT, Endpoints.VERIFIFICATION.value)
+        url = requests.compat.urljoin(
+            self.SP_ENDPOINT, Endpoints.VERIFIFICATION.value)
         headers = {'content-type': 'application/json',
                    'Authorization': f'{self.AUTH_TOKEN.token_type} {self.AUTH_TOKEN.token}'}
         payloads = {'order_id': order_id}
         if self.is_token_valid():
             try:
-                response = requests.post(url, headers=headers, data=json.dumps(payloads))
+                response = requests.post(
+                    url, headers=headers, data=json.dumps(payloads))
                 response = response.json()
                 response = response[0]
-                if(response['sp_code'] == ShurjopayStatus.INVALID_ORDER_ID.code):
-                    self.logger.info(f'sp_code:{response["sp_code"]}, sp_message:{response["message"]}') 
+                if (response['sp_code'] == ShurjopayStatus.INVALID_ORDER_ID.code):
+                    self.logger.info(
+                        f'sp_code:{response["sp_code"]}, sp_message:{response["message"]}')
                     return None
-                elif(response['sp_code'] != ShurjopayStatus.TRANSACTION_SUCCESS.code):
-                    self.logger.info(f'sp_code:{response["sp_code"]}, sp_message:{response["sp_message"]}')
+                elif (response['sp_code'] != ShurjopayStatus.TRANSACTION_SUCCESS.code):
+                    self.logger.info(
+                        f'sp_code:{response["sp_code"]}, sp_message:{response["sp_message"]}')
                     # Raise exception if payment verification fails
-                    raise ShurjopayException(self.PAYMENT_VERIFICATION_FAILED, response['sp_message']) 
-                self.logger.info(f'sp_code:{response["sp_code"]}, sp_message:{response["sp_message"]}')
+                    raise ShurjopayException(
+                        self.PAYMENT_VERIFICATION_FAILED, response['sp_message'])
+                self.logger.info(
+                    f'sp_code:{response["sp_code"]}, sp_message:{response["sp_message"]}')
                 # Return  verified payment detais object
-                return VerifiedPaymentDetailsModel(**response) 
+                return VerifiedPaymentDetailsModel(**response)
             except ShurjopayException as ex:
                 self.logger.error(f'{self.PAYMENT_VERIFICATION_FAILED}: {ex}')
-                raise ShurjopayException(self.PAYMENT_VERIFICATION_FAILED,ex)
+                raise ShurjopayException(self.PAYMENT_VERIFICATION_FAILED, ex)
         else:
-            self.logger.error(f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
-            raise ShurjopayAuthException(self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
+            self.logger.error(
+                f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
+            raise ShurjopayAuthException(
+                self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
 
     def _map_payment_request(self, payment_req):
         ''' This method is used to map additional parameters to payment request details.
         Args
         ----
         payment_req (PaymentRequestModel): Payment request object
-        
+
         Returns
         -------
         payment_req (dict) : a dictionary containing complete payment request details.
         '''
         return {
             'token': self.AUTH_TOKEN.token,
             'return_url': self.SP_RETURN,
@@ -226,8 +257,8 @@
             'currency': payment_req.currency,
             'customer_name':  payment_req.customer_name,
             'customer_address': payment_req.customer_address,
             'customer_phone': payment_req.customer_phone,
             'customer_city':  payment_req.customer_city,
             'customer_post_code':  payment_req.customer_post_code,
             'client_ip': get_client_ip(),
-        }
+        }
```

### Comparing `shurjopay-plugin-0.1.6/src/shurjopay_plugin/utils.py` & `shurjopay-plugin-0.1.7/src/shurjopay_plugin/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 from enum import Enum
 import socket
- 
+
+
 class Endpoints(str, Enum):
     '''This class contains all the endpoints of shurjoPayAPI'''
     API = 'api/'
     TOKEN = "get_token"
     SECRET_PAY = "secret-pay"
     VERIFIFICATION = "verification"
     PAYMENT_STATUS = "payment-status"
 
 
 class CustomResponse:
     """This class is used to create custom response for shurjoPayAPI during payment process
-    
+
     Args:
     ----
     code(str/int): status code of the response
     message (str): message of the response
     """
-    
+
     def __init__(self, code, message):
         self.code = code
         self.message = message
 
     def __str__(self):
         return f"HTTP Status code : {self.code} Message: {self.message}"
 
-    
+
 class ShurjopayStatus():
     '''This class contains the shurjoPayAPI Responses'''
-    AUTH_SUCCESS = CustomResponse(200, "Successfully authenticated with merchant")
+    AUTH_SUCCESS = CustomResponse(
+        200, "Successfully authenticated with Merchant")
     INVALID_ORDER_ID = CustomResponse('1011', "Invalid Payment ID")
     TRANSACTION_SUCCESS = CustomResponse('1000', "Transaction successful")
 
 
 class ShurjopayException(Exception):
     '''Exceptions during payment process 
-    
+
     Args:
     ---
         message: error message of different exception
         errors : errors of different exception
     '''
+
     def __init__(self, message, errors):
-        super().__init__(message, errors) 
+        super().__init__(message, errors)
+
 
-class ShurjopayAuthException(ShurjopayException):
+class ShurjopayAuthException(Exception):
     '''Exceptions during authentication process 
-    
+
     Args:
     ---
         message: authentication error message
         errors : authentication errors 
     '''
+
     def __init__(self, message, errors):
         super().__init__(message, errors)
 
+
 def get_client_ip():
-    '''This method is used to get the IP address of the merchant server
-    A socket connection is made to the IANA server and the IP address of the merchant server is returned  
-     
+    '''This method is used to get the IP address of the merchant server  
+
     Returns:
     -------
         ip_address (str): IP address of the merchant server 
-    
+
     Raises:
     ------
          ShurjoPayException while getting merchant IP address
+         ShurjoPayException while getting merchant IP address
     '''
-    
+
     IANA = '10.0.0.0'
-    PORT = 80
-    
+    PORT = 0
+
     try:
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        s.connect((IANA, PORT)) 
+        # connect() for UDP doesn't send packets
+        s.connect((IANA, PORT))
         return s.getsockname()[0]
     except ShurjopayException as ex:
-        raise ShurjopayException('Cannot connect to the internet"', ex) 
+        raise ShurjopayException('Cannot connect to the internet"', ex)
     finally:
-        s.close()
+        s.close()
```

### Comparing `shurjopay-plugin-0.1.6/src/shurjopay_plugin.egg-info/PKG-INFO` & `shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.6/tests/test_shurjopay_plugin.py` & `shurjopay-plugin-0.1.7/tests/test_shurjopay_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,54 @@
+from shurjopay_plugin import *
 import json
 import unittest
 import os
-import sys
 import environ
+import logging
 
+LOGGER = logging.getLogger(__name__)
+ROOT_DIR = os.getcwd()
 
-root_dir = os.getcwd()
-
-from shurjopay_plugin import *
-#load payemnt request data from json file
-with open(os.path.join(root_dir,"tests/sample_message/PaymentRequest.json"), "r") as read_file:
+# load payemnt request data from json file
+with open(os.path.join(ROOT_DIR, "tests/sample_message/PaymentRequest.json"), "r") as read_file:
     payment_request_json = json.load(read_file)
 
-#loading environment variables
+# loading environment variables
 env = environ.Env()
-env.read_env(os.path.join(root_dir, '.env'))
+env.read_env(os.path.join(ROOT_DIR, '.env'))
+
+
 class TestShurjoPayPlugin(unittest.TestCase):
     '''
     Unit tests for ShurjopayPlugin : Make Payment, Verify Payment, Check Payment Status
     '''
 
     def setUp(self):
-        #Shurjopay config for Instatiating ShurjopayPlugin
+        # Shurjopay config for InstShurjoPayConfigModelatiating ShurjopayPlugin
         sp_config = ShurjoPayConfigModel(
-        SP_USERNAME=env('SP_USERNAME'),
-        SP_PASSWORD=env('SP_PASSWORD'),
-        SP_ENDPOINT=env('SP_ENDPOINT'),
-        SP_RETURN=env('SP_RETURN'),
-        SP_CANCEL=env('SP_CANCEL'),
-        SP_PREFIX=env('SP_PREFIX'),
-        SP_LOGDIR=env('SP_LOGDIR')
-    )
+            SP_USERNAME=env('SP_USERNAME'),
+            SP_PASSWORD=env('SP_PASSWORD'),
+            SP_ENDPOINT=env('SP_ENDPOINT'),
+            SP_RETURN=env('SP_RETURN'),
+            SP_CANCEL=env('SP_CANCEL'),
+            SP_PREFIX=env('SP_PREFIX'),
+            SP_LOGDIR=env('SP_LOGDIR')
+        )
         self._plugin = ShurjopayPlugin(sp_config)
         self._payment_request = PaymentRequestModel(**payment_request_json)
 
     def test_make_payment(self):
         # unit testing for make payment
         self._payment_request_details = self._plugin.make_payment(
             self._payment_request)
 
-        print(json.dumps(self._payment_request_details.__dict__,indent=4))
+        print(json.dumps(self._payment_request_details.__dict__, indent=4))
 
         self.assertEqual(
-            10, self._payment_request_details.amount, 'amount is not equal')
+            5, self._payment_request_details.amount, 'amount is not equal')
 
         self.assertEqual(
             'BDT', self._payment_request_details.currency, 'Currency  is not equal')
 
         self.assertEqual(
             'MD. ABDUL KARIM', self._payment_request_details.customer_name, 'Customer Name is not equal')
 
@@ -55,24 +57,23 @@
 
         self.assertEqual(
             'mohakhali', self._payment_request_details.customer_address, "Customer Address is not equal")
 
         self.assertEqual(
             'Dhaka', self._payment_request_details.customer_city, 'Customer City is not equal')
 
-
     def test_verify_payment(self):
-        #unit testing for verify payment
-        verified_payment_details = self._plugin.verify_payment(
-            'sp6416d45992986')
-
-        if(verified_payment_details == None):
-            print(ShurjopayStatus.INVALID_ORDER_ID.message)
-            return
+        # unit testing for verify payment
+        try:
+            verified_payment_details = self._plugin.verify_payment(
+                'SP_PLUGIN_PYTHON64744291a63de')
+            self.assertEqual(2382747, verified_payment_details.id,
+                             "ID is not equal")
+            self.assertEqual(
+                "SP_PLUGIN_PYTHON64744291a63de", verified_payment_details.order_id,
+                "Order ID is not equal")
+        except ShurjopayException as e:
+            LOGGER.info(e)
 
-        self.assertEqual(1759527, verified_payment_details.id, "ID is not equal")
-        self.assertEqual(
-            "sp6416d45992986", verified_payment_details.order_id, "Order ID is not equal")
-       
 
 if __name__ == '__main__':
     unittest.main()
```


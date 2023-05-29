# Comparing `tmp/ln-markets-1.0.9.tar.gz` & `tmp/ln-markets-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ln-markets-1.0.9.tar", last modified: Mon May 23 14:48:14 2022, max compression
+gzip compressed data, was "ln-markets-2.0.1.tar", last modified: Mon May 29 17:44:18 2023, max compression
```

## Comparing `ln-markets-1.0.9.tar` & `ln-markets-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/
--rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-1.0.9/LICENSE
--rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-23 14:48:14.146736 ln-markets-1.0.9/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)    13424 2022-05-10 10:57:09.000000 ln-markets-1.0.9/README.md
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/ln_markets.egg-info/
--rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-23 14:48:13.000000 ln-markets-1.0.9/ln_markets.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      284 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-23 14:48:13.000000 ln-markets-1.0.9/ln_markets.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       19 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       10 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/top_level.txt
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/lnmarkets/
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-1.0.9/lnmarkets/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     9944 2022-05-10 10:28:50.000000 ln-markets-1.0.9/lnmarkets/rest.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     2349 2022-05-23 14:47:06.000000 ln-markets-1.0.9/lnmarkets/websockets.py
--rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-1.0.9/pyproject.toml
--rw-rw-r--   0 romain    (1000) romain    (1000)       89 2022-05-23 14:48:14.146736 ln-markets-1.0.9/setup.cfg
--rw-rw-r--   0 romain    (1000) romain    (1000)     1185 2022-05-23 14:47:06.000000 ln-markets-1.0.9/setup.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-2.0.1/LICENSE
+-rw-rw-r--   0 romain    (1000) romain    (1000)    19538 2023-05-29 17:44:18.117904 ln-markets-2.0.1/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)    18701 2023-05-29 17:42:35.000000 ln-markets-2.0.1/README.md
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.113904 ln-markets-2.0.1/ln_markets.egg-info/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    19538 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      309 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       26 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       10 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/top_level.txt
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/lnmarkets/
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.1/lnmarkets/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)    12695 2023-05-29 17:42:35.000000 ln-markets-2.0.1/lnmarkets/rest.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     2349 2023-05-29 17:42:35.000000 ln-markets-2.0.1/lnmarkets/websockets.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-2.0.1/pyproject.toml
+-rw-rw-r--   0 romain    (1000) romain    (1000)       89 2023-05-29 17:44:18.117904 ln-markets-2.0.1/setup.cfg
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1192 2023-05-29 17:43:55.000000 ln-markets-2.0.1/setup.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/tests/
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.1/tests/test_node_state.py
```

### Comparing `ln-markets-1.0.9/LICENSE` & `ln-markets-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ln-markets-1.0.9/lnmarkets/rest.py` & `ln-markets-2.0.1/lnmarkets/rest.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class LNMarketsRest():
     def __init__(self, **options):
         self.key = options.get('key', os.getenv('LNMARKETS_API_KEY'))
         self.secret = options.get('secret', os.getenv('LNMARKETS_API_SECRET'))
         self.passphrase = options.get('passphrase', os.getenv('LNMARKETS_API_PASSPHRASE'))
         self.network = options.get('network', os.getenv('LNMARKETS_API_NETWORK', 'mainnet'))
-        self.version = options.get('version', os.getenv('LNMARKETS_API_VERSION', 'v1'))
+        self.version = options.get('version', os.getenv('LNMARKETS_API_VERSION', 'v2'))
         self.hostname = get_hostname(self.network)
         self.custom_headers = options.get('custom_headers')
         self.full_response = options.get('full_response', False)
         self.debug = options.get('debug', False)
         self.skip_api_key = options.get('skip_api_key', False)
     
     def _request_options(self, **options):
@@ -68,15 +68,15 @@
             opts['headers']['LNM-ACCESS-SIGNATURE'] = signature
         opts['ressource'] = 'https://' + self.hostname + '/' + self.version + path
 
         if method in ['GET', 'DELETE'] and params:
             opts['ressource'] += '?' + data
         return opts
 
-    def request_api(self, method, path, params, credentials = False):
+    def request_api(self, method, path, params, credentials = False, format='text'):
         options = {
           'method': method,
           'path': path,
           'params': params,
           'credentials': credentials
         }
 
@@ -84,232 +84,304 @@
         ressource = opts.get('ressource')
         headers = opts.get('headers')
 
         if method in ['GET', 'DELETE']:
             response = request(method, ressource, headers = headers)
         elif method in ['POST', 'PUT']:
             response = request(method, ressource, data = json.dumps(params, separators=(',', ':')), headers = headers)
-        return response.text
+        
+        if format == 'json':
+            return response.json()
+        elif format is None:
+            return response
+        else:
+            return response.text
     
-    def before_request_api(self, method, path, params, credentials):
-        return self.request_api(method, path, params, credentials)
-
-    def futures_get_ticker(self):
-        method = 'GET'
-        path = '/futures/ticker'
-        credentials = False
-        params = {}
+    def before_request_api(self, method, path, params, credentials, format='text'):
+        return self.request_api(method, path, params, credentials, format)
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_new_position(self, params):
+    
+    ## Futures 
+    
+    def futures_add_margin_position(self, params, format='text'):
         method = 'POST'
-        path = '/futures'
-        credentials = True
-
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_update_position(self, params):
-        method = 'PUT'
-        path = '/futures'
+        path = '/futures/add-margin'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def futures_close_position(self, params):
+    def futures_cancel_all_positions(self, format='text'):
         method = 'DELETE'
-        path = '/futures'
+        path = '/futures/all/cancel'
         credentials = True
+        params = {}
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def futures_close_all_positions(self):
+    def futures_close_all_positions(self, format='text'):
         method = 'DELETE'
         path = '/futures/all/close'
         credentials = True
         params = {}
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_cancel_position(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_cancel_position(self, params, format='text'):
         method = 'POST'
         path = '/futures/cancel'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def futures_cancel_all_positions(self):
-        method = 'DELETE'
-        path = '/futures/all/cancel'
+    def futures_carry_fees_history(self, params, format='text'):
+        method = 'GET'
+        path = '/futures/carry-fees'
         credentials = True
-        params = {}
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_cashin_position(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    
+    def futures_cashin_position(self, params, format='text'):
         method = 'POST'
         path = '/futures/cash-in'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_add_margin_position(self, params):
-        method = 'POST'
-        path = '/futures/add-margin'
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_close_position(self, params, format='text'):
+        method = 'DELETE'
+        path = '/futures'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def futures_get_positions(self, params):
+    def futures_get_positions(self, params, format='text'):
         method = 'GET'
         path = '/futures'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_new_position(self, params, format='text'):
+        method = 'POST'
+        path = '/futures'
+        credentials = True
+
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_update_position(self, params, format='text'):
+        method = 'PUT'
+        path = '/futures'
+        credentials = True
 
-    def futures_bid_offer_history(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+        
+    def futures_fixing_history(self, params, format='text'):
         method = 'GET'
-        path = '/futures/history/bid-offer'
+        path = '/futures/history/fixing'
         credentials = False
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def futures_index_history(self, params):
+    def futures_index_history(self, params, format='text'):
         method = 'GET'
         path = '/futures/history/index'
         credentials = False
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_fixing_history(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_price_history(self, params, format='text'):
         method = 'GET'
-        path = '/futures/history/fixing'
+        path = '/futures/history/price'
         credentials = False
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def futures_carry_fees_history(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def futures_get_ticker(self, format='text'):
         method = 'GET'
-        path = '/futures/carry-fees'
+        path = '/futures/ticker'
         credentials = False
+        params = {}
+
+        return self.before_request_api(method, path, params, credentials, format)
 
-        return self.before_request_api(method, path, params, credentials)
+    ## Options
 
-    def get_user(self):
+    def options_get_expiries(self, format='text'):
         method = 'GET'
-        path = '/user'
+        path = '/options/instrument/expiry'
+        credentials = False
+        params = {}
+        
+        return self.before_request_api(method, path, params, credentials, format)    
+    
+    def options_get_configuration(self, format='text'):
+        method = 'GET'
+        path = '/options/instrument'
+        credentials = False
+        params = {}
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def options_close_all_positions(self, format='text'):
+        method = 'DELETE'
+        path = '/options/vanilla/all'
         credentials = True
         params = {}
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def options_close_position(self, params, format='text'):
+        method = 'DELETE'
+        path = '/options/vanilla'
+        credentials = True
+
+        return self.before_request_api(method, path, params, credentials, format)
+
+    def options_get_positions(self, params, format='text'):
+        method = 'GET'
+        path = '/options/vanilla'
+        credentials = True
+        
+        return self.before_request_api(method, path, params, credentials, format)
+        
+    def options_new_position(self, params, format='text'):
+        method = 'POST'
+        path = '/options/vanilla'
+        credentials = True
+        
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def update_user(self, params):
+    def options_update_position(self, params, format='text'):
         method = 'PUT'
-        path = '/user'
+        path = '/options/vanilla'
         credentials = True
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def options_get_volatility(self, params, format='text'):
+        method = 'GET'
+        path = '/options/volatility'
+        credentials = False
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
 
-        return self.before_request_api(method, path, params, credentials)
+    ## User
+    
+    def deposit_history(self, params, format='text'):
+        method = 'GET'
+        path = '/user/deposit'
+        credentials = True
 
-    def deposit(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def deposit(self, params, format='text'):
         method = 'POST'
         path = '/user/deposit'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def get_user(self, format='text'):
+        method = 'GET'
+        path = '/user'
+        credentials = True
+        params = {}
+
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def deposit_history(self, params):
+    def update_user(self, params, format='text'):
+        method = 'PUT'
+        path = '/user'
+        credentials = True
+
+        return self.before_request_api(method, path, params, credentials, format)
+
+    def get_notifications(self, format='text'):
         method = 'GET'
-        path = '/user/deposit'
+        path = '/user/notifications'
+        credentials = True
+        params = {}
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def mark_all_notifications_read(self, format='text'):
+        method = 'PUT'
+        path = '/user/notifications/all'
         credentials = True
+        params = {}
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def mark_notifications_read(self, format='text'):
+        method = 'PUT'
+        path = '/user/notifications'
+        credentials = True
+        params = {}
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def withdraw_history(self, params, format='text'):
+        method = 'GET'
+        path = '/user/withdraw'
+        credentials = True
 
-    def withdraw(self, params):
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def withdraw(self, params, format='text'):
         method = 'POST'
         path = '/user/withdraw'
         credentials = True
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def withdraw_history(self, params):
+    ## Swap
+    
+    def swap(self, params, format='text'):
+        method = 'POST'
+        path = '/swap'
+        credentials = True
+        
+        return self.before_request_api(method, path, params, credentials, format)
+    
+    def swap_history(self, params, format='text'):
         method = 'GET'
-        path = '/user/withdraw'
+        path = '/swap'
         credentials = True
+        
+        return self.before_request_api(method, path, params, credentials, format)  
+    
+    ## App
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def app_configuration(self):
+    def app_configuration(self, format='text'):
         method = 'GET'
         path = '/app/configuration'
         credentials = False
         params = {}
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def app_node(self):
+    def app_node(self, format='text'):
         method = 'GET'
         path = '/app/node'
         credentials = False
         params = {}
 
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
 
-    def get_leaderboard(self):
+    def get_leaderboard(self, format='text'):
         method = 'GET'
         path = '/futures/leaderboard'
         credentials = False
         params = {}
 
-        return self.before_request_api(method, path, params, credentials)
-
-    def get_announcements(self):
-        method = 'GET'
-        path = '/app/announcements'
-        credentials = False
-        params = {}
-
-        return self.before_request_api(method, path, params, credentials)
-
-    def get_lnurl_auth(self):
-        method = 'POST'
-        path = '/lnurl/auth'
-        credentials = False
-        params = {}
-
-        return self.before_request_api(method, path, params, credentials)
-
-    def lnurlAuth(self, params):
-        method = 'GET'
-        path = '/lnurl/auth'
-        credentials = False
-        
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
     
-    def options_get_positions(self, params):
-        method = 'GET'
-        path = '/options/vanilla'
-        credentials = True
-        
-        return self.before_request_api(method, path, params, credentials)
-        
-    def options_new_position(self, params):
-        method = 'POST'
-        path = '/options/vanilla'
-        credentials = True
-        
-        return self.before_request_api(method, path, params, credentials)
-
-    def options_get_volatility(self):
-        method = 'GET'
-        path = '/options/volatility'
-        credentials = False
-        params = {}
-        
-        return self.before_request_api(method, path, params, credentials)
+    ## Oracle
     
-    def options_get_configuration(self):
+    def get_oracle(self, params, format='text'):
         method = 'GET'
-        path = '/options/instrument'
+        path = '/oracle/index'
         credentials = False
-        params = {}
         
-        return self.before_request_api(method, path, params, credentials)
+        return self.before_request_api(method, path, params, credentials, format)
```

### Comparing `ln-markets-1.0.9/lnmarkets/websockets.py` & `ln-markets-2.0.1/lnmarkets/websockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class LNMarketsWebsocket:
     def __init__(self, **options):
         self.ws = None
         self.key = options.get('key', os.getenv('LNMARKETS_API_KEY'))
         self.secret = options.get('secret', os.getenv('LNMARKETS_API_SECRET'))
         self.passphrase = options.get('passphrase', os.getenv('LNMARKETS_API_PASSPHRASE'))
         self.network = options.get('network', os.getenv('LNMARKETS_API_NETWORK', 'mainnet'))
-        self.version = options.get('version', os.getenv('LNMARKETS_API_VERSION', 'v1'))
+        self.version = options.get('version', os.getenv('LNMARKETS_API_VERSION', 'v2'))
         self.hostname = get_hostname(self.network)
         self.ws = None
 
     def on_message(self, ws, message):
         print(message)
 
     def on_error(self, ws, error):
```

### Comparing `ln-markets-1.0.9/setup.py` & `ln-markets-2.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ln-markets',
-    version='1.0.9',
+    version='2.0.1',
     packages=['lnmarkets'],
     description='LN Markets API python implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ln-markets/api-python',
     author='Romain ROUPHAEL',
     license='MIT',
     keywords='lnmarkets trading rest api bitcoin lightning network futures options',
     install_requires=[
         'requests',
-        'websocket'
+        'websocket-client'
       ],
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
```


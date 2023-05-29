# Comparing `tmp/dgl_client-0.2.tar.gz` & `tmp/dgl_client-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.2.tar` & `dgl_client-0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       36 2023-05-24 07:54:55.455568 dgl_client-0.2/.gitignore
--rw-r--r--   0        0        0       69 2023-05-24 07:54:55.456197 dgl_client-0.2/README.md
--rw-r--r--   0        0        0       62 2023-05-26 14:27:51.075075 dgl_client-0.2/dgl_client/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-26 14:29:12.176627 dgl_client-0.2/dgl_client/api_cli.py
--rw-r--r--   0        0        0     3733 2023-05-24 08:36:13.792363 dgl_client-0.2/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-24 07:54:55.458038 dgl_client-0.2/dgl_client/utils.py
--rw-r--r--   0        0        0      438 2023-05-24 08:17:05.106570 dgl_client-0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 07:54:55.460270 dgl_client-0.2/tests/__init__.py
--rw-r--r--   0        0        0     1602 2023-05-26 14:26:13.928381 dgl_client-0.2/tests/test_decode.py
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 dgl_client-0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-05-26 06:08:29.040320 dgl_client-0.3/.gitignore
+-rw-r--r--   0        0        0       69 2023-05-26 06:08:29.040320 dgl_client-0.3/README.md
+-rw-r--r--   0        0        0       62 2023-05-29 11:33:58.648532 dgl_client-0.3/dgl_client/__init__.py
+-rw-r--r--   0        0        0     6036 2023-05-29 11:24:12.508534 dgl_client-0.3/dgl_client/api_cli.py
+-rw-r--r--   0        0        0     3928 2023-05-29 11:12:10.896537 dgl_client-0.3/dgl_client/main.py
+-rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3/dgl_client/utils.py
+-rw-r--r--   0        0        0      438 2023-05-26 06:08:29.040320 dgl_client-0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3/tests/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-29 11:23:50.236534 dgl_client-0.3/tests/create_token.py
+-rw-r--r--   0        0        0     2074 2023-05-29 08:36:18.388573 dgl_client-0.3/tests/test_decode.py
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 dgl_client-0.3/PKG-INFO
```

### Comparing `dgl_client-0.2/dgl_client/api_cli.py` & `dgl_client-0.3/dgl_client/api_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 import json
 import requests
 import sseclient
 import uuid
 
 logger = logging.getLogger(__name__)
 
+import json
+from base64 import b64decode, b64encode
+
+def prepare_token(api_key: str, user_id: str , provider_account_id: str, username: str, client="website"):
+    token_data = {
+        "api_key": api_key,
+        "client": client,
+        "user_id": user_id,
+        "provider_account_id": provider_account_id,
+        "username": username
+    }
+
+    token = b64encode(json.dumps(token_data).encode())
+    return token
+
+
 def login_check(endp, tok):
     logger.info("Trying to login...")
     username = None
     try:
       response = requests.get(
           f"{endp}/auth/check",
           json={},
@@ -39,33 +55,50 @@
       new_tok = response.json()
     except:
       raise
     logger.info("New token is %s"%str(new_tok))
 
     return new_tok
 
+def ak2token(endp, access_key):
+    logger.info("Logging in using access_key...")
+    new_tok = None
+    try:
+      response = requests.post(
+          f"{endp}/auth/trusted_login",
+          json={},
+          headers={
+              "TrustedClient": f"{access_key}"
+              },
+      )
+      response.raise_for_status()
+      new_tok = response.json()
+    except:
+      raise
+    logger.info("New token is %s"%str(new_tok))
+
+    return new_tok
+
+
 class APIClient:
     def __init__(self, backend_url, http_client=requests):
         self.backend_url = backend_url
         self.http_client = http_client
         self.auth_headers = None
         self.message_id = None
 
-    def login(self, tokens):
-        print(tokens)
-        atok = tokens["access_token"]["access_token"] + "e"
-        rtok = tokens["refresh_token"]["access_token"]
-        self.auth_headers = {"Authorization": f"Bearer {atok}"}
+    def login(self, access_key):
+        print(access_key)
+        atok = ak2token(self.backend_url, access_key)
+
         username = login_check(self.backend_url, atok)
-        if username is None:
-          atok = refresh_token(self.backend_url, atok, rtok)
-          if atok:
-            username = login_check(self.backend_url, atok)
 
-        logger.info(f"Logged in as {username}")
+        if username:
+            logger.info(f"Logged in as {username}")    
+            self.auth_headers = {"Authorization": f"Bearer {atok}"}
 
 
     def continue_chat(self, chat_id):
         self.chat_id = chat_id
         return self.chat_id
 
     def create_chat(self):
```

### Comparing `dgl_client-0.2/dgl_client/main.py` & `dgl_client-0.3/dgl_client/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import logging
 import os
 import sys
-from .api_cli import APIClient
+from .api_cli import APIClient, prepare_token
 import uuid
 from glob import glob
 import json
 
 logFormatter = logging.Formatter("%(asctime)s [%(levelname)-5.5s] - [%(filename)s > %(funcName)s() > %(lineno)s] %(message)s")
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
@@ -32,20 +32,21 @@
       list_models(args)
     case "model":
       list_models(args)      
     case _:
       logger.error("Resource not found!")
 
 def do_login(args, client):
-  if args.token_file:
-    if os.path.exists(args.token_file):
-      tokens = {}
-      with open(args.token_file,"r") as fp:
-        tokens = json.load(fp)
-      client.login(tokens)
+  if args.access_key:
+    client.login(args.access_key)
+    # if os.path.exists(args.token_file):
+    #   tokens = {}
+    #   with open(args.token_file,"r") as fp:
+    #     tokens = json.load(fp)
+    #   client.login(tokens)
 
   return True
 
 def main_chat(args):
   client = get_client(args)
 
   model_config_name = args.model
@@ -71,31 +72,33 @@
   for event in events:
       print(event, end="", flush=True)
       ass_reply.append(event)
   print()
   return ass_reply
 
 def main():
-  API_ENDPOINT = "https://www.diglife.eu/inference"
+  DGL_API_ENDPOINT = "https://www.diglife.eu/inference"
+  if "DGL_API_ENDPOINT" in os.environ and os.environ["DGL_API_ENDPOINT"]:
+    DGL_API_ENDPOINT = os.environ["DGL_API_ENDPOINT"]
 
   parser = argparse.ArgumentParser(description='DigLife API Client.')
   parser.add_argument('--logdir', type=str, default="logs/",
                       help='Where to store logs')
-  parser.add_argument('--endpoint', type=str, default=API_ENDPOINT,
+  parser.add_argument('--endpoint', type=str, default=DGL_API_ENDPOINT,
                       help='Endpoint for the inference')
 
   subparsers = parser.add_subparsers(help='You can choose between different commands')
   chat_p = subparsers.add_parser('chat', help='chat with the assistants')
   chat_p.set_defaults(func=main_chat)
 
   chat_p.add_argument('message', type=str, 
                       help='say something to the model')
   chat_p.add_argument('-c','--chat-id', type=str,
                       help='Continue previous chat')
-  chat_p.add_argument('-t','--token-file', type=str, required=True,
+  chat_p.add_argument('-k','--access_key', type=str, required=True,
                       help='Access keys to authenticate to the API')
   chat_p.add_argument('-m','--model', type=str, required=True,
                       help='Which model do you want to talk to?')
   chat_p.add_argument('-i','--interactive', action='store_true',
                       help='Run interactive chat')
   
   config_p = subparsers.add_parser('ls', help='List resources')
```

### Comparing `dgl_client-0.2/tests/test_decode.py` & `dgl_client-0.3/tests/test_decode.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 aTok  = tokens["access_token"]["access_token"]
 rTok  = tokens["refresh_token"]["access_token"]
 
 from jose import jwe, jws, jwt
 
 def decode_access_token(authorisation_token):
     TEST = "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0..jwv1zIaiPCcji0-lT4MF9A.PEM0NQ5LuicwWqDvzvAoIlpHq3d6R5dt_rOJbrLvXV12pI4cMy3ooCGiiROOTFRkdnj_cge9a29Wm5QatccgJ7U9ao_YBW6Az33Vn4o2RjiRPiAFJA.OzmRfSDdsmZXM0UkhafsfA"
-    print(authorisation_token)
-    print(TEST)
+    TEST2= "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0..yta4b2GIgWE62x-bEjkVBg.ymXYrMxrC4PxYUnZl5la5MfoseWcxQgID-vaD2OgbdeC7xRpxgOykirjbqfnlbCL30gsRNTudRjqcc7s3IPSc7XBRU9gNyxUTGqrKW82v5SjCjnU.g1CzngLUoI8aG32Fd3dfqQe"
+    TEST2= "eyJhbGciOiJkaXIiLCJlbmMiOiJBMjU2R0NNIn0..RQEWaFb_T06bCV7TPf874g.0YGh9jtMDGSMVo8obR8mfldoSboRhFQNLP3FqNlGZyn3_yW-8CdyqQbvsLp3xkjNH30ulOaDXVZCeZkULmKUJ9ojnGt4.kkTwu7Q7wWJ9Vb9y-mOd3A"
+    #print(authorisation_token)
+    #print(TEST)
+    print(TEST2)
     # get public key from jwks uri
 
     # gives the set of jwks keys.the keys has to be passed as it is to jwt.decode() for signature verification.
     key = b'y\xf8l\xf3\xf7n\xd5y\xcf]N\xd4P;\nuy\xa2\x96\xc6\xc6~@\x00\x96\rn\x1dq]\x12\xd6'
 
     # get the algorithm type from the request header
-    algorithm = jwt.get_unverified_header(authorisation_token).get('alg')
-    print(jwt.get_unverified_header(TEST))
+    #algorithm = jwt.get_unverified_header(authorisation_token).get('alg')
+    #print(jwt.get_unverified_header(TEST))
+    print(jwt.get_unverified_header(TEST2))
 
-
-    user_info = jwe.decrypt(TEST,
+    user_info = jwe.decrypt(TEST2,
                            key=key)
 
     return user_info
 
 
 print(decode_access_token(rTok))
```


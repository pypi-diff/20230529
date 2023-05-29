# Comparing `tmp/vector_vault-1.3.0.tar.gz` & `tmp/vector_vault-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.3.0.tar", last modified: Sun May 28 08:45:04 2023, max compression
+gzip compressed data, was "vector_vault-1.4.0.tar", last modified: Mon May 29 07:50:46 2023, max compression
```

## Comparing `vector_vault-1.3.0.tar` & `vector_vault-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.479519 vector_vault-1.3.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.3.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-28 08:45:04.479325 vector_vault-1.3.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19322 2023-05-27 22:01:20.000000 vector_vault-1.3.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-28 08:45:04.479568 vector_vault-1.3.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-28 08:43:08.000000 vector_vault-1.3.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.475514 vector_vault-1.3.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-28 08:45:04.000000 vector_vault-1.3.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-28 08:45:04.478783 vector_vault-1.3.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.3.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.3.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3222 2023-05-28 08:43:39.000000 vector_vault-1.3.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.3.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.3.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1742 2023-05-28 08:43:47.000000 vector_vault-1.3.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.3.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17379 2023-05-28 08:43:26.000000 vector_vault-1.3.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2381 2023-05-28 08:31:16.000000 vector_vault-1.3.0/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.3.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.572583 vector_vault-1.4.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.4.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-29 07:50:46.572407 vector_vault-1.4.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19322 2023-05-27 22:01:20.000000 vector_vault-1.4.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-29 07:50:46.572626 vector_vault-1.4.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-29 07:50:37.000000 vector_vault-1.4.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.569253 vector_vault-1.4.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.572043 vector_vault-1.4.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.4.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.4.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3214 2023-05-29 07:49:21.000000 vector_vault-1.4.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1848 2023-05-29 05:20:39.000000 vector_vault-1.4.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.4.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1742 2023-05-29 07:49:07.000000 vector_vault-1.4.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.4.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17961 2023-05-29 07:49:36.000000 vector_vault-1.4.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3376 2023-05-29 07:21:37.000000 vector_vault-1.4.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.4.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.3.0/LICENSE` & `vector_vault-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/PKG-INFO` & `vector_vault-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.3.0
+Version: 1.4.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.3.0/README.md` & `vector_vault-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/setup.py` & `vector_vault-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.3.0",
+    version="1.4.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.3.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.4.0/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.3.0
+Version: 1.4.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.3.0/vectorvault/__init__.py` & `vector_vault-1.4.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/vectorvault/ai.py` & `vector_vault-1.4.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/vectorvault/cloudmanager.py` & `vector_vault-1.4.0/vectorvault/cloudmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from .vecreq import call_proj
 from .itemize import cloud_name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
-        self.user = self.get_user_id(user)
+        self.user = user
         self.api = api_key
         self.vault = vault
         # Creates the credentials
         credentials = CustomCredentials(user, self.api)
         # Instantiates the client 
         self.storage_client = storage.Client(project=call_proj(), credentials=credentials)
-        self.cloud = self.storage_client.bucket(self.user)
+        self.cloud = self.storage_client.bucket(self.get_bkt(self.user))
         print(f'Connected to Vault: {self.vault}')
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.cloud, name=vault_name).exists(self.storage_client)
 
     def upload_to_cloud(self, vault_name, content):
         blob = self.cloud.blob(vault_name)
@@ -60,15 +60,15 @@
         with ThreadPoolExecutor() as executor:
             executor.submit(self.upload_to_cloud, cloud_name(self.vault, item, self.user, text, self.api, item=True), text)
             executor.submit(self.upload_to_cloud, cloud_name(self.vault, item, self.user, meta, self.api, meta=True), json.dumps(meta))
     
     def delete_blob(self, blob):
         blob.delete()
      
-    def get_user_id(self, input_string):
+    def get_bkt(self, input_string):
         return input_string.replace("@", "_at_").replace(".", "_dot_") + '_vvclient'
 
     def delete(self):
         # Get all objects
         blobs = self.cloud.list_blobs(prefix=self.vault)
         
         # Delete each object concurrently
```

### Comparing `vector_vault-1.3.0/vectorvault/creds.py` & `vector_vault-1.4.0/vectorvault/creds.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def refresh(self):
         if not self.valid:
             data = {
                 "user_id": self.user,
                 "api_key": self.api,
             }
-            response = requests.post('https://vv-creds-etrszydrna-uc.a.run.app/access', json=data)
+            response = requests.post('https://get-loc-etrszydrna-uc.a.run.app/access', json=data)
             response.raise_for_status()  
             response_data = response.json()
             self.token = response_data['access_token']
             self.expiry = datetime.datetime.fromisoformat(response_data['expiry'])
 
     def before_request(self, auth_request, method, url, request_headers):
         self.apply(request_headers)
```

### Comparing `vector_vault-1.3.0/vectorvault/download.py` & `vector_vault-1.4.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/vectorvault/itemize.py` & `vector_vault-1.4.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/vectorvault/signup.py` & `vector_vault-1.4.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.3.0/vectorvault/vault.py` & `vector_vault-1.4.0/vectorvault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 import time
 import re
 import openai
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .ai import AI
 from .itemize import itemize, name_vecs, get_item, get_vectors
-from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults
+from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
         self.dims = dims
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
-        except:
+        except Exception as e:
             print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work')
             # user can still use the get_chat() function without an api key
             pass
-        self.user = self.cloud_manager.user
+        self.user = user
         self.x = 0
         self.x_checked = False
         self.vecs_loaded = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
@@ -155,15 +155,18 @@
         if current_segment:
             segments.append(" ".join(current_segment))
 
         return segments
     
     def get_similar(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return call_items_by_vector(self.user, self.vault, vector, self.api, n)
+        return call_items_by_vector(self.user, self.vault, self.api, vector, n)
+    
+    def get_similar_cloud(self, text, n: int = 4):
+        return call_get_similar(self.user, self.vault, self.api, text, n)
 
     def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         if self.x_checked == False:
@@ -216,16 +219,16 @@
     def process_batch(self, batch_text_chunks, never_stop, loop_timeout):
         loop_start_time = time.time()
         while True:
             try:
                 res = openai.Embedding.create(input=batch_text_chunks, engine="text-embedding-ada-002")
                 break
             except Exception as e:
-                print(f"API Error: {e}. Sleeping 15 seconds")
-                time.sleep(15)
+                print(f"API Error: {e}. Sleeping 5 seconds")
+                time.sleep(5)
                 if not never_stop or (time.time() - loop_start_time) > loop_timeout:
                     try:
                         res = openai.Embedding.create(input=batch_text_chunks, engine="text-embedding-ada-002")
                         break
                     except Exception as e:
                         raise TimeoutError("Loop timed out")
         return [record['embedding'] for record in res['data']]
@@ -285,15 +288,17 @@
                 current_item_index += 1
 
         self.last_time = start_time
         self.first_run = False
         if self.verbose == True:
             print("get vectors time --- %s seconds ---" % (time.time() - start_time))
 
-
+    def get_chat_cloud(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
+        return call_get_chat(self.user, self.vault, self.api, text, history, summary, get_context, n_context, return_context, expansion, history_search, model, include_context_meta)
+    
     def get_chat(self, text: str, history: str = None, summary: bool = False, get_context = False, n_context = 4, return_context = False, expansion = False, history_search = False, model='gpt-3.5-turbo', include_context_meta=False):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
             Enter your text, add optional chat history, and optionally choose a summary response (default: summmary = False)
 
             Example Signle Usage:
```

### Comparing `vector_vault-1.3.0/vectorvault/wrap.py` & `vector_vault-1.4.0/vectorvault/wrap.py`

 * *Files identical despite different names*


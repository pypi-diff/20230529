# Comparing `tmp/vector_vault-1.4.0.tar.gz` & `tmp/vector_vault-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.4.0.tar", last modified: Mon May 29 07:50:46 2023, max compression
+gzip compressed data, was "vector_vault-1.5.0.tar", last modified: Mon May 29 20:32:34 2023, max compression
```

## Comparing `vector_vault-1.4.0.tar` & `vector_vault-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.572583 vector_vault-1.4.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.4.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-29 07:50:46.572407 vector_vault-1.4.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19322 2023-05-27 22:01:20.000000 vector_vault-1.4.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-29 07:50:46.572626 vector_vault-1.4.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-29 07:50:37.000000 vector_vault-1.4.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.569253 vector_vault-1.4.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20047 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-29 07:50:46.000000 vector_vault-1.4.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 07:50:46.572043 vector_vault-1.4.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.4.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.4.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3214 2023-05-29 07:49:21.000000 vector_vault-1.4.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1848 2023-05-29 05:20:39.000000 vector_vault-1.4.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.4.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1742 2023-05-29 07:49:07.000000 vector_vault-1.4.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.4.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17961 2023-05-29 07:49:36.000000 vector_vault-1.4.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3376 2023-05-29 07:21:37.000000 vector_vault-1.4.0/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.4.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 20:32:34.733271 vector_vault-1.5.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.5.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20799 2023-05-29 20:32:34.733114 vector_vault-1.5.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20074 2023-05-29 20:31:26.000000 vector_vault-1.5.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-29 20:32:34.733311 vector_vault-1.5.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-29 20:32:14.000000 vector_vault-1.5.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 20:32:34.730167 vector_vault-1.5.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20799 2023-05-29 20:32:34.000000 vector_vault-1.5.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-29 20:32:34.000000 vector_vault-1.5.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-29 20:32:34.000000 vector_vault-1.5.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-29 20:32:34.000000 vector_vault-1.5.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-29 20:32:34.000000 vector_vault-1.5.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-29 20:32:34.732738 vector_vault-1.5.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.5.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.5.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3214 2023-05-29 20:31:58.000000 vector_vault-1.5.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1848 2023-05-29 05:20:39.000000 vector_vault-1.5.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.5.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1742 2023-05-29 20:31:47.000000 vector_vault-1.5.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.5.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18197 2023-05-29 20:31:41.000000 vector_vault-1.5.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3376 2023-05-29 07:21:37.000000 vector_vault-1.5.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.5.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.4.0/LICENSE` & `vector_vault-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/PKG-INFO` & `vector_vault-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.4.0
+Version: 1.5.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -37,24 +37,26 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text 
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+<br>
+`get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Interact with your Vault:
+# Build Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -123,20 +125,32 @@
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
-# Reference Your Vault:
+# Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-After you've added some data and want to reference it later, you can call it like this:
+Making a call to your vault is really easy. You can even do it by command line:
+```
+curl -X POST "https://api.vectorvault.io/get_similar" \
+     -H "Content-Type: application/json" \
+     -d '{
+        "user": "your_username",
+        "api_key": "your_api_key",
+        "vault": "your_vault_name",
+        "text": "your_text"
+     }'
+```
+    
+This is the same exact call, but in Python:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
@@ -150,17 +164,108 @@
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
+<br>
+
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+```
+question = "This text will be used find contextually similar references in the vault"
+
+answer = vault.get_chat(question, get_context=True)  
+print(answer)
+```
+The following line will send chatgpt the question for response and not interact with the vault in any way
+```
+answer = vault.get_chat(question) 
+```
+
+
+<br>
+<br>
+
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
+<br>
+
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
+
+- Example Signle Usage: 
+`response = vault.get_chat(text)`
+
+- Example Chat: 
+`response = vault.get_chat(text, chat_history)`
+
+- Example Summary: 
+`summary = vault.get_chat(text, summary=True)`
+
+- Example Context-Based Response:
+`response = vault.get_chat(text, get_context=True)`
+
+- Example Context-Based Response w/ Chat History:
+`response = vault.get_chat(text, chat_history, get_context=True)`
+
+- Example Context-Response with Context Samples Returned:
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
+<br>
+
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+```
+# print response:
+print(vault_response['response'])
+
+# print context:
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
+    print(item['data'])
+```
+<br>
+<br>
+
+# Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
+You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
+```
+summary = vault.get_chat(text, summary=True)
+```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
+
+<br>
+<br>
+<br>
 
-## Metadata
-To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+# Metadata
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/9d9bae20-e358-4545-9e3b-32f782314541/add+all+the+metadata.png?" width="40%" height="40%" />
+</p>
+
+Metadata is really useful later, when you want to know the deets about the data you've added. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
@@ -237,31 +342,14 @@
 similar_data = vault.get_similar("How will the government control you in the future?") 
 print(similar_data[0]['metadata']['title'])
 ```
 
 <br>
 <br>
 
-### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
-question = "This text will be used find contextually similar references in the vault"
-
-answer = vault.get_chat(question, get_context=True)  
-print(answer)
-```
-The following line will send chatgpt the question for response and not interact with the vault in any way
-```
-answer = vault.get_chat(question) 
-```
-
-
-<br>
-<br>
-
 # Change Vaults
 
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
@@ -286,83 +374,15 @@
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
-<br>
-<br>
 
-# ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
-
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
-</p>
-<br>
-
-Get chat response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
-Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
-
-- Example Signle Usage: 
-`response = vault.get_chat(text)`
-
-- Example Chat: 
-`response = vault.get_chat(text, chat_history)`
-
-- Example Summary: 
-`summary = vault.get_chat(text, summary=True)`
-
-- Example Context-Based Response:
-`response = vault.get_chat(text, get_context=True)`
-
-- Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context=True)`
-
-- Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
-<br>
-
-Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
-```
-# print response:
-print(vault_response['response'])
-
-# print context:
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['name']}")
-    print(item['data'])
-```
-<br>
-<br>
-
-# Summarize Anything:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
-</p>
-
-You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
-summary = vault.get_chat(text, summary=True)
-```
-<br>
-
-want to make a summary of a certain length?...
-```
-summary = vault.get_chat(text, summary=True)
-
-while len(summary) > 1000:
-    summary = vault.get_chat(summary, summary=True)
-```
-^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
-
-<br>
-<br>
 <br>
 
 ## Real world usage:
 ```
 user_input = input("What's your question?")
 
 # Get response from Language model
@@ -481,15 +501,15 @@
 <br>
 <br>
 
 
 ## FAQ
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
 
 ### What if I'm a large company with very large data
```

### Comparing `vector_vault-1.4.0/README.md` & `vector_vault-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text 
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+<br>
+`get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Interact with your Vault:
+# Build Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -104,20 +106,32 @@
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
-# Reference Your Vault:
+# Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-After you've added some data and want to reference it later, you can call it like this:
+Making a call to your vault is really easy. You can even do it by command line:
+```
+curl -X POST "https://api.vectorvault.io/get_similar" \
+     -H "Content-Type: application/json" \
+     -d '{
+        "user": "your_username",
+        "api_key": "your_api_key",
+        "vault": "your_vault_name",
+        "text": "your_text"
+     }'
+```
+    
+This is the same exact call, but in Python:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
@@ -131,17 +145,108 @@
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
+<br>
+
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+```
+question = "This text will be used find contextually similar references in the vault"
+
+answer = vault.get_chat(question, get_context=True)  
+print(answer)
+```
+The following line will send chatgpt the question for response and not interact with the vault in any way
+```
+answer = vault.get_chat(question) 
+```
+
+
+<br>
+<br>
+
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
+<br>
+
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
+
+- Example Signle Usage: 
+`response = vault.get_chat(text)`
+
+- Example Chat: 
+`response = vault.get_chat(text, chat_history)`
+
+- Example Summary: 
+`summary = vault.get_chat(text, summary=True)`
+
+- Example Context-Based Response:
+`response = vault.get_chat(text, get_context=True)`
+
+- Example Context-Based Response w/ Chat History:
+`response = vault.get_chat(text, chat_history, get_context=True)`
+
+- Example Context-Response with Context Samples Returned:
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
+<br>
+
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+```
+# print response:
+print(vault_response['response'])
+
+# print context:
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
+    print(item['data'])
+```
+<br>
+<br>
+
+# Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
+You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
+```
+summary = vault.get_chat(text, summary=True)
+```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
+
+<br>
+<br>
+<br>
 
-## Metadata
-To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+# Metadata
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/9d9bae20-e358-4545-9e3b-32f782314541/add+all+the+metadata.png?" width="40%" height="40%" />
+</p>
+
+Metadata is really useful later, when you want to know the deets about the data you've added. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
@@ -218,31 +323,14 @@
 similar_data = vault.get_similar("How will the government control you in the future?") 
 print(similar_data[0]['metadata']['title'])
 ```
 
 <br>
 <br>
 
-### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
-question = "This text will be used find contextually similar references in the vault"
-
-answer = vault.get_chat(question, get_context=True)  
-print(answer)
-```
-The following line will send chatgpt the question for response and not interact with the vault in any way
-```
-answer = vault.get_chat(question) 
-```
-
-
-<br>
-<br>
-
 # Change Vaults
 
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
@@ -267,83 +355,15 @@
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
-<br>
-<br>
 
-# ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
-
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
-</p>
-<br>
-
-Get chat response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
-Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
-
-- Example Signle Usage: 
-`response = vault.get_chat(text)`
-
-- Example Chat: 
-`response = vault.get_chat(text, chat_history)`
-
-- Example Summary: 
-`summary = vault.get_chat(text, summary=True)`
-
-- Example Context-Based Response:
-`response = vault.get_chat(text, get_context=True)`
-
-- Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context=True)`
-
-- Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
-<br>
-
-Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
-```
-# print response:
-print(vault_response['response'])
-
-# print context:
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['name']}")
-    print(item['data'])
-```
-<br>
-<br>
-
-# Summarize Anything:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
-</p>
-
-You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
-summary = vault.get_chat(text, summary=True)
-```
-<br>
-
-want to make a summary of a certain length?...
-```
-summary = vault.get_chat(text, summary=True)
-
-while len(summary) > 1000:
-    summary = vault.get_chat(summary, summary=True)
-```
-^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
-
-<br>
-<br>
 <br>
 
 ## Real world usage:
 ```
 user_input = input("What's your question?")
 
 # Get response from Language model
@@ -462,15 +482,15 @@
 <br>
 <br>
 
 
 ## FAQ
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
 
 ### What if I'm a large company with very large data
```

### Comparing `vector_vault-1.4.0/setup.py` & `vector_vault-1.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.4.0",
+    version="1.5.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.4.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.5.0/vector_vault.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.4.0
+Version: 1.5.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -37,24 +37,26 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text 
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+<br>
+`get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
-# Interact with your Vault:
+# Build Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
@@ -123,20 +125,32 @@
 ^ these three lines execute fast and can be called as often as you like. For example: you can use `add()`, `get_vectors()`, and `save()` mid conversation to save every message to the vault as soon as they comes in. Small loads are usually finished in less than a second. Large loads depend on total data size. 
 >> A test was done adding the full text of 37 books at once. The `get_vectors()` function took 8 minutes and 56 seconds. (For comparison, processing one at a time via openai's embedding function would take roughly two days)
 
 
 <br>
 <br>
 
-# Reference Your Vault:
+# Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-After you've added some data and want to reference it later, you can call it like this:
+Making a call to your vault is really easy. You can even do it by command line:
+```
+curl -X POST "https://api.vectorvault.io/get_similar" \
+     -H "Content-Type: application/json" \
+     -d '{
+        "user": "your_username",
+        "api_key": "your_api_key",
+        "vault": "your_vault_name",
+        "text": "your_text"
+     }'
+```
+    
+This is the same exact call, but in Python:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['data'])
 ```
 ^ this prints each similar item that was retieved. The `get_similar()` function retrieves items from the vault using vector cosine similarity search algorithm to find results. Default returns a list with 4 results. 
@@ -150,17 +164,108 @@
 
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
+<br>
+
+### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+```
+question = "This text will be used find contextually similar references in the vault"
+
+answer = vault.get_chat(question, get_context=True)  
+print(answer)
+```
+The following line will send chatgpt the question for response and not interact with the vault in any way
+```
+answer = vault.get_chat(question) 
+```
+
+
+<br>
+<br>
+
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
+</p>
+<br>
+
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
+
+- Example Signle Usage: 
+`response = vault.get_chat(text)`
+
+- Example Chat: 
+`response = vault.get_chat(text, chat_history)`
+
+- Example Summary: 
+`summary = vault.get_chat(text, summary=True)`
+
+- Example Context-Based Response:
+`response = vault.get_chat(text, get_context=True)`
+
+- Example Context-Based Response w/ Chat History:
+`response = vault.get_chat(text, chat_history, get_context=True)`
+
+- Example Context-Response with Context Samples Returned:
+`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
+<br>
+
+Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
+```
+# print response:
+print(vault_response['response'])
+
+# print context:
+for item in vault_response['context']:
+    print("\n\n", f"item {item['metadata']['name']}")
+    print(item['data'])
+```
+<br>
+<br>
+
+# Summarize Anything:
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
+</p>
+
+You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
+```
+summary = vault.get_chat(text, summary=True)
+```
+<br>
+
+want to make a summary of a certain length?...
+```
+summary = vault.get_chat(text, summary=True)
+
+while len(summary) > 1000:
+    summary = vault.get_chat(summary, summary=True)
+```
+^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
+
+<br>
+<br>
+<br>
 
-## Metadata
-To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+# Metadata
+
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/9d9bae20-e358-4545-9e3b-32f782314541/add+all+the+metadata.png?" width="40%" height="40%" />
+</p>
+
+Metadata is really useful later, when you want to know the deets about the data you've added. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
@@ -237,31 +342,14 @@
 similar_data = vault.get_similar("How will the government control you in the future?") 
 print(similar_data[0]['metadata']['title'])
 ```
 
 <br>
 <br>
 
-### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
-```
-question = "This text will be used find contextually similar references in the vault"
-
-answer = vault.get_chat(question, get_context=True)  
-print(answer)
-```
-The following line will send chatgpt the question for response and not interact with the vault in any way
-```
-answer = vault.get_chat(question) 
-```
-
-
-<br>
-<br>
-
 # Change Vaults
 
 In this example science vault, we will print a list of vaults in the current vault directory
 ```
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
@@ -286,83 +374,15 @@
 
 
 - lab notes vault within chemistry vault
 ```
 lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
-<br>
-<br>
 
-# ChatGPT
-## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
-
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
-</p>
-<br>
-
-Get chat response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
-Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
-
-- Example Signle Usage: 
-`response = vault.get_chat(text)`
-
-- Example Chat: 
-`response = vault.get_chat(text, chat_history)`
-
-- Example Summary: 
-`summary = vault.get_chat(text, summary=True)`
-
-- Example Context-Based Response:
-`response = vault.get_chat(text, get_context=True)`
-
-- Example Context-Based Response w/ Chat History:
-`response = vault.get_chat(text, chat_history, get_context=True)`
-
-- Example Context-Response with Context Samples Returned:
-`vault_response = vault.get_chat(text, get_context=True, return_context=True)`
-<br>
-
-Response is a string, unless `return_context=True` is passed, then response will be a dictionary containing the results from the vault as well as the response:
-```
-# print response:
-print(vault_response['response'])
-
-# print context:
-for item in vault_response['context']:
-    print("\n\n", f"item {item['metadata']['name']}")
-    print(item['data'])
-```
-<br>
-<br>
-
-# Summarize Anything:
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/e1ff4ca3-e18b-4c8f-b3c9-ff6ddcc907a1/wisdomandwealth_a_summary_being_created._A_bunch_of_texts_are_f_df58744a-13cb-46fd-b39d-3f090349bbb7.png" width="60%" height="60%" />
-</p>
-
-You can summarize any text, no matter how large - even an entire book all at once. Long texts are split into the largest possible chunk sizes and a summary is generated for each chunk. When all summaries are finished, they are concatenated and returned as one.
-```
-summary = vault.get_chat(text, summary=True)
-```
-<br>
-
-want to make a summary of a certain length?...
-```
-summary = vault.get_chat(text, summary=True)
-
-while len(summary) > 1000:
-    summary = vault.get_chat(summary, summary=True)
-```
-^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
-
-<br>
-<br>
 <br>
 
 ## Real world usage:
 ```
 user_input = input("What's your question?")
 
 # Get response from Language model
@@ -481,15 +501,15 @@
 <br>
 <br>
 
 
 ## FAQ
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is under one second response time with the similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking longer than 1 second, its recommended that you segment you data into multiple vaults to keep latency below 1 second on api calls. 
+To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
 
 ### What if I'm a large company with very large data
```

### Comparing `vector_vault-1.4.0/vectorvault/__init__.py` & `vector_vault-1.5.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/ai.py` & `vector_vault-1.5.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/cloudmanager.py` & `vector_vault-1.5.0/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/creds.py` & `vector_vault-1.5.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/download.py` & `vector_vault-1.5.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/itemize.py` & `vector_vault-1.5.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/signup.py` & `vector_vault-1.5.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/vault.py` & `vector_vault-1.5.0/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,49 +44,53 @@
         self.vecs_loaded = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
         self.last_chat_time = None
         self.first_run = True
         self.needed_sleep_time = None
+        self.saved_already = False
         self.ai = AI()
 
     def get_vaults(self, vault: str = None):
         vault = self.vault if vault is None else vault
         return call_get_vaults(self.user, self.api, vault)
 
     def get_total_vectors(self):
         return call_get_total_vectors(self.user, self.vault, self.api)
     
     def save(self, trees=16):
+        if self.saved_already == True:
+            self.clear_cache()
+            raise "The last save was aborted before the build finished. The cache was cleared and Save is empty now."
+        self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
             bytesize = os.path.getsize(temp_file.name)
             self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault, self.user, self.api, bytesize))
 
         total_saved_items = 0
         for item in self.items:
             item_text, item_id, item_meta = get_item(item)
             self.cloud_manager.upload(item_id, item_text, item_meta)
             total_saved_items += 1
 
-        self.items.clear()
-        self.x_checked = False
-        self.vecs_loaded = False
+        self.clear_cache()
 
         if self.verbose:
             print("save vectors time --- %s seconds ---" % (time.time() - start_time))
-
+        
     def clear_cache(self):
         self.items.clear()
         self.x_checked = False
         self.vecs_loaded = False
+        self.saved_already = False
 
     def delete(self):
         if self.verbose == True:
             print('Deleting started. Note: this can take a while for large datasets')
         # Clear the local vector data
         self.vectors = get_vectors(self.dims)
         self.items.clear()
@@ -153,19 +157,19 @@
             current_segment.append(last_sentence)
 
         if current_segment:
             segments.append(" ".join(current_segment))
 
         return segments
     
-    def get_similar(self, text, n: int = 4):
+    def get_similar_local(self, text, n: int = 4):
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
         return call_items_by_vector(self.user, self.vault, self.api, vector, n)
     
-    def get_similar_cloud(self, text, n: int = 4):
+    def get_similar(self, text, n: int = 4):
         return call_get_similar(self.user, self.vault, self.api, text, n)
 
     def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length lenght is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
```

### Comparing `vector_vault-1.4.0/vectorvault/vecreq.py` & `vector_vault-1.5.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.4.0/vectorvault/wrap.py` & `vector_vault-1.5.0/vectorvault/wrap.py`

 * *Files identical despite different names*


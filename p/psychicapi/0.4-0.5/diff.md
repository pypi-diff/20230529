# Comparing `tmp/psychicapi-0.4.tar.gz` & `tmp/psychicapi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.4.tar", last modified: Fri May 19 17:44:40 2023, max compression
+gzip compressed data, was "psychicapi-0.5.tar", last modified: Sun May 28 22:18:37 2023, max compression
```

## Comparing `psychicapi-0.4.tar` & `psychicapi-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.633012 psychicapi-0.4/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1759 2023-05-19 17:44:40.628633 psychicapi-0.4/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1520 2023-05-19 17:42:55.000000 psychicapi-0.4/README.md
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.599245 psychicapi-0.4/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       41 2023-05-18 20:09:12.000000 psychicapi-0.4/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1753 2023-05-18 23:32:28.000000 psychicapi-0.4/psychicapi/psychic.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-05-19 17:44:40.607410 psychicapi-0.4/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     1759 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-05-19 17:44:40.000000 psychicapi-0.4/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-05-19 17:44:40.633266 psychicapi-0.4/setup.cfg
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      638 2023-05-19 17:43:25.000000 psychicapi-0.4/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.957611 psychicapi-0.5/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1745 2023-05-28 22:18:37.957480 psychicapi-0.5/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1509 2023-05-28 19:19:43.000000 psychicapi-0.5/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.956445 psychicapi-0.5/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.5/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1732 2023-05-28 19:19:43.000000 psychicapi-0.5/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-05-28 22:18:37.957299 psychicapi-0.5/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1745 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-05-28 22:18:37.000000 psychicapi-0.5/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-05-28 22:18:37.957646 psychicapi-0.5/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      635 2023-05-28 22:15:38.000000 psychicapi-0.5/setup.py
```

### Comparing `psychicapi-0.4/PKG-INFO` & `psychicapi-0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.4
+Version: 0.5
 Summary: Psychic.dev is an open-source universal data connector for knowledgebases.
 Author: Ayan Bandyopadhyay
-Author-email: ayan@getsidekick.ai
+Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
-Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Sidekick API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
+Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/sidekick-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
 from psychicapi import ConnectorId, Psychic 
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
-# Get all active connections and optionally filter by connector id and/or connection id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, connection_id=None)
+# Get all active connections and optionally filter by connector id and/or account id
+connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "connection-id")
+docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
 ```
```

### Comparing `psychicapi-0.4/README.md` & `psychicapi-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
-Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Sidekick API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
+Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/sidekick-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
 from psychicapi import ConnectorId, Psychic 
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
-# Get all active connections and optionally filter by connector id and/or connection id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, connection_id=None)
+# Get all active connections and optionally filter by connector id and/or account id
+connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "connection-id")
+docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
 ```
```

### Comparing `psychicapi-0.4/psychicapi/psychic.py` & `psychicapi-0.5/psychicapi/psychic.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,39 +9,39 @@
     gdrive = "gdrive"
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://sidekick-ezml2kwdva-uc.a.run.app/"
         self.secret_key = secret_key
 
-    def get_documents(self, connector_id: ConnectorId, connection_id: str):
+    def get_documents(self, connector_id: ConnectorId, account_id: str):
         response = requests.post(
             self.api_url + "get-documents",
             json={
                 "connector_id": connector_id.value,
-                "connection_id": connection_id,
+                "account_id": account_id,
             },
             headers={
                 'Authorization': 'Bearer ' + self.secret_key,
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
             documents = response.json()["documents"]
             return documents
         else:
             return None
         
-    def get_connections(self, connector_id: Optional[ConnectorId] = None, connection_id: Optional[str] = None):
+    def get_connections(self, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
         filter = {}
 
         if connector_id is not None:
             filter["connector_id"] = connector_id.value
-        if connection_id is not None:
-            filter["connection_id"] = connection_id
+        if account_id is not None:
+            filter["account_id"] = account_id
 
         response = requests.post(
             self.api_url + "get-connections",
             json={
                 "filter": filter,
             },
             headers={
```

### Comparing `psychicapi-0.4/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.5/psychicapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.4
+Version: 0.5
 Summary: Psychic.dev is an open-source universal data connector for knowledgebases.
 Author: Ayan Bandyopadhyay
-Author-email: ayan@getsidekick.ai
+Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
-Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Sidekick API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
+Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
 
 ## Quick start
 
 1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-2. Use the [react library](https://docs.psychic.dev/sidekick-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps.
 3. Use `psychicapi` to retrieve documents from your active connections.
 
 ## Usage 
 
 ### Initialization
 
 ```
 from psychicapi import ConnectorId, Psychic 
 psychic = Psychic(secret_key="secret-key")
 ```
 
 ### Get active connections
 
 ```
-# Get all active connections and optionally filter by connector id and/or connection id
-connections = psychic.get_connections(connector_id=ConnectorId.notion, connection_id=None)
+# Get all active connections and optionally filter by connector id and/or account id
+connections = psychic.get_connections(connector_id=ConnectorId.notion, account_id=None)
 ```
 
 ### Retrieve documents from a connection
 
 ```
-docs = psychic.get_documents(ConnectorId.zendesk, "connection-id")
+docs = psychic.get_documents(ConnectorId.zendesk, "account_id")
 ```
```

### Comparing `psychicapi-0.4/setup.py` & `psychicapi-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.4',
+    version='0.5',
     description='Psychic.dev is an open-source universal data connector for knowledgebases.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
-    author_email='ayan@getsidekick.ai',
+    author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
         'requests',
     ],
 )
```


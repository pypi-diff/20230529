# Comparing `tmp/embedbase-1.2.1.tar.gz` & `tmp/embedbase-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.1.tar", max compression
+gzip compressed data, was "embedbase-1.2.2.tar", max compression
```

## Comparing `embedbase-1.2.1.tar` & `embedbase-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-24 18:53:24.608554 embedbase-1.2.1/LICENSE
--rw-r--r--   0        0        0     4905 2023-05-24 18:53:24.608554 embedbase-1.2.1/README.md
--rw-r--r--   0        0        0      121 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/api.py
--rw-r--r--   0        0        0    17884 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/base.py
--rw-r--r--   0        0        0     6220 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    10191 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     7571 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1095 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-24 18:53:24.724556 embedbase-1.2.1/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-24 18:53:24.728556 embedbase-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     6337 1970-01-01 00:00:00.000000 embedbase-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 17:06:51.527840 embedbase-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4931 2023-05-29 17:06:51.527840 embedbase-1.2.2/README.md
+-rw-r--r--   0        0        0      121 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/api.py
+-rw-r--r--   0        0        0    17884 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3436 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/base.py
+-rw-r--r--   0        0        0     6220 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10254 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7608 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1095 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-29 17:06:51.667847 embedbase-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.2/PKG-INFO
```

### Comparing `embedbase-1.2.1/LICENSE` & `embedbase-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/README.md` & `embedbase-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,29 +46,33 @@
 const question = 'What can I do with Embedbase API?'
 
 const embedbase = createClient(
   'https://api.embedbase.xyz',
   'api-key')
 
 const context = await embedbase
-.dataset('embedbase-docs')
-.createContext('What can I do with Embedbase API?', { limit: 3 });
+.dataset('my-documentation')
+.createContext(question);
 
-console.log(context) 
-[
+console.log(context)
+/* [
   "Embedbase API allows to store unstructured data...",
   "Embedbase API has 3 main functions a) provides a plug and play solution to store embeddings b) makes it easy to connect to get the right data into llms c)..",
   "Embedabase API is self-hostable...",
-]
+] */
 
-// refer to https://github.com/openai/openai-node for the exact api
-openai.createCompletion(
-  `Write a response to question: ${question} 
-  based on the follwing context ${context.toString()}`
-)
+
+const prompt =
+`Based on the following context:\n${context.join()}\nAnswer the user's question: ${question}`
+
+// for await allows you to stream answers
+for await (const res of embedbase.generate(prompt)) {
+    console.log(res)
+    // You, can, use, ...
+}
 // answer:
 // You can use the Embedbase API to store unstructured data and then use the data to connect it to LLMs
 ```
 
 ## Table of Contents
 
 - [Getting started](#getting-started)
```

### Comparing `embedbase-1.2.1/embedbase/__main__.py` & `embedbase-1.2.2/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/api.py` & `embedbase-1.2.2/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/app.py` & `embedbase-1.2.2/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/database/base.py` & `embedbase-1.2.2/embedbase/database/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from embedbase.models import Document
 
 
 # TODO use pydantic validation
 class Dataset(BaseModel):
     dataset_id: str
     documents_count: int
+    created_at: Optional[str]
 
 
 class SearchResponse(Document):
     score: float
 
 
 class SelectResponse(Document):
```

### Comparing `embedbase-1.2.1/embedbase/database/memory_db.py` & `embedbase-1.2.2/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/database/postgres_db.py` & `embedbase-1.2.2/embedbase/database/postgres_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     and (query_user_id is null or query_user_id = documents.user_id)
     and (metadata_field is null or documents.metadata->>metadata_field = metadata_value) -- filter by metadata
   order by documents.embedding <=> query_embedding
   limit match_count;
 end;
 $$;"""
             )
-            self.conn.execute(
+            self.conn.execute( # TODO. make this deprecated and use new api - see supabase_db
                 """
 CREATE OR REPLACE VIEW distinct_datasets AS
 SELECT dataset_id, user_id, COUNT(*) AS documents_count
 FROM documents
 GROUP BY dataset_id, user_id;
 """
             )
```

### Comparing `embedbase-1.2.1/embedbase/database/supabase_db.py` & `embedbase-1.2.2/embedbase/database/supabase_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,24 +185,25 @@
     async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
         req.execute()
 
     async def get_datasets(self, user_id: Optional[str] = None):
-        req = self.supabase.table("distinct_datasets").select(
-            "dataset_id", "documents_count"
+        req = self.supabase.table("datasets").select(
+            "name", "documents_count", "created_at"
         )
         if user_id:
-            req = req.eq("user_id", user_id)
+            req = req.eq("owner", user_id)
         data = req.execute().data
         return [
             Dataset(
-                dataset_id=row["dataset_id"],
+                dataset_id=row["name"],
                 documents_count=row["documents_count"],
+                created_at=row["created_at"],
             )
             for row in data
         ]
 
     async def list(
         self,
         dataset_id: str,
```

### Comparing `embedbase-1.2.1/embedbase/embedding/base.py` & `embedbase-1.2.2/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/embedding/cohere.py` & `embedbase-1.2.2/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/embedding/openai.py` & `embedbase-1.2.2/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/firebase_auth.py` & `embedbase-1.2.2/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/logging_utils.py` & `embedbase-1.2.2/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/models.py` & `embedbase-1.2.2/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/settings.py` & `embedbase-1.2.2/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/strings.py` & `embedbase-1.2.2/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/embedbase/utils.py` & `embedbase-1.2.2/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.1/pyproject.toml` & `embedbase-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.1"
+version = "1.2.2"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.1/PKG-INFO` & `embedbase-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.1
+Version: 1.2.2
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
@@ -79,29 +79,33 @@
 const question = 'What can I do with Embedbase API?'
 
 const embedbase = createClient(
   'https://api.embedbase.xyz',
   'api-key')
 
 const context = await embedbase
-.dataset('embedbase-docs')
-.createContext('What can I do with Embedbase API?', { limit: 3 });
+.dataset('my-documentation')
+.createContext(question);
 
-console.log(context) 
-[
+console.log(context)
+/* [
   "Embedbase API allows to store unstructured data...",
   "Embedbase API has 3 main functions a) provides a plug and play solution to store embeddings b) makes it easy to connect to get the right data into llms c)..",
   "Embedabase API is self-hostable...",
-]
+] */
 
-// refer to https://github.com/openai/openai-node for the exact api
-openai.createCompletion(
-  `Write a response to question: ${question} 
-  based on the follwing context ${context.toString()}`
-)
+
+const prompt =
+`Based on the following context:\n${context.join()}\nAnswer the user's question: ${question}`
+
+// for await allows you to stream answers
+for await (const res of embedbase.generate(prompt)) {
+    console.log(res)
+    // You, can, use, ...
+}
 // answer:
 // You can use the Embedbase API to store unstructured data and then use the data to connect it to LLMs
 ```
 
 ## Table of Contents
 
 - [Getting started](#getting-started)
```


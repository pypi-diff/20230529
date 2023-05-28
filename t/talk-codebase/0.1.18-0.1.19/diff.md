# Comparing `tmp/talk_codebase-0.1.18.tar.gz` & `tmp/talk_codebase-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.18.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.19.tar", max compression
```

## Comparing `talk_codebase-0.1.18.tar` & `talk_codebase-0.1.19.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1236 2023-05-28 20:47:11.082286 talk_codebase-0.1.18/README.md
--rw-r--r--   0        0        0      811 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1972 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/consts.py
--rw-r--r--   0        0        0     2301 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/llm.py
--rw-r--r--   0        0        0     1947 2023-05-28 20:47:11.086286 talk_codebase-0.1.18/talk_codebase/utils.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.18/PKG-INFO
+-rw-r--r--   0        0        0     1236 2023-05-28 23:29:25.976742 talk_codebase-0.1.19/README.md
+-rw-r--r--   0        0        0      811 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1972 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2854 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1955 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.19/PKG-INFO
```

### Comparing `talk_codebase-0.1.18/README.md` & `talk_codebase-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.18/pyproject.toml` & `talk_codebase-0.1.19/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.18"
+version = "0.1.19"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.18/talk_codebase/cli.py` & `talk_codebase-0.1.19/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.18/talk_codebase/consts.py` & `talk_codebase-0.1.19/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.18/talk_codebase/llm.py` & `talk_codebase-0.1.19/talk_codebase/llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,35 @@
     all_text = ''.join([text.page_content for text in texts])
     tokens = enc.encode(all_text)
     token_count = len(tokens)
     cost = (token_count / 1000) * 0.0004
     return cost
 
 
+def get_local_vector_store(embeddings):
+    try:
+        return FAISS.load_local("vector_store", embeddings)
+    except:
+        return None
+
+
 def create_vector_store(root_dir, openai_api_key, model_name):
+    embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
+    new_db = get_local_vector_store(embeddings)
+    if new_db is not None:
+        approve = questionary.select(
+            f"Found existing vector store. Do you want to use it?",
+            choices=[
+                {"name": "Yes", "value": True},
+                {"name": "No", "value": False},
+            ]
+        ).ask()
+        if approve:
+            return new_db
+
     docs = load_files(root_dir)
     if len(docs) == 0:
         print("✘ No documents found")
         exit(0)
     text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
     texts = text_splitter.split_documents(docs)
 
@@ -39,16 +59,16 @@
         ]
     ).ask()
 
     if not approve:
         exit(0)
 
     spinners = Halo(text='Creating vector store', spinner='dots').start()
-    embeddings = OpenAIEmbeddings(openai_api_key=openai_api_key)
     db = FAISS.from_documents(texts, embeddings)
+    db.save_local("vector_store")
     spinners.succeed(f"Created vector store with {len(docs)} documents")
 
     return db
 
 
 def send_question(question, vector_store, openai_api_key, model_name):
     model = ChatOpenAI(model_name=model_name, openai_api_key=openai_api_key, streaming=True,
```

### Comparing `talk_codebase-0.1.18/talk_codebase/utils.py` & `talk_codebase-0.1.19/talk_codebase/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def on_llm_end(self, response, **kwargs):
         sys.stdout.write("\n")
         sys.stdout.flush()
 
 
 def load_files(root_dir):
-    spinners = Halo(text='Loading files', spinner='dots')
+    spinners = Halo(text='Loading files', spinner='dots').start()
     docs = []
     for dirpath, dirnames, filenames in os.walk(root_dir):
         if is_ignored(dirpath, root_dir):
             continue
         if any(exclude_dir in dirpath for exclude_dir in EXCLUDE_DIRS):
             continue
         if not filenames:
```

### Comparing `talk_codebase-0.1.18/PKG-INFO` & `talk_codebase-0.1.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.18
+Version: 0.1.19
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


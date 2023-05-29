# Comparing `tmp/talk_codebase-0.1.21.tar.gz` & `tmp/talk_codebase-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.21.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.22.tar", max compression
```

## Comparing `talk_codebase-0.1.21.tar` & `talk_codebase-0.1.22.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      866 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/README.md
--rw-r--r--   0        0        0      811 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1974 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/consts.py
--rw-r--r--   0        0        0     2822 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/llm.py
--rw-r--r--   0        0        0     1568 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/utils.py
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 talk_codebase-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      866 2023-05-29 12:31:03.637641 talk_codebase-0.1.22/README.md
+-rw-r--r--   0        0        0      811 2023-05-29 12:31:03.637641 talk_codebase-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1974 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2872 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1568 2023-05-29 12:31:03.641641 talk_codebase-0.1.22/talk_codebase/utils.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 talk_codebase-0.1.22/PKG-INFO
```

### Comparing `talk_codebase-0.1.21/README.md` & `talk_codebase-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.21/pyproject.toml` & `talk_codebase-0.1.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.21"
+version = "0.1.22"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.21/talk_codebase/cli.py` & `talk_codebase-0.1.22/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.21/talk_codebase/consts.py` & `talk_codebase-0.1.22/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.21/talk_codebase/llm.py` & `talk_codebase-0.1.22/talk_codebase/llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tiktoken
 from halo import Halo
 from langchain import FAISS
 from langchain.callbacks.manager import CallbackManager
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
-from langchain.text_splitter import CharacterTextSplitter
+from langchain.text_splitter import RecursiveCharacterTextSplitter
 
 from talk_codebase.utils import StreamStdOut, load_files
 
 
 def calculate_cost(texts, model_name):
     enc = tiktoken.encoding_for_model(model_name)
     all_text = ''.join([text.page_content for text in texts])
@@ -43,15 +43,15 @@
         if approve:
             return new_db
 
     docs = load_files(root_dir)
     if len(docs) == 0:
         print("✘ No documents found")
         exit(0)
-    text_splitter = CharacterTextSplitter()
+    text_splitter = RecursiveCharacterTextSplitter(chunk_size=500, chunk_overlap=50)
     texts = text_splitter.split_documents(docs)
 
     cost = calculate_cost(docs, model_name)
     approve = questionary.select(
         f"Creating a vector store for {len(docs)} documents will cost ~${cost:.5f}. Do you want to continue?",
         choices=[
             {"name": "Yes", "value": True},
@@ -70,12 +70,12 @@
     return db
 
 
 def send_question(question, vector_store, openai_api_key, model_name):
     model = ChatOpenAI(model_name=model_name, openai_api_key=openai_api_key, streaming=True,
                        callback_manager=CallbackManager([StreamStdOut()]))
     qa = ConversationalRetrievalChain.from_llm(model,
-                                               retriever=vector_store.as_retriever(search_kwargs={"k": 2}),
+                                               retriever=vector_store.as_retriever(search_kwargs={"k": 4}),
                                                return_source_documents=True)
     answer = qa({"question": question, "chat_history": []})
     print('\n' + '\n'.join([f'📄 {os.path.abspath(s.metadata["source"])}:' for s in answer["source_documents"]]))
     return answer
```

### Comparing `talk_codebase-0.1.21/talk_codebase/utils.py` & `talk_codebase-0.1.22/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.21/PKG-INFO` & `talk_codebase-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.21
+Version: 0.1.22
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


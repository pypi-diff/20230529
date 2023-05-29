# Comparing `tmp/talk_codebase-0.1.19.tar.gz` & `tmp/talk_codebase-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.19.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.20.tar", max compression
```

## Comparing `talk_codebase-0.1.19.tar` & `talk_codebase-0.1.20.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1236 2023-05-28 23:29:25.976742 talk_codebase-0.1.19/README.md
--rw-r--r--   0        0        0      811 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1972 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/consts.py
--rw-r--r--   0        0        0     2854 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/llm.py
--rw-r--r--   0        0        0     1955 2023-05-28 23:29:25.980742 talk_codebase-0.1.19/talk_codebase/utils.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0     1236 2023-05-29 00:30:33.804166 talk_codebase-0.1.20/README.md
+-rw-r--r--   0        0        0      811 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1972 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2822 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1955 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/utils.py
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.20/PKG-INFO
```

### Comparing `talk_codebase-0.1.19/README.md` & `talk_codebase-0.1.20/README.md`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.19/pyproject.toml` & `talk_codebase-0.1.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.19"
+version = "0.1.20"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.19/talk_codebase/cli.py` & `talk_codebase-0.1.20/talk_codebase/cli.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.19/talk_codebase/consts.py` & `talk_codebase-0.1.20/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.19/talk_codebase/llm.py` & `talk_codebase-0.1.20/talk_codebase/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if approve:
             return new_db
 
     docs = load_files(root_dir)
     if len(docs) == 0:
         print("✘ No documents found")
         exit(0)
-    text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
+    text_splitter = CharacterTextSplitter()
     texts = text_splitter.split_documents(docs)
 
     cost = calculate_cost(docs, model_name)
     approve = questionary.select(
         f"Creating a vector store for {len(docs)} documents will cost ~${cost:.5f}. Do you want to continue?",
         choices=[
             {"name": "Yes", "value": True},
```

### Comparing `talk_codebase-0.1.19/talk_codebase/utils.py` & `talk_codebase-0.1.20/talk_codebase/utils.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.19/PKG-INFO` & `talk_codebase-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.19
+Version: 0.1.20
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


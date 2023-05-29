# Comparing `tmp/talk_codebase-0.1.20.tar.gz` & `tmp/talk_codebase-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talk_codebase-0.1.20.tar", max compression
+gzip compressed data, was "talk_codebase-0.1.21.tar", max compression
```

## Comparing `talk_codebase-0.1.20.tar` & `talk_codebase-0.1.21.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1236 2023-05-29 00:30:33.804166 talk_codebase-0.1.20/README.md
--rw-r--r--   0        0        0      811 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/__init__.py
--rw-r--r--   0        0        0     1972 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/cli.py
--rw-r--r--   0        0        0      518 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/consts.py
--rw-r--r--   0        0        0     2822 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/llm.py
--rw-r--r--   0        0        0     1955 2023-05-29 00:30:33.808166 talk_codebase-0.1.20/talk_codebase/utils.py
--rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 talk_codebase-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0      866 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/README.md
+-rw-r--r--   0        0        0      811 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/__init__.py
+-rw-r--r--   0        0        0     1974 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/cli.py
+-rw-r--r--   0        0        0      518 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/consts.py
+-rw-r--r--   0        0        0     2822 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/llm.py
+-rw-r--r--   0        0        0     1568 2023-05-29 12:09:12.191593 talk_codebase-0.1.21/talk_codebase/utils.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 talk_codebase-0.1.21/PKG-INFO
```

### Comparing `talk_codebase-0.1.20/pyproject.toml` & `talk_codebase-0.1.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talk-codebase"
-version = "0.1.20"
+version = "0.1.21"
 description = "talk-codebase is a powerful tool for querying and analyzing codebases."
 authors = ["Saryev Rustam <rustam1997@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "talk_codebase" }]
 keywords = ["chatgpt", "openai", "cli"]
 
 [tool.poetry.dependencies]
```

### Comparing `talk_codebase-0.1.20/talk_codebase/cli.py` & `talk_codebase-0.1.21/talk_codebase/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key.")
             configure()
             chat(root_dir)
         else:
-            print(f"🤖 Error: {e}")
+            print(f"\n🤖 Error: {e}")
 
 
 def main():
     fire.Fire({
         "chat": chat,
         "configure": configure,
     })
```

### Comparing `talk_codebase-0.1.20/talk_codebase/consts.py` & `talk_codebase-0.1.21/talk_codebase/consts.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.20/talk_codebase/llm.py` & `talk_codebase-0.1.21/talk_codebase/llm.py`

 * *Files identical despite different names*

### Comparing `talk_codebase-0.1.20/talk_codebase/utils.py` & `talk_codebase-0.1.21/talk_codebase/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import glob
 import os
 import sys
 
 from git import Repo
 from halo import Halo
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.document_loaders import TextLoader
 
-from talk_codebase.consts import EXCLUDE_DIRS, EXCLUDE_FILES, ALLOW_FILES
+from talk_codebase.consts import EXCLUDE_FILES, ALLOW_FILES
 
 
 def get_repo(root_dir):
     try:
         return Repo(root_dir)
     except:
         return None
@@ -38,26 +39,16 @@
         sys.stdout.write("\n")
         sys.stdout.flush()
 
 
 def load_files(root_dir):
     spinners = Halo(text='Loading files', spinner='dots').start()
     docs = []
-    for dirpath, dirnames, filenames in os.walk(root_dir):
-        if is_ignored(dirpath, root_dir):
+    for file_path in glob.glob(os.path.join(root_dir, '**/*'), recursive=True):
+        if is_ignored(file_path, root_dir):
             continue
-        if any(exclude_dir in dirpath for exclude_dir in EXCLUDE_DIRS):
-            continue
-        if not filenames:
-            continue
-        for file in filenames:
-            if is_ignored(os.path.join(dirpath, file), root_dir):
-                continue
-            if any(file.endswith(allow_file) for allow_file in ALLOW_FILES) and not any(
-                    file == exclude_file for exclude_file in EXCLUDE_FILES):
-                try:
-                    loader = TextLoader(os.path.join(dirpath, file), encoding='utf-8')
-                    docs.extend(loader.load_and_split())
-                except Exception as e:
-                    print(f"Error loading file {file}: {e}")
+        if any(file_path.endswith(allow_file) for allow_file in ALLOW_FILES) and not any(
+                file_path.endswith(exclude_file) for exclude_file in EXCLUDE_FILES):
+            loader = TextLoader(file_path, encoding='utf-8')
+            docs.extend(loader.load_and_split())
     spinners.succeed(f"Loaded {len(docs)} documents")
     return docs
```

### Comparing `talk_codebase-0.1.20/PKG-INFO` & `talk_codebase-0.1.21/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talk-codebase
-Version: 0.1.20
+Version: 0.1.21
 Summary: talk-codebase is a powerful tool for querying and analyzing codebases.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rustam1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,21 +25,14 @@
 
 [![Node.js Package](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rsaryev/talk-codebase/actions/workflows/python-publish.yml)
 
 <p align="center">
   <img src="https://github.com/rsaryev/talk-codebase/assets/70219513/b5d338f9-14a5-417b-9690-83f5cd66facf" width="800" alt="chat">
 </p>
 
-## Description
-
-In the chat, you can ask questions about the codebase. AI will answer your questions, and if necessary, it will offer
-code improvements. This is very convenient when you want to quickly find something in the codebase, but don't want to
-waste time searching. It is also convenient when you want to improve a specific function, you can ask "How can I improve
-the function {function name}?" and AI will suggest improvements. Codebase is analyzed using openai.
-
 ## Installation
 
 ```bash
 pip install talk-codebase
 ```
 
 ## Usage
@@ -54,7 +47,11 @@
 # Configure
 talk-codebase configure
 
 # Help
 talk-codebase --help
 ```
 
+## Requirements
+
+- Python 3.9
+- OpenAI API key [api-keys](https://platform.openai.com/account/api-keys)
```


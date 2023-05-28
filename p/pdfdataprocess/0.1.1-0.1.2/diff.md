# Comparing `tmp/pdfdataprocess-0.1.1.tar.gz` & `tmp/pdfdataprocess-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfdataprocess-0.1.1.tar", max compression
+gzip compressed data, was "pdfdataprocess-0.1.2.tar", max compression
```

## Comparing `pdfdataprocess-0.1.1.tar` & `pdfdataprocess-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1488 2023-05-28 22:19:47.614985 pdfdataprocess-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-28 20:36:12.887072 pdfdataprocess-0.1.1/pdfdataprocess/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-28 21:20:53.332188 pdfdataprocess-0.1.1/pdfdataprocess/cli.py
--rw-r--r--   0        0        0     1911 2023-05-28 21:26:05.916932 pdfdataprocess-0.1.1/pdfdataprocess/process.py
--rw-r--r--   0        0        0      531 2023-05-28 22:22:35.181111 pdfdataprocess-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 pdfdataprocess-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-05-28 22:19:47.614985 pdfdataprocess-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 20:36:12.887072 pdfdataprocess-0.1.2/pdfdataprocess/__init__.py
+-rw-r--r--   0        0        0     1559 2023-05-28 23:17:58.852146 pdfdataprocess-0.1.2/pdfdataprocess/cli.py
+-rw-r--r--   0        0        0     1911 2023-05-28 21:26:05.916932 pdfdataprocess-0.1.2/pdfdataprocess/process.py
+-rw-r--r--   0        0        0      531 2023-05-28 23:18:57.051246 pdfdataprocess-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 pdfdataprocess-0.1.2/PKG-INFO
```

### Comparing `pdfdataprocess-0.1.1/README.md` & `pdfdataprocess-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pdfdataprocess-0.1.1/pdfdataprocess/cli.py` & `pdfdataprocess-0.1.2/pdfdataprocess/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,16 @@
 from .process import processJSON
 
 app = typer.Typer(
     name = "pdf-dataset-process",
     help = "Process a PDF dataset to a JSONL file.",
     no_args_is_help=True
 )
-
-@app.command("init", help="Initialize the project.")
-def init():
-    """
-    Initialize the project.
-    """
-    npm.call(['i', 'pdf2json'])
-    
     
+@app.command("make-json", help="Process a PDF dataset to a JSONL file.")    
 @app.command("mkjson", help="Process a PDF dataset to a JSONL file.")
 def mkjson(
     file: str = typer.Option(None, '-f', '--file')
     ):
     """
     Process a PDF dataset to a JSONL file.
     """
```

### Comparing `pdfdataprocess-0.1.1/pdfdataprocess/process.py` & `pdfdataprocess-0.1.2/pdfdataprocess/process.py`

 * *Files identical despite different names*

### Comparing `pdfdataprocess-0.1.1/pyproject.toml` & `pdfdataprocess-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdfdataprocess"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["arnos-stuff <bcda0276@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/arnos-stuff/pdf-data-process.git"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `pdfdataprocess-0.1.1/PKG-INFO` & `pdfdataprocess-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdataprocess
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/arnos-stuff/pdf-data-process.git
 Author: arnos-stuff
 Author-email: bcda0276@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


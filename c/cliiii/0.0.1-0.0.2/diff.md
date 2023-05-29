# Comparing `tmp/cliiii-0.0.1.tar.gz` & `tmp/cliiii-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliiii-0.0.1.tar", max compression
+gzip compressed data, was "cliiii-0.0.2.tar", max compression
```

## Comparing `cliiii-0.0.1.tar` & `cliiii-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 cliiii-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 cliiii-0.0.1/README.md
--rw-r--r--   0        0        0      646 2023-05-29 10:29:16.405304 cliiii-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 cliiii-0.0.1/src/cliiii/__init__.py
--rw-r--r--   0        0        0     1749 2023-05-29 10:29:27.266173 cliiii-0.0.1/src/cliiii/main.py
--rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 cliiii-0.0.1/src/cliiii/utils.py
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 cliiii-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 cliiii-0.0.2/LICENSE
+-rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 cliiii-0.0.2/README.md
+-rw-r--r--   0        0        0      646 2023-05-29 10:32:06.789594 cliiii-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 cliiii-0.0.2/src/cliiii/__init__.py
+-rw-r--r--   0        0        0     1749 2023-05-29 10:32:25.256832 cliiii-0.0.2/src/cliiii/main.py
+-rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 cliiii-0.0.2/src/cliiii/utils.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 cliiii-0.0.2/PKG-INFO
```

### Comparing `cliiii-0.0.1/LICENSE` & `cliiii-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliiii-0.0.1/pyproject.toml` & `cliiii-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cliiii"
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Shubham Dogra <shubham.dogra@pingsafe.com>"]
 description = "A small example package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -16,13 +16,13 @@
 
 
 [tool.poetry.dependencies]
 requests = "^2.30.0"
 
 
 [tool.poetry.scripts]
-cli = "piicli.main:run_cli"
+cli = "cliiii.main:run_cli"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `cliiii-0.0.1/src/cliiii/main.py` & `cliiii-0.0.2/src/cliiii/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def run_cli():
     try:
         package_name = "piicli"
         binary_name = "secrets"
         pre_execution_workflow(package_name, binary_name)
-        print("Running main cli, version: 0.0.1")
+        print("Running main cli, version: 0.0.2")
         execute_binary(package_name, binary_name)
     except Exception as e:
         print(e)
 
 
 if __name__ == '__main__':
     run_cli()
```

### Comparing `cliiii-0.0.1/PKG-INFO` & `cliiii-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliiii
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author: Shubham Dogra
 Author-email: shubham.dogra@pingsafe.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```


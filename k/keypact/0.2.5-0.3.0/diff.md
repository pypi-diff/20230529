# Comparing `tmp/keypact-0.2.5.tar.gz` & `tmp/keypact-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.2.5.tar", last modified: Tue May  9 07:29:21 2023, max compression
+gzip compressed data, was "keypact-0.3.0.tar", last modified: Mon May 29 10:02:13 2023, max compression
```

## Comparing `keypact-0.2.5.tar` & `keypact-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:29:21.644160 keypact-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-09 07:29:12.000000 keypact-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-09 07:29:21.644160 keypact-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-09 07:29:12.000000 keypact-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:29:21.644160 keypact-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 07:29:12.000000 keypact-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:29:21.640160 keypact-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:29:21.644160 keypact-0.2.5/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 07:29:12.000000 keypact-0.2.5/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-09 07:29:12.000000 keypact-0.2.5/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:29:21.644160 keypact-0.2.5/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 07:29:21.000000 keypact-0.2.5/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:02:13.352301 keypact-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 10:02:01.000000 keypact-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 10:02:13.352301 keypact-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-29 10:02:01.000000 keypact-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:02:13.352301 keypact-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 10:02:01.000000 keypact-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:02:13.348301 keypact-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:02:13.348301 keypact-0.3.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 10:02:01.000000 keypact-0.3.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-29 10:02:01.000000 keypact-0.3.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:02:13.352301 keypact-0.3.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:02:13.000000 keypact-0.3.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.2.5/LICENSE` & `keypact-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.2.5/PKG-INFO` & `keypact-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.5
+Version: 0.3.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
         
         ## Features
         - Multithread Support
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
+        - Able to saving files
         
         
         ## Installation
-        You can install Keypact by pip3:
+        You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
         ```
         
         ## Usage
-        Keypact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
+        KeyPact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
         
         
         ### In Python
         
         ```python
         import keypact
         
@@ -47,15 +48,15 @@
         ```
         ```console
         keypact --name=client_addresses get Onur
         ```
         
         
         ## Contributing
-        Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
+        Contributions to KeyPact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
         
         ## License
-        Keypact is released under the MIT License.
+        KeyPact is released under the MIT License.
         
 Platform: UNKNOWN
 Requires-Python: >= 3
 Description-Content-Type: text/markdown
```

### Comparing `keypact-0.2.5/README.md` & `keypact-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 ## Features
 - Multithread Support
 - Simultaneous Writing
 - Easy to use
 - Easy to integrate
 - Easy to deploy
+- Able to saving files
 
 
 ## Installation
-You can install Keypact by pip3:
+You can install KeyPact by pip3:
 
 ```console
 pip3 install keypact
 ```
 
 ## Usage
-Keypact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
+KeyPact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
 
 
 ### In Python
 
 ```python
 import keypact
 
@@ -39,11 +40,11 @@
 ```
 ```console
 keypact --name=client_addresses get Onur
 ```
 
 
 ## Contributing
-Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
+Contributions to KeyPact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
 
 ## License
-Keypact is released under the MIT License.
+KeyPact is released under the MIT License.
```

### Comparing `keypact-0.2.5/setup.py` & `keypact-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.2.5',
+version='0.3.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.2.5/src/keypact/keypact.py` & `keypact-0.3.0/src/keypact/keypact.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from hashlib import sha256
 import pickle
 
 import fire
 
 import time
+from shutil import move, copy
 
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
@@ -21,23 +22,40 @@
     def initialize(self):
         try: 
             os.makedirs(self.location)
         except OSError:
             if not os.path.isdir(self.location):
                 raise
 
-    def set(self, key: str, value):
+    def set(self, key: str, value, type_of_value="str"):
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         with open(os.path.join(self.location, key_location), "wb") as f:
-            pickle.dump({"key":key,"value":value}, f)
+            pickle.dump({"key":key,"value":value, "type":type}, f)
+
+
+    def set_file(self, key: str, file, dont_remove: bool = False):
+
+        self.set(key, file, type_of_value="file")
+        key_name = self.get_file(key)
+        if not dont_remove:
+            move(file, os.path.join(self.location, key_name))
+        else:
+            copy(file, os.path.join(self.location, key_name))
+
+    def get_file(self, key: str, custom_key_location: str = None):
+        the_key = self.get(key,custom_key_location)
+        return the_key+the_key.split("/")[-1]
+
+
+
 
     def get(self, key: str, custom_key_location: str = None):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
 
@@ -61,14 +79,16 @@
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
         total_result = None
 
         try:
             with open(os.path.join(self.location, key_location), "rb") as f:
                 result = pickle.load(f)
+                if not "type" in result:
+                    result["type"] = "str"
                 try:
                     total_result = result["key"]
                 except TypeError:
                     total_result = False
         except EOFError or FileNotFoundError:
             pass            
         return total_result
@@ -77,14 +97,24 @@
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
         try:
             os.remove(os.path.join(self.location, key_location))
         except OSError:
             pass
 
+    def delete_file(self, key: str):
+        
+
+        try:
+            os.remove(os.path.join(self.location, self.get_file(key)))
+        except OSError:
+            pass
+
+        self.delete(key)
+        
 
     def dict(self):
         result ={}
         for key in os.listdir(self.location):
             the_key = self.get_key(key)
             if not the_key is None:
                 if the_key != False:
```

### Comparing `keypact-0.2.5/src/keypact.egg-info/PKG-INFO` & `keypact-0.3.0/src/keypact.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.2.5
+Version: 0.3.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
         
         ## Features
         - Multithread Support
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
+        - Able to saving files
         
         
         ## Installation
-        You can install Keypact by pip3:
+        You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
         ```
         
         ## Usage
-        Keypact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
+        KeyPact is aimed to be used in Python and command line as well. You can use it in your Python code or in command line.
         
         
         ### In Python
         
         ```python
         import keypact
         
@@ -47,15 +48,15 @@
         ```
         ```console
         keypact --name=client_addresses get Onur
         ```
         
         
         ## Contributing
-        Contributions to Keypact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
+        Contributions to KeyPact are welcome! If you have any suggestions or find a bug, please open an issue on the GitHub repository. If you want to contribute code, please fork the repository and create a pull request.
         
         ## License
-        Keypact is released under the MIT License.
+        KeyPact is released under the MIT License.
         
 Platform: UNKNOWN
 Requires-Python: >= 3
 Description-Content-Type: text/markdown
```


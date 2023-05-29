# Comparing `tmp/keypact-0.3.1.tar.gz` & `tmp/keypact-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.3.1.tar", last modified: Mon May 29 10:16:11 2023, max compression
+gzip compressed data, was "keypact-0.4.0.tar", last modified: Mon May 29 17:19:52 2023, max compression
```

## Comparing `keypact-0.3.1.tar` & `keypact-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:16:11.106815 keypact-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 10:15:58.000000 keypact-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 10:16:11.106815 keypact-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-29 10:15:58.000000 keypact-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:16:11.106815 keypact-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 10:15:58.000000 keypact-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:16:11.106815 keypact-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:16:11.106815 keypact-0.3.1/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 10:15:58.000000 keypact-0.3.1/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-29 10:15:58.000000 keypact-0.3.1/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:16:11.106815 keypact-0.3.1/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 10:16:11.000000 keypact-0.3.1/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:16:10.000000 keypact-0.3.1/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.981456 keypact-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 17:19:39.000000 keypact-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 17:19:52.981456 keypact-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-29 17:19:39.000000 keypact-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:19:52.981456 keypact-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 17:19:39.000000 keypact-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.973456 keypact-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.977456 keypact-0.4.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 17:19:39.000000 keypact-0.4.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-29 17:19:39.000000 keypact-0.4.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.981456 keypact-0.4.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.3.1/LICENSE` & `keypact-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.3.1/PKG-INFO` & `keypact-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.3.1
+Version: 0.4.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

### Comparing `keypact-0.3.1/README.md` & `keypact-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `keypact-0.3.1/setup.py` & `keypact-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.3.1',
+version='0.4.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.3.1/src/keypact/keypact.py` & `keypact-0.4.0/src/keypact/keypact.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,70 +13,124 @@
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
 
+
+        self.counter = 0
+
         self.initialize()
 
     def initialize(self):
         try: 
             os.makedirs(self.location)
         except OSError:
             if not os.path.isdir(self.location):
                 raise
 
-    def set(self, key: str, value, type_of_value="str"):
+    def set(self, key: str, value, type_of_value="str") -> str:
+        self.counter += 1
+        
+        
+
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
         key_location_loading = os.path.join(self.location, key_location+".l")
+        key_location_loading_indicator = os.path.join(self.location, key_location+".li")
+
+        key_location_reading_indicator = os.path.join(self.location, key_location+".re")
+
+        
+
+
         with open(key_location_loading, "wb") as f:
             pickle.dump({"key":key,"value":value, "type":type}, f)
 
+
+        #Create a file that inform is loading
+        with open(key_location_loading_indicator, "wb") as f:
+            f.write(b"1")
+
+        while os.path.exists(key_location_reading_indicator):
+                    time.sleep(0.25)
+
         move(key_location_loading, key_location)
 
+        #Remove the loading indicator
+        os.remove(key_location_loading_indicator)
+
+        return key
+
 
-    def set_file(self, key: str, file, dont_remove: bool = False):
+    def set_withrkey(self, value, type_of_value="str") -> str:
+        key = str(self.counter) + str(time.time())
+        return self.set(key, value, type_of_value)
 
-        self.set(key, file, type_of_value="file")
+
+    def set_file(self, key: str, file, dont_remove: bool = False) -> str:
+
+        the_key = self.set(key, file, type_of_value="file")
         key_name = self.get_file(key)
         if not dont_remove:
             move(file, os.path.join(self.location, key_name))
         else:
             copy(file, os.path.join(self.location, key_name))
 
+        return the_key
+
+
+    def set_file_withrkey(self, file, dont_remove: bool = False) -> str:
+        key = str(self.counter) + str(time.time())
+        return self.set_file(key, file, dont_remove)
+
+
     def get_file(self, key: str, custom_key_location: str = None):
         the_key = self.get(key,custom_key_location)
         return the_key+the_key.split("/")[-1]
 
 
 
 
     def get(self, key: str, custom_key_location: str = None):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
+        key_location_loading_indicator = os.path.join(self.location, key_location+".li")
+        key_location_reading_indicator = os.path.join(self.location, key_location+".re")
+
+        while os.path.exists(key_location_loading_indicator):
+            time.sleep(0.1)
+
+
+
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
 
         total_result = None
 
         try:
+            
+            with open(key_location_reading_indicator, "wb") as f:
+                f.write(b"1")
             with open(os.path.join(self.location, key_location), "rb") as f:
                 result = pickle.load(f)
                 try:
                     total_result = result["value"]
                 except TypeError:
                     total_result = result
         except EOFError or FileNotFoundError:
             pass
 
+        if os.path.isfile(key_location_reading_indicator):
+            os.remove(key_location_reading_indicator)
+
         return total_result
 
     def get_key(self, key_location: str):
        
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
```

### Comparing `keypact-0.3.1/src/keypact.egg-info/PKG-INFO` & `keypact-0.4.0/src/keypact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.3.1
+Version: 0.4.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```


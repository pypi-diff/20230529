# Comparing `tmp/graphql_service_framework-1.1.8.tar.gz` & `tmp/graphql_service_framework-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_service_framework-1.1.8.tar", last modified: Thu Apr 27 15:54:06 2023, max compression
+gzip compressed data, was "graphql_service_framework-1.1.9.tar", last modified: Thu Apr 27 16:19:29 2023, max compression
```

## Comparing `graphql_service_framework-1.1.8.tar` & `graphql_service_framework-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:54:06.793369 graphql_service_framework-1.1.8/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 15:54:06.793369 graphql_service_framework-1.1.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:54:06.790369 graphql_service_framework-1.1.8/graphql_service_framework/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15660 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/query.graphql
--rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/schema_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/service.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/graphql_service_framework/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:54:06.792369 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-27 15:54:06.000000 graphql_service_framework-1.1.8/graphql_service_framework.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-27 15:54:06.794369 graphql_service_framework-1.1.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:54:06.793369 graphql_service_framework-1.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/tests/test_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-27 15:53:56.000000 graphql_service_framework-1.1.8/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:19:29.076861 graphql_service_framework-1.1.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 16:19:29.076861 graphql_service_framework-1.1.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-27 16:19:28.000000 graphql_service_framework-1.1.9/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:19:29.073861 graphql_service_framework-1.1.9/graphql_service_framework/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15660 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/query.graphql
+-rw-rw-rw-   0 root         (0) root         (0)     7954 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8360 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/schema_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/graphql_service_framework/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:19:29.075861 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      693 2023-04-27 16:19:29.000000 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-27 16:19:29.000000 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:19:29.000000 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-27 16:19:29.000000 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-27 16:19:29.000000 graphql_service_framework-1.1.9/graphql_service_framework.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-27 16:19:29.077861 graphql_service_framework-1.1.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1465 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:19:29.076861 graphql_service_framework-1.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/tests/test_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-27 16:19:18.000000 graphql_service_framework-1.1.9/tests/utils.py
```

### Comparing `graphql_service_framework-1.1.8/LICENSE` & `graphql_service_framework-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/PKG-INFO` & `graphql_service_framework-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_service_framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.8.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.9.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/conftest.py` & `graphql_service_framework-1.1.9/graphql_service_framework/conftest.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/mesh.py` & `graphql_service_framework-1.1.9/graphql_service_framework/mesh.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/middleware.py` & `graphql_service_framework-1.1.9/graphql_service_framework/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/schema.py` & `graphql_service_framework-1.1.9/graphql_service_framework/schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/schema_tracker.py` & `graphql_service_framework-1.1.9/graphql_service_framework/schema_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,18 +86,25 @@
             print(
                 f"Installed package " f"{self.name} version {v} at "
                 f"{install_location}"
             )
             schema = None
             err = None
             try:
+                location = os.path.join(install_location, self.package_name, self.name)
+                package_name = f"{self.package_name}.{self.name}"
                 prev_modules = find_modules(
-                    os.path.join(install_location, self.package_name, self.name),
-                    f"{self.package_name}.{self.name}",
+                    location,
+                    package_name,
                 )
+                if not prev_modules:
+                    raise TypeError(
+                        f"Could not find any modules in {location} with package "
+                        f"name {package_name}"
+                    )
 
                 schema = find_schema(prev_modules)
             except Exception as _err:
                 err = _err
 
             if not schema:
                 raise TypeError(
@@ -215,20 +222,23 @@
 
         print(f"Releasing {self.name} because {release_reason}")
         print(f"Creating setup.py in {self.path} for {self.name}")
 
         setup_data = (
             inspect.cleandoc(
                 """
-            from setuptools import setup, find_packages
+            from setuptools import setup, find_namespace_packages
 
             setup(
                 name='SERVICE_NAME',
                 version='SERVICE_VERSION',
-                packages=find_packages(include=['SERVICE_PACKAGE','SERVICE_PACKAGE.*']),
+                packages=find_namespace_packages(include=[
+                    'SERVICE_PACKAGE',
+                    'SERVICE_PACKAGE.*'
+                ]),
                 install_requires=[
                     'packaging',
                     'graphql-service-framework'
                 ]
             )
             """
             )
```

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/service.py` & `graphql_service_framework-1.1.9/graphql_service_framework/service.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework/utils.py` & `graphql_service_framework-1.1.9/graphql_service_framework/utils.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework.egg-info/PKG-INFO` & `graphql_service_framework-1.1.9/graphql_service_framework.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-service-framework
-Version: 1.1.8
+Version: 1.1.9
 Summary: GraphQL Service Framework.
 Home-page: https://gitlab.com/parob/graphql-service-framework
-Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.8.zip
+Download-URL: https://gitlab.com/parob/graphql-service-framework/-/archive/master/graphql-service-framework-v1.1.9.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_service_framework-1.1.8/graphql_service_framework.egg-info/SOURCES.txt` & `graphql_service_framework-1.1.9/graphql_service_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/setup.py` & `graphql_service_framework-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/tests/test_schema.py` & `graphql_service_framework-1.1.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/tests/test_service_manager.py` & `graphql_service_framework-1.1.9/tests/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `graphql_service_framework-1.1.8/tests/utils.py` & `graphql_service_framework-1.1.9/tests/utils.py`

 * *Files identical despite different names*


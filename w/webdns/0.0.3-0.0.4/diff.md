# Comparing `tmp/webdns-0.0.3.tar.gz` & `tmp/webdns-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdns-0.0.3.tar", last modified: Mon May 29 13:10:35 2023, max compression
+gzip compressed data, was "webdns-0.0.4.tar", last modified: Mon May 29 18:37:31 2023, max compression
```

## Comparing `webdns-0.0.3.tar` & `webdns-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.130000 webdns-0.0.3/
--rwxrwxr-x   0 root         (0) root         (0)     1055 2023-05-25 14:04:05.000000 webdns-0.0.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-29 13:10:35.129000 webdns-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 13:10:35.130000 webdns-0.0.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     3976 2023-05-25 18:25:34.000000 webdns-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:34.964000 webdns-0.0.3/webdns/
--rwxrwxr-x   0 root         (0) root         (0)       75 2023-05-25 13:50:57.000000 webdns-0.0.3/webdns/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)       98 2023-05-29 13:04:09.000000 webdns-0.0.3/webdns/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.127000 webdns-0.0.3/webdns/api/
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-05-25 13:50:59.000000 webdns-0.0.3/webdns/api/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2083 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/api/api.py
--rwxrwxr-x   0 root         (0) root         (0)      826 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/api/utils.py
--rwxrwxr-x   0 root         (0) root         (0)     2896 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/app.py
--rwxrwxr-x   0 root         (0) root         (0)     3394 2023-05-24 20:14:17.000000 webdns-0.0.3/webdns/methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.072000 webdns-0.0.3/webdns.egg-info/
--rwxrwxr-x   0 root         (0) root         (0)      720 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)      303 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/SOURCES.txt
--rwxrwxr-x   0 root         (0) root         (0)        1 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/dependency_links.txt
--rwxrwxr-x   0 root         (0) root         (0)       26 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/requires.txt
--rwxrwxr-x   0 root         (0) root         (0)        7 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 18:37:31.602000 webdns-0.0.4/
+-rwxrwxr-x   0 root         (0) root         (0)     1055 2023-05-25 14:04:05.000000 webdns-0.0.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-29 18:37:31.601000 webdns-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 18:37:31.602000 webdns-0.0.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     4073 2023-05-29 18:36:56.000000 webdns-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 18:37:31.599000 webdns-0.0.4/webdns/
+-rwxrwxr-x   0 root         (0) root         (0)       75 2023-05-25 13:50:57.000000 webdns-0.0.4/webdns/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)       98 2023-05-29 18:33:17.000000 webdns-0.0.4/webdns/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 18:37:31.601000 webdns-0.0.4/webdns/api/
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-05-25 13:50:59.000000 webdns-0.0.4/webdns/api/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2083 2023-05-24 14:43:52.000000 webdns-0.0.4/webdns/api/api.py
+-rwxrwxr-x   0 root         (0) root         (0)      826 2023-05-24 14:43:52.000000 webdns-0.0.4/webdns/api/utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     2896 2023-05-24 14:43:52.000000 webdns-0.0.4/webdns/app.py
+-rwxrwxr-x   0 root         (0) root         (0)     3394 2023-05-24 20:14:17.000000 webdns-0.0.4/webdns/methods.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 18:37:31.600000 webdns-0.0.4/webdns.egg-info/
+-rwxrwxr-x   0 root         (0) root         (0)      720 2023-05-29 18:37:31.000000 webdns-0.0.4/webdns.egg-info/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)      303 2023-05-29 18:37:31.000000 webdns-0.0.4/webdns.egg-info/SOURCES.txt
+-rwxrwxr-x   0 root         (0) root         (0)        1 2023-05-29 18:37:31.000000 webdns-0.0.4/webdns.egg-info/dependency_links.txt
+-rwxrwxr-x   0 root         (0) root         (0)       26 2023-05-29 18:37:31.000000 webdns-0.0.4/webdns.egg-info/requires.txt
+-rwxrwxr-x   0 root         (0) root         (0)        7 2023-05-29 18:37:31.000000 webdns-0.0.4/webdns.egg-info/top_level.txt
```

### Comparing `webdns-0.0.3/LICENSE.txt` & `webdns-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webdns-0.0.3/PKG-INFO` & `webdns-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdns
-Version: 0.0.3
+Version: 0.0.4
 Summary: DnsMasq utility to name IP addresses from Netbox NSOT.
 Home-page: https://git.rnp.br/pop-rj/dns-conectividade
 Author: PoP-RJ/RNP - BR
 Author-email: infra@pop-rj.rnp.br
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `webdns-0.0.3/setup.py` & `webdns-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,15 +109,22 @@
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
-    install_requires=REQUIRED,
+    # install_requires=REQUIRED,
+
+    install_requires=[
+        'pynetbox',
+        'jsonschema',
+        'flask',
+    ],
+    
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
```

### Comparing `webdns-0.0.3/webdns/api/api.py` & `webdns-0.0.4/webdns/api/api.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.3/webdns/api/utils.py` & `webdns-0.0.4/webdns/api/utils.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.3/webdns/app.py` & `webdns-0.0.4/webdns/app.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.3/webdns/methods.py` & `webdns-0.0.4/webdns/methods.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.3/webdns.egg-info/PKG-INFO` & `webdns-0.0.4/webdns.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdns
-Version: 0.0.3
+Version: 0.0.4
 Summary: DnsMasq utility to name IP addresses from Netbox NSOT.
 Home-page: https://git.rnp.br/pop-rj/dns-conectividade
 Author: PoP-RJ/RNP - BR
 Author-email: infra@pop-rj.rnp.br
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```


# Comparing `tmp/c2client-0.8.tar.gz` & `tmp/c2client-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/c2client-0.8.tar", last modified: Wed Mar 31 14:08:33 2021, max compression
+gzip compressed data, was "dist/c2client-0.9.tar", last modified: Fri Jul  2 07:58:56 2021, max compression
```

## Comparing `c2client-0.8.tar` & `c2client-0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-03-31 14:08:33.000000 c2client-0.8/
-drwxr-xr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-03-31 14:08:33.000000 c2client-0.8/c2client/
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)       20 2021-03-31 14:06:11.000000 c2client-0.8/c2client/__init__.py
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)     3650 2021-03-31 13:58:30.000000 c2client-0.8/c2client/shell.py
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)      856 2021-03-31 13:58:30.000000 c2client-0.8/c2client/c2rc_convert.py
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      723 2019-11-11 13:34:53.000000 c2client-0.8/c2client/compat.py
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1957 2019-11-11 13:34:53.000000 c2client-0.8/c2client/utils.py
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       59 2019-06-14 12:45:36.000000 c2client-0.8/MANIFEST.in
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)       38 2021-03-31 14:08:33.000000 c2client-0.8/setup.cfg
-drwxr-xr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)        9 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/top_level.txt
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      350 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/SOURCES.txt
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       14 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/requires.txt
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)        1 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/dependency_links.txt
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      156 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/entry_points.txt
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     2142 2021-03-31 14:08:33.000000 c2client-0.8/c2client.egg-info/PKG-INFO
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)     1541 2021-03-31 14:06:11.000000 c2client-0.8/setup.py
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)     2142 2021-03-31 14:08:33.000000 c2client-0.8/PKG-INFO
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1258 2019-06-14 12:45:36.000000 c2client-0.8/Makefile
--rw-r--r--   0 akulaev   (1000) akulaev   (1000)     1797 2021-03-31 14:06:11.000000 c2client-0.8/c2-client.spec
--rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1069 2019-06-14 12:45:36.000000 c2client-0.8/README.rst
+drwxrwxr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-07-02 07:58:56.000000 c2client-0.9/
+drwxrwxr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-07-02 07:58:56.000000 c2client-0.9/c2client/
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       20 2021-07-02 07:55:52.000000 c2client-0.9/c2client/__init__.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     4177 2021-07-02 07:51:56.000000 c2client-0.9/c2client/shell.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      377 2021-07-02 07:51:56.000000 c2client-0.9/c2client/errors.py
+-rw-r--r--   0 akulaev   (1000) akulaev   (1000)      856 2021-03-31 13:58:30.000000 c2client-0.9/c2client/c2rc_convert.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      723 2019-11-11 13:34:53.000000 c2client-0.9/c2client/compat.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     2086 2021-07-02 07:51:56.000000 c2client-0.9/c2client/utils.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       59 2019-06-14 12:45:36.000000 c2client-0.9/MANIFEST.in
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       38 2021-07-02 07:58:56.000000 c2client-0.9/setup.cfg
+drwxrwxr-x   0 akulaev   (1000) akulaev   (1000)        0 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)        9 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/top_level.txt
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      369 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/SOURCES.txt
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)       38 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/requires.txt
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)        1 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/dependency_links.txt
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)      189 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/entry_points.txt
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     2142 2021-07-02 07:58:56.000000 c2client-0.9/c2client.egg-info/PKG-INFO
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1636 2021-07-02 07:51:56.000000 c2client-0.9/setup.py
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     2142 2021-07-02 07:58:56.000000 c2client-0.9/PKG-INFO
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1258 2019-06-14 12:45:36.000000 c2client-0.9/Makefile
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1873 2021-07-02 07:56:45.000000 c2client-0.9/c2-client.spec
+-rw-rw-r--   0 akulaev   (1000) akulaev   (1000)     1069 2019-06-14 12:45:36.000000 c2client-0.9/README.rst
```

### Comparing `c2client-0.8/c2client/c2rc_convert.py` & `c2client-0.9/c2client/c2rc_convert.py`

 * *Files identical despite different names*

### Comparing `c2client-0.8/c2client/compat.py` & `c2client-0.9/c2client/compat.py`

 * *Files identical despite different names*

### Comparing `c2client-0.8/c2client/utils.py` & `c2client-0.9/c2client/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+import os
+
 from lxml import etree
 
+from c2client.errors import EnvironmentVariableError, MalformedParametersError
+
 
 def prettify_xml(string):
     """Returns prettified XML string."""
 
     parser = etree.XMLParser(remove_blank_text=True)
     tree = etree.fromstring(string, parser)
     return etree.tostring(tree, pretty_print=True, encoding="unicode")
 
 
-class MalformedParametersException(Exception):
-    def __init__(self):
-        super(MalformedParametersException, self).__init__(
-            "Malformed parameters.")
-
-
 def from_dot_notation(source):
     """Converts a incoming query to a request dictionary.
     For example::
         1. {"Action": ["Action"], "Param": ["Value"]}
         2. {"Action": ["Action"], "Param.2": ["Value2"], "Param.1": ["Value1"]}
         3. {"Action": ["Action"], "Param.SubParam": ["Value"]}
     would  result in the params dict::
@@ -29,15 +27,15 @@
     :param query: This is dictionary, returned by '_get_query()'.
     """
     result = {"result": {}}
     for key, value in sorted(source.items()):
         try:
             _process_tokens(key.split("."), value, result, "result")
         except Exception:
-            raise MalformedParametersException
+            raise MalformedParametersError
     return result["result"]
 
 
 def _process_tokens(tokens, value, parent, index):
     key, rest = tokens[0], tokens[1:]
     if key.isdigit():
         key = int(key) - 1
@@ -45,13 +43,22 @@
     if not isinstance(key, int):
         parent[index].setdefault(key, {})
     elif isinstance(parent[index], dict) and not parent[index]:
         parent[index] = [{}]
     elif isinstance(parent[index], list) and len(parent[index]) == key:
         parent[index].append({})
     elif not (isinstance(parent[index], list) and len(parent[index]) > key):
-        raise MalformedParametersException
+        raise MalformedParametersError
 
     if rest:
         _process_tokens(rest, value, parent[index], key)
     else:
         parent[index][key] = value
+
+
+def get_env_var(name):
+    """Returns env_var by it's name or raises EnvironmentError."""
+
+    env_var = os.environ.get(name)
+    if env_var is None:
+        raise EnvironmentVariableError(name)
+    return env_var
```

### Comparing `c2client-0.8/c2client.egg-info/PKG-INFO` & `c2client-0.9/c2client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: c2client
-Version: 0.8
+Version: 0.9
 Summary: CROC Cloud Platform - API Client
 Home-page: https://github.com/c2devel/c2-client
 Author: CROC Cloud Team
 Author-email: devel@croc.ru
 Maintainer: Andrey Kulaev
 Maintainer-email: adkulaev@gmail.com
 License: GPL3
```

### Comparing `c2client-0.8/setup.py` & `c2client-0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 PACKAGE_PATH = os.path.abspath(os.path.dirname(__file__))
 
 def get_description():
     with open(os.path.join(PACKAGE_PATH, "README.rst")) as readme:
         return readme.read()
 
 install_requires = [
-    "boto", "lxml", "six"
+    "boto",
+    "boto3",
+    "inflection==0.3.1",
+    "lxml",
+    "six",
 ]
 # argparse moved to stdlib in python2.7
 if sys.version_info[0] == 2 and sys.version_info[1] <= 6:
     install_requires.append("argparse")
 
 setup(
     name="c2client",
@@ -42,11 +46,12 @@
     install_requires=install_requires,
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "c2-ct = c2client.shell:ct_main",
             "c2-cw = c2client.shell:cw_main",
             "c2-ec2 = c2client.shell:ec2_main",
+            "c2-eks = c2client.shell:eks_main",
             "c2rc-convert = c2client.c2rc_convert:main",
         ]
     },
 )
```

### Comparing `c2client-0.8/PKG-INFO` & `c2client-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: c2client
-Version: 0.8
+Version: 0.9
 Summary: CROC Cloud Platform - API Client
 Home-page: https://github.com/c2devel/c2-client
 Author: CROC Cloud Team
 Author-email: devel@croc.ru
 Maintainer: Andrey Kulaev
 Maintainer-email: adkulaev@gmail.com
 License: GPL3
```

### Comparing `c2client-0.8/Makefile` & `c2client-0.9/Makefile`

 * *Files identical despite different names*

### Comparing `c2client-0.8/c2-client.spec` & `c2client-0.9/c2-client.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 %if 0%{?rhel} && 0%{?rhel} <= 6
 %{!?__python2: %global __python2 /usr/bin/python2}
 %{!?python2_sitelib: %global python2_sitelib %(%{__python2} -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())")}
 %endif
 
 Name:    c2-client
-Version: 0.8
+Version: 0.9
 Release: 1%{?dist}
 Summary: CROC Cloud platform API client
 
 Group:   Development/Tools
 License: GPLv3
 URL:     https://github.com/c2devel/c2-client
 Source:  %name-%version.tar.gz
@@ -58,14 +58,17 @@
 
 
 %clean
 [ "%buildroot" = "/" ] || rm -rf "%buildroot"
 
 
 %changelog
+* Fri Jul 02 2021 Andrey Kulaev <adkulaev@gmail.com> - 0.9-1
+- New version
+
 * Wed Mar 31 2021 Andrey Kulaev <adkulaev@gmail.com> - 0.8-1
 - New version
 
 * Mon Dec 02 2019 Andrey Kulaev <adkulaev@gmail.com> - 0.7-1
 - New version
 
 * Mon Nov 11 2019 Andrey Kulaev <adkulaev@gmail.com> - 0.6-1
```

### Comparing `c2client-0.8/README.rst` & `c2client-0.9/README.rst`

 * *Files identical despite different names*


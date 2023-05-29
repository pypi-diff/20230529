# Comparing `tmp/salespyforce-1.0.0.tar.gz` & `tmp/salespyforce-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salespyforce-1.0.0.tar", last modified: Mon May  8 21:43:05 2023, max compression
+gzip compressed data, was "salespyforce-1.1.0.tar", last modified: Mon May 29 19:57:38 2023, max compression
```

## Comparing `salespyforce-1.0.0.tar` & `salespyforce-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.329912 salespyforce-1.0.0/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.0.0/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)     6118 2023-05-08 21:43:05.329493 salespyforce-1.0.0/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     4761 2023-05-08 21:38:49.000000 salespyforce-1.0.0/README.md
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-08 21:43:05.330028 salespyforce-1.0.0/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.0.0/setup.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.305652 salespyforce-1.0.0/src/
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.314649 salespyforce-1.0.0/src/salespyforce/
--rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.0.0/src/salespyforce/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.0.0/src/salespyforce/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.0.0/src/salespyforce/chatter.py
--rw-r--r--   0 shurtj     (501) staff       (20)    44432 2023-03-14 20:25:38.000000 salespyforce-1.0.0/src/salespyforce/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.324116 salespyforce-1.0.0/src/salespyforce/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.0.0/src/salespyforce/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.0.0/src/salespyforce/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.0.0/src/salespyforce/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.0.0/src/salespyforce/knowledge.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.328976 salespyforce-1.0.0/src/salespyforce/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.0.0/src/salespyforce/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5697 2023-03-16 21:08:51.000000 salespyforce-1.0.0/src/salespyforce/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.0.0/src/salespyforce/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.0.0/src/salespyforce/utils/log_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-05-08 21:39:27.000000 salespyforce-1.0.0/src/salespyforce/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-08 21:43:05.319036 salespyforce-1.0.0/src/salespyforce.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)     6118 2023-05-08 21:43:05.000000 salespyforce-1.0.0/src/salespyforce.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)      646 2023-05-08 21:43:05.000000 salespyforce-1.0.0/src/salespyforce.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-08 21:43:05.000000 salespyforce-1.0.0/src/salespyforce.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-05-08 21:43:05.000000 salespyforce-1.0.0/src/salespyforce.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-05-08 21:43:05.000000 salespyforce-1.0.0/src/salespyforce.egg-info/top_level.txt
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.447479 salespyforce-1.1.0/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2023-01-22 19:54:55.000000 salespyforce-1.1.0/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-05-29 19:57:38.446785 salespyforce-1.1.0/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     7818 2023-05-24 20:39:33.000000 salespyforce-1.1.0/README.md
+-rw-r--r--   0 shurtj     (501) staff       (20)      569 2023-05-23 21:22:33.000000 salespyforce-1.1.0/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-29 19:57:38.447782 salespyforce-1.1.0/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3153 2023-05-08 21:41:53.000000 salespyforce-1.1.0/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.415876 salespyforce-1.1.0/src/
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.423567 salespyforce-1.1.0/src/salespyforce/
+-rw-r--r--   0 shurtj     (501) staff       (20)     2031 2023-05-08 21:19:50.000000 salespyforce-1.1.0/src/salespyforce/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5763 2023-02-17 19:12:52.000000 salespyforce-1.1.0/src/salespyforce/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7494 2023-03-13 21:18:18.000000 salespyforce-1.1.0/src/salespyforce/chatter.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    45246 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.434429 salespyforce-1.1.0/src/salespyforce/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      320 2023-03-13 21:37:03.000000 salespyforce-1.1.0/src/salespyforce/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    17057 2023-03-13 21:39:59.000000 salespyforce-1.1.0/src/salespyforce/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      479 2023-02-22 22:06:11.000000 salespyforce-1.1.0/src/salespyforce/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    21657 2023-02-22 22:09:03.000000 salespyforce-1.1.0/src/salespyforce/knowledge.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.441744 salespyforce-1.1.0/src/salespyforce/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      292 2023-03-13 21:51:57.000000 salespyforce-1.1.0/src/salespyforce/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5697 2023-03-16 21:08:51.000000 salespyforce-1.1.0/src/salespyforce/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5661 2023-03-14 20:43:01.000000 salespyforce-1.1.0/src/salespyforce/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11799 2023-01-22 21:52:54.000000 salespyforce-1.1.0/src/salespyforce/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.445539 salespyforce-1.1.0/src/salespyforce/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      242 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4772 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1416 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_instantiate_object.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1840 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_sobjects.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      709 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_soql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      809 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/tests/test_sosl.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      733 2023-05-29 19:55:32.000000 salespyforce-1.1.0/src/salespyforce/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-29 19:57:38.429594 salespyforce-1.1.0/src/salespyforce.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)     9175 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)      930 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      272 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)       13 2023-05-29 19:57:38.000000 salespyforce-1.1.0/src/salespyforce.egg-info/top_level.txt
```

### Comparing `salespyforce-1.0.0/LICENSE` & `salespyforce-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/setup.py` & `salespyforce-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/__init__.py` & `salespyforce-1.1.0/src/salespyforce/__init__.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/api.py` & `salespyforce-1.1.0/src/salespyforce/api.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/chatter.py` & `salespyforce-1.1.0/src/salespyforce/chatter.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/core.py` & `salespyforce-1.1.0/src/salespyforce/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,21 @@
 
     def get_api_versions(self):
         """This method returns the API versions for the Salesforce releases.
         (`Reference <https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/dome_versions.htm>`_)
         """
         return self.get('/services/data')
 
+    def get_org_limits(self):
+        """This method returns a list of all org limits.
+
+        .. versionadded:: 1.1.0
+        """
+        return self.get(f'/services/data/{self.version}/limits')
+
     def get_all_sobjects(self):
         """This method returns a list of all Salesforce objects. (i.e. sObjects)
         (`Reference <https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/dome_describeGlobal.htm>`_)
         """
         return self.get(f'/services/data/{self.version}/sobjects')
 
     def get_sobject(self, object_name, describe=False):
@@ -324,14 +331,29 @@
         :returns: The result of the SOQL query
         """
         if replace_quotes:
             query = query.replace('"', "'")
         query = core_utils.url_encode(query)
         return self.get(f'/services/data/{self.version}/query/?q={query}')
 
+    def search_string(self, string_to_search):
+        """This method performs a SOSL query to search for a given string.
+        (`Reference <https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/resources_search.htm>`_)
+
+        .. versionadded:: 1.1.0
+
+        :param string_to_search: The string for which to search
+        :type string_to_search: str
+        :returns: The SOSL response data in JSON format
+        """
+        query = 'FIND {' + string_to_search + '}'
+        query = core_utils.url_encode(query)
+        return self.get(f'/services/data/{self.version}/search/?q={query}')
+
+
     def create_sobject_record(self, sobject, payload):
         """This method creates a new record for a specific sObject.
         (`Reference <https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/dome_sobject_create.htm>`_)
 
         :param sobject: The sObject under which to create the new record
         :type sobject: str
         :param payload: The JSON payload with the record details
```

### Comparing `salespyforce-1.0.0/src/salespyforce/errors/exceptions.py` & `salespyforce-1.1.0/src/salespyforce/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/knowledge.py` & `salespyforce-1.1.0/src/salespyforce/knowledge.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/utils/core_utils.py` & `salespyforce-1.1.0/src/salespyforce/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/utils/helper.py` & `salespyforce-1.1.0/src/salespyforce/utils/helper.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/utils/log_utils.py` & `salespyforce-1.1.0/src/salespyforce/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `salespyforce-1.0.0/src/salespyforce/utils/version.py` & `salespyforce-1.1.0/src/salespyforce/utils/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 :Module:            salespyforce.utils.version
 :Synopsis:          This simple script contains the package version
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     22 Jan 2023
+:Modified Date:     27 May 2023
 """
 
 from . import log_utils
 
 # Initialize logging
 logger = log_utils.initialize_logging(__name__)
 
 # Define special and global variables
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 def get_full_version():
     """This function returns the current full version of the ``salespyforce`` package."""
     return __version__
```


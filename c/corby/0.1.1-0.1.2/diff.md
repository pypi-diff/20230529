# Comparing `tmp/corby-0.1.1.tar.gz` & `tmp/corby-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.1.1.tar", last modified: Fri May 26 15:08:01 2023, max compression
+gzip compressed data, was "corby-0.1.2.tar", last modified: Mon May 29 08:20:50 2023, max compression
```

## Comparing `corby-0.1.1.tar` & `corby-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-26 15:07:43.000000 corby-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 15:08:01.203511 corby-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-26 15:07:43.000000 corby-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:07:43.000000 corby-0.1.1/corby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:07:43.000000 corby-0.1.1/corby/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/corby/generator/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/base_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/chatbot/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.203511 corby-0.1.1/corby/generator/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 15:07:43.000000 corby-0.1.1/corby/generator/notebook/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-26 15:07:43.000000 corby-0.1.1/corby/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:08:01.199511 corby-0.1.1/corby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 15:08:01.000000 corby-0.1.1/corby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:08:01.203511 corby-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-26 15:07:43.000000 corby-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.012341 corby-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-29 08:20:23.000000 corby-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-29 08:20:50.012341 corby-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-29 08:20:23.000000 corby-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.004341 corby-0.1.2/corby/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-29 08:20:23.000000 corby-0.1.2/corby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-29 08:20:23.000000 corby-0.1.2/corby/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.008341 corby-0.1.2/corby/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.008341 corby-0.1.2/corby/generator/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/base_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/chatbot/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.012341 corby-0.1.2/corby/generator/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-29 08:20:23.000000 corby-0.1.2/corby/generator/notebook/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-29 08:20:23.000000 corby-0.1.2/corby/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:20:50.008341 corby-0.1.2/corby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-29 08:20:49.000000 corby-0.1.2/corby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-29 08:20:50.000000 corby-0.1.2/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:20:49.000000 corby-0.1.2/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 08:20:49.000000 corby-0.1.2/corby.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 08:20:49.000000 corby-0.1.2/corby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 08:20:49.000000 corby-0.1.2/corby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:20:50.012341 corby-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 08:20:23.000000 corby-0.1.2/setup.py
```

### Comparing `corby-0.1.1/LICENSE` & `corby-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/PKG-INFO` & `corby-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.1.1
+Version: 0.1.2
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `corby-0.1.1/README.md` & `corby-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/corby/generator/base.py` & `corby-0.1.2/corby/generator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,19 @@
         raise NotImplementedError
 
     def create(self, name):
         '''Generates a new entity'''
         app_path = os.getcwd() + '/' + name
         selected_template = self.ask_template()
         template_params = {}
-        if hasattr(self, 'get_generator_params'):
-            template_params.update(self.get_generator_params(name))
+        try:
+            generator_params = self.get_generator_params(name)
+        except NotImplementedError:
+            generator_params = {}
+        template_params.update(generator_params)
         self.clone_template(selected_template["template_url"], selected_template["template_name"])
         template_custom_inputs = self.ask_template_inputs(selected_template["template_name"])
         if bool(template_custom_inputs):
             template_params.update(template_custom_inputs)
         self.replace_in_folder(
             selected_template["template_name"] + '/skeleton',
             template_params
```

### Comparing `corby-0.1.1/corby/generator/chatbot/base_chatbot.py` & `corby-0.1.2/corby/generator/chatbot/base_chatbot.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     def get_chatbot_params(self):
         '''Returns the specific questions required for each kind of chatbot'''
         raise NotImplementedError
 
     def get_generator_params(self, name):
         '''Returns the specific parameters for chatbots'''
         template_params = {'chatbot_name': name}
-        if hasattr(self, 'get_chatbot_params'):
+        try:
             chatbot_specific_params = self.get_chatbot_params()
-            if bool(chatbot_specific_params):
-                template_params.update(chatbot_specific_params)
+        except NotImplementedError:
+            chatbot_specific_params = {}
+        if bool(chatbot_specific_params):
+            template_params.update(chatbot_specific_params)
         return template_params
 
     def create_chatbot(self, name):
         '''Calls super.create() to generate a new chatbot
         we may have custom logic here on the future'''
         return super().create(name)
```

### Comparing `corby-0.1.1/corby/generator/chatbot/index.py` & `corby-0.1.2/corby/generator/chatbot/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/corby/generator/chatbot/telegram.py` & `corby-0.1.2/corby/generator/chatbot/telegram.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/corby/generator/notebook/index.py` & `corby-0.1.2/corby/generator/notebook/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/corby/index.py` & `corby-0.1.2/corby/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Main CLI entrypoint for Corby"""
 
 import argparse
 from string import Template
 from .generator.chatbot.index import create_chatbot
 from .generator.notebook.index import create_notebook
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 # We'll include more features in the future
 available_actions = ['new']
 
 available_entities = ['chatbot', 'notebook']
 
 parser = argparse.ArgumentParser(
```

### Comparing `corby-0.1.1/corby.egg-info/PKG-INFO` & `corby-0.1.2/corby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.1.1
+Version: 0.1.2
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `corby-0.1.1/corby.egg-info/SOURCES.txt` & `corby-0.1.2/corby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corby-0.1.1/setup.py` & `corby-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Pypi setup file for corby'''
 
 from setuptools import setup, find_packages
 
 setup(
     name="corby",
-    version="0.1.1",
+    version="0.1.2",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     # pylint: disable=consider-using-with
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
```


# Comparing `tmp/taskcli-0.0.5.tar.gz` & `tmp/taskcli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcli-0.0.5.tar", last modified: Mon May 29 15:01:35 2023, max compression
+gzip compressed data, was "taskcli-0.0.6.tar", last modified: Mon May 29 15:06:47 2023, max compression
```

## Comparing `taskcli-0.0.5.tar` & `taskcli-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.857935 taskcli-0.0.5/
--rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.5/LICENSE
--rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:01:35.858008 taskcli-0.0.5/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)     1781 2023-05-29 14:52:00.000000 taskcli-0.0.5/README.md
--rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.5/pyproject.toml
--rw-r--r--   0 p          (501) staff       (20)      405 2023-05-29 15:01:35.858346 taskcli-0.0.5/setup.cfg
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.855103 taskcli-0.0.5/src/
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.856896 taskcli-0.0.5/src/taskcli/
--rw-r--r--   0 p          (501) staff       (20)      144 2023-05-29 14:27:39.000000 taskcli-0.0.5/src/taskcli/__init__.py
--rw-r--r--   0 p          (501) staff       (20)     8253 2023-05-29 14:25:30.000000 taskcli-0.0.5/src/taskcli/old.py
--rw-r--r--   0 p          (501) staff       (20)    18599 2023-05-29 14:59:52.000000 taskcli-0.0.5/src/taskcli/taskcli.py
-drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.857828 taskcli-0.0.5/src/taskcli.egg-info/
--rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)      248 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/SOURCES.txt
--rw-r--r--   0 p          (501) staff       (20)        1 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/dependency_links.txt
--rw-r--r--   0 p          (501) staff       (20)        8 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/top_level.txt
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.801714 taskcli-0.0.6/
+-rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.6/LICENSE
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:06:47.801781 taskcli-0.0.6/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)     1781 2023-05-29 14:52:00.000000 taskcli-0.0.6/README.md
+-rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.6/pyproject.toml
+-rw-r--r--   0 p          (501) staff       (20)      405 2023-05-29 15:06:47.802058 taskcli-0.0.6/setup.cfg
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.798726 taskcli-0.0.6/src/
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.800525 taskcli-0.0.6/src/taskcli/
+-rw-r--r--   0 p          (501) staff       (20)      144 2023-05-29 14:27:39.000000 taskcli-0.0.6/src/taskcli/__init__.py
+-rw-r--r--   0 p          (501) staff       (20)     8253 2023-05-29 14:25:30.000000 taskcli-0.0.6/src/taskcli/old.py
+-rw-r--r--   0 p          (501) staff       (20)    18634 2023-05-29 15:06:23.000000 taskcli-0.0.6/src/taskcli/taskcli.py
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:06:47.801613 taskcli-0.0.6/src/taskcli.egg-info/
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)      248 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/SOURCES.txt
+-rw-r--r--   0 p          (501) staff       (20)        1 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/dependency_links.txt
+-rw-r--r--   0 p          (501) staff       (20)        8 2023-05-29 15:06:47.000000 taskcli-0.0.6/src/taskcli.egg-info/top_level.txt
```

### Comparing `taskcli-0.0.5/LICENSE` & `taskcli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.5/README.md` & `taskcli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.5/src/taskcli/old.py` & `taskcli-0.0.6/src/taskcli/old.py`

 * *Files identical despite different names*

### Comparing `taskcli-0.0.5/src/taskcli/taskcli.py` & `taskcli-0.0.6/src/taskcli/taskcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,19 +219,20 @@
 
 
 def trace(msg):
     print(msg)
     pass
 
 
-def task(namespace=None, foo=None, env=None, required_env=None, main=False):
+def task(namespace=None, foo=None, env=None, required_env=None, main=False, aliases=None):
     """
     ns: command namespace. Allows for laying command in additional namespace
     env: environment variables to assert
     main: if True, this task will be run if no task name is specified
+    aliases: not implemented yet
     """
 
     def task_wrapper(fn):
         # this generats the decorator
         @functools.wraps(fn)
         def wrapper(*args, **kwargs):
             # this gets called right before the function
@@ -308,15 +309,14 @@
 #         self.previous_task = None
 
 #     def processing_arg(self, func_name):
 #         self.current_task = func_name
 #         if self.previous_task != self.current_task:
 #             for k,v in task_data.items():
 
-import rich
 
 
 def arg(
     *names,
     type=None,
     default=EMPTY,
     choices=None,
```


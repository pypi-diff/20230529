# Comparing `tmp/xenoslib-0.1.28.1.tar.gz` & `tmp/xenoslib-0.1.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.28.1.tar", last modified: Mon May 29 02:26:03 2023, max compression
+gzip compressed data, was "xenoslib-0.1.28.2.tar", last modified: Mon May 29 02:29:50 2023, max compression
```

## Comparing `xenoslib-0.1.28.1.tar` & `xenoslib-0.1.28.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:26:03.324610 xenoslib-0.1.28.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:26:03.324610 xenoslib-0.1.28.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:26:03.324610 xenoslib-0.1.28.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:26:03.320609 xenoslib-0.1.28.1/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-29 02:25:47.000000 xenoslib-0.1.28.1/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:26:03.324610 xenoslib-0.1.28.1/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:26:03.000000 xenoslib-0.1.28.1/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 02:26:03.000000 xenoslib-0.1.28.1/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:26:03.000000 xenoslib-0.1.28.1/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 02:26:03.000000 xenoslib-0.1.28.1/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 02:26:03.000000 xenoslib-0.1.28.1/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.376768 xenoslib-0.1.28.2/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-29 02:29:34.000000 xenoslib-0.1.28.2/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:29:50.380768 xenoslib-0.1.28.2/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 02:29:50.000000 xenoslib-0.1.28.2/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.28.1/LICENSE` & `xenoslib-0.1.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/README.md` & `xenoslib-0.1.28.2/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/setup.py` & `xenoslib-0.1.28.2/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/base.py` & `xenoslib-0.1.28.2/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/dev.py` & `xenoslib-0.1.28.2/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/extend.py` & `xenoslib-0.1.28.2/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/linux.py` & `xenoslib-0.1.28.2/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/mail.py` & `xenoslib-0.1.28.2/xenoslib/mail.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/mock.py` & `xenoslib-0.1.28.2/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/onedrive.py` & `xenoslib-0.1.28.2/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/win_trayicon.py` & `xenoslib-0.1.28.2/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.28.1/xenoslib/windows.py` & `xenoslib-0.1.28.2/xenoslib/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,31 +100,29 @@
             return value
 
     def update(self, environs):
         for key, value in environs.items():
             self.set(key, value)
         self.refresh()
 
-    def set_and_update(self, key, value):
-        self.set(key, value)
-        self.refresh()
+
 
 def add_windows_path_env(new_path):
     """Add directory to Windows path environment variable"""
     env = Environment()
     path_str = env.get("Path")
     path_list = path_str.split(";")
     if new_path in path_list:
         print(f"{new_path} already exists in the path, skip.")
         return False
     else:
         path_list.append(new_path)
         new_path_list = ";".join(path_list)
         try:
-            env.set_and_update("Path", new_path_list)
+            env.update({"Path": new_path_list})
             print(f"Added {new_path} to the path")
             return True
         except Exception as exc:
             print(f"Failed to update the path: {str(exc)}")
             return False
```


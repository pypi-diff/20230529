# Comparing `tmp/serializer-for-oop-progect-1.0.0.tar.gz` & `tmp/serializer-for-oop-progect-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/annayedka/Documents/MySerializer/dist/.tmp-o6x9cmm0/serializer-for-oop-progect-1.0.0.tar", last modified: Mon May 29 07:47:59 2023, max compression
+gzip compressed data, was "/Users/annayedka/Documents/MySerializer/dist/.tmp-hj4hgw8k/serializer-for-oop-progect-1.1.0.tar", last modified: Mon May 29 14:44:18 2023, max compression
```

## Comparing `serializer-for-oop-progect-1.0.0.tar` & `serializer-for-oop-progect-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 07:47:59.800845 serializer-for-oop-progect-1.0.0/
-drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 07:47:59.797081 serializer-for-oop-progect-1.0.0/MySer/
--rw-r--r--   0 annayedka   (501) staff       (20)      635 2023-05-29 07:38:40.000000 serializer-for-oop-progect-1.0.0/MySer/JSONSer.py
--rw-r--r--   0 annayedka   (501) staff       (20)        0 2023-05-29 07:43:41.000000 serializer-for-oop-progect-1.0.0/MySer/__init__.py
--rw-r--r--   0 annayedka   (501) staff       (20)       88 2023-05-29 07:47:59.800328 serializer-for-oop-progect-1.0.0/PKG-INFO
-drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 07:47:59.799676 serializer-for-oop-progect-1.0.0/serializer_for_oop_progect.egg-info/
--rw-r--r--   0 annayedka   (501) staff       (20)       88 2023-05-29 07:47:59.000000 serializer-for-oop-progect-1.0.0/serializer_for_oop_progect.egg-info/PKG-INFO
--rw-r--r--   0 annayedka   (501) staff       (20)      243 2023-05-29 07:47:59.000000 serializer-for-oop-progect-1.0.0/serializer_for_oop_progect.egg-info/SOURCES.txt
--rw-r--r--   0 annayedka   (501) staff       (20)        1 2023-05-29 07:47:59.000000 serializer-for-oop-progect-1.0.0/serializer_for_oop_progect.egg-info/dependency_links.txt
--rw-r--r--   0 annayedka   (501) staff       (20)        6 2023-05-29 07:47:59.000000 serializer-for-oop-progect-1.0.0/serializer_for_oop_progect.egg-info/top_level.txt
--rw-r--r--   0 annayedka   (501) staff       (20)       38 2023-05-29 07:47:59.800978 serializer-for-oop-progect-1.0.0/setup.cfg
--rw-r--r--   0 annayedka   (501) staff       (20)      145 2023-05-29 07:44:36.000000 serializer-for-oop-progect-1.0.0/setup.py
+drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 14:44:18.882645 serializer-for-oop-progect-1.1.0/
+drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 14:44:18.874492 serializer-for-oop-progect-1.1.0/MySer/
+-rw-r--r--   0 annayedka   (501) staff       (20)      653 2023-05-29 14:43:52.000000 serializer-for-oop-progect-1.1.0/MySer/JSONSer.py
+-rw-r--r--   0 annayedka   (501) staff       (20)        0 2023-05-29 07:43:41.000000 serializer-for-oop-progect-1.1.0/MySer/__init__.py
+-rw-r--r--   0 annayedka   (501) staff       (20)       88 2023-05-29 14:44:18.881173 serializer-for-oop-progect-1.1.0/PKG-INFO
+drwxr-xr-x   0 annayedka   (501) staff       (20)        0 2023-05-29 14:44:18.879778 serializer-for-oop-progect-1.1.0/serializer_for_oop_progect.egg-info/
+-rw-r--r--   0 annayedka   (501) staff       (20)       88 2023-05-29 14:44:18.000000 serializer-for-oop-progect-1.1.0/serializer_for_oop_progect.egg-info/PKG-INFO
+-rw-r--r--   0 annayedka   (501) staff       (20)      243 2023-05-29 14:44:18.000000 serializer-for-oop-progect-1.1.0/serializer_for_oop_progect.egg-info/SOURCES.txt
+-rw-r--r--   0 annayedka   (501) staff       (20)        1 2023-05-29 14:44:18.000000 serializer-for-oop-progect-1.1.0/serializer_for_oop_progect.egg-info/dependency_links.txt
+-rw-r--r--   0 annayedka   (501) staff       (20)        6 2023-05-29 14:44:18.000000 serializer-for-oop-progect-1.1.0/serializer_for_oop_progect.egg-info/top_level.txt
+-rw-r--r--   0 annayedka   (501) staff       (20)       38 2023-05-29 14:44:18.883024 serializer-for-oop-progect-1.1.0/setup.cfg
+-rw-r--r--   0 annayedka   (501) staff       (20)      145 2023-05-29 14:44:02.000000 serializer-for-oop-progect-1.1.0/setup.py
```

### Comparing `serializer-for-oop-progect-1.0.0/MySer/JSONSer.py` & `serializer-for-oop-progect-1.1.0/MySer/JSONSer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any
 
 
 class JSONEncoderForClass(json.JSONEncoder):
     def default(self, o: Any) -> Any:
         try:
             d = o.__dict__
-        except TypeError:
+        except (TypeError, AttributeError):
             pass
         else:
             return d
         return json.JSONEncoder.default(self, o)
 
 
 class MyJSONSer:
```


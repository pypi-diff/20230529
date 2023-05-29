# Comparing `tmp/tensorflou-1.0.tar.gz` & `tmp/tensorflou-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflou-1.0.tar", last modified: Mon May 29 01:58:25 2023, max compression
+gzip compressed data, was "tensorflou-2.0.tar", last modified: Mon May 29 02:02:24 2023, max compression
```

## Comparing `tensorflou-1.0.tar` & `tensorflou-2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:58:25.489015 tensorflou-1.0/
--rw-rw-rw-   0        0        0      162 2023-05-29 01:58:25.488000 tensorflou-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-29 01:58:25.489972 tensorflou-1.0/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-05-29 01:57:54.000000 tensorflou-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:58:25.477974 tensorflou-1.0/tensorflou/
--rw-rw-rw-   0        0        0     4089 2023-05-28 17:30:49.000000 tensorflou-1.0/tensorflou/1.txt
--rw-rw-rw-   0        0        0     4079 2023-05-28 17:33:57.000000 tensorflou-1.0/tensorflou/11.txt
--rw-rw-rw-   0        0        0     5964 2023-05-28 17:34:39.000000 tensorflou-1.0/tensorflou/12.txt
--rw-rw-rw-   0        0        0     2790 2023-05-28 17:34:58.000000 tensorflou-1.0/tensorflou/13.txt
--rw-rw-rw-   0        0        0     4356 2023-05-28 17:35:15.000000 tensorflou-1.0/tensorflou/14.txt
--rw-rw-rw-   0        0        0      869 2023-05-28 17:35:30.000000 tensorflou-1.0/tensorflou/15.txt
--rw-rw-rw-   0        0        0     2315 2023-05-28 17:35:41.000000 tensorflou-1.0/tensorflou/16.txt
--rw-rw-rw-   0        0        0     2954 2023-05-28 17:36:05.000000 tensorflou-1.0/tensorflou/17.txt
--rw-rw-rw-   0        0        0     5831 2023-05-28 17:36:23.000000 tensorflou-1.0/tensorflou/18.txt
--rw-rw-rw-   0        0        0     1438 2023-05-28 17:36:41.000000 tensorflou-1.0/tensorflou/19.txt
--rw-rw-rw-   0        0        0     6452 2023-05-28 17:31:44.000000 tensorflou-1.0/tensorflou/2.txt
--rw-rw-rw-   0        0        0     2619 2023-05-28 17:36:53.000000 tensorflou-1.0/tensorflou/20.txt
--rw-rw-rw-   0        0        0     2189 2023-05-28 17:32:00.000000 tensorflou-1.0/tensorflou/3.txt
--rw-rw-rw-   0        0        0     4135 2023-05-28 17:32:28.000000 tensorflou-1.0/tensorflou/4.txt
--rw-rw-rw-   0        0        0     2536 2023-05-28 17:32:57.000000 tensorflou-1.0/tensorflou/5.txt
--rw-rw-rw-   0        0        0      226 2023-05-29 01:58:01.000000 tensorflou-1.0/tensorflou/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:58:25.484986 tensorflou-1.0/tensorflou.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-29 01:58:25.000000 tensorflou-1.0/tensorflou.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-05-29 01:58:25.000000 tensorflou-1.0/tensorflou.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:58:25.000000 tensorflou-1.0/tensorflou.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 01:58:25.000000 tensorflou-1.0/tensorflou.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 02:02:24.011740 tensorflou-2.0/
+-rw-rw-rw-   0        0        0      162 2023-05-29 02:02:24.010756 tensorflou-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-29 02:02:24.011740 tensorflou-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-05-29 02:02:18.000000 tensorflou-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:02:23.999756 tensorflou-2.0/tensorflou/
+-rw-rw-rw-   0        0        0     4089 2023-05-28 17:30:49.000000 tensorflou-2.0/tensorflou/1.txt
+-rw-rw-rw-   0        0        0     4079 2023-05-28 17:33:57.000000 tensorflou-2.0/tensorflou/11.txt
+-rw-rw-rw-   0        0        0     3843 2023-05-29 02:00:09.000000 tensorflou-2.0/tensorflou/12.txt
+-rw-rw-rw-   0        0        0     2790 2023-05-28 17:34:58.000000 tensorflou-2.0/tensorflou/13.txt
+-rw-rw-rw-   0        0        0     4356 2023-05-28 17:35:15.000000 tensorflou-2.0/tensorflou/14.txt
+-rw-rw-rw-   0        0        0      869 2023-05-28 17:35:30.000000 tensorflou-2.0/tensorflou/15.txt
+-rw-rw-rw-   0        0        0     2315 2023-05-28 17:35:41.000000 tensorflou-2.0/tensorflou/16.txt
+-rw-rw-rw-   0        0        0     2954 2023-05-28 17:36:05.000000 tensorflou-2.0/tensorflou/17.txt
+-rw-rw-rw-   0        0        0     5831 2023-05-28 17:36:23.000000 tensorflou-2.0/tensorflou/18.txt
+-rw-rw-rw-   0        0        0     1438 2023-05-28 17:36:41.000000 tensorflou-2.0/tensorflou/19.txt
+-rw-rw-rw-   0        0        0     6452 2023-05-28 17:31:44.000000 tensorflou-2.0/tensorflou/2.txt
+-rw-rw-rw-   0        0        0     2619 2023-05-28 17:36:53.000000 tensorflou-2.0/tensorflou/20.txt
+-rw-rw-rw-   0        0        0     2189 2023-05-28 17:32:00.000000 tensorflou-2.0/tensorflou/3.txt
+-rw-rw-rw-   0        0        0     4135 2023-05-28 17:32:28.000000 tensorflou-2.0/tensorflou/4.txt
+-rw-rw-rw-   0        0        0     2536 2023-05-28 17:32:57.000000 tensorflou-2.0/tensorflou/5.txt
+-rw-rw-rw-   0        0        0      226 2023-05-29 02:02:19.000000 tensorflou-2.0/tensorflou/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:02:24.008740 tensorflou-2.0/tensorflou.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-29 02:02:23.000000 tensorflou-2.0/tensorflou.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-05-29 02:02:23.000000 tensorflou-2.0/tensorflou.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:02:23.000000 tensorflou-2.0/tensorflou.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 02:02:23.000000 tensorflou-2.0/tensorflou.egg-info/top_level.txt
```

### Comparing `tensorflou-1.0/tensorflou/1.txt` & `tensorflou-2.0/tensorflou/1.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/11.txt` & `tensorflou-2.0/tensorflou/11.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/13.txt` & `tensorflou-2.0/tensorflou/13.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/14.txt` & `tensorflou-2.0/tensorflou/14.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/15.txt` & `tensorflou-2.0/tensorflou/15.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/16.txt` & `tensorflou-2.0/tensorflou/16.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/17.txt` & `tensorflou-2.0/tensorflou/17.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/18.txt` & `tensorflou-2.0/tensorflou/18.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/19.txt` & `tensorflou-2.0/tensorflou/19.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/2.txt` & `tensorflou-2.0/tensorflou/2.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/20.txt` & `tensorflou-2.0/tensorflou/20.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/3.txt` & `tensorflou-2.0/tensorflou/3.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/4.txt` & `tensorflou-2.0/tensorflou/4.txt`

 * *Files identical despite different names*

### Comparing `tensorflou-1.0/tensorflou/5.txt` & `tensorflou-2.0/tensorflou/5.txt`

 * *Files identical despite different names*


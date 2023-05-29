# Comparing `tmp/yt-fts-0.1.6.tar.gz` & `tmp/yt-fts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.6.tar", last modified: Mon May 29 06:22:40 2023, max compression
+gzip compressed data, was "yt-fts-0.1.7.tar", last modified: Mon May 29 06:41:17 2023, max compression
```

## Comparing `yt-fts-0.1.6.tar` & `yt-fts-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:22:40.481619 yt-fts-0.1.6/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.6/LICENSE
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:22:40.481039 yt-fts-0.1.6/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.6/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 06:22:40.481779 yt-fts-0.1.6/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 06:22:29.000000 yt-fts-0.1.6/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:22:40.475932 yt-fts-0.1.6/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.6/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.6/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     2873 2023-05-29 05:22:56.000000 yt-fts-0.1.6/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10682 2023-05-29 06:11:35.000000 yt-fts-0.1.6/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:22:40.480011 yt-fts-0.1.6/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      284 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      679 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 06:22:40.000000 yt-fts-0.1.6/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.183439 yt-fts-0.1.7/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.7/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:41:17.182860 yt-fts-0.1.7/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.7/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 06:41:17.183813 yt-fts-0.1.7/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 06:40:23.000000 yt-fts-0.1.7/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.177447 yt-fts-0.1.7/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.7/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.7/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     2873 2023-05-29 05:22:56.000000 yt-fts-0.1.7/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10682 2023-05-29 06:11:35.000000 yt-fts-0.1.7/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.181741 yt-fts-0.1.7/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      284 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      288 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.6/LICENSE` & `yt-fts-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.6/PKG-INFO` & `yt-fts-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.6
+Version: 0.1.7
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yt-fts-0.1.6/README.md` & `yt-fts-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.6/setup.py` & `yt-fts-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'console_scripts': [
         'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.6',
+    version='0.1.7',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
```

### Comparing `yt-fts-0.1.6/yt_fts/db_scripts.py` & `yt-fts-0.1.7/yt_fts/db_scripts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.6/yt_fts/yt_fts.py` & `yt-fts-0.1.7/yt_fts/yt_fts.py`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.6/yt_fts.egg-info/PKG-INFO` & `yt-fts-0.1.7/yt_fts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.6
+Version: 0.1.7
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


# Comparing `tmp/fivbvis-0.1.2.tar.gz` & `tmp/fivbvis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fivbvis-0.1.2.tar", last modified: Sun May 28 06:47:18 2023, max compression
+gzip compressed data, was "fivbvis-0.1.3.tar", last modified: Mon May 29 06:35:09 2023, max compression
```

## Comparing `fivbvis-0.1.2.tar` & `fivbvis-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-28 06:47:18.193414 fivbvis-0.1.2/
--rw-r--r--   0 claromes  (1000) claromes  (1000)    35149 2023-05-28 06:23:07.000000 fivbvis-0.1.2/LICENSE.md
--rw-r--r--   0 claromes  (1000) claromes  (1000)     2636 2023-05-28 06:47:18.193414 fivbvis-0.1.2/PKG-INFO
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1655 2023-05-28 06:26:02.000000 fivbvis-0.1.2/README.md
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-28 06:47:18.183414 fivbvis-0.1.2/fivbvis/
--rw-r--r--   0 claromes  (1000) claromes  (1000)      124 2023-05-28 06:30:16.000000 fivbvis-0.1.2/fivbvis/__init__.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)      418 2023-05-28 06:23:07.000000 fivbvis-0.1.2/fivbvis/article.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)       21 2023-05-28 06:30:12.000000 fivbvis-0.1.2/fivbvis/version.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)      704 2023-05-28 06:23:07.000000 fivbvis-0.1.2/fivbvis/volley_match.py
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-28 06:47:18.183414 fivbvis-0.1.2/fivbvis.egg-info/
--rw-r--r--   0 claromes  (1000) claromes  (1000)     2636 2023-05-28 06:47:18.000000 fivbvis-0.1.2/fivbvis.egg-info/PKG-INFO
--rw-r--r--   0 claromes  (1000) claromes  (1000)      314 2023-05-28 06:47:18.000000 fivbvis-0.1.2/fivbvis.egg-info/SOURCES.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)        1 2023-05-28 06:47:18.000000 fivbvis-0.1.2/fivbvis.egg-info/dependency_links.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)       17 2023-05-28 06:47:18.000000 fivbvis-0.1.2/fivbvis.egg-info/requires.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)        8 2023-05-28 06:47:18.000000 fivbvis-0.1.2/fivbvis.egg-info/top_level.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)       38 2023-05-28 06:47:18.193414 fivbvis-0.1.2/setup.cfg
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1553 2023-05-28 06:30:35.000000 fivbvis-0.1.2/setup.py
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-28 06:47:18.193414 fivbvis-0.1.2/tests/
--rw-r--r--   0 claromes  (1000) claromes  (1000)      656 2023-05-28 06:23:07.000000 fivbvis-0.1.2/tests/test_article.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1731 2023-05-28 06:23:07.000000 fivbvis-0.1.2/tests/test_volley_match.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-29 06:35:09.271959 fivbvis-0.1.3/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)    35149 2023-05-28 06:23:07.000000 fivbvis-0.1.3/LICENSE.md
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     5384 2023-05-29 06:35:09.271959 fivbvis-0.1.3/PKG-INFO
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     4284 2023-05-29 06:31:07.000000 fivbvis-0.1.3/README.md
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-29 06:35:09.261959 fivbvis-0.1.3/fivbvis/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      124 2023-05-28 06:55:00.000000 fivbvis-0.1.3/fivbvis/__init__.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      710 2023-05-29 06:30:43.000000 fivbvis-0.1.3/fivbvis/article.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       21 2023-05-29 06:30:43.000000 fivbvis-0.1.3/fivbvis/version.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      704 2023-05-28 06:23:07.000000 fivbvis-0.1.3/fivbvis/volley_match.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-29 06:35:09.271959 fivbvis-0.1.3/fivbvis.egg-info/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     5384 2023-05-29 06:35:09.000000 fivbvis-0.1.3/fivbvis.egg-info/PKG-INFO
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      314 2023-05-29 06:35:09.000000 fivbvis-0.1.3/fivbvis.egg-info/SOURCES.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)        1 2023-05-29 06:35:09.000000 fivbvis-0.1.3/fivbvis.egg-info/dependency_links.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       17 2023-05-29 06:35:09.000000 fivbvis-0.1.3/fivbvis.egg-info/requires.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)        8 2023-05-29 06:35:09.000000 fivbvis-0.1.3/fivbvis.egg-info/top_level.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       38 2023-05-29 06:35:09.271959 fivbvis-0.1.3/setup.cfg
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1692 2023-05-29 06:31:22.000000 fivbvis-0.1.3/setup.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-05-29 06:35:09.271959 fivbvis-0.1.3/tests/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      656 2023-05-29 04:22:45.000000 fivbvis-0.1.3/tests/test_article.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1731 2023-05-28 06:23:07.000000 fivbvis-0.1.3/tests/test_volley_match.py
```

### Comparing `fivbvis-0.1.2/LICENSE.md` & `fivbvis-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fivbvis-0.1.2/fivbvis/volley_match.py` & `fivbvis-0.1.3/fivbvis/volley_match.py`

 * *Files identical despite different names*

### Comparing `fivbvis-0.1.2/setup.py` & `fivbvis-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,26 @@
     version = re.search(r"^__version__\s*=\s*'(.*)'.*$",
         f.read(), flags=re.MULTILINE).group(1)
 
 setup(
     name='fivbvis',
     version=version,
     author='claromes',
-    license='GPLv3',
     description='FIVB VIS Web Service Python Client',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='api-wrapper fivbvis fivb volleyball beachvolleyball',
     url='https://github.com/claromes/fivbvis',
+    project_urls={
+        'Documentation': 'https://claromes.github.io/fivbvis/',
+        'Issue Tracker': 'https://github.com/claromes/fivbvis/issues',
+    },
     packages=find_packages(exclude=['docs', 'tests*']),
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
```

### Comparing `fivbvis-0.1.2/tests/test_article.py` & `fivbvis-0.1.3/tests/test_article.py`

 * *Files identical despite different names*

### Comparing `fivbvis-0.1.2/tests/test_volley_match.py` & `fivbvis-0.1.3/tests/test_volley_match.py`

 * *Files identical despite different names*


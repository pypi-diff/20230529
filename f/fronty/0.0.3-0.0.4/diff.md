# Comparing `tmp/fronty-0.0.3.tar.gz` & `tmp/fronty-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fronty-0.0.3.tar", last modified: Thu Mar  2 21:10:53 2023, max compression
+gzip compressed data, was "fronty-0.0.4.tar", last modified: Mon May 29 20:07:15 2023, max compression
```

## Comparing `fronty-0.0.3.tar` & `fronty-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.272834 fronty-0.0.3/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4866 2023-03-02 21:10:53.271958 fronty-0.0.3/PKG-INFO
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4069 2023-03-01 18:16:35.000000 fronty-0.0.3/README.md
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.247778 fronty-0.0.3/fronty/
--rwxrwxrwx   0 legend    (1000) legend    (1000)      226 2023-03-02 21:10:25.000000 fronty-0.0.3/fronty/__init__.py
--rwxrwxrwx   0 legend    (1000) legend    (1000)      558 2023-02-28 18:10:59.000000 fronty-0.0.3/fronty/cli.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.265391 fronty-0.0.3/fronty/css/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     3722 2023-03-01 16:43:50.000000 fronty-0.0.3/fronty/css/__init__.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.267720 fronty-0.0.3/fronty/html/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     5341 2023-03-01 17:02:25.000000 fronty-0.0.3/fronty/html/__init__.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.269951 fronty-0.0.3/fronty/middlewares/
--rwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-02-28 17:53:45.000000 fronty-0.0.3/fronty/middlewares/__init__.py
-drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-03-02 21:10:53.262779 fronty-0.0.3/fronty.egg-info/
--rwxrwxrwx   0 legend    (1000) legend    (1000)     4866 2023-03-02 21:10:53.000000 fronty-0.0.3/fronty.egg-info/PKG-INFO
--rwxrwxrwx   0 legend    (1000) legend    (1000)      282 2023-03-02 21:10:53.000000 fronty-0.0.3/fronty.egg-info/SOURCES.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)        1 2023-03-02 21:10:53.000000 fronty-0.0.3/fronty.egg-info/dependency_links.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)       44 2023-03-02 21:10:53.000000 fronty-0.0.3/fronty.egg-info/entry_points.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)        7 2023-03-02 21:10:53.000000 fronty-0.0.3/fronty.egg-info/top_level.txt
--rwxrwxrwx   0 legend    (1000) legend    (1000)       38 2023-03-02 21:10:53.273158 fronty-0.0.3/setup.cfg
--rwxrwxrwx   0 legend    (1000) legend    (1000)     1104 2023-03-02 21:08:43.000000 fronty-0.0.3/setup.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.322857 fronty-0.0.4/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     1065 2023-05-09 14:36:52.000000 fronty-0.0.4/LICENSE
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:07:15.321548 fronty-0.0.4/PKG-INFO
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4069 2023-03-02 21:13:50.000000 fronty-0.0.4/README.md
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.279060 fronty-0.0.4/fronty/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      226 2023-03-02 21:10:25.000000 fronty-0.0.4/fronty/__init__.py
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      558 2023-02-28 18:10:59.000000 fronty-0.0.4/fronty/cli.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.301821 fronty-0.0.4/fronty/css/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     3722 2023-03-01 16:43:50.000000 fronty-0.0.4/fronty/css/__init__.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.311311 fronty-0.0.4/fronty/html/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)    18671 2023-05-29 18:41:45.000000 fronty-0.0.4/fronty/html/__init__.py
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     7361 2023-05-29 18:43:53.000000 fronty-0.0.4/fronty/html/widgets.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.317860 fronty-0.0.4/fronty/middlewares/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-02-28 17:53:45.000000 fronty-0.0.4/fronty/middlewares/__init__.py
+drwxrwxrwx   0 legend    (1000) legend    (1000)        0 2023-05-29 20:07:15.299119 fronty-0.0.4/fronty.egg-info/
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     4847 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/PKG-INFO
+-rwxrwxrwx   0 legend    (1000) legend    (1000)      313 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/SOURCES.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        1 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/dependency_links.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)       43 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/entry_points.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)        7 2023-05-29 20:07:15.000000 fronty-0.0.4/fronty.egg-info/top_level.txt
+-rwxrwxrwx   0 legend    (1000) legend    (1000)       38 2023-05-29 20:07:15.323446 fronty-0.0.4/setup.cfg
+-rwxrwxrwx   0 legend    (1000) legend    (1000)     1100 2023-05-29 20:06:15.000000 fronty-0.0.4/setup.py
```

### Comparing `fronty-0.0.3/PKG-INFO` & `fronty-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fronty
-Version: 0.0.3
+Version: 0.0.4
 Summary: A frontend web framework
 Home-page: https://github.com/Almas-Ali/fronty
 Author: Almas Ali
 Author-email: almaspr3@gmail.com
-License: UNKNOWN
 Keywords: web framework
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Fronty - A frontend web framework
 
 Created by [**@Almas-Ali**](https://github.com/Almas-Ali)
 
 Learn from the official [**`Documentation`**](https://almas-ali.github.io/fronty/)
 
@@ -54,15 +53,15 @@
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/starter%20project/screenshot_1.png "Starter Project Screenshot 1")
 
 [**`Bootstrap Integration`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Bootstrap%20integration)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Bootstrap%20integration/screenshot_1.png "Bootstrap Integration Screenshot 1")
 
-[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20project)
+[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20Project)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_1.png "Custom CSS Project Screenshot 1")
 
 ![Screenshort_2](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_2.png "Custom CSS Project Screenshot 2")
 
 ## How to run the example projects
 
@@ -164,9 +163,7 @@
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/starter%20project/screenshot_1.png "Starter Project Screenshot 1")
 
 ## Contributing
 
 Pull requests are welcome. For any changes, please open an issue first to discuss what you would like to change.
 
 **Thanks for using Fronty!**
-
-
```

### Comparing `fronty-0.0.3/README.md` & `fronty-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/starter%20project/screenshot_1.png "Starter Project Screenshot 1")
 
 [**`Bootstrap Integration`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Bootstrap%20integration)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Bootstrap%20integration/screenshot_1.png "Bootstrap Integration Screenshot 1")
 
-[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20project)
+[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20Project)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_1.png "Custom CSS Project Screenshot 1")
 
 ![Screenshort_2](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_2.png "Custom CSS Project Screenshot 2")
 
 ## How to run the example projects
```

### Comparing `fronty-0.0.3/fronty/cli.py` & `fronty-0.0.4/fronty/cli.py`

 * *Files identical despite different names*

### Comparing `fronty-0.0.3/fronty/css/__init__.py` & `fronty-0.0.4/fronty/css/__init__.py`

 * *Files identical despite different names*

### Comparing `fronty-0.0.3/fronty.egg-info/PKG-INFO` & `fronty-0.0.4/fronty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fronty
-Version: 0.0.3
+Version: 0.0.4
 Summary: A frontend web framework
 Home-page: https://github.com/Almas-Ali/fronty
 Author: Almas Ali
 Author-email: almaspr3@gmail.com
-License: UNKNOWN
 Keywords: web framework
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Fronty - A frontend web framework
 
 Created by [**@Almas-Ali**](https://github.com/Almas-Ali)
 
 Learn from the official [**`Documentation`**](https://almas-ali.github.io/fronty/)
 
@@ -54,15 +53,15 @@
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/starter%20project/screenshot_1.png "Starter Project Screenshot 1")
 
 [**`Bootstrap Integration`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Bootstrap%20integration)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Bootstrap%20integration/screenshot_1.png "Bootstrap Integration Screenshot 1")
 
-[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20project)
+[**`Custom CSS Project`**](https://github.com/Almas-Ali/fronty/tree/master/examples/Custom%20CSS%20Project)
 
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_1.png "Custom CSS Project Screenshot 1")
 
 ![Screenshort_2](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/Custom%20CSS%20Project/screenshot_2.png "Custom CSS Project Screenshot 2")
 
 ## How to run the example projects
 
@@ -164,9 +163,7 @@
 ![Screenshort_1](https://raw.githubusercontent.com/Almas-Ali/fronty/master/examples/starter%20project/screenshot_1.png "Starter Project Screenshot 1")
 
 ## Contributing
 
 Pull requests are welcome. For any changes, please open an issue first to discuss what you would like to change.
 
 **Thanks for using Fronty!**
-
-
```

### Comparing `fronty-0.0.3/setup.py` & `fronty-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='fronty',
-    version='0.0.3',
+    version='0.0.4',
     description='A frontend web framework',
     long_description_content_type='text/markdown',
     long_description=long_description,
     author='Almas Ali',
     author_email='almaspr3@gmail.com',
     url='https://github.com/Almas-Ali/fronty',
     packages=find_packages(),
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.9',
```


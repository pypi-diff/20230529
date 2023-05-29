# Comparing `tmp/rgmining-fraud-eagle-0.9.6.tar.gz` & `tmp/rgmining-fraud-eagle-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rgmining-fraud-eagle-0.9.6.tar", last modified: Wed Jun 21 17:04:20 2017, max compression
+gzip compressed data, was "dist/rgmining-fraud-eagle-0.9.7.tar", last modified: Wed Sep 27 06:45:11 2017, max compression
```

## Comparing `rgmining-fraud-eagle-0.9.6.tar` & `rgmining-fraud-eagle-0.9.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/docs/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/docs/source/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/docs/source/_static/
--rw-r--r--   0 travis    (1000) travis    (1000)    25686 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/docs/source/_static/image.png
--rw-r--r--   0 travis    (1000) travis    (1000)    10750 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/docs/source/conf.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7204 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/docs/source/index.rst
--rw-r--r--   0 travis    (1000) travis    (1000)       15 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/docs/.gitignore
--rw-r--r--   0 travis    (1000) travis    (1000)     8354 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/docs/Makefile
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/
--rw-r--r--   0 travis    (1000) travis    (1000)     1073 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1222 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/constants.py
--rw-r--r--   0 travis    (1000) travis    (1000)    22331 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/graph.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3670 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/likelihood.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3257 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/fraud_eagle/prior.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/misc/
--rw-r--r--   0 travis    (1000) travis    (1000)      357 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/misc/index.html
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     2814 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      743 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       93 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       12 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)      898 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/tests/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    24230 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/tests/graph_test.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1890 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/tests/likelihood_test.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1653 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/tests/prior_test.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1602 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/tests/test_suite.py
--rw-r--r--   0 travis    (1000) travis    (1000)      165 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/.bumpversion.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)      195 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/.codeclimate.yml
--rw-r--r--   0 travis    (1000) travis    (1000)     1150 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/.gitignore
--rw-r--r--   0 travis    (1000) travis    (1000)      120 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/.gitmodules
--rw-r--r--   0 travis    (1000) travis    (1000)      909 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/.travis.yml
--rw-r--r--   0 travis    (1000) travis    (1000)    34500 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/COPYING
--rw-r--r--   0 travis    (1000) travis    (1000)       59 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     1557 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/README.md
--rw-r--r--   0 travis    (1000) travis    (1000)     1793 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)       31 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/requirements.in
--rw-r--r--   0 travis    (1000) travis    (1000)      225 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/requirements.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     2251 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      563 2017-06-21 17:04:06.000000 rgmining-fraud-eagle-0.9.6/wercker.yml
--rw-r--r--   0 travis    (1000) travis    (1000)     2814 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2017-06-21 17:04:20.000000 rgmining-fraud-eagle-0.9.6/setup.cfg
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/docs/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/docs/source/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/docs/source/_static/
+-rw-r--r--   0 travis    (2000) travis    (2000)    25686 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/docs/source/_static/image.png
+-rw-r--r--   0 travis    (2000) travis    (2000)    10750 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/docs/source/conf.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     7213 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/docs/source/index.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)       15 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/docs/.gitignore
+-rw-r--r--   0 travis    (2000) travis    (2000)     8354 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/docs/Makefile
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1073 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1222 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/constants.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    22345 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/graph.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3670 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/likelihood.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3257 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/fraud_eagle/prior.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/misc/
+-rw-r--r--   0 travis    (2000) travis    (2000)      357 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/misc/index.html
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     2914 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      743 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       70 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       12 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/tests/
+-rw-r--r--   0 travis    (2000) travis    (2000)      898 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/tests/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    24230 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/tests/graph_test.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1890 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/tests/likelihood_test.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1653 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/tests/prior_test.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1602 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/tests/test_suite.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      165 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/.bumpversion.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)      195 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/.codeclimate.yml
+-rw-r--r--   0 travis    (2000) travis    (2000)     1150 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/.gitignore
+-rw-r--r--   0 travis    (2000) travis    (2000)      120 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/.gitmodules
+-rw-r--r--   0 travis    (2000) travis    (2000)      909 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/.travis.yml
+-rw-r--r--   0 travis    (2000) travis    (2000)    34500 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/COPYING
+-rw-r--r--   0 travis    (2000) travis    (2000)       59 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/MANIFEST.in
+-rw-r--r--   0 travis    (2000) travis    (2000)     1557 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/README.md
+-rw-r--r--   0 travis    (2000) travis    (2000)     1793 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/README.rst
+-rw-r--r--   0 travis    (2000) travis    (2000)       31 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/requirements.in
+-rw-r--r--   0 travis    (2000) travis    (2000)      225 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/requirements.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     2349 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)      563 2017-09-27 06:44:39.000000 rgmining-fraud-eagle-0.9.7/wercker.yml
+-rw-r--r--   0 travis    (2000) travis    (2000)     2914 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2017-09-27 06:45:11.000000 rgmining-fraud-eagle-0.9.7/setup.cfg
```

### Comparing `rgmining-fraud-eagle-0.9.6/docs/source/_static/image.png` & `rgmining-fraud-eagle-0.9.7/docs/source/_static/image.png`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/docs/source/conf.py` & `rgmining-fraud-eagle-0.9.7/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 author = u'Junpei Kawamoto'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = u'0.9.6'
+release = u'0.9.7'
 # The short X.Y version.
 version = release[:3]
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `rgmining-fraud-eagle-0.9.6/docs/source/index.rst` & `rgmining-fraud-eagle-0.9.7/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
    print("Start iterations.")
    max_iteration = 10000
    for i in range(max_iteration):
 
       # Run one iteration.
       diff = graph.update()
-      print("Iteration %d ends. (diff=%s)", i + 1, diff)
+      print("Iteration {0} ends. (diff={1})".format(i + 1, diff))
 
       if diff < 10**-5: # Set 10^-5 as an acceptable small number.
           break
 
 
 Result
 ^^^^^^^^
```

### Comparing `rgmining-fraud-eagle-0.9.6/docs/Makefile` & `rgmining-fraud-eagle-0.9.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/fraud_eagle/__init__.py` & `rgmining-fraud-eagle-0.9.7/fraud_eagle/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/fraud_eagle/constants.py` & `rgmining-fraud-eagle-0.9.7/fraud_eagle/constants.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/fraud_eagle/graph.py` & `rgmining-fraud-eagle-0.9.7/fraud_eagle/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 
         Raises:
           ValueError: if the given product isn't an instance of Product.
         """
         if not isinstance(product, Product):
             raise ValueError(
                 "Given product isn't an instance of Product:", product)
-        return self.graph.predecessors(product)
+        return list(self.graph.predecessors(product))
 
     @memoized
     def retrieve_products(self, reviewer):
         """Retrieve products a given reviewer reviews.
 
         Args:
           reviewer: Reviewer.
@@ -365,15 +365,15 @@
 
         Raises:
           ValueError: if the given reviewer isn't an instance of Reviewer.
         """
         if not isinstance(reviewer, Reviewer):
             raise ValueError(
                 "Given reviewer isn't an instance of Reviewer:", reviewer)
-        return self.graph.successors(reviewer)
+        return list(self.graph.successors(reviewer))
 
     @memoized
     def retrieve_review(self, reviewer, product):
         """Retrieve a review a given reviewer posts to a given product.
 
         Args:
           reviewer: Reviewer,
@@ -477,15 +477,15 @@
                         np.exp(review.product_to_user(ulabel)) - np.exp(updated)))
                     review.update_product_to_user(ulabel, updated)
 
         histo, edges = np.histogram(diffs)
         LOGGER.info(
             "Differentials:\n" + "\n".join(
                 "  {0}-{1}: {2}".format(
-                    edges[i], edges[i+1], v) for i, v in enumerate(histo)))
+                    edges[i], edges[i + 1], v) for i, v in enumerate(histo)))
 
         return max(diffs)
 
     def _update_user_to_product(self, reviewer, product, plabel):
         """Compute an updated message from a user to a product with a product label.
 
         The updated message is defined as
```

### Comparing `rgmining-fraud-eagle-0.9.6/fraud_eagle/likelihood.py` & `rgmining-fraud-eagle-0.9.7/fraud_eagle/likelihood.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/fraud_eagle/prior.py` & `rgmining-fraud-eagle-0.9.7/fraud_eagle/prior.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/PKG-INFO` & `rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rgmining-fraud-eagle
-Version: 0.9.6
+Version: 0.9.7
 Summary: An implementation of Fraud Eagle algorithm
 Home-page: https://github.com/rgmining/frad-eagle
 Author: Junpei Kawamoto
 Author-email: kawamoto.junpei@gmail.com
 License: GPLv3
 Description: Fraud Eagle Algorithm
         =====================
@@ -42,22 +42,24 @@
            :target: https://www.gnu.org/copyleft/gpl.html
         .. |Build Status| image:: https://travis-ci.org/rgmining/fraud-eagle.svg?branch=master
            :target: https://travis-ci.org/rgmining/fraud-eagle
         .. |wercker status| image:: https://app.wercker.com/status/fb1061f0043991bf7609a198a96acbaf/s/master
            :target: https://app.wercker.com/project/byKey/fb1061f0043991bf7609a198a96acbaf
         .. |Code Climate| image:: https://codeclimate.com/github/rgmining/fraud-eagle/badges/gpa.svg
            :target: https://codeclimate.com/github/rgmining/fraud-eagle
-        .. |Release| image:: https://img.shields.io/badge/release-0.9.6-brightgreen.svg
-           :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.6
+        .. |Release| image:: https://img.shields.io/badge/release-0.9.7-brightgreen.svg
+           :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.7
         .. |Japanese| image:: https://img.shields.io/badge/qiita-%E6%97%A5%E6%9C%AC%E8%AA%9E-brightgreen.svg
            :target: http://qiita.com/jkawamoto/items/d2284316cc37cd810bfd
         .. |Logo| image:: https://rgmining.github.io/fraud-eagle/_static/image.png
            :target: https://rgmining.github.io/fraud-eagle/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `rgmining-fraud-eagle-0.9.6/rgmining_fraud_eagle.egg-info/SOURCES.txt` & `rgmining-fraud-eagle-0.9.7/rgmining_fraud_eagle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/tests/__init__.py` & `rgmining-fraud-eagle-0.9.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/tests/graph_test.py` & `rgmining-fraud-eagle-0.9.7/tests/graph_test.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/tests/likelihood_test.py` & `rgmining-fraud-eagle-0.9.7/tests/likelihood_test.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/tests/prior_test.py` & `rgmining-fraud-eagle-0.9.7/tests/prior_test.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/tests/test_suite.py` & `rgmining-fraud-eagle-0.9.7/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/.gitignore` & `rgmining-fraud-eagle-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/.travis.yml` & `rgmining-fraud-eagle-0.9.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/COPYING` & `rgmining-fraud-eagle-0.9.7/COPYING`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/README.md` & `rgmining-fraud-eagle-0.9.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Fraud Eagle Algorithm
 [![GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/copyleft/gpl.html)
 [![Build Status](https://travis-ci.org/rgmining/fraud-eagle.svg?branch=master)](https://travis-ci.org/rgmining/fraud-eagle)
 [![wercker status](https://app.wercker.com/status/fb1061f0043991bf7609a198a96acbaf/s/master "wercker status")](https://app.wercker.com/project/byKey/fb1061f0043991bf7609a198a96acbaf)
 [![Code Climate](https://codeclimate.com/github/rgmining/fraud-eagle/badges/gpa.svg)](https://codeclimate.com/github/rgmining/fraud-eagle)
-[![Release](https://img.shields.io/badge/release-0.9.6-brightgreen.svg)](https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.6)
+[![Release](https://img.shields.io/badge/release-0.9.7-brightgreen.svg)](https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.7)
 [![Japanese](https://img.shields.io/badge/qiita-%E6%97%A5%E6%9C%AC%E8%AA%9E-brightgreen.svg)](http://qiita.com/jkawamoto/items/d2284316cc37cd810bfd)
 
 [![Logo](https://rgmining.github.io/fraud-eagle/_static/image.png)](https://rgmining.github.io/fraud-eagle/)
 
 This package provides an implementation of Fraud Eagle algorithm.
 This algorithm has been introduced by Leman Akoglu, *et al.* in
 [ICWSM 2013](https://www.aaai.org/ocs/index.php/ICWSM/ICWSM13/paper/viewFile/5981/6338)
```

### Comparing `rgmining-fraud-eagle-0.9.6/README.rst` & `rgmining-fraud-eagle-0.9.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -34,13 +34,13 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://travis-ci.org/rgmining/fraud-eagle.svg?branch=master
    :target: https://travis-ci.org/rgmining/fraud-eagle
 .. |wercker status| image:: https://app.wercker.com/status/fb1061f0043991bf7609a198a96acbaf/s/master
    :target: https://app.wercker.com/project/byKey/fb1061f0043991bf7609a198a96acbaf
 .. |Code Climate| image:: https://codeclimate.com/github/rgmining/fraud-eagle/badges/gpa.svg
    :target: https://codeclimate.com/github/rgmining/fraud-eagle
-.. |Release| image:: https://img.shields.io/badge/release-0.9.6-brightgreen.svg
-   :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.6
+.. |Release| image:: https://img.shields.io/badge/release-0.9.7-brightgreen.svg
+   :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.7
 .. |Japanese| image:: https://img.shields.io/badge/qiita-%E6%97%A5%E6%9C%AC%E8%AA%9E-brightgreen.svg
    :target: http://qiita.com/jkawamoto/items/d2284316cc37cd810bfd
 .. |Logo| image:: https://rgmining.github.io/fraud-eagle/_static/image.png
    :target: https://rgmining.github.io/fraud-eagle/
```

### Comparing `rgmining-fraud-eagle-0.9.6/setup.py` & `rgmining-fraud-eagle-0.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,11 +61,13 @@
     license="GPLv3",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.6",
         "Topic :: Software Development :: Libraries",
         "Topic :: Scientific/Engineering :: Information Analysis"
     ]
 )
```

### Comparing `rgmining-fraud-eagle-0.9.6/wercker.yml` & `rgmining-fraud-eagle-0.9.7/wercker.yml`

 * *Files identical despite different names*

### Comparing `rgmining-fraud-eagle-0.9.6/PKG-INFO` & `rgmining-fraud-eagle-0.9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rgmining-fraud-eagle
-Version: 0.9.6
+Version: 0.9.7
 Summary: An implementation of Fraud Eagle algorithm
 Home-page: https://github.com/rgmining/frad-eagle
 Author: Junpei Kawamoto
 Author-email: kawamoto.junpei@gmail.com
 License: GPLv3
 Description: Fraud Eagle Algorithm
         =====================
@@ -42,22 +42,24 @@
            :target: https://www.gnu.org/copyleft/gpl.html
         .. |Build Status| image:: https://travis-ci.org/rgmining/fraud-eagle.svg?branch=master
            :target: https://travis-ci.org/rgmining/fraud-eagle
         .. |wercker status| image:: https://app.wercker.com/status/fb1061f0043991bf7609a198a96acbaf/s/master
            :target: https://app.wercker.com/project/byKey/fb1061f0043991bf7609a198a96acbaf
         .. |Code Climate| image:: https://codeclimate.com/github/rgmining/fraud-eagle/badges/gpa.svg
            :target: https://codeclimate.com/github/rgmining/fraud-eagle
-        .. |Release| image:: https://img.shields.io/badge/release-0.9.6-brightgreen.svg
-           :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.6
+        .. |Release| image:: https://img.shields.io/badge/release-0.9.7-brightgreen.svg
+           :target: https://github.com/rgmining/fraud-eagle/releases/tag/v0.9.7
         .. |Japanese| image:: https://img.shields.io/badge/qiita-%E6%97%A5%E6%9C%AC%E8%AA%9E-brightgreen.svg
            :target: http://qiita.com/jkawamoto/items/d2284316cc37cd810bfd
         .. |Logo| image:: https://rgmining.github.io/fraud-eagle/_static/image.png
            :target: https://rgmining.github.io/fraud-eagle/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```


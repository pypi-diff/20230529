# Comparing `tmp/django_jsform-5.0.0.tar.gz` & `tmp/django_jsform-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_jsform-5.0.0.tar", last modified: Thu Jun  2 19:11:52 2022, max compression
+gzip compressed data, was "dist/django_jsform-5.1.0.tar", last modified: Mon May 29 16:58:20 2023, max compression
```

## Comparing `django_jsform-5.0.0.tar` & `django_jsform-5.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:52.000000 django_jsform-5.0.0/
--rw-r--r--   0 alex       (502) staff       (20)     1522 2022-06-02 19:11:52.000000 django_jsform-5.0.0/PKG-INFO
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/templatetags/
--rw-r--r--   0 alex       (502) staff       (20)     6148 2020-06-29 15:39:01.000000 django_jsform-5.0.0/django_jsform/templatetags/.DS_Store
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:52.000000 django_jsform-5.0.0/django_jsform/templatetags/__pycache__/
--rw-r--r--   0 alex       (502) staff       (20)     3102 2022-01-20 16:19:51.000000 django_jsform-5.0.0/django_jsform/templatetags/__pycache__/jsform.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     3057 2022-01-20 16:19:50.000000 django_jsform-5.0.0/django_jsform/templatetags/jsform.py
--rw-r--r--   0 alex       (502) staff       (20)     6148 2020-05-25 20:16:10.000000 django_jsform-5.0.0/django_jsform/.DS_Store
--rw-r--r--   0 alex       (502) staff       (20)     4959 2021-01-27 15:58:24.000000 django_jsform-5.0.0/django_jsform/js_response.py
--rw-r--r--   0 alex       (502) staff       (20)        0 2020-05-26 15:03:30.000000 django_jsform-5.0.0/django_jsform/__init__.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/__pycache__/
--rw-r--r--   0 alex       (502) staff       (20)     5798 2021-01-27 15:58:24.000000 django_jsform-5.0.0/django_jsform/__pycache__/js_response.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      156 2020-05-27 21:52:32.000000 django_jsform-5.0.0/django_jsform/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      160 2021-08-03 19:25:59.000000 django_jsform-5.0.0/django_jsform/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/static/
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/static/jsform/
--rw-r--r--   0 alex       (502) staff       (20)     1259 2020-11-16 15:52:57.000000 django_jsform-5.0.0/django_jsform/static/jsform/jsform_execresponse.js
--rw-r--r--   0 alex       (502) staff       (20)     9265 2021-04-16 14:55:10.000000 django_jsform-5.0.0/django_jsform/static/jsform/jsform_elementmerge.js
--rw-r--r--   0 alex       (502) staff       (20)     1073 2020-05-21 20:29:15.000000 django_jsform-5.0.0/django_jsform/static/jsform/LICENSE
--rw-r--r--   0 alex       (502) staff       (20)     1516 2020-05-25 20:59:29.000000 django_jsform-5.0.0/django_jsform/static/jsform/jsform_focus_error_element.js
--rw-r--r--   0 alex       (502) staff       (20)    12439 2022-06-02 18:52:33.000000 django_jsform-5.0.0/django_jsform/static/jsform/README.md
--rw-r--r--   0 alex       (502) staff       (20)    11197 2022-06-02 19:01:06.000000 django_jsform-5.0.0/django_jsform/static/jsform/jsform.js
--rw-r--r--   0 alex       (502) staff       (20)       58 2020-05-21 20:29:15.000000 django_jsform-5.0.0/django_jsform/static/jsform/.git
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/static/django_jsform/
--rw-r--r--   0 alex       (502) staff       (20)     1648 2020-10-16 17:08:53.000000 django_jsform-5.0.0/django_jsform/static/django_jsform/django_jsform.css
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/templates/
--rw-r--r--   0 alex       (502) staff       (20)     6148 2020-05-25 20:16:17.000000 django_jsform-5.0.0/django_jsform/templates/.DS_Store
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/
--rw-r--r--   0 alex       (502) staff       (20)      353 2020-08-21 15:53:52.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/standard_field.html
--rw-r--r--   0 alex       (502) staff       (20)      474 2020-08-21 15:57:38.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/form_fields.html
--rw-r--r--   0 alex       (502) staff       (20)      370 2020-10-05 17:44:31.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/inline_field.html
--rw-r--r--   0 alex       (502) staff       (20)      475 2020-08-21 15:51:28.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/checkbox_field.html
--rw-r--r--   0 alex       (502) staff       (20)      572 2021-01-27 15:52:42.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/complete_form.html
--rw-r--r--   0 alex       (502) staff       (20)      464 2020-05-25 20:36:29.000000 django_jsform-5.0.0/django_jsform/templates/django_jsform/form_test.html
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)     1522 2021-08-03 19:25:14.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)        0 2021-08-03 19:25:14.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)       17 2021-08-03 19:25:14.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/requires.txt
--rw-r--r--   0 alex       (502) staff       (20)       14 2021-08-03 19:25:14.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/top_level.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2021-08-03 19:25:14.000000 django_jsform-5.0.0/django_jsform/django_jsform.egg-info/dependency_links.txt
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform/js_helpers/
--rw-r--r--   0 alex       (502) staff       (20)      728 2020-05-25 19:43:03.000000 django_jsform-5.0.0/django_jsform/js_helpers/clear_form_errors.js
--rw-r--r--   0 alex       (502) staff       (20)     1636 2021-01-27 15:36:03.000000 django_jsform-5.0.0/django_jsform/js_helpers/focus_form_errors.js
--rw-r--r--   0 alex       (502) staff       (20)     1526 2020-05-25 20:58:59.000000 django_jsform-5.0.0/django_jsform/js_helpers/set_form_errors.js
--rw-r--r--   0 alex       (502) staff       (20)      276 2021-08-03 19:28:04.000000 django_jsform-5.0.0/MANIFEST.in
--rw-r--r--   0 alex       (502) staff       (20)      901 2020-05-28 20:42:36.000000 django_jsform-5.0.0/README.md
--rw-r--r--   0 alex       (502) staff       (20)      781 2021-08-03 19:28:58.000000 django_jsform-5.0.0/setup.py
--rw-r--r--   0 alex       (502) staff       (20)        5 2022-06-02 19:08:29.000000 django_jsform-5.0.0/VERSION
--rw-r--r--   0 alex       (502) staff       (20)     4634 2022-06-02 19:11:35.000000 django_jsform-5.0.0/RELEASE_NOTES.md
--rw-r--r--   0 alex       (502) staff       (20)       38 2022-06-02 19:11:52.000000 django_jsform-5.0.0/setup.cfg
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)     1522 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)     1725 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)       17 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/requires.txt
--rw-r--r--   0 alex       (502) staff       (20)       14 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/top_level.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2022-06-02 19:11:51.000000 django_jsform-5.0.0/django_jsform.egg-info/dependency_links.txt
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/
+-rw-r--r--   0 alex       (502) staff       (20)     1522 2023-05-29 16:58:20.000000 django_jsform-5.1.0/PKG-INFO
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/templatetags/
+-rw-r--r--   0 alex       (502) staff       (20)     6148 2020-06-29 15:39:01.000000 django_jsform-5.1.0/django_jsform/templatetags/.DS_Store
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/templatetags/__pycache__/
+-rw-r--r--   0 alex       (502) staff       (20)     3102 2022-01-20 16:19:51.000000 django_jsform-5.1.0/django_jsform/templatetags/__pycache__/jsform.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     3057 2022-01-20 16:19:50.000000 django_jsform-5.1.0/django_jsform/templatetags/jsform.py
+-rw-r--r--   0 alex       (502) staff       (20)     6148 2020-05-25 20:16:10.000000 django_jsform-5.1.0/django_jsform/.DS_Store
+-rw-r--r--   0 alex       (502) staff       (20)     4959 2021-01-27 15:58:24.000000 django_jsform-5.1.0/django_jsform/js_response.py
+-rw-r--r--   0 alex       (502) staff       (20)        0 2020-05-26 15:03:30.000000 django_jsform-5.1.0/django_jsform/__init__.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/__pycache__/
+-rw-r--r--   0 alex       (502) staff       (20)     5798 2021-01-27 15:58:24.000000 django_jsform-5.1.0/django_jsform/__pycache__/js_response.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      156 2020-05-27 21:52:32.000000 django_jsform-5.1.0/django_jsform/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      160 2021-08-03 19:25:59.000000 django_jsform-5.1.0/django_jsform/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/static/
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/static/jsform/
+-rw-r--r--   0 alex       (502) staff       (20)     1259 2020-11-16 15:52:57.000000 django_jsform-5.1.0/django_jsform/static/jsform/jsform_execresponse.js
+-rw-r--r--   0 alex       (502) staff       (20)     9265 2021-04-16 14:55:10.000000 django_jsform-5.1.0/django_jsform/static/jsform/jsform_elementmerge.js
+-rw-r--r--   0 alex       (502) staff       (20)     1073 2020-05-21 20:29:15.000000 django_jsform-5.1.0/django_jsform/static/jsform/LICENSE
+-rw-r--r--   0 alex       (502) staff       (20)     1516 2020-05-25 20:59:29.000000 django_jsform-5.1.0/django_jsform/static/jsform/jsform_focus_error_element.js
+-rw-r--r--   0 alex       (502) staff       (20)    12751 2023-05-29 16:55:51.000000 django_jsform-5.1.0/django_jsform/static/jsform/README.md
+-rw-r--r--   0 alex       (502) staff       (20)    11643 2023-05-29 16:51:05.000000 django_jsform-5.1.0/django_jsform/static/jsform/jsform.js
+-rw-r--r--   0 alex       (502) staff       (20)       58 2020-05-21 20:29:15.000000 django_jsform-5.1.0/django_jsform/static/jsform/.git
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/static/django_jsform/
+-rw-r--r--   0 alex       (502) staff       (20)     1648 2020-10-16 17:08:53.000000 django_jsform-5.1.0/django_jsform/static/django_jsform/django_jsform.css
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/templates/
+-rw-r--r--   0 alex       (502) staff       (20)     6148 2020-05-25 20:16:17.000000 django_jsform-5.1.0/django_jsform/templates/.DS_Store
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/
+-rw-r--r--   0 alex       (502) staff       (20)      353 2020-08-21 15:53:52.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/standard_field.html
+-rw-r--r--   0 alex       (502) staff       (20)      474 2020-08-21 15:57:38.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/form_fields.html
+-rw-r--r--   0 alex       (502) staff       (20)      370 2020-10-05 17:44:31.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/inline_field.html
+-rw-r--r--   0 alex       (502) staff       (20)      475 2020-08-21 15:51:28.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/checkbox_field.html
+-rw-r--r--   0 alex       (502) staff       (20)      572 2021-01-27 15:52:42.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/complete_form.html
+-rw-r--r--   0 alex       (502) staff       (20)      464 2020-05-25 20:36:29.000000 django_jsform-5.1.0/django_jsform/templates/django_jsform/form_test.html
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)     1522 2021-08-03 19:25:14.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)        0 2021-08-03 19:25:14.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)       17 2021-08-03 19:25:14.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/requires.txt
+-rw-r--r--   0 alex       (502) staff       (20)       14 2021-08-03 19:25:14.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/top_level.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2021-08-03 19:25:14.000000 django_jsform-5.1.0/django_jsform/django_jsform.egg-info/dependency_links.txt
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform/js_helpers/
+-rw-r--r--   0 alex       (502) staff       (20)      728 2020-05-25 19:43:03.000000 django_jsform-5.1.0/django_jsform/js_helpers/clear_form_errors.js
+-rw-r--r--   0 alex       (502) staff       (20)     1636 2021-01-27 15:36:03.000000 django_jsform-5.1.0/django_jsform/js_helpers/focus_form_errors.js
+-rw-r--r--   0 alex       (502) staff       (20)     1526 2020-05-25 20:58:59.000000 django_jsform-5.1.0/django_jsform/js_helpers/set_form_errors.js
+-rw-r--r--   0 alex       (502) staff       (20)      276 2021-08-03 19:28:04.000000 django_jsform-5.1.0/MANIFEST.in
+-rw-r--r--   0 alex       (502) staff       (20)      901 2020-05-28 20:42:36.000000 django_jsform-5.1.0/README.md
+-rw-r--r--   0 alex       (502) staff       (20)      781 2021-08-03 19:28:58.000000 django_jsform-5.1.0/setup.py
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-29 16:57:27.000000 django_jsform-5.1.0/VERSION
+-rw-r--r--   0 alex       (502) staff       (20)     4695 2023-05-29 16:57:57.000000 django_jsform-5.1.0/RELEASE_NOTES.md
+-rw-r--r--   0 alex       (502) staff       (20)       38 2023-05-29 16:58:20.000000 django_jsform-5.1.0/setup.cfg
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)     1522 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)     1725 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)       17 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/requires.txt
+-rw-r--r--   0 alex       (502) staff       (20)       14 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/top_level.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2023-05-29 16:58:20.000000 django_jsform-5.1.0/django_jsform.egg-info/dependency_links.txt
```

### Comparing `django_jsform-5.0.0/PKG-INFO` & `django_jsform-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_jsform
-Version: 5.0.0
+Version: 5.1.0
 Summary: Django integration for jsform
 Home-page: https://github.com/quadrant-newmedia/django_jsform
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # django_jsform
         Django integration for [jsform](https://github.com/quadrant-newmedia/jsform). In a nutshell, this package:
```

### Comparing `django_jsform-5.0.0/django_jsform/templatetags/.DS_Store` & `django_jsform-5.1.0/django_jsform/templatetags/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/templatetags/__pycache__/jsform.cpython-36.pyc` & `django_jsform-5.1.0/django_jsform/templatetags/__pycache__/jsform.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/templatetags/jsform.py` & `django_jsform-5.1.0/django_jsform/templatetags/jsform.py`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/.DS_Store` & `django_jsform-5.1.0/django_jsform/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/js_response.py` & `django_jsform-5.1.0/django_jsform/js_response.py`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/__pycache__/js_response.cpython-36.pyc` & `django_jsform-5.1.0/django_jsform/__pycache__/js_response.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/jsform_execresponse.js` & `django_jsform-5.1.0/django_jsform/static/jsform/jsform_execresponse.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/jsform_elementmerge.js` & `django_jsform-5.1.0/django_jsform/static/jsform/jsform_elementmerge.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/LICENSE` & `django_jsform-5.1.0/django_jsform/static/jsform/LICENSE`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/jsform_focus_error_element.js` & `django_jsform-5.1.0/django_jsform/static/jsform/jsform_focus_error_element.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/README.md` & `django_jsform-5.1.0/django_jsform/static/jsform/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 
 When a form is submitted, we add a `block-submissions` attribute to the form. Whenever this attribute is present, we will not allow further submissions. You _may_ want to use this attribute as a selector to style the form differently, or to block user input via javascript.
 
 This attribute is set at the very beiggning of the submission process, before any of our events are fired. You may remove this attribute in any of your event listeners if you wish to allow further submissions.
 
 Our default `jsformsuccess` and `jsformnetworkerror` actions will unblock the form _if and only if_ the submission method is GET. Our default `jsformerror` action will always unblock the form. In this case, we're assuming your server has not processed the data, and it's safe to retry submitting (this is especially helpful during development). If you want different handling of any of these events, be sure to handle them and call `event.preventDefault()`.
 
+### Alternate Behaviour - Submission Replacing
+If you add the "replace-overlapping-requests" attribute to your form, we will _not_ add the `block-submissions` attribute. Instead, each submission will cause the previous submission request (if still pending) to abort. This is useful bevhaviour for filter forms.
+
 ## Intended Usage
 
 You _could_ manually add event listeners to each form you create, writing custom javascript to handle each response. 
 
 Where jsform really shines, though, is when you create a framework with global event listeners, for handling common patterns. `jsform.js` includes one built-in event listener, and we also supply some opt-in listeners in separate scripts.
 
 ### `replace-query`
```

### Comparing `django_jsform-5.0.0/django_jsform/static/jsform/jsform.js` & `django_jsform-5.1.0/django_jsform/static/jsform/jsform.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -88,23 +88,32 @@
     }
 
     function unblock(form) {
         form.removeAttribute('block-submissions');
     }
 
     function jsform_submit(form) {
-        /*
-            By default, we don't allow duplicate form submissions.
+        if (form.hasAttribute('replace-overlapping-requests')) {
+            /*
+                In this mode, we do allow duplicate (even overlapping) requests, but we abort any pending requests (so their responses will be ignored).
+
+                This is useful for filter forms.
+            */
+            if (form._most_recent_jsform_xhr) form._most_recent_jsform_xhr.abort()
+        } else {
+            /*
+                By default, we don't allow duplicate form submissions.
 
-            If the end-user should be able to re-submit the same form, it's up to you to remove this attribute.
+                If the end-user should be able to re-submit the same form, it's up to you to remove this attribute.
 
-            You may remove the attribute in an event listener listening to any of our events (jsformsubmitted, jsformerror, or jsformsuccess).
-        */
-        if (form.hasAttribute('block-submissions')) return
-        form.setAttribute('block-submissions', '')
+                You may remove the attribute in an event listener listening to any of our events (jsformsubmitted, jsformerror, or jsformsuccess).
+            */
+            if (form.hasAttribute('block-submissions')) return
+            form.setAttribute('block-submissions', '')
+        }
 
         /*
             Form elements (inputs) can mask standard form properties,
             so we cannot safely access form.action, form.method, etc.
             
             Also, the js properties are more convenient that html attributes, since they do things like resolve the action url for us.
 
@@ -171,14 +180,15 @@
         }
         form_clone.dispatchEvent.call(form, (new CustomEvent('jsformsubmitted', {
             bubbles: true,
             detail: jsform_data
         })));
 
         var r = new XMLHttpRequest();
+        form._most_recent_jsform_xhr = r;
         r.open(method, get_url());
         r.onerror = function(event) {
             var e = new CustomEvent('jsformnetworkerror', {
                 bubbles: true,
                 cancelable: true
             });
             form_clone.dispatchEvent.call(form, (e));
```

### Comparing `django_jsform-5.0.0/django_jsform/static/django_jsform/django_jsform.css` & `django_jsform-5.1.0/django_jsform/static/django_jsform/django_jsform.css`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/templates/.DS_Store` & `django_jsform-5.1.0/django_jsform/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/templates/django_jsform/complete_form.html` & `django_jsform-5.1.0/django_jsform/templates/django_jsform/complete_form.html`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/django_jsform.egg-info/PKG-INFO` & `django_jsform-5.1.0/django_jsform/django_jsform.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/js_helpers/clear_form_errors.js` & `django_jsform-5.1.0/django_jsform/js_helpers/clear_form_errors.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/js_helpers/focus_form_errors.js` & `django_jsform-5.1.0/django_jsform/js_helpers/focus_form_errors.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/django_jsform/js_helpers/set_form_errors.js` & `django_jsform-5.1.0/django_jsform/js_helpers/set_form_errors.js`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/README.md` & `django_jsform-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/setup.py` & `django_jsform-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django_jsform-5.0.0/RELEASE_NOTES.md` & `django_jsform-5.1.0/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 5.1.0
+Add replace-overlapping-requests option to jsform.
+
 # 5.0.0
 Ensure that non-GET forms are never empty (send a "__hack_ensure_body_not_empty__" key, with no value).
 This is to work-around browsers/firewalls/proxies that have issues with empty multipart/form-data POST requests.
 
 For most projects, this will be backward compatible with v4. 
 It's only an issue if your code has an issue with this extra value
 (ie. it checks for an "empty" data set, or does something with all keys in the data set).
```

### Comparing `django_jsform-5.0.0/django_jsform.egg-info/PKG-INFO` & `django_jsform-5.1.0/django_jsform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jsform
-Version: 5.0.0
+Version: 5.1.0
 Summary: Django integration for jsform
 Home-page: https://github.com/quadrant-newmedia/django_jsform
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # django_jsform
         Django integration for [jsform](https://github.com/quadrant-newmedia/jsform). In a nutshell, this package:
```

### Comparing `django_jsform-5.0.0/django_jsform.egg-info/SOURCES.txt` & `django_jsform-5.1.0/django_jsform.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/pretix-computop-1.1.0.tar.gz` & `tmp/pretix-computop-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-computop-1.1.0.tar", last modified: Mon Jan 30 13:31:27 2023, max compression
+gzip compressed data, was "pretix-computop-1.1.1.tar", last modified: Sun May 28 23:06:24 2023, max compression
```

## Comparing `pretix-computop-1.1.0.tar` & `pretix-computop-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.755317 pretix-computop-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1835 2023-01-30 13:31:27.755317 pretix-computop-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.747316 pretix-computop-1.1.0/pretix_computop/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.743317 pretix-computop-1.1.0/pretix_computop/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.743317 pretix-computop-1.1.0/pretix_computop/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.747316 pretix-computop-1.1.0/pretix_computop/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.747316 pretix-computop-1.1.0/pretix_computop/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.747316 pretix-computop-1.1.0/pretix_computop/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    17372 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     7775 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.743317 pretix-computop-1.1.0/pretix_computop/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.751317 pretix-computop-1.1.0/pretix_computop/static/pretix_computop/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/static/pretix_computop/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/static/pretix_computop/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.743317 pretix-computop-1.1.0/pretix_computop/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.751317 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/control.html
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/return.html
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_computop/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.747316 pretix-computop-1.1.0/pretix_computop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1835 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1240 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-30 13:31:27.000000 pretix-computop-1.1.0/pretix_computop.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.755317 pretix-computop-1.1.0/pretix_firstcash/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/payment.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.743317 pretix-computop-1.1.0/pretix_firstcash/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:31:27.755317 pretix-computop-1.1.0/pretix_firstcash/static/pretix_firstcash/
--rw-rw-rw-   0 root         (0) root         (0)    21933 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/static/pretix_firstcash/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/pretix_firstcash/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-01-30 13:31:27.755317 pretix-computop-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-01-30 13:26:32.000000 pretix-computop-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.257862 pretix-computop-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-05-28 23:06:24.257862 pretix-computop-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.249862 pretix-computop-1.1.1/pretix_computop/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.249862 pretix-computop-1.1.1/pretix_computop/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:52.000000 pretix-computop-1.1.1/pretix_computop/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    17479 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     7775 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.249862 pretix-computop-1.1.1/pretix_computop/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/static/pretix_computop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:52.000000 pretix-computop-1.1.1/pretix_computop/static/pretix_computop/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/static/pretix_computop/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.249862 pretix-computop-1.1.1/pretix_computop/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:52.000000 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/control.html
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/return.html
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_computop/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_computop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-28 23:06:24.000000 pretix-computop-1.1.1/pretix_computop.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_firstcash/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.249862 pretix-computop-1.1.1/pretix_firstcash/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:24.253862 pretix-computop-1.1.1/pretix_firstcash/static/pretix_firstcash/
+-rw-rw-rw-   0 root         (0) root         (0)    21933 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/static/pretix_firstcash/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pretix_firstcash/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-28 23:06:24.257862 pretix-computop-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:33:53.000000 pretix-computop-1.1.1/setup.py
```

### Comparing `pretix-computop-1.1.0/LICENSE` & `pretix-computop-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/PKG-INFO` & `pretix-computop-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-computop
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use Computop based payment providers
-Home-page: https://github.com/pretix/pretix-computop
-Author: Phin Wolkwitz
-Author-email: wolkwitz@rami.io
-License: Apache
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2022 rami.io GmbH
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+        
+Project-URL: homepage, https://github.com/pretix/pretix-computop
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Computop – First Cash Solution
 ==============================
 
 This is a plugin for `pretix`_. 
 
@@ -21,15 +39,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 This plugin has CI set up to enforce a few code style rules. To check locally, you need these packages installed::
```

### Comparing `pretix-computop-1.1.0/README.rst` & `pretix-computop-1.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 This plugin has CI set up to enforce a few code style rules. To check locally, you need these packages installed::
```

### Comparing `pretix-computop-1.1.0/pretix_computop/apps.py` & `pretix-computop-1.1.1/pretix_computop/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/payment.py` & `pretix-computop-1.1.1/pretix_computop/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,17 @@
             "id": payment.info_data.get("PayID", None),
             "payment_method": payment.info_data.get("pt", None),
         }
 
     def matching_id(self, payment: OrderPayment):
         return payment.info_data.get("PayID", None)
 
+    def refund_matching_id(self, refund: OrderRefund):
+        return refund.info_data.get("PayID", None)
+
     def payment_control_render(
         self, request: HttpRequest, payment: OrderPayment
     ) -> str:
         template = get_template("pretix_computop/control.html")
         ctx = {
             "request": request,
             "event": self.event,
```

### Comparing `pretix-computop-1.1.0/pretix_computop/paymentmethods.py` & `pretix-computop-1.1.1/pretix_computop/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/signals.py` & `pretix-computop-1.1.1/pretix_computop/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/static/pretix_computop/logo.svg` & `pretix-computop-1.1.1/pretix_computop/static/pretix_computop/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/templates/pretix_computop/control.html` & `pretix-computop-1.1.1/pretix_computop/templates/pretix_computop/control.html`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/urls.py` & `pretix-computop-1.1.1/pretix_computop/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop/views.py` & `pretix-computop-1.1.1/pretix_computop/views.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_computop.egg-info/PKG-INFO` & `pretix-computop-1.1.1/pretix_computop.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-computop
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use Computop based payment providers
-Home-page: https://github.com/pretix/pretix-computop
-Author: Phin Wolkwitz
-Author-email: wolkwitz@rami.io
-License: Apache
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2022 rami.io GmbH
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+        
+Project-URL: homepage, https://github.com/pretix/pretix-computop
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Computop – First Cash Solution
 ==============================
 
 This is a plugin for `pretix`_. 
 
@@ -21,15 +39,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 This plugin has CI set up to enforce a few code style rules. To check locally, you need these packages installed::
```

### Comparing `pretix-computop-1.1.0/pretix_computop.egg-info/SOURCES.txt` & `pretix-computop-1.1.1/pretix_computop.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_computop/__init__.py
 pretix_computop/apps.py
 pretix_computop/payment.py
 pretix_computop/paymentmethods.py
 pretix_computop/signals.py
```

### Comparing `pretix-computop-1.1.0/pretix_firstcash/apps.py` & `pretix-computop-1.1.1/pretix_firstcash/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_firstcash/paymentmethods.py` & `pretix-computop-1.1.1/pretix_firstcash/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/pretix_firstcash/static/pretix_firstcash/logo.svg` & `pretix-computop-1.1.1/pretix_firstcash/static/pretix_firstcash/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-computop-1.1.0/setup.cfg` & `pretix-computop-1.1.1/setup.cfg`

 * *Files identical despite different names*


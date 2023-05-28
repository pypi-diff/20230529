# Comparing `tmp/pretix-closer2event-1.2.0.tar.gz` & `tmp/pretix-closer2event-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-closer2event-1.2.0.tar", last modified: Mon Jan 30 15:03:32 2023, max compression
+gzip compressed data, was "pretix-closer2event-1.2.1.tar", last modified: Sun May 28 23:05:51 2023, max compression
```

## Comparing `pretix-closer2event-1.2.0.tar` & `pretix-closer2event-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1216 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.416550 pretix-closer2event-1.2.0/pretix_closer2event/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.416550 pretix-closer2event-1.2.0/pretix_closer2event/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.412550 pretix-closer2event-1.2.0/pretix_closer2event/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.416550 pretix-closer2event-1.2.0/pretix_closer2event/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.416550 pretix-closer2event-1.2.0/pretix_closer2event/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/pretix_closer2event/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)     4576 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.412550 pretix-closer2event-1.2.0/pretix_closer2event/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/pretix_closer2event/static/pretix_closer2event/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/static/pretix_closer2event/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     5313 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/static/pretix_closer2event/postamble.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.412550 pretix-closer2event-1.2.0/pretix_closer2event/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1444 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/order_info.html
--rw-rw-rw-   0 root         (0) root         (0)     1172 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/settings.html
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/pretix_closer2event/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:32.416550 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1216 2023-01-30 15:03:32.000000 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      921 2023-01-30 15:03:32.000000 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 15:03:32.000000 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-30 15:03:32.000000 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-30 15:03:32.000000 pretix-closer2event-1.2.0/pretix_closer2event.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-01-30 15:03:32.420550 pretix-closer2event-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-01-30 14:57:30.000000 pretix-closer2event-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.561059 pretix-closer2event-1.2.1/pretix_closer2event/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.561059 pretix-closer2event-1.2.1/pretix_closer2event/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.557058 pretix-closer2event-1.2.1/pretix_closer2event/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/pretix_closer2event/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/pretix_closer2event/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:22.000000 pretix-closer2event-1.2.1/pretix_closer2event/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/pretix_closer2event/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.557058 pretix-closer2event-1.2.1/pretix_closer2event/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/pretix_closer2event/static/pretix_closer2event/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:22.000000 pretix-closer2event-1.2.1/pretix_closer2event/static/pretix_closer2event/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/static/pretix_closer2event/postamble.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.557058 pretix-closer2event-1.2.1/pretix_closer2event/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:22.000000 pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/order_info.html
+-rw-rw-rw-   0 root         (0) root         (0)     1172 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/settings.html
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pretix_closer2event/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:51.561059 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-05-28 23:05:51.000000 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-28 23:05:51.000000 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:05:51.000000 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-28 23:05:51.000000 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-28 23:05:51.000000 pretix-closer2event-1.2.1/pretix_closer2event.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-05-28 23:05:51.565059 pretix-closer2event-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:33:32.000000 pretix-closer2event-1.2.1/setup.py
```

### Comparing `pretix-closer2event-1.2.0/LICENSE` & `pretix-closer2event-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/PKG-INFO` & `pretix-closer2event-1.2.1/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-closer2event
-Version: 1.2.0
-Summary: This plugin allows to integrate the closer2event hotel map into your pretix shop
-Home-page: https://github.com/pretix/pretix-closer2event
-Author: Martin Gross
-Author-email: gross@rami.io
-License: Apache Software License
-License-File: LICENSE
-
 closer2event Hotel map
 ======================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-closer2event``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/apps.py` & `pretix-closer2event-1.2.1/pretix_closer2event/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/locale/de/LC_MESSAGES/django.po` & `pretix-closer2event-1.2.1/pretix_closer2event/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-closer2event-1.2.1/pretix_closer2event/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/locale/django.pot` & `pretix-closer2event-1.2.1/pretix_closer2event/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/signals.py` & `pretix-closer2event-1.2.1/pretix_closer2event/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/static/pretix_closer2event/postamble.scss` & `pretix-closer2event-1.2.1/pretix_closer2event/static/pretix_closer2event/postamble.scss`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/order_info.html` & `pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/order_info.html`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/templates/pretix_closer2event/settings.html` & `pretix-closer2event-1.2.1/pretix_closer2event/templates/pretix_closer2event/settings.html`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event/views.py` & `pretix-closer2event-1.2.1/pretix_closer2event/views.py`

 * *Files identical despite different names*

### Comparing `pretix-closer2event-1.2.0/pretix_closer2event.egg-info/SOURCES.txt` & `pretix-closer2event-1.2.1/pretix_closer2event.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_closer2event/__init__.py
 pretix_closer2event/apps.py
 pretix_closer2event/signals.py
 pretix_closer2event/urls.py
 pretix_closer2event/views.py
```

### Comparing `pretix-closer2event-1.2.0/setup.cfg` & `pretix-closer2event-1.2.1/setup.cfg`

 * *Files identical despite different names*


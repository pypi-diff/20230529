# Comparing `tmp/django-forbid-0.0.7.tar.gz` & `tmp/django-forbid-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.0.7.tar", last modified: Tue May 16 18:13:36 2023, max compression
+gzip compressed data, was "django-forbid-0.1.0.tar", last modified: Wed May 24 09:55:59 2023, max compression
```

## Comparing `django-forbid-0.0.7.tar` & `django-forbid-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 18:13:23.000000 django-forbid-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-16 18:13:36.357143 django-forbid-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-16 18:13:23.000000 django-forbid-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 18:13:23.000000 django-forbid-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-16 18:13:36.357143 django-forbid-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 18:13:23.000000 django-forbid-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 18:13:23.000000 django-forbid-0.0.7/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:13:36.357143 django-forbid-0.0.7/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 18:13:36.000000 django-forbid-0.0.7/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 09:55:43.000000 django-forbid-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-24 09:55:59.327195 django-forbid-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-24 09:55:43.000000 django-forbid-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 09:55:43.000000 django-forbid-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-24 09:55:59.327195 django-forbid-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 09:55:43.000000 django-forbid-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.0.7/LICENSE` & `django-forbid-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.7/PKG-INFO` & `django-forbid-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.7
+Version: 0.1.0
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
-Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
+Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
+Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -32,22 +34,22 @@
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
-[![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
+[![Docs](https://github.com/pysnippet/django-forbid/actions/workflows/docs.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/docs.yml)
 
 Django Forbid aims to make website access managed and secure for the maintainers. It provides a middleware to grant or
 deny user access based on device and/or location. It also supports VPN detection for banning users who want to lie about
 their country and geolocation. Also, users can use only the VPN detection feature or disable it.
 
-## Install
+## Installation
 
 ```shell
 python -m pip install django-forbid
 ```
 
 ## Configuration
 
@@ -80,53 +82,37 @@
 All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
 following keys:
 
 - `DEVICES` - list of devices to permit or forbid access to
 - `COUNTRIES` - list of countries to permit or forbid access to
 - `TERRITORIES` - list of territories to permit or forbid access to
 - `OPTIONS` - a dictionary for additional settings
-    - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
-    - `PERIOD` - time in seconds to check for access again, 0 means on each request
     - `VPN` - use VPN detection and forbid access to VPN users
     - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
-        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
-        - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
-        - `FORBIDDEN_KIT` - the URL to redirect to when the user is using a forbidden device
-
-Unlike the `COUNTRIES` and `TERRITORIES`, where the middleware decides whether to permit or forbid access based on the
-given `ACTION` value, the `DEVICES` list accepts device types where the names starting with `!` are forbidden. This is
-done to make it possible to make them all mix together.
-
-```python
-# Forbid access to all devices that have a small screen.
-'DEVICES': ['!car', '!player', '!peripheral', '!camera']
-
-# Allow access to all devices having regular or large screens.
-'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv']
-```
+        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden geolocation
+        - `FORBIDDEN_NET` - the URL to redirect to when the user is using a forbidden network (VPN)
+        - `FORBIDDEN_DEV` - the URL to redirect to when the user is using a forbidden device
 
 The available device types are: `smartphone`, `peripheral` - refers to all hardware components that are attached to a
 computer, `wearable` - common types of wearable technology include smartwatches and smartglasses, `phablet` - a
 smartphone having a larger screen, `console` - PlayStation, Xbox, etc., `display`, `speaker` - Google Assistant, Siri,
 Alexa, etc., `desktop`, `tablet`, `camera`, `player` - iPod, Sony Walkman, Creative Zen, etc., `phone`, `car` - refers
 to a car browser and `tv` - refers to TVs having internet access.
 
 ```python
 DJANGO_FORBID = {
     'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv'],
     'COUNTRIES': ['US', 'GB'],
     'TERRITORIES': ['EU'],
     'OPTIONS': {
-        'ACTION': 'PERMIT',
-        'PERIOD': 300,
         'VPN': True,
         'URL': {
             'FORBIDDEN_LOC': 'forbidden_location',
-            'FORBIDDEN_VPN': 'forbidden_network',
-            'FORBIDDEN_KIT': 'forbidden_device',
+            'FORBIDDEN_NET': 'forbidden_network',
+            'FORBIDDEN_DEV': 'forbidden_device',
         },
     },
 }
 ```
 
 The available country codes in the required ISO 3166 alpha-2 format are
 listed [here](https://www.iban.com/country-codes). And the available continent codes (territories) are: `AF` -
```

### Comparing `django-forbid-0.0.7/README.md` & `django-forbid-0.1.0/src/django_forbid.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,55 @@
+Metadata-Version: 2.1
+Name: django-forbid
+Version: 0.1.0
+Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
+Author: Artyom Vancyan
+Author-email: artyom@pysnippet.org
+License: MIT
+Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
+Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
+Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
+Platform: unix
+Platform: linux
+Platform: osx
+Platform: win32
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.1
+Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
-[![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
+[![Docs](https://github.com/pysnippet/django-forbid/actions/workflows/docs.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/docs.yml)
 
 Django Forbid aims to make website access managed and secure for the maintainers. It provides a middleware to grant or
 deny user access based on device and/or location. It also supports VPN detection for banning users who want to lie about
 their country and geolocation. Also, users can use only the VPN detection feature or disable it.
 
-## Install
+## Installation
 
 ```shell
 python -m pip install django-forbid
 ```
 
 ## Configuration
 
@@ -47,53 +82,37 @@
 All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
 following keys:
 
 - `DEVICES` - list of devices to permit or forbid access to
 - `COUNTRIES` - list of countries to permit or forbid access to
 - `TERRITORIES` - list of territories to permit or forbid access to
 - `OPTIONS` - a dictionary for additional settings
-    - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
-    - `PERIOD` - time in seconds to check for access again, 0 means on each request
     - `VPN` - use VPN detection and forbid access to VPN users
     - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
-        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
-        - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
-        - `FORBIDDEN_KIT` - the URL to redirect to when the user is using a forbidden device
-
-Unlike the `COUNTRIES` and `TERRITORIES`, where the middleware decides whether to permit or forbid access based on the
-given `ACTION` value, the `DEVICES` list accepts device types where the names starting with `!` are forbidden. This is
-done to make it possible to make them all mix together.
-
-```python
-# Forbid access to all devices that have a small screen.
-'DEVICES': ['!car', '!player', '!peripheral', '!camera']
-
-# Allow access to all devices having regular or large screens.
-'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv']
-```
+        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden geolocation
+        - `FORBIDDEN_NET` - the URL to redirect to when the user is using a forbidden network (VPN)
+        - `FORBIDDEN_DEV` - the URL to redirect to when the user is using a forbidden device
 
 The available device types are: `smartphone`, `peripheral` - refers to all hardware components that are attached to a
 computer, `wearable` - common types of wearable technology include smartwatches and smartglasses, `phablet` - a
 smartphone having a larger screen, `console` - PlayStation, Xbox, etc., `display`, `speaker` - Google Assistant, Siri,
 Alexa, etc., `desktop`, `tablet`, `camera`, `player` - iPod, Sony Walkman, Creative Zen, etc., `phone`, `car` - refers
 to a car browser and `tv` - refers to TVs having internet access.
 
 ```python
 DJANGO_FORBID = {
     'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv'],
     'COUNTRIES': ['US', 'GB'],
     'TERRITORIES': ['EU'],
     'OPTIONS': {
-        'ACTION': 'PERMIT',
-        'PERIOD': 300,
         'VPN': True,
         'URL': {
             'FORBIDDEN_LOC': 'forbidden_location',
-            'FORBIDDEN_VPN': 'forbidden_network',
-            'FORBIDDEN_KIT': 'forbidden_device',
+            'FORBIDDEN_NET': 'forbidden_network',
+            'FORBIDDEN_DEV': 'forbidden_device',
         },
     },
 }
 ```
 
 The available country codes in the required ISO 3166 alpha-2 format are
 listed [here](https://www.iban.com/country-codes). And the available continent codes (territories) are: `AF` -
```

### Comparing `django-forbid-0.0.7/setup.cfg` & `django-forbid-0.1.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 name = django-forbid
 version = attr: django_forbid.__version__
 author = Artyom Vancyan
 author_email = artyom@pysnippet.org
 description = Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/pysnippet/django-forbid
+project_urls = 
+	Documentation=https://docs.pysnippet.org/django-forbid/
+	Source Code=https://github.com/pysnippet/django-forbid/
 keywords = 
 	python
 	django
 	permit
 	forbid
 	access
 	device
@@ -24,14 +26,15 @@
 	detection
 	django-forbid
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Operating System :: OS Independent
+	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
```

### Comparing `django-forbid-0.0.7/src/django_forbid/middleware.py` & `django-forbid-0.1.0/src/django_forbid/middleware.py`

 * *Files identical despite different names*


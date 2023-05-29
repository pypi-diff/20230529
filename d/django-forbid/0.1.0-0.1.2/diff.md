# Comparing `tmp/django-forbid-0.1.0.tar.gz` & `tmp/django-forbid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.1.0.tar", last modified: Wed May 24 09:55:59 2023, max compression
+gzip compressed data, was "django-forbid-0.1.2.tar", last modified: Mon May 29 17:50:08 2023, max compression
```

## Comparing `django-forbid-0.1.0.tar` & `django-forbid-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-24 09:55:43.000000 django-forbid-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-24 09:55:59.327195 django-forbid-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-24 09:55:43.000000 django-forbid-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 09:55:43.000000 django-forbid-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-24 09:55:59.327195 django-forbid-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 09:55:43.000000 django-forbid-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 09:55:43.000000 django-forbid-0.1.0/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:55:59.327195 django-forbid-0.1.0/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 09:55:59.000000 django-forbid-0.1.0/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 17:49:55.000000 django-forbid-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 17:49:55.000000 django-forbid-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-29 17:50:08.087865 django-forbid-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-29 17:49:55.000000 django-forbid-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-29 17:49:55.000000 django-forbid-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-29 17:50:08.087865 django-forbid-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 17:49:55.000000 django-forbid-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.083865 django-forbid-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/skills/forbid_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 17:49:55.000000 django-forbid-0.1.2/src/django_forbid/templates/timezone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:50:08.087865 django-forbid-0.1.2/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 17:50:08.000000 django-forbid-0.1.2/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.1.0/LICENSE` & `django-forbid-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.0/PKG-INFO` & `django-forbid-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.0
+Version: 0.1.2
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```

### Comparing `django-forbid-0.1.0/README.md` & `django-forbid-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.0/setup.cfg` & `django-forbid-0.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	security
 	location
 	territory
 	vpn
 	detection
 	django-forbid
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Operating System :: OS Independent
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
@@ -46,14 +46,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: MIT License
 
 [options]
 packages = 
 	django_forbid
+	django_forbid.skills
 install_requires = 
 	Django>=2.1
 	geoip2
 	device_detector
 include_package_data = yes
 python_requires = >=3.6
 package_dir =
```

### Comparing `django-forbid-0.1.0/src/django_forbid/middleware.py` & `django-forbid-0.1.2/src/django_forbid/middleware.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .skills.forbid_device import ForbidDeviceMiddleware
 from .skills.forbid_location import ForbidLocationMiddleware
 from .skills.forbid_network import ForbidNetworkMiddleware
 
 __skills__ = (
-    ForbidDeviceMiddleware,
-    ForbidLocationMiddleware,
     ForbidNetworkMiddleware,
+    ForbidLocationMiddleware,
+    ForbidDeviceMiddleware,
 )
 
 
 class ForbidMiddleware:
     """Middleware to forbid access to the site."""
 
     def __init__(self, get_response):
```

### Comparing `django-forbid-0.1.0/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.1.2/src/django_forbid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.0
+Version: 0.1.2
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```


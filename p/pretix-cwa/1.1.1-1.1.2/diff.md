# Comparing `tmp/pretix-cwa-1.1.1.tar.gz` & `tmp/pretix-cwa-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-cwa-1.1.1.tar", last modified: Mon Jan 30 15:14:27 2023, max compression
+gzip compressed data, was "pretix-cwa-1.1.2.tar", last modified: Sun May 28 23:08:14 2023, max compression
```

## Comparing `pretix-cwa-1.1.1.tar` & `pretix-cwa-1.1.2.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3071 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.688347 pretix-cwa-1.1.1/pretix_cwa/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3042 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.692347 pretix-cwa-1.1.1/pretix_cwa/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.668347 pretix-cwa-1.1.1/pretix_cwa/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.692347 pretix-cwa-1.1.1/pretix_cwa/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7015 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/pretix_cwa/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/pretix_cwa/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6996 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     4997 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)     2871 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.684347 pretix-cwa-1.1.1/pretix_cwa/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)    10524 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/signage.scss
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.684347 pretix-cwa-1.1.1/pretix_cwa/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.696348 pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     6103 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/settings.html
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/signage.html
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5208 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/pretix_cwa/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:14:27.692347 pretix-cwa-1.1.1/pretix_cwa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      835 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-30 15:14:27.000000 pretix-cwa-1.1.1/pretix_cwa.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-01-30 15:14:27.700348 pretix-cwa-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-01-30 15:13:02.000000 pretix-cwa-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.216564 pretix-cwa-1.1.2/pretix_cwa/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.216564 pretix-cwa-1.1.2/pretix_cwa/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.184563 pretix-cwa-1.1.2/pretix_cwa/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.216564 pretix-cwa-1.1.2/pretix_cwa/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7015 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.216564 pretix-cwa-1.1.2/pretix_cwa/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:07:42.000000 pretix-cwa-1.1.2/pretix_cwa/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/pretix_cwa/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6996 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.184563 pretix-cwa-1.1.2/pretix_cwa/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:07:42.000000 pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)    10524 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/signage.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.184563 pretix-cwa-1.1.2/pretix_cwa/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:07:42.000000 pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/settings.html
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/signage.html
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5208 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pretix_cwa/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.216564 pretix-cwa-1.1.2/pretix_cwa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-28 23:08:14.000000 pretix-cwa-1.1.2/pretix_cwa.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:14.220564 pretix-cwa-1.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 08:38:55.000000 pretix-cwa-1.1.2/tests/test_main.py
```

### Comparing `pretix-cwa-1.1.1/LICENSE` & `pretix-cwa-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/PKG-INFO` & `pretix-cwa-1.1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-cwa
-Version: 1.1.1
-Summary: pretix integration for the Corona Warn App (CWA)
-Home-page: https://github.com/pretix/pretix-cwa
-Author: pretix team
-Author-email: support@pretix.eu
-License: Apache
-License-File: LICENSE
-
 CWA integration
 ===============
 
 This is a plugin for `pretix`_. It integrates pretix with the German Corona Warn App (CWA) by making it easy for event
 organizers to generate event QR codes while at the same time making it really easy for attendees to use them and remind
 them of using it.
 
@@ -37,15 +27,15 @@
 
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

### Comparing `pretix-cwa-1.1.1/README.rst` & `pretix-cwa-1.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: pretix-cwa
+Version: 1.1.2
+Summary: pretix integration for the Corona Warn App (CWA)
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2021 pretix team
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
+Project-URL: homepage, https://github.com/pretix/pretix-cwa
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 CWA integration
 ===============
 
 This is a plugin for `pretix`_. It integrates pretix with the German Corona Warn App (CWA) by making it easy for event
 organizers to generate event QR codes while at the same time making it really easy for attendees to use them and remind
 them of using it.
 
@@ -27,15 +55,15 @@
 
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

### Comparing `pretix-cwa-1.1.1/pretix_cwa/apps.py` & `pretix-cwa-1.1.2/pretix_cwa/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.translation import gettext_lazy
+
 from . import __version__
 
 try:
     from pretix.base.plugins import PluginConfig
 except ImportError:
     raise RuntimeError("Please use pretix 2.7 or above to run this plugin!")
 
@@ -24,9 +25,7 @@
         visible = True
         version = __version__
         category = "INTEGRATION"
         compatibility = "pretix>=3.17.0"
 
     def ready(self):
         from . import signals  # NOQA
-
-
```

### Comparing `pretix-cwa-1.1.1/pretix_cwa/forms.py` & `pretix-cwa-1.1.2/pretix_cwa/forms.py`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/generator.py` & `pretix-cwa-1.1.2/pretix_cwa/generator.py`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/locale/de/LC_MESSAGES/django.po` & `pretix-cwa-1.1.2/pretix_cwa/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-cwa-1.1.2/pretix_cwa/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/locale/django.pot` & `pretix-cwa-1.1.2/pretix_cwa/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/signals.py` & `pretix-cwa-1.1.2/pretix_cwa/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.dispatch import receiver
 from django.urls import resolve, reverse
-from django.utils.translation import gettext_noop, gettext_lazy as _
+from django.utils.translation import gettext_lazy as _, gettext_noop
 from i18nfield.strings import LazyI18nString
 from pretix.base.email import SimpleFunctionalMailTextPlaceholder
 from pretix.base.settings import settings_hierarkey
 from pretix.base.signals import checkin_created, register_mail_placeholders
 from pretix.control.signals import nav_event_settings
 
 from pretix_cwa.generator import generate_url
```

### Comparing `pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/logo.svg` & `pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/static/pretix_cwa/signage.scss` & `pretix-cwa-1.1.2/pretix_cwa/static/pretix_cwa/signage.scss`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/tasks.py` & `pretix-cwa-1.1.2/pretix_cwa/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/settings.html` & `pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/settings.html`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/templates/pretix_cwa/signage.html` & `pretix-cwa-1.1.2/pretix_cwa/templates/pretix_cwa/signage.html`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/urls.py` & `pretix-cwa-1.1.2/pretix_cwa/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa/views.py` & `pretix-cwa-1.1.2/pretix_cwa/views.py`

 * *Files identical despite different names*

### Comparing `pretix-cwa-1.1.1/pretix_cwa.egg-info/SOURCES.txt` & `pretix-cwa-1.1.2/pretix_cwa.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_cwa/__init__.py
 pretix_cwa/apps.py
 pretix_cwa/forms.py
 pretix_cwa/generator.py
 pretix_cwa/signals.py
@@ -22,8 +23,9 @@
 pretix_cwa/locale/de_Informal/.gitkeep
 pretix_cwa/locale/de_Informal/LC_MESSAGES/django.po
 pretix_cwa/static/pretix_cwa/.gitkeep
 pretix_cwa/static/pretix_cwa/logo.svg
 pretix_cwa/static/pretix_cwa/signage.scss
 pretix_cwa/templates/pretix_cwa/.gitkeep
 pretix_cwa/templates/pretix_cwa/settings.html
-pretix_cwa/templates/pretix_cwa/signage.html
+pretix_cwa/templates/pretix_cwa/signage.html
+tests/test_main.py
```

### Comparing `pretix-cwa-1.1.1/setup.cfg` & `pretix-cwa-1.1.2/setup.cfg`

 * *Files identical despite different names*


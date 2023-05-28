# Comparing `tmp/pretix-covid-certificates-2.3.0.tar.gz` & `tmp/pretix-covid-certificates-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-covid-certificates-2.3.0.tar", last modified: Mon Jan 30 13:36:22 2023, max compression
+gzip compressed data, was "pretix-covid-certificates-2.3.1.tar", last modified: Sun May 28 23:06:47 2023, max compression
```

## Comparing `pretix-covid-certificates-2.3.0.tar` & `pretix-covid-certificates-2.3.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1827 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1474 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.282414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 13:34:50.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.282414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16817 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16790 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    11301 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9244 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.282414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/static/pretix_covid_certificates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/static/pretix_covid_certificates/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.282414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates/templates/pretix_covid_certificates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/templates/pretix_covid_certificates/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2688 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/templates/pretix_covid_certificates/settings.html
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    22708 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1827 2023-01-30 13:36:22.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-01-30 13:36:22.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 13:36:22.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-01-30 13:36:22.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-30 13:36:22.000000 pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-01-30 13:36:22.286414 pretix-covid-certificates-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-01-30 13:31:16.000000 pretix-covid-certificates-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.550434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.554434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.546434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.554434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16817 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.554434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:06:10.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.554434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    11301 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/pretix_covid_certificates/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:06:10.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     9244 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.546434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/pretix_covid_certificates/static/pretix_covid_certificates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:06:10.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/static/pretix_covid_certificates/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.546434 pretix-covid-certificates-2.3.1/pretix_covid_certificates/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/pretix_covid_certificates/templates/pretix_covid_certificates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:06:10.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/templates/pretix_covid_certificates/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2688 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/templates/pretix_covid_certificates/settings.html
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    22714 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.554434 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-05-28 23:06:47.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-28 23:06:47.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:06:47.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-28 23:06:47.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-28 23:06:47.000000 pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:06:47.558435 pretix-covid-certificates-2.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 08:34:53.000000 pretix-covid-certificates-2.3.1/tests/test_main.py
```

### Comparing `pretix-covid-certificates-2.3.0/LICENSE` & `pretix-covid-certificates-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/PKG-INFO` & `pretix-covid-certificates-2.3.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-covid-certificates
-Version: 2.3.0
-Summary: This plugin allows to configure the validation of COVID test- and vaccination certificates using pretixSCAN for Android
-Home-page: https://github.com/pretix/pretix-covid-certificates
-Author: Martin Gross
-Author-email: support@pretix.eu
-License: Apache
-License-File: LICENSE
-
 Digital Covid Certificates
 ==========================
 
 This is a plugin for `pretix`_. 
 
 This plugin allows to configure the validation of COVID test- and vaccination certificates using pretixSCAN for Android
 
@@ -20,15 +10,15 @@
 
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

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/apps.py` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.translation import gettext_lazy
+
 from . import __version__
 
 try:
     from pretix.base.plugins import PluginConfig
 except ImportError:
     raise RuntimeError("Please use pretix 3.6 or above to run this plugin!")
 
@@ -22,9 +23,7 @@
         featured = True
         version = __version__
         category = "INTEGRATION"
         compatibility = "pretix>=3.6.0"
 
     def ready(self):
         from . import signals  # NOQA
-
-
```

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de/LC_MESSAGES/django.po` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/locale/django.pot` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/migrations/0001_initial.py` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/signals.py` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/templates/pretix_covid_certificates/settings.html` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/templates/pretix_covid_certificates/settings.html`

 * *Files identical despite different names*

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates/views.py` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 VACCINATION_PRODUCTS = (
     ("EU/1/20/1528", _("Comirnaty (BioNTech/Pfizer)")),
     ("EU/1/20/1525", _("Janssen (Johnson & Johnson)")),
     ("EU/1/20/1507", _("Spikevax (Moderna)")),
     ("EU/1/21/1529", _("Vaxzevria (AstraZeneca)")),
     ("EU/1/21/1618", _("Nuvaxovid (Novavax)")),
     ("NVX-CoV2373", _("NVX-CoV2373 (old name of Nuvaxovid)")),
-    # Preliminary names present in https://github.com/Digitaler-Impfnachweis/covpass-android/blob/20faa2bc04f4296d2a220d5676e964272ad3092b/covpass-sdk/src/main/assets/covpass-sdk/eu-value-sets.json
+    # Preliminary names present in
+    # https://github.com/Digitaler-Impfnachweis/covpass-android/blob/20faa2bc04f4296d2a220d5676e964272ad3092b/covpass-sdk/src/main/assets/covpass-sdk/eu-value-sets.json
     ("Sputnik-V", _("Sputnik-V")),
     ("Sputnik-Light", _("Sputnik Light")),
     ("Convidecia", _("Convidecia")),
     ("Inactivated-SARS-CoV-2-Vero-Cell", _("Inactivated SARS-CoV-2 (Vero Cell)")),
     ("CoviVac", _("CoviVac")),
     ("CoronaVac", _("CoronaVac")),
     ("Covishield", _("Covishield (ChAdOx1_nCoV-19)")),
```

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/PKG-INFO` & `pretix-covid-certificates-2.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-covid-certificates
-Version: 2.3.0
+Version: 2.3.1
 Summary: This plugin allows to configure the validation of COVID test- and vaccination certificates using pretixSCAN for Android
-Home-page: https://github.com/pretix/pretix-covid-certificates
-Author: Martin Gross
-Author-email: support@pretix.eu
-License: Apache
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
+Project-URL: homepage, https://github.com/pretix/pretix-covid-certificates
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Digital Covid Certificates
 ==========================
 
 This is a plugin for `pretix`_. 
 
@@ -20,15 +38,15 @@
 
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

### Comparing `pretix-covid-certificates-2.3.0/pretix_covid_certificates.egg-info/SOURCES.txt` & `pretix-covid-certificates-2.3.1/pretix_covid_certificates.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_covid_certificates/__init__.py
 pretix_covid_certificates/apps.py
 pretix_covid_certificates/models.py
 pretix_covid_certificates/signals.py
 pretix_covid_certificates/urls.py
@@ -18,8 +19,9 @@
 pretix_covid_certificates/locale/de/LC_MESSAGES/django.po
 pretix_covid_certificates/locale/de_Informal/.gitkeep
 pretix_covid_certificates/locale/de_Informal/LC_MESSAGES/django.po
 pretix_covid_certificates/migrations/0001_initial.py
 pretix_covid_certificates/migrations/__init__.py
 pretix_covid_certificates/static/pretix_covid_certificates/.gitkeep
 pretix_covid_certificates/templates/pretix_covid_certificates/.gitkeep
-pretix_covid_certificates/templates/pretix_covid_certificates/settings.html
+pretix_covid_certificates/templates/pretix_covid_certificates/settings.html
+tests/test_main.py
```

### Comparing `pretix-covid-certificates-2.3.0/setup.cfg` & `pretix-covid-certificates-2.3.1/setup.cfg`

 * *Files identical despite different names*


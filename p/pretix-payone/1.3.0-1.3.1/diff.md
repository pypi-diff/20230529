# Comparing `tmp/pretix-payone-1.3.0.tar.gz` & `tmp/pretix-payone-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-payone-1.3.0.tar", last modified: Mon Jan 30 14:05:16 2023, max compression
+gzip compressed data, was "pretix-payone-1.3.1.tar", last modified: Sun May 28 23:20:01 2023, max compression
```

## Comparing `pretix-payone-1.3.0.tar` & `pretix-payone-1.3.1.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.116189 pretix-payone-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1668 2023-01-30 14:05:16.116189 pretix-payone-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1397 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:04:43.000000 pretix-payone-1.3.0/pretix_payone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-01-30 14:04:43.000000 pretix-payone-1.3.0/pretix_payone/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.092189 pretix-payone-1.3.0/pretix_payone/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10537 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10484 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8146 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/migrations/0002_auto_20220204_1638.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/models.py
--rw-rw-rw-   0 root         (0) root         (0)    33654 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     2484 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.092189 pretix-payone-1.3.0/pretix_payone/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone/static/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/static/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     6372 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/static/pretix_payone/cc.js
--rw-rw-rw-   0 root         (0) root         (0)     3517 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/static/pretix_payone/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.096189 pretix-payone-1.3.0/pretix_payone/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.116189 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/control.html
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8681 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/pretix_payone/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:05:16.112189 pretix-payone-1.3.0/pretix_payone.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1668 2023-01-30 14:05:16.000000 pretix-payone-1.3.0/pretix_payone.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1240 2023-01-30 14:05:16.000000 pretix-payone-1.3.0/pretix_payone.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:05:16.000000 pretix-payone-1.3.0/pretix_payone.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-30 14:05:16.000000 pretix-payone-1.3.0/pretix_payone.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-30 14:05:16.000000 pretix-payone-1.3.0/pretix_payone.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-01-30 14:05:16.116189 pretix-payone-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-01-30 14:01:53.000000 pretix-payone-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.233943 pretix-payone-1.3.1/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10537 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10484 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8146 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/migrations/0002_auto_20220204_1638.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    33634 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/cc.js
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/static/pretix_payone/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.229943 pretix-payone-1.3.1/pretix_payone/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:19:29.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8795 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pretix_payone/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.237943 pretix-payone-1.3.1/pretix_payone.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:20:01.000000 pretix-payone-1.3.1/pretix_payone.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:20:01.241943 pretix-payone-1.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 23:15:08.000000 pretix-payone-1.3.1/tests/test_main.py
```

### Comparing `pretix-payone-1.3.0/LICENSE` & `pretix-payone-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/PKG-INFO` & `pretix-payone-1.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-payone
-Version: 1.3.0
-Summary: Allows to process payments through PAYONE (formerly BS Payone)
-Home-page: https://github.com/pretix/pretix-payone
-Author: pretix team
-Author-email: support@pretix.eu
-License: Apache
-License-File: LICENSE
-
 PayOne
 ==========================
 
 This is a plugin for `pretix`_. 
 
 Allows to process payments through PAYONE (formerly BS Payone)
 
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

### Comparing `pretix-payone-1.3.0/pretix_payone/apps.py` & `pretix-payone-1.3.1/pretix_payone/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.translation import gettext_lazy
+
 from . import __version__
 
 try:
     from pretix.base.plugins import PluginConfig
 except ImportError:
     raise RuntimeError("Please use pretix 2.7 or above to run this plugin!")
 
@@ -18,13 +19,11 @@
         description = gettext_lazy(
             "Accept payments through PAYONE (formerly BS Payone)."
         )
         picture = "pretix_payone/logo.svg"
         visible = True
         version = __version__
         category = "PAYMENT"
-        compatibility = "pretix>=4.16.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
-
-
```

### Comparing `pretix-payone-1.3.0/pretix_payone/locale/de/LC_MESSAGES/django.po` & `pretix-payone-1.3.1/pretix_payone/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-payone-1.3.1/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/locale/django.pot` & `pretix-payone-1.3.1/pretix_payone/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/migrations/0001_initial.py` & `pretix-payone-1.3.1/pretix_payone/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.12 on 2021-03-22 16:00
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("pretixbase", "0179_auto_20210311_1653"),
     ]
 
     operations = [
```

### Comparing `pretix-payone-1.3.0/pretix_payone/migrations/0002_auto_20220204_1638.py` & `pretix-payone-1.3.1/pretix_payone/migrations/0002_auto_20220204_1638.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                 )
             )
 
         EventSettingsStore.objects.bulk_create(b, ignore_conflicts=True)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("pretix_payone", "0001_initial"),
     ]
 
     operations = [
         migrations.RunPython(
             code=set_default_cardtypes,
```

### Comparing `pretix-payone-1.3.0/pretix_payone/payment.py` & `pretix-payone-1.3.1/pretix_payone/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import hashlib
 import json
 import logging
 import requests
-import urllib.parse
 from collections import OrderedDict
 from django import forms
 from django.conf import settings
 from django.contrib import messages
 from django.core import signing
 from django.http import HttpRequest
 from django.template.loader import get_template
```

### Comparing `pretix-payone-1.3.0/pretix_payone/signals.py` & `pretix-payone-1.3.1/pretix_payone/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/static/pretix_payone/cc.js` & `pretix-payone-1.3.1/pretix_payone/static/pretix_payone/cc.js`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/static/pretix_payone/logo.svg` & `pretix-payone-1.3.1/pretix_payone/static/pretix_payone/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html` & `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/control.html` & `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/control.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/pending.html` & `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/templates/pretix_payone/redirect.html` & `pretix-payone-1.3.1/pretix_payone/templates/pretix_payone/redirect.html`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <html>
 <head>
     <title>{{ settings.PRETIX_INSTANCE_NAME }}</title>
     {% compress css %}
         <link rel="stylesheet" type="text/x-scss" href="{% static "pretixbase/scss/cachedfiles.scss" %}"/>
     {% endcompress %}
     {% compress js %}
-        <script type="text/javascript" src="{% static "jquery/js/jquery-2.1.1.min.js" %}"></script>
+        <script type="text/javascript" src="{% static "jquery/js/jquery-3.6.4.min.js" %}"></script>
     {% endcompress %}
 </head>
 <body>
     <div class="container">
         <h1>{% trans "The payment process has started in a new window." %}</h1>
 
         <p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load compress %} {% load i18n %} {% load static %}
 {% compress css %}
 css/cachedfiles.scss" %}"/> {% endcompress %} {% compress js %}
-s/jquery-2.1.1.min.js" %}">
+s/jquery-3.6.4.min.js" %}">
 {% endcompress %}
 ****** {% trans "The payment process has started in a new window." %} ******
 {% trans "The window to enter your payment data was not opened or was closed?"
 %}
 _{%_trans_"Click_here_in_order_to_open_the_window."_%}
```

### Comparing `pretix-payone-1.3.0/pretix_payone/urls.py` & `pretix-payone-1.3.1/pretix_payone/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.0/pretix_payone/views.py` & `pretix-payone-1.3.1/pretix_payone/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,40 +89,46 @@
 
 
 @method_decorator(xframe_options_exempt, "dispatch")
 class ReturnView(PayoneOrderView, View):
     def get(self, request, *args, **kwargs):
         if kwargs["action"] == "error":
             with transaction.atomic():
-                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=self.payment.pk)
+                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(
+                    pk=self.payment.pk
+                )
                 if p.state == OrderPayment.PAYMENT_STATE_CREATED:
                     self.payment.fail()
             messages.error(
                 self.request,
                 _("The payment process has failed. See below for more information."),
             )
             return self._redirect_to_order()
         elif kwargs["action"] == "cancel":
             with transaction.atomic():
-                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=self.payment.pk)
+                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(
+                    pk=self.payment.pk
+                )
                 if p.state == OrderPayment.PAYMENT_STATE_CREATED:
                     self.payment.state = OrderPayment.PAYMENT_STATE_CANCELED
                     self.payment.save(update_fields=["state"])
                     self.payment.order.log_action(
                         "pretix.event.order.payment.canceled",
                         {
                             "local_id": self.payment.local_id,
                             "provider": self.payment.provider,
                             "data": self.payment.info_data,
                         },
                     )
             return self._redirect_to_order()
         elif kwargs["action"] == "success":
             with transaction.atomic():
-                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=self.payment.pk)
+                p = OrderPayment.objects.select_for_update(of=OF_SELF).get(
+                    pk=self.payment.pk
+                )
                 if p.state == OrderPayment.PAYMENT_STATE_CREATED:
                     p.state = OrderPayment.PAYMENT_STATE_PENDING
                     p.save(update_fields=["state"])
             return self._redirect_to_order()
 
     def _redirect_to_order(self):
         if self.request.session.get("payment_payone_order_secret") != self.order.secret:
```

### Comparing `pretix-payone-1.3.0/pretix_payone.egg-info/PKG-INFO` & `pretix-payone-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-payone
-Version: 1.3.0
+Version: 1.3.1
 Summary: Allows to process payments through PAYONE (formerly BS Payone)
-Home-page: https://github.com/pretix/pretix-payone
-Author: pretix team
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
+Project-URL: homepage, https://github.com/pretix/pretix-payone
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PayOne
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

### Comparing `pretix-payone-1.3.0/pretix_payone.egg-info/SOURCES.txt` & `pretix-payone-1.3.1/pretix_payone.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_payone/__init__.py
 pretix_payone/apps.py
 pretix_payone/models.py
 pretix_payone/payment.py
 pretix_payone/signals.py
@@ -27,8 +28,9 @@
 pretix_payone/static/pretix_payone/logo.svg
 pretix_payone/templates/pretix_payone/.gitkeep
 pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
 pretix_payone/templates/pretix_payone/checkout_payment_form.html
 pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
 pretix_payone/templates/pretix_payone/control.html
 pretix_payone/templates/pretix_payone/pending.html
-pretix_payone/templates/pretix_payone/redirect.html
+pretix_payone/templates/pretix_payone/redirect.html
+tests/test_main.py
```

### Comparing `pretix-payone-1.3.0/setup.cfg` & `pretix-payone-1.3.1/setup.cfg`

 * *Files identical despite different names*


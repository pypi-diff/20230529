# Comparing `tmp/pretix-modirum-1.1.0.tar.gz` & `tmp/pretix-modirum-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-modirum-1.1.0.tar", last modified: Mon Jan 30 14:51:43 2023, max compression
+gzip compressed data, was "pretix-modirum-1.1.1.tar", last modified: Sun May 28 23:08:38 2023, max compression
```

## Comparing `pretix-modirum-1.1.0.tar` & `pretix-modirum-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.011444 pretix-modirum-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2391 2023-01-30 14:51:43.011444 pretix-modirum-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/static/pretix_modirum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/static/pretix_modirum/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/static/pretix_modirum/js/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/static/pretix_modirum/js/redirect.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.011444 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/control.html
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/redirecting.html
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5470 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/pretix_modirum/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:51:43.007444 pretix-modirum-1.1.0/pretix_modirum.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2391 2023-01-30 14:51:42.000000 pretix-modirum-1.1.0/pretix_modirum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2023-01-30 14:51:42.000000 pretix-modirum-1.1.0/pretix_modirum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:51:42.000000 pretix-modirum-1.1.0/pretix_modirum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-01-30 14:51:42.000000 pretix-modirum-1.1.0/pretix_modirum.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-30 14:51:42.000000 pretix-modirum-1.1.0/pretix_modirum.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-01-30 14:51:43.011444 pretix-modirum-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-01-30 14:50:45.000000 pretix-modirum-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.929171 pretix-modirum-1.1.1/pretix_modirum/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.929171 pretix-modirum-1.1.1/pretix_modirum/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:10.000000 pretix-modirum-1.1.1/pretix_modirum/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.929171 pretix-modirum-1.1.1/pretix_modirum/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/static/pretix_modirum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:10.000000 pretix-modirum-1.1.1/pretix_modirum/static/pretix_modirum/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/static/pretix_modirum/js/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/static/pretix_modirum/js/redirect.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.929171 pretix-modirum-1.1.1/pretix_modirum/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:10.000000 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/redirecting.html
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5470 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pretix_modirum/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:38.933172 pretix-modirum-1.1.1/pretix_modirum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-05-28 23:08:38.000000 pretix-modirum-1.1.1/pretix_modirum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      946 2023-05-28 23:08:38.000000 pretix-modirum-1.1.1/pretix_modirum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:08:38.000000 pretix-modirum-1.1.1/pretix_modirum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-28 23:08:38.000000 pretix-modirum-1.1.1/pretix_modirum.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-28 23:08:38.000000 pretix-modirum-1.1.1/pretix_modirum.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-05-28 23:08:38.937172 pretix-modirum-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:46:57.000000 pretix-modirum-1.1.1/setup.py
```

### Comparing `pretix-modirum-1.1.0/LICENSE` & `pretix-modirum-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-modirum-1.1.0/PKG-INFO` & `pretix-modirum-1.1.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-modirum
-Version: 1.1.0
-Summary: Integration for payment providers based on the Modirum platform
-Home-page: https://code.rami.io/pretix/pretix-modirum
-Author: Martin Gross
-Author-email: gross@rami.io
-License: Apache Software License
-License-File: LICENSE
-
 Modirum payments for pretix
 ===========================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-modirum``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
 
 Test card numbers
```

### Comparing `pretix-modirum-1.1.0/pretix_modirum/apps.py` & `pretix-modirum-1.1.1/pretix_modirum/apps.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
     class PretixPluginMeta:
         name = gettext_lazy('Modirum payments for pretix')
         author = 'Martin Gross'
         description = gettext_lazy('Integration for payment providers based on the Modirum platform')
         visible = True
         version = __version__
-        compatibility = "pretix>=2.7.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-modirum-1.1.0/pretix_modirum/payment.py` & `pretix-modirum-1.1.1/pretix_modirum/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-modirum-1.1.0/pretix_modirum/signals.py` & `pretix-modirum-1.1.1/pretix_modirum/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/control.html` & `pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/control.html`

 * *Files identical despite different names*

### Comparing `pretix-modirum-1.1.0/pretix_modirum/templates/pretix_modirum/redirecting.html` & `pretix-modirum-1.1.1/pretix_modirum/templates/pretix_modirum/redirecting.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <html>
 <head>
     <title>{% trans "Redirecting..." %}</title>
     {% compress css %}
         <link rel="stylesheet" type="text/x-scss" href="{% static "pretixbase/scss/cachedfiles.scss" %}"/>
     {% endcompress %}
     {% compress js %}
-        <script type="text/javascript" src="{% static "jquery/js/jquery-2.1.1.min.js" %}"></script>
+        <script type="text/javascript" src="{% static "jquery/js/jquery-3.6.4.min.js" %}"></script>
         <script type="text/javascript" src="{% static "pretix_modirum/js/redirect.js" %}"></script>
     {% endcompress %}
     <meta name="viewport" content="width=device-width, initial-scale=1">
 </head>
 <body>
     <div class="container">
         <i class="fa fa-cog big-animated-icon"></i>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load compress %} {% load i18n %} {% load staticfiles %}
 {% compress css %}
 css/cachedfiles.scss" %}"/> {% endcompress %} {% compress js %}
-s/jquery-2.1.1.min.js" %}">
+s/jquery-3.6.4.min.js" %}">
 s/redirect.js" %}">
 {% endcompress %}
 ****** {% trans "You will be redirected shortly." %} ******
 {% trans "If this takes longer than a few seconds, press this button:" %}
 {% trans "Please turn on JavaScript, before you continue." %}
 {% for k, v in params.items %}  {% endfor %}
 {% trans "Continue" %}
```

### Comparing `pretix-modirum-1.1.0/pretix_modirum/views.py` & `pretix-modirum-1.1.1/pretix_modirum/views.py`

 * *Files identical despite different names*

### Comparing `pretix-modirum-1.1.0/pretix_modirum.egg-info/SOURCES.txt` & `pretix-modirum-1.1.1/pretix_modirum.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_modirum/__init__.py
 pretix_modirum/apps.py
 pretix_modirum/payment.py
 pretix_modirum/signals.py
 pretix_modirum/urls.py
```

### Comparing `pretix-modirum-1.1.0/setup.cfg` & `pretix-modirum-1.1.1/setup.cfg`

 * *Files identical despite different names*


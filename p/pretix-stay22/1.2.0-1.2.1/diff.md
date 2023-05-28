# Comparing `tmp/pretix-stay22-1.2.0.tar.gz` & `tmp/pretix-stay22-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-stay22-1.2.0.tar", last modified: Mon Jan 30 14:54:56 2023, max compression
+gzip compressed data, was "pretix-stay22-1.2.1.tar", last modified: Sun May 28 23:30:44 2023, max compression
```

## Comparing `pretix-stay22-1.2.0.tar` & `pretix-stay22-1.2.1.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1743 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1984 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2009 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2207 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.712117 pretix-stay22-1.2.0/pretix_stay22/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2139 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1589 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1594 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     3803 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     7540 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/postamble.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.716117 pretix-stay22-1.2.0/pretix_stay22/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.724117 pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/order_info.html
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/settings.html
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1351 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/pretix_stay22/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:54:56.720117 pretix-stay22-1.2.0/pretix_stay22.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-30 14:54:56.000000 pretix-stay22-1.2.0/pretix_stay22.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1479 2023-01-30 14:54:56.000000 pretix-stay22-1.2.0/pretix_stay22.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:54:56.000000 pretix-stay22-1.2.0/pretix_stay22.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-30 14:54:56.000000 pretix-stay22-1.2.0/pretix_stay22.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-30 14:54:56.000000 pretix-stay22-1.2.0/pretix_stay22.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-01-30 14:54:56.728117 pretix-stay22-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-01-30 14:54:01.000000 pretix-stay22-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.153740 pretix-stay22-1.2.1/pretix_stay22/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.153740 pretix-stay22-1.2.1/pretix_stay22/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1784 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.153740 pretix-stay22-1.2.1/pretix_stay22/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1743 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.165740 pretix-stay22-1.2.1/pretix_stay22/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.181740 pretix-stay22-1.2.1/pretix_stay22/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.185741 pretix-stay22-1.2.1/pretix_stay22/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.185741 pretix-stay22-1.2.1/pretix_stay22/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.185741 pretix-stay22-1.2.1/pretix_stay22/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.185741 pretix-stay22-1.2.1/pretix_stay22/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/pretix_stay22/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/pretix_stay22/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1594 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     3803 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     7540 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/postamble.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.157740 pretix-stay22-1.2.1/pretix_stay22/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.189741 pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/order_info.html
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/settings.html
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pretix_stay22/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:30:44.161740 pretix-stay22-1.2.1/pretix_stay22.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-28 23:30:44.000000 pretix-stay22-1.2.1/pretix_stay22.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-05-28 23:30:44.000000 pretix-stay22-1.2.1/pretix_stay22.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:30:44.000000 pretix-stay22-1.2.1/pretix_stay22.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:30:44.000000 pretix-stay22-1.2.1/pretix_stay22.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:30:44.000000 pretix-stay22-1.2.1/pretix_stay22.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-05-28 23:30:44.193741 pretix-stay22-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 23:30:18.000000 pretix-stay22-1.2.1/setup.py
```

### Comparing `pretix-stay22-1.2.0/LICENSE` & `pretix-stay22-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/PKG-INFO` & `pretix-stay22-1.2.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-stay22
-Version: 1.2.0
-Summary: This plugin allows to integrate the Stay22 hotel map into your pretix shop
-Home-page: https://github.com/pretix/pretix-stay22
-Author: Raphael Michel
-Author-email: michel@rami.io
-License: Apache Software License
-License-File: LICENSE
-
 Stay22 Hotel map
 ================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-stay22``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/apps.py` & `pretix-stay22-1.2.1/pretix_stay22/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/ar/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/cs/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-10-21 18:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_stay22/__init__.py:13
 msgid "Stay22 Hotel map"
 msgstr ""
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/da/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/de/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/django.pot` & `pretix-stay22-1.2.1/pretix_stay22/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/el/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/es/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/fi/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/fr/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/hr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-10-21 18:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: fr\n"
+"Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_stay22/__init__.py:13
 msgid "Stay22 Hotel map"
 msgstr ""
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/hr/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-10-21 18:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: hr\n"
+"Language: nl_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_stay22/__init__.py:13
 msgid "Stay22 Hotel map"
 msgstr ""
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/lv/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/nl/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/ru/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-10-21 18:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: nl_Informal\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_stay22/__init__.py:13
 msgid "Stay22 Hotel map"
 msgstr ""
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/ru/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2019-10-21 18:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ru\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_stay22/__init__.py:13
 msgid "Stay22 Hotel map"
 msgstr ""
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22/locale/si/LC_MESSAGES/django.po` & `pretix-stay22-1.2.1/pretix_stay22/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/signals.py` & `pretix-stay22-1.2.1/pretix_stay22/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/logo.svg` & `pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/static/pretix_stay22/postamble.scss` & `pretix-stay22-1.2.1/pretix_stay22/static/pretix_stay22/postamble.scss`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/order_info.html` & `pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/order_info.html`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/templates/pretix_stay22/settings.html` & `pretix-stay22-1.2.1/pretix_stay22/templates/pretix_stay22/settings.html`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22/views.py` & `pretix-stay22-1.2.1/pretix_stay22/views.py`

 * *Files identical despite different names*

### Comparing `pretix-stay22-1.2.0/pretix_stay22.egg-info/PKG-INFO` & `pretix-stay22-1.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-stay22
-Version: 1.2.0
+Version: 1.2.1
 Summary: This plugin allows to integrate the Stay22 hotel map into your pretix shop
-Home-page: https://github.com/pretix/pretix-stay22
-Author: Raphael Michel
-Author-email: michel@rami.io
-License: Apache Software License
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2019 Raphael Michel
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
+Project-URL: homepage, https://github.com/pretix/pretix-stay22
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Stay22 Hotel map
 ================
 
 This is a plugin for `pretix`_. 
 
@@ -18,15 +36,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-stay22``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-stay22-1.2.0/pretix_stay22.egg-info/SOURCES.txt` & `pretix-stay22-1.2.1/pretix_stay22.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_stay22/__init__.py
 pretix_stay22/apps.py
 pretix_stay22/signals.py
 pretix_stay22/urls.py
 pretix_stay22/views.py
```

### Comparing `pretix-stay22-1.2.0/setup.cfg` & `pretix-stay22-1.2.1/setup.cfg`

 * *Files identical despite different names*


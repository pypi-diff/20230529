# Comparing `tmp/pretix-servicefees-1.8.0.tar.gz` & `tmp/pretix-servicefees-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-servicefees-1.8.0.tar", last modified: Fri Apr  1 10:39:51 2022, max compression
+gzip compressed data, was "pretix-servicefees-1.9.0.tar", last modified: Thu Sep 29 11:32:59 2022, max compression
```

## Comparing `pretix-servicefees-1.8.0.tar` & `pretix-servicefees-1.9.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      141 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1213 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      899 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/
--rw-rw-rw-   0 root         (0) root         (0)      584 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3873 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3742 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5492 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5531 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     3599 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4971 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4127 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5828 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3577 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5869 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.269768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3583 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3577 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3789 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3574 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4474 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     3804 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6973 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/static/pretix_servicefees/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/static/pretix_servicefees/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/pretix_servicefees/templates/pretix_servicefees/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/templates/pretix_servicefees/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1935 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/templates/pretix_servicefees/settings.html
--rw-rw-rw-   0 root         (0) root         (0)      223 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/pretix_servicefees/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-01 10:39:51.273768 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1213 2022-04-01 10:39:50.000000 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1999 2022-04-01 10:39:51.000000 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-01 10:39:50.000000 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-04-01 10:39:50.000000 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-04-01 10:39:50.000000 pretix-servicefees-1.8.0/pretix_servicefees.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      363 2022-04-01 10:39:51.277768 pretix-servicefees-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-03-31 20:32:46.000000 pretix-servicefees-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      141 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1193 2022-09-29 11:32:59.131025 pretix-servicefees-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      899 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/
+-rw-rw-rw-   0 root         (0) root         (0)      584 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3873 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3742 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5531 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.119024 pretix-servicefees-1.9.0/pretix_servicefees/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4127 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5869 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3583 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3574 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4474 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     8635 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/static/pretix_servicefees/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/static/pretix_servicefees/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.123025 pretix-servicefees-1.9.0/pretix_servicefees/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees/templates/pretix_servicefees/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/templates/pretix_servicefees/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2015 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/templates/pretix_servicefees/settings.html
+-rw-rw-rw-   0 root         (0) root         (0)      223 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/pretix_servicefees/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 11:32:59.127025 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1193 2022-09-29 11:32:59.000000 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1999 2022-09-29 11:32:59.000000 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-29 11:32:59.000000 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-09-29 11:32:59.000000 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-29 11:32:59.000000 pretix-servicefees-1.9.0/pretix_servicefees.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      363 2022-09-29 11:32:59.131025 pretix-servicefees-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2022-09-29 11:32:16.000000 pretix-servicefees-1.9.0/setup.py
```

### Comparing `pretix-servicefees-1.8.0/LICENSE` & `pretix-servicefees-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/PKG-INFO` & `pretix-servicefees-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretix-servicefees
-Version: 1.8.0
+Version: 1.9.0
 Summary: Allows you to impose a service fee on all non-free orders.
 Home-page: https://github.com/pretix/pretix-servicefees
 Author: Raphael Michel
 Author-email: michel@rami.io
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 pretix Service Fees
 ==========================
 
 This is a plugin for `pretix`_. 
 
@@ -37,9 +36,7 @@
 Copyright 2018 Raphael Michel
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
-
-
```

### Comparing `pretix-servicefees-1.8.0/README.rst` & `pretix-servicefees-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/__init__.py` & `pretix-servicefees-1.9.0/pretix_servicefees/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
     class PretixPluginMeta:
         name = gettext_lazy('Service Fees')
         author = 'Raphael Michel'
         category = 'FEATURE'
         description = gettext_lazy('This plugin allows to charge a service fee on all non-free orders.')
         visible = True
-        version = '1.8.0'
+        version = '1.9.0'
 
     def ready(self):
         from . import signals  # NOQA
 
 
 default_app_config = 'pretix_servicefees.PluginApp'
```

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/ar/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/ca/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/cs/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/da/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/de/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/django.pot` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/el/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/es/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/fi/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/fr/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/it/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/ja/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/lv/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/nl/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/pl/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/pt/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/ru/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/si/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/sl/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/sv/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/tr/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-servicefees-1.9.0/pretix_servicefees/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/signals.py` & `pretix-servicefees-1.9.0/pretix_servicefees/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from collections import defaultdict
 from decimal import Decimal
-
-from django.urls import resolve, reverse
 from django.dispatch import receiver
 from django.http import HttpRequest
-from django.utils.translation import gettext_lazy as _, gettext, get_language
+from django.urls import resolve, reverse
+from django.utils.translation import get_language, gettext, gettext_lazy as _
 from pretix.base.decimal import round_decimal
-from pretix.base.models import Event, Order, TaxRule
+from pretix.base.models import CartPosition, Event, Order, TaxRule
 from pretix.base.models.orders import OrderFee
 from pretix.base.settings import settings_hierarkey
 from pretix.base.signals import order_fee_calculation
 from pretix.base.templatetags.money import money_filter
 from pretix.control.signals import nav_event_settings
-from pretix.presale.signals import fee_calculation_for_cart, front_page_top, order_meta_from_request
+from pretix.presale.signals import (
+    fee_calculation_for_cart, front_page_top, order_meta_from_request,
+)
 from pretix.presale.views import get_cart
 from pretix.presale.views.cart import cart_session
 
 
 @receiver(nav_event_settings, dispatch_uid='service_fee_nav_settings')
 def navbar_settings(sender, request, **kwargs):
     url = resolve(request.path_info)
@@ -72,33 +74,70 @@
             fval = Decimal(gc.value)  # TODO: don't require an extra query
             fval = min(fval, total - summed)
             if fval > 0:
                 total -= fval
                 summed += fval
 
     if (fee_per_ticket or fee_abs or fee_percent) and total != Decimal('0.00'):
+        tax_rule_zero = TaxRule.zero()
         fee = round_decimal(fee_abs + total * (fee_percent / 100) + len(positions) * fee_per_ticket, event.currency)
-        tax_rule = event.settings.tax_rate_default or TaxRule.zero()
-        tax = tax_rule.tax(fee, invoice_address=invoice_address, base_price_is='gross')
-        return [OrderFee(
-            fee_type=OrderFee.FEE_TYPE_SERVICE,
-            internal_type='',
-            value=fee,
-            tax_rate=tax.rate,
-            tax_value=tax.tax,
-            tax_rule=tax_rule
-        )]
+        split_taxes = event.settings.get('service_fee_split_taxes', as_type=bool)
+        if split_taxes:
+            # split taxes based on products ordered
+            d = defaultdict(lambda: Decimal('0.00'))
+            for p in positions:
+                if isinstance(p, CartPosition):
+                    tr = p.item.tax_rule
+                else:
+                    tr = p.tax_rule
+                d[tr] += p.price - p.tax_value
+
+            base_values = sorted([tuple(t) for t in d.items()], key=lambda t: t[0].rate)
+            sum_base = sum(t[1] for t in base_values)
+            if sum_base:
+                fee_values = [(t[0], round_decimal(fee * t[1] / sum_base, event.currency))
+                              for t in base_values]
+                sum_fee = sum(t[1] for t in fee_values)
+
+                # If there are rounding differences, we fix them up, but always leaning to the benefit of the tax
+                # authorities
+                if sum_fee > fee:
+                    fee_values[0] = (fee_values[0][0], fee_values[0][1] + (fee - sum_fee))
+                elif sum_fee < fee:
+                    fee_values[-1] = (fee_values[-1][0], fee_values[-1][1] + (fee - sum_fee))
+            else:
+                fee_values = [(event.settings.tax_rate_default or tax_rule_zero, fee)]
+
+        else:
+            fee_values = [(event.settings.tax_rate_default or tax_rule_zero, fee)]
+
+        fees = []
+        for tax_rule, price in fee_values:
+            tax_rule = tax_rule or tax_rule_zero
+            tax = tax_rule.tax(price, invoice_address=invoice_address, base_price_is='gross')
+            fees.append(OrderFee(
+                fee_type=OrderFee.FEE_TYPE_SERVICE,
+                internal_type='',
+                value=price,
+                tax_rate=tax.rate,
+                tax_value=tax.tax,
+                tax_rule=tax_rule
+            ))
+        return fees
+
     return []
 
 
 @receiver(fee_calculation_for_cart, dispatch_uid="service_fee_calc_cart")
 def cart_fee(sender: Event, request: HttpRequest, invoice_address, total, **kwargs):
     mod = ''
     try:
-        from pretix_resellers.utils import ResellerException, get_reseller_and_user
+        from pretix_resellers.utils import (
+            ResellerException, get_reseller_and_user,
+        )
     except ImportError:
         pass
     else:
         try:
             reseller, user = get_reseller_and_user(request)
             config = reseller.configs.get(organizer_id=sender.organizer_id)
             if config.skip_default_service_fees:
@@ -149,15 +188,17 @@
         )
 
 
 @receiver(order_meta_from_request, dispatch_uid="servicefees_order_meta")
 def order_meta_signal(sender: Event, request: HttpRequest, **kwargs):
     meta = {}
     try:
-        from pretix_resellers.utils import ResellerException, get_reseller_and_user
+        from pretix_resellers.utils import (
+            ResellerException, get_reseller_and_user,
+        )
     except ImportError:
         pass
     else:
         try:
             reseller, user = get_reseller_and_user(request)
             meta['servicefees_reseller_id'] = reseller.pk
         except ResellerException:
```

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/templates/pretix_servicefees/settings.html` & `pretix-servicefees-1.9.0/pretix_servicefees/templates/pretix_servicefees/settings.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
           <legend>{% trans "Service fees" %}</legend>
             {% bootstrap_field form.service_fee_per_ticket addon_after=request.event.currency layout="control" %}
             {% bootstrap_field form.service_fee_skip_non_admission layout="control" %}
             {% bootstrap_field form.service_fee_skip_addons layout="control" %}
             {% bootstrap_field form.service_fee_skip_free layout="control" %}
             {% bootstrap_field form.service_fee_abs addon_after=request.event.currency layout="control" %}
             {% bootstrap_field form.service_fee_percent addon_after="%" layout="control" %}
+            {% bootstrap_field form.service_fee_split_taxes layout="control" %}
             {% bootstrap_field form.service_fee_skip_if_gift_card layout="control" %}
         </fieldset>
         <fieldset>
           <legend>{% trans "Service fees with resellers" %}</legend>
             <p>
                 {% trans "If you keep values empty, we will fall back to the values from above. If you do not want to charge any fees through this sales channel, set them to zero explicity." %}
             </p>
```

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees/views.py` & `pretix-servicefees-1.9.0/pretix_servicefees/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         required=False
     )
     service_fee_skip_free = forms.BooleanField(
         label=_('Do not charge per-ticket service fee on free products'),
         help_text=_('Note that regardless of this setting, a per-ticket fee will not be charged if the entire order is free.'),
         required=False
     )
+    service_fee_split_taxes = forms.BooleanField(
+        label=_('Split taxes proportionate to the tax rates and net values of the ordered products.'),
+        help_text=_('If not split based on ordered products, the tax rate falls back to the event’s base tax rate or no tax, if none is given.'),
+        required=False
+    )
 
     service_fee_abs_resellers = forms.DecimalField(
         label=_('Fixed fee per order'),
         required=False
     )
     service_fee_percent_resellers = forms.DecimalField(
         label=_('Percentual fee per order'),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees.egg-info/PKG-INFO` & `pretix-servicefees-1.9.0/pretix_servicefees.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretix-servicefees
-Version: 1.8.0
+Version: 1.9.0
 Summary: Allows you to impose a service fee on all non-free orders.
 Home-page: https://github.com/pretix/pretix-servicefees
 Author: Raphael Michel
 Author-email: michel@rami.io
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 pretix Service Fees
 ==========================
 
 This is a plugin for `pretix`_. 
 
@@ -37,9 +36,7 @@
 Copyright 2018 Raphael Michel
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretix: https://github.com/pretix/pretix
 .. _pretix development setup: https://docs.pretix.eu/en/latest/development/setup.html
-
-
```

### Comparing `pretix-servicefees-1.8.0/pretix_servicefees.egg-info/SOURCES.txt` & `pretix-servicefees-1.9.0/pretix_servicefees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-servicefees-1.8.0/setup.py` & `pretix-servicefees-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 cmdclass = {
     'build': CustomBuild
 }
 
 
 setup(
     name='pretix-servicefees',
-    version='1.8.0',
+    version='1.9.0',
     description='Allows you to impose a service fee on all non-free orders.',
     long_description=long_description,
     url='https://github.com/pretix/pretix-servicefees',
     author='Raphael Michel',
     author_email='michel@rami.io',
     license='Apache Software License',
```


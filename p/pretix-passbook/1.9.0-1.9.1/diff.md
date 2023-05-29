# Comparing `tmp/pretix-passbook-1.9.0.tar.gz` & `tmp/pretix-passbook-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-passbook-1.9.0.tar", last modified: Fri Aug 27 14:24:31 2021, max compression
+gzip compressed data, was "pretix-passbook-1.9.1.tar", last modified: Mon Nov 29 10:35:15 2021, max compression
```

## Comparing `pretix-passbook-1.9.0.tar` & `pretix-passbook-1.9.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      579 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      132 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2926 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2655 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.511206 pretix-passbook-1.9.0/pretix_passbook/
--rw-rw-rw-   0 root         (0) root         (0)     1167 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3044 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.515206 pretix-passbook-1.9.0/pretix_passbook/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.491207 pretix-passbook-1.9.0/pretix_passbook/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.515206 pretix-passbook-1.9.0/pretix_passbook/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5340 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ar/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.491207 pretix-passbook-1.9.0/pretix_passbook/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.515206 pretix-passbook-1.9.0/pretix_passbook/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4970 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ca/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.515206 pretix-passbook-1.9.0/pretix_passbook/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4970 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/cs/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.519206 pretix-passbook-1.9.0/pretix_passbook/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5190 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/da/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.519206 pretix-passbook-1.9.0/pretix_passbook/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7399 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1209 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.519206 pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.519206 pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7422 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1204 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/LC_MESSAGES/djangojs.po
--rw-rw-rw-   0 root         (0) root         (0)     4995 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)      981 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/djangojs.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.527206 pretix-passbook-1.9.0/pretix_passbook/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4970 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/el/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.527206 pretix-passbook-1.9.0/pretix_passbook/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7459 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1304 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.527206 pretix-passbook-1.9.0/pretix_passbook/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5196 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.495206 pretix-passbook-1.9.0/pretix_passbook/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.527206 pretix-passbook-1.9.0/pretix_passbook/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5191 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/it/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.531206 pretix-passbook-1.9.0/pretix_passbook/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7116 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/lv/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1465 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.531206 pretix-passbook-1.9.0/pretix_passbook/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7457 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1322 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.531206 pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4973 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      959 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.531206 pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7482 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1352 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.535205 pretix-passbook-1.9.0/pretix_passbook/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6886 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pl/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1359 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.499206 pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.535205 pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4979 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      965 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.535205 pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5230 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1338 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.535205 pretix-passbook-1.9.0/pretix_passbook/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8338 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ru/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.535205 pretix-passbook-1.9.0/pretix_passbook/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4970 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/sl/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/pretix_passbook/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5190 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/sv/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      956 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/pretix_passbook/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7250 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/tr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1333 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/tr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5205 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     1253 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/LC_MESSAGES/djangojs.po
--rw-rw-rw-   0 root         (0) root         (0)    15428 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/passbook.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.503206 pretix-passbook-1.9.0/pretix_passbook/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/pretix_passbook/static/pretix_passbook/
--rw-rw-rw-   0 root         (0) root         (0)     1936 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/static/pretix_passbook/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     3599 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/pretix_passbook/static/pretix_passbook/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-27 14:24:31.515206 pretix-passbook-1.9.0/pretix_passbook.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2926 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2835 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-08-27 14:24:31.000000 pretix-passbook-1.9.0/pretix_passbook.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      372 2021-08-27 14:24:31.539205 pretix-passbook-1.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1024 2021-08-27 14:22:53.000000 pretix-passbook-1.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.004233 pretix-passbook-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      132 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2926 2021-11-29 10:35:15.004233 pretix-passbook-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.992234 pretix-passbook-1.9.1/pretix_passbook/
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.992234 pretix-passbook-1.9.1/pretix_passbook/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.984234 pretix-passbook-1.9.1/pretix_passbook/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.992234 pretix-passbook-1.9.1/pretix_passbook/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ar/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.984234 pretix-passbook-1.9.1/pretix_passbook/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.992234 pretix-passbook-1.9.1/pretix_passbook/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ca/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.984234 pretix-passbook-1.9.1/pretix_passbook/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/cs/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.984234 pretix-passbook-1.9.1/pretix_passbook/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/da/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7422 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)      981 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/djangojs.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/el/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7459 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5196 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5191 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/it/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.996234 pretix-passbook-1.9.1/pretix_passbook/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/lv/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7457 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      959 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7482 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6886 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4979 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      965 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5230 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ru/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/sl/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/sv/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      956 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.000234 pretix-passbook-1.9.1/pretix_passbook/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7250 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/tr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/tr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.004233 pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 root         (0) root         (0)    15456 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/passbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.988234 pretix-passbook-1.9.1/pretix_passbook/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:15.004233 pretix-passbook-1.9.1/pretix_passbook/static/pretix_passbook/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/static/pretix_passbook/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/pretix_passbook/static/pretix_passbook/logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-29 10:35:14.992234 pretix-passbook-1.9.1/pretix_passbook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2926 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2835 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2021-11-29 10:35:14.000000 pretix-passbook-1.9.1/pretix_passbook.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      372 2021-11-29 10:35:15.004233 pretix-passbook-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2021-11-29 10:33:54.000000 pretix-passbook-1.9.1/setup.py
```

### Comparing `pretix-passbook-1.9.0/LICENSE` & `pretix-passbook-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/PKG-INFO` & `pretix-passbook-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-passbook
-Version: 1.9.0
+Version: 1.9.1
 Summary: Passbook tickets for pretix
 Home-page: https://github.com/pretix/pretix-passbook
 Author: Tobias Kunze
 Author-email: rixx@cutebit.de
 License: Apache License 2.0
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `pretix-passbook-1.9.0/README.rst` & `pretix-passbook-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/__init__.py` & `pretix-passbook-1.9.1/pretix_passbook/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     class PretixPluginMeta:
         name = gettext_lazy('Passbook Tickets')
         author = 'Tobias Kunze, Raphael Michel'
         description = gettext_lazy('Provides passbook tickets for pretix')
         category = 'FORMAT'
         visible = True
-        version = '1.9.0'
+        version = '1.9.1'
 
     def ready(self):
         from . import signals  # NOQA
 
     @cached_property
     def compatibility_errors(self):
         import shutil
```

### Comparing `pretix-passbook-1.9.0/pretix_passbook/forms.py` & `pretix-passbook-1.9.1/pretix_passbook/forms.py`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ar/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ar/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ca/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ca/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/cs/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/cs/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/da/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/da/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/de/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/de/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/de_Informal/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/de_Informal/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/django.pot` & `pretix-passbook-1.9.1/pretix_passbook/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/djangojs.pot` & `pretix-passbook-1.9.1/pretix_passbook/locale/djangojs.pot`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/el/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/el/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/es/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/es/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/fr/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/fr/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/it/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/it/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/lv/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/lv/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl_BE/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl_BE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/nl_Informal/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/nl_Informal/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pl/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pl/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pl_Informal/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pl_Informal/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/pt_BR/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ru/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/ru/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/sl/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/sl/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/sv/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/sv/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/tr/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/tr/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/tr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `pretix-passbook-1.9.1/pretix_passbook/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/passbook.py` & `pretix-passbook-1.9.1/pretix_passbook/passbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,16 @@
                 card.addBackField('doorsClose', ev.get_date_to_display(tz, short=True), gettext('To'))
             else:
                 card.addAuxiliaryField('doorsClose', ev.get_date_to_display(tz, short=True), gettext('To'))
 
         if order_position.attendee_name:
             card.addBackField('name', order_position.attendee_name, gettext('Attendee name'))
 
-        card.addBackField('email', order.email, gettext('Ordered by'))
+        if order.email:
+            card.addBackField('email', order.email, gettext('Ordered by'))
         card.addBackField('organizer', str(order.event.organizer), gettext('Organizer'))
         if order.event.settings.contact_mail:
             card.addBackField('organizerContact', order.event.settings.contact_mail, gettext('Organizer contact'))
         card.addBackField('orderCode', order.code, gettext('Order code'))
 
         if order_position.subevent:
             card.addBackField('website', build_absolute_uri(order.event, 'presale:event.index', {
```

### Comparing `pretix-passbook-1.9.0/pretix_passbook/signals.py` & `pretix-passbook-1.9.1/pretix_passbook/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/static/pretix_passbook/icon.png` & `pretix-passbook-1.9.1/pretix_passbook/static/pretix_passbook/icon.png`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook/static/pretix_passbook/logo.png` & `pretix-passbook-1.9.1/pretix_passbook/static/pretix_passbook/logo.png`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/pretix_passbook.egg-info/PKG-INFO` & `pretix-passbook-1.9.1/pretix_passbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-passbook
-Version: 1.9.0
+Version: 1.9.1
 Summary: Passbook tickets for pretix
 Home-page: https://github.com/pretix/pretix-passbook
 Author: Tobias Kunze
 Author-email: rixx@cutebit.de
 License: Apache License 2.0
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `pretix-passbook-1.9.0/pretix_passbook.egg-info/SOURCES.txt` & `pretix-passbook-1.9.1/pretix_passbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-passbook-1.9.0/setup.py` & `pretix-passbook-1.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 cmdclass = {
     'build': CustomBuild
 }
 
 
 setup(
     name='pretix-passbook',
-    version='1.9.0',
+    version='1.9.1',
     description='Passbook tickets for pretix',
     long_description=long_description,
     url='https://github.com/pretix/pretix-passbook',
     author='Tobias Kunze',
     author_email='rixx@cutebit.de',
     license='Apache License 2.0',
```


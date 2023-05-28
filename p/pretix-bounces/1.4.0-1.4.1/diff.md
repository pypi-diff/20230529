# Comparing `tmp/pretix-bounces-1.4.0.tar.gz` & `tmp/pretix-bounces-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-bounces-1.4.0.tar", last modified: Mon Jan 30 15:03:50 2023, max compression
+gzip compressed data, was "pretix-bounces-1.4.1.tar", last modified: Sun May 28 23:05:32 2023, max compression
```

## Comparing `pretix-bounces-1.4.0.tar` & `pretix-bounces-1.4.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2048 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1728 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.860995 pretix-bounces-1.4.0/pretix_bounces/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.860995 pretix-bounces-1.4.0/pretix_bounces/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.860995 pretix-bounces-1.4.0/pretix_bounces/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.864995 pretix-bounces-1.4.0/pretix_bounces/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.864995 pretix-bounces-1.4.0/pretix_bounces/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      879 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      935 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      933 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      919 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.880996 pretix-bounces-1.4.0/pretix_bounces/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/migrations/0002_auto_20190830_0932.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/migrations/0003_mailalias_customer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5478 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/static/pretix_bounces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/static/pretix_bounces/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.888996 pretix-bounces-1.4.0/pretix_bounces/templates/pretix_bounces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/templates/pretix_bounces/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/pretix_bounces/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:03:50.884996 pretix-bounces-1.4.0/pretix_bounces.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2048 2023-01-30 15:03:50.000000 pretix-bounces-1.4.0/pretix_bounces.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2031 2023-01-30 15:03:50.000000 pretix-bounces-1.4.0/pretix_bounces.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 15:03:50.000000 pretix-bounces-1.4.0/pretix_bounces.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-01-30 15:03:50.000000 pretix-bounces-1.4.0/pretix_bounces.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-30 15:03:50.000000 pretix-bounces-1.4.0/pretix_bounces.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-01-30 15:03:50.892996 pretix-bounces-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-01-30 14:58:21.000000 pretix-bounces-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.312586 pretix-bounces-1.4.1/pretix_bounces/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.312586 pretix-bounces-1.4.1/pretix_bounces/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.312586 pretix-bounces-1.4.1/pretix_bounces/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:03.000000 pretix-bounces-1.4.1/pretix_bounces/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.316586 pretix-bounces-1.4.1/pretix_bounces/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.304585 pretix-bounces-1.4.1/pretix_bounces/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      879 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.320586 pretix-bounces-1.4.1/pretix_bounces/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      935 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.324586 pretix-bounces-1.4.1/pretix_bounces/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/pretix_bounces/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/pretix_bounces/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/migrations/0002_auto_20190830_0932.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/migrations/0003_mailalias_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:03.000000 pretix-bounces-1.4.1/pretix_bounces/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5478 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/pretix_bounces/static/pretix_bounces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:03.000000 pretix-bounces-1.4.1/pretix_bounces/static/pretix_bounces/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.308586 pretix-bounces-1.4.1/pretix_bounces/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.328586 pretix-bounces-1.4.1/pretix_bounces/templates/pretix_bounces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:05:03.000000 pretix-bounces-1.4.1/pretix_bounces/templates/pretix_bounces/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pretix_bounces/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:05:32.312586 pretix-bounces-1.4.1/pretix_bounces.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-05-28 23:05:32.000000 pretix-bounces-1.4.1/pretix_bounces.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-05-28 23:05:32.000000 pretix-bounces-1.4.1/pretix_bounces.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:05:32.000000 pretix-bounces-1.4.1/pretix_bounces.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-28 23:05:32.000000 pretix-bounces-1.4.1/pretix_bounces.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-28 23:05:32.000000 pretix-bounces-1.4.1/pretix_bounces.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-05-28 23:05:32.332586 pretix-bounces-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:31:31.000000 pretix-bounces-1.4.1/setup.py
```

### Comparing `pretix-bounces-1.4.0/LICENSE` & `pretix-bounces-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/PKG-INFO` & `pretix-bounces-1.4.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-bounces
-Version: 1.4.0
-Summary: Allows automatic processing of bounces or automatic replies to emails sent by pretix.
-Home-page: https://github.com/pretix/pretix-bounces
-Author: Raphael Michel
-Author-email: mail@raphaelmichel.de
-License: Apache Software License
-License-File: LICENSE
-
 Bounce processing for pretix
 ============================
 
 This is a plugin for `pretix`_. Once installed and configured, it makes pretix use random ``Sender`` headers
 for emails like ``noreply-amCwRFatawEjetS8@pretix.eu`` for outgoing emails. The ``From`` and ``Reply-To``
 headers remain untouched. It then periodically checks for emails in a specified IMAP inbox and adds replied
 emails to the log of an order. This leads to an automatic logging of bounces on pretix-level.
@@ -36,15 +26,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-bounces``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-bounces-1.4.0/pretix_bounces/apps.py` & `pretix-bounces-1.4.1/pretix_bounces/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/ar/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/ca/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/cs/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/pt/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-03-06 16:53+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bounces/signals.py:79
 msgid "An email reply has been received by the user."
 msgstr ""
```

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/da/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/django.pot` & `pretix-bounces-1.4.1/pretix_bounces/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/el/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/es/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/fi/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/fr/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/hr/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/it/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/ja/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/lv/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/nl/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/pl/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/pt/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-03-06 16:53+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: pt\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bounces/signals.py:79
 msgid "An email reply has been received by the user."
 msgstr ""
```

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/ru/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/sv/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-03-06 16:53+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ru\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_bounces/signals.py:79
 msgid "An email reply has been received by the user."
 msgstr ""
```

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/si/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/sl/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/tr/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-bounces-1.4.1/pretix_bounces/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/migrations/0001_initial.py` & `pretix-bounces-1.4.1/pretix_bounces/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/migrations/0002_auto_20190830_0932.py` & `pretix-bounces-1.4.1/pretix_bounces/migrations/0002_auto_20190830_0932.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/migrations/0003_mailalias_customer.py` & `pretix-bounces-1.4.1/pretix_bounces/migrations/0003_mailalias_customer.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/signals.py` & `pretix-bounces-1.4.1/pretix_bounces/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces/utils.py` & `pretix-bounces-1.4.1/pretix_bounces/utils.py`

 * *Files identical despite different names*

### Comparing `pretix-bounces-1.4.0/pretix_bounces.egg-info/PKG-INFO` & `pretix-bounces-1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 Metadata-Version: 2.1
 Name: pretix-bounces
-Version: 1.4.0
+Version: 1.4.1
 Summary: Allows automatic processing of bounces or automatic replies to emails sent by pretix.
-Home-page: https://github.com/pretix/pretix-bounces
-Author: Raphael Michel
-Author-email: mail@raphaelmichel.de
-License: Apache Software License
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: Copyright 2017 Raphael Michel
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
+Project-URL: homepage, https://github.com/pretix/pretix-bounces
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Bounce processing for pretix
 ============================
 
 This is a plugin for `pretix`_. Once installed and configured, it makes pretix use random ``Sender`` headers
 for emails like ``noreply-amCwRFatawEjetS8@pretix.eu`` for outgoing emails. The ``From`` and ``Reply-To``
@@ -36,15 +52,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-bounces``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-bounces-1.4.0/pretix_bounces.egg-info/SOURCES.txt` & `pretix-bounces-1.4.1/pretix_bounces.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_bounces/__init__.py
 pretix_bounces/apps.py
 pretix_bounces/models.py
 pretix_bounces/signals.py
 pretix_bounces/utils.py
```

### Comparing `pretix-bounces-1.4.0/setup.cfg` & `pretix-bounces-1.4.1/setup.cfg`

 * *Files identical despite different names*


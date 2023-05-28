# Comparing `tmp/pretix-sepadebit-2.4.0.post1.tar.gz` & `tmp/pretix-sepadebit-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sepadebit-2.4.0.post1.tar", last modified: Thu Apr 27 16:32:58 2023, max compression
+gzip compressed data, was "pretix-sepadebit-2.4.1.tar", last modified: Sun May 28 23:25:54 2023, max compression
```

## Comparing `pretix-sepadebit-2.4.0.post1.tar` & `pretix-sepadebit-2.4.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)   109251 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/bicdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15987 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16372 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16052 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23666 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    23666 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    15738 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16269 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16075 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16034 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16032 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.741506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16132 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24127 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15716 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    24357 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16508 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15722 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16025 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15963 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16039 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16095 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    16063 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0006_sepaexport_currency.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0007_sepaduedate.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/models.py
--rw-rw-rw-   0 root         (0) root         (0)    19281 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     9441 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.753507 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.745506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/control.html
--rw-rw-rw-   0 root         (0) root         (0)     5782 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/export.html
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
--rw-rw-rw-   0 root         (0) root         (0)     3400 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/orders.html
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/pending.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/test_payment.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    12651 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:32:58.749506 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2014 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3070 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-27 16:32:58.000000 pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-04-27 16:32:58.757506 pretix-sepadebit-2.4.0.post1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-27 16:32:34.000000 pretix-sepadebit-2.4.0.post1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.990635 pretix-sepadebit-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-28 23:25:54.990635 pretix-sepadebit-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.934633 pretix-sepadebit-2.4.1/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)   109251 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/bicdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.934633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15987 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16372 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15982 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16052 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    23675 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.938633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    23684 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    15738 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.942633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.946633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16269 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.946633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16075 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.910633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.946633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16060 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.946633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.946633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16030 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.950634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.950634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16132 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.950634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24127 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.950634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15716 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    24357 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16508 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15722 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16025 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.954634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15713 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.914633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.958634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15963 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.958634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.962634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16039 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.966634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16095 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.982634 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    16063 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.986635 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0004_sepaexport_testmode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0006_sepaexport_currency.py
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0007_sepaduedate.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    19281 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     9441 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.986635 pretix-sepadebit-2.4.1/pretix_sepadebit/static/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/static/pretix_sepadebit/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.918633 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.990635 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     5782 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/export.html
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/mail.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/orders.html
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/pending.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.990635 pretix-sepadebit-2.4.1/pretix_sepadebit/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/tests/test_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    12651 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pretix_sepadebit/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:25:54.934633 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-28 23:25:54.000000 pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-28 23:25:54.990635 pretix-sepadebit-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 23:25:22.000000 pretix-sepadebit-2.4.1/setup.py
```

### Comparing `pretix-sepadebit-2.4.0.post1/LICENSE` & `pretix-sepadebit-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/PKG-INFO` & `pretix-sepadebit-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sepadebit
-Version: 2.4.0.post1
+Version: 2.4.1
 Summary: This plugin adds SEPA direct debit support to pretix
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-sepadebit-2.4.0.post1/README.rst` & `pretix-sepadebit-2.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/apps.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     class PretixPluginMeta:
         name = gettext_lazy('SEPA Direct debit')
         category = 'PAYMENT'
         author = 'Raphael Michel'
         description = gettext_lazy('This plugin adds SEPA direct debit support to pretix')
         visible = True
         version = __version__
-        compatibility = "pretix>=4.16.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/bicdata.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/bicdata.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/exporters.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/exporters.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-02-07 11:16+0100\n"
-"Last-Translator: Raphael Michel <michel@rami.io>\n"
-"Language-Team: German <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/de/>\n"
+"PO-Revision-Date: 2023-05-16 20:00+0000\n"
+"Last-Translator: Moritz Lerch <dev@moritz-lerch.de>\n"
+"Language-Team: German <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sepadebit/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Poedit 3.2.2\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr "SEPA-Bankeinzug"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -272,15 +272,15 @@
 "used."
 msgstr ""
 "Die Felder für die E-Mail-Inhalte der Vorabinformation sind verpflichtend "
 "auszufüllen, wenn das früheste Einzugsdatum verwendet wird."
 
 #: pretix_sepadebit/payment.py:244
 msgid "Account holder"
-msgstr "Kontoinhaber"
+msgstr "Kontoinhaber*in"
 
 #: pretix_sepadebit/payment.py:245
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
 #: pretix_sepadebit/payment.py:246
@@ -464,15 +464,15 @@
 msgstr ""
 "Diese Bestellung sollte per SEPA-Lastschrift bezahlt werden, wurde aber "
 "entweder wieder als unbezahlt markiert oder konnte nie als bezahlt markiert "
 "werden."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:34
 msgid "Account name"
-msgstr "Kontoinhaber"
+msgstr "Kontoinhaber*in"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:36
 msgid "Mandate reference"
 msgstr "Mandatsrefernz"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:38
 msgid "Due date"
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2023-02-07 11:16+0100\n"
-"Last-Translator: Raphael Michel <michel@rami.io>\n"
+"PO-Revision-Date: 2023-05-16 20:00+0000\n"
+"Last-Translator: Moritz Lerch <dev@moritz-lerch.de>\n"
 "Language-Team: German (informal) <https://translate.pretix.eu/projects/"
 "pretix/pretix-plugin-sepadebit/de_Informal/>\n"
-"Language: de\n"
+"Language: de_Informal\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Poedit 3.2.2\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr "SEPA-Bankeinzug"
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -272,15 +272,15 @@
 "used."
 msgstr ""
 "Die Felder für die E-Mail-Inhalte der Vorabinformation sind verpflichtend "
 "auszufüllen, wenn das früheste Einzugsdatum verwendet wird."
 
 #: pretix_sepadebit/payment.py:244
 msgid "Account holder"
-msgstr "Kontoinhaber"
+msgstr "Kontoinhaber*in"
 
 #: pretix_sepadebit/payment.py:245
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
 msgstr "IBAN"
 
 #: pretix_sepadebit/payment.py:246
@@ -464,15 +464,15 @@
 msgstr ""
 "Diese Bestellung sollte per SEPA-Lastschrift bezahlt werden, wurde aber "
 "entweder wieder als unbezahlt markiert oder konnte nie als bezahlt markiert "
 "werden."
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:34
 msgid "Account name"
-msgstr "Kontoinhaber"
+msgstr "Kontoinhaber*in"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:36
 msgid "Mandate reference"
 msgstr "Mandatsrefernz"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:38
 msgid "Due date"
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/django.pot` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2022-08-04 06:00+0000\n"
-"Last-Translator: Guy Foetz <guy.foetz@lereveil.lu>\n"
-"Language-Team: French <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/fr/>\n"
+"PO-Revision-Date: 2023-04-06 22:00+0000\n"
+"Last-Translator: Loïc Alejandro <loic.alejandro@e.email>\n"
+"Language-Team: French <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sepadebit/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -60,15 +60,15 @@
 #: pretix_sepadebit/exporters.py:24
 msgid "SEPA export date"
 msgstr ""
 
 #: pretix_sepadebit/exporters.py:24
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr ""
+msgstr "Montant du paiement"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2020-06-24 15:00+0000\n"
-"Last-Translator: Frank <webappconcept@gmail.com>\n"
-"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/it/>\n"
+"PO-Revision-Date: 2023-05-18 00:00+0000\n"
+"Last-Translator: M C <micasadmail@gmail.com>\n"
+"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sepadebit/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.10.3\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -233,15 +233,15 @@
 #: pretix_sepadebit/payment.py:244
 msgid "Account holder"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:245
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr ""
+msgstr "IBAN"
 
 #: pretix_sepadebit/payment.py:246
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:248
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ja/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ja\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/ru/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: ru\n"
+"PO-Revision-Date: 2021-03-01 23:24+0000\n"
+"Last-Translator: lapor-kris <kristijan.tkalec@posteo.si>\n"
+"Language-Team: Slovenian <https://translate.pretix.eu/projects/pretix/pretix-"
+"plugin-sepadebit/sl/>\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3;\n"
+"X-Generator: Weblate 4.4.2\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -488,15 +492,15 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr ""
+msgstr "Plačilo"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sl/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-02-07 11:16+0100\n"
-"PO-Revision-Date: 2021-03-01 23:24+0000\n"
-"Last-Translator: lapor-kris <kristijan.tkalec@posteo.si>\n"
-"Language-Team: Slovenian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sepadebit/sl/>\n"
-"Language: sl\n"
+"PO-Revision-Date: 2023-03-26 05:00+0000\n"
+"Last-Translator: Michael <michael.happl@gmx.at>\n"
+"Language-Team: Czech <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sepadebit/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
-"n%100==4 ? 2 : 3;\n"
-"X-Generator: Weblate 4.4.2\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: pretix_sepadebit/apps.py:11
 msgid "SEPA Direct debit"
 msgstr ""
 
 #: pretix_sepadebit/apps.py:14
 msgid "This plugin adds SEPA direct debit support to pretix"
@@ -59,15 +58,15 @@
 #: pretix_sepadebit/exporters.py:24
 msgid "SEPA export date"
 msgstr ""
 
 #: pretix_sepadebit/exporters.py:24
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:36
 msgid "Payment amount"
-msgstr ""
+msgstr "Částka platby"
 
 #: pretix_sepadebit/payment.py:36
 msgid ""
 "Direct debit is not allowed for this IBAN, please get in touch with the "
 "event organizer or choose a different payment method."
 msgstr ""
 
@@ -91,15 +90,15 @@
 "Test mode payments will only be debited if you submit a file created in test "
 "mode to your bank."
 msgstr ""
 
 #: pretix_sepadebit/payment.py:83
 #, python-brace-format
 msgid "Available placeholders: {list}"
-msgstr ""
+msgstr "Dostupné zástupné symboly: {list}"
 
 #: pretix_sepadebit/payment.py:96
 msgid ""
 "I have understood that I need to regularly create SEPA XML export files and "
 "transfer them to my bank in order to have my bank collect the customer "
 "payments."
 msgstr ""
@@ -227,25 +226,25 @@
 msgid ""
 "Due date reminder email fields are required if earliest due date feature is "
 "used."
 msgstr ""
 
 #: pretix_sepadebit/payment.py:244
 msgid "Account holder"
-msgstr ""
+msgstr "Majitel účtu"
 
 #: pretix_sepadebit/payment.py:245
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:30
 msgid "IBAN"
-msgstr ""
+msgstr "IBAN"
 
 #: pretix_sepadebit/payment.py:246
 #: pretix_sepadebit/templates/pretix_sepadebit/control.html:32
 msgid "BIC"
-msgstr ""
+msgstr "BIC"
 
 #: pretix_sepadebit/payment.py:248
 msgid "I hereby grant the SEPA direct debit mandate for this order (see below)"
 msgstr ""
 
 #: pretix_sepadebit/payment.py:410
 msgid "will be debited"
@@ -492,15 +491,15 @@
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:32
 msgid "Order"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:33
 msgid "Payment"
-msgstr "Plačilo"
+msgstr "Platba"
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:34
 msgid "Mandate date"
 msgstr ""
 
 #: pretix_sepadebit/templates/pretix_sepadebit/orders.html:35
 msgid "Associated invoices"
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-sepadebit-2.4.1/pretix_sepadebit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0001_initial.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0002_auto_20170530_1527.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0003_sepaexportorder_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0005_auto_20190429_0811.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0007_sepaduedate.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0007_sepaduedate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Generated by Django 3.0.14 on 2021-04-22 20:47
 
 import django.db.models.deletion
 import json
-from datetime import date, datetime, tzinfo
+from datetime import datetime, timezone
 from django.db import migrations, models
-from django.utils.timezone import utc
-from pytz import timezone
 
 
 def roll_forwards(apps, schema_editor):
     OrderPayment = apps.get_model('pretixbase', 'OrderPayment')
     SepaDueDate = apps.get_model('pretix_sepadebit', 'SepaDueDate')
 
     create_sepaduedate_instances(OrderPayment, SepaDueDate)
@@ -50,15 +48,15 @@
 def create_sepaduedate_instances(OrderPayment, SepaDueDate):
     for op in OrderPayment.objects.filter(provider='sepadebit').filter(info__isnull=False):
         # prevents dependency from the info_data property
         op_info_data = json.loads(op.info)
 
         # either use provided remind_after value or date and add a ts to it
         r_a=getattr(op_info_data,'remind_after', op_info_data['date'])
-        remind_after=utc.localize(datetime.strptime(r_a, '%Y-%m-%d'))
+        remind_after=timezone.utc.localize(datetime.strptime(r_a, '%Y-%m-%d'))
 
         due_date = SepaDueDate(date=op_info_data['date'], reminded=getattr(op_info_data,'reminded', True), remind_after=remind_after)
         due_date.payment = op
         due_date.save()
         del op_info_data['date']
         op.info = json.dumps(op_info_data, sort_keys=True)
         op.save()
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/migrations/0008_alter_sepaduedate_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/models.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/models.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/payment.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/signals.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html` & `pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_confirm.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html` & `pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/control.html` & `pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/export.html` & `pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/export.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/templates/pretix_sepadebit/orders.html` & `pretix-sepadebit-2.4.1/pretix_sepadebit/templates/pretix_sepadebit/orders.html`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/tests/test_payment.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/urls.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit/views.py` & `pretix-sepadebit-2.4.1/pretix_sepadebit/views.py`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/PKG-INFO` & `pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-sepadebit
-Version: 2.4.0.post1
+Version: 2.4.1
 Summary: This plugin adds SEPA direct debit support to pretix
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2017 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-sepadebit-2.4.0.post1/pretix_sepadebit.egg-info/SOURCES.txt` & `pretix-sepadebit-2.4.1/pretix_sepadebit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-sepadebit-2.4.0.post1/pyproject.toml` & `pretix-sepadebit-2.4.1/pyproject.toml`

 * *Files identical despite different names*


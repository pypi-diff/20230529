# Comparing `tmp/pretix-mollie-1.5.2.tar.gz` & `tmp/pretix-mollie-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mollie-1.5.2.tar", last modified: Tue Mar 28 08:15:15 2023, max compression
+gzip compressed data, was "pretix-mollie-1.5.3.tar", last modified: Sun May 28 23:08:30 2023, max compression
```

## Comparing `pretix-mollie-1.5.2.tar` & `pretix-mollie-1.5.3.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.572968 pretix-mollie-1.5.2/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1193 2023-03-28 08:15:15.572968 pretix-mollie-1.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.540967 pretix-mollie-1.5.2/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    12020 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15783 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    10733 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11506 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11735 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15802 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10711 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.548967 pretix-mollie-1.5.2/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15845 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.532967 pretix-mollie-1.5.2/pretix_mollie/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10969 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10717 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.552968 pretix-mollie-1.5.2/pretix_mollie/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.564968 pretix-mollie-1.5.2/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11446 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    26131 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.568968 pretix-mollie-1.5.2/pretix_mollie/static/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/static/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/static/pretix_mollie/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.536967 pretix-mollie-1.5.2/pretix_mollie/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.572968 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/control.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/order_pending.txt
--rw-rw-rw-   0 root         (0) root         (0)     4832 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14737 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/pretix_mollie/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:15:15.544968 pretix-mollie-1.5.2/pretix_mollie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1193 2023-03-28 08:15:15.000000 pretix-mollie-1.5.2/pretix_mollie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-28 08:15:15.000000 pretix-mollie-1.5.2/pretix_mollie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 08:15:15.000000 pretix-mollie-1.5.2/pretix_mollie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-28 08:15:15.000000 pretix-mollie-1.5.2/pretix_mollie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-28 08:15:15.000000 pretix-mollie-1.5.2/pretix_mollie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-28 08:15:15.572968 pretix-mollie-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-03-28 08:14:30.000000 pretix-mollie-1.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.456963 pretix-mollie-1.5.3/pretix_mollie/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.456963 pretix-mollie-1.5.3/pretix_mollie/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15783 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    10733 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11506 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15802 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10711 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15845 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10969 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10717 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.460963 pretix-mollie-1.5.3/pretix_mollie/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11446 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    26131 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:08:00.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/order_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14737 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pretix_mollie/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:08:30.464963 pretix-mollie-1.5.3/pretix_mollie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:08:30.000000 pretix-mollie-1.5.3/pretix_mollie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-28 23:08:30.480964 pretix-mollie-1.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:46:57.000000 pretix-mollie-1.5.3/setup.py
```

### Comparing `pretix-mollie-1.5.2/LICENSE` & `pretix-mollie-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/PKG-INFO` & `pretix-mollie-1.5.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-Metadata-Version: 2.1
-Name: pretix-mollie
-Version: 1.5.2
-Summary: Integration for the Mollie payment provider.
-Home-page: https://github.com/pretix/pretix-mollie
-Author: Raphael Michel
-Author-email: michel@rami.io
-License: Apache Software License
-License-File: LICENSE
-
 Mollie payment integration for pretix
 =====================================
 
 This is a plugin for `pretix`_. 
 
 Development setup
 -----------------
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-mollie``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-mollie-1.5.2/pretix_mollie/apps.py` & `pretix-mollie-1.5.3/pretix_mollie/apps.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,13 +13,13 @@
         description = gettext_lazy('Accept payments through Mollie, a European payment provider supporting '
                                    'credit cards as well as many local payment methods such as giropay, '
                                    'direct debit, iDEAL, wire transfers, and many more.')
         picture = "pretix_mollie/logo.svg"
         category = 'PAYMENT'
         visible = True
         version = __version__
-        compatibility = "pretix>=4.16.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-mollie-1.5.2/pretix_mollie/forms.py` & `pretix-mollie-1.5.3/pretix_mollie/forms.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/ca/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/de/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/django.pot` & `pretix-mollie-1.5.3/pretix_mollie/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/el/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/fi/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/ja/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/lv/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/nl/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/pl/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/pt/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/ru/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/si/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/sl/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/sv/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-mollie-1.5.3/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/payment.py` & `pretix-mollie-1.5.3/pretix_mollie/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/signals.py` & `pretix-mollie-1.5.3/pretix_mollie/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/static/pretix_mollie/logo.svg` & `pretix-mollie-1.5.3/pretix_mollie/static/pretix_mollie/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/control.html` & `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/control.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/pending.html` & `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/templates/pretix_mollie/redirect.html` & `pretix-mollie-1.5.3/pretix_mollie/templates/pretix_mollie/redirect.html`

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

### Comparing `pretix-mollie-1.5.2/pretix_mollie/urls.py` & `pretix-mollie-1.5.3/pretix_mollie/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/utils.py` & `pretix-mollie-1.5.3/pretix_mollie/utils.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie/views.py` & `pretix-mollie-1.5.3/pretix_mollie/views.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.5.2/pretix_mollie.egg-info/SOURCES.txt` & `pretix-mollie-1.5.3/pretix_mollie.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_mollie/__init__.py
 pretix_mollie/apps.py
 pretix_mollie/forms.py
 pretix_mollie/payment.py
 pretix_mollie/signals.py
```


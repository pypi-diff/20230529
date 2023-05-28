# Comparing `tmp/pretix-oppwa-1.1.1.tar.gz` & `tmp/pretix-oppwa-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-oppwa-1.1.1.tar", last modified: Tue Jan 31 09:53:23 2023, max compression
+gzip compressed data, was "pretix-oppwa-1.1.2.tar", last modified: Sun May 28 23:11:56 2023, max compression
```

## Comparing `pretix-oppwa-1.1.1.tar` & `pretix-oppwa-1.1.2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1227 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_hobex/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/pretix_hobex/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_hobex/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.545698 pretix-oppwa-1.1.1/pretix_hobex/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_hobex/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.545698 pretix-oppwa-1.1.1/pretix_hobex/locale/de_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_hobex/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/payment.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.545698 pretix-oppwa-1.1.1/pretix_hobex/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_hobex/static/pretix_hobex/
--rw-rw-rw-   0 root         (0) root         (0)     6117 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/static/pretix_hobex/logo.png
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_hobex/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.553698 pretix-oppwa-1.1.1/pretix_oppwa/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/pretix_oppwa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/pretix_oppwa/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.545698 pretix-oppwa-1.1.1/pretix_oppwa/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17451 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17409 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    16405 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)    16548 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/payment.py
--rw-rw-rw-   0 root         (0) root         (0)    26744 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.549698 pretix-oppwa-1.1.1/pretix_oppwa/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa/static/pretix_oppwa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/static/pretix_oppwa/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.549698 pretix-oppwa-1.1.1/pretix_oppwa/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/control.html
--rw-rw-rw-   0 root         (0) root         (0)     1395 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/pay.html
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/pending.html
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5400 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_oppwa/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.557698 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1227 2023-01-31 09:53:23.000000 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1566 2023-01-31 09:53:23.000000 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 09:53:23.000000 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-01-31 09:53:23.000000 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-01-31 09:53:23.000000 pretix-oppwa-1.1.1/pretix_oppwa.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_vrpay/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/pretix_vrpay/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_vrpay/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.549698 pretix-oppwa-1.1.1/pretix_vrpay/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_vrpay/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.549698 pretix-oppwa-1.1.1/pretix_vrpay/locale/de_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_vrpay/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      946 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/locale/django.pot
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/payment.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.549698 pretix-oppwa-1.1.1/pretix_vrpay/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:53:23.561698 pretix-oppwa-1.1.1/pretix_vrpay/static/pretix_vrpay/
--rw-rw-rw-   0 root         (0) root         (0)     8856 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/static/pretix_vrpay/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-01-31 09:50:11.000000 pretix-oppwa-1.1.1/pretix_vrpay/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-01-31 09:53:23.565698 pretix-oppwa-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-01-31 09:52:42.000000 pretix-oppwa-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_hobex/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_hobex/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.546028 pretix-oppwa-1.1.2/pretix_hobex/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_hobex/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.546028 pretix-oppwa-1.1.2/pretix_hobex/locale/de_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_hobex/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_hobex/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_hobex/static/pretix_hobex/
+-rw-rw-rw-   0 root         (0) root         (0)     6117 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/static/pretix_hobex/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_hobex/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.554028 pretix-oppwa-1.1.2/pretix_oppwa/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.558028 pretix-oppwa-1.1.2/pretix_oppwa/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_oppwa/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.558028 pretix-oppwa-1.1.2/pretix_oppwa/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17451 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.558028 pretix-oppwa-1.1.2/pretix_oppwa/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.558028 pretix-oppwa-1.1.2/pretix_oppwa/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    17409 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    16405 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)    16548 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)    26744 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_oppwa/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_oppwa/static/pretix_oppwa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/static/pretix_oppwa/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_oppwa/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/pay.html
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     5400 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_oppwa/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.558028 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-05-28 23:11:56.000000 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-05-28 23:11:56.000000 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:11:56.000000 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2023-05-28 23:11:56.000000 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-28 23:11:56.000000 pretix-oppwa-1.1.2/pretix_oppwa.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_vrpay/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_vrpay/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_vrpay/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_vrpay/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_vrpay/locale/de_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_vrpay/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.550028 pretix-oppwa-1.1.2/pretix_vrpay/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/pretix_vrpay/static/pretix_vrpay/
+-rw-rw-rw-   0 root         (0) root         (0)     8856 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/static/pretix_vrpay/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pretix_vrpay/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-28 23:11:56.562029 pretix-oppwa-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 23:11:32.000000 pretix-oppwa-1.1.2/setup.py
```

### Comparing `pretix-oppwa-1.1.1/LICENSE` & `pretix-oppwa-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/PKG-INFO` & `pretix-oppwa-1.1.2/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-oppwa
-Version: 1.1.1
-Summary: This plugin allows you to use OPPWA based payment providers
-Home-page: https://github.com/pretix/pretix-oppwa/
-Author: pretix Team
-Author-email: support@pretix.eu
-License: Apache
-License-File: LICENSE
-
 OPPWA payments for pretix
 ==========================
 
 This is a plugin for `pretix`_. 
 
 This plugin allows you to use OPPWA based payment providers
 
@@ -20,15 +10,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-oppwa``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/apps.py` & `pretix-oppwa-1.1.2/pretix_hobex/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/locale/de/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_hobex/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_hobex/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/locale/django.pot` & `pretix-oppwa-1.1.2/pretix_hobex/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/payment.py` & `pretix-oppwa-1.1.2/pretix_hobex/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/paymentmethods.py` & `pretix-oppwa-1.1.2/pretix_hobex/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/signals.py` & `pretix-oppwa-1.1.2/pretix_hobex/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_hobex/static/pretix_hobex/logo.png` & `pretix-oppwa-1.1.2/pretix_hobex/static/pretix_hobex/logo.png`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/apps.py` & `pretix-oppwa-1.1.2/pretix_oppwa/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/locale/de/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_oppwa/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_oppwa/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/locale/django.pot` & `pretix-oppwa-1.1.2/pretix_oppwa/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/payment.py` & `pretix-oppwa-1.1.2/pretix_oppwa/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/paymentmethods.py` & `pretix-oppwa-1.1.2/pretix_oppwa/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/signals.py` & `pretix-oppwa-1.1.2/pretix_oppwa/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/control.html` & `pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/control.html`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/pay.html` & `pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/pay.html`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/templates/pretix_oppwa/pending.html` & `pretix-oppwa-1.1.2/pretix_oppwa/templates/pretix_oppwa/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/urls.py` & `pretix-oppwa-1.1.2/pretix_oppwa/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa/views.py` & `pretix-oppwa-1.1.2/pretix_oppwa/views.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_oppwa.egg-info/SOURCES.txt` & `pretix-oppwa-1.1.2/pretix_oppwa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_hobex/__init__.py
 pretix_hobex/apps.py
 pretix_hobex/payment.py
 pretix_hobex/paymentmethods.py
 pretix_hobex/signals.py
```

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/apps.py` & `pretix-oppwa-1.1.2/pretix_vrpay/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/locale/de/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_vrpay/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-oppwa-1.1.2/pretix_vrpay/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/locale/django.pot` & `pretix-oppwa-1.1.2/pretix_vrpay/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/payment.py` & `pretix-oppwa-1.1.2/pretix_vrpay/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/paymentmethods.py` & `pretix-oppwa-1.1.2/pretix_vrpay/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/signals.py` & `pretix-oppwa-1.1.2/pretix_vrpay/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/pretix_vrpay/static/pretix_vrpay/logo.svg` & `pretix-oppwa-1.1.2/pretix_vrpay/static/pretix_vrpay/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-oppwa-1.1.1/setup.cfg` & `pretix-oppwa-1.1.2/setup.cfg`

 * *Files identical despite different names*


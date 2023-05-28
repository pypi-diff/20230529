# Comparing `tmp/pretix-quickpay-1.1.0.tar.gz` & `tmp/pretix-quickpay-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-quickpay-1.1.0.tar", last modified: Mon Jan 30 14:13:22 2023, max compression
+gzip compressed data, was "pretix-quickpay-1.1.1.tar", last modified: Sun May 28 23:33:37 2023, max compression
```

## Comparing `pretix-quickpay-1.1.0.tar` & `pretix-quickpay-1.1.1.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.583933 pretix-quickpay-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1940 2023-01-30 14:13:22.583933 pretix-quickpay-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.547932 pretix-quickpay-1.1.0/pretix_quickpay/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:11:58.000000 pretix-quickpay-1.1.0/pretix_quickpay/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.539932 pretix-quickpay-1.1.0/pretix_quickpay/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.539932 pretix-quickpay-1.1.0/pretix_quickpay/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.551932 pretix-quickpay-1.1.0/pretix_quickpay/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9113 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.551932 pretix-quickpay-1.1.0/pretix_quickpay/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.551932 pretix-quickpay-1.1.0/pretix_quickpay/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9090 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    14149 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     6599 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.539932 pretix-quickpay-1.1.0/pretix_quickpay/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.551932 pretix-quickpay-1.1.0/pretix_quickpay/static/pretix_quickpay/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/static/pretix_quickpay/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/static/pretix_quickpay/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.539932 pretix-quickpay-1.1.0/pretix_quickpay/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.555933 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1149 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/control.html
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/pending.html
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_quickpay/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.551932 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1940 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1526 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-01-30 14:13:22.000000 pretix-quickpay-1.1.0/pretix_quickpay.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.555933 pretix-quickpay-1.1.0/pretix_unzerdirect/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.543932 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.543932 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.555933 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      943 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.555933 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.555933 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/payment.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.543932 pretix-quickpay-1.1.0/pretix_unzerdirect/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.583933 pretix-quickpay-1.1.0/pretix_unzerdirect/static/pretix_unzerdirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/static/pretix_unzerdirect/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1346 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/static/pretix_unzerdirect/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.543932 pretix-quickpay-1.1.0/pretix_unzerdirect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:13:22.583933 pretix-quickpay-1.1.0/pretix_unzerdirect/templates/pretix_unzerdirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/templates/pretix_unzerdirect/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/pretix_unzerdirect/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-01-30 14:13:22.587933 pretix-quickpay-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-01-30 14:09:16.000000 pretix-quickpay-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.265994 pretix-quickpay-1.1.1/pretix_quickpay/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_quickpay/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.257994 pretix-quickpay-1.1.1/pretix_quickpay/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9113 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_quickpay/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9090 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    14253 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     6599 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_quickpay/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay/static/pretix_quickpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_quickpay/static/pretix_quickpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/static/pretix_quickpay/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_quickpay/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_quickpay/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.285995 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-28 23:33:37.000000 pretix-quickpay-1.1.1/pretix_quickpay.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_unzerdirect/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/static/pretix_unzerdirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/static/pretix_unzerdirect/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1346 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/static/pretix_unzerdirect/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.261994 pretix-quickpay-1.1.1/pretix_unzerdirect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/pretix_unzerdirect/templates/pretix_unzerdirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:33:00.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/templates/pretix_unzerdirect/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pretix_unzerdirect/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:33:37.289995 pretix-quickpay-1.1.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-28 23:22:17.000000 pretix-quickpay-1.1.1/tests/test_main.py
```

### Comparing `pretix-quickpay-1.1.0/LICENSE` & `pretix-quickpay-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/PKG-INFO` & `pretix-quickpay-1.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pretix-quickpay
-Version: 1.1.0
-Summary: Use Quickpay as a payment provider, where you can activate various payment methods for your customers.
-Home-page: https://github.com/pretix/pretix-quickpay
-Author: Phin Wolkwitz
-Author-email: wolkwitz@rami.io
-License: Apache
-License-File: LICENSE
-
 Quickpay payments for pretix
 ============================
 
 This is a plugin for `pretix`_. 
 
 This allows you to to process payments through Quickpay as a payment provider or payment provider's that use Quickpay
 like Unzer Direct.
@@ -23,15 +13,15 @@
 
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

### Comparing `pretix-quickpay-1.1.0/README.rst` & `pretix-quickpay-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: pretix-quickpay
+Version: 1.1.1
+Summary: Use Quickpay as a payment provider, where you can activate various payment methods for your customers.
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2022 rami.io GmbH
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
+Project-URL: homepage, https://github.com/pretix/pretix-quickpay
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 Quickpay payments for pretix
 ============================
 
 This is a plugin for `pretix`_. 
 
 This allows you to to process payments through Quickpay as a payment provider or payment provider's that use Quickpay
 like Unzer Direct.
@@ -13,15 +41,15 @@
 
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

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/apps.py` & `pretix-quickpay-1.1.1/pretix_quickpay/apps.py`

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
             "Use Quickpay as a payment provider, where you can activate various payment methods for your customers."
         )
         visible = True
         version = __version__
         category = "PAYMENT"
         picture = "pretix_quickpay/logo.svg"
-        compatibility = "pretix>=2.7.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
-
-
```

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/locale/de/LC_MESSAGES/django.po` & `pretix-quickpay-1.1.1/pretix_quickpay/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-quickpay-1.1.1/pretix_quickpay/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/payment.py` & `pretix-quickpay-1.1.1/pretix_quickpay/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,17 @@
         return {
             "id": payment.info_data.get("id", None),
         }
 
     def matching_id(self, payment: OrderPayment):
         return payment.info_data.get("id", None)
 
+    def refund_matching_id(self, refund: OrderRefund):
+        return refund.info_data.get("id", None)
+
     def payment_pending_render(self, request, payment) -> str:
         if payment.info:
             payment_info = json.loads(payment.info)
         else:
             payment_info = None
         template = get_template("pretix_quickpay/pending.html")
         ctx = {
```

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/paymentmethods.py` & `pretix-quickpay-1.1.1/pretix_quickpay/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/signals.py` & `pretix-quickpay-1.1.1/pretix_quickpay/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/static/pretix_quickpay/logo.svg` & `pretix-quickpay-1.1.1/pretix_quickpay/static/pretix_quickpay/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/control.html` & `pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/control.html`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/templates/pretix_quickpay/pending.html` & `pretix-quickpay-1.1.1/pretix_quickpay/templates/pretix_quickpay/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/urls.py` & `pretix-quickpay-1.1.1/pretix_quickpay/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay/views.py` & `pretix-quickpay-1.1.1/pretix_quickpay/views.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay.egg-info/PKG-INFO` & `pretix-quickpay-1.1.1/pretix_quickpay.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 Metadata-Version: 2.1
 Name: pretix-quickpay
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use Quickpay as a payment provider, where you can activate various payment methods for your customers.
-Home-page: https://github.com/pretix/pretix-quickpay
-Author: Phin Wolkwitz
-Author-email: wolkwitz@rami.io
-License: Apache
+Author-email: pretix team <support@pretix.eu>
+Maintainer-email: pretix team <support@pretix.eu>
+License: 
+        Copyright 2022 rami.io GmbH
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
+Project-URL: homepage, https://github.com/pretix/pretix-quickpay
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Quickpay payments for pretix
 ============================
 
 This is a plugin for `pretix`_. 
 
@@ -23,15 +41,15 @@
 
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

### Comparing `pretix-quickpay-1.1.0/pretix_quickpay.egg-info/SOURCES.txt` & `pretix-quickpay-1.1.1/pretix_quickpay.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_quickpay/__init__.py
 pretix_quickpay/apps.py
 pretix_quickpay/payment.py
 pretix_quickpay/paymentmethods.py
 pretix_quickpay/signals.py
@@ -33,8 +34,9 @@
 pretix_unzerdirect/signals.py
 pretix_unzerdirect/urls.py
 pretix_unzerdirect/locale/de/LC_MESSAGES/django.po
 pretix_unzerdirect/locale/de_Informal/.gitkeep
 pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/django.po
 pretix_unzerdirect/static/pretix_unzerdirect/.gitkeep
 pretix_unzerdirect/static/pretix_unzerdirect/logo.svg
-pretix_unzerdirect/templates/pretix_unzerdirect/.gitkeep
+pretix_unzerdirect/templates/pretix_unzerdirect/.gitkeep
+tests/test_main.py
```

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/apps.py` & `pretix-quickpay-1.1.1/pretix_unzerdirect/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.utils.translation import gettext_lazy
+
 from pretix_quickpay import __version__
 
 try:
     from pretix.base.plugins import PluginConfig
 except ImportError:
     raise RuntimeError("Please use pretix 2.7 or above to run this plugin!")
 
@@ -18,13 +19,11 @@
         description = gettext_lazy(
             "Use Unzer Direct as a payment provider, where you can activate various payment methods for your customers."
         )
         visible = True
         version = __version__
         category = "PAYMENT"
         picture = "pretix_unzerdirect/logo.svg"
-        compatibility = "pretix>=2.7.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
-
-
```

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de/LC_MESSAGES/django.po` & `pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-quickpay-1.1.1/pretix_unzerdirect/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/payment.py` & `pretix-quickpay-1.1.1/pretix_unzerdirect/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/paymentmethods.py` & `pretix-quickpay-1.1.1/pretix_unzerdirect/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/signals.py` & `pretix-quickpay-1.1.1/pretix_unzerdirect/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/pretix_unzerdirect/static/pretix_unzerdirect/logo.svg` & `pretix-quickpay-1.1.1/pretix_unzerdirect/static/pretix_unzerdirect/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-quickpay-1.1.0/setup.cfg` & `pretix-quickpay-1.1.1/setup.cfg`

 * *Files identical despite different names*


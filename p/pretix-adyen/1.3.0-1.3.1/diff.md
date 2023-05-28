# Comparing `tmp/pretix-adyen-1.3.0.tar.gz` & `tmp/pretix-adyen-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-adyen-1.3.0.tar", last modified: Mon Jan 30 15:12:35 2023, max compression
+gzip compressed data, was "pretix-adyen-1.3.1.tar", last modified: Sun May 28 22:59:28 2023, max compression
```

## Comparing `pretix-adyen-1.3.0.tar` & `pretix-adyen-1.3.1.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.093633 pretix-adyen-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1176 2023-01-30 15:12:35.093633 pretix-adyen-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9303 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6064 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9559 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6618 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    27403 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/payment.py
--rw-rw-rw-   0 root         (0) root         (0)    19433 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/paymentmethods.py
--rw-rw-rw-   0 root         (0) root         (0)     3324 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.093633 pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/adyen_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     5591 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/pretix-adyen.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.085633 pretix-adyen-1.3.0/pretix_adyen/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.093633 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/control.html
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/control_settings.html
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/pending.html
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/presale_head.html
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/sca.html
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1715 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9302 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/pretix_adyen/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 15:12:35.089633 pretix-adyen-1.3.0/pretix_adyen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1340 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-01-30 15:12:34.000000 pretix-adyen-1.3.0/pretix_adyen.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-01-30 15:12:35.093633 pretix-adyen-1.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-01-30 15:05:58.000000 pretix-adyen-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.119615 pretix-adyen-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-28 22:59:28.119615 pretix-adyen-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6325 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9303 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 22:59:04.000000 pretix-adyen-1.3.1/pretix_adyen/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6064 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9559 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6618 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    27403 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)    19433 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/paymentmethods.py
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 22:59:04.000000 pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/adyen_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/pretix-adyen.css
+-rw-rw-rw-   0 root         (0) root         (0)     5715 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/pretix-adyen.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.111615 pretix-adyen-1.3.1/pretix_adyen/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.119615 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 22:59:04.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/control.html
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/control_settings.html
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/presale_head.html
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/sca.html
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1715 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9302 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pretix_adyen/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 22:59:28.115615 pretix-adyen-1.3.1/pretix_adyen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-28 22:59:28.000000 pretix-adyen-1.3.1/pretix_adyen.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-28 22:59:28.119615 pretix-adyen-1.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-28 08:28:11.000000 pretix-adyen-1.3.1/setup.py
```

### Comparing `pretix-adyen-1.3.0/LICENSE` & `pretix-adyen-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/README.rst` & `pretix-adyen-1.3.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-adyen``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-adyen-1.3.0/pretix_adyen/apps.py` & `pretix-adyen-1.3.1/pretix_adyen/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/de/LC_MESSAGES/django.po` & `pretix-adyen-1.3.1/pretix_adyen/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-adyen-1.3.1/pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/django.pot` & `pretix-adyen-1.3.1/pretix_adyen/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/hr/LC_MESSAGES/django.po` & `pretix-adyen-1.3.1/pretix_adyen/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/nl/LC_MESSAGES/django.po` & `pretix-adyen-1.3.1/pretix_adyen/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-adyen-1.3.1/pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/payment.py` & `pretix-adyen-1.3.1/pretix_adyen/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/paymentmethods.py` & `pretix-adyen-1.3.1/pretix_adyen/paymentmethods.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/signals.py` & `pretix-adyen-1.3.1/pretix_adyen/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/adyen_logo.svg` & `pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/adyen_logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/static/pretix_adyen/pretix-adyen.js` & `pretix-adyen-1.3.1/pretix_adyen/static/pretix_adyen/pretix-adyen.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,17 @@
         $('.adyen-container').closest("form").find(".checkout-button-row .btn-primary").prop("disabled", true);
 
         pretixadyen.adyen = await AdyenCheckout({
             locale: $.trim($("#adyen_locale").html()),
             environment: $.trim($("#adyen_environment").html()),
             clientKey: $.trim($("#adyen_clientKey").html()),
             paymentMethodsResponse: JSON.parse($.trim($("#adyen_paymentMethodsResponse").html())),
+            analytics: {
+                enabled: false
+            },
             onChange: function(state, component) {
                 switch (pretixadyen.method) {
                     case 'scheme':
                         if (state.isValid) {
                             $("#adyen_paymentMethodData-" + pretixadyen.method).val(JSON.stringify(state.data));
                             $('.adyen-container').closest("form").find(".checkout-button-row .btn-primary").prop("disabled", false);
                         } else {
@@ -53,35 +56,33 @@
             onPaymentCompleted: function(result, component) {
                 console.log("onPaymentCompleted", result, component);
             }
         });
 
         switch (pretixadyen.method) {
             case "scheme":
-                pretixadyen.adyen.create(pretixadyen.method, {
+                pretixadyen.mountedcomponent = pretixadyen.adyen.create(pretixadyen.method, {
                     hasHolderName: true,
                     holderNameRequired: true,
                 }).mount("#adyen-component-" + pretixadyen.method);
                 break;
             case "giftcard":
-                pretixadyen.adyen.create(pretixadyen.method, {
+                pretixadyen.mountedcomponent = pretixadyen.adyen.create(pretixadyen.method, {
                     brand: pretixadyen.brand
                 }).mount("#adyen-component-" + method_brand);
                 break;
             default:
-                pretixadyen.adyen.create(pretixadyen.method).mount("#adyen-component-" + method_brand);
+                pretixadyen.mountedcomponent = pretixadyen.adyen.create(pretixadyen.method).mount("#adyen-component-" + method_brand);
                 break;
         }
-
-        pretixadyen.mountedcomponent = method_brand;
     },
 
     'unmountcomponent': function() {
-        $('#adyen-component-' + pretixadyen.mountedcomponent).empty();
-        pretixadyen.mountedcomponent = null;
+        pretixadyen.mountedcomponent.unmount();
+        console.log(pretixadyen.mountedcomponent);
         pretixadyen.adyen = null;
         $('.adyen-container').closest("form").find(".checkout-button-row .btn-primary").prop("disabled", false);
     },
 
     'action': async function() {
         if (pretixadyen.adyen !== null) {
             return;
@@ -99,15 +100,15 @@
                 $('#continuebutton').removeClass('hidden');
                 $('#continuebutton').closest("form").submit();
                 waitingDialog.show(gettext("Contacting your bank …"));
             }
         });
 
         let action = JSON.parse($("#adyen_action").val());
-        pretixadyen.adyen.createFromAction(action).mount('#scacontainer');
+        pretixadyen.mountedcomponent = pretixadyen.adyen.createFromAction(action).mount('#scacontainer');
         waitingDialog.hide();
     },
 
     'get_method': function(method_brand) {
         return method_brand.split("__")[0]
     },
```

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/control.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/control.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/control_settings.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/control_settings.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/pending.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/presale_head.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/presale_head.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 {% load static %}
 {% load compress %}
 {% load i18n %}
 
 {% compress js %}
     <script type="text/javascript" src="{% static "pretix_adyen/pretix-adyen.js" %}"></script>
 {% endcompress %}
-<script src="https://checkoutshopper-{{ environment }}.adyen.com/checkoutshopper/sdk/5.14.0/adyen.js"
-        integrity="sha384-JsWtX9H7PkCMYb50ZDb4AdPdVNcPDx/O+aUYtLyLxU3D04jiqFEqnLKMDUIWxBpv"
+{% compress css %}
+    <link type="text/css" rel="stylesheet" href="{% static "pretix_adyen/pretix-adyen.css" %}">
+{% endcompress %}
+
+<script src="https://checkoutshopper-{{ environment }}.adyen.com/checkoutshopper/sdk/5.38.0/adyen.js"
+        integrity="sha384-uoYZHqftW2oZ6ZlSSv3pu0w4+zqVc0lKpXeVl2b/rgwsOvVAVYYSoFBkChjWls50"
         crossorigin="anonymous"></script>
 
-<link rel="stylesheet" href="https://checkoutshopper-{{ environment }}.adyen.com/checkoutshopper/sdk/5.14.0/adyen.css"
-     integrity="sha384-Dm1w8jaVOWA8rxpzkxA41DIyw5VlBjpoMTPfAijlfepYGgLKF+hke3NKeU/KTX7t"
+<link rel="stylesheet" href="https://checkoutshopper-{{ environment }}.adyen.com/checkoutshopper/sdk/5.38.0/adyen.css"
+     integrity="sha384-dzFUmC8dpGlHeo+gB2Bf4d9PXOtHJj90UPbuZhE8U41Fy1ONLJwBOCJVWZ5DhxFM"
      crossorigin="anonymous" />
 
 <script type="text/plain" id="adyen_locale">{{ locale }}</script>
 <script type="text/plain" id="adyen_environment">{{ environment }}</script>
 <script type="text/plain" id="adyen_clientKey">{{ clientKey }}</script>
 <script type="text/plain" id="adyen_paymentMethodsResponse">{{ paymentMethodsResponse|safe }}</script>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 {% load static %} {% load compress %} {% load i18n %} {% compress js %}
 retix-adyen.js" %}">
-{% endcompress %}
+{% endcompress %} {% compress css %}
+retix-adyen.css" %}"> {% endcompress %}
```

### Comparing `pretix-adyen-1.3.0/pretix_adyen/templates/pretix_adyen/sca.html` & `pretix-adyen-1.3.1/pretix_adyen/templates/pretix_adyen/sca.html`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/utils.py` & `pretix-adyen-1.3.1/pretix_adyen/utils.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen/views.py` & `pretix-adyen-1.3.1/pretix_adyen/views.py`

 * *Files identical despite different names*

### Comparing `pretix-adyen-1.3.0/pretix_adyen.egg-info/SOURCES.txt` & `pretix-adyen-1.3.1/pretix_adyen.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_adyen/__init__.py
 pretix_adyen/apps.py
 pretix_adyen/payment.py
 pretix_adyen/paymentmethods.py
 pretix_adyen/signals.py
@@ -14,22 +15,24 @@
 pretix_adyen.egg-info/PKG-INFO
 pretix_adyen.egg-info/SOURCES.txt
 pretix_adyen.egg-info/dependency_links.txt
 pretix_adyen.egg-info/entry_points.txt
 pretix_adyen.egg-info/requires.txt
 pretix_adyen.egg-info/top_level.txt
 pretix_adyen/locale/django.pot
+pretix_adyen/locale/cs/LC_MESSAGES/django.po
 pretix_adyen/locale/de/LC_MESSAGES/django.po
 pretix_adyen/locale/de_Informal/.gitkeep
 pretix_adyen/locale/de_Informal/LC_MESSAGES/django.po
 pretix_adyen/locale/hr/LC_MESSAGES/django.po
 pretix_adyen/locale/nl/LC_MESSAGES/django.po
 pretix_adyen/locale/nl_Informal/LC_MESSAGES/django.po
 pretix_adyen/static/pretix_adyen/.gitkeep
 pretix_adyen/static/pretix_adyen/adyen_logo.svg
+pretix_adyen/static/pretix_adyen/pretix-adyen.css
 pretix_adyen/static/pretix_adyen/pretix-adyen.js
 pretix_adyen/templates/pretix_adyen/.gitkeep
 pretix_adyen/templates/pretix_adyen/checkout_payment_confirm.html
 pretix_adyen/templates/pretix_adyen/checkout_payment_form.html
 pretix_adyen/templates/pretix_adyen/control.html
 pretix_adyen/templates/pretix_adyen/control_settings.html
 pretix_adyen/templates/pretix_adyen/pending.html
```

### Comparing `pretix-adyen-1.3.0/setup.cfg` & `pretix-adyen-1.3.1/setup.cfg`

 * *Files identical despite different names*


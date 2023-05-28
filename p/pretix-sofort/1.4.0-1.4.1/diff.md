# Comparing `tmp/pretix-sofort-1.4.0.tar.gz` & `tmp/pretix-sofort-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-sofort-1.4.0.tar", last modified: Mon Jan 30 14:29:53 2023, max compression
+gzip compressed data, was "pretix-sofort-1.4.1.tar", last modified: Sun May 28 23:29:47 2023, max compression
```

## Comparing `pretix-sofort-1.4.0.tar` & `pretix-sofort-1.4.1.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.911857 pretix-sofort-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1135 2023-01-30 14:29:53.911857 pretix-sofort-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.899857 pretix-sofort-1.4.0/pretix_sofort/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10539 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10423 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     5105 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5262 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7383 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5774 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7612 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7633 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5324 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5089 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5297 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5347 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5080 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5086 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     9917 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.895857 pretix-sofort-1.4.0/pretix_sofort/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5500 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.907858 pretix-sofort-1.4.0/pretix_sofort/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/migrations/0002_referencedsoforttransaction_payment.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9215 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/signals.py
--rw-rw-rw-   0 root         (0) root         (0)    10126 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/sofort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.899857 pretix-sofort-1.4.0/pretix_sofort/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.911857 pretix-sofort-1.4.0/pretix_sofort/static/pretix_sofort/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/static/pretix_sofort/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)    12103 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/static/pretix_sofort/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.899857 pretix-sofort-1.4.0/pretix_sofort/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.911857 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/action_overpaid.html
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/action_refund.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/control.html
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/pretix_sofort/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-30 14:29:53.903857 pretix-sofort-1.4.0/pretix_sofort.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1135 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2221 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-30 14:29:53.000000 pretix-sofort-1.4.0/pretix_sofort.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-01-30 14:29:53.911857 pretix-sofort-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1055 2023-01-30 14:29:08.000000 pretix-sofort-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10539 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10423 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     5105 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5262 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7346 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.096338 pretix-sofort-1.4.1/pretix_sofort/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5297 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5347 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5080 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5086 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5500 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/migrations/0002_referencedsoforttransaction_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     9215 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)    10126 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/sofort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/static/pretix_sofort/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/static/pretix_sofort/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)    12103 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/static/pretix_sofort/logo.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.100338 pretix-sofort-1.4.1/pretix_sofort/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/action_overpaid.html
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/action_refund.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pretix_sofort/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 23:29:47.104338 pretix-sofort-1.4.1/pretix_sofort.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-28 23:29:47.000000 pretix-sofort-1.4.1/pretix_sofort.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-28 23:29:47.108338 pretix-sofort-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 23:29:20.000000 pretix-sofort-1.4.1/setup.py
```

### Comparing `pretix-sofort-1.4.0/LICENSE` & `pretix-sofort-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/README.rst` & `pretix-sofort-1.4.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-sofort``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/apps.py` & `pretix-sofort-1.4.1/pretix_sofort/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
         name = 'SOFORT'
         author = 'Raphael Michel'
         category = 'PAYMENT'
         description = gettext_lazy('Accept payments through Sofort, a payment method offered by Klarna.')
         visible = True
         picture = "pretix_sofort/logo.png"
         version = __version__
-        compatibility = "pretix>=4.16.0"
+        compatibility = "pretix>=4.20.0"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/ca/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/cs/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/hr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/de/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/django.pot` & `pretix-sofort-1.4.1/pretix_sofort/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/el/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/fi/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/hr/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: hr\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/it/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/it/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
-"PO-Revision-Date: 2022-02-21 07:00+0000\n"
-"Last-Translator: Emanuele Signoretta <signorettae@gmail.com>\n"
-"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/pretix-"
-"plugin-sofort/it/>\n"
+"PO-Revision-Date: 2023-05-18 01:00+0000\n"
+"Last-Translator: M C <micasadmail@gmail.com>\n"
+"Language-Team: Italian <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sofort/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.8\n"
+"X-Generator: Weblate 4.17\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
 
 #: pretix_sofort/payment.py:30
 #, fuzzy
@@ -133,15 +133,15 @@
 
 #: pretix_sofort/templates/pretix_sofort/control.html:18
 msgid "Payer name"
 msgstr "Pagante"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:20
 msgid "IBAN"
-msgstr "Codice IBAN"
+msgstr "IBAN"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:22
 msgid "Bank"
 msgstr "Istituto bancario"
 
 #: pretix_sofort/templates/pretix_sofort/pending.html:4
 msgid ""
@@ -160,16 +160,18 @@
 "contattaci se ci dovesse impiegare più di qualche ora."
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:17
 msgid "The payment process has started in a new window."
 msgstr "Il processo di pagamento è iniziato in una nuova finestra."
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:20
+#, fuzzy
 msgid "The window to enter your payment data was not opened or was closed?"
-msgstr "La finestra di pagamento non è stata aperta o è stata chiusa?"
+msgstr ""
+"La finestra per inserire i dati di pagamento non era aperta o era chiusa?"
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:25
 msgid "Click here in order to open the window."
 msgstr "Clicca qui per aprire la finestra."
 
 #: pretix_sofort/views.py:117
 msgid ""
@@ -204,16 +206,16 @@
 msgstr "Scusa, c'è stato un errore durante l'elaborazione del pagamento."
 
 #: pretix_sofort/views.py:193
 msgid ""
 "Sorry, there was an error in the payment process. Please check the link in "
 "your emails to continue."
 msgstr ""
-"Scusa, c'è stato un errore durante l'elaborazione del pagamento. Per favore "
-"controlla il link nelle email ricevute per continuare."
+"Spiacenti, c'è stato un errore durante il pagamento. Segui il link "
+"nell'email per continuare."
 
 #, fuzzy
 #~ msgid "Sofort payment"
 #~ msgstr "Paga con Sofort"
 
 #, fuzzy
 #~ msgid "pretix payment via Klarna Sofort"
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/ja/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ja\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/lv/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/nl/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/pl/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/pt/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/ru/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/sl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ru\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/si/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/sl/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/sv/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: sl\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
@@ -112,15 +112,15 @@
 
 #: pretix_sofort/templates/pretix_sofort/control.html:10
 msgid "Time"
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/control.html:14
 msgid "Status"
-msgstr ""
+msgstr "Status"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:18
 msgid "Payer name"
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/control.html:20
 msgid "IBAN"
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/sv/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: sv\n"
+"PO-Revision-Date: 2019-03-20 11:00+0000\n"
+"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
+"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
+"pretix/pretix-plugin-sofort/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 3.4\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
 
 #: pretix_sofort/payment.py:30
 msgid "Sofort"
@@ -108,31 +111,31 @@
 
 #: pretix_sofort/templates/pretix_sofort/control.html:6
 msgid "Transaction"
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/control.html:10
 msgid "Time"
-msgstr ""
+msgstr "时间"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:14
 msgid "Status"
-msgstr "Status"
+msgstr "状态"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:18
 msgid "Payer name"
-msgstr ""
+msgstr "付款人姓名"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:20
 msgid "IBAN"
-msgstr ""
+msgstr "国际银行账号"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:22
 msgid "Bank"
-msgstr ""
+msgstr "银行"
 
 #: pretix_sofort/templates/pretix_sofort/pending.html:4
 msgid ""
 "Our attempt to execute your payment has failed. Please try again or contact "
 "us."
 msgstr ""
 
@@ -140,23 +143,23 @@
 msgid ""
 "We're waiting for an answer regarding your payment. Please contact us, if "
 "this takes more than a few hours."
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:17
 msgid "The payment process has started in a new window."
-msgstr ""
+msgstr "付款流程已在新窗口中启动。"
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:20
 msgid "The window to enter your payment data was not opened or was closed?"
-msgstr ""
+msgstr "输入付款数据的窗口未打开或已关闭？"
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:25
 msgid "Click here in order to open the window."
-msgstr ""
+msgstr "单击此处打开窗口。"
 
 #: pretix_sofort/views.py:117
 msgid ""
 "Your payment could not be handled as the event sold out in the meantime. "
 "Please contact the organizer for more information."
 msgstr ""
 
@@ -179,8 +182,8 @@
 msgid "Sorry, there was an error in the payment process."
 msgstr ""
 
 #: pretix_sofort/views.py:193
 msgid ""
 "Sorry, there was an error in the payment process. Please check the link in "
 "your emails to continue."
-msgstr ""
+msgstr "抱歉，付款过程中出错。请检查电子邮件中的链接以继续。"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/tr/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-sofort-1.4.1/pretix_sofort/locale/cs/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-11-07 16:32+0100\n"
-"PO-Revision-Date: 2019-03-20 11:00+0000\n"
-"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
-"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
-"pretix/pretix-plugin-sofort/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"PO-Revision-Date: 2023-03-19 18:00+0000\n"
+"Last-Translator: Michael <michael.happl@gmx.at>\n"
+"Language-Team: Czech <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-sofort/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.4\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: pretix_sofort/__init__.py:15
 msgid "Accept payments through Sofort, a payment method offered by Klarna."
 msgstr ""
 
 #: pretix_sofort/payment.py:30
 msgid "Sofort"
 msgstr ""
 
 #: pretix_sofort/payment.py:31
 msgid "SOFORT (instant bank transfer)"
-msgstr ""
+msgstr "SOFORT (okamžitý bankovní převod)"
 
 #: pretix_sofort/payment.py:40
 msgid "Customer ID"
 msgstr ""
 
 #: pretix_sofort/payment.py:44
 msgid "API key"
@@ -111,31 +111,31 @@
 
 #: pretix_sofort/templates/pretix_sofort/control.html:6
 msgid "Transaction"
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/control.html:10
 msgid "Time"
-msgstr "时间"
+msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/control.html:14
 msgid "Status"
-msgstr "状态"
+msgstr "Status"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:18
 msgid "Payer name"
-msgstr "付款人姓名"
+msgstr "Jméno poplatníka"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:20
 msgid "IBAN"
-msgstr "国际银行账号"
+msgstr "IBAN"
 
 #: pretix_sofort/templates/pretix_sofort/control.html:22
 msgid "Bank"
-msgstr "银行"
+msgstr "Banka"
 
 #: pretix_sofort/templates/pretix_sofort/pending.html:4
 msgid ""
 "Our attempt to execute your payment has failed. Please try again or contact "
 "us."
 msgstr ""
 
@@ -143,23 +143,23 @@
 msgid ""
 "We're waiting for an answer regarding your payment. Please contact us, if "
 "this takes more than a few hours."
 msgstr ""
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:17
 msgid "The payment process has started in a new window."
-msgstr "付款流程已在新窗口中启动。"
+msgstr "Proces platby se spustil v novém okně."
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:20
 msgid "The window to enter your payment data was not opened or was closed?"
-msgstr "输入付款数据的窗口未打开或已关闭？"
+msgstr "Okno pro zadání platebních údajů se neotevřelo nebo bylo zavřeno?"
 
 #: pretix_sofort/templates/pretix_sofort/redirect.html:25
 msgid "Click here in order to open the window."
-msgstr "单击此处打开窗口。"
+msgstr "Kliknutím zde otevřete okno."
 
 #: pretix_sofort/views.py:117
 msgid ""
 "Your payment could not be handled as the event sold out in the meantime. "
 "Please contact the organizer for more information."
 msgstr ""
 
@@ -176,14 +176,16 @@
 
 #: pretix_sofort/views.py:171
 msgid "The payment process was canceled. You can click below to try again."
 msgstr ""
 
 #: pretix_sofort/views.py:182
 msgid "Sorry, there was an error in the payment process."
-msgstr ""
+msgstr "Omlouváme se, při platbě došlo k chybě."
 
 #: pretix_sofort/views.py:193
 msgid ""
 "Sorry, there was an error in the payment process. Please check the link in "
 "your emails to continue."
-msgstr "抱歉，付款过程中出错。请检查电子邮件中的链接以继续。"
+msgstr ""
+"Omlouváme se, při platbě došlo k chybě. Zkontrolujte prosím odkaz ve svých e-"
+"mailech a pokračujte."
```

### Comparing `pretix-sofort-1.4.0/pretix_sofort/migrations/0001_initial.py` & `pretix-sofort-1.4.1/pretix_sofort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/migrations/0002_referencedsoforttransaction_payment.py` & `pretix-sofort-1.4.1/pretix_sofort/migrations/0002_referencedsoforttransaction_payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/payment.py` & `pretix-sofort-1.4.1/pretix_sofort/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/signals.py` & `pretix-sofort-1.4.1/pretix_sofort/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/sofort.py` & `pretix-sofort-1.4.1/pretix_sofort/sofort.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/static/pretix_sofort/logo.png` & `pretix-sofort-1.4.1/pretix_sofort/static/pretix_sofort/logo.png`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/control.html` & `pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/control.html`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort/templates/pretix_sofort/redirect.html` & `pretix-sofort-1.4.1/pretix_sofort/templates/pretix_sofort/redirect.html`

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

### Comparing `pretix-sofort-1.4.0/pretix_sofort/views.py` & `pretix-sofort-1.4.1/pretix_sofort/views.py`

 * *Files identical despite different names*

### Comparing `pretix-sofort-1.4.0/pretix_sofort.egg-info/SOURCES.txt` & `pretix-sofort-1.4.1/pretix_sofort.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_sofort/__init__.py
 pretix_sofort/apps.py
 pretix_sofort/models.py
 pretix_sofort/payment.py
 pretix_sofort/signals.py
```


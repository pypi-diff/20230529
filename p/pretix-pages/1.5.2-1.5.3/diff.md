# Comparing `tmp/pretix-pages-1.5.2.tar.gz` & `tmp/pretix-pages-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-pages-1.5.2.tar", last modified: Tue Mar 28 08:16:09 2023, max compression
+gzip compressed data, was "pretix-pages-1.5.3.tar", last modified: Mon May 29 07:21:45 2023, max compression
```

## Comparing `pretix-pages-1.5.2.tar` & `pretix-pages-1.5.3.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.238262 pretix-pages-1.5.2/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1726 2023-03-28 08:16:09.238262 pretix-pages-1.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.222261 pretix-pages-1.5.2/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.222261 pretix-pages-1.5.2/pretix_pages/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/ar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.222261 pretix-pages-1.5.2/pretix_pages/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.222261 pretix-pages-1.5.2/pretix_pages/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4539 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/cs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/da/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/da/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5450 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5461 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5440 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     4157 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5629 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.210261 pretix-pages-1.5.2/pretix_pages/locale/gl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/gl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/hr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.226261 pretix-pages-1.5.2/pretix_pages/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/it/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4557 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5629 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5663 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4141 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5550 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/pt_BR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.214261 pretix-pages-1.5.2/pretix_pages/locale/pt_PT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/pt_PT/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4297 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/tr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5533 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.230262 pretix-pages-1.5.2/pretix_pages/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     4407 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.234262 pretix-pages-1.5.2/pretix_pages/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/migrations/0002_auto_20170220_1423.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/migrations/0003_auto_20170504_0706.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/migrations/0004_auto_20170517_1550.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.234262 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2175 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/editor.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.234262 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/
--rw-rw-rw-   0 root         (0) root         (0)    22595 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.bubble.css
--rw-rw-rw-   0 root         (0) root         (0)     8421 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.core.css
--rw-rw-rw-   0 root         (0) root         (0)   284512 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.core.js
--rw-rw-rw-   0 root         (0) root         (0)   414471 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.js
--rw-rw-rw-   0 root         (0) root         (0)    23088 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.snow.css
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill-edit.css
--rw-rw-rw-   0 root         (0) root         (0)     6518 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill-show.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.218261 pretix-pages-1.5.2/pretix_pages/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.238262 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/control_head.html
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/delete.html
--rw-rw-rw-   0 root         (0) root         (0)     3327 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/form.html
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/front_page.html
--rw-rw-rw-   0 root         (0) root         (0)     3105 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/index.html
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/presale_head.html
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/show.html
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    10404 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/pretix_pages/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 08:16:09.222261 pretix-pages-1.5.2/pretix_pages.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1726 2023-03-28 08:16:09.000000 pretix-pages-1.5.2/pretix_pages.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2853 2023-03-28 08:16:09.000000 pretix-pages-1.5.2/pretix_pages.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 08:16:09.000000 pretix-pages-1.5.2/pretix_pages.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-03-28 08:16:09.000000 pretix-pages-1.5.2/pretix_pages.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-28 08:16:09.000000 pretix-pages-1.5.2/pretix_pages.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-03-28 08:16:09.238262 pretix-pages-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-03-28 08:15:26.000000 pretix-pages-1.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.953563 pretix-pages-1.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-29 07:21:45.953563 pretix-pages-1.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/ar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4539 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/cs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4379 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/da/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/da/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5629 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/gl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/gl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/hr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/hr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/it/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5629 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.933562 pretix-pages-1.5.3/pretix_pages/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5663 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4477 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4141 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/pt_BR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/pt_PT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/pt_PT/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.945562 pretix-pages-1.5.3/pretix_pages/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4339 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4297 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/tr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5533 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     4407 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/migrations/0002_auto_20170220_1423.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/migrations/0003_auto_20170504_0706.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/migrations/0004_auto_20170517_1550.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.949562 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/editor.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.953563 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/
+-rw-rw-rw-   0 root         (0) root         (0)    22595 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.bubble.css
+-rw-rw-rw-   0 root         (0) root         (0)     8421 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.core.css
+-rw-rw-rw-   0 root         (0) root         (0)   284512 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.core.js
+-rw-rw-rw-   0 root         (0) root         (0)   414471 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.js
+-rw-rw-rw-   0 root         (0) root         (0)    23088 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.snow.css
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill-edit.css
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill-show.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.937562 pretix-pages-1.5.3/pretix_pages/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.953563 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/control_head.html
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/delete.html
+-rw-rw-rw-   0 root         (0) root         (0)     3327 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/form.html
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/front_page.html
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/index.html
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/presale_head.html
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/show.html
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    10404 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pretix_pages/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:21:45.941562 pretix-pages-1.5.3/pretix_pages.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-05-29 07:21:45.000000 pretix-pages-1.5.3/pretix_pages.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-29 07:21:45.000000 pretix-pages-1.5.3/pretix_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 07:21:45.000000 pretix-pages-1.5.3/pretix_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-29 07:21:45.000000 pretix-pages-1.5.3/pretix_pages.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 07:21:45.000000 pretix-pages-1.5.3/pretix_pages.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-29 07:21:45.953563 pretix-pages-1.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-29 07:21:20.000000 pretix-pages-1.5.3/setup.py
```

### Comparing `pretix-pages-1.5.2/LICENSE` & `pretix-pages-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/PKG-INFO` & `pretix-pages-1.5.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 Metadata-Version: 2.1
 Name: pretix-pages
-Version: 1.5.2
+Version: 1.5.3
 Summary: pretix plugin that allows you to add static pages to your event site, for example for a FAQ, terms of service, etc.
-Home-page: https://github.com/pretix/pretix-pages
-Author: Raphael Michel
-Author-email: mail@raphaelmichel.de
-License: Apache License 2.0
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
+Project-URL: homepage, https://github.com/pretix/pretix-pages
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pretix pages
 ============
 
 This is a plugin for `pretix`_ that allows you to add static pages to your event site, for example for a FAQ, terms of
 service, etc.
@@ -28,15 +44,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-pages``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-pages-1.5.2/README.rst` & `pretix-pages-1.5.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-pages``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-pages-1.5.2/pretix_pages/apps.py` & `pretix-pages-1.5.3/pretix_pages/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/ar/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/ca/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/cs/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/fi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: cs\n"
+"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/da/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/de/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/django.pot` & `pretix-pages-1.5.3/pretix_pages/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/el/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/es/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/fi/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/gl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: fi\n"
+"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/fr/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/gl/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: gl\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/hr/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/it/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/ja/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/sl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ja\n"
+"Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/lv/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/nl/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/pl/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/pt/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: pt_PT\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/ru/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: ru\n"
+"PO-Revision-Date: 2019-03-20 11:00+0000\n"
+"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
+"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
+"pretix/pretix-plugin-pages/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 3.4\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
 msgid "Pages"
 msgstr ""
 
@@ -89,36 +92,36 @@
 #: pretix_pages/templates/pretix_pages/delete.html:9
 #, python-format
 msgid "Are you sure you want to delete the page <strong>%(name)s</strong>?"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:14
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
 #: pretix_pages/templates/pretix_pages/delete.html:17
 msgid "Delete"
-msgstr ""
+msgstr "删除"
 
 #: pretix_pages/templates/pretix_pages/form.html:5
 #: pretix_pages/templates/pretix_pages/form.html:7
 msgid "Page"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:14
 msgid "General information"
-msgstr ""
+msgstr "一般信息"
 
 #: pretix_pages/templates/pretix_pages/form.html:25
 msgid "Please enable JavaScript"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:53
 msgid "Save"
-msgstr ""
+msgstr "保存"
 
 #: pretix_pages/templates/pretix_pages/form.html:62
 msgid "Page history"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/front_page.html:4
 msgid "More information"
@@ -147,16 +150,16 @@
 
 #: pretix_pages/views.py:136
 msgid "The selected page has been deleted."
 msgstr ""
 
 #: pretix_pages/views.py:179
 msgid "Your changes have been saved."
-msgstr ""
+msgstr "您的更改已保存。"
 
 #: pretix_pages/views.py:190 pretix_pages/views.py:227
 msgid "We could not save your changes. See below for details."
-msgstr ""
+msgstr "我们无法保存您的更改。详见下文。"
 
 #: pretix_pages/views.py:219
 msgid "The new page has been created."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/si/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/sl/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/sv/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: sl\n"
+"PO-Revision-Date: 2022-03-03 07:00+0000\n"
+"Last-Translator: MaLund13 <mart.lund13@gmail.com>\n"
+"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-pages/sv/>\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.8\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
 msgid "Pages"
 msgstr ""
 
@@ -89,15 +92,15 @@
 #: pretix_pages/templates/pretix_pages/delete.html:9
 #, python-format
 msgid "Are you sure you want to delete the page <strong>%(name)s</strong>?"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:14
 msgid "Cancel"
-msgstr ""
+msgstr "Avbryt"
 
 #: pretix_pages/templates/pretix_pages/delete.html:17
 msgid "Delete"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:5
 #: pretix_pages/templates/pretix_pages/form.html:7
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/sv/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/cs/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
-"PO-Revision-Date: 2022-03-03 07:00+0000\n"
-"Last-Translator: MaLund13 <mart.lund13@gmail.com>\n"
-"Language-Team: Swedish <https://translate.pretix.eu/projects/pretix/"
-"pretix-plugin-pages/sv/>\n"
-"Language: sv\n"
+"PO-Revision-Date: 2023-03-23 05:00+0000\n"
+"Last-Translator: Michael <michael.happl@gmx.at>\n"
+"Language-Team: Czech <https://translate.pretix.eu/projects/pretix/"
+"pretix-plugin-pages/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.8\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
 msgid "Pages"
 msgstr ""
 
@@ -92,36 +92,36 @@
 #: pretix_pages/templates/pretix_pages/delete.html:9
 #, python-format
 msgid "Are you sure you want to delete the page <strong>%(name)s</strong>?"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:14
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:17
 msgid "Delete"
-msgstr ""
+msgstr "Smazat"
 
 #: pretix_pages/templates/pretix_pages/form.html:5
 #: pretix_pages/templates/pretix_pages/form.html:7
 msgid "Page"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:14
 msgid "General information"
-msgstr ""
+msgstr "Základní informace"
 
 #: pretix_pages/templates/pretix_pages/form.html:25
 msgid "Please enable JavaScript"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:53
 msgid "Save"
-msgstr ""
+msgstr "Uložit"
 
 #: pretix_pages/templates/pretix_pages/form.html:62
 msgid "Page history"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/front_page.html:4
 msgid "More information"
@@ -150,15 +150,15 @@
 
 #: pretix_pages/views.py:136
 msgid "The selected page has been deleted."
 msgstr ""
 
 #: pretix_pages/views.py:179
 msgid "Your changes have been saved."
-msgstr ""
+msgstr "Vaše změny byly uloženy."
 
 #: pretix_pages/views.py:190 pretix_pages/views.py:227
 msgid "We could not save your changes. See below for details."
 msgstr ""
 
 #: pretix_pages/views.py:219
 msgid "The new page has been created."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/tr/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-pages-1.5.3/pretix_pages/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2018-12-06 10:11+0100\n"
-"PO-Revision-Date: 2019-03-20 11:00+0000\n"
-"Last-Translator: yichengsd <sunzl@jxepub.com>\n"
-"Language-Team: Chinese (Simplified) <https://translate.pretix.eu/projects/"
-"pretix/pretix-plugin-pages/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"PO-Revision-Date: 2023-03-06 07:00+0000\n"
+"Last-Translator: Vasco Baleia <vb2003.12@gmail.com>\n"
+"Language-Team: Portuguese (Portugal) <https://translate.pretix.eu/projects/"
+"pretix/pretix-plugin-pages/pt_PT/>\n"
+"Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.4\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.15.2\n"
 
 #: pretix_pages/__init__.py:10 pretix_pages/signals.py:23
 #: pretix_pages/templates/pretix_pages/index.html:6
 #: pretix_pages/templates/pretix_pages/index.html:8
 msgid "Pages"
-msgstr ""
+msgstr "Páginas"
 
 #: pretix_pages/__init__.py:12
 msgid ""
 "Allows you to add static pages to your event site, for example for a FAQ, "
 "terms of service, etc."
 msgstr ""
+"Permite adicionar páginas estáticas ao site do evento, para, por exemplo, "
+"FAQs, termos e condições, etc."
 
 #: pretix_pages/models.py:11 pretix_pages/views.py:101
 msgid "URL form"
 msgstr ""
 
 #: pretix_pages/models.py:15
 msgid "The slug may only contain letters, numbers, dots and dashes."
@@ -92,36 +94,36 @@
 #: pretix_pages/templates/pretix_pages/delete.html:9
 #, python-format
 msgid "Are you sure you want to delete the page <strong>%(name)s</strong>?"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:14
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
 
 #: pretix_pages/templates/pretix_pages/delete.html:17
 msgid "Delete"
-msgstr "删除"
+msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:5
 #: pretix_pages/templates/pretix_pages/form.html:7
 msgid "Page"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:14
 msgid "General information"
-msgstr "一般信息"
+msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:25
 msgid "Please enable JavaScript"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:53
 msgid "Save"
-msgstr "保存"
+msgstr ""
 
 #: pretix_pages/templates/pretix_pages/form.html:62
 msgid "Page history"
 msgstr ""
 
 #: pretix_pages/templates/pretix_pages/front_page.html:4
 msgid "More information"
@@ -150,16 +152,16 @@
 
 #: pretix_pages/views.py:136
 msgid "The selected page has been deleted."
 msgstr ""
 
 #: pretix_pages/views.py:179
 msgid "Your changes have been saved."
-msgstr "您的更改已保存。"
+msgstr ""
 
 #: pretix_pages/views.py:190 pretix_pages/views.py:227
 msgid "We could not save your changes. See below for details."
-msgstr "我们无法保存您的更改。详见下文。"
+msgstr ""
 
 #: pretix_pages/views.py:219
 msgid "The new page has been created."
 msgstr ""
```

### Comparing `pretix-pages-1.5.2/pretix_pages/migrations/0001_initial.py` & `pretix-pages-1.5.3/pretix_pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/migrations/0002_auto_20170220_1423.py` & `pretix-pages-1.5.3/pretix_pages/migrations/0002_auto_20170220_1423.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/migrations/0003_auto_20170504_0706.py` & `pretix-pages-1.5.3/pretix_pages/migrations/0003_auto_20170504_0706.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/migrations/0004_auto_20170517_1550.py` & `pretix-pages-1.5.3/pretix_pages/migrations/0004_auto_20170517_1550.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/models.py` & `pretix-pages-1.5.3/pretix_pages/models.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/signals.py` & `pretix-pages-1.5.3/pretix_pages/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/editor.js` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/editor.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.bubble.css` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.bubble.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.core.css` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.core.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.core.js` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.core.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.js` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.js`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill/quill.snow.css` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill/quill.snow.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/static/pretix_pages/quill-show.css` & `pretix-pages-1.5.3/pretix_pages/static/pretix_pages/quill-show.css`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/delete.html` & `pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/delete.html`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/form.html` & `pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/form.html`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/templates/pretix_pages/index.html` & `pretix-pages-1.5.3/pretix_pages/templates/pretix_pages/index.html`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/urls.py` & `pretix-pages-1.5.3/pretix_pages/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages/views.py` & `pretix-pages-1.5.3/pretix_pages/views.py`

 * *Files identical despite different names*

### Comparing `pretix-pages-1.5.2/pretix_pages.egg-info/PKG-INFO` & `pretix-pages-1.5.3/pretix_pages.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 Metadata-Version: 2.1
 Name: pretix-pages
-Version: 1.5.2
+Version: 1.5.3
 Summary: pretix plugin that allows you to add static pages to your event site, for example for a FAQ, terms of service, etc.
-Home-page: https://github.com/pretix/pretix-pages
-Author: Raphael Michel
-Author-email: mail@raphaelmichel.de
-License: Apache License 2.0
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
+Project-URL: homepage, https://github.com/pretix/pretix-pages
+Keywords: pretix
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pretix pages
 ============
 
 This is a plugin for `pretix`_ that allows you to add static pages to your event site, for example for a FAQ, terms of
 service, etc.
@@ -28,15 +44,15 @@
 
 1. Make sure that you have a working `pretix development setup`_.
 
 2. Clone this repository, eg to ``local/pretix-pages``.
 
 3. Activate the virtual environment you use for pretix development.
 
-4. Execute ``python setup.py develop`` within this directory to register this application with pretix's plugin registry.
+4. Execute ``pip install -e .`` within this directory to register this application with pretix's plugin registry.
 
 5. Execute ``make`` within this directory to compile translations.
 
 6. Restart your local pretix server. You can now use the plugin from this repository for your events by enabling it in
    the 'plugins' tab in the settings.
```

### Comparing `pretix-pages-1.5.2/pretix_pages.egg-info/SOURCES.txt` & `pretix-pages-1.5.3/pretix_pages.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 pretix_pages/__init__.py
 pretix_pages/apps.py
 pretix_pages/models.py
 pretix_pages/signals.py
 pretix_pages/urls.py
```


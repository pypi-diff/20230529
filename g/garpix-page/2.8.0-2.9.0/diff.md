# Comparing `tmp/garpix_page-2.8.0.tar.gz` & `tmp/garpix_page-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_page-2.8.0.tar", last modified: Fri Sep 10 13:37:18 2021, max compression
+gzip compressed data, was "garpix_page-2.9.0.tar", last modified: Tue Sep 14 20:27:38 2021, max compression
```

## Comparing `garpix_page-2.8.0.tar` & `garpix_page-2.9.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.801728 garpix_page-2.8.0/
--rw-r--r--   0 crusat     (501) staff       (20)       32 2021-09-10 13:37:18.000000 garpix_page-2.8.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     9899 2021-09-10 13:37:18.801453 garpix_page-2.8.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.784378 garpix_page-2.8.0/garpix_page/
--rw-r--r--   0 crusat     (501) staff       (20)       32 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     9239 2021-08-06 09:11:54.000000 garpix_page-2.8.0/garpix_page/README.rst
--rw-r--r--   0 crusat     (501) staff       (20)       57 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785406 garpix_page-2.8.0/garpix_page/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      213 2021-08-03 11:35:09.000000 garpix_page-2.8.0/garpix_page/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      487 2021-08-03 11:35:09.000000 garpix_page-2.8.0/garpix_page/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3231 2021-09-10 13:34:39.000000 garpix_page-2.8.0/garpix_page/__pycache__/codegenerator.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     4480 2021-09-10 13:21:54.000000 garpix_page-2.8.0/garpix_page/__pycache__/constants.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785602 garpix_page-2.8.0/garpix_page/admin/
--rw-r--r--   0 crusat     (501) staff       (20)       94 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/admin/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785799 garpix_page-2.8.0/garpix_page/admin/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      250 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3612 2021-09-08 09:21:08.000000 garpix_page-2.8.0/garpix_page/admin/__pycache__/base_page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3472 2021-09-08 09:21:07.000000 garpix_page-2.8.0/garpix_page/admin/base_page.py
--rw-r--r--   0 crusat     (501) staff       (20)      182 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/apps.py
--rw-r--r--   0 crusat     (501) staff       (20)     5092 2021-09-10 13:34:33.000000 garpix_page-2.8.0/garpix_page/codegenerator.py
--rw-r--r--   0 crusat     (501) staff       (20)     4528 2021-09-10 13:21:48.000000 garpix_page-2.8.0/garpix_page/constants.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785904 garpix_page-2.8.0/garpix_page/locale/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/locale/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785987 garpix_page-2.8.0/garpix_page/locale/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      164 2021-09-08 07:23:20.000000 garpix_page-2.8.0/garpix_page/locale/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.782189 garpix_page-2.8.0/garpix_page/locale/en/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.786089 garpix_page-2.8.0/garpix_page/locale/en/LC_MESSAGES/
--rw-r--r--   0 crusat     (501) staff       (20)      681 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.782290 garpix_page-2.8.0/garpix_page/locale/ru_RU/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.786192 garpix_page-2.8.0/garpix_page/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 crusat     (501) staff       (20)      646 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.786290 garpix_page-2.8.0/garpix_page/management/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-08 17:27:57.000000 garpix_page-2.8.0/garpix_page/management/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.786373 garpix_page-2.8.0/garpix_page/management/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      168 2021-09-08 17:29:45.000000 garpix_page-2.8.0/garpix_page/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.796104 garpix_page-2.8.0/garpix_page/management/commands/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-08 17:28:12.000000 garpix_page-2.8.0/garpix_page/management/commands/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.796432 garpix_page-2.8.0/garpix_page/management/commands/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      177 2021-09-08 17:29:45.000000 garpix_page-2.8.0/garpix_page/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1058 2021-09-09 16:27:12.000000 garpix_page-2.8.0/garpix_page/management/commands/__pycache__/startpage.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      644 2021-09-09 16:27:10.000000 garpix_page-2.8.0/garpix_page/management/commands/startpage.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.796554 garpix_page-2.8.0/garpix_page/migrations/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/migrations/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.796655 garpix_page-2.8.0/garpix_page/migrations/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      168 2021-09-08 07:23:20.000000 garpix_page-2.8.0/garpix_page/migrations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.797070 garpix_page-2.8.0/garpix_page/models/
--rw-r--r--   0 crusat     (501) staff       (20)      142 2021-09-08 10:03:05.000000 garpix_page-2.8.0/garpix_page/models/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.797539 garpix_page-2.8.0/garpix_page/models/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      312 2021-09-08 10:03:06.000000 garpix_page-2.8.0/garpix_page/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1183 2021-09-08 10:22:49.000000 garpix_page-2.8.0/garpix_page/models/__pycache__/base_list_page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     5666 2021-09-08 09:39:14.000000 garpix_page-2.8.0/garpix_page/models/__pycache__/base_page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1659 2021-09-08 11:04:50.000000 garpix_page-2.8.0/garpix_page/models/__pycache__/base_search_page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      814 2021-09-08 10:22:48.000000 garpix_page-2.8.0/garpix_page/models/base_list_page.py
--rw-r--r--   0 crusat     (501) staff       (20)     5711 2021-09-08 09:39:13.000000 garpix_page-2.8.0/garpix_page/models/base_page.py
--rw-r--r--   0 crusat     (501) staff       (20)     1541 2021-09-08 11:04:48.000000 garpix_page-2.8.0/garpix_page/models/base_search_page.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.797779 garpix_page-2.8.0/garpix_page/serializers/
--rw-r--r--   0 crusat     (501) staff       (20)       47 2021-09-08 07:24:34.000000 garpix_page-2.8.0/garpix_page/serializers/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.798018 garpix_page-2.8.0/garpix_page/serializers/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      218 2021-09-08 07:25:08.000000 garpix_page-2.8.0/garpix_page/serializers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      501 2021-08-06 09:16:37.000000 garpix_page-2.8.0/garpix_page/serializers/__pycache__/serializer.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      365 2021-08-06 09:11:54.000000 garpix_page-2.8.0/garpix_page/serializers/serializer.py
--rw-r--r--   0 crusat     (501) staff       (20)     1306 2021-09-10 13:36:45.000000 garpix_page-2.8.0/garpix_page/setup.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.782974 garpix_page-2.8.0/garpix_page/templates/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.798989 garpix_page-2.8.0/garpix_page/templates/garpix_page/
--rw-r--r--   0 crusat     (501) staff       (20)     1207 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/admin_toolbar.html
--rw-r--r--   0 crusat     (501) staff       (20)      449 2021-09-10 13:18:29.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/base.html
--rw-r--r--   0 crusat     (501) staff       (20)      423 2021-09-10 13:16:51.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/breadcrumb.html
--rw-r--r--   0 crusat     (501) staff       (20)      106 2021-09-08 08:24:29.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/default.html
--rw-r--r--   0 crusat     (501) staff       (20)      353 2021-09-08 10:28:31.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/default_list.html
--rw-r--r--   0 crusat     (501) staff       (20)      794 2021-09-08 10:28:31.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/default_search.html
--rw-r--r--   0 crusat     (501) staff       (20)      561 2021-09-08 07:49:52.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/index.html
--rw-r--r--   0 crusat     (501) staff       (20)      402 2021-09-08 10:47:28.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/pagination.html
--rw-r--r--   0 crusat     (501) staff       (20)      824 2021-08-03 12:11:34.000000 garpix_page-2.8.0/garpix_page/templates/garpix_page/seo.html
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.799186 garpix_page-2.8.0/garpix_page/translation/
--rw-r--r--   0 crusat     (501) staff       (20)       58 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/translation/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.799390 garpix_page-2.8.0/garpix_page/translation/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      229 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      563 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/translation/__pycache__/base_page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      260 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/translation/base_page.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.799793 garpix_page-2.8.0/garpix_page/utils/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.800228 garpix_page-2.8.0/garpix_page/utils/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      590 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/utils/__pycache__/check_redirect.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      829 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/utils/__pycache__/get_file_path.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      514 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/utils/__pycache__/get_garpix_page_models.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      425 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/utils/check_redirect.py
--rw-r--r--   0 crusat     (501) staff       (20)      919 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/utils/check_sites.py
--rw-r--r--   0 crusat     (501) staff       (20)      598 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/utils/get_file_path.py
--rw-r--r--   0 crusat     (501) staff       (20)      307 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/utils/get_garpix_page_models.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.800749 garpix_page-2.8.0/garpix_page/views/
--rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.8.0/garpix_page/views/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.801271 garpix_page-2.8.0/garpix_page/views/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      163 2021-08-03 11:35:10.000000 garpix_page-2.8.0/garpix_page/views/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      423 2021-09-08 07:21:09.000000 garpix_page-2.8.0/garpix_page/views/__pycache__/index.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3695 2021-09-08 07:20:59.000000 garpix_page-2.8.0/garpix_page/views/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1957 2021-09-08 07:25:08.000000 garpix_page-2.8.0/garpix_page/views/__pycache__/page_api.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      570 2021-09-08 11:12:45.000000 garpix_page-2.8.0/garpix_page/views/__pycache__/sitemap.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      129 2021-09-08 07:21:09.000000 garpix_page-2.8.0/garpix_page/views/index.py
--rw-r--r--   0 crusat     (501) staff       (20)     4229 2021-09-08 07:20:58.000000 garpix_page-2.8.0/garpix_page/views/page.py
--rw-r--r--   0 crusat     (501) staff       (20)     1942 2021-09-08 07:24:29.000000 garpix_page-2.8.0/garpix_page/views/page_api.py
--rw-r--r--   0 crusat     (501) staff       (20)      420 2021-09-08 11:10:44.000000 garpix_page-2.8.0/garpix_page/views/sitemap.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-10 13:37:18.785009 garpix_page-2.8.0/garpix_page.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     9899 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)     3290 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)      143 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       12 2021-09-10 13:37:18.000000 garpix_page-2.8.0/garpix_page.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2021-09-10 13:37:18.801774 garpix_page-2.8.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1306 2021-09-10 13:37:18.000000 garpix_page-2.8.0/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.022765 garpix_page-2.9.0/
+-rw-r--r--   0 crusat     (501) staff       (20)       32 2021-09-14 20:27:37.000000 garpix_page-2.9.0/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     9899 2021-09-14 20:27:38.022515 garpix_page-2.9.0/PKG-INFO
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.011296 garpix_page-2.9.0/garpix_page/
+-rw-r--r--   0 crusat     (501) staff       (20)       32 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/MANIFEST.in
+-rw-r--r--   0 crusat     (501) staff       (20)     9239 2021-08-06 09:11:54.000000 garpix_page-2.9.0/garpix_page/README.rst
+-rw-r--r--   0 crusat     (501) staff       (20)       57 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.015628 garpix_page-2.9.0/garpix_page/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      213 2021-08-03 11:35:09.000000 garpix_page-2.9.0/garpix_page/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      487 2021-08-03 11:35:09.000000 garpix_page-2.9.0/garpix_page/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     3231 2021-09-10 13:34:39.000000 garpix_page-2.9.0/garpix_page/__pycache__/codegenerator.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     4480 2021-09-10 13:21:54.000000 garpix_page-2.9.0/garpix_page/__pycache__/constants.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.015931 garpix_page-2.9.0/garpix_page/admin/
+-rw-r--r--   0 crusat     (501) staff       (20)       94 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/admin/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016219 garpix_page-2.9.0/garpix_page/admin/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      250 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     4183 2021-09-13 16:00:16.000000 garpix_page-2.9.0/garpix_page/admin/__pycache__/base_page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     4054 2021-09-13 16:00:15.000000 garpix_page-2.9.0/garpix_page/admin/base_page.py
+-rw-r--r--   0 crusat     (501) staff       (20)      182 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/apps.py
+-rw-r--r--   0 crusat     (501) staff       (20)     5092 2021-09-10 13:34:33.000000 garpix_page-2.9.0/garpix_page/codegenerator.py
+-rw-r--r--   0 crusat     (501) staff       (20)     4528 2021-09-10 13:21:48.000000 garpix_page-2.9.0/garpix_page/constants.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016337 garpix_page-2.9.0/garpix_page/locale/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/locale/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016424 garpix_page-2.9.0/garpix_page/locale/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      164 2021-09-08 07:23:20.000000 garpix_page-2.9.0/garpix_page/locale/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.005605 garpix_page-2.9.0/garpix_page/locale/en/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016538 garpix_page-2.9.0/garpix_page/locale/en/LC_MESSAGES/
+-rw-r--r--   0 crusat     (501) staff       (20)      681 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.005729 garpix_page-2.9.0/garpix_page/locale/ru_RU/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016648 garpix_page-2.9.0/garpix_page/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 crusat     (501) staff       (20)      646 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016753 garpix_page-2.9.0/garpix_page/management/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-08 17:27:57.000000 garpix_page-2.9.0/garpix_page/management/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.016836 garpix_page-2.9.0/garpix_page/management/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      168 2021-09-08 17:29:45.000000 garpix_page-2.9.0/garpix_page/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.017032 garpix_page-2.9.0/garpix_page/management/commands/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-09-08 17:28:12.000000 garpix_page-2.9.0/garpix_page/management/commands/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.017248 garpix_page-2.9.0/garpix_page/management/commands/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      177 2021-09-08 17:29:45.000000 garpix_page-2.9.0/garpix_page/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1058 2021-09-09 16:27:12.000000 garpix_page-2.9.0/garpix_page/management/commands/__pycache__/startpage.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      644 2021-09-09 16:27:10.000000 garpix_page-2.9.0/garpix_page/management/commands/startpage.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.017363 garpix_page-2.9.0/garpix_page/migrations/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/migrations/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.017450 garpix_page-2.9.0/garpix_page/migrations/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      168 2021-09-08 07:23:20.000000 garpix_page-2.9.0/garpix_page/migrations/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.018007 garpix_page-2.9.0/garpix_page/models/
+-rw-r--r--   0 crusat     (501) staff       (20)      142 2021-09-08 10:03:05.000000 garpix_page-2.9.0/garpix_page/models/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.018433 garpix_page-2.9.0/garpix_page/models/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      312 2021-09-08 10:03:06.000000 garpix_page-2.9.0/garpix_page/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1190 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page/models/__pycache__/base_list_page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     5666 2021-09-08 09:39:14.000000 garpix_page-2.9.0/garpix_page/models/__pycache__/base_page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1666 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page/models/__pycache__/base_search_page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      827 2021-09-14 20:22:58.000000 garpix_page-2.9.0/garpix_page/models/base_list_page.py
+-rw-r--r--   0 crusat     (501) staff       (20)     5711 2021-09-08 09:39:13.000000 garpix_page-2.9.0/garpix_page/models/base_page.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1554 2021-09-14 20:23:34.000000 garpix_page-2.9.0/garpix_page/models/base_search_page.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.018649 garpix_page-2.9.0/garpix_page/serializers/
+-rw-r--r--   0 crusat     (501) staff       (20)       47 2021-09-08 07:24:34.000000 garpix_page-2.9.0/garpix_page/serializers/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.018855 garpix_page-2.9.0/garpix_page/serializers/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      218 2021-09-08 07:25:08.000000 garpix_page-2.9.0/garpix_page/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      501 2021-08-06 09:16:37.000000 garpix_page-2.9.0/garpix_page/serializers/__pycache__/serializer.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      365 2021-08-06 09:11:54.000000 garpix_page-2.9.0/garpix_page/serializers/serializer.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1338 2021-09-14 20:22:58.000000 garpix_page-2.9.0/garpix_page/setup.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.006467 garpix_page-2.9.0/garpix_page/templates/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.019822 garpix_page-2.9.0/garpix_page/templates/garpix_page/
+-rw-r--r--   0 crusat     (501) staff       (20)     1207 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/admin_toolbar.html
+-rw-r--r--   0 crusat     (501) staff       (20)      449 2021-09-10 13:18:29.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/base.html
+-rw-r--r--   0 crusat     (501) staff       (20)      423 2021-09-10 13:16:51.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/breadcrumb.html
+-rw-r--r--   0 crusat     (501) staff       (20)      106 2021-09-08 08:24:29.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/default.html
+-rw-r--r--   0 crusat     (501) staff       (20)      353 2021-09-08 10:28:31.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/default_list.html
+-rw-r--r--   0 crusat     (501) staff       (20)      794 2021-09-08 10:28:31.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/default_search.html
+-rw-r--r--   0 crusat     (501) staff       (20)      561 2021-09-08 07:49:52.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/index.html
+-rw-r--r--   0 crusat     (501) staff       (20)      415 2021-09-14 20:11:02.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/pagination.html
+-rw-r--r--   0 crusat     (501) staff       (20)      824 2021-08-03 12:11:34.000000 garpix_page-2.9.0/garpix_page/templates/garpix_page/seo.html
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.020024 garpix_page-2.9.0/garpix_page/translation/
+-rw-r--r--   0 crusat     (501) staff       (20)       58 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/translation/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.020235 garpix_page-2.9.0/garpix_page/translation/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      229 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      563 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/translation/__pycache__/base_page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      260 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/translation/base_page.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.020664 garpix_page-2.9.0/garpix_page/utils/
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.021024 garpix_page-2.9.0/garpix_page/utils/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      590 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/utils/__pycache__/check_redirect.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      829 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/utils/__pycache__/get_file_path.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      514 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/utils/__pycache__/get_garpix_page_models.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      425 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/utils/check_redirect.py
+-rw-r--r--   0 crusat     (501) staff       (20)      919 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/utils/check_sites.py
+-rw-r--r--   0 crusat     (501) staff       (20)      598 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/utils/get_file_path.py
+-rw-r--r--   0 crusat     (501) staff       (20)      307 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/utils/get_garpix_page_models.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.021614 garpix_page-2.9.0/garpix_page/views/
+-rw-r--r--   0 crusat     (501) staff       (20)        0 2021-08-03 11:25:10.000000 garpix_page-2.9.0/garpix_page/views/__init__.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.022276 garpix_page-2.9.0/garpix_page/views/__pycache__/
+-rw-r--r--   0 crusat     (501) staff       (20)      163 2021-08-03 11:35:10.000000 garpix_page-2.9.0/garpix_page/views/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      423 2021-09-08 07:21:09.000000 garpix_page-2.9.0/garpix_page/views/__pycache__/index.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     3695 2021-09-08 07:20:59.000000 garpix_page-2.9.0/garpix_page/views/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)     1957 2021-09-08 07:25:08.000000 garpix_page-2.9.0/garpix_page/views/__pycache__/page_api.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      570 2021-09-08 11:12:45.000000 garpix_page-2.9.0/garpix_page/views/__pycache__/sitemap.cpython-38.pyc
+-rw-r--r--   0 crusat     (501) staff       (20)      129 2021-09-08 07:21:09.000000 garpix_page-2.9.0/garpix_page/views/index.py
+-rw-r--r--   0 crusat     (501) staff       (20)     4229 2021-09-08 07:20:58.000000 garpix_page-2.9.0/garpix_page/views/page.py
+-rw-r--r--   0 crusat     (501) staff       (20)     1942 2021-09-08 07:24:29.000000 garpix_page-2.9.0/garpix_page/views/page_api.py
+-rw-r--r--   0 crusat     (501) staff       (20)      420 2021-09-08 11:10:44.000000 garpix_page-2.9.0/garpix_page/views/sitemap.py
+drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-14 20:27:38.011905 garpix_page-2.9.0/garpix_page.egg-info/
+-rw-r--r--   0 crusat     (501) staff       (20)     9899 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/PKG-INFO
+-rw-r--r--   0 crusat     (501) staff       (20)     3290 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/SOURCES.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/dependency_links.txt
+-rw-r--r--   0 crusat     (501) staff       (20)        1 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/not-zip-safe
+-rw-r--r--   0 crusat     (501) staff       (20)      163 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/requires.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       12 2021-09-14 20:27:37.000000 garpix_page-2.9.0/garpix_page.egg-info/top_level.txt
+-rw-r--r--   0 crusat     (501) staff       (20)       38 2021-09-14 20:27:38.022817 garpix_page-2.9.0/setup.cfg
+-rw-r--r--   0 crusat     (501) staff       (20)     1338 2021-09-14 20:27:37.000000 garpix_page-2.9.0/setup.py
```

### Comparing `garpix_page-2.8.0/PKG-INFO` & `garpix_page-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_page
-Version: 2.8.0
+Version: 2.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/garpixcms/garpix_page
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `garpix_page-2.8.0/garpix_page/README.rst` & `garpix_page-2.9.0/garpix_page/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/__pycache__/codegenerator.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/__pycache__/codegenerator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/__pycache__/constants.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/__pycache__/constants.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/admin/__pycache__/base_page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/admin/__pycache__/base_page.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Sep  8 09:21:07 2021 UTC, .py size: 3472 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,226 +1,262 @@
-00000000: 550d 0d0a 0000 0000 8380 3861 900d 0000  U.........8a....
+00000000: 550d 0d0a 0000 0000 8f75 3f61 d60f 0000  U........u?a....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000020: 0006 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6402 6406 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6407 6c0b 6d0c 5a0c 0100 4700 6408 6409  d.l.m.Z...G.d.d.
-00000080: 8400 6409 6505 6508 8304 5a0d 6501 a00e  ..d.e.e...Z.e...
-00000090: 6503 a101 4700 640a 640b 8400 640b 6505  e...G.d.d...d.e.
-000000a0: 6507 8304 8301 5a0f 640c 5300 290d e900  e.....Z.d.S.)...
-000000b0: 0000 0029 01da 0561 646d 696e e902 0000  ...)...admin....
-000000c0: 0029 01da 0842 6173 6550 6167 6529 01da  .)...BasePage)..
-000000d0: 1654 6162 6265 6454 7261 6e73 6c61 7469  .TabbedTranslati
-000000e0: 6f6e 4164 6d69 6e29 02da 1f50 6f6c 796d  onAdmin)...Polym
-000000f0: 6f72 7068 6963 4d50 5454 5061 7265 6e74  orphicMPTTParent
-00000100: 4d6f 6465 6c41 646d 696e da1e 506f 6c79  ModelAdmin..Poly
-00000110: 6d6f 7270 6869 634d 5054 5443 6869 6c64  morphicMPTTChild
-00000120: 4d6f 6465 6c41 646d 696e 2901 da16 6765  ModelAdmin)...ge
-00000130: 745f 6761 7270 6978 5f70 6167 655f 6d6f  t_garpix_page_mo
-00000140: 6465 6c73 2901 da08 7365 7474 696e 6773  dels)...settings
-00000150: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000160: 0003 0000 0000 0000 0073 6400 0000 6500  .........sd...e.
-00000170: 5a01 6400 5a02 6503 5a04 6505 6506 6401  Z.d.Z.e.Z.e.e.d.
-00000180: 8302 721c 6506 6a07 6e02 6402 5a08 6403  ..r.e.j.n.d.Z.d.
-00000190: 5a09 6404 5a0a 6404 5a0b 6405 5a0c 6406  Z.d.Z.d.Z.d.Z.d.
-000001a0: 6407 6901 5a0d 6407 5a0e 6408 5a0f 6409  d.i.Z.d.Z.d.Z.d.
-000001b0: 5a10 640a 5a11 640b 5a12 640c 5a13 8700  Z.d.Z.d.Z.d.Z...
-000001c0: 6601 640d 640e 8408 5a14 8700 0400 5a15  f.d.d...Z.....Z.
-000001d0: 5300 290f da0d 4261 7365 5061 6765 4164  S.)...BasePageAd
-000001e0: 6d69 6eda 1f47 4152 5049 585f 5041 4745  min..GARPIX_PAGE
-000001f0: 5f41 444d 494e 5f4c 4953 545f 5045 525f  _ADMIN_LIST_PER_
-00000200: 5041 4745 e919 0000 00f5 0a00 0000 2d20  PAGE..........- 
-00000210: d0bd d0b5 d182 202d 54da 0a63 7265 6174  ...... -T..creat
-00000220: 6564 5f61 74da 0473 6c75 67a9 01da 0574  ed_at..slug....t
-00000230: 6974 6c65 a903 da09 6973 5f61 6374 6976  itle....is_activ
-00000240: 6572 0e00 0000 da0a 7570 6461 7465 645f  er......updated_
-00000250: 6174 a902 da0c 636c 6f6e 655f 6f62 6a65  at....clone_obje
-00000260: 6374 da07 7265 6275 696c 6429 0472 1100  ct..rebuild).r..
-00000270: 0000 720e 0000 0072 1300 0000 da10 6765  ..r....r......ge
-00000280: 745f 6162 736f 6c75 7465 5f75 726c a901  t_absolute_url..
-00000290: 7213 0000 00a9 0272 0e00 0000 7214 0000  r......r....r...
-000002a0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-000002b0: 0000 0300 0000 0f00 0000 7318 0000 0074  ..........s....t
-000002c0: 0083 006a 017c 0166 017c 029e 027c 038e  ...j.|.f.|...|..
-000002d0: 017d 047c 0453 00a9 014e 2902 da05 7375  .}.|.S...N)...su
-000002e0: 7065 72da 0867 6574 5f66 6f72 6d29 05da  per..get_form)..
-000002f0: 0473 656c 66da 0772 6571 7565 7374 da04  .self..request..
-00000300: 6172 6773 da06 6b77 6172 6773 da04 666f  args..kwargs..fo
-00000310: 726d a901 da09 5f5f 636c 6173 735f 5fa9  rm....__class__.
-00000320: 00fa 492f 5573 6572 732f 6372 7573 6174  ..I/Users/crusat
-00000330: 2f70 726f 6a65 6374 732f 6761 7270 6978  /projects/garpix
-00000340: 5f70 6167 652f 6261 636b 656e 642f 6761  _page/backend/ga
-00000350: 7270 6978 5f70 6167 652f 6164 6d69 6e2f  rpix_page/admin/
-00000360: 6261 7365 5f70 6167 652e 7079 721d 0000  base_page.pyr...
-00000370: 001e 0000 0073 0400 0000 0001 1402 7a16  .....s........z.
-00000380: 4261 7365 5061 6765 4164 6d69 6e2e 6765  BasePageAdmin.ge
-00000390: 745f 666f 726d 2916 da08 5f5f 6e61 6d65  t_form)...__name
-000003a0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000003b0: 5f5f 7175 616c 6e61 6d65 5f5f 7204 0000  __qualname__r...
-000003c0: 00da 0a62 6173 655f 6d6f 6465 6cda 0768  ...base_model..h
-000003d0: 6173 6174 7472 7209 0000 0072 0b00 0000  asattrr....r....
-000003e0: da0d 6c69 7374 5f70 6572 5f70 6167 65da  ..list_per_page.
-000003f0: 1365 6d70 7479 5f76 616c 7565 5f64 6973  .empty_value_dis
-00000400: 706c 6179 da0b 7361 7665 5f6f 6e5f 746f  play..save_on_to
-00000410: 70da 0c76 6965 775f 6f6e 5f73 6974 65da  p..view_on_site.
-00000420: 0e64 6174 655f 6869 6572 6172 6368 79da  .date_hierarchy.
-00000430: 1370 7265 706f 7075 6c61 7465 645f 6669  .prepopulated_fi
-00000440: 656c 6473 da0d 7365 6172 6368 5f66 6965  elds..search_fie
-00000450: 6c64 73da 0b6c 6973 745f 6669 6c74 6572  lds..list_filter
-00000460: da07 6163 7469 6f6e 73da 0c6c 6973 745f  ..actions..list_
-00000470: 6469 7370 6c61 79da 0d6c 6973 745f 6564  display..list_ed
-00000480: 6974 6162 6c65 da0f 7265 6164 6f6e 6c79  itable..readonly
-00000490: 5f66 6965 6c64 7372 1d00 0000 da0d 5f5f  _fieldsr......__
-000004a0: 636c 6173 7363 656c 6c5f 5f72 2500 0000  classcell__r%...
-000004b0: 7225 0000 0072 2300 0000 7226 0000 0072  r%...r#...r&...r
-000004c0: 0a00 0000 0900 0000 731c 0000 0008 0104  ........s.......
-000004d0: 0214 0204 0104 0104 0204 0108 0204 0104  ................
-000004e0: 0104 0204 0104 0204 0272 0a00 0000 6300  .........r....c.
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000500: 0000 0000 0000 0073 9e00 0000 6500 5a01  .......s....e.Z.
-00000510: 6400 5a02 6401 5a03 6504 5a05 6506 8300  d.Z.d.Z.e.Z.e...
-00000520: 5a07 6508 6509 6402 8302 7226 6509 6a0a  Z.e.e.d...r&e.j.
-00000530: 6e02 6403 5a0b 6404 5a0c 6405 5a0d 6405  n.d.Z.d.Z.d.Z.d.
-00000540: 5a0e 6406 5a0f 6407 6408 6901 5a10 6408  Z.d.Z.d.d.i.Z.d.
-00000550: 5a11 6409 5a12 640a 5a13 640b 5a14 640c  Z.d.Z.d.Z.d.Z.d.
-00000560: 5a15 640d 5a16 8700 6601 640e 640f 8408  Z.d.Z...f.d.d...
-00000570: 5a17 6410 6411 8400 5a18 6412 6518 5f19  Z.d.d...Z.d.e._.
-00000580: 6413 6414 8400 5a1a 6415 6416 8400 5a1b  d.d...Z.d.d...Z.
-00000590: 6417 651b 5f19 8700 6601 6418 6419 8408  d.e._...f.d.d...
-000005a0: 5a1c 8700 0400 5a1d 5300 291a da11 5265  Z.....Z.S.)...Re
-000005b0: 616c 4261 7365 5061 6765 4164 6d69 6e75  alBasePageAdminu
-000005c0: 5900 0000 0a20 2020 20d0 a1d1 82d0 b0d0  Y....    .......
-000005d0: bdd0 b4d0 b0d1 80d1 82d0 bdd1 8bd0 b520  ............... 
-000005e0: d0bd d0b0 d181 d182 d180 d0be d0b9 d0ba  ................
-000005f0: d0b8 20d0 b4d0 bbd1 8f20 d0b1 d0b0 d0b7  .. ...... ......
-00000600: d0be d0b2 d18b d185 20d1 81d1 82d1 80d0  ........ .......
-00000610: b0d0 bdd0 b8d1 862e 0a20 2020 2072 0b00  .........    r..
-00000620: 0000 720c 0000 0072 0d00 0000 5472 0e00  ..r....r....Tr..
-00000630: 0000 720f 0000 0072 1000 0000 7212 0000  ..r....r....r...
-00000640: 0072 1500 0000 2904 7211 0000 0072 0e00  .r....).r....r..
-00000650: 0000 7213 0000 00da 1567 6574 5f61 6273  ..r......get_abs
-00000660: 6f6c 7574 655f 7572 6c5f 6874 6d6c 7219  olute_url_htmlr.
-00000670: 0000 0072 1a00 0000 6301 0000 0000 0000  ...r....c.......
-00000680: 0000 0000 0003 0000 0003 0000 000f 0000  ................
-00000690: 0073 3e00 0000 7400 8300 6a01 7c01 7c02  .s>...t...j.|.|.
-000006a0: 8e01 0100 6401 7c02 6b06 723a 7c00 6a02  ....d.|.k.r:|.j.
-000006b0: a003 a100 7c00 6a04 6402 1900 5f05 7c00  ....|.j.d..._.|.
-000006c0: 6a02 a006 a100 7c00 6a04 6402 1900 5f07  j.....|.j.d..._.
-000006d0: 6400 5300 2903 4eda 0769 6e69 7469 616c  d.S.).N..initial
-000006e0: da06 7061 7265 6e74 2908 721c 0000 00da  ..parent).r.....
-000006f0: 085f 5f69 6e69 745f 5fda 056d 6f64 656c  .__init__..model
-00000700: 5a1a 6765 745f 6176 6169 6c61 626c 655f  Z.get_available_
-00000710: 7061 6765 5f70 6172 656e 7473 da06 6669  page_parents..fi
-00000720: 656c 6473 da08 7175 6572 7973 6574 5a12  elds..querysetZ.
-00000730: 6765 745f 6465 6661 756c 745f 7061 7265  get_default_pare
-00000740: 6e74 da07 6465 6661 756c 7429 0372 1e00  nt..default).r..
-00000750: 0000 7220 0000 0072 2100 0000 7223 0000  ..r ...r!...r#..
-00000760: 0072 2500 0000 7226 0000 0072 3d00 0000  .r%...r&...r=...
-00000770: 3e00 0000 7308 0000 0000 010e 0108 0112  >...s...........
-00000780: 017a 1a52 6561 6c42 6173 6550 6167 6541  .z.RealBasePageA
-00000790: 646d 696e 2e5f 5f69 6e69 745f 5f63 0300  dmin.__init__c..
-000007a0: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-000007b0: 0000 4300 0000 7346 0000 007c 0244 005d  ..C...sF...|.D.]
-000007c0: 3c7d 0364 017d 047c 037d 057c 0504 006a  <}.d.}.|.}.|...j
-000007d0: 007c 0437 0002 005f 007c 0504 006a 017c  .|.7..._.|...j.|
-000007e0: 0437 0002 005f 0164 027c 055f 0264 037c  .7..._.d.|._.d.|
-000007f0: 055f 037c 05a0 04a1 0001 0071 0464 0253  ._.|.......q.d.S
-00000800: 0029 0475 5d00 0000 d09a d0be d0bf d0b8  .).u]...........
-00000810: d180 d0be d0b2 d0b0 d0bd d0b8 d0b5 28d0  ..............(.
-00000820: bad0 bbd0 bed0 bdd0 b8d1 80d0 bed0 b2d0  ................
-00000830: b0d0 bdd0 b8d0 b529 20d0 b2d1 8bd0 b1d1  .......) .......
-00000840: 80d0 b0d0 bdd0 bdd1 8bd1 8520 d0be d0b1  ........... ....
-00000850: d18a d0b5 d0ba d182 d0be d0b2 202d 2061  ............ - a
-00000860: 6374 696f 6e7a 062d 434c 4f4e 454e 4629  ctionz.-CLONENF)
-00000870: 0572 1100 0000 720f 0000 00da 0269 6472  .r....r......idr
-00000880: 1300 0000 da04 7361 7665 2906 721e 0000  ......save).r...
-00000890: 0072 1f00 0000 7240 0000 00da 036f 626a  .r....r@.....obj
-000008a0: da06 7072 6566 6978 da05 636c 6f6e 6572  ..prefix..cloner
-000008b0: 2500 0000 7225 0000 0072 2600 0000 7216  %...r%...r&...r.
-000008c0: 0000 0044 0000 0073 1000 0000 0002 0801  ...D...s........
-000008d0: 0401 0401 0e01 0e01 0601 0601 7a1e 5265  ............z.Re
-000008e0: 616c 4261 7365 5061 6765 4164 6d69 6e2e  alBasePageAdmin.
-000008f0: 636c 6f6e 655f 6f62 6a65 6374 7523 0000  clone_objectu#..
-00000900: 00d0 9ad0 bbd0 bed0 bdd0 b8d1 80d0 bed0  ................
-00000910: b2d0 b0d1 82d1 8c20 d0be d0b1 d18a d0b5  ....... ........
-00000920: d0ba d182 6301 0000 0000 0000 0000 0000  ....c...........
-00000930: 0001 0000 0006 0000 0043 0000 0073 2a00  .........C...s*.
-00000940: 0000 7a10 7c00 6a00 6a01 a002 a100 0100  ..z.|.j.j.......
-00000950: 5700 6e14 0100 0100 0100 7403 6401 8301  W.n.......t.d...
-00000960: 0100 5900 6e02 5800 6400 5300 2902 4e75  ..Y.n.X.d.S.).Nu
-00000970: 5f00 0000 5b45 5252 4f52 5d3a 20d0 9ed1  _...[ERROR]: ...
-00000980: 88d0 b8d0 b1d0 bad0 b020 d0bf d180 d0b8  ......... ......
-00000990: 20d0 bfd0 b5d1 80d0 b5d0 b7d0 b0d0 b3d1   ...............
-000009a0: 80d1 83d0 b7d0 bad0 b820 d0b4 d180 d0b5  ......... ......
-000009b0: d0b2 d0be d0b2 d0b8 d0b4 d0bd d0be d0b9  ................
-000009c0: 20d1 81d1 82d1 80d1 83d0 bad1 82d1 83d1   ...............
-000009d0: 80d1 8b29 0472 3e00 0000 da07 6f62 6a65  ...).r>.....obje
-000009e0: 6374 7372 1700 0000 da05 7072 696e 7429  ctsr......print)
-000009f0: 0172 1e00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00000a00: 7226 0000 00da 085f 7265 6275 696c 6451  r&....._rebuildQ
-00000a10: 0000 0073 0800 0000 0001 0201 1001 0601  ...s............
-00000a20: 7a1a 5265 616c 4261 7365 5061 6765 4164  z.RealBasePageAd
-00000a30: 6d69 6e2e 5f72 6562 7569 6c64 6303 0000  min._rebuildc...
-00000a40: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00000a50: 0043 0000 0073 0c00 0000 7c00 a000 a100  .C...s....|.....
-00000a60: 0100 6401 5300 2902 757b 0000 00d0 9fd0  ..d.S.).u{......
-00000a70: b5d1 80d0 b5d1 81d0 bed1 80d0 b1d0 b0d1  ................
-00000a80: 82d1 8c20 d09c d09f d0a2 d0a2 20d0 bcd0  ... ........ ...
-00000a90: bed0 b4d0 b5d0 bbd1 8c2e 20d0 98d0 bdd0  .......... .....
-00000aa0: bed0 b3d0 b4d0 b020 d182 d180 d0b5 d0b1  ....... ........
-00000ab0: d183 d0b5 d182 d181 d18f 20d0 b4d0 bbd1  .......... .....
-00000ac0: 8f20 d0bf d0b5 d180 d0b5 d0b7 d0b0 d0b3  . ..............
-00000ad0: d180 d183 d0b7 d0ba d0b8 20d0 b4d0 b5d1  .......... .....
-00000ae0: 80d0 b5d0 b2d0 b02e 4e29 0172 4900 0000  ........N).rI...
-00000af0: 2903 721e 0000 0072 1f00 0000 7240 0000  ).r....r....r@..
-00000b00: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00000b10: 7217 0000 0057 0000 0073 0200 0000 0002  r....W...s......
-00000b20: 7a19 5265 616c 4261 7365 5061 6765 4164  z.RealBasePageAd
-00000b30: 6d69 6e2e 7265 6275 696c 6475 3200 0000  min.rebuildu2...
-00000b40: d09f d0b5 d180 d0b5 d181 d0be d0b1 d180  ................
-00000b50: d0b0 d182 d18c 20d0 bfd1 83d0 bdd0 bad1  ...... .........
-00000b60: 82d1 8b20 d180 d0b0 d0b7 d0b4 d0b5 d0bb  ... ............
-00000b70: d0b0 6305 0000 0000 0000 0000 0000 0005  ..c.............
-00000b80: 0000 0006 0000 0003 0000 0073 1e00 0000  ...........s....
-00000b90: 7c00 a000 a100 0100 7401 8300 a002 7c01  |.......t.....|.
-00000ba0: 7c02 7c03 7c04 a104 0100 6400 5300 721b  |.|.|.....d.S.r.
-00000bb0: 0000 0029 0372 4900 0000 721c 0000 00da  ...).rI...r.....
-00000bc0: 0a73 6176 655f 6d6f 6465 6c29 0572 1e00  .save_model).r..
-00000bd0: 0000 721f 0000 0072 4400 0000 7222 0000  ..r....rD...r"..
-00000be0: 00da 0663 6861 6e67 6572 2300 0000 7225  ...changer#...r%
-00000bf0: 0000 0072 2600 0000 724a 0000 005d 0000  ...r&...rJ...]..
-00000c00: 0073 0400 0000 0001 0801 7a1c 5265 616c  .s........z.Real
-00000c10: 4261 7365 5061 6765 4164 6d69 6e2e 7361  BasePageAdmin.sa
-00000c20: 7665 5f6d 6f64 656c 291e 7227 0000 0072  ve_model).r'...r
-00000c30: 2800 0000 7229 0000 00da 075f 5f64 6f63  (...r).....__doc
-00000c40: 5f5f 7204 0000 0072 2a00 0000 7208 0000  __r....r*...r...
-00000c50: 00da 0c63 6869 6c64 5f6d 6f64 656c 7372  ...child_modelsr
-00000c60: 2b00 0000 7209 0000 0072 0b00 0000 722c  +...r....r....r,
-00000c70: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-00000c80: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
-00000c90: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
-00000ca0: 7236 0000 0072 3700 0000 723d 0000 0072  r6...r7...r=...r
-00000cb0: 1600 0000 da11 7368 6f72 745f 6465 7363  ......short_desc
-00000cc0: 7269 7074 696f 6e72 4900 0000 7217 0000  riptionrI...r...
-00000cd0: 0072 4a00 0000 7238 0000 0072 2500 0000  .rJ...r8...r%...
-00000ce0: 7225 0000 0072 2300 0000 7226 0000 0072  r%...r#...r&...r
-00000cf0: 3900 0000 2400 0000 732c 0000 0008 0204  9...$...s,......
-00000d00: 0304 0106 0214 0204 0104 0104 0204 0108  ................
-00000d10: 0204 0104 0104 0204 0104 0204 020c 0608  ................
-00000d20: 0b06 0208 0608 0406 0272 3900 0000 4e29  .........r9...N)
-00000d30: 105a 0e64 6a61 6e67 6f2e 636f 6e74 7269  .Z.django.contri
-00000d40: 6272 0200 0000 5a10 6d6f 6465 6c73 2e62  br....Z.models.b
-00000d50: 6173 655f 7061 6765 7204 0000 005a 166d  ase_pager....Z.m
-00000d60: 6f64 656c 7472 616e 736c 6174 696f 6e2e  odeltranslation.
-00000d70: 6164 6d69 6e72 0500 0000 5a16 706f 6c79  adminr....Z.poly
-00000d80: 6d6f 7270 6869 635f 7472 6565 2e61 646d  morphic_tree.adm
-00000d90: 696e 7206 0000 0072 0700 0000 5a1c 7574  inr....r....Z.ut
-00000da0: 696c 732e 6765 745f 6761 7270 6978 5f70  ils.get_garpix_p
-00000db0: 6167 655f 6d6f 6465 6c73 7208 0000 00da  age_modelsr.....
-00000dc0: 0b64 6a61 6e67 6f2e 636f 6e66 7209 0000  .django.confr...
-00000dd0: 0072 0a00 0000 da08 7265 6769 7374 6572  .r......register
-00000de0: 7239 0000 0072 2500 0000 7225 0000 0072  r9...r%...r%...r
-00000df0: 2500 0000 7226 0000 00da 083c 6d6f 6475  %...r&.....<modu
-00000e00: 6c65 3e01 0000 0073 1000 0000 0c01 0c01  le>....s........
-00000e10: 0c01 1001 0c01 0c03 121b 0801            ............
+00000070: 6407 6c0b 6d0c 5a0c 0100 6400 6408 6c0d  d.l.m.Z...d.d.l.
+00000080: 6d0e 5a0f 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+00000090: 6505 6508 8304 5a10 6501 a011 6503 a101  e.e...Z.e...e...
+000000a0: 4700 640b 640c 8400 640c 6505 6507 8304  G.d.d...d.e.e...
+000000b0: 8301 5a12 640d 5300 290e e900 0000 0029  ..Z.d.S.)......)
+000000c0: 01da 0561 646d 696e e902 0000 0029 01da  ...admin.....)..
+000000d0: 0842 6173 6550 6167 6529 01da 1654 6162  .BasePage)...Tab
+000000e0: 6265 6454 7261 6e73 6c61 7469 6f6e 4164  bedTranslationAd
+000000f0: 6d69 6e29 02da 1f50 6f6c 796d 6f72 7068  min)...Polymorph
+00000100: 6963 4d50 5454 5061 7265 6e74 4d6f 6465  icMPTTParentMode
+00000110: 6c41 646d 696e da1e 506f 6c79 6d6f 7270  lAdmin..Polymorp
+00000120: 6869 634d 5054 5443 6869 6c64 4d6f 6465  hicMPTTChildMode
+00000130: 6c41 646d 696e 2901 da16 6765 745f 6761  lAdmin)...get_ga
+00000140: 7270 6978 5f70 6167 655f 6d6f 6465 6c73  rpix_page_models
+00000150: 2901 da08 7365 7474 696e 6773 2901 da07  )...settings)...
+00000160: 6765 7474 6578 7463 0000 0000 0000 0000  gettextc........
+00000170: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000180: 7378 0000 0065 005a 0164 005a 0265 035a  sx...e.Z.d.Z.e.Z
+00000190: 0465 0565 0664 0183 0272 1c65 066a 076e  .e.e.d...r.e.j.n
+000001a0: 0264 025a 0864 035a 0964 045a 0a64 045a  .d.Z.d.Z.d.Z.d.Z
+000001b0: 0b64 055a 0c64 0664 0769 015a 0d64 075a  .d.Z.d.d.i.Z.d.Z
+000001c0: 0e64 085a 0f64 095a 1064 0a5a 1164 0b5a  .d.Z.d.Z.d.Z.d.Z
+000001d0: 1264 0c5a 1387 0066 0164 0d64 0e84 085a  .d.Z...f.d.d...Z
+000001e0: 1464 0f64 1084 005a 1587 0066 0164 1164  .d.d...Z...f.d.d
+000001f0: 1284 085a 1687 0004 005a 1753 0029 13da  ...Z.....Z.S.)..
+00000200: 0d42 6173 6550 6167 6541 646d 696e da1f  .BasePageAdmin..
+00000210: 4741 5250 4958 5f50 4147 455f 4144 4d49  GARPIX_PAGE_ADMI
+00000220: 4e5f 4c49 5354 5f50 4552 5f50 4147 45e9  N_LIST_PER_PAGE.
+00000230: 1900 0000 f50a 0000 002d 20d0 bdd0 b5d1  .........- .....
+00000240: 8220 2d54 da0a 6372 6561 7465 645f 6174  . -T..created_at
+00000250: da04 736c 7567 a901 da05 7469 746c 65a9  ..slug....title.
+00000260: 03da 0969 735f 6163 7469 7665 720f 0000  ...is_activer...
+00000270: 00da 0a75 7064 6174 6564 5f61 74a9 02da  ...updated_at...
+00000280: 0c63 6c6f 6e65 5f6f 626a 6563 74da 0772  .clone_object..r
+00000290: 6562 7569 6c64 2904 7212 0000 0072 0f00  ebuild).r....r..
+000002a0: 0000 7214 0000 00da 1067 6574 5f61 6273  ..r......get_abs
+000002b0: 6f6c 7574 655f 7572 6ca9 0172 1400 0000  olute_url..r....
+000002c0: a902 720f 0000 0072 1500 0000 6302 0000  ..r....r....c...
+000002d0: 0000 0000 0000 0000 0005 0000 0003 0000  ................
+000002e0: 000f 0000 0073 1800 0000 7400 8300 6a01  .....s....t...j.
+000002f0: 7c01 6601 7c02 9e02 7c03 8e01 7d04 7c04  |.f.|...|...}.|.
+00000300: 5300 a901 4e29 02da 0573 7570 6572 da08  S...N)...super..
+00000310: 6765 745f 666f 726d 2905 da04 7365 6c66  get_form)...self
+00000320: da07 7265 7175 6573 74da 0461 7267 73da  ..request..args.
+00000330: 066b 7761 7267 73da 0466 6f72 6da9 01da  .kwargs..form...
+00000340: 095f 5f63 6c61 7373 5f5f a900 fa49 2f55  .__class__...I/U
+00000350: 7365 7273 2f63 7275 7361 742f 7072 6f6a  sers/crusat/proj
+00000360: 6563 7473 2f67 6172 7069 785f 7061 6765  ects/garpix_page
+00000370: 2f62 6163 6b65 6e64 2f67 6172 7069 785f  /backend/garpix_
+00000380: 7061 6765 2f61 646d 696e 2f62 6173 655f  page/admin/base_
+00000390: 7061 6765 2e70 7972 1e00 0000 1f00 0000  page.pyr........
+000003a0: 7304 0000 0000 0114 027a 1642 6173 6550  s........z.BaseP
+000003b0: 6167 6541 646d 696e 2e67 6574 5f66 6f72  ageAdmin.get_for
+000003c0: 6d63 0300 0000 0000 0000 0000 0000 0300  mc..............
+000003d0: 0000 0500 0000 4300 0000 732a 0000 007c  ......C...s*...|
+000003e0: 006a 006a 016a 027c 026a 0364 0164 0264  .j.j.j.|.j.d.d.d
+000003f0: 038d 0264 048d 0101 007c 006a 006a 01a0  ...d.....|.j.j..
+00000400: 04a1 0001 0064 0053 0029 054e da02 6964  .....d.S.).N..id
+00000410: 5429 01da 0466 6c61 7429 01da 0669 645f  T)...flat)...id_
+00000420: 5f69 6e29 05da 056d 6f64 656c da07 6f62  _in)...model..ob
+00000430: 6a65 6374 73da 0664 656c 6574 65da 0b76  jects..delete..v
+00000440: 616c 7565 735f 6c69 7374 7218 0000 00a9  alues_listr.....
+00000450: 0372 1f00 0000 7220 0000 00da 0871 7565  .r....r .....que
+00000460: 7279 7365 7472 2600 0000 7226 0000 0072  rysetr&...r&...r
+00000470: 2700 0000 da0f 6465 6c65 7465 5f71 7565  '.....delete_que
+00000480: 7279 7365 7424 0000 0073 0400 0000 0001  ryset$...s......
+00000490: 1a01 7a1d 4261 7365 5061 6765 4164 6d69  ..z.BasePageAdmi
+000004a0: 6e2e 6465 6c65 7465 5f71 7565 7279 7365  n.delete_queryse
+000004b0: 7463 0200 0000 0000 0000 0000 0000 0300  tc..............
+000004c0: 0000 0400 0000 0300 0000 7334 0000 0074  ..........s4...t
+000004d0: 0083 00a0 017c 01a1 017d 027c 0264 006b  .....|...}.|.d.k
+000004e0: 0972 3064 017c 026b 0672 307c 006a 0264  .r0d.|.k.r0|.j.d
+000004f0: 0174 0364 0283 0166 037c 0264 013c 007c  .t.d...f.|.d.<.|
+00000500: 0253 0029 034e da0f 6465 6c65 7465 5f73  .S.).N..delete_s
+00000510: 656c 6563 7465 647a 2744 656c 6574 6520  electedz'Delete 
+00000520: 7365 6c65 6374 6564 2025 2876 6572 626f  selected %(verbo
+00000530: 7365 5f6e 616d 655f 706c 7572 616c 2973  se_name_plural)s
+00000540: 2904 721d 0000 00da 0b67 6574 5f61 6374  ).r......get_act
+00000550: 696f 6e73 7231 0000 00da 015f 2903 721f  ionsr1....._).r.
+00000560: 0000 0072 2000 0000 da07 6163 7469 6f6e  ...r .....action
+00000570: 7372 2400 0000 7226 0000 0072 2700 0000  sr$...r&...r'...
+00000580: 7233 0000 0028 0000 0073 0e00 0000 0001  r3...(...s......
+00000590: 0c01 1002 0401 0201 06fd 0805 7a19 4261  ............z.Ba
+000005a0: 7365 5061 6765 4164 6d69 6e2e 6765 745f  sePageAdmin.get_
+000005b0: 6163 7469 6f6e 7329 18da 085f 5f6e 616d  actions)...__nam
+000005c0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000005d0: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0400  .__qualname__r..
+000005e0: 0000 da0a 6261 7365 5f6d 6f64 656c da07  ....base_model..
+000005f0: 6861 7361 7474 7272 0900 0000 720c 0000  hasattrr....r...
+00000600: 00da 0d6c 6973 745f 7065 725f 7061 6765  ...list_per_page
+00000610: da13 656d 7074 795f 7661 6c75 655f 6469  ..empty_value_di
+00000620: 7370 6c61 79da 0b73 6176 655f 6f6e 5f74  splay..save_on_t
+00000630: 6f70 da0c 7669 6577 5f6f 6e5f 7369 7465  op..view_on_site
+00000640: da0e 6461 7465 5f68 6965 7261 7263 6879  ..date_hierarchy
+00000650: da13 7072 6570 6f70 756c 6174 6564 5f66  ..prepopulated_f
+00000660: 6965 6c64 73da 0d73 6561 7263 685f 6669  ields..search_fi
+00000670: 656c 6473 da0b 6c69 7374 5f66 696c 7465  elds..list_filte
+00000680: 7272 3500 0000 da0c 6c69 7374 5f64 6973  rr5.....list_dis
+00000690: 706c 6179 da0d 6c69 7374 5f65 6469 7461  play..list_edita
+000006a0: 626c 65da 0f72 6561 646f 6e6c 795f 6669  ble..readonly_fi
+000006b0: 656c 6473 721e 0000 0072 3100 0000 7233  eldsr....r1...r3
+000006c0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+000006d0: 5f5f 7226 0000 0072 2600 0000 7224 0000  __r&...r&...r$..
+000006e0: 0072 2700 0000 720b 0000 000a 0000 0073  .r'...r........s
+000006f0: 2000 0000 0801 0402 1402 0401 0401 0402   ...............
+00000700: 0401 0802 0401 0401 0402 0401 0402 0402  ................
+00000710: 0c05 0804 720b 0000 0063 0000 0000 0000  ....r....c......
+00000720: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+00000730: 0000 739e 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000740: 015a 0365 045a 0565 0683 005a 0765 0865  .Z.e.Z.e...Z.e.e
+00000750: 0964 0283 0272 2665 096a 0a6e 0264 035a  .d...r&e.j.n.d.Z
+00000760: 0b64 045a 0c64 055a 0d64 055a 0e64 065a  .d.Z.d.Z.d.Z.d.Z
+00000770: 0f64 0764 0869 015a 1064 085a 1164 095a  .d.d.i.Z.d.Z.d.Z
+00000780: 1264 0a5a 1364 0b5a 1464 0c5a 1564 0d5a  .d.Z.d.Z.d.Z.d.Z
+00000790: 1687 0066 0164 0e64 0f84 085a 1764 1064  ...f.d.d...Z.d.d
+000007a0: 1184 005a 1864 1265 185f 1964 1364 1484  ...Z.d.e._.d.d..
+000007b0: 005a 1a64 1564 1684 005a 1b64 1765 1b5f  .Z.d.d...Z.d.e._
+000007c0: 1987 0066 0164 1864 1984 085a 1c87 0004  ...f.d.d...Z....
+000007d0: 005a 1d53 0029 1ada 1152 6561 6c42 6173  .Z.S.)...RealBas
+000007e0: 6550 6167 6541 646d 696e 7559 0000 000a  ePageAdminuY....
+000007f0: 2020 2020 d0a1 d182 d0b0 d0bd d0b4 d0b0      ............
+00000800: d180 d182 d0bd d18b d0b5 20d0 bdd0 b0d1  .......... .....
+00000810: 81d1 82d1 80d0 bed0 b9d0 bad0 b820 d0b4  ............. ..
+00000820: d0bb d18f 20d0 b1d0 b0d0 b7d0 bed0 b2d1  .... ...........
+00000830: 8bd1 8520 d181 d182 d180 d0b0 d0bd d0b8  ... ............
+00000840: d186 2e0a 2020 2020 720c 0000 0072 0d00  ....    r....r..
+00000850: 0000 720e 0000 0054 720f 0000 0072 1000  ..r....Tr....r..
+00000860: 0000 7211 0000 0072 1300 0000 7216 0000  ..r....r....r...
+00000870: 0029 0472 1200 0000 720f 0000 0072 1400  .).r....r....r..
+00000880: 0000 da15 6765 745f 6162 736f 6c75 7465  ....get_absolute
+00000890: 5f75 726c 5f68 746d 6c72 1a00 0000 721b  _url_htmlr....r.
+000008a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000008b0: 0300 0000 0300 0000 0f00 0000 733e 0000  ............s>..
+000008c0: 0074 0083 006a 017c 017c 028e 0101 0064  .t...j.|.|.....d
+000008d0: 017c 026b 0672 3a7c 006a 02a0 03a1 007c  .|.k.r:|.j.....|
+000008e0: 006a 0464 0219 005f 057c 006a 02a0 06a1  .j.d..._.|.j....
+000008f0: 007c 006a 0464 0219 005f 0764 0053 0029  .|.j.d..._.d.S.)
+00000900: 034e da07 696e 6974 6961 6cda 0670 6172  .N..initial..par
+00000910: 656e 7429 0872 1d00 0000 da08 5f5f 696e  ent).r......__in
+00000920: 6974 5f5f 722b 0000 005a 1a67 6574 5f61  it__r+...Z.get_a
+00000930: 7661 696c 6162 6c65 5f70 6167 655f 7061  vailable_page_pa
+00000940: 7265 6e74 73da 0666 6965 6c64 7372 3000  rents..fieldsr0.
+00000950: 0000 5a12 6765 745f 6465 6661 756c 745f  ..Z.get_default_
+00000960: 7061 7265 6e74 da07 6465 6661 756c 7429  parent..default)
+00000970: 0372 1f00 0000 7221 0000 0072 2200 0000  .r....r!...r"...
+00000980: 7224 0000 0072 2600 0000 7227 0000 0072  r$...r&...r'...r
+00000990: 4b00 0000 4d00 0000 7308 0000 0000 010e  K...M...s.......
+000009a0: 0108 0112 017a 1a52 6561 6c42 6173 6550  .....z.RealBaseP
+000009b0: 6167 6541 646d 696e 2e5f 5f69 6e69 745f  ageAdmin.__init_
+000009c0: 5f63 0300 0000 0000 0000 0000 0000 0600  _c..............
+000009d0: 0000 0400 0000 4300 0000 7346 0000 007c  ......C...sF...|
+000009e0: 0244 005d 3c7d 0364 017d 047c 037d 057c  .D.]<}.d.}.|.}.|
+000009f0: 0504 006a 007c 0437 0002 005f 007c 0504  ...j.|.7..._.|..
+00000a00: 006a 017c 0437 0002 005f 0164 027c 055f  .j.|.7..._.d.|._
+00000a10: 0264 037c 055f 037c 05a0 04a1 0001 0071  .d.|._.|.......q
+00000a20: 0464 0253 0029 0475 5d00 0000 d09a d0be  .d.S.).u].......
+00000a30: d0bf d0b8 d180 d0be d0b2 d0b0 d0bd d0b8  ................
+00000a40: d0b5 28d0 bad0 bbd0 bed0 bdd0 b8d1 80d0  ..(.............
+00000a50: bed0 b2d0 b0d0 bdd0 b8d0 b529 20d0 b2d1  ...........) ...
+00000a60: 8bd0 b1d1 80d0 b0d0 bdd0 bdd1 8bd1 8520  ............... 
+00000a70: d0be d0b1 d18a d0b5 d0ba d182 d0be d0b2  ................
+00000a80: 202d 2061 6374 696f 6e7a 062d 434c 4f4e   - actionz.-CLON
+00000a90: 454e 4629 0572 1200 0000 7210 0000 0072  ENF).r....r....r
+00000aa0: 2800 0000 7214 0000 00da 0473 6176 6529  (...r......save)
+00000ab0: 0672 1f00 0000 7220 0000 0072 3000 0000  .r....r ...r0...
+00000ac0: da03 6f62 6ada 0670 7265 6669 78da 0563  ..obj..prefix..c
+00000ad0: 6c6f 6e65 7226 0000 0072 2600 0000 7227  loner&...r&...r'
+00000ae0: 0000 0072 1700 0000 5300 0000 7310 0000  ...r....S...s...
+00000af0: 0000 0208 0104 0104 010e 010e 0106 0106  ................
+00000b00: 017a 1e52 6561 6c42 6173 6550 6167 6541  .z.RealBasePageA
+00000b10: 646d 696e 2e63 6c6f 6e65 5f6f 626a 6563  dmin.clone_objec
+00000b20: 7475 2300 0000 d09a d0bb d0be d0bd d0b8  tu#.............
+00000b30: d180 d0be d0b2 d0b0 d182 d18c 20d0 bed0  ............ ...
+00000b40: b1d1 8ad0 b5d0 bad1 8263 0100 0000 0000  .........c......
+00000b50: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
+00000b60: 0000 732a 0000 007a 107c 006a 006a 01a0  ..s*...z.|.j.j..
+00000b70: 02a1 0001 0057 006e 1401 0001 0001 0074  .....W.n.......t
+00000b80: 0364 0183 0101 0059 006e 0258 0064 0053  .d.....Y.n.X.d.S
+00000b90: 0029 024e 755f 0000 005b 4552 524f 525d  .).Nu_...[ERROR]
+00000ba0: 3a20 d09e d188 d0b8 d0b1 d0ba d0b0 20d0  : ............ .
+00000bb0: bfd1 80d0 b820 d0bf d0b5 d180 d0b5 d0b7  ..... ..........
+00000bc0: d0b0 d0b3 d180 d183 d0b7 d0ba d0b8 20d0  .............. .
+00000bd0: b4d1 80d0 b5d0 b2d0 bed0 b2d0 b8d0 b4d0  ................
+00000be0: bdd0 bed0 b920 d181 d182 d180 d183 d0ba  ..... ..........
+00000bf0: d182 d183 d180 d18b 2904 722b 0000 0072  ........).r+...r
+00000c00: 2c00 0000 7218 0000 00da 0570 7269 6e74  ,...r......print
+00000c10: 2901 721f 0000 0072 2600 0000 7226 0000  ).r....r&...r&..
+00000c20: 0072 2700 0000 da08 5f72 6562 7569 6c64  .r'....._rebuild
+00000c30: 6000 0000 7308 0000 0000 0102 0110 0106  `...s...........
+00000c40: 017a 1a52 6561 6c42 6173 6550 6167 6541  .z.RealBasePageA
+00000c50: 646d 696e 2e5f 7265 6275 696c 6463 0300  dmin._rebuildc..
+00000c60: 0000 0000 0000 0000 0000 0300 0000 0200  ................
+00000c70: 0000 4300 0000 730c 0000 007c 00a0 00a1  ..C...s....|....
+00000c80: 0001 0064 0153 0029 0275 7b00 0000 d09f  ...d.S.).u{.....
+00000c90: d0b5 d180 d0b5 d181 d0be d180 d0b1 d0b0  ................
+00000ca0: d182 d18c 20d0 9cd0 9fd0 a2d0 a220 d0bc  .... ........ ..
+00000cb0: d0be d0b4 d0b5 d0bb d18c 2e20 d098 d0bd  ........... ....
+00000cc0: d0be d0b3 d0b4 d0b0 20d1 82d1 80d0 b5d0  ........ .......
+00000cd0: b1d1 83d0 b5d1 82d1 81d1 8f20 d0b4 d0bb  ........... ....
+00000ce0: d18f 20d0 bfd0 b5d1 80d0 b5d0 b7d0 b0d0  .. .............
+00000cf0: b3d1 80d1 83d0 b7d0 bad0 b820 d0b4 d0b5  ........... ....
+00000d00: d180 d0b5 d0b2 d0b0 2e4e 2901 7253 0000  .........N).rS..
+00000d10: 0072 2f00 0000 7226 0000 0072 2600 0000  .r/...r&...r&...
+00000d20: 7227 0000 0072 1800 0000 6600 0000 7302  r'...r....f...s.
+00000d30: 0000 0000 027a 1952 6561 6c42 6173 6550  .....z.RealBaseP
+00000d40: 6167 6541 646d 696e 2e72 6562 7569 6c64  ageAdmin.rebuild
+00000d50: 7532 0000 00d0 9fd0 b5d1 80d0 b5d1 81d0  u2..............
+00000d60: bed0 b1d1 80d0 b0d1 82d1 8c20 d0bf d183  ........... ....
+00000d70: d0bd d0ba d182 d18b 20d1 80d0 b0d0 b7d0  ........ .......
+00000d80: b4d0 b5d0 bbd0 b063 0500 0000 0000 0000  .......c........
+00000d90: 0000 0000 0500 0000 0600 0000 0300 0000  ................
+00000da0: 731e 0000 007c 00a0 00a1 0001 0074 0183  s....|.......t..
+00000db0: 00a0 027c 017c 027c 037c 04a1 0401 0064  ...|.|.|.|.....d
+00000dc0: 0053 0072 1c00 0000 2903 7253 0000 0072  .S.r....).rS...r
+00000dd0: 1d00 0000 da0a 7361 7665 5f6d 6f64 656c  ......save_model
+00000de0: 2905 721f 0000 0072 2000 0000 724f 0000  ).r....r ...rO..
+00000df0: 0072 2300 0000 da06 6368 616e 6765 7224  .r#.....changer$
+00000e00: 0000 0072 2600 0000 7227 0000 0072 5400  ...r&...r'...rT.
+00000e10: 0000 6c00 0000 7304 0000 0000 0108 017a  ..l...s........z
+00000e20: 1c52 6561 6c42 6173 6550 6167 6541 646d  .RealBasePageAdm
+00000e30: 696e 2e73 6176 655f 6d6f 6465 6c29 1e72  in.save_model).r
+00000e40: 3600 0000 7237 0000 0072 3800 0000 da07  6...r7...r8.....
+00000e50: 5f5f 646f 635f 5f72 0400 0000 7239 0000  __doc__r....r9..
+00000e60: 0072 0800 0000 da0c 6368 696c 645f 6d6f  .r......child_mo
+00000e70: 6465 6c73 723a 0000 0072 0900 0000 720c  delsr:...r....r.
+00000e80: 0000 0072 3b00 0000 723c 0000 0072 3d00  ...r;...r<...r=.
+00000e90: 0000 723e 0000 0072 3f00 0000 7240 0000  ..r>...r?...r@..
+00000ea0: 0072 4100 0000 7242 0000 0072 3500 0000  .rA...rB...r5...
+00000eb0: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
+00000ec0: 4b00 0000 7217 0000 00da 1173 686f 7274  K...r......short
+00000ed0: 5f64 6573 6372 6970 7469 6f6e 7253 0000  _descriptionrS..
+00000ee0: 0072 1800 0000 7254 0000 0072 4600 0000  .r....rT...rF...
+00000ef0: 7226 0000 0072 2600 0000 7224 0000 0072  r&...r&...r$...r
+00000f00: 2700 0000 7247 0000 0033 0000 0073 2c00  '...rG...3...s,.
+00000f10: 0000 0802 0403 0401 0602 1402 0401 0401  ................
+00000f20: 0402 0401 0802 0401 0401 0402 0401 0402  ................
+00000f30: 0402 0c06 080b 0602 0806 0804 0602 7247  ..............rG
+00000f40: 0000 004e 2913 5a0e 646a 616e 676f 2e63  ...N).Z.django.c
+00000f50: 6f6e 7472 6962 7202 0000 005a 106d 6f64  ontribr....Z.mod
+00000f60: 656c 732e 6261 7365 5f70 6167 6572 0400  els.base_pager..
+00000f70: 0000 5a16 6d6f 6465 6c74 7261 6e73 6c61  ..Z.modeltransla
+00000f80: 7469 6f6e 2e61 646d 696e 7205 0000 005a  tion.adminr....Z
+00000f90: 1670 6f6c 796d 6f72 7068 6963 5f74 7265  .polymorphic_tre
+00000fa0: 652e 6164 6d69 6e72 0600 0000 7207 0000  e.adminr....r...
+00000fb0: 00da 1c75 7469 6c73 2e67 6574 5f67 6172  ...utils.get_gar
+00000fc0: 7069 785f 7061 6765 5f6d 6f64 656c 7372  pix_page_modelsr
+00000fd0: 0800 0000 da0b 646a 616e 676f 2e63 6f6e  ......django.con
+00000fe0: 6672 0900 0000 da18 646a 616e 676f 2e75  fr......django.u
+00000ff0: 7469 6c73 2e74 7261 6e73 6c61 7469 6f6e  tils.translation
+00001000: 720a 0000 0072 3400 0000 720b 0000 00da  r....r4...r.....
+00001010: 0872 6567 6973 7465 7272 4700 0000 7226  .registerrG...r&
+00001020: 0000 0072 2600 0000 7226 0000 0072 2700  ...r&...r&...r'.
+00001030: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001040: 7312 0000 000c 010c 010c 0110 010c 010c  s...............
+00001050: 010c 0312 2908 01                        ....)..
```

### Comparing `garpix_page-2.8.0/garpix_page/admin/base_page.py` & `garpix_page-2.9.0/garpix_page/admin/base_page.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib import admin
 from ..models.base_page import BasePage
 from modeltranslation.admin import TabbedTranslationAdmin
 from polymorphic_tree.admin import PolymorphicMPTTParentModelAdmin, PolymorphicMPTTChildModelAdmin
 from ..utils.get_garpix_page_models import get_garpix_page_models
 from django.conf import settings
+from django.utils.translation import gettext as _
 
 
 class BasePageAdmin(TabbedTranslationAdmin, PolymorphicMPTTChildModelAdmin):
     base_model = BasePage
 
     list_per_page = settings.GARPIX_PAGE_ADMIN_LIST_PER_PAGE if hasattr(settings, 'GARPIX_PAGE_ADMIN_LIST_PER_PAGE') else 25
 
@@ -28,14 +29,28 @@
     readonly_fields = ('created_at', 'updated_at')
 
     def get_form(self, request, *args, **kwargs):
         form = super().get_form(request, *args, **kwargs)
         # form.current_user = request.user
         return form
 
+    def delete_queryset(self, request, queryset):
+        self.model.objects.delete(id__in=queryset.values_list('id', flat=True))
+        self.model.objects.rebuild()
+
+    def get_actions(self, request):
+        actions = super().get_actions(request)
+        if actions is not None and "delete_selected" in actions:
+            actions["delete_selected"] = (
+                self.delete_queryset,
+                "delete_selected",
+                _("Delete selected %(verbose_name_plural)s"),
+            )
+        return actions
+
 
 @admin.register(BasePage)
 class RealBasePageAdmin(TabbedTranslationAdmin, PolymorphicMPTTParentModelAdmin):
     """
     Стандартные настройки для базовых страниц.
     """
     base_model = BasePage
```

### Comparing `garpix_page-2.8.0/garpix_page/codegenerator.py` & `garpix_page-2.9.0/garpix_page/codegenerator.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/constants.py` & `garpix_page-2.9.0/garpix_page/constants.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/locale/en/LC_MESSAGES/django.po` & `garpix_page-2.9.0/garpix_page/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/locale/ru_RU/LC_MESSAGES/django.po` & `garpix_page-2.9.0/garpix_page/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/management/commands/__pycache__/startpage.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/management/commands/__pycache__/startpage.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/management/commands/startpage.py` & `garpix_page-2.9.0/garpix_page/management/commands/startpage.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/models/__pycache__/base_list_page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/models/__pycache__/base_list_page.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Sep  8 10:22:48 2021 UTC, .py size: 814 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-00000000: 550d 0d0a 0000 0000 f88e 3861 2e03 0000  U.........8a....
+00000000: 550d 0d0a 0000 0000 a204 4161 3b03 0000  U.........Aa;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000050: 6501 8303 5a04 6406 5300 2907 e901 0000  e...Z.d.S.).....
 00000060: 0029 01da 0842 6173 6550 6167 65e9 0000  .)...BasePage...
-00000070: 0000 2901 da09 5061 6769 6e61 746f 7263  ..)...Paginatorc
-00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0400 0000 0000 0000 7334 0000 0065 005a  ........s4...e.Z
-000000a0: 0164 005a 0264 015a 0364 025a 0464 0887  .d.Z.d.Z.d.Z.d..
-000000b0: 0066 0164 0464 0584 095a 0547 0064 0664  .f.d.d...Z.G.d.d
-000000c0: 0784 0064 0783 025a 0687 0004 005a 0753  ...d...Z.....Z.S
-000000d0: 0029 09da 0c42 6173 654c 6973 7450 6167  .)...BaseListPag
-000000e0: 65e9 1900 0000 7a1d 6761 7270 6978 5f70  e.....z.garpix_p
-000000f0: 6167 652f 6465 6661 756c 745f 6c69 7374  age/default_list
-00000100: 2e68 746d 6c4e 6302 0000 0000 0000 0000  .htmlNc.........
-00000110: 0000 0009 0000 0008 0000 000f 0000 0073  ...............s
-00000120: 7e00 0000 7400 8300 6a01 7c01 6601 7c02  ~...t...j.|.f.|.
-00000130: 9e02 7c03 8e01 7d04 7c00 6a02 6a03 6401  ..|...}.|.j.j.d.
-00000140: 6402 8d01 7d05 7404 7c05 7c00 6a05 8302  d...}.t.|.|.j...
-00000150: 7d06 7a16 7406 7c01 6a07 a008 6403 6404  }.z.t.|.j...d.d.
-00000160: a102 8301 7d07 5700 6e18 0400 7409 6b0a  ....}.W.n...t.k.
-00000170: 725c 0100 0100 0100 6404 7d07 5900 6e02  r\......d.}.Y.n.
-00000180: 5800 7c06 a00a 7c07 a101 7d08 7c04 a00b  X.|...|...}.|...
-00000190: 7c06 7c08 7c07 6405 9c03 a101 0100 7c04  |.|.|.d.......|.
-000001a0: 5300 2906 4e54 2901 da09 6973 5f61 6374  S.).NT)...is_act
-000001b0: 6976 65da 0470 6167 6572 0100 0000 2903  ive..pager....).
-000001c0: da09 7061 6769 6e61 746f 72da 1570 6167  ..paginator..pag
-000001d0: 696e 6174 6564 5f6f 626a 6563 745f 6c69  inated_object_li
-000001e0: 7374 7208 0000 0029 0cda 0573 7570 6572  str....)...super
-000001f0: da0b 6765 745f 636f 6e74 6578 74da 0863  ..get_context..c
-00000200: 6869 6c64 7265 6eda 0666 696c 7465 7272  hildren..filterr
-00000210: 0400 0000 da0b 7061 6769 6e61 7465 5f62  ......paginate_b
-00000220: 79da 0369 6e74 da03 4745 54da 0367 6574  y..int..GET..get
-00000230: da0a 5661 6c75 6545 7272 6f72 da08 6765  ..ValueError..ge
-00000240: 745f 7061 6765 da06 7570 6461 7465 2909  t_page..update).
-00000250: da04 7365 6c66 da07 7265 7175 6573 74da  ..self..request.
-00000260: 0461 7267 73da 066b 7761 7267 73da 0763  .args..kwargs..c
-00000270: 6f6e 7465 7874 da0b 6f62 6a65 6374 5f6c  ontext..object_l
-00000280: 6973 7472 0900 0000 7208 0000 0072 0a00  istr....r....r..
-00000290: 0000 a901 da09 5f5f 636c 6173 735f 5fa9  ......__class__.
-000002a0: 00fa 4f2f 5573 6572 732f 6372 7573 6174  ..O/Users/crusat
-000002b0: 2f70 726f 6a65 6374 732f 6761 7270 6978  /projects/garpix
-000002c0: 5f70 6167 652f 6261 636b 656e 642f 6761  _page/backend/ga
-000002d0: 7270 6978 5f70 6167 652f 6d6f 6465 6c73  rpix_page/models
-000002e0: 2f62 6173 655f 6c69 7374 5f70 6167 652e  /base_list_page.
-000002f0: 7079 720c 0000 0009 0000 0073 1c00 0000  pyr........s....
-00000300: 0001 1402 0e01 0c02 0201 1601 0e01 0a02  ................
-00000310: 0a02 0401 0201 0201 02fd 0805 7a18 4261  ............z.Ba
-00000320: 7365 4c69 7374 5061 6765 2e67 6574 5f63  seListPage.get_c
-00000330: 6f6e 7465 7874 6300 0000 0000 0000 0000  ontextc.........
-00000340: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00000350: 1000 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000360: 6402 5300 2903 7a11 4261 7365 4c69 7374  d.S.).z.BaseList
-00000370: 5061 6765 2e4d 6574 6154 4e29 04da 085f  Page.MetaTN)..._
-00000380: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00000390: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-000003a0: 5fda 0861 6273 7472 6163 7472 1e00 0000  _..abstractr....
-000003b0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-000003c0: 044d 6574 611d 0000 0073 0200 0000 0801  .Meta....s......
-000003d0: 7224 0000 0029 014e 2908 7220 0000 0072  r$...).N).r ...r
-000003e0: 2100 0000 7222 0000 0072 0f00 0000 da08  !...r"...r......
-000003f0: 7465 6d70 6c61 7465 720c 0000 0072 2400  templater....r$.
-00000400: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00000410: 5f72 1e00 0000 721e 0000 0072 1c00 0000  _r....r....r....
-00000420: 721f 0000 0072 0500 0000 0500 0000 7308  r....r........s.
-00000430: 0000 0008 0104 0104 020e 1472 0500 0000  ...........r....
-00000440: 4e29 05da 0962 6173 655f 7061 6765 7202  N)...base_pager.
-00000450: 0000 00da 1564 6a61 6e67 6f2e 636f 7265  .....django.core
-00000460: 2e70 6167 696e 6174 6f72 7204 0000 0072  .paginatorr....r
-00000470: 0500 0000 721e 0000 0072 1e00 0000 721e  ....r....r....r.
-00000480: 0000 0072 1f00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000490: 653e 0100 0000 7304 0000 000c 010c 03    e>....s........
+00000070: 0000 2901 da0f 4761 7270 6978 5061 6769  ..)...GarpixPagi
+00000080: 6e61 746f 7263 0000 0000 0000 0000 0000  natorc..........
+00000090: 0000 0000 0000 0400 0000 0000 0000 7334  ..............s4
+000000a0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000000b0: 025a 0464 0887 0066 0164 0464 0584 095a  .Z.d...f.d.d...Z
+000000c0: 0547 0064 0664 0784 0064 0783 025a 0687  .G.d.d...d...Z..
+000000d0: 0004 005a 0753 0029 09da 0c42 6173 654c  ...Z.S.)...BaseL
+000000e0: 6973 7450 6167 65e9 1900 0000 7a1d 6761  istPage.....z.ga
+000000f0: 7270 6978 5f70 6167 652f 6465 6661 756c  rpix_page/defaul
+00000100: 745f 6c69 7374 2e68 746d 6c4e 6302 0000  t_list.htmlNc...
+00000110: 0000 0000 0000 0000 0009 0000 0008 0000  ................
+00000120: 000f 0000 0073 7e00 0000 7400 8300 6a01  .....s~...t...j.
+00000130: 7c01 6601 7c02 9e02 7c03 8e01 7d04 7c00  |.f.|...|...}.|.
+00000140: 6a02 6a03 6401 6402 8d01 7d05 7404 7c05  j.j.d.d...}.t.|.
+00000150: 7c00 6a05 8302 7d06 7a16 7406 7c01 6a07  |.j...}.z.t.|.j.
+00000160: a008 6403 6404 a102 8301 7d07 5700 6e18  ..d.d.....}.W.n.
+00000170: 0400 7409 6b0a 725c 0100 0100 0100 6404  ..t.k.r\......d.
+00000180: 7d07 5900 6e02 5800 7c06 a00a 7c07 a101  }.Y.n.X.|...|...
+00000190: 7d08 7c04 a00b 7c06 7c08 7c07 6405 9c03  }.|...|.|.|.d...
+000001a0: a101 0100 7c04 5300 2906 4e54 2901 da09  ....|.S.).NT)...
+000001b0: 6973 5f61 6374 6976 65da 0470 6167 6572  is_active..pager
+000001c0: 0100 0000 2903 da09 7061 6769 6e61 746f  ....)...paginato
+000001d0: 72da 1570 6167 696e 6174 6564 5f6f 626a  r..paginated_obj
+000001e0: 6563 745f 6c69 7374 7208 0000 0029 0cda  ect_listr....)..
+000001f0: 0573 7570 6572 da0b 6765 745f 636f 6e74  .super..get_cont
+00000200: 6578 74da 0863 6869 6c64 7265 6eda 0666  ext..children..f
+00000210: 696c 7465 7272 0400 0000 da0b 7061 6769  ilterr......pagi
+00000220: 6e61 7465 5f62 79da 0369 6e74 da03 4745  nate_by..int..GE
+00000230: 54da 0367 6574 da0a 5661 6c75 6545 7272  T..get..ValueErr
+00000240: 6f72 da08 6765 745f 7061 6765 da06 7570  or..get_page..up
+00000250: 6461 7465 2909 da04 7365 6c66 da07 7265  date)...self..re
+00000260: 7175 6573 74da 0461 7267 73da 066b 7761  quest..args..kwa
+00000270: 7267 73da 0763 6f6e 7465 7874 da0b 6f62  rgs..context..ob
+00000280: 6a65 6374 5f6c 6973 7472 0900 0000 7208  ject_listr....r.
+00000290: 0000 0072 0a00 0000 a901 da09 5f5f 636c  ...r........__cl
+000002a0: 6173 735f 5fa9 00fa 4f2f 5573 6572 732f  ass__...O/Users/
+000002b0: 6372 7573 6174 2f70 726f 6a65 6374 732f  crusat/projects/
+000002c0: 6761 7270 6978 5f70 6167 652f 6261 636b  garpix_page/back
+000002d0: 656e 642f 6761 7270 6978 5f70 6167 652f  end/garpix_page/
+000002e0: 6d6f 6465 6c73 2f62 6173 655f 6c69 7374  models/base_list
+000002f0: 5f70 6167 652e 7079 720c 0000 0009 0000  _page.pyr.......
+00000300: 0073 1c00 0000 0001 1402 0e01 0c02 0201  .s..............
+00000310: 1601 0e01 0a02 0a02 0401 0201 0201 02fd  ................
+00000320: 0805 7a18 4261 7365 4c69 7374 5061 6765  ..z.BaseListPage
+00000330: 2e67 6574 5f63 6f6e 7465 7874 6300 0000  .get_contextc...
+00000340: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000350: 0040 0000 0073 1000 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000360: 5a02 6401 5a03 6402 5300 2903 7a11 4261  Z.d.Z.d.S.).z.Ba
+00000370: 7365 4c69 7374 5061 6765 2e4d 6574 6154  seListPage.MetaT
+00000380: 4e29 04da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000003a0: 6c6e 616d 655f 5fda 0861 6273 7472 6163  lname__..abstrac
+000003b0: 7472 1e00 0000 721e 0000 0072 1e00 0000  tr....r....r....
+000003c0: 721f 0000 00da 044d 6574 611d 0000 0073  r......Meta....s
+000003d0: 0200 0000 0801 7224 0000 0029 014e 2908  ......r$...).N).
+000003e0: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
+000003f0: 0f00 0000 da08 7465 6d70 6c61 7465 720c  ......templater.
+00000400: 0000 0072 2400 0000 da0d 5f5f 636c 6173  ...r$.....__clas
+00000410: 7363 656c 6c5f 5f72 1e00 0000 721e 0000  scell__r....r...
+00000420: 0072 1c00 0000 721f 0000 0072 0500 0000  .r....r....r....
+00000430: 0500 0000 7308 0000 0008 0104 0104 020e  ....s...........
+00000440: 1472 0500 0000 4e29 05da 0962 6173 655f  .r....N)...base_
+00000450: 7061 6765 7202 0000 005a 1667 6172 7069  pager....Z.garpi
+00000460: 785f 7574 696c 732e 7061 6769 6e61 746f  x_utils.paginato
+00000470: 7272 0400 0000 7205 0000 0072 1e00 0000  rr....r....r....
+00000480: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000490: 083c 6d6f 6475 6c65 3e01 0000 0073 0400  .<module>....s..
+000004a0: 0000 0c01 0c03                           ......
```

### Comparing `garpix_page-2.8.0/garpix_page/models/__pycache__/base_page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/models/__pycache__/base_page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/models/__pycache__/base_search_page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/models/__pycache__/base_search_page.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Sep  8 11:04:48 2021 UTC, .py size: 1541 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,105 @@
-00000000: 550d 0d0a 0000 0000 d098 3861 0506 0000  U.........8a....
+00000000: 550d 0d0a 0000 0000 c604 4161 1206 0000  U.........Aa....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6405 6406 8400 6406 6501 8303  ..G.d.d...d.e...
 00000060: 5a06 6407 5300 2908 e901 0000 0029 01da  Z.d.S.)......)..
 00000070: 0842 6173 6550 6167 65e9 0000 0000 2901  .BasePage.....).
-00000080: da01 5129 01da 0950 6167 696e 6174 6f72  ..Q)...Paginator
-00000090: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000a0: 0004 0000 0000 0000 0073 3400 0000 6500  .........s4...e.
-000000b0: 5a01 6400 5a02 6401 5a03 6402 5a04 6408  Z.d.Z.d.Z.d.Z.d.
-000000c0: 8700 6601 6404 6405 8409 5a05 4700 6406  ..f.d.d...Z.G.d.
-000000d0: 6407 8400 6407 8302 5a06 8700 0400 5a07  d...d...Z.....Z.
-000000e0: 5300 2909 da0e 4261 7365 5365 6172 6368  S.)...BaseSearch
-000000f0: 5061 6765 e919 0000 007a 1f67 6172 7069  Page.....z.garpi
-00000100: 785f 7061 6765 2f64 6566 6175 6c74 5f73  x_page/default_s
-00000110: 6561 7263 682e 6874 6d6c 4e63 0200 0000  earch.htmlNc....
-00000120: 0000 0000 0000 0000 1000 0000 0800 0000  ................
-00000130: 0f00 0000 7316 0100 0064 0164 026c 006d  ....s....d.d.l.m
-00000140: 017d 0401 0074 0283 006a 037c 0166 017c  .}...t...j.|.f.|
-00000150: 029e 027c 038e 017d 057c 016a 04a0 0564  ...|...}.|.j...d
-00000160: 0364 00a1 027d 0674 066a 07a0 08a1 007d  .d...}.t.j.....}
-00000170: 077a 1674 097c 016a 04a0 0564 0464 05a1  .z.t.|.j...d.d..
-00000180: 0283 017d 0857 006e 1804 0074 0a6b 0a72  ...}.W.n...t.k.r
-00000190: 6601 0001 0001 0064 057d 0859 006e 0258  f......d.}.Y.n.X
-000001a0: 007c 0664 006b 0972 e267 007d 097c 0483  .|.d.k.r.g.}.|..
-000001b0: 0044 005d 587d 0a74 0b83 007d 0b7c 0a6a  .D.]X}.t...}.|.j
-000001c0: 0c44 005d 207d 0c7c 0c9b 0064 069d 027c  .D.] }.|...d...|
-000001d0: 0669 017d 0d7c 0b74 0b66 007c 0d8e 014f  .i.}.|.t.f.|...O
-000001e0: 007d 0b71 8a7c 0974 0d7c 0a6a 0e6a 0f64  .}.q.|.t.|.j.j.d
-000001f0: 0764 088d 01a0 0f7c 0ba1 016a 1064 0964  .d.....|...j.d.d
-00000200: 0764 0a8d 0283 0137 007d 0971 7a74 066a  .d.....7.}.qzt.j
-00000210: 076a 0f7c 0964 0b8d 017d 0774 117c 077c  .j.|.d...}.t.|.|
-00000220: 006a 1283 027d 0e7c 0ea0 137c 08a1 017d  .j...}.|...|...}
-00000230: 0f7c 05a0 147c 0e7c 0f7c 087c 0690 0170  .|...|.|.|.|...p
-00000240: 0a64 0c64 0d9c 04a1 0101 007c 0553 0029  .d.d.......|.S.)
-00000250: 0e4e e902 0000 0029 01da 1667 6574 5f67  .N.....)...get_g
-00000260: 6172 7069 785f 7061 6765 5f6d 6f64 656c  arpix_page_model
-00000270: 73da 0171 da04 7061 6765 7201 0000 005a  s..q..pager....Z
-00000280: 0b5f 5f69 636f 6e74 6169 6e73 5429 01da  .__icontainsT)..
-00000290: 0969 735f 6163 7469 7665 da02 6964 2901  .is_active..id).
-000002a0: da04 666c 6174 2901 5a06 6964 5f5f 696e  ..flat).Z.id__in
-000002b0: da00 2904 da09 7061 6769 6e61 746f 72da  ..)...paginator.
-000002c0: 1570 6167 696e 6174 6564 5f6f 626a 6563  .paginated_objec
-000002d0: 745f 6c69 7374 720b 0000 0072 0a00 0000  t_listr....r....
-000002e0: 2915 5a1c 7574 696c 732e 6765 745f 6761  ).Z.utils.get_ga
-000002f0: 7270 6978 5f70 6167 655f 6d6f 6465 6c73  rpix_page_models
-00000300: 7209 0000 00da 0573 7570 6572 da0b 6765  r......super..ge
-00000310: 745f 636f 6e74 6578 74da 0347 4554 da03  t_context..GET..
-00000320: 6765 7472 0200 0000 da07 6f62 6a65 6374  getr......object
-00000330: 73da 046e 6f6e 65da 0369 6e74 da0a 5661  s..none..int..Va
-00000340: 6c75 6545 7272 6f72 7204 0000 00da 1173  lueErrorr......s
-00000350: 6561 7263 6861 626c 655f 6669 656c 6473  earchable_fields
-00000360: da04 6c69 7374 da07 6f6e 5f73 6974 65da  ..list..on_site.
-00000370: 0666 696c 7465 72da 0b76 616c 7565 735f  .filter..values_
-00000380: 6c69 7374 7205 0000 00da 0b70 6167 696e  listr......pagin
-00000390: 6174 655f 6279 da08 6765 745f 7061 6765  ate_by..get_page
-000003a0: da06 7570 6461 7465 2910 da04 7365 6c66  ..update)...self
-000003b0: da07 7265 7175 6573 74da 0461 7267 73da  ..request..args.
-000003c0: 066b 7761 7267 7372 0900 0000 da07 636f  .kwargsr......co
-000003d0: 6e74 6578 745a 0c73 6561 7263 685f 7175  ntextZ.search_qu
-000003e0: 6572 79da 0b6f 626a 6563 745f 6c69 7374  ery..object_list
-000003f0: 720b 0000 005a 0369 6473 da05 4d6f 6465  r....Z.ids..Mode
-00000400: 6c72 0a00 0000 5a10 7365 6172 6368 6162  lr....Z.searchab
-00000410: 6c65 5f66 6965 6c64 5a0f 7365 6172 6368  le_fieldZ.search
-00000420: 6162 6c65 5f64 6963 7472 1000 0000 7211  able_dictr....r.
-00000430: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
-00000440: a900 fa51 2f55 7365 7273 2f63 7275 7361  ...Q/Users/crusa
-00000450: 742f 7072 6f6a 6563 7473 2f67 6172 7069  t/projects/garpi
-00000460: 785f 7061 6765 2f62 6163 6b65 6e64 2f67  x_page/backend/g
-00000470: 6172 7069 785f 7061 6765 2f6d 6f64 656c  arpix_page/model
-00000480: 732f 6261 7365 5f73 6561 7263 685f 7061  s/base_search_pa
-00000490: 6765 2e70 7972 1300 0000 0a00 0000 7338  ge.pyr........s8
-000004a0: 0000 0000 010c 0114 010e 010a 0202 0116  ................
-000004b0: 010e 010a 0208 0104 010a 0106 010a 0208  ................
-000004c0: 0002 ff04 0310 0128 010e 020c 010a 0104  .......(........
-000004d0: 0102 0102 0102 0108 fc08 067a 1a42 6173  ...........z.Bas
-000004e0: 6553 6561 7263 6850 6167 652e 6765 745f  eSearchPage.get_
-000004f0: 636f 6e74 6578 7463 0000 0000 0000 0000  contextc........
-00000500: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000510: 7310 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000520: 0364 0253 0029 037a 1342 6173 6553 6561  .d.S.).z.BaseSea
-00000530: 7263 6850 6167 652e 4d65 7461 544e 2904  rchPage.MetaTN).
-00000540: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000550: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000560: 6d65 5f5f da08 6162 7374 7261 6374 722b  me__..abstractr+
-00000570: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
-00000580: 0000 da04 4d65 7461 2b00 0000 7302 0000  ....Meta+...s...
-00000590: 0008 0172 3100 0000 2901 4e29 0872 2d00  ...r1...).N).r-.
-000005a0: 0000 722e 0000 0072 2f00 0000 721f 0000  ..r....r/...r...
-000005b0: 00da 0874 656d 706c 6174 6572 1300 0000  ...templater....
-000005c0: 7231 0000 00da 0d5f 5f63 6c61 7373 6365  r1.....__classce
-000005d0: 6c6c 5f5f 722b 0000 0072 2b00 0000 7229  ll__r+...r+...r)
-000005e0: 0000 0072 2c00 0000 7206 0000 0006 0000  ...r,...r.......
-000005f0: 0073 0800 0000 0801 0401 0402 0e21 7206  .s...........!r.
-00000600: 0000 004e 2907 da09 6261 7365 5f70 6167  ...N)...base_pag
-00000610: 6572 0200 0000 da10 646a 616e 676f 2e64  er......django.d
-00000620: 622e 6d6f 6465 6c73 7204 0000 00da 1564  b.modelsr......d
-00000630: 6a61 6e67 6f2e 636f 7265 2e70 6167 696e  jango.core.pagin
-00000640: 6174 6f72 7205 0000 0072 0600 0000 722b  atorr....r....r+
-00000650: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
-00000660: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000670: 7306 0000 000c 010c 010c 03              s..........
+00000080: da01 5129 01da 0f47 6172 7069 7850 6167  ..Q)...GarpixPag
+00000090: 696e 6174 6f72 6300 0000 0000 0000 0000  inatorc.........
+000000a0: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
+000000b0: 3400 0000 6500 5a01 6400 5a02 6401 5a03  4...e.Z.d.Z.d.Z.
+000000c0: 6402 5a04 6408 8700 6601 6404 6405 8409  d.Z.d...f.d.d...
+000000d0: 5a05 4700 6406 6407 8400 6407 8302 5a06  Z.G.d.d...d...Z.
+000000e0: 8700 0400 5a07 5300 2909 da0e 4261 7365  ....Z.S.)...Base
+000000f0: 5365 6172 6368 5061 6765 e919 0000 007a  SearchPage.....z
+00000100: 1f67 6172 7069 785f 7061 6765 2f64 6566  .garpix_page/def
+00000110: 6175 6c74 5f73 6561 7263 682e 6874 6d6c  ault_search.html
+00000120: 4e63 0200 0000 0000 0000 0000 0000 1000  Nc..............
+00000130: 0000 0800 0000 0f00 0000 7316 0100 0064  ..........s....d
+00000140: 0164 026c 006d 017d 0401 0074 0283 006a  .d.l.m.}...t...j
+00000150: 037c 0166 017c 029e 027c 038e 017d 057c  .|.f.|...|...}.|
+00000160: 016a 04a0 0564 0364 00a1 027d 0674 066a  .j...d.d...}.t.j
+00000170: 07a0 08a1 007d 077a 1674 097c 016a 04a0  .....}.z.t.|.j..
+00000180: 0564 0464 05a1 0283 017d 0857 006e 1804  .d.d.....}.W.n..
+00000190: 0074 0a6b 0a72 6601 0001 0001 0064 057d  .t.k.rf......d.}
+000001a0: 0859 006e 0258 007c 0664 006b 0972 e267  .Y.n.X.|.d.k.r.g
+000001b0: 007d 097c 0483 0044 005d 587d 0a74 0b83  .}.|...D.]X}.t..
+000001c0: 007d 0b7c 0a6a 0c44 005d 207d 0c7c 0c9b  .}.|.j.D.] }.|..
+000001d0: 0064 069d 027c 0669 017d 0d7c 0b74 0b66  .d...|.i.}.|.t.f
+000001e0: 007c 0d8e 014f 007d 0b71 8a7c 0974 0d7c  .|...O.}.q.|.t.|
+000001f0: 0a6a 0e6a 0f64 0764 088d 01a0 0f7c 0ba1  .j.j.d.d.....|..
+00000200: 016a 1064 0964 0764 0a8d 0283 0137 007d  .j.d.d.d.....7.}
+00000210: 0971 7a74 066a 076a 0f7c 0964 0b8d 017d  .qzt.j.j.|.d...}
+00000220: 0774 117c 077c 006a 1283 027d 0e7c 0ea0  .t.|.|.j...}.|..
+00000230: 137c 08a1 017d 0f7c 05a0 147c 0e7c 0f7c  .|...}.|...|.|.|
+00000240: 087c 0690 0170 0a64 0c64 0d9c 04a1 0101  .|...p.d.d......
+00000250: 007c 0553 0029 0e4e e902 0000 0029 01da  .|.S.).N.....)..
+00000260: 1667 6574 5f67 6172 7069 785f 7061 6765  .get_garpix_page
+00000270: 5f6d 6f64 656c 73da 0171 da04 7061 6765  _models..q..page
+00000280: 7201 0000 005a 0b5f 5f69 636f 6e74 6169  r....Z.__icontai
+00000290: 6e73 5429 01da 0969 735f 6163 7469 7665  nsT)...is_active
+000002a0: da02 6964 2901 da04 666c 6174 2901 5a06  ..id)...flat).Z.
+000002b0: 6964 5f5f 696e da00 2904 da09 7061 6769  id__in..)...pagi
+000002c0: 6e61 746f 72da 1570 6167 696e 6174 6564  nator..paginated
+000002d0: 5f6f 626a 6563 745f 6c69 7374 720b 0000  _object_listr...
+000002e0: 0072 0a00 0000 2915 5a1c 7574 696c 732e  .r....).Z.utils.
+000002f0: 6765 745f 6761 7270 6978 5f70 6167 655f  get_garpix_page_
+00000300: 6d6f 6465 6c73 7209 0000 00da 0573 7570  modelsr......sup
+00000310: 6572 da0b 6765 745f 636f 6e74 6578 74da  er..get_context.
+00000320: 0347 4554 da03 6765 7472 0200 0000 da07  .GET..getr......
+00000330: 6f62 6a65 6374 73da 046e 6f6e 65da 0369  objects..none..i
+00000340: 6e74 da0a 5661 6c75 6545 7272 6f72 7204  nt..ValueErrorr.
+00000350: 0000 00da 1173 6561 7263 6861 626c 655f  .....searchable_
+00000360: 6669 656c 6473 da04 6c69 7374 da07 6f6e  fields..list..on
+00000370: 5f73 6974 65da 0666 696c 7465 72da 0b76  _site..filter..v
+00000380: 616c 7565 735f 6c69 7374 7205 0000 00da  alues_listr.....
+00000390: 0b70 6167 696e 6174 655f 6279 da08 6765  .paginate_by..ge
+000003a0: 745f 7061 6765 da06 7570 6461 7465 2910  t_page..update).
+000003b0: da04 7365 6c66 da07 7265 7175 6573 74da  ..self..request.
+000003c0: 0461 7267 73da 066b 7761 7267 7372 0900  .args..kwargsr..
+000003d0: 0000 da07 636f 6e74 6578 745a 0c73 6561  ....contextZ.sea
+000003e0: 7263 685f 7175 6572 79da 0b6f 626a 6563  rch_query..objec
+000003f0: 745f 6c69 7374 720b 0000 005a 0369 6473  t_listr....Z.ids
+00000400: da05 4d6f 6465 6c72 0a00 0000 5a10 7365  ..Modelr....Z.se
+00000410: 6172 6368 6162 6c65 5f66 6965 6c64 5a0f  archable_fieldZ.
+00000420: 7365 6172 6368 6162 6c65 5f64 6963 7472  searchable_dictr
+00000430: 1000 0000 7211 0000 00a9 01da 095f 5f63  ....r........__c
+00000440: 6c61 7373 5f5f a900 fa51 2f55 7365 7273  lass__...Q/Users
+00000450: 2f63 7275 7361 742f 7072 6f6a 6563 7473  /crusat/projects
+00000460: 2f67 6172 7069 785f 7061 6765 2f62 6163  /garpix_page/bac
+00000470: 6b65 6e64 2f67 6172 7069 785f 7061 6765  kend/garpix_page
+00000480: 2f6d 6f64 656c 732f 6261 7365 5f73 6561  /models/base_sea
+00000490: 7263 685f 7061 6765 2e70 7972 1300 0000  rch_page.pyr....
+000004a0: 0a00 0000 7338 0000 0000 010c 0114 010e  ....s8..........
+000004b0: 010a 0202 0116 010e 010a 0208 0104 010a  ................
+000004c0: 0106 010a 0208 0002 ff04 0310 0128 010e  .............(..
+000004d0: 020c 010a 0104 0102 0102 0102 0108 fc08  ................
+000004e0: 067a 1a42 6173 6553 6561 7263 6850 6167  .z.BaseSearchPag
+000004f0: 652e 6765 745f 636f 6e74 6578 7463 0000  e.get_contextc..
+00000500: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000510: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+00000520: 005a 0264 015a 0364 0253 0029 037a 1342  .Z.d.Z.d.S.).z.B
+00000530: 6173 6553 6561 7263 6850 6167 652e 4d65  aseSearchPage.Me
+00000540: 7461 544e 2904 da08 5f5f 6e61 6d65 5f5f  taTN)...__name__
+00000550: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000560: 7175 616c 6e61 6d65 5f5f da08 6162 7374  qualname__..abst
+00000570: 7261 6374 722b 0000 0072 2b00 0000 722b  ractr+...r+...r+
+00000580: 0000 0072 2c00 0000 da04 4d65 7461 2b00  ...r,.....Meta+.
+00000590: 0000 7302 0000 0008 0172 3100 0000 2901  ..s......r1...).
+000005a0: 4e29 0872 2d00 0000 722e 0000 0072 2f00  N).r-...r....r/.
+000005b0: 0000 721f 0000 00da 0874 656d 706c 6174  ..r......templat
+000005c0: 6572 1300 0000 7231 0000 00da 0d5f 5f63  er....r1.....__c
+000005d0: 6c61 7373 6365 6c6c 5f5f 722b 0000 0072  lasscell__r+...r
+000005e0: 2b00 0000 7229 0000 0072 2c00 0000 7206  +...r)...r,...r.
+000005f0: 0000 0006 0000 0073 0800 0000 0801 0401  .......s........
+00000600: 0402 0e21 7206 0000 004e 2907 da09 6261  ...!r....N)...ba
+00000610: 7365 5f70 6167 6572 0200 0000 da10 646a  se_pager......dj
+00000620: 616e 676f 2e64 622e 6d6f 6465 6c73 7204  ango.db.modelsr.
+00000630: 0000 00da 1667 6172 7069 785f 7574 696c  .....garpix_util
+00000640: 732e 7061 6769 6e61 746f 7272 0500 0000  s.paginatorr....
+00000650: 7206 0000 0072 2b00 0000 722b 0000 0072  r....r+...r+...r
+00000660: 2b00 0000 722c 0000 00da 083c 6d6f 6475  +...r,.....<modu
+00000670: 6c65 3e01 0000 0073 0600 0000 0c01 0c01  le>....s........
+00000680: 0c03                                     ..
```

### Comparing `garpix_page-2.8.0/garpix_page/models/base_list_page.py` & `garpix_page-2.9.0/garpix_page/models/base_list_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .base_page import BasePage
-from django.core.paginator import Paginator
+from garpix_utils.paginator import GarpixPaginator
 
 
 class BaseListPage(BasePage):
     paginate_by = 25
     template = 'garpix_page/default_list.html'
 
     def get_context(self, request=None, *args, **kwargs):
         context = super().get_context(request, *args, **kwargs)
 
         object_list = self.children.filter(is_active=True)
-        paginator = Paginator(object_list, self.paginate_by)
+        paginator = GarpixPaginator(object_list, self.paginate_by)
 
         try:
             page = int(request.GET.get('page', 1))
         except ValueError:
             page = 1
 
         paginated_object_list = paginator.get_page(page)
```

### Comparing `garpix_page-2.8.0/garpix_page/models/base_page.py` & `garpix_page-2.9.0/garpix_page/models/base_page.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/models/base_search_page.py` & `garpix_page-2.9.0/garpix_page/models/base_search_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .base_page import BasePage
 from django.db.models import Q
-from django.core.paginator import Paginator
+from garpix_utils.paginator import GarpixPaginator
 
 
 class BaseSearchPage(BasePage):
     paginate_by = 25
     template = 'garpix_page/default_search.html'
 
     def get_context(self, request=None, *args, **kwargs):
@@ -26,15 +26,15 @@
                     searchable_dict = {
                         f'{searchable_field}__icontains': search_query,
                     }
                     q |= Q(**searchable_dict)
                 ids += list(Model.on_site.filter(is_active=True).filter(q).values_list('id', flat=True))
             object_list = BasePage.objects.filter(id__in=ids)
 
-        paginator = Paginator(object_list, self.paginate_by)
+        paginator = GarpixPaginator(object_list, self.paginate_by)
         paginated_object_list = paginator.get_page(page)
         context.update({
             'paginator': paginator,
             'paginated_object_list': paginated_object_list,
             'page': page,
             'q': search_query or '',
         })
```

### Comparing `garpix_page-2.8.0/garpix_page/setup.py` & `garpix_page-2.9.0/garpix_page/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_page')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_page',
-    version='2.8.0',
+    version='2.9.0',
     description='',
     long_description=long_description,
     url='https://github.com/garpixcms/garpix_page',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
@@ -32,9 +32,10 @@
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-polymorphic-tree-for-garpix-page >= 2.0.1',
         'django-modeltranslation >= 0.16.2',
         'django-multiurl >= 1.4.0',
         'djangorestframework >= 3.12.4',
+        'garpix_utils >= 1.4.0'
     ],
 )
```

### Comparing `garpix_page-2.8.0/garpix_page/templates/garpix_page/admin_toolbar.html` & `garpix_page-2.9.0/garpix_page/templates/garpix_page/admin_toolbar.html`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/templates/garpix_page/default_search.html` & `garpix_page-2.9.0/garpix_page/templates/garpix_page/default_search.html`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/templates/garpix_page/index.html` & `garpix_page-2.9.0/garpix_page/templates/garpix_page/index.html`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/templates/garpix_page/seo.html` & `garpix_page-2.9.0/garpix_page/templates/garpix_page/seo.html`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/translation/__pycache__/base_page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/translation/__pycache__/base_page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/utils/__pycache__/check_redirect.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/utils/__pycache__/check_redirect.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/utils/__pycache__/get_file_path.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/utils/__pycache__/get_file_path.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/utils/__pycache__/get_garpix_page_models.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/utils/__pycache__/get_garpix_page_models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/utils/check_sites.py` & `garpix_page-2.9.0/garpix_page/utils/check_sites.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/utils/get_file_path.py` & `garpix_page-2.9.0/garpix_page/utils/get_file_path.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/views/__pycache__/page.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/views/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/views/__pycache__/page_api.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/views/__pycache__/page_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/views/__pycache__/sitemap.cpython-38.pyc` & `garpix_page-2.9.0/garpix_page/views/__pycache__/sitemap.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/views/page.py` & `garpix_page-2.9.0/garpix_page/views/page.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page/views/page_api.py` & `garpix_page-2.9.0/garpix_page/views/page_api.py`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/garpix_page.egg-info/PKG-INFO` & `garpix_page-2.9.0/garpix_page.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-page
-Version: 2.8.0
+Version: 2.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/garpixcms/garpix_page
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `garpix_page-2.8.0/garpix_page.egg-info/SOURCES.txt` & `garpix_page-2.9.0/garpix_page.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_page-2.8.0/setup.py` & `garpix_page-2.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_page')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_page',
-    version='2.8.0',
+    version='2.9.0',
     description='',
     long_description=long_description,
     url='https://github.com/garpixcms/garpix_page',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
@@ -32,9 +32,10 @@
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'django-polymorphic-tree-for-garpix-page >= 2.0.1',
         'django-modeltranslation >= 0.16.2',
         'django-multiurl >= 1.4.0',
         'djangorestframework >= 3.12.4',
+        'garpix_utils >= 1.4.0'
     ],
 )
```


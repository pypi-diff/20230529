# Comparing `tmp/garpixcms-4.1.1.tar.gz` & `tmp/garpixcms-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpixcms-4.1.1.tar", last modified: Fri May 12 13:23:20 2023, max compression
+gzip compressed data, was "garpixcms-4.2.0.tar", last modified: Mon May 29 10:13:16 2023, max compression
```

## Comparing `garpixcms-4.1.1.tar` & `garpixcms-4.2.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.109029 garpixcms-4.1.1/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-05-12 13:23:19.000000 garpixcms-4.1.1/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-12 13:23:20.108761 garpixcms-4.1.1/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.086426 garpixcms-4.1.1/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13366 2023-05-12 12:35:58.000000 garpixcms-4.1.1/garpixcms/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.087533 garpixcms-4.1.1/garpixcms/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.1.1/garpixcms/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.1.1/garpixcms/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.1.1/garpixcms/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/__pycache__/urls.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.087788 garpixcms-4.1.1/garpixcms/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/admin/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.089432 garpixcms-4.1.1/garpixcms/admin/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/admin/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/admin/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/apps.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.089877 garpixcms-4.1.1/garpixcms/contexts/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/contexts/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/contexts/global_context.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.090278 garpixcms-4.1.1/garpixcms/management/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/management/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.090379 garpixcms-4.1.1/garpixcms/management/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.1.1/garpixcms/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.090753 garpixcms-4.1.1/garpixcms/management/commands/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/management/commands/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/management/commands/update_user_module.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.091087 garpixcms-4.1.1/garpixcms/middleware/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/middleware/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.091949 garpixcms-4.1.1/garpixcms/middleware/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.1.1/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.1.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/middleware/locale.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.093210 garpixcms-4.1.1/garpixcms/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.093986 garpixcms-4.1.1/garpixcms/models/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/models/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/models/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-12 12:35:58.000000 garpixcms-4.1.1/garpixcms/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.084475 garpixcms-4.1.1/garpixcms/static/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.084647 garpixcms-4.1.1/garpixcms/static/admin/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.099760 garpixcms-4.1.1/garpixcms/static/admin/css/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/autocomplete.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/base.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/changelists.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/dashboard.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/fonts.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/forms.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/login.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/nav_sidebar.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/responsive.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/responsive_rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/rtl.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/tabbed_translation_fields.css
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/css/widgets.css
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.101762 garpixcms-4.1.1/garpixcms/static/admin/img/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/img/icon-addlink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/img/icon-changelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/img/icon-custom-checked.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/img/search.svg
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.101977 garpixcms-4.1.1/garpixcms/static/admin/js/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/static/admin/js/admin.js
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.084821 garpixcms-4.1.1/garpixcms/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.102716 garpixcms-4.1.1/garpixcms/templates/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/admin/app_list.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/admin/base.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/admin/base_site.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.102903 garpixcms-4.1.1/garpixcms/templates/garpixcms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/base.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.103683 garpixcms-4.1.1/garpixcms/templates/garpixcms/include/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/include/footer.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/include/header.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/include/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.104408 garpixcms-4.1.1/garpixcms/templates/garpixcms/menus/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/menus/footer_menu.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/menus/header_menu.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.105966 garpixcms-4.1.1/garpixcms/templates/garpixcms/pages/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/pages/default.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/pages/home.html
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/templates/garpixcms/pages/login.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.106737 garpixcms-4.1.1/garpixcms/translation/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/translation/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.107925 garpixcms-4.1.1/garpixcms/translation/__pycache__/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.1.1/garpixcms/translation/__pycache__/page.cpython-38.pyc
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/translation/page.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.1.1/garpixcms/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-12 13:23:20.087087 garpixcms-4.1.1/garpixcms.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-05-12 13:23:20.000000 garpixcms-4.1.1/garpixcms.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-12 13:23:20.109093 garpixcms-4.1.1/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-12 13:23:19.000000 garpixcms-4.1.1/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.186556 garpixcms-4.2.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-05-29 10:13:16.000000 garpixcms-4.2.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-29 10:13:16.186406 garpixcms-4.2.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.151274 garpixcms-4.2.0/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    13433 2023-05-29 10:12:36.000000 garpixcms-4.2.0/garpixcms/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1084 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       30 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1207 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.152488 garpixcms-4.2.0/garpixcms/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      161 2023-04-18 20:28:30.000000 garpixcms-4.2.0/garpixcms/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-04-18 20:28:30.000000 garpixcms-4.2.0/garpixcms/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6796 2023-04-18 20:28:30.000000 garpixcms-4.2.0/garpixcms/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1743 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/__pycache__/urls.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.152740 garpixcms-4.2.0/garpixcms/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       36 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.152987 garpixcms-4.2.0/garpixcms/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      205 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      487 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/admin/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      173 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/admin/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       93 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/apps.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.153208 garpixcms-4.2.0/garpixcms/contexts/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/contexts/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      691 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/contexts/global_context.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.153331 garpixcms-4.2.0/garpixcms/management/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/management/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.153441 garpixcms-4.2.0/garpixcms/management/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:01:00.000000 garpixcms-4.2.0/garpixcms/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.153663 garpixcms-4.2.0/garpixcms/management/commands/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/management/commands/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      872 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/management/commands/update_user_module.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.153872 garpixcms-4.2.0/garpixcms/middleware/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/middleware/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.154119 garpixcms-4.2.0/garpixcms/middleware/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      172 2023-05-10 14:00:43.000000 garpixcms-4.2.0/garpixcms/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2037 2023-05-10 14:00:43.000000 garpixcms-4.2.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2196 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/middleware/locale.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.154379 garpixcms-4.2.0/garpixcms/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.154789 garpixcms-4.2.0/garpixcms/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      201 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      818 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/models/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      413 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/models/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-29 10:13:07.000000 garpixcms-4.2.0/garpixcms/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.149413 garpixcms-4.2.0/garpixcms/static/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.149579 garpixcms-4.2.0/garpixcms/static/admin/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.163227 garpixcms-4.2.0/garpixcms/static/admin/css/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8440 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/autocomplete.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    22662 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/base.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6469 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/changelists.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      355 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/dashboard.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      423 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/fonts.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8370 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/forms.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1185 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/login.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    18344 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/responsive.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1741 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3487 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/rtl.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/tabbed_translation_fields.css
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10010 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/css/widgets.css
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.182865 garpixcms-4.2.0/garpixcms/static/admin/img/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      908 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      825 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      218 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/img/icon-custom-checked.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      705 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      930 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/img/search.svg
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.183051 garpixcms-4.2.0/garpixcms/static/admin/js/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      291 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/static/admin/js/admin.js
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.149749 garpixcms-4.2.0/garpixcms/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.184623 garpixcms-4.2.0/garpixcms/templates/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4421 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/admin/app_list.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4395 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/admin/base.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      809 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/admin/base_site.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.184764 garpixcms-4.2.0/garpixcms/templates/garpixcms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      450 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/base.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.185132 garpixcms-4.2.0/garpixcms/templates/garpixcms/include/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      730 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/include/footer.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      642 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/include/header.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      428 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/include/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.185400 garpixcms-4.2.0/garpixcms/templates/garpixcms/menus/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/menus/footer_menu.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/menus/header_menu.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.185774 garpixcms-4.2.0/garpixcms/templates/garpixcms/pages/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      139 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/pages/default.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      202 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/pages/home.html
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      346 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/templates/garpixcms/pages/login.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.185994 garpixcms-4.2.0/garpixcms/translation/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       49 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/translation/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.186236 garpixcms-4.2.0/garpixcms/translation/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      224 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/translation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      502 2023-04-18 20:28:31.000000 garpixcms-4.2.0/garpixcms/translation/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      189 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/translation/page.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1842 2023-04-18 19:40:20.000000 garpixcms-4.2.0/garpixcms/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-29 10:13:16.151921 garpixcms-4.2.0/garpixcms.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1766 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2848 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      401 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       10 2023-05-29 10:13:16.000000 garpixcms-4.2.0/garpixcms.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-29 10:13:16.186600 garpixcms-4.2.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1697 2023-05-29 10:13:16.000000 garpixcms-4.2.0/setup.py
```

### Comparing `garpixcms-4.1.1/PKG-INFO` & `garpixcms-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.1.1
+Version: 4.2.0
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.1.1/garpixcms/CHANGELOG.md` & `garpixcms-4.2.0/garpixcms/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 4.2.0 (29.05.2023)
+
+- Upgrade `garpix_page` to version 2.47.0
+
 ### 4.1.1 (12.05.2023)
 
 - Upgrade `garpix_page` to version 2.46.1
 
 ### 4.1.0 (12.05.2023)
 
 - Upgrade `garpix_page` to version 2.46.0
```

### Comparing `garpixcms-4.1.1/garpixcms/CONTRIBUTING.md` & `garpixcms-4.2.0/garpixcms/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/README.rst` & `garpixcms-4.2.0/garpixcms/README.rst`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/__pycache__/settings.cpython-38.pyc` & `garpixcms-4.2.0/garpixcms/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/__pycache__/urls.cpython-38.pyc` & `garpixcms-4.2.0/garpixcms/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/contexts/global_context.py` & `garpixcms-4.2.0/garpixcms/contexts/global_context.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/management/commands/update_user_module.py` & `garpixcms-4.2.0/garpixcms/management/commands/update_user_module.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/middleware/__pycache__/locale.cpython-38.pyc` & `garpixcms-4.2.0/garpixcms/middleware/__pycache__/locale.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/middleware/locale.py` & `garpixcms-4.2.0/garpixcms/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/models/__pycache__/page.cpython-38.pyc` & `garpixcms-4.2.0/garpixcms/models/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/settings.py` & `garpixcms-4.2.0/garpixcms/settings.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/setup.py` & `garpixcms-4.2.0/garpixcms/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.1.1',
+    version='4.2.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -28,15 +28,15 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
-        'garpix_page == 2.46.1',
+        'garpix_page == 2.47.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
         'garpix_user == 3.5.0',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
```

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/autocomplete.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/base.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/changelists.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/forms.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/login.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/nav_sidebar.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/responsive.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/responsive_rtl.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/rtl.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/css/widgets.css` & `garpixcms-4.2.0/garpixcms/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/img/icon-addlink.svg` & `garpixcms-4.2.0/garpixcms/static/admin/img/icon-addlink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/img/icon-changelink.svg` & `garpixcms-4.2.0/garpixcms/static/admin/img/icon-changelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/img/icon-deletelink.svg` & `garpixcms-4.2.0/garpixcms/static/admin/img/icon-deletelink.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/static/admin/img/search.svg` & `garpixcms-4.2.0/garpixcms/static/admin/img/search.svg`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/templates/admin/app_list.html` & `garpixcms-4.2.0/garpixcms/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/templates/admin/base.html` & `garpixcms-4.2.0/garpixcms/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/templates/admin/base_site.html` & `garpixcms-4.2.0/garpixcms/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/templates/garpixcms/include/footer.html` & `garpixcms-4.2.0/garpixcms/templates/garpixcms/include/footer.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/templates/garpixcms/include/header.html` & `garpixcms-4.2.0/garpixcms/templates/garpixcms/include/header.html`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms/urls.py` & `garpixcms-4.2.0/garpixcms/urls.py`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/garpixcms.egg-info/PKG-INFO` & `garpixcms-4.2.0/garpixcms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpixcms
-Version: 4.1.1
+Version: 4.2.0
 Home-page: https://github.com/garpixcms/garpixcms
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpixcms-4.1.1/garpixcms.egg-info/SOURCES.txt` & `garpixcms-4.2.0/garpixcms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpixcms-4.1.1/setup.py` & `garpixcms-4.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpixcms')
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpixcms',
-    version='4.1.1',
+    version='4.2.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpixcms',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -28,15 +28,15 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 3.1, < 4',
         'garpix_utils == 1.8.0',
-        'garpix_page == 2.46.1',
+        'garpix_page == 2.47.0',
         'garpix_menu == 1.16.0',
         'eqator == 2.7.0',
         'garpix_auth == 2.3.0',
         'garpix_notify == 5.16.0',
         'garpix_user == 3.5.0',
         'garpix_package == 2.0.1',
         'psycopg2-binary >= 2.8.6',
```


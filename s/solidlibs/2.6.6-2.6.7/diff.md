# Comparing `tmp/solidlibs-2.6.6.tar.gz` & `tmp/solidlibs-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidlibs-2.6.6.tar", last modified: Wed May 24 08:08:41 2023, max compression
+gzip compressed data, was "solidlibs-2.6.7.tar", last modified: Mon May 29 12:29:52 2023, max compression
```

## Comparing `solidlibs-2.6.6.tar` & `solidlibs-2.6.7.tar`

### file list

```diff
@@ -1,471 +1,471 @@
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.110609 solidlibs-2.6.6/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      105 2023-05-20 08:29:26.000000 solidlibs-2.6.6/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1669 2023-05-24 08:08:41.110609 solidlibs-2.6.6/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      675 2023-05-24 06:13:24.000000 solidlibs-2.6.6/README.md
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2023-05-24 08:08:41.110609 solidlibs-2.6.6/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1413 2023-05-24 08:08:40.000000 solidlibs-2.6.6/setup.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      224 2023-05-17 14:01:55.000000 solidlibs-2.6.6/solidlibs/__init__.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.038609 solidlibs-2.6.6/solidlibs/django_addons/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      278 2023-05-17 13:50:05.000000 solidlibs-2.6.6/solidlibs/django_addons/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2023-05-17 13:56:22.000000 solidlibs-2.6.6/solidlibs/django_addons/apps.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.038609 solidlibs-2.6.6/solidlibs/django_addons/context_processors/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3933 2023-05-17 13:46:13.000000 solidlibs-2.6.6/solidlibs/django_addons/context_processors/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3054 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/context_processors/css_selector.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6931 2023-05-17 13:55:29.000000 solidlibs-2.6.6/solidlibs/django_addons/data_image.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.038609 solidlibs-2.6.6/solidlibs/django_addons/middleware/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      186 2023-05-17 08:29:12.000000 solidlibs-2.6.6/solidlibs/django_addons/middleware/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2083 2023-05-17 13:47:28.000000 solidlibs-2.6.6/solidlibs/django_addons/middleware/debug.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3297 2023-05-17 13:46:45.000000 solidlibs-2.6.6/solidlibs/django_addons/middleware/proxy404.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2062 2023-05-17 13:47:22.000000 solidlibs-2.6.6/solidlibs/django_addons/middleware/redirect404.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1329 2023-05-17 13:46:38.000000 solidlibs-2.6.6/solidlibs/django_addons/middleware/template.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       27 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/models.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3308 2023-05-17 13:55:19.000000 solidlibs-2.6.6/solidlibs/django_addons/singleton.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.038609 solidlibs-2.6.6/solidlibs/django_addons/static/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.042610 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      730 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/action_icons.1e02e82dbdcd.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      670 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/action_icons.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9114 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/autocomplete.4a81fc4242d0.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9114 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/autocomplete.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20509 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/base.01580fff1759.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20344 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/base.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6395 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/changelists.ae46354f4e80.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6395 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/changelists.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dark_mode.4e3d1504ca81.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dark_mode.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dashboard.be83f13e4369.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dashboard.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      462 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/fonts.168bab448fee.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      423 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/fonts.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8987 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/forms.c192d1ec6902.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8944 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/forms.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      958 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/login.586129c60a93.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      958 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/login.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2619 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/nav_sidebar.30423191f399.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2619 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/nav_sidebar.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1254 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/object_tools.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1284 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/object_tools.ec5c6a50631e.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    18854 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive.02281633b5f1.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    18854 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1741 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive_rtl.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1741 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive_rtl.e13ae754cceb.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3628 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/rtl.8473f45bd49b.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3598 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/rtl.css
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.030609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.042610 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.md
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    17358 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.a2194c262648.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    17358 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    14966 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.9f54e6414f87.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    14966 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11507 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/widgets.00318bc424d3.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11297 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/widgets.css
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.046609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/LICENSE.d273d63619c9.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/LICENSE.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      214 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/README.ab99e6b541ea.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      214 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/README.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    86184 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.50d75e48e0a3.woff
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    86184 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.woff
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85692 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.c73eb1ceba33.woff
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85692 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.woff
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85876 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.35b07eb2f871.woff
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85876 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.woff
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.050609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1081 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/LICENSE
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1081 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/LICENSE.2c54f4e1ca1c
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      319 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/README.a70711a38d87.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      319 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/README.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1094 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/calendar-icons.39b290681a8b.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1094 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/calendar-icons.svg
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.050609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.0047eba25b67.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-addlink.d519b3bab011.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-addlink.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      504 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-alert.034cc7d8a67f.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      504 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-alert.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1086 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-calendar.ac7aea671bea.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1086 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-calendar.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-changelink.18d2fd706348.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-changelink.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      677 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-clock.e1d4dfac3f2b.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      677 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-clock.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      392 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-deletelink.564ef9dc3854.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      392 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-deletelink.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-no.439e821418cd.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-no.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown-alt.81536e128bb6.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown-alt.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown.a18cb4398978.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      581 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-viewlink.41eb31f7826e.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      581 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-viewlink.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      436 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-yes.d2f9f035226a.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      436 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-yes.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/inline-delete.fec1b761f254.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/inline-delete.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      458 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/search.7cf54ff789c6.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      458 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/search.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3291 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/selector-icons.b4555096cea2.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3291 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/selector-icons.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/sorting-icons.3a097b59f104.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/sorting-icons.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/tooltag-add.e59d620a9742.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/tooltag-add.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      280 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/tooltag-arrowright.bbfb788a849e.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      280 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/tooltag-arrowright.svg
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.058609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4360 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectBox.8161741c7647.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4360 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectBox.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11317 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectFilter2.3f53e33c88d6.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11317 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectFilter2.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7872 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.eac7e3441574.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7872 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.min.5fa8cb0403f1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.min.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.058609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19379 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.300591891b2b.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19379 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8985 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.de5309ac06dd.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8985 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1060 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/autocomplete.01591ab27be7.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1060 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/autocomplete.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8466 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/calendar.f8a5d055eb33.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8466 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/calendar.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      884 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/cancel.ecc4c5ca7b32.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      884 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/cancel.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      606 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/change_form.9d8ca4f96b75.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      606 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/change_form.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1803 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.f84e7410290f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1803 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1685 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.min.2ee8a0086864.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1685 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5698 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/core.5d6b384a08b5.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5698 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/core.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      966 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/filters.295a9d3d8b6a.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      966 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/filters.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15526 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.22d4d93c00b4.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15526 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5864 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.min.4d23f8660b21.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5864 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/jquery.init.b7781a0897fc.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/jquery.init.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3763 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/nav_sidebar.36a64ecb39ed.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3763 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/nav_sidebar.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/popup_response.c6cc78ea5551.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/popup_response.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1531 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.bd2361dfd64d.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1531 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      379 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.min.85fd5e0fb706.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      379 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      586 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate_init.6cac7f3105b8.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      586 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate_init.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.058609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6538 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.2fb8e8349c22.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6538 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.min.5fa8cb0403f1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2984 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/timeparse.51258861a46a.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2984 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/timeparse.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7902 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/urlify.25cc3eac8123.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7902 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/urlify.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.062610 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.2849239b95f5.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.8fb8fee4fcc3.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.062610 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.f94142512c91.md
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.md
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.078609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      905 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      905 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      721 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.270c257daf81.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      721 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      968 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      968 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1291 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1291 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      965 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.91624382358e.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      965 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.a166b745933a.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1292 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1292 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      828 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.766346afe4dd.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      828 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.8a1c222b0204.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1017 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1017 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1182 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.27097f071856.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1182 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      844 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.cf932ba09a98.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      844 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      922 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      922 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      801 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.2b96fd98289d.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      801 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      868 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      868 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1023 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1023 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      803 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      803 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      984 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      984 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1175 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.70640d41628f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1175 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      852 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      852 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1018 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1018 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      831 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      831 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1028 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1028 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.04debded514d.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      807 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      807 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      897 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      897 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      862 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.170ae885d74f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      862 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.2083264a54f0.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1195 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1088 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.c23089cb06ca.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1088 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      855 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      855 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      944 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.23c7ce903300.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      944 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.08e62128eac1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1038 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.dabbb9087130.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1038 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      811 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      811 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      778 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.da2fce143f27.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      778 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1357 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1357 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      904 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.997868a37ed8.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      904 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      947 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.6031b4f16452.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      947 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1049 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1049 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      876 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      876 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      878 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      878 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      938 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      938 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1171 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1171 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1306 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1306 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      925 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.131a78bc0752.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      925 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      903 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      903 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      980 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      980 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      786 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      786 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1074 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.f38c20b0221b.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1074 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      771 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      771 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      775 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      775 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1156 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1156 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      707 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      707 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   173566 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.c2afdeda3058.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   173566 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    79212 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    79212 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.078609 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1103 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1103 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   232381 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.efda034b9537.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   232381 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   125266 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   125266 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.js
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.086609 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    67871 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   157964 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.468fca75a599.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   157964 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    67884 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.db5f9ed61039.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    50948 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.3a434cc0b44e.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    50935 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   115021 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.57e1ce0c5850.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   115021 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4806 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.921561dba489.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4793 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    77346 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.602658511f99.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    77346 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3940 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.677eb73b7cf8.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3927 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    32546 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.88a457cfbc95.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    32546 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   197183 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.668abc6a7653.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   197170 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   504418 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.4563f76d1380.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   504418 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   159528 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.3a855e8d68d8.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   159515 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   641867 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.2e863a645ac3.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   641867 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.098610 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   227993 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.9e7256cb17ff.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   227980 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   410007 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.f71cf6369adc.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   410007 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    80711 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.451eff9b562a.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    80698 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   318045 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.4e47e3045b5c.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   318045 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   135092 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.ffede5391ab5.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   135079 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   256099 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.a73716a97566.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   256099 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    60023 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.874762f06dc0.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    60010 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   194435 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.e7faa89b97be.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   194435 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   522340 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.155fd16d1aa1.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   522340 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   372911 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js.8cd46a572e05.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   372911 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   176010 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.808bdaf3f29c.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   176010 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   271775 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js.6a4eee3bf46c.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   271775 2022-12-29 11:19:12.000000 solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js.map
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.098610 solidlibs-2.6.6/solidlibs/django_addons/static/css/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1519 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/admin.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      406 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/bignum.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4807 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/black-rock.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   155838 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/blackrock-digital.original.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      323 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/btn_hov-png.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      981 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/django_addons.bootstrap.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      444 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/django_addons.bootstrap.min.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1262 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/sudoSlider.css
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      609 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/css/tufte-graph.css
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.098610 solidlibs-2.6.6/solidlibs/django_addons/static/images/
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)      246 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/Hamburger_icon.png
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      605 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/Hamburger_icon.svg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      342 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/Kebab_icon.png
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4367 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/Kebab_icon.svg
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.102609 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4934 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/comments.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4465 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/delicious.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     5068 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/digg.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4800 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/facebook.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4738 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/flickr.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4856 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/linkedin.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     5053 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/rss.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4882 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/stumbleupon.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4788 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/technorati.png
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4765 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/twitter.png
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.102609 solidlibs-2.6.6/solidlibs/django_addons/static/js/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   137972 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.min.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.min.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)   137972 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.min.map
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19033 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/popper.js
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19033 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/js/popper.min.js
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)      173 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/static/robots.txt
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs/django_addons/templates/
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.102609 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/403.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      943 2023-05-17 13:48:16.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/404.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1111 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/500.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/50x.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6826 2023-05-20 23:16:22.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/base_content.html
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.106609 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      526 2023-05-17 13:49:29.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/change_language.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      408 2023-05-17 13:49:10.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/css_basic.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1025 2023-05-17 13:49:35.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/form_error_handling.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      576 2023-05-17 13:49:22.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/form_field_error_handling.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      360 2023-05-17 13:49:16.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/js_basic.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      741 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/json2.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2335 2023-05-17 13:49:47.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/sign_in.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1390 2023-05-17 13:49:41.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/user_tools.html
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1524 2023-05-17 13:47:34.000000 solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/csrf.html
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.106609 solidlibs-2.6.6/solidlibs/django_addons/templatetags/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15817 2023-05-17 08:29:29.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/custom.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      890 2023-05-17 08:29:29.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/data_img.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2686 2023-05-17 08:29:29.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/expr.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      837 2022-04-23 12:10:56.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/lookup.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3320 2023-05-17 08:27:13.000000 solidlibs-2.6.6/solidlibs/django_addons/templatetags/var.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9099 2023-05-17 13:54:50.000000 solidlibs-2.6.6/solidlibs/django_addons/utils.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4544 2023-05-17 13:55:34.000000 solidlibs-2.6.6/solidlibs/django_addons/views.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.106609 solidlibs-2.6.6/solidlibs/net/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      225 2023-05-17 13:52:17.000000 solidlibs-2.6.6/solidlibs/net/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20719 2023-05-17 23:06:53.000000 solidlibs-2.6.6/solidlibs/net/browser.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19278 2023-05-18 06:40:11.000000 solidlibs-2.6.6/solidlibs/net/html_addons.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16236 2023-05-17 23:08:06.000000 solidlibs-2.6.6/solidlibs/net/http_addons.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2168 2023-05-17 13:52:11.000000 solidlibs-2.6.6/solidlibs/net/mime_constants.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15502 2023-05-17 13:52:25.000000 solidlibs-2.6.6/solidlibs/net/openssl.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    23792 2023-05-17 23:09:41.000000 solidlibs-2.6.6/solidlibs/net/utils.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    10269 2023-05-17 23:09:43.000000 solidlibs-2.6.6/solidlibs/net/web_log_parser.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.106609 solidlibs-2.6.6/solidlibs/os/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      230 2023-05-17 13:45:34.000000 solidlibs-2.6.6/solidlibs/os/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6640 2023-05-17 13:45:23.000000 solidlibs-2.6.6/solidlibs/os/cli.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19351 2023-05-19 15:52:40.000000 solidlibs-2.6.6/solidlibs/os/command.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7735 2023-05-17 13:45:41.000000 solidlibs-2.6.6/solidlibs/os/drive.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    40531 2023-05-17 13:45:29.000000 solidlibs-2.6.6/solidlibs/os/fs.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16781 2023-05-17 13:45:06.000000 solidlibs-2.6.6/solidlibs/os/lock.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3447 2023-05-17 13:44:47.000000 solidlibs-2.6.6/solidlibs/os/osid.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15556 2023-05-17 13:44:42.000000 solidlibs-2.6.6/solidlibs/os/process.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3997 2023-05-17 13:45:01.000000 solidlibs-2.6.6/solidlibs/os/profile_addons.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    10113 2023-05-18 06:24:55.000000 solidlibs-2.6.6/solidlibs/os/user.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.110609 solidlibs-2.6.6/solidlibs/python/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      238 2023-05-17 13:43:23.000000 solidlibs-2.6.6/solidlibs/python/__init__.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2929 2023-05-17 13:41:49.000000 solidlibs-2.6.6/solidlibs/python/_log.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5668 2023-05-17 13:41:37.000000 solidlibs-2.6.6/solidlibs/python/abstract_build_venv.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    25506 2023-05-17 13:43:58.000000 solidlibs-2.6.6/solidlibs/python/dict.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2238 2023-05-17 13:42:02.000000 solidlibs-2.6.6/solidlibs/python/elapsed_time.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    26570 2023-05-17 13:43:36.000000 solidlibs-2.6.6/solidlibs/python/format.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    22781 2023-05-18 06:24:54.000000 solidlibs-2.6.6/solidlibs/python/internals.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5345 2023-05-17 13:44:23.000000 solidlibs-2.6.6/solidlibs/python/iter.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    29579 2023-05-18 06:24:54.000000 solidlibs-2.6.6/solidlibs/python/log.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5784 2023-05-17 13:43:12.000000 solidlibs-2.6.6/solidlibs/python/performance.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3064 2023-05-17 13:42:38.000000 solidlibs-2.6.6/solidlibs/python/text_file.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    49198 2023-05-17 13:44:14.000000 solidlibs-2.6.6/solidlibs/python/times.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20476 2023-05-17 13:41:29.000000 solidlibs-2.6.6/solidlibs/python/utils.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16694 2023-05-17 13:44:05.000000 solidlibs-2.6.6/solidlibs/python/ve.py
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      223 2023-05-17 14:06:29.000000 solidlibs-2.6.6/solidlibs/version.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:41.034609 solidlibs-2.6.6/solidlibs.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1669 2023-05-24 08:08:40.000000 solidlibs-2.6.6/solidlibs.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)    27040 2023-05-24 08:08:40.000000 solidlibs-2.6.6/solidlibs.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2023-05-24 08:08:40.000000 solidlibs-2.6.6/solidlibs.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       10 2023-05-24 08:08:40.000000 solidlibs-2.6.6/solidlibs.egg-info/top_level.txt
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.455707 solidlibs-2.6.7/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      105 2023-05-20 08:29:26.000000 solidlibs-2.6.7/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1669 2023-05-29 12:29:52.455707 solidlibs-2.6.7/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      675 2023-05-24 06:13:24.000000 solidlibs-2.6.7/README.md
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2023-05-29 12:29:52.455707 solidlibs-2.6.7/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1413 2023-05-29 12:29:40.000000 solidlibs-2.6.7/setup.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.303707 solidlibs-2.6.7/solidlibs/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      224 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/__init__.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.303707 solidlibs-2.6.7/solidlibs/django_addons/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      278 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/apps.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.307707 solidlibs-2.6.7/solidlibs/django_addons/context_processors/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3933 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/context_processors/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3054 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/context_processors/css_selector.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6931 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/data_image.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.307707 solidlibs-2.6.7/solidlibs/django_addons/middleware/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      186 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/middleware/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2083 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/middleware/debug.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3297 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/middleware/proxy404.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2062 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/middleware/redirect404.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1329 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/middleware/template.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       27 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/models.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3308 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/singleton.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.307707 solidlibs-2.6.7/solidlibs/django_addons/static/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.299707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.315707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      730 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/action_icons.1e02e82dbdcd.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      670 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/action_icons.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9114 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/autocomplete.4a81fc4242d0.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9114 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/autocomplete.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20509 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/base.01580fff1759.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20344 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/base.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6395 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/changelists.ae46354f4e80.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6395 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/changelists.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dark_mode.4e3d1504ca81.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dark_mode.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dashboard.be83f13e4369.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dashboard.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      462 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/fonts.168bab448fee.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      423 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/fonts.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8987 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/forms.c192d1ec6902.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8944 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/forms.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      958 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/login.586129c60a93.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      958 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/login.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2619 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/nav_sidebar.30423191f399.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2619 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/nav_sidebar.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1254 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/object_tools.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1284 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/object_tools.ec5c6a50631e.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    18854 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive.02281633b5f1.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    18854 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1741 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive_rtl.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1741 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive_rtl.e13ae754cceb.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3628 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/rtl.8473f45bd49b.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3598 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/rtl.css
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.299707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.315707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    17358 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.a2194c262648.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    17358 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    14966 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.9f54e6414f87.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    14966 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11507 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/widgets.00318bc424d3.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11297 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/widgets.css
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.315707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/LICENSE.d273d63619c9.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/LICENSE.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      214 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/README.ab99e6b541ea.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      214 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/README.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    86184 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.50d75e48e0a3.woff
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    86184 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.woff
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85692 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.c73eb1ceba33.woff
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85692 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.woff
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85876 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.35b07eb2f871.woff
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    85876 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.woff
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.323707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1081 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/LICENSE
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1081 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/LICENSE.2c54f4e1ca1c
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      319 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/README.a70711a38d87.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      319 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/README.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1094 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/calendar-icons.39b290681a8b.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1094 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/calendar-icons.svg
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.323707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.0047eba25b67.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1129 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-addlink.d519b3bab011.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-addlink.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      504 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-alert.034cc7d8a67f.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      504 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-alert.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1086 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-calendar.ac7aea671bea.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1086 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-calendar.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-changelink.18d2fd706348.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      380 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-changelink.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      677 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-clock.e1d4dfac3f2b.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      677 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-clock.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      392 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-deletelink.564ef9dc3854.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      392 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-deletelink.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-no.439e821418cd.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-no.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown-alt.81536e128bb6.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown.a18cb4398978.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      655 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      581 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-viewlink.41eb31f7826e.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      581 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-viewlink.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      436 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-yes.d2f9f035226a.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      436 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-yes.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/inline-delete.fec1b761f254.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      560 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/inline-delete.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      458 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/search.7cf54ff789c6.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      458 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/search.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3291 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/selector-icons.b4555096cea2.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3291 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/selector-icons.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/sorting-icons.3a097b59f104.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/sorting-icons.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/tooltag-add.e59d620a9742.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      331 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/tooltag-add.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      280 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/tooltag-arrowright.bbfb788a849e.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      280 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/tooltag-arrowright.svg
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.327707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4360 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectBox.8161741c7647.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4360 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectBox.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11317 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectFilter2.3f53e33c88d6.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    11317 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectFilter2.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7872 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.eac7e3441574.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7872 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.min.5fa8cb0403f1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.min.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.331707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19379 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.300591891b2b.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19379 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8985 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.de5309ac06dd.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8985 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1060 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/autocomplete.01591ab27be7.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1060 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/autocomplete.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8466 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/calendar.f8a5d055eb33.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     8466 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/calendar.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      884 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/cancel.ecc4c5ca7b32.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      884 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/cancel.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      606 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/change_form.9d8ca4f96b75.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      606 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/change_form.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1803 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.f84e7410290f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1803 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1685 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.min.2ee8a0086864.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1685 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5698 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/core.5d6b384a08b5.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5698 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/core.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      966 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/filters.295a9d3d8b6a.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      966 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/filters.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15526 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.22d4d93c00b4.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15526 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5864 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.min.4d23f8660b21.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5864 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/jquery.init.b7781a0897fc.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      347 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/jquery.init.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3763 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/nav_sidebar.36a64ecb39ed.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3763 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/nav_sidebar.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/popup_response.c6cc78ea5551.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      551 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/popup_response.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1531 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.bd2361dfd64d.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1531 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      379 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.min.85fd5e0fb706.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      379 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      586 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate_init.6cac7f3105b8.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      586 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate_init.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.331707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6538 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.2fb8e8349c22.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6538 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.min.5fa8cb0403f1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2984 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/timeparse.51258861a46a.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2984 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/timeparse.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7902 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/urlify.25cc3eac8123.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7902 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/urlify.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.299707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.331707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1097 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.2849239b95f5.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.8fb8fee4fcc3.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.335707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.f94142512c91.md
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1124 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.md
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.351707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      905 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      905 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      721 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.270c257daf81.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      721 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      968 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      968 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1291 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1291 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      965 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.91624382358e.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      965 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.a166b745933a.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1292 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1292 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      828 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.766346afe4dd.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      828 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.8a1c222b0204.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      866 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1017 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1017 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1182 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.27097f071856.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1182 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      844 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.cf932ba09a98.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      844 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      922 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      922 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      801 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.2b96fd98289d.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      801 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      868 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      868 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1023 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1023 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      803 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      803 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      924 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      984 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      984 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1175 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.70640d41628f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1175 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      852 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      852 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1018 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1018 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      831 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      831 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1028 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1028 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.04debded514d.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      807 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      807 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      897 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      897 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      862 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.170ae885d74f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      862 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.2083264a54f0.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1195 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1088 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.c23089cb06ca.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1088 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      855 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      855 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      944 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.23c7ce903300.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      944 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.08e62128eac1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      900 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1038 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.dabbb9087130.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1038 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      811 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      811 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      778 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.da2fce143f27.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      778 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1357 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1357 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      904 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.997868a37ed8.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      904 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      947 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.6031b4f16452.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      947 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1049 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1049 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      876 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      876 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      878 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      878 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      938 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      938 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1171 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1171 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1306 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1306 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      925 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.131a78bc0752.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      925 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      903 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      903 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      980 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      980 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      786 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      786 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1074 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.f38c20b0221b.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1074 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      771 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      771 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      775 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      775 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1156 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1156 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      796 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      768 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      707 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      707 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   173566 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.c2afdeda3058.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   173566 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    79212 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    79212 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.351707 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1103 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1103 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   232381 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.efda034b9537.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   232381 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   125266 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   125266 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.js
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.299707 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.359707 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    67871 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   157964 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.468fca75a599.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   157964 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    67884 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.db5f9ed61039.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    50948 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.3a434cc0b44e.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    50935 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   115021 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.57e1ce0c5850.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   115021 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4806 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.921561dba489.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4793 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    77346 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.602658511f99.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    77346 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3940 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.677eb73b7cf8.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3927 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    32546 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.88a457cfbc95.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    32546 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   197183 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.668abc6a7653.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   197170 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   504418 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.4563f76d1380.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   504418 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   159528 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.3a855e8d68d8.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   159515 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   641867 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.2e863a645ac3.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   641867 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.375707 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   227993 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.9e7256cb17ff.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   227980 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   410007 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.f71cf6369adc.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   410007 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    80711 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.451eff9b562a.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    80698 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   318045 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.4e47e3045b5c.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   318045 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   135092 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.ffede5391ab5.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   135079 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   256099 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.a73716a97566.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   256099 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    60023 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.874762f06dc0.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    60010 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   194435 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.e7faa89b97be.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   194435 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   522340 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.155fd16d1aa1.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   522340 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   372911 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js.8cd46a572e05.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   372911 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   176010 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.808bdaf3f29c.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   176010 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   271775 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js.6a4eee3bf46c.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   271775 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js.map
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.375707 solidlibs-2.6.7/solidlibs/django_addons/static/css/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1519 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/admin.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      406 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/bignum.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4807 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/black-rock.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   155838 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/blackrock-digital.original.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      323 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/btn_hov-png.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      981 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/django_addons.bootstrap.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      444 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/django_addons.bootstrap.min.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1262 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/sudoSlider.css
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      609 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/css/tufte-graph.css
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.375707 solidlibs-2.6.7/solidlibs/django_addons/static/images/
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)      246 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/Hamburger_icon.png
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      605 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/Hamburger_icon.svg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      342 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/Kebab_icon.png
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4367 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/Kebab_icon.svg
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.375707 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4934 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/comments.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4465 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/delicious.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     5068 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/digg.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4800 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/facebook.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4738 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/flickr.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4856 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/linkedin.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     5053 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/rss.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4882 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/stumbleupon.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4788 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/technorati.png
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)     4765 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/twitter.png
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.379707 solidlibs-2.6.7/solidlibs/django_addons/static/js/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   137972 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.min.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   288580 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    89501 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.min.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)   137972 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.min.map
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19033 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/popper.js
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19033 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/static/js/popper.min.js
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)      173 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/static/robots.txt
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.299707 solidlibs-2.6.7/solidlibs/django_addons/templates/
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.379707 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/403.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      943 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/404.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1111 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/500.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1109 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/50x.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6826 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/base_content.html
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.379707 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      526 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/change_language.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      408 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/css_basic.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1025 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/form_error_handling.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      576 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/form_field_error_handling.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      360 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/js_basic.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      741 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/json2.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2335 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/sign_in.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1390 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/user_tools.html
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1524 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/csrf.html
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.383707 solidlibs-2.6.7/solidlibs/django_addons/templatetags/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15817 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/custom.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      890 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/data_img.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2686 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/expr.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      837 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/lookup.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3320 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/django_addons/templatetags/var.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     9099 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/utils.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     4544 2023-05-29 09:05:31.000000 solidlibs-2.6.7/solidlibs/django_addons/views.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.383707 solidlibs-2.6.7/solidlibs/net/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      225 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20719 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/browser.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19278 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/html_addons.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16236 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/http_addons.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2168 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/mime_constants.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15502 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/openssl.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    23792 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/utils.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    10269 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/net/web_log_parser.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.383707 solidlibs-2.6.7/solidlibs/os/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      230 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     6640 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/cli.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    19351 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/command.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     7735 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/drive.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    40531 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/fs.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16781 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/lock.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3447 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/osid.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    15556 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/process.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3997 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/profile_addons.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    10113 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/os/user.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.447707 solidlibs-2.6.7/solidlibs/python/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      238 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/__init__.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2929 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/_log.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5668 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/abstract_build_venv.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    25506 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/dict.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     2238 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/elapsed_time.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    26570 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/format.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    22781 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/internals.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5345 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/iter.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    29579 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/log.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5784 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/performance.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3064 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/text_file.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    49198 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/times.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    20476 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/utils.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    16694 2023-05-29 09:05:32.000000 solidlibs-2.6.7/solidlibs/python/ve.py
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      223 2023-05-29 12:28:53.000000 solidlibs-2.6.7/solidlibs/version.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:29:52.303707 solidlibs-2.6.7/solidlibs.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1669 2023-05-29 12:29:50.000000 solidlibs-2.6.7/solidlibs.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)    27040 2023-05-29 12:29:51.000000 solidlibs-2.6.7/solidlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2023-05-29 12:29:50.000000 solidlibs-2.6.7/solidlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       10 2023-05-29 12:29:50.000000 solidlibs-2.6.7/solidlibs.egg-info/top_level.txt
```

### Comparing `solidlibs-2.6.6/PKG-INFO` & `solidlibs-2.6.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidlibs
-Version: 2.6.6
+Version: 2.6.7
 Summary: Open source python and django enhancements
 Home-page: https://github.com/safeapps/solidlibs/
 Author: solidlibs
 Maintainer: solidlibs
 License: GNU General Public License v3 (GPLv3)
 Download-URL: https://github.com/safeapps/solidlibs/
 Project-URL: Source Code, https://github.com/safeapps/solidlibs/
```

### Comparing `solidlibs-2.6.6/README.md` & `solidlibs-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/setup.py` & `solidlibs-2.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
     Set up for open source libraries.
 
     Copyright 2018-2023 solidlibs
-    Last modified: 2023-05-24
+    Last modified: 2023-05-29
 '''
 
 import os.path
 import setuptools
 
 # read long description
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="solidlibs",
-    version="2.6.6",
+    version="2.6.7",
     author="solidlibs",
     maintainer="solidlibs",
     description="Open source python and django enhancements",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="locks logs log-parser openssl",
     license="GNU General Public License v3 (GPLv3)",
```

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/context_processors/__init__.py` & `solidlibs-2.6.7/solidlibs/django_addons/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/context_processors/css_selector.py` & `solidlibs-2.6.7/solidlibs/django_addons/context_processors/css_selector.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/data_image.py` & `solidlibs-2.6.7/solidlibs/django_addons/data_image.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/middleware/debug.py` & `solidlibs-2.6.7/solidlibs/django_addons/middleware/debug.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/middleware/proxy404.py` & `solidlibs-2.6.7/solidlibs/django_addons/middleware/proxy404.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/middleware/redirect404.py` & `solidlibs-2.6.7/solidlibs/django_addons/middleware/redirect404.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/middleware/template.py` & `solidlibs-2.6.7/solidlibs/django_addons/middleware/template.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/singleton.py` & `solidlibs-2.6.7/solidlibs/django_addons/singleton.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/action_icons.1e02e82dbdcd.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/action_icons.1e02e82dbdcd.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/action_icons.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/action_icons.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/autocomplete.4a81fc4242d0.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/autocomplete.4a81fc4242d0.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/autocomplete.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/base.01580fff1759.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/base.01580fff1759.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/base.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/changelists.ae46354f4e80.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/changelists.ae46354f4e80.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/changelists.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/changelists.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dark_mode.4e3d1504ca81.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dark_mode.4e3d1504ca81.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/dark_mode.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/dark_mode.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/forms.c192d1ec6902.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/forms.c192d1ec6902.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/forms.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/forms.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/login.586129c60a93.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/login.586129c60a93.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/login.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/login.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/nav_sidebar.30423191f399.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/nav_sidebar.30423191f399.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/nav_sidebar.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/nav_sidebar.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/object_tools.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/object_tools.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/object_tools.ec5c6a50631e.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/object_tools.ec5c6a50631e.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive.02281633b5f1.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive.02281633b5f1.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive_rtl.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive_rtl.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/responsive_rtl.e13ae754cceb.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/responsive_rtl.e13ae754cceb.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/rtl.8473f45bd49b.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/rtl.8473f45bd49b.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/rtl.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/rtl.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.md` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/LICENSE-SELECT2.md`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.a2194c262648.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.a2194c262648.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.9f54e6414f87.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.9f54e6414f87.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/widgets.00318bc424d3.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/widgets.00318bc424d3.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/css/widgets.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/css/widgets.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/LICENSE.d273d63619c9.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/LICENSE.d273d63619c9.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/LICENSE.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.50d75e48e0a3.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.50d75e48e0a3.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.c73eb1ceba33.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.c73eb1ceba33.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.35b07eb2f871.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.35b07eb2f871.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.woff` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/fonts/Roboto-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/LICENSE` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/LICENSE`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/LICENSE.2c54f4e1ca1c` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/LICENSE.2c54f4e1ca1c`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/calendar-icons.39b290681a8b.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/calendar-icons.39b290681a8b.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/calendar-icons.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/calendar-icons.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_off.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.0047eba25b67.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.0047eba25b67.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/gis/move_vertex_on.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-calendar.ac7aea671bea.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-calendar.ac7aea671bea.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-calendar.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-calendar.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-clock.e1d4dfac3f2b.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-clock.e1d4dfac3f2b.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-clock.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-clock.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-no.439e821418cd.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-no.439e821418cd.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-no.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-no.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown-alt.81536e128bb6.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown-alt.81536e128bb6.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown-alt.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown-alt.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown.a18cb4398978.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown.a18cb4398978.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-unknown.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-unknown.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-viewlink.41eb31f7826e.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-viewlink.41eb31f7826e.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/icon-viewlink.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/icon-viewlink.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/inline-delete.fec1b761f254.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/inline-delete.fec1b761f254.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/inline-delete.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/inline-delete.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/selector-icons.b4555096cea2.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/selector-icons.b4555096cea2.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/selector-icons.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/selector-icons.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/sorting-icons.3a097b59f104.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/sorting-icons.3a097b59f104.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/img/sorting-icons.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/img/sorting-icons.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectBox.8161741c7647.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectBox.8161741c7647.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectBox.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectBox.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectFilter2.3f53e33c88d6.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectFilter2.3f53e33c88d6.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/SelectFilter2.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/SelectFilter2.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.eac7e3441574.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.eac7e3441574.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.min.5fa8cb0403f1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.min.5fa8cb0403f1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/actions.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/actions.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.300591891b2b.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.300591891b2b.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.de5309ac06dd.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.de5309ac06dd.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/autocomplete.01591ab27be7.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/autocomplete.01591ab27be7.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/autocomplete.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/calendar.f8a5d055eb33.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/calendar.f8a5d055eb33.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/calendar.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/cancel.ecc4c5ca7b32.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/cancel.ecc4c5ca7b32.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/cancel.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/cancel.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/change_form.9d8ca4f96b75.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/change_form.9d8ca4f96b75.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/change_form.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/change_form.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.f84e7410290f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.f84e7410290f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.min.2ee8a0086864.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.min.2ee8a0086864.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/collapse.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/collapse.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/core.5d6b384a08b5.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/core.5d6b384a08b5.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/core.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/core.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/filters.295a9d3d8b6a.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/filters.295a9d3d8b6a.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/filters.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/filters.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.22d4d93c00b4.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.22d4d93c00b4.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.min.4d23f8660b21.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.min.4d23f8660b21.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/inlines.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/inlines.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/nav_sidebar.36a64ecb39ed.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/nav_sidebar.36a64ecb39ed.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/nav_sidebar.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/nav_sidebar.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/popup_response.c6cc78ea5551.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/popup_response.c6cc78ea5551.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/popup_response.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/popup_response.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.bd2361dfd64d.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.bd2361dfd64d.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate_init.6cac7f3105b8.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate_init.6cac7f3105b8.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/prepopulate_init.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/prepopulate_init.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.2fb8e8349c22.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.2fb8e8349c22.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.min.5fa8cb0403f1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.min.5fa8cb0403f1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/stash/actions.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/stash/actions.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/timeparse.51258861a46a.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/timeparse.51258861a46a.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/timeparse.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/timeparse.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/urlify.25cc3eac8123.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/urlify.25cc3eac8123.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/urlify.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/urlify.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.2849239b95f5.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.2849239b95f5.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.8fb8fee4fcc3.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.8fb8fee4fcc3.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.f94142512c91.md` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.f94142512c91.md`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.md` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/af.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.270c257daf81.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.270c257daf81.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.91624382358e.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.91624382358e.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.a166b745933a.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.a166b745933a.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.766346afe4dd.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.766346afe4dd.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.8a1c222b0204.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.8a1c222b0204.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.27097f071856.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.27097f071856.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.cf932ba09a98.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.cf932ba09a98.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.2b96fd98289d.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.2b96fd98289d.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.70640d41628f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.70640d41628f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.04debded514d.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.04debded514d.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.170ae885d74f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.170ae885d74f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.2083264a54f0.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.2083264a54f0.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.c23089cb06ca.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.c23089cb06ca.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.23c7ce903300.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.23c7ce903300.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.08e62128eac1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.08e62128eac1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.dabbb9087130.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.dabbb9087130.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.da2fce143f27.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.da2fce143f27.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.997868a37ed8.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.997868a37ed8.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.6031b4f16452.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.6031b4f16452.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.131a78bc0752.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.131a78bc0752.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.f38c20b0221b.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.f38c20b0221b.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.c2afdeda3058.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.c2afdeda3058.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.txt` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.efda034b9537.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.efda034b9537.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/admin/js/vendor/xregexp/xregexp.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.468fca75a599.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.468fca75a599.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.db5f9ed61039.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.db5f9ed61039.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.3a434cc0b44e.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.3a434cc0b44e.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.57e1ce0c5850.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.57e1ce0c5850.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.921561dba489.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.921561dba489.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.602658511f99.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.602658511f99.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.677eb73b7cf8.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.677eb73b7cf8.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.88a457cfbc95.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.88a457cfbc95.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.668abc6a7653.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.668abc6a7653.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.4563f76d1380.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.4563f76d1380.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.3a855e8d68d8.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.3a855e8d68d8.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.2e863a645ac3.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.2e863a645ac3.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.9e7256cb17ff.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.9e7256cb17ff.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.f71cf6369adc.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.f71cf6369adc.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.451eff9b562a.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.451eff9b562a.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.4e47e3045b5c.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.4e47e3045b5c.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.ffede5391ab5.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.ffede5391ab5.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.a73716a97566.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.a73716a97566.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.874762f06dc0.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.874762f06dc0.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.e7faa89b97be.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.e7faa89b97be.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.155fd16d1aa1.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.155fd16d1aa1.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js.8cd46a572e05.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js.8cd46a572e05.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.808bdaf3f29c.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.808bdaf3f29c.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js.6a4eee3bf46c.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js.6a4eee3bf46c.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/bootstrap/js/popper.min.js.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/bootstrap/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/admin.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/admin.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/black-rock.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/black-rock.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/blackrock-digital.original.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/blackrock-digital.original.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/django_addons.bootstrap.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/django_addons.bootstrap.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/sudoSlider.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/sudoSlider.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/css/tufte-graph.css` & `solidlibs-2.6.7/solidlibs/django_addons/static/css/tufte-graph.css`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/Hamburger_icon.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/Hamburger_icon.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/Kebab_icon.svg` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/Kebab_icon.svg`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/comments.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/comments.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/delicious.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/delicious.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/digg.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/digg.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/facebook.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/facebook.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/flickr.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/flickr.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/linkedin.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/linkedin.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/rss.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/rss.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/stumbleupon.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/stumbleupon.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/technorati.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/technorati.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/images/social_media/twitter.png` & `solidlibs-2.6.7/solidlibs/django_addons/static/images/social_media/twitter.png`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery-3.6.0.min.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/jquery.min.map` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/jquery.min.map`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/popper.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/static/js/popper.min.js` & `solidlibs-2.6.7/solidlibs/django_addons/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/403.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/403.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/404.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/404.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/500.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/500.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/50x.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/50x.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/base_content.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/base_content.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/change_language.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/change_language.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/form_error_handling.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/form_error_handling.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/form_field_error_handling.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/form_field_error_handling.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/json2.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/json2.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/sign_in.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/sign_in.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/clips/user_tools.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/clips/user_tools.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templates/django_addons/csrf.html` & `solidlibs-2.6.7/solidlibs/django_addons/templates/django_addons/csrf.html`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templatetags/custom.py` & `solidlibs-2.6.7/solidlibs/django_addons/templatetags/custom.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templatetags/data_img.py` & `solidlibs-2.6.7/solidlibs/django_addons/templatetags/data_img.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templatetags/expr.py` & `solidlibs-2.6.7/solidlibs/django_addons/templatetags/expr.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templatetags/lookup.py` & `solidlibs-2.6.7/solidlibs/django_addons/templatetags/lookup.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/templatetags/var.py` & `solidlibs-2.6.7/solidlibs/django_addons/templatetags/var.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/utils.py` & `solidlibs-2.6.7/solidlibs/django_addons/utils.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/django_addons/views.py` & `solidlibs-2.6.7/solidlibs/django_addons/views.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/browser.py` & `solidlibs-2.6.7/solidlibs/net/browser.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/html_addons.py` & `solidlibs-2.6.7/solidlibs/net/html_addons.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/http_addons.py` & `solidlibs-2.6.7/solidlibs/net/http_addons.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/mime_constants.py` & `solidlibs-2.6.7/solidlibs/net/mime_constants.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/openssl.py` & `solidlibs-2.6.7/solidlibs/net/openssl.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/utils.py` & `solidlibs-2.6.7/solidlibs/net/utils.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/net/web_log_parser.py` & `solidlibs-2.6.7/solidlibs/net/web_log_parser.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/cli.py` & `solidlibs-2.6.7/solidlibs/os/cli.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/command.py` & `solidlibs-2.6.7/solidlibs/os/command.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/drive.py` & `solidlibs-2.6.7/solidlibs/os/drive.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/fs.py` & `solidlibs-2.6.7/solidlibs/os/fs.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/lock.py` & `solidlibs-2.6.7/solidlibs/os/lock.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/osid.py` & `solidlibs-2.6.7/solidlibs/os/osid.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/process.py` & `solidlibs-2.6.7/solidlibs/os/process.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/profile_addons.py` & `solidlibs-2.6.7/solidlibs/os/profile_addons.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/os/user.py` & `solidlibs-2.6.7/solidlibs/os/user.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/_log.py` & `solidlibs-2.6.7/solidlibs/python/_log.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/abstract_build_venv.py` & `solidlibs-2.6.7/solidlibs/python/abstract_build_venv.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/dict.py` & `solidlibs-2.6.7/solidlibs/python/dict.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/elapsed_time.py` & `solidlibs-2.6.7/solidlibs/python/elapsed_time.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/format.py` & `solidlibs-2.6.7/solidlibs/python/format.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/internals.py` & `solidlibs-2.6.7/solidlibs/python/internals.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/iter.py` & `solidlibs-2.6.7/solidlibs/python/iter.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/log.py` & `solidlibs-2.6.7/solidlibs/python/log.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/performance.py` & `solidlibs-2.6.7/solidlibs/python/performance.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/text_file.py` & `solidlibs-2.6.7/solidlibs/python/text_file.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/times.py` & `solidlibs-2.6.7/solidlibs/python/times.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/utils.py` & `solidlibs-2.6.7/solidlibs/python/utils.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs/python/ve.py` & `solidlibs-2.6.7/solidlibs/python/ve.py`

 * *Files identical despite different names*

### Comparing `solidlibs-2.6.6/solidlibs.egg-info/PKG-INFO` & `solidlibs-2.6.7/solidlibs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidlibs
-Version: 2.6.6
+Version: 2.6.7
 Summary: Open source python and django enhancements
 Home-page: https://github.com/safeapps/solidlibs/
 Author: solidlibs
 Maintainer: solidlibs
 License: GNU General Public License v3 (GPLv3)
 Download-URL: https://github.com/safeapps/solidlibs/
 Project-URL: Source Code, https://github.com/safeapps/solidlibs/
```

### Comparing `solidlibs-2.6.6/solidlibs.egg-info/SOURCES.txt` & `solidlibs-2.6.7/solidlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


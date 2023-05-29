# Comparing `tmp/gitbuilding-0.9.0.tar.gz` & `tmp/gitbuilding-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitbuilding-0.9.0.tar", last modified: Thu Jul  8 15:22:57 2021, max compression
+gzip compressed data, was "dist/gitbuilding-0.9.1.tar", last modified: Fri Oct 29 11:58:14 2021, max compression
```

## Comparing `gitbuilding-0.9.0.tar` & `gitbuilding-0.9.1.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3656 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2461 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/README.md
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/__init__.py
--rwxrwxr-x   0 js3214    (1000) js3214    (1000)     9549 2021-07-06 14:59:44.000000 gitbuilding-0.9.0/gitbuilding/__main__.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/buildup/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      602 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/buildup/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    12108 2021-05-25 12:52:24.000000 gitbuilding-0.9.0/gitbuilding/buildup/basepart.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    16709 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/buildup.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4955 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/config.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    17934 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/core.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7718 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/buildup/files.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4751 2021-05-25 12:52:24.000000 gitbuilding-0.9.0/gitbuilding/buildup/libraries.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    26237 2021-05-25 12:56:38.000000 gitbuilding-0.9.0/gitbuilding/buildup/link.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    22622 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/page.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9534 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/pageorder.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     6334 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/buildup/partlist.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    11629 2021-05-25 14:34:28.000000 gitbuilding-0.9.0/gitbuilding/buildup/parts.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2753 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/buildup/preview.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    16324 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/buildup/quantity.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    14094 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/buildup/unit.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5082 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/buildup/url.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2246 2021-05-25 12:52:24.000000 gitbuilding-0.9.0/gitbuilding/buildup/utilities.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4310 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/config.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7300 2021-07-06 15:07:42.000000 gitbuilding-0.9.0/gitbuilding/example.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3289 2021-07-06 13:28:56.000000 gitbuilding-0.9.0/gitbuilding/generate_ci.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2765 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/handler.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/licenses/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    34520 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/AGPL-3.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    11357 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/Apache-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1317 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/BSD-2-Clause.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1512 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/BSD-3-Clause.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    19467 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-3.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    18657 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-4.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    22240 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-SA-3.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    20138 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-SA-4.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     8108 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-1.1.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9153 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-1.2.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     8240 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-P-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    12340 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-S-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    13335 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-W-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    11514 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/EPL-1.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    18046 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/GPL-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    35141 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/GPL-3.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    26461 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/LGPL-2.1.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7651 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/LGPL-3.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1069 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/MIT.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    16725 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/MPL-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    11534 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/SHL-0.5.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    11526 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/SHL-0.51.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2777 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/SHL-2.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    13940 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/TAPR-OHL-1.0.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1211 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/gitbuilding/licenses/Unlicense.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5011 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/native_file_operations.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    12381 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/output.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3980 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/previewers.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    18421 2021-05-25 14:32:03.000000 gitbuilding-0.9.0/gitbuilding/render.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    28567 2021-07-06 15:07:42.000000 gitbuilding-0.9.0/gitbuilding/server.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)  1748967 2021-07-08 15:22:42.000000 gitbuilding-0.9.0/gitbuilding/static/3d-viewer.js
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1595 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding.pdf
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5526 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding.svg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    24223 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding500x.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1233 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/favicon-16x16.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1828 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/favicon-32x32.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    13094 2019-06-18 15:37:09.000000 gitbuilding-0.9.0/gitbuilding/static/Logo/favicon.ico
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/css/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2284 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/css/app.2bbbc00f.css
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4286 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/favicon.ico
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      988 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/index.html
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/js/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     8520 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/js/app.da0d2df1.js
--rw-rw-r--   0 js3214    (1000) js3214    (1000)    33617 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/js/app.da0d2df1.js.map
--rw-rw-r--   0 js3214    (1000) js3214    (1000)   200082 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js
--rw-rw-r--   0 js3214    (1000) js3214    (1000)   808379 2021-07-08 15:22:56.000000 gitbuilding-0.9.0/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js.map
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7832 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/DuplicatePage.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9102 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/DuplicatePage.svg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4487 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/EmptyPage.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2756 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/EmptyPage.svg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)   215341 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/Missing_image.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9598 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/Missing_image.svg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5432 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/StepByStepPage.png
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     6790 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/static/local-server/StepByStepPage.svg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4884 2021-05-25 14:34:28.000000 gitbuilding-0.9.0/gitbuilding/static/style.css
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding/templates/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2172 2021-05-25 14:34:28.000000 gitbuilding-0.9.0/gitbuilding/templates/body.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      596 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/templates/contents.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      246 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/templates/favicon.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      550 2021-07-06 13:28:56.000000 gitbuilding-0.9.0/gitbuilding/templates/footer.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      569 2021-05-25 14:56:27.000000 gitbuilding-0.9.0/gitbuilding/templates/full_page.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1171 2021-07-06 13:28:56.000000 gitbuilding-0.9.0/gitbuilding/templates/full_pdf.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      321 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/templates/gallery.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      376 2021-05-25 14:34:28.000000 gitbuilding-0.9.0/gitbuilding/templates/header.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      110 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/templates/iframe.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      634 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/templates/nav.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      791 2021-07-06 13:28:56.000000 gitbuilding-0.9.0/gitbuilding/templates/new1.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      513 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/templates/new2.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      131 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/gitbuilding/templates/pdfpage.html.jinja
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2881 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/gitbuilding/utilities.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3656 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4031 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/SOURCES.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/dependency_links.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       59 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/entry_points.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2020-05-03 13:03:50.000000 gitbuilding-0.9.0/gitbuilding.egg-info/not-zip-safe
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      145 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/requires.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       18 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/gitbuilding.egg-info/top_level.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1148 2021-07-06 13:28:56.000000 gitbuilding-0.9.0/pyproject.toml
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/setup.cfg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2821 2021-07-08 15:22:21.000000 gitbuilding-0.9.0/setup.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/tests/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1368 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/tests/checklogs.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      224 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/test.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1782 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/test_handler.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5726 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/tests/test_main.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2751 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/test_utilities.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-07-08 15:22:57.000000 gitbuilding-0.9.0/tests/tests_buildup/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/tests_buildup/__init__.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     9527 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/tests/tests_buildup/test_buildup.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1401 2020-10-04 14:21:02.000000 gitbuilding-0.9.0/tests/tests_buildup/test_config.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3155 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/tests/tests_buildup/test_files.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1998 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/tests/tests_buildup/test_part.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     3152 2021-05-25 12:52:24.000000 gitbuilding-0.9.0/tests/tests_buildup/test_partlist.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7219 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/tests/tests_buildup/test_quantity.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     5232 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/tests/tests_buildup/test_unit.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1074 2020-10-04 14:22:35.000000 gitbuilding-0.9.0/tests/tests_buildup/test_url.py
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      744 2021-05-25 12:50:23.000000 gitbuilding-0.9.0/tests/tests_buildup/test_utilities.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    35147 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/LICENSE
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3676 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2461 2021-05-25 14:32:03.000000 gitbuilding-0.9.1/README.md
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/__init__.py
+-rwxrwxr-x   0 js3214    (1000) js3214    (1000)     9549 2021-07-06 14:59:44.000000 gitbuilding-0.9.1/gitbuilding/__main__.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/buildup/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      602 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/buildup/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    12108 2021-05-25 12:52:24.000000 gitbuilding-0.9.1/gitbuilding/buildup/basepart.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    16709 2021-05-25 14:32:03.000000 gitbuilding-0.9.1/gitbuilding/buildup/buildup.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4955 2021-05-25 14:32:03.000000 gitbuilding-0.9.1/gitbuilding/buildup/config.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    18207 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/buildup/core.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     8132 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/buildup/files.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4751 2021-05-25 12:52:24.000000 gitbuilding-0.9.1/gitbuilding/buildup/libraries.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    26440 2021-09-16 10:15:00.000000 gitbuilding-0.9.1/gitbuilding/buildup/link.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    23169 2021-10-29 09:28:59.000000 gitbuilding-0.9.1/gitbuilding/buildup/page.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    10345 2021-09-16 10:15:00.000000 gitbuilding-0.9.1/gitbuilding/buildup/pageorder.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     6334 2021-05-25 14:32:03.000000 gitbuilding-0.9.1/gitbuilding/buildup/partlist.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    11629 2021-05-25 14:34:28.000000 gitbuilding-0.9.1/gitbuilding/buildup/parts.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2909 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/buildup/preview.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    16324 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/buildup/quantity.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    14091 2021-10-29 11:22:43.000000 gitbuilding-0.9.1/gitbuilding/buildup/unit.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5082 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/buildup/url.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2745 2021-09-16 10:15:00.000000 gitbuilding-0.9.1/gitbuilding/buildup/utilities.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4310 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/config.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     7300 2021-07-06 15:07:42.000000 gitbuilding-0.9.1/gitbuilding/example.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3289 2021-07-06 13:28:56.000000 gitbuilding-0.9.1/gitbuilding/generate_ci.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2765 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/handler.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/licenses/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    34520 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/AGPL-3.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    11357 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/Apache-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1317 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/BSD-2-Clause.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1512 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/BSD-3-Clause.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    19467 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-3.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    18657 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-4.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    22240 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-SA-3.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    20138 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-SA-4.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     8108 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-1.1.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9153 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-1.2.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     8240 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-P-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    12340 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-S-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    13335 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-W-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    11514 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/EPL-1.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    18046 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/GPL-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    35141 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/GPL-3.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    26461 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/LGPL-2.1.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     7651 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/LGPL-3.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1069 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/MIT.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    16725 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/MPL-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    11534 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/SHL-0.5.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    11526 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/SHL-0.51.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2777 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/SHL-2.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    13940 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/TAPR-OHL-1.0.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1211 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/gitbuilding/licenses/Unlicense.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5011 2021-08-17 14:23:28.000000 gitbuilding-0.9.1/gitbuilding/native_file_operations.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    12530 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/output.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4161 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/previewers.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    18554 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/render.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    28640 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/server.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)  1748967 2021-10-29 11:57:57.000000 gitbuilding-0.9.1/gitbuilding/static/3d-viewer.js
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1595 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding.pdf
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5526 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding.svg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    24223 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding500x.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1233 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/favicon-16x16.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1828 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/favicon-32x32.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    13094 2019-06-18 15:37:09.000000 gitbuilding-0.9.1/gitbuilding/static/Logo/favicon.ico
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/css/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2284 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/css/app.2bbbc00f.css
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4286 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/favicon.ico
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      988 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/index.html
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/js/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     8520 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/js/app.da0d2df1.js
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    33617 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/js/app.da0d2df1.js.map
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)   200082 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)   808379 2021-10-29 11:58:12.000000 gitbuilding-0.9.1/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js.map
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     7832 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/DuplicatePage.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9102 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/DuplicatePage.svg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4487 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/EmptyPage.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2756 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/EmptyPage.svg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)   215341 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/Missing_image.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9598 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/Missing_image.svg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5432 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/StepByStepPage.png
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     6790 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/static/local-server/StepByStepPage.svg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4884 2021-05-25 14:34:28.000000 gitbuilding-0.9.1/gitbuilding/static/style.css
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding/templates/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2172 2021-05-25 14:34:28.000000 gitbuilding-0.9.1/gitbuilding/templates/body.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      596 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/templates/contents.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      246 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/templates/favicon.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      550 2021-07-06 13:28:56.000000 gitbuilding-0.9.1/gitbuilding/templates/footer.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      627 2021-10-29 09:28:40.000000 gitbuilding-0.9.1/gitbuilding/templates/full_page.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1171 2021-07-06 13:28:56.000000 gitbuilding-0.9.1/gitbuilding/templates/full_pdf.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      321 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/templates/gallery.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      376 2021-05-25 14:34:28.000000 gitbuilding-0.9.1/gitbuilding/templates/header.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      110 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/templates/iframe.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      634 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/templates/nav.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      791 2021-07-06 13:28:56.000000 gitbuilding-0.9.1/gitbuilding/templates/new1.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      513 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/templates/new2.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      131 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/gitbuilding/templates/pdfpage.html.jinja
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2881 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/gitbuilding/utilities.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding.egg-info/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3676 2021-10-29 11:58:13.000000 gitbuilding-0.9.1/gitbuilding.egg-info/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     4039 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/gitbuilding.egg-info/SOURCES.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2021-10-29 11:58:13.000000 gitbuilding-0.9.1/gitbuilding.egg-info/dependency_links.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       59 2021-10-29 11:58:13.000000 gitbuilding-0.9.1/gitbuilding.egg-info/entry_points.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2020-05-03 13:03:50.000000 gitbuilding-0.9.1/gitbuilding.egg-info/not-zip-safe
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      201 2021-10-29 11:58:13.000000 gitbuilding-0.9.1/gitbuilding.egg-info/requires.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       18 2021-10-29 11:58:13.000000 gitbuilding-0.9.1/gitbuilding.egg-info/top_level.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1148 2021-07-06 13:28:56.000000 gitbuilding-0.9.1/pyproject.toml
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/setup.cfg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3094 2021-10-29 11:22:43.000000 gitbuilding-0.9.1/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/tests/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1368 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/tests/checklogs.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      224 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/test.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1782 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/test_handler.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5726 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/tests/test_main.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2751 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/test_utilities.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2021-10-29 11:58:14.000000 gitbuilding-0.9.1/tests/tests_buildup/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/tests_buildup/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     9527 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/tests/tests_buildup/test_buildup.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1401 2020-10-04 14:21:02.000000 gitbuilding-0.9.1/tests/tests_buildup/test_config.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3155 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/tests/tests_buildup/test_files.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1998 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/tests/tests_buildup/test_part.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3152 2021-05-25 12:52:24.000000 gitbuilding-0.9.1/tests/tests_buildup/test_partlist.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     7219 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/tests/tests_buildup/test_quantity.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5232 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/tests/tests_buildup/test_unit.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1074 2020-10-04 14:22:35.000000 gitbuilding-0.9.1/tests/tests_buildup/test_url.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      744 2021-05-25 12:50:23.000000 gitbuilding-0.9.1/tests/tests_buildup/test_utilities.py
```

### Comparing `gitbuilding-0.9.0/PKG-INFO` & `gitbuilding-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbuilding
-Version: 0.9.0
+Version: 0.9.1
 Summary: For documenting hardware projects with minimal effort,so you can stop writing and GitBuilding.
 Home-page: https://gitbuilding.io/
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/gitbuilding/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/gitbuilding
@@ -70,7 +70,8 @@
 Keywords: Documentation,Hardware
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `gitbuilding-0.9.0/README.md` & `gitbuilding-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/__main__.py` & `gitbuilding-0.9.1/gitbuilding/__main__.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/__init__.py` & `gitbuilding-0.9.1/gitbuilding/buildup/__init__.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/basepart.py` & `gitbuilding-0.9.1/gitbuilding/buildup/basepart.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/buildup.py` & `gitbuilding-0.9.1/gitbuilding/buildup/buildup.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/config.py` & `gitbuilding-0.9.1/gitbuilding/buildup/config.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/core.py` & `gitbuilding-0.9.1/gitbuilding/buildup/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,25 +285,24 @@
                                               duplicate_of)
 
         self._append_page_for_duplicates(all_output_files)
 
         return all_output_files
 
     def _append_page_for_duplicates(self, all_output_files):
-        list_roots = [plist[0] for plist in self._page_order.pagelists]
         for duplicate in self._page_order.duplicates:
             page = self.get_page_by_path(duplicate)
             links = []
-            # duplicates is a dictionary each page that is duplicated is a key,
-            # the value is the list of the root of each documentation path that contains
-            # the page
+            # Duplicates is a dictionary.
+            # Each page that is duplicated is a key who's value is the list of the root of
+            # each documentation path that contains the page
             for root_pagename in self._page_order.duplicates[duplicate]:
                 #For each copy find the output path, and the title of the root page.
                 root_page = self.get_page_by_path(root_pagename)
-                list_no = list_roots.index(root_pagename)
+                list_no = self._page_order.get_list_number(root_pagename)
                 replace_links = self._page_order.link_replacement_dictionaries[list_no]
                 url_translator = self.url_rules.create_translator(duplicate,
                                                                   replace_links=replace_links)
                 translated_target = url_translator.simple_translate(duplicate)
                 links.append((root_page.title, translated_target))
             content = ("# There are multiple versions of this page.\n\nPlease select one "
                        "of these projects:\n\n")
@@ -322,44 +321,49 @@
                                  duplicate_of=None):
 
         page_content = page.generate_output(nav_pagelist, overloaded_path, replace_links)
         outpath = overloaded_path if overloaded_path is not None else page.filepath
         file_obj = FileInfo(outpath,
                             dynamic_content=True,
                             content=page_content,
+                            meta_info=page.meta_info,
                             duplicate_of=duplicate_of)
         all_output_files.append(file_obj)
         if page.get_bom_page(as_filelist=True) is not None:
             all_output_files += page.get_bom_page(as_filelist=True)
         for link in page.all_links_and_images:
             linked_file = None
             if link.content_generated:
                 if isinstance(link, LibraryLink):
                     linked_file = self._libs.part_page(*link.library_location)
                 else:
-                    if link.link_rel_to_root not in self._filelist:
-                        _LOGGER.warning("Linked markdown page does not exist: %s", link.link_rel_to_root)
+                    link_path = utilities.strip_internal_links(link.link_rel_to_root)
+                    if link_path not in (self._filelist + self._page_order.filenames_of_duplicates):
+                        _LOGGER.warning("Linked markdown page does not exist: %s", link_path)
             else:
                 linked_file = link.as_output_file()
             if linked_file is not None:
                 if linked_file not in all_output_files:
-                    if not( linked_file.dynamic_content or linked_file in self._filelist):
+                    if not(linked_file.dynamic_content or linked_file in self._filelist):
                         _LOGGER.warning("Linked file does not exist: %s", linked_file.path)
                     # append even if missing to avoid duplicate warnings
                     all_output_files.append(linked_file)
 
     def _append_preview_pages(self, all_output_files):
         for output_file in all_output_files:
             output_path = output_file.path
             if self.previewer_for_uri(output_path) is not None:
                 previewer = self.previewer_for_uri(output_path)
                 if previewer.create_preview_page:
                     prev_path = previewer.preview_page_uri(output_path)
                     md = previewer.preview_page_content(output_path)
-                    file_obj = FileInfo(prev_path, dynamic_content=True, content=md)
+                    file_obj = FileInfo(prev_path,
+                                        dynamic_content=True,
+                                        content=md,
+                                        meta_info={'previewers_used': previewer.name})
                     all_output_files.append(file_obj)
 
     def buildall(self, filelist):
         """
         Builds the output documentation as a list of FileInfo objects based on the input
         documentation directory defined by `filelist` (also a list of FileInfo objects)
         """
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/files.py` & `gitbuilding-0.9.1/gitbuilding/buildup/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,22 +111,29 @@
     """
 
     def __init__(self,
                  path,
                  location_on_disk=None,
                  dynamic_content: bool = False,
                  content=None,
+                 meta_info=None,
                  duplicate_of=None):
 
         self._path = as_posix(path)
         if posixpath.isabs(self._path):
             raise RuntimeError('FileInfo objects cannot specify paths outside the build'
                                f' directory. Requested path is "{self._path}"')
 
         self._dynamic_content = bool(dynamic_content)
+        if isinstance(meta_info, dict):
+            self._meta_info = meta_info
+        elif meta_info is None:
+            self._meta_info = {}
+        else:
+            raise TypeError('meta_info for a file should be a dictionary')
 
         if self._dynamic_content:
             self._location_on_disk = None
             self._duplicate_of = duplicate_of
             if content is None:
                 raise RuntimeError('Buildup file must have a content string')
             self._content = str(content)
@@ -197,14 +204,21 @@
     @property
     def content(self):
         '''
         Returns the content of the file (this is only valid if `dynamic_content` is True)
         '''
         return self._content
 
+    @property
+    def meta_info(self):
+        '''
+        Returns any meta information about the file
+        '''
+        return self._meta_info
+
     def as_dict(self):
         '''
         Serialise the file object as a dictionary
         '''
         output = {'path': self.path,
                   'dynamic_content': self._dynamic_content}
         if self.dynamic_content:
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/libraries.py` & `gitbuilding-0.9.1/gitbuilding/buildup/libraries.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/link.py` & `gitbuilding-0.9.1/gitbuilding/buildup/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 import posixpath
 import logging
 from dataclasses import dataclass
 import regex as re
 from marshmallow import Schema, fields, post_load, pre_load, ValidationError
 from gitbuilding.buildup.files import FileInfo
 from gitbuilding.buildup.quantity import Quantity
-from gitbuilding.buildup.utilities import clean_id, as_posix, raise_validation_error_as_warning
+from gitbuilding.buildup.utilities import (clean_id,
+                                           as_posix,
+                                           raise_validation_error_as_warning,
+                                           strip_internal_links)
 
 _LOGGER = logging.getLogger('BuildUp')
 
 @dataclass
 class LinkData:
     """
     A simple data class for the BuildUp data stored with a link
@@ -472,15 +475,16 @@
         return self.buildup_data.previewpage
 
     @property
     def content_generated(self):
         """Returns true if the content is generated in build up and otherwise
         return false"""
         #Note the link_rel_to_page has converted library links into .md links
-        if self.link_rel_to_page_no_preview.endswith('.md'):
+        rel_link = strip_internal_links(self.link_rel_to_page_no_preview)
+        if rel_link.endswith('.md'):
             return True
         if self.raw_linklocation.startswith('{{'):
             return True
         return False
 
     def as_output_file(self):
         """ Returns the link as an FileInfo object.
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/page.py` & `gitbuilding-0.9.1/gitbuilding/buildup/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from copy import copy, deepcopy
 
 from gitbuilding.buildup.link import FromStepLink
 from gitbuilding.buildup.parts import UsedPart
 from gitbuilding.buildup.partlist import PartList
 from gitbuilding.buildup.buildup import BuildUpParser
 from gitbuilding.buildup.files import FileInfo
-import gitbuilding.buildup.utilities as utilities
+from gitbuilding.buildup import utilities
 
 _LOGGER = logging.getLogger('BuildUp')
 
 def notify_logger(wrapped_func):
     """
     Notifies the logger of the page being processed
     """
@@ -37,14 +37,15 @@
     AS_CSV = 1
 
     def __init__(self, file_obj, doc):
         self._file_obj = deepcopy(file_obj)
         self._doc = doc
         self._overloaded_path = None
         self._replace_links = None
+        self._meta_info = {}
 
         self._part_list = PartList(self._doc.config)
         self._all_parts = None
         self._bom_pages = None
 
         self._step_tree = None
         self._set_parser(self.get_raw())
@@ -111,14 +112,21 @@
     def filename(self):
         '''
         The filename of the input page and output pages
         '''
         return posixpath.basename(self.filepath)
 
     @property
+    def meta_info(self):
+        '''
+        Return a dictionary of any meta information for the page.
+        '''
+        return self._meta_info
+
+    @property
     def counted(self):
         '''
         Sets whether the main part list has been counted (this happens after running
         count_page)
         '''
         return self._all_parts is not None
 
@@ -245,14 +253,15 @@
           live edited text and a different URL.
         """
 
         self._part_list = PartList(self._doc.config)
         self._all_parts = None
         self._step_tree = None
         self._bom_pages = None
+        self._meta_info = {}
 
         self._set_parser(md)
 
         self.get_step_tree()
         self.count()
 
         if self._doc.page_order.number_of_paths == 0:
@@ -426,14 +435,19 @@
         the only processing here is the url translation rules
         """
         for image in self._parser.images:
             previewer =  self._doc.previewer_for_uri(image.image_rel_to_root)
             if previewer is None:
                 rep_text = image.image_md(self._url_translator)
             else:
+                if 'previewers_used' in self._meta_info:
+                    if previewer.name not in self._meta_info['previewers_used']:
+                        self._meta_info['previewers_used'].append(previewer.name)
+                else:
+                    self._meta_info['previewers_used'] = [previewer.name]
                 location = image.output_url(self._url_translator)
                 rep_text = previewer.display_code(location, image.alttext, image.hovertext)
             processed_text = processed_text.replace(image.fullmatch, rep_text)
         return processed_text
 
     def _replace_part_links(self, processed_text):
         """
@@ -578,15 +592,15 @@
         Makes separate Bill of materials page for the all parts on this page (including those
         in steps). Returns the filepath of the resulting file and the markdown in a dictionary
         """
 
         md_path = self._bom_url()
         csv_path = self._bom_url(self.AS_CSV)
 
-        bom_intro = f"Download this as a [CSV file]({csv_path})"
+        bom_intro = f"Download this as a [CSV file]({posixpath.basename(csv_path)})"
         # Fine to use self._url_translator as the BOM page will be in same
         # output directory
         md = self._all_parts.bom_md("# Bill of Materials", self._part_url_translator, intro=bom_intro)
         if not self._doc.config.remove_bottom_nav:
             md = self._add_bottom_navigation(md, nav_pagelist, overload_path=md_path)
         csv = self._all_parts.bom_csv(self._doc)
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/pageorder.py` & `gitbuilding-0.9.1/gitbuilding/buildup/pageorder.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,24 @@
         Read-only property which returns a dictionary. The keys are the pagenames of any pages
         that are used in more than one path through the documentation, the value is a list of
         the pagenames of the roots of those paths.
         """
         return deepcopy(self._duplicates)
 
     @property
+    def filenames_of_duplicates(self):
+        filenames = []
+        for duplicate in self.duplicates:
+            for root_pagename in self.duplicates[duplicate]:
+                list_no = self.get_list_number(root_pagename)
+                replacement_dict = self.link_replacement_dictionaries[list_no]
+                filenames.append(replacement_dict[duplicate])
+        return filenames
+
+    @property
     def pagelists(self):
         """
         Read-only property which returns a copy of the pagelists. One list for each path through
         the documentation. The items in each list are just the page_names.
         """
         pagelists = []
         for pagelist in self._tuple_pagelists:
@@ -126,14 +136,25 @@
                     if bom_pages is not None:
                         for bom_page in bom_pages:
                             in_paths.append(bom_page)
                             out_paths.append(posixpath.join(subdir, bom_page))
             out_lists.append(dict(zip(in_paths, out_paths)))
         return out_lists
 
+    def get_list_number(self, root_pagename):
+        """
+        Return the number (index) of the pagelist with the input page name as root. If the input
+        page is not a root of any pagelist then reutn None.
+        """
+        list_roots = [plist[0] for plist in self.pagelists]
+        try:
+            return list_roots.index(root_pagename)
+        except ValueError:
+            return None
+
     def _validate_pagelists(self, landing_page):
         """
         Checks the page order doesn't have unexpected problems like repeated steps. The
         landing page doesn't need to be in the page order list, but if it is in it must
         be at the start.
         The function does not return anything, it just logs any issues
         """
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/partlist.py` & `gitbuilding-0.9.1/gitbuilding/buildup/partlist.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/parts.py` & `gitbuilding-0.9.1/gitbuilding/buildup/parts.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/preview.py` & `gitbuilding-0.9.1/gitbuilding/buildup/preview.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class Previewer():
     """
     Base class for previewers this should be sub-classed
     for use.
     """
 
     def __init__(self, enabled):
+        self._name = "Unknown_previewer"
         self._enabled = enabled
         self._drop_dir = "misc"
         self._create_preview_page_when_enabled = False
 
     @property
     def pattern(self):
         """
@@ -55,14 +56,21 @@
         This returns the markdown to replace the image syntax with if the previewing is
         not enabled. This will just be a link to the URI
         """
         # pylint: disable=no-self-use
         return f'[{alt_text}]({uri} "{hover_text}")'
 
     @property
+    def name(self):
+        """
+        Name of the previewer
+        """
+        return self._name
+
+    @property
     def dir_for_dropped_files(self):
         """
         Directory where dropped files of this type are saved
         """
         return self._drop_dir
 
     @property
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/quantity.py` & `gitbuilding-0.9.1/gitbuilding/buildup/quantity.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/unit.py` & `gitbuilding-0.9.1/gitbuilding/buildup/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         self.all_groups = []
         self._init_mass()
         self._init_lengths()
         self._init_areas()
         self._init_volumes()
 
     def _init_mass(self):
-        microgramme = Unit([u'μg', 'ug'],
+        microgramme = Unit(['μg', 'ug'],
                            ['microgramme', 'microgram', 'microgrammes', 'micrograms'])
         milligramme = Unit(['mg'],
                            ['milligramme', 'milligram', 'milligrammes', 'milligrams'])
         gramme = Unit(['g'],
                       ['gramme', 'gram', 'grammes', 'grams'])
         kilogramme = Unit(['kg'],
                           ['kilogramme', 'kilogram', 'kilorammes', 'kilograms'])
@@ -256,15 +256,15 @@
 
         sq_centimetre = Unit(['cm^2'],
                              ['centimetre^2', 'centimeter^2', 'centimetres^2', 'centimeters^2'])
         secondary_metric_areas = UnitGroup(sq_centimetre, [], metric_areas, 1e-4)
         self.all_groups.append(secondary_metric_areas)
 
     def _init_volumes(self):
-        microlitre = Unit([u'μL', u'μl', 'uL', 'ul'],
+        microlitre = Unit(['μL', 'μl', 'uL', 'ul'],
                           ['microlitre', 'microliter', 'microlitres', 'microliters'])
         millilitre = Unit(['mL', 'ml'],
                           ['millilitre', 'milliliter', 'millilitres', 'milliliters'])
         litre = Unit(['L', 'l'],
                      ['litre', 'liter', 'litres', 'liters'])
         litre_scales = [(millilitre, 0.001),
                         (microlitre, 1e-6)]
```

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/url.py` & `gitbuilding-0.9.1/gitbuilding/buildup/url.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/buildup/utilities.py` & `gitbuilding-0.9.1/gitbuilding/buildup/utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,28 +10,42 @@
 
 import regex as re
 
 _LOGGER = logging.getLogger('BuildUp')
 
 def as_posix(path, warn=False):
     """
-    Returns the input path as a posix path
+    Returns the input path as a posix path.
+
+    By posix path we mean something that will work with python "posixpath" library.
+    This includes URLs with internal links. This is done so that all file paths within
+    buildup are the same on any OS to reduce the number of file path bugs when changing
+    systems.
     """
 
     if path == "":
         return path
     if warn:
         pos_path = as_posix(path)
         if path not in [pos_path, './'+pos_path]:
             _LOGGER.warning('"%s" is not a normalised posixpath. This may cause '
                             'unexpected results. Using "%s"',
                             path, pos_path)
         return pos_path
     return posixpath.normpath(PureWindowsPath(path).as_posix())
 
+def strip_internal_links(path):
+    """
+    Remove internal links from a path. i.e. Links ending with #ID
+    For example:
+    Input: page/subpage.md#section
+    Output: page/subpage.md
+    """
+    return path.split('#')[0]
+
 def clean_id(id_in):
     """
     Input a string and output is a string that can be used an an ID in HTML
     """
     id_out = id_in.replace(' ', '-')
     id_out = id_out.lower()
     return re.sub(r'[^a-z0-9\_\-]', '', id_out)
```

### Comparing `gitbuilding-0.9.0/gitbuilding/config.py` & `gitbuilding-0.9.1/gitbuilding/config.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/example.py` & `gitbuilding-0.9.1/gitbuilding/example.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/generate_ci.py` & `gitbuilding-0.9.1/gitbuilding/generate_ci.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/handler.py` & `gitbuilding-0.9.1/gitbuilding/handler.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/AGPL-3.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/AGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/Apache-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/BSD-2-Clause.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/BSD-3-Clause.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-3.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-3.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-4.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-SA-3.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CC-BY-SA-4.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-1.1.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-1.1.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-1.2.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-1.2.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-P-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-P-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-S-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-S-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/CERN-OHL-W-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/CERN-OHL-W-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/EPL-1.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/GPL-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/GPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/GPL-3.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/GPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/LGPL-2.1.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/LGPL-2.1.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/LGPL-3.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/MIT.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/MPL-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/SHL-0.5.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/SHL-0.5.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/SHL-0.51.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/SHL-0.51.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/SHL-2.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/SHL-2.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/TAPR-OHL-1.0.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/TAPR-OHL-1.0.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/licenses/Unlicense.txt` & `gitbuilding-0.9.1/gitbuilding/licenses/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/native_file_operations.py` & `gitbuilding-0.9.1/gitbuilding/native_file_operations.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/output.py` & `gitbuilding-0.9.1/gitbuilding/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,19 +181,20 @@
         if outfile.path.endswith('.md'):
             self._markdown_content(outfile, full_out_path)
         else:
             write_local_file(full_out_path, outfile.content)
 
     def _markdown_content(self, outfile, full_out_path):
         if outfile.path == self.doc.config.landing_page:
-            full_out_path = self._out_dir+ "/index.html"
+            full_out_path = self._out_dir + "/index.html"
         else:
             full_out_path = posixpath.splitext(full_out_path)[0]+'.html'
         page_html = self._renderer.render_md(outfile.content,
                                              posixpath.splitext(outfile.path)[0]+'.html',
+                                             meta_info=outfile.meta_info,
                                              editorbutton=False)
         write_local_file(full_out_path, page_html)
 
     def _copy_static_files(self):
         """
         Copies all the static web files that come as default with gitbuilding.
         This includes the CSS, the favicons, and the 3D viewer
@@ -299,14 +300,15 @@
         HTML(html_path).write_pdf(as_native_path('_pdf/' + filename))
 
     def _build_dynamic_conent(self, outfile, _):
         if not outfile.path.endswith('.md'):
             return
         page_html = self._renderer.render_md(outfile.content,
                                              posixpath.splitext(outfile.path)[0],
+                                             meta_info=outfile.meta_info,
                                              editorbutton=False,
                                              nav=False,
                                              template=self._renderer.PDFPAGE)
         self._html[outfile.path] = page_html
 
     def _build_static_conent(self, outfile, full_out_path):
         # Convert all images to a smallish PNG due to GDK_pixbuf bug. Can remove this
```

### Comparing `gitbuilding-0.9.0/gitbuilding/previewers.py` & `gitbuilding-0.9.1/gitbuilding/previewers.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class ThreeDimPreviewer(Previewer):
     """
     Build-up previewer that will preview 3D models with GB3D
     """
 
     def __init__(self, enabled):
         super().__init__(enabled)
+        self._name = "3D-previewer"
         self._drop_dir = "models"
         self._create_preview_page_when_enabled = True
 
     @property
     def pattern(self):
         """
         Pattern to match supported models
@@ -71,14 +72,15 @@
 class PDFPreviewer(Previewer):
     """
     Build-up previewer that will preview PDF files
     """
 
     def __init__(self, enabled):
         super().__init__(enabled)
+        self._name = "PDF-previewer"
         self._drop_dir = "documents"
 
     @property
     def pattern(self):
         """
         Pattern to match pdf files
         """
@@ -96,14 +98,17 @@
 
         return html
 
 class YouTubePreviewer(Previewer):
     """
     Build-up previewer that will embed YouTube links.
     """
+    def __init__(self, enabled):
+        super().__init__(enabled)
+        self._name = "YouTube-previewer"
 
     @property
     def pattern(self):
         """
         Pattern to match a youtube link
         """
         return re.compile(r'^https?\:\/\/(?:www\.)?youtube\.com\/watch\?v=([a-zA-Z0-9_\-]+)$')
```

### Comparing `gitbuilding-0.9.0/gitbuilding/render.py` & `gitbuilding-0.9.1/gitbuilding/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,15 @@
     def render(self, html, link, **kwargs):
         """
         This function creates the full HTML page from the input HTML generated from BuildUp
         """
         template = kwargs.get('template', self.FULLPAGE)
         nav = kwargs.get('nav', True)
         editorbutton = kwargs.get('editorbutton', False)
+        meta_info = kwargs.get('meta_info', {})
 
         if link is None:
             editor_link = "-/editor"
         else:
             editor_link = f"/{link}/-/editor"
 
         input_dictionary = {'favicon_html': self.favicon_html(link),
@@ -357,15 +358,16 @@
                             'nav': nav,
                             'nav_links': self.nav_links(link),
                             'project_header': self.project_header(link=link),
                             'project_footer': self.project_footer(link),
                             'static': self._static,
                             'warning_count': self._warning_count,
                             'editorbutton': editorbutton,
-                            'editor_link': editor_link}
+                            'editor_link': editor_link,
+                            'previewers_used': meta_info.get('previewers_used', [])}
 
         if template == self.FULLPAGE:
             tmpl = self.env.get_template("full_page.html.jinja")
             input_dictionary['custom_stylesheets'] = self.custom_stylesheets
         elif template == self.IFRAME:
             tmpl = self.env.get_template("iframe.html.jinja")
             custom_style = []
```

### Comparing `gitbuilding-0.9.0/gitbuilding/server.py` & `gitbuilding-0.9.1/gitbuilding/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,14 +519,15 @@
             editorbutton = True
         if path.is_homepage:
             link = None
         else:
             link = path.web_path
         return self.renderer.render_md(path.gb_file.content,
                                        link,
+                                       meta_info=path.gb_file.meta_info,
                                        editorbutton=editorbutton)
 
     def _render_missing_file(self, path):
         """
         Render a file that is not found in the GitBuilding documentation object. This could be
         a recently dragged and dropped file, or a file that is in
         the gitbuilding directory but was not processed during the last full build
```

### Comparing `gitbuilding-0.9.0/gitbuilding/static/3d-viewer.js` & `gitbuilding-0.9.1/gitbuilding/static/3d-viewer.js`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding.pdf` & `gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding.pdf`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding.svg` & `gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding.svg`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/GitBuilding500x.png` & `gitbuilding-0.9.1/gitbuilding/static/Logo/GitBuilding500x.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/favicon-16x16.png` & `gitbuilding-0.9.1/gitbuilding/static/Logo/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/favicon-32x32.png` & `gitbuilding-0.9.1/gitbuilding/static/Logo/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/Logo/favicon.ico` & `gitbuilding-0.9.1/gitbuilding/static/Logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/css/app.2bbbc00f.css` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/css/app.2bbbc00f.css`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/favicon.ico` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/favicon.ico`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/index.html` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/index.html`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/js/app.da0d2df1.js` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/js/app.da0d2df1.js`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/js/app.da0d2df1.js.map` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/js/app.da0d2df1.js.map`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js.map` & `gitbuilding-0.9.1/gitbuilding/static/live-editor/js/chunk-vendors.2965e1bb.js.map`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/DuplicatePage.png` & `gitbuilding-0.9.1/gitbuilding/static/local-server/DuplicatePage.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/DuplicatePage.svg` & `gitbuilding-0.9.1/gitbuilding/static/local-server/DuplicatePage.svg`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/EmptyPage.png` & `gitbuilding-0.9.1/gitbuilding/static/local-server/EmptyPage.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/EmptyPage.svg` & `gitbuilding-0.9.1/gitbuilding/static/local-server/EmptyPage.svg`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/Missing_image.png` & `gitbuilding-0.9.1/gitbuilding/static/local-server/Missing_image.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/Missing_image.svg` & `gitbuilding-0.9.1/gitbuilding/static/local-server/Missing_image.svg`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/StepByStepPage.png` & `gitbuilding-0.9.1/gitbuilding/static/local-server/StepByStepPage.png`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/local-server/StepByStepPage.svg` & `gitbuilding-0.9.1/gitbuilding/static/local-server/StepByStepPage.svg`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/static/style.css` & `gitbuilding-0.9.1/gitbuilding/static/style.css`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/body.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/body.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/contents.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/contents.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/footer.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/footer.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/full_page.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/full_page.html.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     {{ favicon_html | safe }}
     <link href="{{root}}static/style.css" rel="stylesheet">
     {% for sheet in custom_stylesheets %}
         <link href="{{root}}{{sheet}}" rel="stylesheet">
     {% endfor %}
+    {% if '3D-previewer' in previewers_used %}
     <script type="text/javascript" src="{{root}}static/3d-viewer.js"></script>
-    
+    {% endif %}
 </head>
 <body>
 {% include 'body.html.jinja' %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 
  {{ favicon_html | safe }}
  {% for sheet in custom_stylesheets %}
- {% endfor %}
+ {% endfor %} {% if '3D-previewer' in previewers_used %}
+ {% endif %}
 {% include 'body.html.jinja' %}
```

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/full_pdf.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/full_pdf.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/nav.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/nav.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/new1.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/new1.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/templates/new2.html.jinja` & `gitbuilding-0.9.1/gitbuilding/templates/new2.html.jinja`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding/utilities.py` & `gitbuilding-0.9.1/gitbuilding/utilities.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/gitbuilding.egg-info/PKG-INFO` & `gitbuilding-0.9.1/gitbuilding.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbuilding
-Version: 0.9.0
+Version: 0.9.1
 Summary: For documenting hardware projects with minimal effort,so you can stop writing and GitBuilding.
 Home-page: https://gitbuilding.io/
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: GPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/gitbuilding/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/gitbuilding
@@ -70,7 +70,8 @@
 Keywords: Documentation,Hardware
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `gitbuilding-0.9.0/gitbuilding.egg-info/SOURCES.txt` & `gitbuilding-0.9.1/gitbuilding.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 gitbuilding/__init__.py
 gitbuilding/__main__.py
 gitbuilding/config.py
 gitbuilding/example.py
```

### Comparing `gitbuilding-0.9.0/pyproject.toml` & `gitbuilding-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/setup.py` & `gitbuilding-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Setup for the module'''
 
 __author__ = 'Julian Stirling'
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 import sys
 from os import path
 import glob
 from setuptools import setup, find_packages
 
 def install():
@@ -57,12 +57,18 @@
                             'markdown',
                             'markdown_katex',
                             'colorama',
                             'marshmallow>=03.8,<3.12',
                             'jinja2',
                             'regex',
                             'waitress'],
+          extras_require={'dev': ['weasyprint',
+                                  'pylint',
+                                  'codecov',
+                                  'curlylint',
+                                  'pydeps',
+                                  'twine']},
           python_requires=">=3.6",
           entry_points={'console_scripts': ['gitbuilding = gitbuilding.__main__:main']})
 
 if __name__ == "__main__":
     install()
```

### Comparing `gitbuilding-0.9.0/tests/checklogs.py` & `gitbuilding-0.9.1/tests/checklogs.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/test_handler.py` & `gitbuilding-0.9.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/test_main.py` & `gitbuilding-0.9.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/test_utilities.py` & `gitbuilding-0.9.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_buildup.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_buildup.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_config.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_config.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_files.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_files.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_part.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_part.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_partlist.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_partlist.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_quantity.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_quantity.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_unit.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_unit.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_url.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_url.py`

 * *Files identical despite different names*

### Comparing `gitbuilding-0.9.0/tests/tests_buildup/test_utilities.py` & `gitbuilding-0.9.1/tests/tests_buildup/test_utilities.py`

 * *Files identical despite different names*


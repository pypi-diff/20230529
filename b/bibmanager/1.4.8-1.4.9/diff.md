# Comparing `tmp/bibmanager-1.4.8.tar.gz` & `tmp/bibmanager-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibmanager-1.4.8.tar", last modified: Mon Jan  2 22:26:18 2023, max compression
+gzip compressed data, was "bibmanager-1.4.9.tar", last modified: Mon May 29 09:07:11 2023, max compression
```

## Comparing `bibmanager-1.4.8.tar` & `bibmanager-1.4.9.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.375392 bibmanager-1.4.8/
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.358286 bibmanager-1.4.8/.github/
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.360856 bibmanager-1.4.8/.github/workflows/
--rw-r--r--   0 pato       (501) staff       (20)     1583 2023-01-02 22:25:56.000000 bibmanager-1.4.8/.github/workflows/python-package.yml
--rw-r--r--   0 pato       (501) staff       (20)    59285 2023-01-02 22:25:56.000000 bibmanager-1.4.8/CHANGELOG.txt
--rw-r--r--   0 pato       (501) staff       (20)     2888 2020-02-02 19:46:06.000000 bibmanager-1.4.8/CONTRIBUTING.md
--rw-r--r--   0 pato       (501) staff       (20)     1074 2018-02-09 22:11:29.000000 bibmanager-1.4.8/LICENSE
--rw-r--r--   0 pato       (501) staff       (20)      201 2022-08-10 10:41:22.000000 bibmanager-1.4.8/MANIFEST.in
--rw-r--r--   0 pato       (501) staff       (20)     3168 2023-01-02 22:26:18.375259 bibmanager-1.4.8/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1759 2022-09-23 08:38:03.000000 bibmanager-1.4.8/README.md
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.361636 bibmanager-1.4.8/bibmanager/
--rw-r--r--   0 pato       (501) staff       (20)      748 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    45977 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/__main__.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.362465 bibmanager-1.4.8/bibmanager/ads_manager/
--rw-r--r--   0 pato       (501) staff       (20)      491 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/ads_manager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    15845 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/ads_manager/ads_manager.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.363155 bibmanager-1.4.8/bibmanager/bib_manager/
--rw-r--r--   0 pato       (501) staff       (20)      543 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/bib_manager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    44939 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/bib_manager/bib_manager.py
--rwxr-xr-x   0 pato       (501) staff       (20)    24747 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/bib_manager/browser.py
--rw-r--r--   0 pato       (501) staff       (20)      113 2020-02-02 19:46:06.000000 bibmanager-1.4.8/bibmanager/config
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.363476 bibmanager-1.4.8/bibmanager/config_manager/
--rw-r--r--   0 pato       (501) staff       (20)      497 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/config_manager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    10143 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/config_manager/config_manager.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.365119 bibmanager-1.4.8/bibmanager/examples/
--rw-r--r--   0 pato       (501) staff       (20)   212301 2019-01-11 16:12:53.000000 bibmanager-1.4.8/bibmanager/examples/aastex62.cls
--rw-r--r--   0 pato       (501) staff       (20)    33792 2019-01-11 16:12:53.000000 bibmanager-1.4.8/bibmanager/examples/apj_hyperref.bst
--rw-r--r--   0 pato       (501) staff       (20)    11187 2022-01-28 16:35:26.000000 bibmanager-1.4.8/bibmanager/examples/sample.bib
--rw-r--r--   0 pato       (501) staff       (20)     3089 2022-01-28 16:35:26.000000 bibmanager-1.4.8/bibmanager/examples/sample.tex
--rw-r--r--   0 pato       (501) staff       (20)    11203 2019-01-11 16:12:53.000000 bibmanager-1.4.8/bibmanager/examples/top-apj.tex
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.365472 bibmanager-1.4.8/bibmanager/latex_manager/
--rw-r--r--   0 pato       (501) staff       (20)      495 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/latex_manager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    13033 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/latex_manager/latex_manager.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.365724 bibmanager-1.4.8/bibmanager/pdf_manager/
--rw-r--r--   0 pato       (501) staff       (20)      491 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/pdf_manager/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    13823 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/pdf_manager/pdf_manager.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.366026 bibmanager-1.4.8/bibmanager/utils/
--rw-r--r--   0 pato       (501) staff       (20)      478 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/utils/__init__.py
--rw-r--r--   0 pato       (501) staff       (20)    49573 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/utils/utils.py
--rw-r--r--   0 pato       (501) staff       (20)      164 2023-01-02 22:25:56.000000 bibmanager-1.4.8/bibmanager/version.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.362228 bibmanager-1.4.8/bibmanager.egg-info/
--rw-r--r--   0 pato       (501) staff       (20)     3168 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/PKG-INFO
--rw-r--r--   0 pato       (501) staff       (20)     1542 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/SOURCES.txt
--rw-r--r--   0 pato       (501) staff       (20)        1 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/dependency_links.txt
--rw-r--r--   0 pato       (501) staff       (20)       51 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/entry_points.txt
--rw-r--r--   0 pato       (501) staff       (20)       85 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/requires.txt
--rw-r--r--   0 pato       (501) staff       (20)       11 2023-01-02 22:26:18.000000 bibmanager-1.4.8/bibmanager.egg-info/top_level.txt
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.373095 bibmanager-1.4.8/docs/
--rw-r--r--   0 pato       (501) staff       (20)     7903 2019-01-07 21:44:28.000000 bibmanager-1.4.8/docs/Makefile
--rw-r--r--   0 pato       (501) staff       (20)    13098 2021-12-05 18:20:36.000000 bibmanager-1.4.8/docs/ads.rst
--rw-r--r--   0 pato       (501) staff       (20)    61437 2021-12-05 18:20:36.000000 bibmanager-1.4.8/docs/api.rst
--rw-r--r--   0 pato       (501) staff       (20)    22964 2022-01-28 16:35:26.000000 bibmanager-1.4.8/docs/bibtex.rst
--rw-r--r--   0 pato       (501) staff       (20)     5354 2019-07-27 10:28:25.000000 bibmanager-1.4.8/docs/conf.py
--rw-r--r--   0 pato       (501) staff       (20)     2970 2019-07-27 10:28:25.000000 bibmanager-1.4.8/docs/contributing.rst
--rw-r--r--   0 pato       (501) staff       (20)     7431 2022-08-10 09:16:15.000000 bibmanager-1.4.8/docs/faq.rst
--rw-r--r--   0 pato       (501) staff       (20)    56914 2020-02-02 19:46:06.000000 bibmanager-1.4.8/docs/fetch.gif
--rw-r--r--   0 pato       (501) staff       (20)     3879 2021-02-28 11:46:21.000000 bibmanager-1.4.8/docs/getstarted.rst
--rw-r--r--   0 pato       (501) staff       (20)     6339 2022-09-23 08:43:15.000000 bibmanager-1.4.8/docs/index.rst
--rw-r--r--   0 pato       (501) staff       (20)   669020 2020-11-02 09:16:17.000000 bibmanager-1.4.8/docs/infograph.png
--rw-r--r--   0 pato       (501) staff       (20)     3309 2019-01-07 21:44:28.000000 bibmanager-1.4.8/docs/latex.rst
--rw-r--r--   0 pato       (501) staff       (20)     1122 2023-01-02 22:25:56.000000 bibmanager-1.4.8/docs/license.rst
--rw-r--r--   0 pato       (501) staff       (20)    21923 2019-01-07 21:44:28.000000 bibmanager-1.4.8/docs/logo_bibmanager.png
--rw-r--r--   0 pato       (501) staff       (20)     7740 2019-01-07 21:44:28.000000 bibmanager-1.4.8/docs/make.bat
--rw-r--r--   0 pato       (501) staff       (20)     7089 2020-09-06 12:24:05.000000 bibmanager-1.4.8/docs/pdf.rst
--rw-r--r--   0 pato       (501) staff       (20)   233120 2022-08-10 09:16:15.000000 bibmanager-1.4.8/docs/raycast_bibmanager_screenshot.png
--rw-r--r--   0 pato       (501) staff       (20)    61199 2020-02-02 19:46:06.000000 bibmanager-1.4.8/docs/search.gif
--rw-r--r--   0 pato       (501) staff       (20)       85 2020-11-02 09:16:17.000000 bibmanager-1.4.8/requirements.txt
--rw-r--r--   0 pato       (501) staff       (20)       38 2023-01-02 22:26:18.375430 bibmanager-1.4.8/setup.cfg
--rw-r--r--   0 pato       (501) staff       (20)     3856 2023-01-02 22:25:56.000000 bibmanager-1.4.8/setup.py
-drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-01-02 22:26:18.374865 bibmanager-1.4.8/tests/
--rw-r--r--   0 pato       (501) staff       (20)    29383 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/conftest.py
--rw-r--r--   0 pato       (501) staff       (20)    12471 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_ads.py
--rw-r--r--   0 pato       (501) staff       (20)    46699 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_bib_manager.py
--rw-r--r--   0 pato       (501) staff       (20)    50979 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_cli.py
--rw-r--r--   0 pato       (501) staff       (20)    11398 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_config_manager.py
--rw-r--r--   0 pato       (501) staff       (20)    10752 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_latex_manager.py
--rw-r--r--   0 pato       (501) staff       (20)    22849 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_pdf_manager.py
--rw-r--r--   0 pato       (501) staff       (20)    22470 2023-01-02 22:25:56.000000 bibmanager-1.4.8/tests/test_utils.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.380995 bibmanager-1.4.9/
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.364176 bibmanager-1.4.9/.github/
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.366347 bibmanager-1.4.9/.github/workflows/
+-rw-r--r--   0 pato       (501) staff       (20)     1583 2023-01-02 22:25:56.000000 bibmanager-1.4.9/.github/workflows/python-package.yml
+-rw-r--r--   0 pato       (501) staff       (20)    60617 2023-05-29 09:06:21.000000 bibmanager-1.4.9/CHANGELOG.txt
+-rw-r--r--   0 pato       (501) staff       (20)     2888 2020-02-02 19:46:06.000000 bibmanager-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 pato       (501) staff       (20)     1074 2018-02-09 22:11:29.000000 bibmanager-1.4.9/LICENSE
+-rw-r--r--   0 pato       (501) staff       (20)      201 2022-08-10 10:41:22.000000 bibmanager-1.4.9/MANIFEST.in
+-rw-r--r--   0 pato       (501) staff       (20)     3168 2023-05-29 09:07:11.380863 bibmanager-1.4.9/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1759 2022-09-23 08:38:03.000000 bibmanager-1.4.9/README.md
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.367285 bibmanager-1.4.9/bibmanager/
+-rw-r--r--   0 pato       (501) staff       (20)      748 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    46952 2023-05-29 09:06:21.000000 bibmanager-1.4.9/bibmanager/__main__.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.368301 bibmanager-1.4.9/bibmanager/ads_manager/
+-rw-r--r--   0 pato       (501) staff       (20)      491 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/ads_manager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    16694 2023-05-29 09:06:21.000000 bibmanager-1.4.9/bibmanager/ads_manager/ads_manager.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.368781 bibmanager-1.4.9/bibmanager/bib_manager/
+-rw-r--r--   0 pato       (501) staff       (20)      543 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/bib_manager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    46053 2023-05-29 09:06:21.000000 bibmanager-1.4.9/bibmanager/bib_manager/bib_manager.py
+-rwxr-xr-x   0 pato       (501) staff       (20)    24747 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/bib_manager/browser.py
+-rw-r--r--   0 pato       (501) staff       (20)      113 2020-02-02 19:46:06.000000 bibmanager-1.4.9/bibmanager/config
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.369338 bibmanager-1.4.9/bibmanager/config_manager/
+-rw-r--r--   0 pato       (501) staff       (20)      497 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/config_manager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    10143 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/config_manager/config_manager.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.370893 bibmanager-1.4.9/bibmanager/examples/
+-rw-r--r--   0 pato       (501) staff       (20)   212301 2019-01-11 16:12:53.000000 bibmanager-1.4.9/bibmanager/examples/aastex62.cls
+-rw-r--r--   0 pato       (501) staff       (20)    33792 2019-01-11 16:12:53.000000 bibmanager-1.4.9/bibmanager/examples/apj_hyperref.bst
+-rw-r--r--   0 pato       (501) staff       (20)    11187 2022-01-28 16:35:26.000000 bibmanager-1.4.9/bibmanager/examples/sample.bib
+-rw-r--r--   0 pato       (501) staff       (20)     3089 2022-01-28 16:35:26.000000 bibmanager-1.4.9/bibmanager/examples/sample.tex
+-rw-r--r--   0 pato       (501) staff       (20)    11203 2019-01-11 16:12:53.000000 bibmanager-1.4.9/bibmanager/examples/top-apj.tex
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.371220 bibmanager-1.4.9/bibmanager/latex_manager/
+-rw-r--r--   0 pato       (501) staff       (20)      495 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/latex_manager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    16997 2023-05-29 09:06:21.000000 bibmanager-1.4.9/bibmanager/latex_manager/latex_manager.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.371478 bibmanager-1.4.9/bibmanager/pdf_manager/
+-rw-r--r--   0 pato       (501) staff       (20)      491 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/pdf_manager/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    13823 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/pdf_manager/pdf_manager.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.371719 bibmanager-1.4.9/bibmanager/utils/
+-rw-r--r--   0 pato       (501) staff       (20)      478 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/utils/__init__.py
+-rw-r--r--   0 pato       (501) staff       (20)    49573 2023-01-02 22:25:56.000000 bibmanager-1.4.9/bibmanager/utils/utils.py
+-rw-r--r--   0 pato       (501) staff       (20)      164 2023-05-29 09:06:21.000000 bibmanager-1.4.9/bibmanager/version.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.367962 bibmanager-1.4.9/bibmanager.egg-info/
+-rw-r--r--   0 pato       (501) staff       (20)     3168 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/PKG-INFO
+-rw-r--r--   0 pato       (501) staff       (20)     1604 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 pato       (501) staff       (20)        1 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 pato       (501) staff       (20)       51 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/entry_points.txt
+-rw-r--r--   0 pato       (501) staff       (20)       85 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/requires.txt
+-rw-r--r--   0 pato       (501) staff       (20)       11 2023-05-29 09:07:11.000000 bibmanager-1.4.9/bibmanager.egg-info/top_level.txt
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.378011 bibmanager-1.4.9/docs/
+-rw-r--r--   0 pato       (501) staff       (20)    94208 2023-05-29 08:58:39.000000 bibmanager-1.4.9/docs/.api.rst.swp
+-rw-r--r--   0 pato       (501) staff       (20)    40960 2023-05-29 08:53:49.000000 bibmanager-1.4.9/docs/.bibtex.rst.swp
+-rw-r--r--   0 pato       (501) staff       (20)     7903 2019-01-07 21:44:28.000000 bibmanager-1.4.9/docs/Makefile
+-rw-r--r--   0 pato       (501) staff       (20)    13098 2021-12-05 18:20:36.000000 bibmanager-1.4.9/docs/ads.rst
+-rw-r--r--   0 pato       (501) staff       (20)    74085 2023-05-29 09:06:21.000000 bibmanager-1.4.9/docs/api.rst
+-rw-r--r--   0 pato       (501) staff       (20)    23250 2023-05-29 09:06:21.000000 bibmanager-1.4.9/docs/bibtex.rst
+-rw-r--r--   0 pato       (501) staff       (20)     5354 2019-07-27 10:28:25.000000 bibmanager-1.4.9/docs/conf.py
+-rw-r--r--   0 pato       (501) staff       (20)     2970 2019-07-27 10:28:25.000000 bibmanager-1.4.9/docs/contributing.rst
+-rw-r--r--   0 pato       (501) staff       (20)     7431 2022-08-10 09:16:15.000000 bibmanager-1.4.9/docs/faq.rst
+-rw-r--r--   0 pato       (501) staff       (20)    56914 2020-02-02 19:46:06.000000 bibmanager-1.4.9/docs/fetch.gif
+-rw-r--r--   0 pato       (501) staff       (20)     3879 2021-02-28 11:46:21.000000 bibmanager-1.4.9/docs/getstarted.rst
+-rw-r--r--   0 pato       (501) staff       (20)     6339 2022-09-23 08:43:15.000000 bibmanager-1.4.9/docs/index.rst
+-rw-r--r--   0 pato       (501) staff       (20)   669020 2020-11-02 09:16:17.000000 bibmanager-1.4.9/docs/infograph.png
+-rw-r--r--   0 pato       (501) staff       (20)     3309 2019-01-07 21:44:28.000000 bibmanager-1.4.9/docs/latex.rst
+-rw-r--r--   0 pato       (501) staff       (20)     1122 2023-01-02 22:25:56.000000 bibmanager-1.4.9/docs/license.rst
+-rw-r--r--   0 pato       (501) staff       (20)    21923 2019-01-07 21:44:28.000000 bibmanager-1.4.9/docs/logo_bibmanager.png
+-rw-r--r--   0 pato       (501) staff       (20)     7740 2019-01-07 21:44:28.000000 bibmanager-1.4.9/docs/make.bat
+-rw-r--r--   0 pato       (501) staff       (20)     7089 2020-09-06 12:24:05.000000 bibmanager-1.4.9/docs/pdf.rst
+-rw-r--r--   0 pato       (501) staff       (20)   233120 2022-08-10 09:16:15.000000 bibmanager-1.4.9/docs/raycast_bibmanager_screenshot.png
+-rw-r--r--   0 pato       (501) staff       (20)    61199 2020-02-02 19:46:06.000000 bibmanager-1.4.9/docs/search.gif
+-rw-r--r--   0 pato       (501) staff       (20)       85 2020-11-02 09:16:17.000000 bibmanager-1.4.9/requirements.txt
+-rw-r--r--   0 pato       (501) staff       (20)       38 2023-05-29 09:07:11.381034 bibmanager-1.4.9/setup.cfg
+-rw-r--r--   0 pato       (501) staff       (20)     3856 2023-01-02 22:25:56.000000 bibmanager-1.4.9/setup.py
+drwxr-xr-x   0 pato       (501) staff       (20)        0 2023-05-29 09:07:11.380590 bibmanager-1.4.9/tests/
+-rw-r--r--   0 pato       (501) staff       (20)    69632 2023-05-29 08:40:25.000000 bibmanager-1.4.9/tests/.test_cli.py.swp
+-rw-r--r--   0 pato       (501) staff       (20)    29383 2023-01-02 22:25:56.000000 bibmanager-1.4.9/tests/conftest.py
+-rw-r--r--   0 pato       (501) staff       (20)    12411 2023-05-29 09:06:21.000000 bibmanager-1.4.9/tests/test_ads.py
+-rw-r--r--   0 pato       (501) staff       (20)    47090 2023-05-29 09:06:21.000000 bibmanager-1.4.9/tests/test_bib_manager.py
+-rw-r--r--   0 pato       (501) staff       (20)    50704 2023-05-29 09:06:21.000000 bibmanager-1.4.9/tests/test_cli.py
+-rw-r--r--   0 pato       (501) staff       (20)    11398 2023-01-02 22:25:56.000000 bibmanager-1.4.9/tests/test_config_manager.py
+-rw-r--r--   0 pato       (501) staff       (20)    12010 2023-05-29 09:06:21.000000 bibmanager-1.4.9/tests/test_latex_manager.py
+-rw-r--r--   0 pato       (501) staff       (20)    22849 2023-01-02 22:25:56.000000 bibmanager-1.4.9/tests/test_pdf_manager.py
+-rw-r--r--   0 pato       (501) staff       (20)    22470 2023-01-02 22:25:56.000000 bibmanager-1.4.9/tests/test_utils.py
```

### Comparing `bibmanager-1.4.8/.github/workflows/python-package.yml` & `bibmanager-1.4.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/CHANGELOG.txt` & `bibmanager-1.4.9/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2710,7 +2710,72 @@
 
 Removed outdated keybindings in browser.
 
 Bumped bibmanager to version 1.4.7.
 
 Fixed bug.
 
+
+*****  Sun May 28 23:57:36 CEST 2023  *****
+
+In remove_duplicates() check isbn unique books before removing dups
+to prevent removing them when in fact they are not duplicates
+
+*****
+
+Modified bm.remove_duplicates() to return dictionary of replaced keys
+that were duplicates of others.
+
+*****
+
+Added return_replacements argument in bm.read_file() function
+to enable collecting dict of replaced keys.
+
+*****
+
+Cosmetics.
+
+*****
+
+Fixed am.display() bug when an entry does not have authors.
+Tests is TBD.
+
+*****
+
+Added return_replacements argument in am.add_bibtex() function
+to keep track of replaced keys.
+Tests TBD.
+
+*****
+
+Added return_replacements argument in am.update() function
+to keep track of replaced keys.
+Tests TBD.
+
+
+*****  Mon May 29 09:46:00 CEST 2023  *****
+
+Implemented lm.get_bibfile() function.
+
+*****
+
+Implemented lm.update_keys() function to update keys in a .tex file
+given a dictionary of replacements.
+Acts recursively into referenced .tex file.
+Does not work in citations referenced inside another citation.
+Tests TBD.
+
+*****
+
+Refactored cleanup command to also take .tex files.
+In this case, the code will filter out duplicates, and will
+update both the .tex and .bib files.  Making sure outdated (removed)
+bibtex keys get updated.
+Tests TBD.
+
+*****
+
+Updated docs.
+
+*****
+
+Bumped bibmanager to version 1.4.9.
```

### Comparing `bibmanager-1.4.8/CONTRIBUTING.md` & `bibmanager-1.4.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/LICENSE` & `bibmanager-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/PKG-INFO` & `bibmanager-1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibmanager
-Version: 1.4.8
+Version: 1.4.9
 Summary: A BibTeX manager for LaTeX projects
 Home-page: https://github.com/pcubillos/bibmanager
 Author: Patricio Cubillos
 Author-email: pcubillos@fulbrightmail.org
 License: MIT
 Description:
```

### Comparing `bibmanager-1.4.8/README.md` & `bibmanager-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/__init__.py` & `bibmanager-1.4.9/bibmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/__main__.py` & `bibmanager-1.4.9/bibmanager/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import os
 from datetime import date
 from packaging import version
 
 import prompt_toolkit
 from prompt_toolkit.history import FileHistory
 
-from . import bib_manager    as bm
-from . import latex_manager  as lm
+from . import bib_manager as bm
+from . import latex_manager as lm
 from . import config_manager as cm
-from . import ads_manager    as am
-from . import pdf_manager    as pm
+from . import ads_manager as am
+from . import pdf_manager as pm
 from . import utils as u
 from .__init__ import __version__
 
 
 # Parser Main Documentation:
 main_description = f"""
 BibTeX Database Management:
@@ -214,23 +214,45 @@
         return
     else:
         print(f"\nError: Invalid file extension ('{extension}'), must be "
                "'.bib' or '.bbl'.")
 
 
 def cli_cleanup(args):
-    """Command-line interface to clean up a bibfile."""
-    bibs = bm.read_file(args.bibfile)
+    """Command-line interface to clean up a tex or a bibfile."""
+    if args.bibtex.endswith('.tex'):
+        texfile = args.bibtex
+        bibfile = lm.get_bibfile(texfile)
+        is_tex = True
+    elif args.bibtex.endswith('.bib'):
+        bibfile = args.bibtex
+        is_tex = False
+    else:
+        raise ValueError('Invalid file extension, must be .tex or .bib')
+
+    # Remove duplicates, store changed keys:
+    bibs, reps = bm.read_file(bibfile, return_replacements=True)
     if args.ads:
         try:
-            updated = am.update(base=bibs)
+            # Store updated keys:
+            updated, ads_reps = am.update(base=bibs, return_replacements=True)
             bibs = updated
+            # Merge ads_reps into reps:
+            for ads_key, ads_val in ads_reps.items():
+                if ads_key in reps.values():
+                    idx = list(reps.values()).index(ads_key)
+                    ads_key = list(reps.keys())[idx]
+                reps[ads_key] = ads_val
         except ValueError as e:
             print(f"\nError: {str(e)}. Continue without ADS update.")
-    bm.export(bibs, args.bibfile)
+    bm.export(bibs, bibfile)
+
+    if is_tex and len(reps) > 0:
+        # Now, update .tex file with updated key names:
+        lm.update_keys(texfile, reps, is_main=True)
 
 
 def cli_config(args):
     """Command-line interface for config call."""
     try:
         if args.param is None:
             cm.display()
@@ -808,33 +830,41 @@
         help="Path to an output BibTeX file.")
     export.add_argument('-meta', action='store_true', default=False,
         help="Also include meta-information in output file.")
     export.set_defaults(func=cli_export)
 
 
     cleanup_description = f"""
-{u.BOLD}Clean up a bibtex file of duplicates and outdated entries.{u.END}
+{u.BOLD}Clean up a bibtex or latex file of duplicates and outdated entries.{u.END}
 
 Description
-  'Clean up' a BibTeX file by removing duplicates, sorting the entries,
-  and (if requested) updating the entries by cross-checking against
-  the ADS database.  All of this is done independently of the bibmanager
-  database.
+  'Clean up' a BibTeX (.bib) or LaTeX (.tex) file by removing duplicates,
+  sorting the entries, and (if requested) updating the entries by
+  cross-checking against the ADS database.  All of this is done
+  independently of the bibmanager database.
 
 Examples
   # Remove duplicates, update ADS entries, and sort:
   bibm cleanup file.bib -ads
 """
-    cleanup = sp.add_parser('cleanup', description=cleanup_description,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
-    cleanup.add_argument("bibfile", action="store",
-        help="Path to an existing BibTeX file.")
-    cleanup.add_argument('-ads', action='store_true', default=False,
+    cleanup = sp.add_parser(
+        'cleanup',
+        description=cleanup_description,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    cleanup.add_argument(
+        "bibtex",
+        action="store",
+        help="Path to an existing .tex or .bib file.",
+    )
+    cleanup.add_argument(
+        '-ads', action='store_true', default=False,
         help="Update the bibfile entries cross-checking against the ADS "
-             "database.")
+             "database."
+    )
     cleanup.set_defaults(func=cli_cleanup)
 
 
     config_description = f"""
 {u.BOLD}Manage the bibmanager configuration parameters.{u.END}
 
 Description
```

### Comparing `bibmanager-1.4.8/bibmanager/ads_manager/ads_manager.py` & `bibmanager-1.4.9/bibmanager/ads_manager/ads_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,20 +174,24 @@
         tokens = [(Token.Text, '\n')]
         title = textwrap.fill(
             f"Title: {result['title'][0]}",
             width=78,
             subsequent_indent='    ')
         tokens += u.tokenizer('Title', title[7:])
 
-        author_list = [u.parse_name(author) for author in result['author']]
-        author_format = 'short' if short else 'long'
-        authors = textwrap.fill(
-            f"Authors: {u.get_authors(author_list, format=author_format)}",
-            width=78,
-            subsequent_indent='    ')
+        if 'author' in result:
+            author_list = [u.parse_name(author) for author in result['author']]
+            author_format = 'short' if short else 'long'
+            authors = textwrap.fill(
+                f"Authors: {u.get_authors(author_list, format=author_format)}",
+                width=78,
+                subsequent_indent='    ',
+            )
+        else:
+            authors = 'Authors: ---'
         tokens += u.tokenizer('Authors', authors[9:])
 
         adsurl = f"https://ui.adsabs.harvard.edu/abs/{result['bibcode']}"
         tokens += u.tokenizer('ADS URL', adsurl)
 
         bibcode = result['bibcode']
         tokens += u.tokenizer('bibcode', bibcode, Token.Name.Label)
@@ -205,16 +209,18 @@
     else:
         more = ""
     print(
         f"\nShowing entries {index+1}--{min(index+rows, nmatch)} out of "
         f"{nmatch} matches.{more}")
 
 
-def add_bibtex(input_bibcodes, input_keys, eprints=[], dois=[],
-               update_keys=True, base=None, tags=None):
+def add_bibtex(
+        input_bibcodes, input_keys, eprints=[], dois=[],
+        update_keys=True, base=None, tags=None, return_replacements=False,
+    ):
     """
     Add bibtex entries from a list of ADS bibcodes, with specified keys.
     New entries will replace old ones without asking if they are
     duplicates.
 
     Parameters
     ----------
@@ -230,19 +236,23 @@
         If True, attempt to update keys of entries that were updated
         from arxiv to published versions.
     base: List of Bib() objects
         If None, merge new entries into the bibmanager database.
         If not None, merge new entries into base.
     tags: Nested list of strings
         The list of tags for each input bibcode.
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
 
     Returns
     -------
     bibs: List of Bib() objects
         Updated list of BibTeX entries.
+    reps: Dict
+        A dictionary of replaced key names.
 
     Examples
     --------
     >>> import bibmanager.ads_manager as am
     >>> # A successful add call:
     >>> bibcodes = ['1925PhDT.........1P']
     >>> keys = ['Payne1925phdStellarAtmospheres']
@@ -304,15 +314,15 @@
 
     # Keep counts of things:
     nreqs = len(bibcodes)
 
     # Split output into separate BibTeX entries (keep as strings):
     results = results.strip().split("\n\n")
 
-    new_keys = []
+    new_keys = {}
     new_bibs = []
     founds = [False for _ in bibcodes]
     arxiv_updates = 0
     # Match results to bibcodes,keys:
     for result in reversed(results):
         ibib = None
         new = bm.Bib(result)
@@ -325,17 +335,17 @@
         elif new.doi is not None and new.doi in dois:
             ibib = dois.index(new.doi)
 
         if ibib is not None:
             new.tags = tags[ibib]
             new_key = keys[ibib]
             updated_key = key_update(new_key, new.bibcode, bibcodes[ibib])
-            if update_keys and updated_key.lower() != new_key.lower():
+            if update_keys and updated_key != new_key:
                 new_key = updated_key
-                new_keys.append([keys[ibib], new_key])
+                new_keys[keys[ibib]] = updated_key
             if 'arXiv' in bibcodes[ibib] and 'arXiv' not in new.bibcode:
                 arxiv_updates += 1
 
             new.update_key(new_key)
             new_bibs.append(new)
             founds[ibib] = True
             results.remove(result)
@@ -355,46 +365,64 @@
         # bibcodes not matched:
         if len(results) > 0:
             warning += '\nThese ADS results did not match input bibcodes:\n\n'
             warning += '\n\n'.join(results) + "\n"
         warning += u.BANNER
         print(warning)
 
+    n_new = len(new_bibs)
+    if base is None:
+        nbibs = len(bm.load())
+    else:
+        nbibs = len(base)
+
     # Add to bibmanager database or base:
     updated = bm.merge(new=new_bibs, take='new', base=base)
-    print('(Not counting updated references)')
+    actually_new = len(updated) - nbibs
+    updated_existing = n_new - actually_new
+    if updated_existing > 0:
+        print(f'Updated {updated_existing} existing entries.')
 
     # Report arXiv updates:
     if arxiv_updates > 0:
-        print(f"\nThere were {arxiv_updates} entries updated from ArXiv to "
-               "their peer-reviewed version.")
+        print(
+            f"\nThere were {arxiv_updates} entries updated from ArXiv to "
+            "their peer-reviewed version."
+        )
     if len(new_keys) > 0:
-        new_keys = [
-            f"  {old} -> {new}"
-            for old,new in new_keys
-            if old != new]
-        if len(new_keys) > 0:
-            print("These entries changed their key:\n" + "\n".join(new_keys))
+        print("These entries changed their key:")
+        for old_key,new_key in new_keys.items():
+            print(f'  {old_key} -> {new_key}')
+
+    if return_replacements:
+        return updated, new_keys
     return updated
 
 
-def update(update_keys=True, base=None):
+def update(update_keys=True, base=None, return_replacements=False):
     """
     Do an ADS query by bibcode for all entries that have an ADS bibcode.
     Replacing old entries with the new ones.  The main use of
     this function is to update arxiv version of articles.
 
     Parameters
     ----------
     update_keys: Bool
         If True, attempt to update keys of entries that were updated
         from arxiv to published versions.
     base: List of Bib() objects
         The bibfile entries to update.  If None, use the entries from
         the bibmanager database as base.
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
+
+    Returns
+    -------
+    reps: Dict
+        A dictionary of replaced key names.
     """
     if base is None:
         bibs = bm.load()
     else:
         bibs = base
 
     # Filter entries that have a bibcode and not frozen:
@@ -410,16 +438,21 @@
     dois = [
         bib.doi for bib in bibs
         if bib.bibcode is not None and not bib.freeze]
     tags = [
         bib.tags for bib in bibs
         if bib.bibcode is not None and not bib.freeze]
     # Query-replace:
-    bibs = add_bibtex(
-        bibcodes, keys, eprints, dois, update_keys, base, tags)
+    bibs, replacements = add_bibtex(
+        bibcodes, keys, eprints, dois, update_keys, base, tags,
+        return_replacements=True,
+    )
+
+    if return_replacements:
+        return bibs, replacements
     return bibs
 
 
 def key_update(key, bibcode, alternate_bibcode):
     r"""
     Update key with year and journal of arxiv version of a key.
```

### Comparing `bibmanager-1.4.8/bibmanager/bib_manager/__init__.py` & `bibmanager-1.4.9/bibmanager/bib_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/bib_manager/bib_manager.py` & `bibmanager-1.4.9/bibmanager/bib_manager/bib_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -513,50 +513,47 @@
 
     Parameters
     ----------
     bibs: List of Bib() objects
         Entries to filter.
     field: String
         Field to use for filtering ('doi', 'isbn', 'bibcode', or 'eprint').
+
+    Returns
+    -------
+    replacements: dict
+        A dictionary of {old:new} duplicated keys that have been removed.
     """
+    replacements = {}
     fieldlist = [
         getattr(bib,field) if getattr(bib,field) is not None else ""
-        for bib in bibs]
+        for bib in bibs
+    ]
     # No entries:
     if len(fieldlist) == 0:
-        return
+        return replacements
 
     ubib, uinv, counts = np.unique(
         fieldlist, return_inverse=True, return_counts=True)
     multis = np.where((counts > 1) & (ubib != ""))[0]
 
     # No duplicates:
     if len(multis) == 0:
-        return
+        return replacements
 
     removes = []
     for m in multis:
         all_indices = np.where(uinv == m)[0]
         entries = [bibs[i].content for i in all_indices]
 
         # Remove identical entries:
         uentries, uidx = np.unique(entries, return_index=True)
         indices = list(all_indices[uidx])
         removes += [idx for idx in all_indices if idx not in indices]
-        nbibs = len(uentries)
-        if nbibs == 1:
-            continue
-
-        # Pick peer-reviewed over ArXiv over non-ADS:
-        pubs = [bibs[i].published() for i in indices]
-        pubmax = np.amax(pubs)
-        removes += [idx for idx,pub in zip(indices,pubs) if pub <  pubmax]
-        indices  = [idx for idx,pub in zip(indices,pubs) if pub == pubmax]
-        nbibs = len(indices)
-        if nbibs == 1:
+        if len(uentries) == 1:
             continue
 
         # If field is isbn, check doi to differentiate chapters from same book:
         if field == 'isbn':
             dois = [
                 bibs[idx].doi if bibs[idx].doi is not None else ""
                 for idx in indices
@@ -564,33 +561,54 @@
             u_doi, doi_counts = np.unique(dois, return_counts=True)
             single_dois = u_doi[doi_counts==1]
             indices = [
                 idx
                 for idx,doi in zip(indices,dois)
                 if doi not in single_dois
             ]
-            nbibs = len(indices)
-            if nbibs <= 1:
+            if len(indices) <= 1:
                 continue
 
+        replace_indices = np.copy(indices)
+        # Pick peer-reviewed over ArXiv over non-ADS:
+        pubs = [bibs[i].published() for i in indices]
+        pubmax = np.amax(pubs)
+        removes += [idx for idx,pub in zip(indices,pubs) if pub <  pubmax]
+        indices  = [idx for idx,pub in zip(indices,pubs) if pub == pubmax]
+        if len(indices) == 1:
+            keep_key = bibs[indices[0]].key
+            for i in all_indices:
+                key = bibs[i].key
+                if key != keep_key:
+                    replacements[key] = keep_key
+            continue
+
         # Query the user:
+        nbibs = len(indices)
         labels = [idx + " ENTRY:\n" for idx in u.ordinal(np.arange(nbibs)+1)]
         display_bibs(labels, [bibs[i] for i in indices])
         s = u.req_input(
             f"Duplicate {field} field, []keep first, [2]second, "
             "[3]third, etc.: ",
             options=[""]+list(np.arange(nbibs)+1))
         if s == "":
-            indices.pop(0)
+            idx_keep = indices.pop(0)
         else:
-            indices.pop(int(s)-1)
+            idx_keep = indices.pop(int(s) - 1)
         removes += indices
 
+        keep_key = bibs[idx_keep].key
+        for i in replace_indices:
+            key = bibs[i].key
+            if key != keep_key:
+                replacements[key] = keep_key
+
     for idx in reversed(sorted(removes)):
         bibs.pop(idx)
+    return replacements
 
 
 def filter_field(bibs, new, field, take):
     """
     Filter duplicate entries by field between new and bibs.
     This routine modifies new removing the duplicates, and may modify
     bibs (depending on take argument).
@@ -643,30 +661,34 @@
             if s == "n":
                 bibs[idx].update_content(bib)
         removes.append(i)
     for idx in reversed(sorted(removes)):
         new.pop(idx)
 
 
-def read_file(bibfile=None, text=None):
+def read_file(bibfile=None, text=None, return_replacements=False):
     r"""
     Create a list of Bib() objects from a BibTeX file (.bib file).
 
     Parameters
     ----------
     bibfile: String
         Path to an existing .bib file.
     text: String
         Content of a .bib file (ignored if bibfile is not None).
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
 
     Returns
     -------
     bibs: List of Bib() objects
         List of Bib() objects of BibTeX entries in bibfile, sorted by
         Sort_author() fields.
+    reps: Dict
+        A dictionary of replaced key names.
 
     Examples
     --------
     >>> import bibmanager.bib_manager as bm
     >>> text = (
     >>>    "@misc{AASteamHendrickson2018aastex62,\n"
     >>>    "author = {{AAS Journals Team} and {Hendrickson}, Amy},\n"
@@ -678,15 +700,16 @@
     entries = []  # Store Lists of bibtex entries
     meta_info = []  # Meta information for each entry
 
     # Load a bib file:
     if bibfile is None and text is None:
         raise TypeError(
             "Missing input arguments for read_file(), at least "
-            "bibfile or text must be provided.")
+            "bibfile or text must be provided."
+        )
     if bibfile is not None:
         with open(bibfile, 'r', encoding='utf-8') as f:
             text = f.read()
 
     position = 0
     while True:
         start_pos = text.find('@', position)
@@ -724,30 +747,37 @@
         position = end_pos
 
     bibs = [
         Bib(entry, **meta)
         for entry,meta in zip(entries,meta_info)
     ]
 
-    remove_duplicates(bibs, "doi")
-    remove_duplicates(bibs, "isbn")
-    remove_duplicates(bibs, "bibcode")
-    remove_duplicates(bibs, "eprint")
+    nbibs_input = len(bibs)
+    reps = remove_duplicates(bibs, "doi")
+    reps.update(remove_duplicates(bibs, "isbn"))
+    reps.update(remove_duplicates(bibs, "bibcode"))
+    reps.update(remove_duplicates(bibs, "eprint"))
+    nbibs_output = len(bibs)
+    if nbibs_output != nbibs_input:
+        print(f'\nRemoved {nbibs_input-nbibs_output} duplicated entries.')
 
     # Check pathed-pdf meta values:
     for i,bib in enumerate(bibs):
         if bib.pdf is not None and os.path.dirname(bib.pdf) != '':
             filename = os.path.expanduser(bib.pdf)
             if not os.path.isfile(filename):
                 bibs[i].pdf = None
             else:
                 shutil.move(
                     os.path.expanduser(filename),
                     f"{u.BM_PDF()}{os.path.basename(filename)}")
                 bibs[i].pdf = os.path.basename(filename)
+
+    if return_replacements:
+        return sorted(bibs), reps
     return sorted(bibs)
 
 
 def save(entries):
     """
     Save list of Bib() entries into bibmanager pickle database.
 
@@ -895,17 +925,19 @@
         'https://pcubillos.github.io/bibmanager/\n\n']
     # Care not to overwrite user's bib files:
     if os.path.exists(bibfile):
         with open(bibfile, 'r', encoding='utf-8') as f:
             head = f.readline()
         if head.strip() != header[0].strip():
             path, bfile = os.path.split(os.path.realpath(bibfile))
+            today = str(datetime.date.today())
             shutil.copy(
-                bibfile, "".join(
-                [path, '/orig_', str(datetime.date.today()), '_', bfile]))
+                bibfile,
+                f'{path}/orig_{today}_{bfile}',
+            )
 
     with open(bibfile, 'w', encoding='utf-8') as f:
         f.writelines(header)
         for bib in entries:
             if meta:
                 f.write(bib.meta())
             f.write(bib.content)
@@ -1003,15 +1035,16 @@
             bibs[idx].update_content(bib)
         elif s == "a":
             keep[i] = True
     new = [bib for bib,keeper in zip(new,keep) if keeper]
 
     # Add all new entries and sort:
     bibs = sorted(bibs + new)
-    print(f"\nMerged {len(new)} new entries.")
+    if len(new) > 0:
+        print(f"\nMerged {len(new)} new entries.")
 
     if base is None:
         save(bibs)
         export(bibs, meta=True)
 
     return bibs
```

### Comparing `bibmanager-1.4.8/bibmanager/bib_manager/browser.py` & `bibmanager-1.4.9/bibmanager/bib_manager/browser.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/config_manager/config_manager.py` & `bibmanager-1.4.9/bibmanager/config_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/examples/aastex62.cls` & `bibmanager-1.4.9/bibmanager/examples/aastex62.cls`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/examples/apj_hyperref.bst` & `bibmanager-1.4.9/bibmanager/examples/apj_hyperref.bst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/examples/sample.bib` & `bibmanager-1.4.9/bibmanager/examples/sample.bib`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/examples/sample.tex` & `bibmanager-1.4.9/bibmanager/examples/sample.tex`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/examples/top-apj.tex` & `bibmanager-1.4.9/bibmanager/examples/top-apj.tex`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/latex_manager/latex_manager.py` & `bibmanager-1.4.9/bibmanager/latex_manager/latex_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,103 @@
 # Copyright (c) 2018-2023 Patricio Cubillos.
 # bibmanager is open-source software under the MIT license (see LICENSE).
 
 __all__ = [
+    'get_bibfile',
     'no_comments',
     'citations',
     'parse_subtex_files',
     'build_bib',
+    'update_keys',
     'clear_latex',
     'compile_latex',
     'compile_pdflatex',
 ]
 
+import datetime
 import os
 import re
+import shutil
 import subprocess
 import numpy as np
 
-from .. import bib_manager    as bm
+from .. import bib_manager as bm
 from .. import config_manager as cm
 from .. import utils as u
 
 
+class Replacer():
+    """
+    Object to keep track of comments and key changes in a .tex file
+    Used in update_keys() function.
+    """
+    def __init__(self, reps):
+        self.index = 0
+        self.reps = reps
+        self.comments = {}
+
+    def mask_comments(self, text):
+        self.index += 1
+        mask = f'BIBM_COMMENT_{self.index:06d}_'
+        self.comments[mask] = text.group()
+        return mask
+
+    def recover_comments(self, text):
+        for key, comment in self.comments.items():
+            text = text.replace(key, comment, 1)
+        return text
+
+    def replace(self, text):
+        refs = text.split(',')
+        citations = []
+        for ref in refs:
+            old_ref = ref.strip()
+            if old_ref in self.reps.keys():
+                new_ref = self.reps[old_ref]
+                ref = ref.replace(ref.strip(), new_ref)
+            citations.append(ref)
+        return ','.join(citations)
+
+
+def get_bibfile(texfile):
+    r"""
+    Find and extract the bibfile used by a .tex file.
+    This is done by looking for a '\bibliography{}' call.
+
+    Parameters
+    ----------
+    texfile: String
+        Name of an input tex file.
+
+    Returns
+    -------
+    bibfile: String
+        bib file referenced in texfile.
+    """
+    with open(texfile, 'r', encoding='utf-8') as f:
+        text = f.read()
+
+    # Start at the beginning:
+    beginning = text.find(r'\begin{document}')
+    if beginning > 0:
+        text = text[beginning:]
+
+    # Remove comments, go through recursive .tex files referenced in text:
+    text = parse_subtex_files(text)
+
+    # Extract bibfile name from texfile:
+    biblio = re.findall(r"\\bibliography{([^}]+)", text)
+    if len(biblio) == 0:
+        raise ValueError("No 'bibiliography' call found in tex file")
+    # Ensure explicit file extension in bibfile:
+    bibfile, extension = os.path.splitext(biblio[0].strip())
+    bibfile += '.bib'
+    return bibfile
+
+
 def no_comments(text):
     r"""
     Remove comments from tex file, partially inspired by this:
     https://stackoverflow.com/questions/2319019
 
     Parameters
     ----------
@@ -139,15 +212,16 @@
     # - The content of the curly braces.
     # With zero or more blanks in between each expression.
     p = re.compile(
         r"\\(?:defcitealias|nocite|cite|"
         r"(?:[Cc]ite(?:p|alp|t|alt|author|year|yearpar)\*?))"
         r"[\s]*(\[[^\]]*\])?"
         r"[\s]*(\[[^\]]*\])?"
-        r"[\s]*{([^}]+)")
+        r"[\s]*{([^}]+)"
+    )
     # Parse matches, do recursive call on the brakets content, yield keys:
     for left, right, cites in p.findall(text):
         # Remove blanks, strip outer commas:
         cites = "".join(cites.split()).strip(",")
 
         for cite in citations(left):
             yield cite
@@ -210,31 +284,29 @@
     path, texfile = os.path.split(os.path.realpath(texfile))
     # Remove extension:
     texfile, extension = os.path.splitext(texfile)
 
     if extension != ".tex":
         raise ValueError("Input file does not have a .tex extension.")
 
-    with open(f"{path}/{texfile}.tex", "r", encoding='utf-8') as f:
+    with open(f'{path}/{texfile}.tex', "r", encoding='utf-8') as f:
         tex = f.read()
 
     # Start at the beginning:
     beginning = tex.find(r'\begin{document}')
     if beginning > 0:
         tex = tex[beginning:]
 
     # Implemented into a separate function to get recursion rolling:
     tex = parse_subtex_files(tex)
 
     # Extract bibfile name from texfile:
     if bibfile is None:
-        biblio = re.findall(r"\\bibliography{([^}]+)", tex)
-        if len(biblio) == 0:
-            raise Exception("No 'bibiliography' call found in tex file.")
-        bibfile = f"{path}/{biblio[0].strip()}.bib"
+        bibfile = get_bibfile(f'{path}/{texfile}.tex')
+        bibfile = f'{path}/{bibfile}'
 
     # Extract citation keys from texfile:
     cites = [citation for citation in citations(tex)]
     tex_keys = np.unique(cites)
 
     # Collect BibTeX references from keys in database:
     bibs = bm.load()
@@ -247,14 +319,78 @@
 
     bibs = [bibs[db_keys.index(key)] for key in tex_keys[found]]
     bm.export(bibs, bibfile=bibfile)
 
     return missing
 
 
+def update_keys(texfile, key_replacements, is_main):
+    r"""
+    Update citation keys in a tex file according to the replace_dict.
+    Work out way recursively into sub-files.
+
+    Parameters
+    ----------
+    textfile: String
+        Path to an existing .tex file.
+    is_main: Bool
+        If True, ignore everything up to '\beging{document}' call.
+    """
+    with open(texfile, 'r', encoding='utf-8') as f:
+        tex = f.read()
+    if is_main:
+        beginning = tex.find(r'\begin{document}')
+    else:
+        beginning = 0
+    # Temporarily replace comments, keep a recod of them:
+    replacer = Replacer(key_replacements)
+    text = re.sub(r"\A%.*|[^\\]%.*", replacer.mask_comments, tex[beginning:])
+
+    # See citations() for an explanation of this pattern:
+    p = re.compile(
+        r"\\(?:defcitealias|nocite|cite|"
+        r"(?:[Cc]ite(?:p|alp|t|alt|author|year|yearpar)\*?))"
+        r"[\s]*(\[[^\]]*\])?"
+        r"[\s]*(\[[^\]]*\])?"
+        r"[\s]*{([^}]+)"
+    )
+    # Reconstruct text, replacing citations as needed:
+    new_text = tex[0:beginning]
+    start = 0
+    while True:
+        match = p.search(text, start)
+        if match is None:
+            new_text += text[start:]
+            break
+        # Text up to citations:
+        pos, _ = match.span(3)
+        new_text += text[start:pos]
+        new_text += replacer.replace(match.groups()[2])
+        start = match.end()
+
+    # Put comments back in:
+    new_text = replacer.recover_comments(new_text)
+
+    path, tfile = os.path.split(os.path.realpath(texfile))
+    today = str(datetime.date.today())
+    shutil.copy(
+        texfile,
+        f"{path}/orig_{today}_{tfile}",
+    )
+    with open(texfile, 'w', encoding='utf-8') as f:
+        f.write(new_text)
+
+    # Recursive calls into referenced .tex files:
+    p = re.compile(r"\\(?:input|include|subfile)[\s]*{([^}]+)")
+    for input_file in p.findall(tex):
+        input_file = os.path.realpath(input_file)
+        input_file, extension = os.path.splitext(input_file.strip())
+        update_keys(f'{input_file}.tex', key_replacements, is_main=False)
+
+
 def clear_latex(texfile):
     """
     Remove by-products of previous latex compilations.
 
     Parameters
     ----------
     texfile: String
```

### Comparing `bibmanager-1.4.8/bibmanager/pdf_manager/pdf_manager.py` & `bibmanager-1.4.9/bibmanager/pdf_manager/pdf_manager.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager/utils/utils.py` & `bibmanager-1.4.9/bibmanager/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/bibmanager.egg-info/PKG-INFO` & `bibmanager-1.4.9/bibmanager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibmanager
-Version: 1.4.8
+Version: 1.4.9
 Summary: A BibTeX manager for LaTeX projects
 Home-page: https://github.com/pcubillos/bibmanager
 Author: Patricio Cubillos
 Author-email: pcubillos@fulbrightmail.org
 License: MIT
 Description:
```

### Comparing `bibmanager-1.4.8/bibmanager.egg-info/SOURCES.txt` & `bibmanager-1.4.9/bibmanager.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 bibmanager/examples/top-apj.tex
 bibmanager/latex_manager/__init__.py
 bibmanager/latex_manager/latex_manager.py
 bibmanager/pdf_manager/__init__.py
 bibmanager/pdf_manager/pdf_manager.py
 bibmanager/utils/__init__.py
 bibmanager/utils/utils.py
+docs/.api.rst.swp
+docs/.bibtex.rst.swp
 docs/Makefile
 docs/ads.rst
 docs/api.rst
 docs/bibtex.rst
 docs/conf.py
 docs/contributing.rst
 docs/faq.rst
@@ -48,14 +50,15 @@
 docs/latex.rst
 docs/license.rst
 docs/logo_bibmanager.png
 docs/make.bat
 docs/pdf.rst
 docs/raycast_bibmanager_screenshot.png
 docs/search.gif
+tests/.test_cli.py.swp
 tests/conftest.py
 tests/test_ads.py
 tests/test_bib_manager.py
 tests/test_cli.py
 tests/test_config_manager.py
 tests/test_latex_manager.py
 tests/test_pdf_manager.py
```

### Comparing `bibmanager-1.4.8/docs/Makefile` & `bibmanager-1.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/ads.rst` & `bibmanager-1.4.9/docs/ads.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/api.rst` & `bibmanager-1.4.9/docs/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,49 +13,77 @@
 ______________________
 
 
 .. py:module:: bibmanager.bib_manager
 
 .. py:class:: Bib(entry, pdf=None, freeze=None, tags=[])
 
-.. code-block:: pycon
+    .. code-block:: pycon
 
-    Bibliographic-entry object.
+        Bibliographic-entry object.
 
-  .. code-block:: pycon
 
-    Create a Bib() object from given entry.
+        Create a Bib() object from given entry.
 
-    Parameters
-    ----------
-    entry: String
-        A bibliographic entry text.
-    pdf: String
-        Name of PDF file associated with this entry.
-    freeze: Bool
-        Flag that, if True, prevents the entry to be ADS-updated.
+        Parameters
+        ----------
+        entry: String
+            A bibliographic entry text.
+        pdf: String
+            Name of PDF file associated with this entry.
+        freeze: Bool
+            Flag that, if True, prevents the entry to be ADS-updated.
 
-    Examples
-    --------
-    >>> import bibmanager.bib_manager as bm
-    >>> entry = '''@Misc{JonesEtal2001scipy,
-              author = {Eric Jones and Travis Oliphant and Pearu Peterson},
-              title  = {{SciPy}: Open source scientific tools for {Python}},
-              year   = {2001},
-            }'''
-    >>> bib = bm.Bib(entry)
-    >>> print(bib.title)
-    SciPy: Open source scientific tools for Python
-    >>> for author in bib.authors:
-    >>>    print(author)
-    Author(last='Jones', first='Eric', von='', jr='')
-    Author(last='Oliphant', first='Travis', von='', jr='')
-    Author(last='Peterson', first='Pearu', von='', jr='')
-    >>> print(bib.sort_author)
-    Sort_author(last='jones', first='e', von='', jr='', year=2001, month=13)
+        Examples
+        --------
+        >>> import bibmanager.bib_manager as bm
+        >>> entry = '''@Misc{JonesEtal2001scipy,
+                  author = {Eric Jones and Travis Oliphant and Pearu Peterson},
+                  title  = {{SciPy}: Open source scientific tools for {Python}},
+                  year   = {2001},
+                }'''
+        >>> bib = bm.Bib(entry)
+        >>> print(bib.title)
+        SciPy: Open source scientific tools for Python
+        >>> for author in bib.authors:
+        >>>    print(author)
+        Author(last='Jones', first='Eric', von='', jr='')
+        Author(last='Oliphant', first='Travis', von='', jr='')
+        Author(last='Peterson', first='Pearu', von='', jr='')
+        >>> print(bib.sort_author)
+        Sort_author(last='jones', first='e', von='', jr='', year=2001, month=13)
+
+    .. py:method:: get_authors(format='short')
+    .. code-block:: pycon
+
+        wrapper for string representation for the author list.
+        See bib_manager.get_authors() for docstring.
+
+    .. py:method:: meta()
+    .. code-block:: pycon
+
+        String containing the non-None meta information.
+
+    .. py:method:: published()
+    .. code-block:: pycon
+
+        Published status according to the ADS bibcode field:
+            Return -1 if bibcode is None.
+            Return  0 if bibcode is arXiv.
+            Return  1 if bibcode is peer-reviewed journal.
+
+    .. py:method:: update_content(other)
+    .. code-block:: pycon
+
+        Update the bibtex content of self with that of other.
+
+    .. py:method:: update_key(new_key)
+    .. code-block:: pycon
+
+        Update key with new_key, making sure to also update content.
 
 .. py:function:: display_bibs(labels, bibs, meta=False)
 .. code-block:: pycon
 
     Display a list of bib entries on screen with flying colors.
 
     Parameters
@@ -127,14 +155,19 @@
     Parameters
     ----------
     bibs: List of Bib() objects
         Entries to filter.
     field: String
         Field to use for filtering ('doi', 'isbn', 'bibcode', or 'eprint').
 
+    Returns
+    -------
+    replacements: dict
+        A dictionary of {old:new} duplicated keys that have been removed.
+
 .. py:function:: filter_field(bibs, new, field, take)
 .. code-block:: pycon
 
     Filter duplicate entries by field between new and bibs.
     This routine modifies new removing the duplicates, and may modify
     bibs (depending on take argument).
 
@@ -149,31 +182,35 @@
     take: String
         Decision-making protocol to resolve conflicts when there are
         duplicated entries:
         'old': Take the database entry over new.
         'new': Take the new entry over the database.
         'ask': Ask user to decide (interactively).
 
-.. py:function:: read_file(bibfile=None, text=None)
+.. py:function:: read_file(bibfile=None, text=None, return_replacements=False)
 .. code-block:: pycon
 
     Create a list of Bib() objects from a BibTeX file (.bib file).
 
     Parameters
     ----------
     bibfile: String
         Path to an existing .bib file.
     text: String
         Content of a .bib file (ignored if bibfile is not None).
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
 
     Returns
     -------
     bibs: List of Bib() objects
         List of Bib() objects of BibTeX entries in bibfile, sorted by
         Sort_author() fields.
+    reps: Dict
+        A dictionary of replaced key names.
 
     Examples
     --------
     >>> import bibmanager.bib_manager as bm
     >>> text = (
     >>>    "@misc{AASteamHendrickson2018aastex62,\n"
     >>>    "author = {{AAS Journals Team} and {Hendrickson}, Amy},\n"
@@ -357,15 +394,15 @@
     ---------
     https://stackoverflow.com/questions/17317219/
     https://docs.python.org/3.6/library/subprocess.html
 
 .. py:function:: search(authors=None, year=None, title=None, key=None, bibcode=None, tags=None)
 .. code-block:: pycon
 
-    Search in bibmanager database by authors, year, or title keywords.
+    Search in bibmanager database by different fields/properties.
 
     Parameters
     ----------
     authors: String or List of strings
         An author name (or list of names) with BibTeX format (see parse_name()
         docstring).  To restrict search to a first author, prepend the
         '^' character to a name.
@@ -602,14 +639,30 @@
 
 bibmanager.latex_manager
 ________________________
 
 
 .. py:module:: bibmanager.latex_manager
 
+.. py:function:: get_bibfile(texfile)
+.. code-block:: pycon
+
+    Find and extract the bibfile used by a .tex file.
+    This is done by looking for a '\bibliography{}' call.
+
+    Parameters
+    ----------
+    texfile: String
+        Name of an input tex file.
+
+    Returns
+    -------
+    bibfile: String
+        bib file referenced in texfile.
+
 .. py:function:: no_comments(text)
 .. code-block:: pycon
 
     Remove comments from tex file, partially inspired by this:
     https://stackoverflow.com/questions/2319019
 
     Parameters
@@ -744,14 +797,27 @@
         bibliography call inside the tex file.
 
     Returns
     -------
     missing: List of strings
         List of the bibkeys not found in the bibmanager database.
 
+.. py:function:: update_keys(texfile, key_replacements, is_main)
+.. code-block:: pycon
+
+    Update citation keys in a tex file according to the replace_dict.
+    Work out way recursively into sub-files.
+
+    Parameters
+    ----------
+    textfile: String
+        Path to an existing .tex file.
+    is_main: Bool
+        If True, ignore everything up to '\beging{document}' call.
+
 .. py:function:: clear_latex(texfile)
 .. code-block:: pycon
 
     Remove by-products of previous latex compilations.
 
     Parameters
     ----------
@@ -898,15 +964,15 @@
     --------
     >>> import bibmanager.ads_manager as am
     >>> start = index = 0
     >>> query = 'author:"^cubillos, p" property:refereed'
     >>> results, nmatch = am.search(query, start=start)
     >>> display(results, start, index, rows, nmatch)
 
-.. py:function:: add_bibtex(input_bibcodes, input_keys, eprints=[], dois=[], update_keys=True, base=None, tags=None)
+.. py:function:: add_bibtex(input_bibcodes, input_keys, eprints=[], dois=[], update_keys=True, base=None, tags=None, return_replacements=False)
 .. code-block:: pycon
 
     Add bibtex entries from a list of ADS bibcodes, with specified keys.
     New entries will replace old ones without asking if they are
     duplicates.
 
     Parameters
@@ -923,19 +989,23 @@
         If True, attempt to update keys of entries that were updated
         from arxiv to published versions.
     base: List of Bib() objects
         If None, merge new entries into the bibmanager database.
         If not None, merge new entries into base.
     tags: Nested list of strings
         The list of tags for each input bibcode.
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
 
     Returns
     -------
     bibs: List of Bib() objects
         Updated list of BibTeX entries.
+    reps: Dict
+        A dictionary of replaced key names.
 
     Examples
     --------
     >>> import bibmanager.ads_manager as am
     >>> # A successful add call:
     >>> bibcodes = ['1925PhDT.........1P']
     >>> keys = ['Payne1925phdStellarAtmospheres']
@@ -950,29 +1020,36 @@
     >>> keys = ['Payne1925phdStellarAtmospheres', 'FolsomEtal2018mnrasHD219134']
     >>> am.add_bibtex(bibcodes, keys)
     >>> # A partially failing call will still add those that succeed:
     >>> bibcodes = ['1925PhDT.....X...1P', '2018MNRAS.481.5286F']
     >>> am.add_bibtex(bibcodes, keys)
     Warning: bibcode '1925PhDT.....X...1P' not found.
 
-.. py:function:: update(update_keys=True, base=None)
+.. py:function:: update(update_keys=True, base=None, return_replacements=False)
 .. code-block:: pycon
 
     Do an ADS query by bibcode for all entries that have an ADS bibcode.
     Replacing old entries with the new ones.  The main use of
     this function is to update arxiv version of articles.
 
     Parameters
     ----------
     update_keys: Bool
         If True, attempt to update keys of entries that were updated
         from arxiv to published versions.
     base: List of Bib() objects
         The bibfile entries to update.  If None, use the entries from
         the bibmanager database as base.
+    return_replacements: Bool
+        If True, also return a dictionary of replaced keys.
+
+    Returns
+    -------
+    reps: Dict
+        A dictionary of replaced key names.
 
 .. py:function:: key_update(key, bibcode, alternate_bibcode)
 .. code-block:: pycon
 
     Update key with year and journal of arxiv version of a key.
 
     This function will search and update the year in a key,
@@ -1256,31 +1333,53 @@
 .. py:function:: BM_PDF()
 .. code-block:: pycon
 
     Folder for PDF files of the BibTex entries
 
 .. py:class:: Author(last, first, von, jr)
 
-.. code-block:: pycon
+    .. code-block:: pycon
 
-    Author(last, first, von, jr)
+        Author(last, first, von, jr)
 
-  .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Initialize self.  See help(type(self)) for accurate signature.
+
+    .. py:method:: count(value, /)
+    .. code-block:: pycon
+
+        Return number of occurrences of value.
+
+    .. py:method:: index(value, start=0, stop=9223372036854775807, /)
+    .. code-block:: pycon
+
+        Return first index of value.
+
+        Raises ValueError if the value is not present.
 
 .. py:class:: Sort_author(last, first, von, jr, year, month)
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Sort_author(last, first, von, jr, year, month)
+
 
-    Sort_author(last, first, von, jr, year, month)
+        Initialize self.  See help(type(self)) for accurate signature.
 
-  .. code-block:: pycon
+    .. py:method:: count(value, /)
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Return number of occurrences of value.
+
+    .. py:method:: index(value, start=0, stop=9223372036854775807, /)
+    .. code-block:: pycon
+
+        Return first index of value.
+
+        Raises ValueError if the value is not present.
 
 .. py:function:: ignored(*exceptions)
 .. code-block:: pycon
 
     Context manager to ignore exceptions. Taken from here:
     https://www.youtube.com/watch?v=anrOzOapJ2E
 
@@ -1860,133 +1959,345 @@
         >>> style = prompt_toolkit.styles.style_from_pygments_cls(
         >>>     get_style_by_name('autumn'))
         >>> prompt_toolkit.print_formatted_text(
         >>>     PygmentsTokens(tokens), style=style)
         Title: Synthesis of the Elements in Stars
     
 
+.. py:function:: parse_search(input_text)
+.. code-block:: pycon
+
+    Parse field-value sets from an input string which is then passed
+    to bm.search().  The format is the same as in ADS and it should
+    be 'intuitive' given the auto-complete functionality.  However,
+    for purposes of documentation see the examples below.
+
+    Parameters
+    ----------
+    input_text: String
+        A user-input search string.
+
+    Returns
+    -------
+    matches: List of Bib() objects
+        Entries that match all input criteria.
+
+    Examples
+    --------
+    >>> # First-author: contain the '^' char and value in quotes:
+    >>> matches = u.parse_search('author:"^Payne, C"')
+    >>> # Author or Title: value should be in quotes:
+    >>> matches = u.parse_search('author:"Payne, C"')
+    >>> # Specific year:
+    >>> matches = u.parse_search('year: 1984')
+    >>> # Year range:
+    >>> matches = u.parse_search('year: 1984-2004')
+    >>> # Open-ended year range (starting from, up to):
+    >>> matches = u.parse_search('year: 1984-')
+    >>> matches = u.parse_search('year: -1984')
+    >>> # key, bibcode, and tags don't need quotes:
+    >>> matches = u.parse_search('key: Payne1925phdStellarAtmospheres')
+    >>> matches = u.parse_search('bibcode: 1925PhDT.........1P')
+    >>> matches = u.parse_search('tags: stars')
+    >>> # Certainly, multiple field can be combined:
+    >>> matches = u.parse_search('author:"Payne, C" year:1925-1930')
+
 .. py:class:: DynamicKeywordCompleter(key_words)
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Provide tab-completion for keys and words in corresponding key.
+
+
+        Initialize self.  See help(type(self)) for accurate signature.
+
+    .. py:method:: get_completions(document, complete_event)
+    .. code-block:: pycon
 
-    Provide tab-completion for keys and words in corresponding key.
+        Get right key/option completions.
 
-  .. code-block:: pycon
+    .. py:method:: get_completions_async(document: prompt_toolkit.document.Document, complete_event: prompt_toolkit.completion.base.CompleteEvent) -> AsyncGenerator[prompt_toolkit.completion.base.Completion, NoneType]
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Asynchronous generator for completions. (Probably, you won't have to
+        override this.)
+
+        Asynchronous generator of :class:`.Completion` objects.
 
 .. py:class:: DynamicKeywordSuggester()
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Give dynamic suggestions as in DynamicKeywordCompleter.
+
 
-    Give dynamic suggestions as in DynamicKeywordCompleter.
+        Initialize self.  See help(type(self)) for accurate signature.
 
-  .. code-block:: pycon
+    .. py:method:: get_suggestion(buffer, document)
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Return `None` or a :class:`.Suggestion` instance.
+
+        We receive both :class:`~prompt_toolkit.buffer.Buffer` and
+        :class:`~prompt_toolkit.document.Document`. The reason is that auto
+        suggestions are retrieved asynchronously. (Like completions.) The
+        buffer text could be changed in the meantime, but ``document`` contains
+        the buffer document like it was at the start of the auto suggestion
+        call. So, from here, don't access ``buffer.text``, but use
+        ``document.text`` instead.
+
+        :param buffer: The :class:`~prompt_toolkit.buffer.Buffer` instance.
+        :param document: The :class:`~prompt_toolkit.document.Document` instance.
+
+    .. py:method:: get_suggestion_async(buff: 'Buffer', document: prompt_toolkit.document.Document) -> Optional[prompt_toolkit.auto_suggest.Suggestion]
+    .. code-block:: pycon
+
+        Return a :class:`.Future` which is set when the suggestions are ready.
+        This function can be overloaded in order to provide an asynchronous
+        implementation.
 
 .. py:class:: KeyWordCompleter(words, bibs)
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Simple autocompletion on a list of words.
+
+        :param words: List of words or callable that returns a list of words.
+        :param ignore_case: If True, case-insensitive completion.
+        :param meta_dict: Optional dict mapping words to their meta-text. (This
+            should map strings to strings or formatted text.)
+        :param WORD: When True, use WORD characters.
+        :param sentence: When True, don't complete by comparing the word before the
+            cursor, but by comparing all the text before the cursor. In this case,
+            the list of words is just a list of strings, where each string can
+            contain spaces. (Can not be used together with the WORD option.)
+        :param match_middle: When True, match not only the start, but also in the
+                             middle of the word.
+        :param pattern: Optional compiled regex for finding the word before
+            the cursor to complete. When given, use this regex pattern instead of
+            default one (see document._FIND_WORD_RE)
+
 
-    Simple autocompletion on a list of words.
+        Initialize self.  See help(type(self)) for accurate signature.
 
-    :param words: List of words or callable that returns a list of words.
-    :param ignore_case: If True, case-insensitive completion.
-    :param meta_dict: Optional dict mapping words to their meta-text. (This
-        should map strings to strings or formatted text.)
-    :param WORD: When True, use WORD characters.
-    :param sentence: When True, don't complete by comparing the word before the
-        cursor, but by comparing all the text before the cursor. In this case,
-        the list of words is just a list of strings, where each string can
-        contain spaces. (Can not be used together with the WORD option.)
-    :param match_middle: When True, match not only the start, but also in the
-                         middle of the word.
-    :param pattern: Optional compiled regex for finding the word before
-        the cursor to complete. When given, use this regex pattern instead of
-        default one (see document._FIND_WORD_RE)
+    .. py:method:: get_completions(document, complete_event)
+    .. code-block:: pycon
 
-  .. code-block:: pycon
+        Get right key/option completions.
 
-    Initialize self.  See help(type(self)) for accurate signature.
+    .. py:method:: get_completions_async(document: prompt_toolkit.document.Document, complete_event: prompt_toolkit.completion.base.CompleteEvent) -> AsyncGenerator[prompt_toolkit.completion.base.Completion, NoneType]
+    .. code-block:: pycon
+
+        Asynchronous generator for completions. (Probably, you won't have to
+        override this.)
+
+        Asynchronous generator of :class:`.Completion` objects.
 
 .. py:class:: AutoSuggestCompleter()
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Give suggestions based on the words in WordCompleter.
+
+
+        Initialize self.  See help(type(self)) for accurate signature.
+
+    .. py:method:: get_suggestion(buffer, document)
+    .. code-block:: pycon
+
+        Return `None` or a :class:`.Suggestion` instance.
+
+        We receive both :class:`~prompt_toolkit.buffer.Buffer` and
+        :class:`~prompt_toolkit.document.Document`. The reason is that auto
+        suggestions are retrieved asynchronously. (Like completions.) The
+        buffer text could be changed in the meantime, but ``document`` contains
+        the buffer document like it was at the start of the auto suggestion
+        call. So, from here, don't access ``buffer.text``, but use
+        ``document.text`` instead.
 
-    Give suggestions based on the words in WordCompleter.
+        :param buffer: The :class:`~prompt_toolkit.buffer.Buffer` instance.
+        :param document: The :class:`~prompt_toolkit.document.Document` instance.
 
-  .. code-block:: pycon
+    .. py:method:: get_suggestion_async(buff: 'Buffer', document: prompt_toolkit.document.Document) -> Optional[prompt_toolkit.auto_suggest.Suggestion]
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Return a :class:`.Future` which is set when the suggestions are ready.
+        This function can be overloaded in order to provide an asynchronous
+        implementation.
 
 .. py:class:: AutoSuggestKeyCompleter()
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Give suggestions based on the words in WordCompleter.
+
+
+        Initialize self.  See help(type(self)) for accurate signature.
 
-    Give suggestions based on the words in WordCompleter.
+    .. py:method:: get_suggestion(buffer, document)
+    .. code-block:: pycon
 
-  .. code-block:: pycon
+        Return `None` or a :class:`.Suggestion` instance.
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        We receive both :class:`~prompt_toolkit.buffer.Buffer` and
+        :class:`~prompt_toolkit.document.Document`. The reason is that auto
+        suggestions are retrieved asynchronously. (Like completions.) The
+        buffer text could be changed in the meantime, but ``document`` contains
+        the buffer document like it was at the start of the auto suggestion
+        call. So, from here, don't access ``buffer.text``, but use
+        ``document.text`` instead.
+
+        :param buffer: The :class:`~prompt_toolkit.buffer.Buffer` instance.
+        :param document: The :class:`~prompt_toolkit.document.Document` instance.
+
+    .. py:method:: get_suggestion_async(buff: 'Buffer', document: prompt_toolkit.document.Document) -> Optional[prompt_toolkit.auto_suggest.Suggestion]
+    .. code-block:: pycon
+
+        Return a :class:`.Future` which is set when the suggestions are ready.
+        This function can be overloaded in order to provide an asynchronous
+        implementation.
 
 .. py:class:: LastKeyCompleter(key_words)
 
-.. code-block:: pycon
+    .. code-block:: pycon
 
-    Give completer options according to last key found in input.
+        Give completer options according to last key found in input.
 
-  .. code-block:: pycon
 
-    Parameters
-    ----------
-    key_words: Dict
-        Dictionary containing the available keys and the
-        set of words corresponding to each key.
-        An empty-string key denotes the default set of words to
-        show when no key is found in the input text.
+        Parameters
+        ----------
+        key_words: Dict
+            Dictionary containing the available keys and the
+            set of words corresponding to each key.
+            An empty-string key denotes the default set of words to
+            show when no key is found in the input text.
+
+    .. py:method:: get_completions(document, complete_event)
+    .. code-block:: pycon
+
+        Get right key/option completions, i.e., the set of possible
+        keys (except the latest key found in the input text) and the
+        set of words according to the latest key in the input text.
+
+    .. py:method:: get_completions_async(document: prompt_toolkit.document.Document, complete_event: prompt_toolkit.completion.base.CompleteEvent) -> AsyncGenerator[prompt_toolkit.completion.base.Completion, NoneType]
+    .. code-block:: pycon
+
+        Asynchronous generator for completions. (Probably, you won't have to
+        override this.)
+
+        Asynchronous generator of :class:`.Completion` objects.
 
 .. py:class:: LastKeySuggestCompleter()
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Give suggestions based on the keys and words in LastKeyCompleter.
 
-    Give suggestions based on the keys and words in LastKeyCompleter.
 
-  .. code-block:: pycon
+        Initialize self.  See help(type(self)) for accurate signature.
 
-    Initialize self.  See help(type(self)) for accurate signature.
+    .. py:method:: get_suggestion(buffer, document)
+    .. code-block:: pycon
+
+        Return `None` or a :class:`.Suggestion` instance.
+
+        We receive both :class:`~prompt_toolkit.buffer.Buffer` and
+        :class:`~prompt_toolkit.document.Document`. The reason is that auto
+        suggestions are retrieved asynchronously. (Like completions.) The
+        buffer text could be changed in the meantime, but ``document`` contains
+        the buffer document like it was at the start of the auto suggestion
+        call. So, from here, don't access ``buffer.text``, but use
+        ``document.text`` instead.
+
+        :param buffer: The :class:`~prompt_toolkit.buffer.Buffer` instance.
+        :param document: The :class:`~prompt_toolkit.document.Document` instance.
+
+    .. py:method:: get_suggestion_async(buff: 'Buffer', document: prompt_toolkit.document.Document) -> Optional[prompt_toolkit.auto_suggest.Suggestion]
+    .. code-block:: pycon
+
+        Return a :class:`.Future` which is set when the suggestions are ready.
+        This function can be overloaded in order to provide an asynchronous
+        implementation.
 
 .. py:class:: KeyPathCompleter(words, bibs)
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Simple autocompletion on a list of words.
+
+        :param words: List of words or callable that returns a list of words.
+        :param ignore_case: If True, case-insensitive completion.
+        :param meta_dict: Optional dict mapping words to their meta-text. (This
+            should map strings to strings or formatted text.)
+        :param WORD: When True, use WORD characters.
+        :param sentence: When True, don't complete by comparing the word before the
+            cursor, but by comparing all the text before the cursor. In this case,
+            the list of words is just a list of strings, where each string can
+            contain spaces. (Can not be used together with the WORD option.)
+        :param match_middle: When True, match not only the start, but also in the
+                             middle of the word.
+        :param pattern: Optional compiled regex for finding the word before
+            the cursor to complete. When given, use this regex pattern instead of
+            default one (see document._FIND_WORD_RE)
 
-    Simple autocompletion on a list of words.
 
-    :param words: List of words or callable that returns a list of words.
-    :param ignore_case: If True, case-insensitive completion.
-    :param meta_dict: Optional dict mapping words to their meta-text. (This
-        should map strings to strings or formatted text.)
-    :param WORD: When True, use WORD characters.
-    :param sentence: When True, don't complete by comparing the word before the
-        cursor, but by comparing all the text before the cursor. In this case,
-        the list of words is just a list of strings, where each string can
-        contain spaces. (Can not be used together with the WORD option.)
-    :param match_middle: When True, match not only the start, but also in the
-                         middle of the word.
-    :param pattern: Optional compiled regex for finding the word before
-        the cursor to complete. When given, use this regex pattern instead of
-        default one (see document._FIND_WORD_RE)
+        Initialize self.  See help(type(self)) for accurate signature.
 
-  .. code-block:: pycon
+    .. py:method:: get_completions(document, complete_event)
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Get right key/option/file completions.
+
+    .. py:method:: get_completions_async(document: prompt_toolkit.document.Document, complete_event: prompt_toolkit.completion.base.CompleteEvent) -> AsyncGenerator[prompt_toolkit.completion.base.Completion, NoneType]
+    .. code-block:: pycon
+
+        Asynchronous generator for completions. (Probably, you won't have to
+        override this.)
+
+        Asynchronous generator of :class:`.Completion` objects.
+
+    .. py:method:: path_completions(text)
+    .. code-block:: pycon
+
+        Slightly modified from PathCompleter.get_completions()
 
 .. py:class:: AlwaysPassValidator(bibs, toolbar_text='')
 
-.. code-block:: pycon
+    .. code-block:: pycon
+
+        Validator that always passes (using actually for bottom toolbar).
+
+
+        Initialize self.  See help(type(self)) for accurate signature.
+
+    .. py:method:: from_callable(validate_func: Callable[[str], bool], error_message: str = 'Invalid input', move_cursor_to_end: bool = False) -> 'Validator'
+    .. code-block:: pycon
+
+        Create a validator from a simple validate callable. E.g.:
+
+        .. code:: python
+
+            def is_valid(text):
+                return text in ['hello', 'world']
+            Validator.from_callable(is_valid, error_message='Invalid input')
+
+        :param validate_func: Callable that takes the input string, and returns
+            `True` if the input is valid input.
+        :param error_message: Message to be displayed if the input is invalid.
+        :param move_cursor_to_end: Move the cursor to the end of the input, if
+            the input is invalid.
+
+    .. py:method:: validate(document)
+    .. code-block:: pycon
+
+        Validate the input.
+        If invalid, this should raise a :class:`.ValidationError`.
 
-    Validator that always passes (using actually for bottom toolbar).
+        :param document: :class:`~prompt_toolkit.document.Document` instance.
 
-  .. code-block:: pycon
+    .. py:method:: validate_async(document: prompt_toolkit.document.Document) -> None
+    .. code-block:: pycon
 
-    Initialize self.  See help(type(self)) for accurate signature.
+        Return a `Future` which is set when the validation is ready.
+        This function can be overloaded in order to provide an asynchronous
+        implementation.
```

### Comparing `bibmanager-1.4.8/docs/bibtex.rst` & `bibmanager-1.4.9/docs/bibtex.rst`

 * *Files 1% similar despite different names*

```diff
@@ -715,36 +715,38 @@
 --------------------------------------------------------------------
 
 .. _cleanup:
 
 cleanup
 -------
 
-Clean up a bibtex file of duplicates and outdated entries.
+Clean up a bibtex or latex file of duplicates and outdated entries.
 
 **Usage**
 
 .. code-block:: shell
 
   bibm cleanup [-h] [-ads] bibfile
 
 **Description**
 
-| Clean up a BibTeX file by removing duplicates, sorting the entries,
+| Clean up a BibTeX (.bib) or LaTeX (.tex) file by removing duplicates,
+  sorting the entries,
   and (if requested) updating the entries by cross-checking against
   the ADS database.  All of this is done independently of the
-  ``bibmanager`` database.  The original file will be preserved by
+  ``bibmanager`` database.  The original files will be preserved by
   prepending the string '*orig\_yyyy\_mm\_dd\_*' with the
   corresponding date.
 | *(New since version 1.1.2)*
 
 **Options**
 
 | **bibfile**
-|       Path to an existing BibTeX file.
+|       Path to an existing .tex or .bib file.
+|       *(New since version 1.4.9 this can also update .tex files)*
 | **-ads**
 |       Update the bibfile entries cross-checking against the ADS database.
 | **-h, -\\-help**
 |       Show this help message and exit.
 
 **Examples**
 
@@ -752,14 +754,18 @@
 
   # Remove duplicates and sort:
   bibm cleanup file.bib
 
   # Remove duplicates, update ADS entries, and sort:
   bibm cleanup file.bib -ads
 
+  # Remove duplicates, update ADS entries, and sort a .tex file
+  # (and also its .bib file and other referenced .tex files in the main .tex file)
+  bibm cleanup file.tex -ads
+
 --------------------------------------------------------------------
 
 .. _config:
 
 config
 ------
```

### Comparing `bibmanager-1.4.8/docs/conf.py` & `bibmanager-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/contributing.rst` & `bibmanager-1.4.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/faq.rst` & `bibmanager-1.4.9/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/fetch.gif` & `bibmanager-1.4.9/docs/fetch.gif`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/getstarted.rst` & `bibmanager-1.4.9/docs/getstarted.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/index.rst` & `bibmanager-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/infograph.png` & `bibmanager-1.4.9/docs/infograph.png`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/latex.rst` & `bibmanager-1.4.9/docs/latex.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/license.rst` & `bibmanager-1.4.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/logo_bibmanager.png` & `bibmanager-1.4.9/docs/logo_bibmanager.png`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/make.bat` & `bibmanager-1.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/pdf.rst` & `bibmanager-1.4.9/docs/pdf.rst`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/raycast_bibmanager_screenshot.png` & `bibmanager-1.4.9/docs/raycast_bibmanager_screenshot.png`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/docs/search.gif` & `bibmanager-1.4.9/docs/search.gif`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/setup.py` & `bibmanager-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/tests/conftest.py` & `bibmanager-1.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/tests/test_ads.py` & `bibmanager-1.4.9/tests/test_ads.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,22 +132,26 @@
     nmatch = 4
     am.display(results, start, index, rows, nmatch, short=True)
     captured = capsys.readouterr()
     expected_output = '\r\nTitle: On the Carbon-to-oxygen Ratio Measurement in nearby Sun-like Stars:\r\n    Implications for Planet Formation and the Determination of Stellar\r\n    Abundances\r\nAuthors: Fortney, Jonathan J.\r\nADS URL: https://ui.adsabs.harvard.edu/abs/2012ApJ...747L..27F\r\nbibcode: 2012ApJ...747L..27F\r\n\nShowing entries 4--4 out of 4 matches.\n'
     assert captured.out == expected_output
 
 
+@pytest.mark.skip(reason='TBD')
+def test_display_no_author_entry(capsys, mock_init, ads_entries):
+    pass
+
+
 def test_add_bibtex_success(capsys, reqs, mock_init):
     captured = capsys.readouterr()
     bibcodes = ['1925PhDT.........1P']
     keys = ['Payne1925phdStellarAtmospheres']
     am.add_bibtex(bibcodes, keys)
     captured = capsys.readouterr()
-    assert captured.out == "\nMerged 1 new entries.\n" \
-                           "(Not counting updated references)\n"
+    assert captured.out == "\nMerged 1 new entries.\n"
     loaded_bibs = bm.load()
     assert len(loaded_bibs) == 1
     assert loaded_bibs[0].content == \
 """@PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
@@ -183,26 +187,25 @@
 There were bibcodes unmatched or not found in ADS:
  - 1925PhDT.....X...1P
 
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 
 
 Merged 1 new entries.
-(Not counting updated references)\n"""
+"""
 
 
 def test_add_bibtex_with_tags(capsys, reqs, mock_init):
     captured = capsys.readouterr()
     bibcodes = ['1925PhDT.........1P']
     keys = ['Payne1925phdStellarAtmospheres']
     tags = [['stars']]
     am.add_bibtex(bibcodes, keys, tags=tags)
     captured = capsys.readouterr()
-    assert captured.out == "\nMerged 1 new entries.\n" \
-                           "(Not counting updated references)\n"
+    assert captured.out == "\nMerged 1 new entries.\n"
     loaded_bibs = bm.load()
     assert len(loaded_bibs) == 1
     assert repr(loaded_bibs[0]) == \
 """tags: stars
 @PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
```

### Comparing `bibmanager-1.4.8/tests/test_bib_manager.py` & `bibmanager-1.4.9/tests/test_bib_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,31 +540,35 @@
     expected_capture = '\r\n::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::\r\n@ARTICLE{Shapley1918apjDistanceGlobularClusters,\r\n   author = {{Shapley}, H.},\r\n    title = "{Studies based on the colors and magnitudes in stellar clusters. VII. The distances, distribution in space, and dimensions of 69 globular clusters.}",\r\n  journal = {\\apj},\r\n     year = 1918,\r\n    month = oct,\r\n   volume = 48,\r\n      doi = {10.1086/142423},\r\n   adsurl = {http://adsabs.harvard.edu/abs/1918ApJ....48..154S},\r\n  adsnote = {Provided by the SAO/NASA Astrophysics Data System}\r\n}\r\n\r\npdf: Slipher1913.pdf\r\n@ARTICLE{Slipher1913lobAndromedaRarialVelocity,\r\n       author = {{Slipher}, V.~M.},\r\n        title = "{The radial velocity of the Andromeda Nebula}",\r\n      journal = {Lowell Observatory Bulletin},\r\n     keywords = {GALAXIES: MOTION IN LINE OF SIGHT, ANDROMEDA GALAXY},\r\n         year = 1913,\r\n        month = Jan,\r\n       volume = {1},\r\n        pages = {56-57},\r\n       adsurl = {https://ui.adsabs.harvard.edu/abs/1913LowOB...2...56S},\r\n      adsnote = {Provided by the SAO/NASA Astrophysics Data System}\r\n}\r\n\r\n'
     assert captured.out == expected_capture
 
 
 def test_remove_duplicates_no_duplicates(bibs):
     # No duplicates, no removal:
     my_bibs = [bibs['beaulieu_apj'], bibs['stodden']]
-    bm.remove_duplicates(my_bibs, "doi")
+    dups = bm.remove_duplicates(my_bibs, "doi")
     assert len(my_bibs) == 2
-
+    assert len(dups) == 0
 
 def test_remove_duplicates_identical(bibs):
     # Identical entries:
     my_bibs = [bibs["beaulieu_apj"], bibs["beaulieu_apj"]]
-    bm.remove_duplicates(my_bibs, "doi")
+    dups = bm.remove_duplicates(my_bibs, "doi")
     assert my_bibs == [bibs["beaulieu_apj"]]
+    assert len(dups) == 0
 
 
 def test_remove_duplicates_diff_published(bibs):
     # Duplicate, differente published status
     my_bibs = [bibs["beaulieu_apj"], bibs["beaulieu_arxiv"]]
-    bm.remove_duplicates(my_bibs, "eprint")
+    dups = bm.remove_duplicates(my_bibs, "eprint")
     assert len(my_bibs) == 1
     assert my_bibs == [bibs["beaulieu_apj"]]
+    assert dups == {
+        'BeaulieuEtal2010arxivGJ436b': 'BeaulieuEtal2011apjGJ436bMethane',
+    }
 
 
 @pytest.mark.parametrize('mock_input', [['2']], indirect=True)
 def test_remove_duplicates_query(bibs, mock_input, mock_init):
     # Query-solve duplicate:
     my_bibs = [bibs["beaulieu_arxiv"], bibs["beaulieu_arxiv_dup"]]
     bm.remove_duplicates(my_bibs, "eprint")
@@ -680,14 +684,24 @@
 
 def test_read_file_ignore_comment_no_commas(mock_init):
     text = """@Comment{jabref-meta: databaseType:biblatex;}"""
     bibs = bm.read_file(text=text)
     assert len(bibs) == 0
 
 
+@pytest.mark.skip(reason='TBD')
+def test_read_file_replacements(mock_init):
+    bibs, reps = bm.read_file(
+        u.ROOT+'examples/sample.bib',
+        return_replacements=True,
+    )
+    assert len(bibs) == nentries
+    assert reps == {}
+
+
 def test_read_file_meta():
     with open(u.ROOT+'examples/sample.bib') as f:
        text = f.read()
     # prepend meta info before first entry:
     text = 'freeze\npdf: file.pdf\n'+ text
     bibs = bm.read_file(text=text)
 
@@ -887,15 +901,15 @@
     captured = capfd.readouterr()
     assert captured.out == f"\nMerged {nentries} new entries.\n"
 
 
 def test_merge_no_new(capfd, bibs, mock_init_sample):
     bm.merge(new=[bibs['hunter']])
     captured = capfd.readouterr()
-    assert captured.out == "\nMerged 0 new entries.\n"
+    assert captured.out == ""
 
 
 def test_merge_base(bibs):
     merged = bm.merge(new=[bibs['hunter']], base=[bibs['stodden']])
     assert len(merged) == 2
     assert merged[0] == bibs['hunter']
     assert merged[1] == bibs['stodden']
```

### Comparing `bibmanager-1.4.8/tests/test_cli.py` & `bibmanager-1.4.9/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,14 +426,24 @@
     sys.argv = "bibm export my_file.tex".split()
     cli.main()
     captured = capsys.readouterr()
     assert captured.out == \
         "\nError: Invalid file extension ('.tex'), must be '.bib' or '.bbl'.\n"
 
 
+@pytest.mark.skip(reason='TBD')
+def test_cli_cleanup_bib():
+    pass
+
+
+@pytest.mark.skip(reason='TBD')
+def test_cli_cleanup_tex():
+    pass
+
+
 def test_cli_config_display(capsys, mock_init_sample):
     sys.argv = "bibm config".split()
     cli.main()
     captured = capsys.readouterr()
     assert captured.out == (
         "\nbibmanager configuration file:\n"
         "PARAMETER    VALUE\n"
@@ -572,16 +582,15 @@
 
 def test_cli_ads_add_with_bibcode_key(capsys, reqs, mock_init):
     sys.argv = (
         'bibm ads-add '
         '1925PhDT.........1P Payne1925phdStellarAtmospheres').split()
     cli.main()
     captured = capsys.readouterr()
-    assert captured.out == \
-        "\nMerged 1 new entries.""\n(Not counting updated references)\n"""
+    assert captured.out == "\nMerged 1 new entries.\n"
     bibs = bm.load()
     assert len(bibs) == 1
     assert repr(bibs[0]) == \
 """@PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
@@ -595,16 +604,15 @@
 
 def test_cli_ads_add_with_bibcode_key_1tag(capsys, reqs, mock_init):
     sys.argv = (
         'bibm ads-add '
         '1925PhDT.........1P Payne1925phdStellarAtmospheres thesis').split()
     cli.main()
     captured = capsys.readouterr()
-    assert captured.out == \
-        "\nMerged 1 new entries.""\n(Not counting updated references)\n"""
+    assert captured.out == "\nMerged 1 new entries.\n"
     assert repr(bm.load()[0]) == \
 """tags: thesis
 @PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
        school = {RADCLIFFE COLLEGE.},
@@ -618,16 +626,15 @@
 def test_cli_ads_add_with_bibcode_key_tags(capsys, reqs, mock_init):
     sys.argv = (
         'bibm ads-add '
         '1925PhDT.........1P Payne1925phdStellarAtmospheres '
         'thesis stars').split()
     cli.main()
     captured = capsys.readouterr()
-    assert captured.out == \
-        "\nMerged 1 new entries.""\n(Not counting updated references)\n"""
+    assert captured.out == "\nMerged 1 new entries.\n"
     assert repr(bm.load()[0]) == \
 """tags: thesis stars
 @PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
        school = {RADCLIFFE COLLEGE.},
@@ -643,17 +650,15 @@
     [['1925PhDT.........1P Payne1925phdStellarAtmospheres']],
     indirect=True)
 def test_cli_ads_add_prompt_bibcode_key(capsys, reqs, mock_prompt, mock_init):
     sys.argv = 'bibm ads-add'.split()
     cli.main()
     captured = capsys.readouterr()
     # Screen output:
-    assert captured.out == (
-        ads_add_prompt
-        + "\nMerged 1 new entries.\n(Not counting updated references)\n")
+    assert captured.out == ads_add_prompt + "\nMerged 1 new entries.\n"
     # Check that entry is in database:
     bibs = bm.load()
     assert len(bibs) == 1
     assert repr(bibs[0]) == \
 """@PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
@@ -671,17 +676,15 @@
     [['1925PhDT.........1P Payne1925phdStellarAtmospheres thesis']],
     indirect=True)
 def test_cli_ads_add_prompt_1tag(capsys, reqs, mock_prompt, mock_init):
     sys.argv = 'bibm ads-add'.split()
     cli.main()
     captured = capsys.readouterr()
     # Screen output:
-    assert captured.out == (
-        ads_add_prompt
-        + "\nMerged 1 new entries.\n(Not counting updated references)\n")
+    assert captured.out == ads_add_prompt + "\nMerged 1 new entries.\n"
     # Check that entry is in database:
     assert repr(bm.load()[0]) == \
 """tags: thesis
 @PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
@@ -698,17 +701,15 @@
     [['1925PhDT.........1P Payne1925phdStellarAtmospheres thesis stars']],
     indirect=True)
 def test_cli_ads_add_prompt_tags(capsys, reqs, mock_prompt, mock_init):
     sys.argv = 'bibm ads-add'.split()
     cli.main()
     captured = capsys.readouterr()
     # Screen output:
-    assert captured.out == (
-        ads_add_prompt
-        + "\nMerged 1 new entries.\n(Not counting updated references)\n")
+    assert captured.out == ads_add_prompt + "\nMerged 1 new entries.\n"
     # Check that entry is in database:
     assert repr(bm.load()[0]) == \
 """tags: thesis stars
 @PHDTHESIS{Payne1925phdStellarAtmospheres,
        author = {{Payne}, Cecilia Helena},
         title = "{Stellar Atmospheres; a Contribution to the Observational Study of High Temperature in the Reversing Layers of Stars.}",
      keywords = {Astronomy},
@@ -727,17 +728,15 @@
     indirect=True)
 def test_cli_ads_add_prompt_multiline_no_tags(
         capsys, reqs, mock_prompt, mock_init):
     sys.argv = 'bibm ads-add'.split()
     cli.main()
     captured = capsys.readouterr()
     # Screen output:
-    assert captured.out == (
-        ads_add_prompt
-        + "\nMerged 2 new entries.\n(Not counting updated references)\n")
+    assert captured.out == ads_add_prompt + "\nMerged 2 new entries.\n"
     # Check that entries are in database:
     bibs = bm.load()
     assert len(bibs) == 2
     assert repr(bibs[0]) == \
 """@ARTICLE{BurbidgeEtal1957rvmpStellarSynthesis,
        author = {{Burbidge}, E. Margaret and {Burbidge}, G.~R. and {Fowler}, William A. and {Hoyle}, F.},
         title = "{Synthesis of the Elements in Stars}",
@@ -771,17 +770,15 @@
     indirect=True)
 def test_cli_ads_add_prompt_multiline_with_tags(
         capsys, reqs, mock_prompt, mock_init):
     sys.argv = 'bibm ads-add'.split()
     cli.main()
     captured = capsys.readouterr()
     # Screen output:
-    assert captured.out == (
-        ads_add_prompt
-        + "\nMerged 2 new entries.\n(Not counting updated references)\n")
+    assert captured.out == ads_add_prompt + "\nMerged 2 new entries.\n"
     # Check that entries are in database:
     bibs = bm.load()
     assert len(bibs) == 2
     assert repr(bibs[0]) == \
 """tags: stars
 @ARTICLE{BurbidgeEtal1957rvmpStellarSynthesis,
        author = {{Burbidge}, E. Margaret and {Burbidge}, G.~R. and {Fowler}, William A. and {Hoyle}, F.},
```

### Comparing `bibmanager-1.4.8/tests/test_config_manager.py` & `bibmanager-1.4.9/tests/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/tests/test_latex_manager.py` & `bibmanager-1.4.9/tests/test_latex_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,66 @@
 import pytest
 import pathlib
 
 import numpy as np
 from conftest import cd
 
 import bibmanager.utils as u
-import bibmanager.bib_manager   as bm
+import bibmanager.bib_manager as bm
 import bibmanager.latex_manager as lm
 
 
+def test_get_bibfile_with_extension(tmp_path):
+    os.chdir(tmp_path)
+    texfile = f'{tmp_path}/texfile.tex'
+    text = r"""
+        \begin{document}
+        Hello, this is latex.
+        \bibliography{bibfile.bib}
+        \end{document}
+        """
+    with open(texfile, 'w') as f:
+        f.write(text)
+
+    bibfile = lm.get_bibfile(texfile)
+    assert bibfile == 'bibfile.bib'
+
+
+def test_get_bibfile_no_extension(tmp_path):
+    os.chdir(tmp_path)
+    texfile = f'{tmp_path}/texfile.tex'
+    text = r"""
+        \begin{document}
+        Hello, this is latex.
+        \bibliography{bibfile}
+        \end{document}
+        """
+    with open(texfile, 'w') as f:
+        f.write(text)
+
+    bibfile = lm.get_bibfile(texfile)
+    assert bibfile == 'bibfile.bib'
+
+
+def test_get_bibfile_no_bibliography(tmp_path):
+    os.chdir(tmp_path)
+    texfile = f'{tmp_path}/texfile.tex'
+    text = r"""
+        \begin{document}
+        Hello, this is latex.
+        \end{document}
+        """
+    with open(texfile, 'w') as f:
+        f.write(text)
+
+    error = "No 'bibiliography' call found in tex file"
+    with pytest.raises(ValueError, match=error):
+        bibfile = lm.get_bibfile(texfile)
+
+
 def test_no_comments():
     assert lm.no_comments("") == ""
     assert lm.no_comments("Hello world.") == "Hello world."
     assert lm.no_comments("inline comment % comment") == "inline comment"
     assert lm.no_comments("% comment line.") == ""
     assert lm.no_comments("percentage \\%") == "percentage \\%"
     # If first line is comment, '\n' stays:
@@ -202,23 +250,28 @@
     # Check content:
     np.testing.assert_array_equal(missing, np.array(["MissingEtal2019"]))
     bibs = bm.read_file(bibfile)
     assert len(bibs) == 1
     assert "Astropycollab2013aaAstropy" in bibs[0].key
 
 
-def test_build_raise(mock_init):
+def test_build_bib_raise(mock_init):
     bm.merge(u.HOME+"examples/sample.bib")
     with open(u.HOME+"examples/mock_file.tex", "w") as f:
         f.write("\\cite{Astropycollab2013aaAstropy}")
-    with pytest.raises(Exception,
-             match="No 'bibiliography' call found in tex file."):
+    match = "No 'bibiliography' call found in tex file"
+    with pytest.raises(Exception, match=match):
         lm.build_bib(u.HOME+"examples/mock_file.tex")
 
 
+@pytest.mark.skip(reason="TBD")
+def test_update_keys():
+    pass
+
+
 def test_clear_latex(mock_init):
     # Mock some 'latex output' files:
     pathlib.Path(u.HOME+"examples/sample.pdf").touch()
     pathlib.Path(u.HOME+"examples/sample.ps").touch()
     pathlib.Path(u.HOME+"examples/sample.bbl").touch()
     pathlib.Path(u.HOME+"examples/sample.dvi").touch()
     pathlib.Path(u.HOME+"examples/sample.out").touch()
```

### Comparing `bibmanager-1.4.8/tests/test_pdf_manager.py` & `bibmanager-1.4.9/tests/test_pdf_manager.py`

 * *Files identical despite different names*

### Comparing `bibmanager-1.4.8/tests/test_utils.py` & `bibmanager-1.4.9/tests/test_utils.py`

 * *Files identical despite different names*


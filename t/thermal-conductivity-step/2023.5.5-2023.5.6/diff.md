# Comparing `tmp/thermal_conductivity_step-2023.5.5.tar.gz` & `tmp/thermal_conductivity_step-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thermal_conductivity_step-2023.5.5.tar", last modified: Fri May  5 15:15:35 2023, max compression
+gzip compressed data, was "thermal_conductivity_step-2023.5.6.tar", last modified: Sat May  6 16:54:56 2023, max compression
```

## Comparing `thermal_conductivity_step-2023.5.5.tar` & `thermal_conductivity_step-2023.5.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.985939 thermal_conductivity_step-2023.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9712 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.989939 thermal_conductivity_step-2023.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/tests/test_thermal_conductivity_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 15:15:34.997939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18589 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    27619 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step/tk_thermal_conductivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:34.993939 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 15:15:34.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:05.000000 thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-05-05 15:14:52.000000 thermal_conductivity_step-2023.5.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.444479 thermal_conductivity_step-2023.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9712 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.448479 thermal_conductivity_step-2023.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/tests/test_thermal_conductivity_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18612 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28749 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step/tk_thermal_conductivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:54:56.452479 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 16:54:56.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:54:45.000000 thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-05-06 16:54:40.000000 thermal_conductivity_step-2023.5.6/versioneer.py
```

### Comparing `thermal_conductivity_step-2023.5.5/CONTRIBUTING.rst` & `thermal_conductivity_step-2023.5.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/HISTORY.rst` & `thermal_conductivity_step-2023.5.6/HISTORY.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2023.5.6 -- Bugfix
+    * Fixed an error handling Nan's and Inf's that caused a crash
+    * Added the predictions from the derivatives of the Helfand moments to the output to
+      give a better feel for the quality of the results.
+      
 2023.5.5 -- Improved analysis
     * Considerable improvements to the analysis, results now seem solid
     * Fixed issues with fitting the linear portion of the Helfand moments
     * Added plot of the slope from the Helfand moments, which is similar to the
       Green-Kubo integral.
     * Cleaned up both the output and graphs.
```

### Comparing `thermal_conductivity_step-2023.5.5/LICENSE` & `thermal_conductivity_step-2023.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/PKG-INFO` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thermal_conductivity_step
-Version: 2023.5.5
+Name: thermal-conductivity-step
+Version: 2023.5.6
 Summary: A SEAMM plug-in for Thermal Conductivity
 Home-page: https://github.com/molssi-seamm/thermal_conductivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -81,14 +81,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.6 -- Bugfix
+    * Fixed an error handling Nan's and Inf's that caused a crash
+    * Added the predictions from the derivatives of the Helfand moments to the output to
+      give a better feel for the quality of the results.
+      
 2023.5.5 -- Improved analysis
     * Considerable improvements to the analysis, results now seem solid
     * Fixed issues with fitting the linear portion of the Helfand moments
     * Added plot of the slope from the Helfand moments, which is similar to the
       Green-Kubo integral.
     * Cleaned up both the output and graphs.
```

### Comparing `thermal_conductivity_step-2023.5.5/README.rst` & `thermal_conductivity_step-2023.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/Makefile` & `thermal_conductivity_step-2023.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/SEAMM Inverted 288x181.png` & `thermal_conductivity_step-2023.5.6/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/SEAMM logo.png` & `thermal_conductivity_step-2023.5.6/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo.png` & `thermal_conductivity_step-2023.5.6/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/molssi_main_logo_inverted_white.png` & `thermal_conductivity_step-2023.5.6/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/molssi_square.png` & `thermal_conductivity_step-2023.5.6/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/_static/nsf.png` & `thermal_conductivity_step-2023.5.6/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/conf.py` & `thermal_conductivity_step-2023.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/developer_guide/installation.rst` & `thermal_conductivity_step-2023.5.6/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/getting_started/index.rst` & `thermal_conductivity_step-2023.5.6/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/index.rst` & `thermal_conductivity_step-2023.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/docs/make.bat` & `thermal_conductivity_step-2023.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/setup.py` & `thermal_conductivity_step-2023.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/__init__.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/__init__.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/analysis.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         err = np.sqrt(np.diag(pcov)).tolist()
         a = [popt[0], popt[2]]
         a_err = [err[0], err[2]]
         tau = [popt[1], popt[3]]
         tau_err = [err[1], err[3]]
         kappa = a[0] + a[1]
         kappa_err = a_err[0] + a_err[1]
-        if kappa > 2 * a1:  # Shouldn't change this much!
+        if kappa < 0 or abs(kappa) > 2 * abs(a1):  # Shouldn't change this much!
             err = np.sqrt(np.diag(pcov1)).tolist()
             a = [popt1[0]]
             a_err = [err[0]]
             tau = [popt1[1]]
             tau_err = [err[1]]
             kappa = a[0]
             kappa_err = a_err[0]
```

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/data/references.bib` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/metadata.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/metadata.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,31 @@
 path = Path(pkg_resources.resource_filename(__name__, "data/"))
 csv_file = path / "properties.csv"
 if path.exists():
     molsystem.add_properties_from_file(csv_file)
 
 
 def fmt_err(value, err, precision=2):
-    decimals = -ceil(log10(err)) + precision
-    if decimals < 0:
-        decimals = 0
-    fmt = f".{decimals}f"
-    e = f"{err:{fmt}}"
-    v = f"{value:{fmt}}"
+    try:
+        decimals = -ceil(log10(err)) + precision
+    except Exception:
+        e = "--"
+        try:
+            v = f"{value:.2f}"
+        except Exception:
+            v = value
+    else:
+        if decimals < 0:
+            decimals = 0
+        fmt = f".{decimals}f"
+        e = f"{err:{fmt}}"
+        try:
+            v = f"{value:{fmt}}"
+        except Exception:
+            v = value
     return v, e
 
 
 class ThermalConductivity(seamm.Node):
     """
     The non-graphical part of a Thermal Conductivity step in a flowchart.
 
@@ -442,42 +453,61 @@
                     a,
                     a_err,
                     tau,
                     tau_err,
                     tf,
                     yf,
                 ) = fit_green_kubo_integral(slope, x, sigma=err)
-                # print(f"{kappa=} {tau=}")
                 fit0.append(
                     {
                         "kappa": kappa,
                         "stderr": kappa_err,
                         "xs": tf,
                         "ys": yf,
                         "a": a,
                         "a_err": a_err,
                         "tau": tau,
                         "tau_err": tau_err,
                     }
                 )
+                v, e = fmt_err(kappa, 2 * kappa_err)
+                if style == "1-line":
+                    if i == 0:
+                        table["Run"].append(len(self.V))
+                    alpha = self.tensor_labels[i][0]
+                    table["K" + alpha].append(v)
+                    table["e" + alpha].append(e)
+                elif style == "full":
+                    table["Method"].append("Helfand Derivative" if i == 0 else "")
+                    table["Dir"].append(self.tensor_labels[i][0])
+                    table["Kappa"].append(v)
+                    table["±"].append("±")
+                    table["95%"].append(e)
+                    table["Units"].append("W/m/K" if i == 0 else "")
+            else:
+                if style == "1-line":
+                    # blank the off-diagonals
+                    alpha = self.tensor_labels[i][0]
+                    table["K" + alpha].append("")
+                    table["e" + alpha].append("")
 
         figure = self.create_figure(
             module_path=("seamm",),
             template="line.graph_template",
-            title="Helfand Slopes",
+            title="Helfand Derivatives",
         )
 
         plot_helfand_slopes(
             figure, slopes, xs[0], err=errs, fit=fit0, labels=self.tensor_labels
         )
 
         figure.grid_plots("Slope")
 
         # Write to disk
-        filename = "Helfand_slopes.graph"
+        filename = "HelfandDerivatives.graph"
         path = Path(self.directory) / filename
         figure.dump(path)
 
         if "html" in self.options and self.options["html"]:
             path = path.with_suffix(".html")
             figure.template = "line.html_template"
             figure.dump(path)
@@ -498,21 +528,19 @@
                     "stderr": err,
                     "xs": xs,
                     "ys": ys,
                 }
             )
             v, e = fmt_err(slope, 2 * err)
             if style == "1-line":
-                if i == 0:
-                    table["Run"].append(len(self.V))
                 alpha = self.tensor_labels[i][0]
                 table["K" + alpha].append(v)
                 table["e" + alpha].append(e)
             elif style == "full":
-                table["Method"].append("Helfand" if i == 0 else "")
+                table["Method"].append("Helfand Moments" if i == 0 else "")
                 table["Dir"].append(self.tensor_labels[i][0])
                 table["Kappa"].append(v)
                 table["±"].append("±")
                 table["95%"].append(e)
                 table["Units"].append("W/m/K" if i == 0 else "")
 
         self.plot_helfand_moment(self.M, ts, M_err=self.M_err, fit=fit)
@@ -543,19 +571,15 @@
                     "ys": yf,
                     "a": a,
                     "a_err": a_err,
                     "tau": tau,
                     "tau_err": tau_err,
                 }
             )
-            try:
-                v, e = fmt_err(kappa, 2 * kappa_err)
-            except Exception:
-                v = f"{kappa:.2f}"
-                e = "--"
+            v, e = fmt_err(kappa, 2 * kappa_err)
 
             if style == "1-line":
                 if i == 0:
                     table["Run"].append("")
                 alpha = self.tensor_labels[i][0]
                 table["K" + alpha].append(v)
                 table["e" + alpha].append(e)
@@ -589,26 +613,26 @@
             if len(self.V) == 2:
                 length = len(tmp.splitlines()[0])
                 text += "\n"
                 text += "Thermal Conductivity".center(length)
                 text += "\n"
                 text += "--------------------".center(length)
                 text += "\n"
-                text += "First line is Helfand moments; second, Green-Kubo".center(
-                    length
-                )
+                text += "First line is the fit to Helfand derivative".center(length)
+                text += "\n"
+                text += "Second line is the slope of the Helfand moments".center(length)
+                text += "\n"
+                text += "Third line is the fit to Green-Kubo integral".center(length)
                 text += "\n"
                 text += "\n".join(tmp.splitlines()[0:-1])
             else:
-                text = tmp.splitlines()[-3]
-                text += "\n"
-                text += tmp.splitlines()[-2]
                 if run is not None and run == P["nruns"]:
-                    text += "\n"
-                    text += tmp.splitlines()[-1]
+                    text += "\n".join(tmp.splitlines()[-4:])
+                else:
+                    text += "\n".join(tmp.splitlines()[-4:-1])
 
             printer.normal(__(text, indent=8 * " ", wrap=False, dedent=False))
         else:
             text = ""
             tmp = tabulate(
                 table,
                 headers="keys",
@@ -792,15 +816,15 @@
         V = Q_(V, "Å^3")
         dt = Q_(timestep, "fs")
         k_B = Q_("k_B")
         Jsq = Q_("W^2/m^4")
 
         # Limit the lengths of the data
         n = J.shape[1]
-        m = min(n // 20, 10000)
+        m = min(n // 10, 10000)
 
         # Create the Helfand moments
         constants = Jsq * V * dt**2 / (2 * k_B * T**2)
         M = create_helfand_moments(J, m=m) * constants.m_as("W/m/K*ps")
         self.Ms.append(M)
 
         # And correlation functions for Green-Kubo method
```

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_parameters.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity_parameters.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/thermal_conductivity_step.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/thermal_conductivity_step.py`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step/tk_thermal_conductivity.py` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step/tk_thermal_conductivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         y = int(0.1 * screen_h / 2)
 
         self.dialog.geometry(f"{w}x{h}+{x}+{y}")
 
         # Add a frame for the flowchart
         notebook = self["notebook"]
         flowchart_frame = ttk.Frame(notebook)
-        self["flowchart frame"] = frame
+        self["flowchart frame"] = flowchart_frame
         notebook.add(flowchart_frame, text="Flowchart", sticky=tk.NSEW)
 
         self.tk_subflowchart = seamm.TkFlowchart(
             master=flowchart_frame,
             flowchart=self.node.subflowchart,
             namespace=self.namespace,
         )
```

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/PKG-INFO` & `thermal_conductivity_step-2023.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thermal-conductivity-step
-Version: 2023.5.5
+Name: thermal_conductivity_step
+Version: 2023.5.6
 Summary: A SEAMM plug-in for Thermal Conductivity
 Home-page: https://github.com/molssi-seamm/thermal_conductivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -81,14 +81,19 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.5.6 -- Bugfix
+    * Fixed an error handling Nan's and Inf's that caused a crash
+    * Added the predictions from the derivatives of the Helfand moments to the output to
+      give a better feel for the quality of the results.
+      
 2023.5.5 -- Improved analysis
     * Considerable improvements to the analysis, results now seem solid
     * Fixed issues with fitting the linear portion of the Helfand moments
     * Added plot of the slope from the Helfand moments, which is similar to the
       Green-Kubo integral.
     * Cleaned up both the output and graphs.
```

### Comparing `thermal_conductivity_step-2023.5.5/thermal_conductivity_step.egg-info/SOURCES.txt` & `thermal_conductivity_step-2023.5.6/thermal_conductivity_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thermal_conductivity_step-2023.5.5/versioneer.py` & `thermal_conductivity_step-2023.5.6/versioneer.py`

 * *Files identical despite different names*


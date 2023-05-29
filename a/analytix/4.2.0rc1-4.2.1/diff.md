# Comparing `tmp/analytix-4.2.0rc1.tar.gz` & `tmp/analytix-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analytix-4.2.0rc1.tar", last modified: Sat Feb 11 22:23:24 2023, max compression
+gzip compressed data, was "analytix-4.2.1.tar", last modified: Mon May 29 21:17:23 2023, max compression
```

## Comparing `analytix-4.2.0rc1.tar` & `analytix-4.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.461297 analytix-4.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-02-11 22:23:24.461297 analytix-4.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.453297 analytix-4.2.0rc1/analytix/
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28927 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.457297 analytix-4.2.0rc1/analytix/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/landing.html
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.457297 analytix-4.2.0rc1/analytix/reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    34369 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/reports/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/analytix/ux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.457297 analytix-4.2.0rc1/analytix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-02-11 22:23:24.000000 analytix-4.2.0rc1/analytix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-11 22:23:24.000000 analytix-4.2.0rc1/analytix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 22:23:24.000000 analytix-4.2.0rc1/analytix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-11 22:23:24.000000 analytix-4.2.0rc1/analytix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-11 22:23:24.000000 analytix-4.2.0rc1/analytix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.461297 analytix-4.2.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/excel.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/plots.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/requirements/types.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 22:23:24.461297 analytix-4.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 22:23:24.461297 analytix-4.2.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/tests/test_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/tests/test_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-02-11 22:23:11.000000 analytix-4.2.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.855634 analytix-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-29 21:17:14.000000 analytix-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 21:17:14.000000 analytix-4.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-29 21:17:23.855634 analytix-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-29 21:17:14.000000 analytix-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.851634 analytix-4.2.1/analytix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.855634 analytix-4.2.1/analytix/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/landing.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.855634 analytix-4.2.1/analytix/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/reports/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/reports/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/reports/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/reports/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 21:17:14.000000 analytix-4.2.1/analytix/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.851634 analytix-4.2.1/analytix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-29 21:17:23.000000 analytix-4.2.1/analytix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-29 21:17:23.000000 analytix-4.2.1/analytix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:17:23.000000 analytix-4.2.1/analytix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-29 21:17:23.000000 analytix-4.2.1/analytix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 21:17:23.000000 analytix-4.2.1/analytix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-29 21:17:14.000000 analytix-4.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.855634 analytix-4.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/excel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/nox.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 21:17:14.000000 analytix-4.2.1/requirements/types.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 21:17:23.855634 analytix-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-29 21:17:14.000000 analytix-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:17:23.855634 analytix-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-29 21:17:14.000000 analytix-4.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-29 21:17:14.000000 analytix-4.2.1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-29 21:17:14.000000 analytix-4.2.1/tests/test_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-29 21:17:14.000000 analytix-4.2.1/tests/test_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-29 21:17:14.000000 analytix-4.2.1/tests/test_utils.py
```

### Comparing `analytix-4.2.0rc1/LICENSE` & `analytix-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/PKG-INFO` & `analytix-4.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: analytix
-Version: 4.2.0rc1
+Version: 4.2.1
 Summary: A simple yet powerful wrapper for the YouTube Analytics API.
 Home-page: https://github.com/parafoxia/analytix
 Author: Ethan Henderson
 Author-email: ethan.henderson.1998@gmail.com
 License: BSD 3-Clause 'New' or 'Revised' License
-Project-URL: Documentation, https://parafoxia.github.io/analytix/
+Project-URL: Documentation, https://parafoxia.github.io/analytix
 Project-URL: Source, https://github.com/parafoxia/analytix
 Project-URL: Bug Tracker, https://github.com/parafoxia/analytix/issues
 Project-URL: CI, https://github.com/parafoxia/analytix/actions
 Project-URL: Changelog, https://github.com/parafoxia/analytix/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
@@ -100,25 +100,30 @@
 You may need to prefix these commands with a call to the Python interpreter depending on your OS and Python configuration.
 
 ## Additional support
 
 You can also install analytix with additional libraries to provide extra functionality:
 
 * `analytix[excel]` — support for exporting reports to Excel spreadsheets
-* `analytix[plots]` — support for plotting graphs for reports
 * `analytix[types]` — type stubs for type-hinted projects
 
 To install multiple at once, use commas:
 
 ```sh
-pip install "analytix[excel,plots,types]"
+pip install "analytix[excel,types]"
 ```
 
-Note that while analytix includes native support for DataFrame and Arrow table conversions, these libraries are not installed automatically.
-You will need to install these libraries yourself to use these features.
+Support for DataFrame and Arrow table conversions is also present.
+analytix supports these libraries natively:
+
+* `pandas` >= 0.23.2
+* `pyarrow` >= 2.0.0
+* `polars` >= 0.17.3
+
+Note: You will need to install your library of choice manually to be able to use it.
 
 ## OAuth authentication
 
 All requests to the YouTube Analytics API need to be authorised through OAuth 2.
 In order to do this, you will need a Google Developers project with the YouTube Analytics API enabled.
 You can find instructions on how to do that in the [API setup guide](https://parafoxia.github.io/analytix/starting/googleapp/), or on [this video](https://www.youtube.com/watch?v=1Xday10ZWeg).
 
@@ -140,14 +145,16 @@
 analytix.enable_logging()
 ```
 
 If anything is going wrong, or analytix appears to be taking a long time to fetch data, try enabling the logger in DEBUG mode.
 
 ## Usage
 
+### Retrieving reports
+
 Retrieving reports from the YouTube Analytics API is easy.
 The below example loads credentials from a secrets file, and gets day-by-day data on views, likes, and comments from the US over the last 28 days:
 
 ```py
 from analytix import Client  # or AsyncClient
 
 client = Client("./secrets.json")
@@ -155,33 +162,23 @@
     dimensions=("day",),
     filters={"country": "US"},
     metrics=("views", "likes", "comments"),
 )
 report.to_csv("./analytics.csv")
 ```
 
-If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame:
+If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame or table.
 
 ```py
-# Return as a pandas DataFrame:
 df = report.to_pandas()
-
-# Return as an Apache Arrow table:
 table = report.to_arrow()
-
-# Return as a Polars DataFrame:
 df = report.to_polars()
 ```
 
-If you want to quickly plot the data, you can use the in-built plotter:
-
-```py
-plot = report.plot(("views",), size=(12, 6))
-plot.save("figure.png")
-```
+### Fetching group information
 
 You can also fetch groups and group items:
 
 ```py
 from analytix import Client
 
 client = Client("./secrets.json")
```

### Comparing `analytix-4.2.0rc1/README.md` & `analytix-4.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -56,25 +56,30 @@
 You may need to prefix these commands with a call to the Python interpreter depending on your OS and Python configuration.
 
 ## Additional support
 
 You can also install analytix with additional libraries to provide extra functionality:
 
 * `analytix[excel]` — support for exporting reports to Excel spreadsheets
-* `analytix[plots]` — support for plotting graphs for reports
 * `analytix[types]` — type stubs for type-hinted projects
 
 To install multiple at once, use commas:
 
 ```sh
-pip install "analytix[excel,plots,types]"
+pip install "analytix[excel,types]"
 ```
 
-Note that while analytix includes native support for DataFrame and Arrow table conversions, these libraries are not installed automatically.
-You will need to install these libraries yourself to use these features.
+Support for DataFrame and Arrow table conversions is also present.
+analytix supports these libraries natively:
+
+* `pandas` >= 0.23.2
+* `pyarrow` >= 2.0.0
+* `polars` >= 0.17.3
+
+Note: You will need to install your library of choice manually to be able to use it.
 
 ## OAuth authentication
 
 All requests to the YouTube Analytics API need to be authorised through OAuth 2.
 In order to do this, you will need a Google Developers project with the YouTube Analytics API enabled.
 You can find instructions on how to do that in the [API setup guide](https://parafoxia.github.io/analytix/starting/googleapp/), or on [this video](https://www.youtube.com/watch?v=1Xday10ZWeg).
 
@@ -96,14 +101,16 @@
 analytix.enable_logging()
 ```
 
 If anything is going wrong, or analytix appears to be taking a long time to fetch data, try enabling the logger in DEBUG mode.
 
 ## Usage
 
+### Retrieving reports
+
 Retrieving reports from the YouTube Analytics API is easy.
 The below example loads credentials from a secrets file, and gets day-by-day data on views, likes, and comments from the US over the last 28 days:
 
 ```py
 from analytix import Client  # or AsyncClient
 
 client = Client("./secrets.json")
@@ -111,33 +118,23 @@
     dimensions=("day",),
     filters={"country": "US"},
     metrics=("views", "likes", "comments"),
 )
 report.to_csv("./analytics.csv")
 ```
 
-If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame:
+If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame or table.
 
 ```py
-# Return as a pandas DataFrame:
 df = report.to_pandas()
-
-# Return as an Apache Arrow table:
 table = report.to_arrow()
-
-# Return as a Polars DataFrame:
 df = report.to_polars()
 ```
 
-If you want to quickly plot the data, you can use the in-built plotter:
-
-```py
-plot = report.plot(("views",), size=(12, 6))
-plot.save("figure.png")
-```
+### Fetching group information
 
 You can also fetch groups and group items:
 
 ```py
 from analytix import Client
 
 client = Client("./secrets.json")
```

### Comparing `analytix-4.2.0rc1/analytix/__init__.py` & `analytix-4.2.1/analytix/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,49 +27,44 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 __all__ = (
     "API_BASE_URL",
     "API_GROUPS_URL",
     "API_GROUP_ITEMS_URL",
     "API_REPORTS_URL",
-    "API_SCOPES",
     "AsyncBaseClient",
     "AsyncClient",
     "can_use",
     "Client",
     "enable_logging",
     "groups",
     "OAUTH_CHECK_URL",
+    "process_path",
     "reports",
-    "requires",
+    "Scopes",
     "UPDATE_CHECK_URL",
-    "warn",
-    "warn_on_call",
 )
 
 __productname__ = "analytix"
-__version__ = "4.2.0rc1"
+__version__ = "4.2.1"
 __description__ = "A simple yet powerful wrapper for the YouTube Analytics API."
 __url__ = "https://github.com/parafoxia/analytix"
-__docs__ = "https://parafoxia.github.io/analytix/"
+__docs__ = "https://parafoxia.github.io/analytix"
 __author__ = "Ethan Henderson"
 __author_email__ = "ethan.henderson.1998@gmail.com"
 __license__ = "BSD 3-Clause 'New' or 'Revised' License"
 __bugtracker__ = "https://github.com/parafoxia/analytix/issues"
 __ci__ = "https://github.com/parafoxia/analytix/actions"
 __changelog__ = "https://github.com/parafoxia/analytix/releases"
 
 API_BASE_URL = "https://youtubeanalytics.googleapis.com/v2/"
 API_REPORTS_URL = API_BASE_URL + "reports?"
 API_GROUPS_URL = API_BASE_URL + "groups?"
 API_GROUP_ITEMS_URL = API_BASE_URL + "groupItems?"
-API_SCOPES = (
-    "https://www.googleapis.com/auth/yt-analytics.readonly",
-    "https://www.googleapis.com/auth/yt-analytics-monetary.readonly",
-)
 OAUTH_CHECK_URL = "https://www.googleapis.com/oauth2/v3/tokeninfo?access_token="
 UPDATE_CHECK_URL = "https://pypi.org/pypi/analytix/json"
 
 from . import groups, reports
 from .client import AsyncBaseClient, AsyncClient, Client
-from .utils import *
+from .oidc import Scopes
+from .utils import can_use, process_path
 from .ux import enable_logging
```

### Comparing `analytix-4.2.0rc1/analytix/__main__.py` & `analytix-4.2.1/analytix/__main__.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/analytix/abc.py` & `analytix-4.2.1/analytix/abc.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/analytix/client.py` & `analytix-4.2.1/analytix/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,35 +55,38 @@
 """
 
 from __future__ import annotations
 
 __all__ = ("AsyncBaseClient", "AsyncClient", "Client")
 
 import asyncio
-import datetime
 import logging
 import os
 import sys
 import typing as t
+import warnings
 import webbrowser
 from contextlib import contextmanager
 from functools import partial
 from pathlib import Path
-from types import TracebackType
 
 from aiohttp import ClientSession
 
 import analytix
 from analytix import oidc
 from analytix.errors import AuthorisationError, RefreshTokenExpired
-from analytix.groups import GroupItemList, GroupList
-from analytix.reports import AnalyticsReport
 from analytix.shard import Shard
+from analytix.warnings import NotUpdatedWarning
 
 if t.TYPE_CHECKING:
+    import datetime
+    from types import TracebackType
+
+    from analytix.groups import GroupItemList, GroupList
+    from analytix.reports import AnalyticsReport
     from analytix.types import OptionalPathLikeT, PathLikeT
 
 _log = logging.getLogger(__name__)
 
 
 class AsyncBaseClient:
     """A basic async client interface for the YouTube Analytics API.
@@ -115,40 +118,48 @@
     ??? example "Basic example"
         ```py
         client = AsyncBaseClient("secrets.json")
         ```
 
     ??? example "Context manager example"
         ```py
-        with AsyncBaseClient("secrets.json") as client:
+        async with AsyncBaseClient("secrets.json") as client:
             await client.teardown()
         ```
     """
 
-    __slots__ = ("_loop", "_secrets", "_session")
+    __slots__ = ("_loop", "_scopes", "_secrets", "_session")
 
     def __init__(
         self,
         secrets_file: PathLikeT,
         *,
+        scopes: oidc.Scopes = oidc.Scopes.ALL,
         loop: asyncio.AbstractEventLoop | None = None,
         session: ClientSession | None = None,
         **kwargs: t.Any,
     ) -> None:
         try:
             self._loop = loop or asyncio.get_running_loop()
         except RuntimeError:
             self._loop = (
                 asyncio.new_event_loop()
                 if sys.version_info >= (3, 10)
                 else asyncio.get_event_loop()
             )
 
         self._secrets = oidc.Secrets.from_file(secrets_file)
-        self._session = session or ClientSession(loop=self._loop, **kwargs)
+        self._scopes = scopes
+
+        with warnings.catch_warnings():
+            # Suppress that annoying warning about ClientSession only
+            # being creatable in an async function, while allowing other
+            # deprecation warnings to be logged.
+            warnings.simplefilter("ignore", DeprecationWarning)
+            self._session = session or ClientSession(loop=self._loop, **kwargs)
 
         if not os.environ.get("PYTEST_CURRENT_TEST"):
             # This causes issues when run in testing, so we'll just make
             # sure we only run it when we want to.
             self._loop.create_task(self._check_for_updates())
 
     def __str__(self) -> str:
@@ -188,16 +199,18 @@
                 # If we can't get the info, just ignore it.
                 _log.debug("Failed to get version information")
                 return
 
             latest = (await resp.json())["info"]["version"]
 
         if analytix.__version__ != latest:
-            _log.warning(
-                f"You do not have the latest stable version of analytix (v{latest})"
+            warnings.warn(
+                f"You do not have the latest stable version of analytix (v{latest})",
+                NotUpdatedWarning,
+                stacklevel=6,
             )
 
     async def teardown(self) -> None:
         """Tears the client down.
 
         This should be called before your program ends. If you're using
         the client in a context manager, this is done automatically.
@@ -248,15 +261,15 @@
                 await shard.retrieve_report(dimensions=("day",))
             ```
         """
 
         if not isinstance(tokens, oidc.Tokens):
             tokens = oidc.Tokens.from_dict(tokens)
 
-        shard = Shard(self._session, self._secrets, tokens)
+        shard = Shard(self._session, self._secrets, tokens, self._scopes)
         yield shard
         del shard
 
 
 class AsyncClient(AsyncBaseClient):
     """An async client interface for the YouTube Analytics API.
 
@@ -271,17 +284,17 @@
     ??? example "Basic example"
         ```py
         client = AsyncClient("secrets.json")
         ```
 
     ??? example "Context manager example"
         ```py
-        with AsyncClient("secrets.json") as client:
+        async with AsyncClient("secrets.json") as client:
             # Perform operations here.
-            await client.teardown()
+            print(client)
         ```
 
     ??? example "Advanced example"
         ```py
         client = AsyncClient(
             "secrets.json",
             tokens_dir="./tokens",
@@ -302,20 +315,22 @@
     def __init__(
         self,
         secrets_file: PathLikeT,
         *,
         tokens_dir: OptionalPathLikeT = ".",
         ws_port: int = 8080,
         auto_open_browser: bool = False,
+        scopes: oidc.Scopes = oidc.Scopes.ALL,
         loop: asyncio.AbstractEventLoop | None = None,
         session: ClientSession | None = None,
         **kwargs: t.Any,
     ) -> None:
         super().__init__(
             secrets_file,
+            scopes=scopes,
             loop=loop,
             session=session,
             **kwargs,
         )
 
         if tokens_dir is not None:
             if not isinstance(tokens_dir, Path):
@@ -327,14 +342,25 @@
         self._tokens_dir = tokens_dir
         self._ws_port = ws_port
         self._auto_open_browser = auto_open_browser
 
         self._active_tokens: str | None = None
         self._shard: Shard | None = None
 
+    async def __aenter__(self) -> AsyncClient:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_value: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.teardown()
+
     @property
     def active_tokens(self) -> str | None:
         return self._active_tokens
 
     async def _get_existing_tokens(self, token_id: str | None) -> oidc.Tokens | None:
         if self._shard and (token_id == self._active_tokens):
             return self._shard._tokens
@@ -351,15 +377,15 @@
     async def authorise(self, token_id: str | None = None) -> None:
         # Determine token ID.
         token_id = token_id or self._active_tokens or self._secrets.project_id
         tokens = await self._get_existing_tokens(token_id)
 
         # Handle existing tokens.
         if tokens:
-            self._shard = Shard(self._session, self._secrets, tokens)
+            self._shard = Shard(self._session, self._secrets, tokens, self._scopes)
 
             try:
                 refreshed = bool(await self._shard.refresh_access_token(check=True))
                 if refreshed and self._tokens_dir:
                     await self._shard._tokens.write(
                         self._tokens_dir / f"{token_id}.json"
                     )
@@ -367,25 +393,26 @@
                 _log.info("Authorisation complete!")
                 return
 
             except RefreshTokenExpired:
                 _log.info("Refresh token expired, starting auth flow")
 
         # If no valid tokens by this point, start auth flow.
-        auth_uri, params = oidc.auth_uri(self._secrets, self._ws_port)
+        auth_uri, params = oidc.auth_uri(self._secrets, self._ws_port, self._scopes)
         _log.debug(f"Auth parameters: {params}")
+        _log.debug(f"Scopes: {self._scopes}")
 
         if self._auto_open_browser:
-            _log.info(f"Opening browser at {self._secrets.auth_uri}?...")
+            _log.info(f"Opening browser at {self._secrets.auth_uri}")
             if not webbrowser.open(auth_uri, 0, True):
                 raise RuntimeError(
                     "web browser failed to open — if you use WSL, refer to the docs"
                 )
         else:
-            print(
+            print(  # noqa: T201
                 "\33[38;5;45mYou need to authorise analytix.\33[0m "
                 f"\33[4m{auth_uri}\33[0m"
             )
 
         code = oidc.authenticate(params)
         _log.debug(f"Auth code: {code}")
 
@@ -401,15 +428,15 @@
                 raise AuthorisationError(
                     f"could not authorise: {resp_data['error_description']} "
                     f"({resp_data['error']})"
                 )
 
         # Configure tokens using response data.
         tokens = oidc.Tokens.from_dict(resp_data)
-        self._shard = Shard(self._session, self._secrets, tokens)
+        self._shard = Shard(self._session, self._secrets, tokens, self._scopes)
         if self._tokens_dir:
             await tokens.write(self._tokens_dir / f"{token_id}.json")
         self._active_tokens = token_id
 
         _log.info("Authorisation complete!")
 
     async def retrieve_report(
@@ -472,14 +499,20 @@
         provided, the current working directory is used.
     ws_port : int, optional
         The webserver port to use when authenticating.
     auto_open_browser : bool, optional
         Whether to automatically open the browser for authentication
         when necessary. If this is `False`, the auth URI is printed to
         the console.
+    scopes : Scopes, optional
+        The scopes to allow when authorising. This defines what data
+        the client can pull. This is especially useful for non-partnered
+        channels for which revenue data cannot be ascertained. If this
+        is not provided, all scopes are used, though non-partnered
+        channels should only use the READONLY scope.
 
     Other Parameters
     ----------------
     loop : AbstractEventLoop, optional
         The asyncio event loop to use. If this is not provided, the
         client will create one.
     session : ClientSession, optional
@@ -492,14 +525,18 @@
         The token directory passed is not, in fact, a directory.
 
     !!! warning
         This client is a sync wrapper of the `AsyncClient`, so is still
         async under the hood. As such, it is not threadsafe.
 
     !!! warning
+        If your channel is not partnered, you may need to configure your
+        client to only use the READONLY scope. See the example below.
+
+    !!! warning
         If you use WSL, the browser may not open even if
         `auto_open_browser` is `True`.
 
         To fix the issue:
 
         1. install [WSLU](https://github.com/wslutilities/wslu)
         2. add `export BROWSER="wslview"` to your shell's rc file
@@ -513,62 +550,76 @@
         client = Client("secrets.json")
         ```
 
     ??? example "Context manager example"
         ```py
         with Client("secrets.json") as client:
             # Perform operations here.
-            client.teardown()
+            print(client)
         ```
 
     ??? example "Advanced example"
         ```py
         client = Client(
             "secrets.json",
             tokens_dir="./tokens",
             ws_port=9999,
             auto_open_browser=True,
         )
         ```
+
+    ??? example "Using custom scopes"
+        ```py
+        from analytix import Scopes
+
+        client = Client(scopes=Scopes.READONLY)
+        ```
     """
 
     __slots__ = ("_client",)
 
     _loop: asyncio.AbstractEventLoop
     _secrets: oidc.Secrets
     _session: ClientSession
     _tokens_dir: Path | None
     _ws_port: int
     _auto_open_browser: bool
+    _scopes: oidc.Scopes
     _active_tokens: str
     _shard: Shard
 
     def __init__(
         self,
         secrets_file: PathLikeT,
         *,
         tokens_dir: OptionalPathLikeT = ".",
         ws_port: int = 8080,
         auto_open_browser: bool = False,
+        scopes: oidc.Scopes = oidc.Scopes.ALL,
         loop: asyncio.AbstractEventLoop | None = None,
         session: ClientSession | None = None,
         **kwargs: t.Any,
     ) -> None:
         self._client = AsyncClient(
             secrets_file,
             tokens_dir=tokens_dir,
             ws_port=ws_port,
             auto_open_browser=auto_open_browser,
+            scopes=scopes,
             loop=loop,
             session=session,
             **kwargs,
         )
 
-        getter = lambda attr, self: getattr(self._client, attr)
-        setter = lambda attr, self, value: setattr(self._client, attr, value)
+        def getter(attr: str, self: Client) -> t.Any:
+            return getattr(self._client, attr)
+
+        def setter(attr: str, self: Client, value: t.Any) -> t.Any:
+            return setattr(self._client, attr, value)
+
         for attr in AsyncBaseClient.__slots__ + AsyncClient.__slots__:
             setattr(
                 self.__class__,
                 attr,
                 property(partial(getter, attr), partial(setter, attr)),
             )
```

### Comparing `analytix-4.2.0rc1/analytix/errors.py` & `analytix-4.2.1/analytix/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -102,28 +102,81 @@
     fails."""
 
 
 class InvalidRequest(AnalytixError):
     """Exception thrown when a request to be made to the YouTube
     Analytics API is not valid."""
 
+    @staticmethod
+    def list_of(values: set[str]) -> str:
+        items = tuple(f"{v!r}" for v in sorted(values))
+
+        if len(items) > 2:
+            return f"{', '.join(items[:-1])}, and {items[-1]}"
+
+        return " and ".join(items)
+
+    @classmethod
+    def invalid(cls, key: str, values: set[str]) -> InvalidRequest:
+        plural = "s" if len(values) > 1 else ""
+        return cls(f"invalid {key}{plural} provided: " + cls.list_of(values))
+
+    @classmethod
+    def incompatible_dimensions(cls, values: set[str]) -> InvalidRequest:
+        return cls(f"dimensions {cls.list_of(values)} cannot be used together")
+
+    @classmethod
+    def incompatible_filters(cls, values: set[str]) -> InvalidRequest:
+        return cls(f"filters {cls.list_of(values)} cannot be used together")
+
+    @classmethod
+    def invalid_filter_value(cls, key: str, value: str) -> InvalidRequest:
+        return cls(f"invalid value {value!r} for filter {key!r}")
+
+    @classmethod
+    def incompatible_filter_value(cls, key: str, value: str) -> InvalidRequest:
+        return cls(
+            f"value {value!r} for filter {key!r} cannot be used with the given "
+            "dimensions"
+        )
+
+    @classmethod
+    def incompatible_metrics(cls, values: set[str]) -> InvalidRequest:
+        plural = "s" if len(values) > 1 else ""
+        return cls(
+            f"metric{plural} {cls.list_of(values)} cannot be used with the given "
+            "dimensions and filters"
+        )
+
+    @classmethod
+    def incompatible_sort_options(cls, values: set[str]) -> InvalidRequest:
+        plural = "s" if len(values) > 1 else ""
+        return cls(
+            f"sort option{plural} {cls.list_of(values)} cannot be used with the given "
+            "dimensions and filters"
+        )
+
+    @classmethod
+    def non_matching_sort_options(cls, values: set[str]) -> InvalidRequest:
+        plural = "s" if len(values) > 1 else ""
+        isare = "are" if plural else "is"
+        return cls(
+            f"sort option{plural} {cls.list_of(values)} {isare} not part of the given "
+            "metrics"
+        )
+
+    @classmethod
+    def invalid_set(
+        cls, key: str, values: set[str], expd: str, recv: int
+    ) -> InvalidRequest:
+        plural = "" if expd in ("1", "at least 1") else "s"
+        return cls(
+            f"expected {expd} {key}{plural} from {cls.list_of(values)}, got {recv}"
+        )
 
-class InvalidFeatures(InvalidRequest):
-    """A helper exception class for `InvalidRequest`. When catching
-    exceptions, use `InvalidRequest` instead."""
 
-    def __init__(self, ctx: str, errors: set[str]) -> None:
-        err_list = ", ".join(errors)
-        super().__init__(f"{ctx}: {err_list}")
+class InvalidFeatures(InvalidRequest):
+    ...
 
 
 class InvalidFeatureSet(InvalidRequest):
-    """A helper exception class for `InvalidRequest`. When catching
-    exceptions, use `InvalidRequest` instead."""
-
-    def __init__(self, type: str, expd: str, recv: int, values: set[str]) -> None:
-        val_list = ", ".join(values)
-        super().__init__(f"expected {expd} {type}(s) from [ {val_list} ], got {recv}")
-
-
-class PlottingError(AnalytixError):
-    """Exception thrown when plotting a report fails."""
+    ...
```

### Comparing `analytix-4.2.0rc1/analytix/groups/__init__.py` & `analytix-4.2.1/analytix/groups/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 __all__ = ("Group", "GroupList", "GroupItem", "GroupItemList")
 
-from .groups import *
+from .groups import Group, GroupItem, GroupItemList, GroupList
```

### Comparing `analytix-4.2.0rc1/analytix/groups/groups.py` & `analytix-4.2.1/analytix/groups/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,21 +26,22 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
 __all__ = ("Group", "GroupList", "GroupItem", "GroupItemList")
 
-import datetime as dt
 import typing as t
 from dataclasses import dataclass
 
 from dateutil.parser import parse as du_parse
 
 if t.TYPE_CHECKING:
+    import datetime as dt
+
     from analytix.types import ResponseT
 
 
 @dataclass(frozen=True)
 class _Resource:
     __slots__ = ("kind", "etag")
```

### Comparing `analytix-4.2.0rc1/analytix/landing.html` & `analytix-4.2.1/analytix/landing.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <style>@font-face{ font-family:'Hind';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/hind/v16/5aU69_a8oxmIRG4.ttf) format('truetype');}@font-face{ font-family:'Michroma';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/michroma/v16/PN_zRfy9qWD8fEagAMg6.ttf) format('truetype');}body, html{ background-color:#0f0f0f;color:#dddddd;font-family:"Hind", sans-serif;width:100%;height:100%;display:flex;justify-content:center;align-items:center;margin:0;padding:0;}h1, h2, h3, h4, h5, h6{ font-family:"Michroma", sans-serif;}h1{ font-size:1.7em;}h2{ font-size:1.2em;}main{ max-width:30em;background-color:#1c1c1c;border-radius:1em;text-align:center;padding:2em;box-shadow:0px 12px 24px -4px rgba(0, 0, 0, 0.5);-webkit-box-shadow:0px 12px 24px -4px rgba(0, 0, 0, 0.5);}a{ color:inherit;}.icon{ height:2em;filter:invert(75%);margin:0.8em 0.8em 0.8em 0;}footer{ position:absolute;bottom:0;margin:2.5em;}footer > div{ display:flex;align-items:center;}.footer-item{ filter:invert(50%);margin:0.8em;display:flex;align-items:center;text-decoration:none;font-family:"Michroma", sans-serif;font-size:smaller;transition:0.1s ease-in-out filter;}.footer-item:hover{ filter:invert(0%);}.footer-item ~ .footer-item > .icon{ margin:0.8em;}</style> <title>Authorisation complete!</title> </head> <body> <main> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/logo.png" alt="Analytix Logo" width="80%" style="padding-top:1em"> <h1>Authorisation complete!</h1> <p> Awesome &#8212; analytix is now authorised! You may now close this window. </p> <h2>What happens now?</h2> <p> Your tokens will be saved to the file path you specified. If you did not specify a file path, you will find them in a JSON file named after the project ID of your Google Developers application in your current working directory. <br><br> Your new tokens will serve you well for the next 7 days, unless your application status is anything other than "Testing". If you do not know whether your application's status is "Testing", it more than likely is. You can find more information regarding the lifetime of tokens on the <a href="https://developers.google.com/identity/protocols/oauth2#expiration">Google Identity documentation</a>. </p> </main> <footer> <div> <a class="footer-item" href="https://analytix.readthedocs.io"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/docs.svg" alt="Docs" class="icon" style> <span>DOCS</span> </a> <a class="footer-item" href="https://pypi.org/project/analytix/"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/pypi.svg" alt="PyPI" class="icon"> <span>PYPI</span> </a> <a class="footer-item" href="https://github.com/parafoxia/analytix"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/github.svg" alt="GitHub" class="icon"> <span>GITHUB</span> </a> <a class="footer-item" href="https://github.com/parafoxia/analytix/releases"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/changelog.svg" alt="Changelog" class="icon"> <span>CHANGELOG</span> </a> </div> </footer> </body> </html>
+<!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <style>@font-face{ font-family:'Hind';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/hind/v16/5aU69_a8oxmIRG4.ttf) format('truetype');}@font-face{ font-family:'Michroma';font-style:normal;font-weight:400;font-display:swap;src:url(https://fonts.gstatic.com/s/michroma/v16/PN_zRfy9qWD8fEagAMg6.ttf) format('truetype');}body, html{ background-color:#0f0f0f;color:#dddddd;font-family:"Hind", sans-serif;width:100%;height:100%;display:flex;justify-content:center;align-items:center;margin:0;padding:0;}h1, h2, h3, h4, h5, h6{ font-family:"Michroma", sans-serif;}h1{ font-size:1.7em;}h2{ font-size:1.2em;}main{ max-width:30em;background-color:#1c1c1c;border-radius:1em;text-align:center;padding:2em;box-shadow:0px 12px 24px -4px rgba(0, 0, 0, 0.5);-webkit-box-shadow:0px 12px 24px -4px rgba(0, 0, 0, 0.5);}a{ color:inherit;}.icon{ height:2em;filter:invert(75%);margin:0.8em 0.8em 0.8em 0;}footer{ position:absolute;bottom:0;margin:2.5em;}footer > div{ display:flex;align-items:center;}.footer-item{ filter:invert(50%);margin:0.8em;display:flex;align-items:center;text-decoration:none;font-family:"Michroma", sans-serif;font-size:smaller;transition:0.1s ease-in-out filter;}.footer-item:hover{ filter:invert(0%);}.footer-item ~ .footer-item > .icon{ margin:0.8em;}</style> <title>Authorisation complete!</title> </head> <body> <main> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/logo.png" alt="Analytix Logo" width="80%" style="padding-top:1em"> <h1>Authorisation complete!</h1> <p> Awesome &#8212; analytix is now authorised! You may now close this window. </p> <h2>What happens now?</h2> <p> Your tokens will be saved to the file path you specified. If you did not specify a file path, you will find them in a JSON file named after the project ID of your Google Developers application in your current working directory. <br><br> Your new tokens will serve you well for the next 7 days, unless your application status is anything other than "Testing". If you do not know whether your application's status is "Testing", it more than likely is. You can find more information regarding the lifetime of tokens on the <a href="https://developers.google.com/identity/protocols/oauth2#expiration">Google Identity documentation</a>. </p> </main> <footer> <div> <a class="footer-item" href="https://parafoxia.github.io/analytix/"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/docs.svg" alt="Docs" class="icon" style> <span>DOCS</span> </a> <a class="footer-item" href="https://pypi.org/project/analytix/"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/pypi.svg" alt="PyPI" class="icon"> <span>PYPI</span> </a> <a class="footer-item" href="https://github.com/parafoxia/analytix"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/github.svg" alt="GitHub" class="icon"> <span>GITHUB</span> </a> <a class="footer-item" href="https://github.com/parafoxia/analytix/releases"> <img src="https://raw.githubusercontent.com/parafoxia/analytix/main/assets/icons/changelog.svg" alt="Changelog" class="icon"> <span>CHANGELOG</span> </a> </div> </footer> </body> </html>
```

### Comparing `analytix-4.2.0rc1/analytix/oidc.py` & `analytix-4.2.1/analytix/oidc.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     [Google Identity documentation](https://developers.google.com/
     identity/openid-connect/openid-connect).
 """
 
 from __future__ import annotations
 
 __all__ = (
+    "Scopes",
     "Secrets",
     "Tokens",
     "state_token",
     "auth_uri",
     "token_uri",
     "refresh_uri",
     "authenticate",
@@ -54,32 +55,51 @@
 import hashlib
 import json
 import logging
 import os
 import re
 import typing as t
 from dataclasses import dataclass
+from enum import Enum
 from http import server
 from pathlib import Path
 from urllib.parse import parse_qsl, urlencode
 
 import aiofiles
 
-import analytix
 from analytix.errors import AuthorisationError
 from analytix.types import SecretT, TokenT
 
 if t.TYPE_CHECKING:
     from analytix.types import AuthUriT, TokenUriT
 
 REDIRECT_URI_PATTERN = re.compile("[^//]*//([^:]*):?([0-9]*)")
 
 _log = logging.getLogger(__name__)
 
 
+class Scopes(Enum):
+    """An enum for API scopes."""
+
+    READONLY = "https://www.googleapis.com/auth/yt-analytics.readonly"
+    """Omit revenue data from reports."""
+
+    MONETARY_READONLY = "https://www.googleapis.com/auth/yt-analytics-monetary.readonly"
+    """Only include revenue data in reports."""
+
+    ALL = f"{READONLY} {MONETARY_READONLY}"
+    """Include all data in reports.
+
+    !!! warning
+        This is the default, though your channel needs to be partnered
+        to use it. If your channel is not partnered, configure your
+        client to use the `READONLY` scope.
+    """
+
+
 @dataclass(frozen=True)
 class Secrets:
     """A representation of your client secrets.
 
     This should always be created using the `from_file` classmethod.
 
     Parameters
@@ -251,15 +271,15 @@
 
         Returns
         -------
         Tokens
             The newly created instance.
         """
 
-        return cls(**data)  # type: ignore
+        return cls(**data)  # type: ignore[arg-type]
 
     @classmethod
     async def from_file(cls, path: Path | str) -> Tokens:
         """Load tokens from a JSON file.
 
         Parameters
         ----------
@@ -359,15 +379,15 @@
     str
         A new state token.
     """
 
     return hashlib.sha256(os.urandom(1024)).hexdigest()
 
 
-def auth_uri(secrets: Secrets, port: int) -> AuthUriT:
+def auth_uri(secrets: Secrets, port: int, scopes: Scopes) -> AuthUriT:
     """Returns the authentication URI and parameters.
 
     Parameters
     ----------
     secrets : Secrets
         Your client secrets.
     port : int
@@ -382,15 +402,15 @@
     """
 
     params = {
         "client_id": secrets.client_id,
         "nonce": state_token(),
         "response_type": "code",
         "redirect_uri": secrets.redirect_uris[-1] + (f":{port}" if port != 80 else ""),
-        "scope": " ".join(analytix.API_SCOPES),
+        "scope": scopes.value,
         "state": state_token(),
         "access_type": "offline",
     }
     return f"{secrets.auth_uri}?{urlencode(params)}", params
 
 
 def token_uri(secrets: Secrets, code: str, auth_params: dict[str, str]) -> TokenUriT:
@@ -456,15 +476,15 @@
     return secrets.token_uri, data, headers
 
 
 class _RequestHandler(server.BaseHTTPRequestHandler):
     def log_request(self, code: int | str = "-", _: int | str = "-") -> None:
         _log.debug(f"Received request ({code})")
 
-    def do_GET(self) -> None:
+    def do_GET(self) -> None:  # noqa: N802
         self.send_response(200)
         self.send_header("Content-type", "text/html")
         self.end_headers()
 
         self.server: _Server  # Overwrite type so code is exposed.
         self.server.query = dict(parse_qsl(self.path.split("?")[1]))
         self.wfile.write((Path(__file__).parent / "landing.html").read_bytes())
```

### Comparing `analytix-4.2.0rc1/analytix/queries.py` & `analytix-4.2.1/analytix/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,25 @@
 from __future__ import annotations
 
 __all__ = ("ReportQuery", "GroupQuery", "GroupItemQuery")
 
 import datetime as dt
 import logging
 import typing as t
+import warnings
 
 import analytix
-from analytix.abc import ReportType
 from analytix.errors import InvalidRequest
+from analytix.oidc import Scopes
 from analytix.reports import data
 from analytix.reports import types as rt
+from analytix.warnings import InvalidMonthFormatWarning
+
+if t.TYPE_CHECKING:
+    from analytix.abc import ReportType
 
 _log = logging.getLogger(__name__)
 
 
 class ReportQuery:
     __slots__ = (
         "dimensions",
@@ -110,15 +115,15 @@
             f"&startDate={self.start_date}"
             f"&endDate={self.end_date}"
             f"&currency={self.currency}"
             f"&startIndex={self.start_index}"
             f"&includeHistoricalData={self.include_historical_data}"
         )
 
-    def validate(self) -> None:
+    def validate(self, scopes: Scopes) -> None:
         _log.info("Validating request")
 
         if self.max_results < 0:
             raise InvalidRequest(
                 "the max results should be non-negative (0 for unlimited results)"
             )
 
@@ -127,41 +132,54 @@
 
         if not isinstance(self._end_date, dt.date):
             raise InvalidRequest("expected end date as date object")
 
         if self._end_date < self._start_date:
             raise InvalidRequest("the start date should be earlier than the end date")
 
-        if "month" in self.dimensions:
-            if self._start_date.day != 1 or self._end_date.day != 1:
-                _log.warning(
-                    "Correcting start and end dates -- if 'month' is passed as a "
-                    "dimension, these should always be the first day of the month"
-                )
-                self._start_date = dt.date(
-                    self._start_date.year, self._start_date.month, 1
-                )
-                self._end_date = dt.date(self._end_date.year, self._end_date.month, 1)
+        if "month" in self.dimensions and (
+            self._start_date.day != 1 or self._end_date.day != 1
+        ):
+            warnings.warn(
+                "Correcting start and end dates -- if 'month' is passed as a "
+                "dimension, these should always be the first day of the month",
+                InvalidMonthFormatWarning,
+                stacklevel=4,
+            )
+            self._start_date = dt.date(self._start_date.year, self._start_date.month, 1)
+            self._end_date = dt.date(self._end_date.year, self._end_date.month, 1)
 
         _log.info(f"Getting data between {self.start_date} and {self.end_date}")
 
         if self.currency not in data.CURRENCIES:
-            raise InvalidRequest("expected a valid ISO 4217 currency code")
+            raise InvalidRequest(
+                f"expected a valid ISO 4217 currency code, got {self.currency!r}"
+            )
 
         if self.start_index < 1:
             raise InvalidRequest("the start index should be positive")
 
         self.set_report_type()
         assert self.rtype is not None
 
         if not self.metrics:
             self.metrics = [
                 m for m in data.ALL_METRICS_ORDERED if m in self.rtype.metrics.values
             ]
-            _log.debug("Metrics set to: " + ", ".join(self.metrics))
+
+        if Scopes.MONETARY_READONLY.value not in scopes.value:
+            self.metrics = [m for m in self.metrics if m not in data.REVENUE_METRICS]
+        elif Scopes.READONLY.value not in scopes.value:
+            self.metrics = [m for m in self.metrics if m in data.REVENUE_METRICS]
+
+        _log.debug("Metrics set to: " + ", ".join(self.metrics))
+
+        diff = {o.strip("-") for o in self.sort_options} - set(self.metrics)
+        if diff:
+            raise InvalidRequest.non_matching_sort_options(diff)
 
         self.rtype.validate(
             self.dimensions,
             self.filters,
             self.metrics,
             self.sort_options,
             self.max_results,
```

### Comparing `analytix-4.2.0rc1/analytix/reports/__init__.py` & `analytix-4.2.1/analytix/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/analytix/reports/data.py` & `analytix-4.2.1/analytix/reports/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1073,7 +1073,18 @@
 }
 
 LOCATION_AND_TRAFFIC_PLAYLIST_SORT_OPTIONS = {
     "views",
     "estimatedMinutesWatched",
     "playlistStarts",
 }
+
+REVENUE_METRICS = {
+    "estimatedAdRevenue",
+    "estimatedRedPartnerRevenue",
+    "adImpressions",
+    "grossRevenue",
+    "estimatedRevenue",
+    "monetizedPlaybacks",
+    "cpm",
+    "playbackBasedCpm",
+}
```

### Comparing `analytix-4.2.0rc1/analytix/reports/features.py` & `analytix-4.2.1/analytix/reports/features.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "ZeroOrOne",
     "ZeroOrMore",
 )
 
 import typing as t
 
 from analytix import abc
-from analytix.errors import InvalidFeatures, InvalidFeatureSet, InvalidRequest
+from analytix.errors import InvalidRequest
 from analytix.reports import data
 
 
 class _CompareMixin:
     values: set[str]
 
     def __eq__(self, other: object) -> bool:
@@ -92,42 +92,38 @@
             raise InvalidRequest("expected at least 1 metric, got 0")
 
         if not isinstance(inputs, set):
             inputs = set(inputs)
 
         diff = inputs - data.ALL_METRICS
         if diff:
-            raise InvalidFeatures("invalid metric(s) provided", diff)
+            raise InvalidRequest.invalid("metric", diff)
 
         diff = inputs - self.values
         if diff:
-            raise InvalidFeatures(
-                "dimensions and filters are incompatible with metric(s)", diff
-            )
+            raise InvalidRequest.incompatible_metrics(diff)
 
 
 class SortOptions(abc.FeatureType, _CompareMixin):
     def __init__(self, *args: str, descending_only: bool = False) -> None:
         super().__init__(*args)
         self.descending_only = descending_only
 
     def validate(self, inputs: t.Collection[str]) -> None:
-        raw_inputs = set(i.strip("-") for i in inputs)
+        raw_inputs = {i.strip("-") for i in inputs}
         if not isinstance(inputs, set):
             inputs = set(inputs)
 
         diff = raw_inputs - data.ALL_METRICS
         if diff:
-            raise InvalidFeatures("invalid sort option(s) provided", diff)
+            raise InvalidRequest.invalid("sort option", diff)
 
         diff = raw_inputs - self.values
         if diff:
-            raise InvalidFeatures(
-                "dimensions and filters are incompatible with sort option(s)", diff
-            )
+            raise InvalidRequest.incompatible_sort_options(diff)
 
         if self.descending_only:
             diff = {i for i in inputs if not i.startswith("-")}
             if diff:
                 raise InvalidRequest(
                     "dimensions and filters are incompatible with ascending sort "
                     "options (hint: prefix with '-')"
@@ -137,19 +133,18 @@
 class Dimensions(abc.SegmentedFeatureType, _NestedCompareMixin):
     def validate(self, inputs: t.Collection[str]) -> None:
         if not isinstance(inputs, set):
             inputs = set(inputs)
 
         diff = inputs - data.ALL_DIMENSIONS
         if diff:
-            raise InvalidFeatures("invalid dimension(s) provided", diff)
+            raise InvalidRequest.invalid("dimension", diff)
 
-        diff = inputs - self.every
-        if diff:
-            raise InvalidFeatures("incompatible combination of dimensions", inputs)
+        if inputs - self.every:
+            raise InvalidRequest.incompatible_dimensions(inputs)
 
         for set_type in self.values:
             set_type.validate_dimensions(inputs)
 
 
 class Filters(abc.MappingFeatureType, _NestedCompareMixin):
     @property
@@ -169,112 +164,115 @@
 
     def validate(self, inputs: dict[str, str]) -> None:
         keys = set(inputs.keys())
         locked = self.locked
 
         diff = keys - data.ALL_FILTERS
         if diff:
-            raise InvalidFeatures("invalid filter(s) provided", diff)
+            raise InvalidRequest.invalid("filter", diff)
 
         for k, v in inputs.items():
             valid = data.VALID_FILTER_OPTIONS[k]
 
             if valid and (v not in valid):
-                raise InvalidRequest(f"invalid value for filter {k!r}: {v!r}")
+                raise InvalidRequest.invalid_filter_value(k, v)
 
-            if k in locked.keys():
-                if v != locked[k]:
-                    raise InvalidRequest(
-                        "dimensions and filters are incompatible with value "
-                        f"{v!r} for filter {k!r}"
-                    )
+            if k in locked and v != locked[k]:
+                raise InvalidRequest.incompatible_filter_value(k, v)
 
-        diff = keys - self.every_key
-        if diff:
-            raise InvalidFeatures("incompatible combination of filters", keys)
+        if keys - self.every_key:
+            raise InvalidRequest.incompatible_filters(keys)
 
         for set_type in self.values:
             set_type.validate_filters(keys)
 
 
 class Required(abc.SetType, _CompareMixin):
     def validate_dimensions(self, inputs: set[str]) -> None:
         if self.values & inputs == self.values:
             return
 
-        common = len(inputs & self.values)
-        raise InvalidFeatureSet("dimension", "all", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "dimension", self.values, "all", len(inputs & self.values)
+        )
 
     def validate_filters(self, keys: set[str]) -> None:
         if self.expd_keys & keys == self.expd_keys:
             return
 
-        common = len(keys & self.expd_keys)
-        raise InvalidFeatureSet("filter", "all", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "filter", self.values, "all", len(keys & self.values)
+        )
 
 
 class ExactlyOne(abc.SetType, _CompareMixin):
     def validate_dimensions(self, inputs: set[str]) -> None:
         if len(self.values & inputs) == 1:
             return
 
-        common = len(inputs & self.values)
-        raise InvalidFeatureSet("dimension", "1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "dimension", self.values, "1", len(inputs & self.values)
+        )
 
     def validate_filters(self, keys: set[str]) -> None:
         if len(self.expd_keys & keys) == 1:
             return
 
-        common = len(keys & self.expd_keys)
-        raise InvalidFeatureSet("filter", "1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "filter", self.values, "1", len(keys & self.values)
+        )
 
 
 class OneOrMore(abc.SetType, _CompareMixin):
     def validate_dimensions(self, inputs: set[str]) -> None:
         if len(self.values & inputs) > 0:
             return
 
-        common = len(inputs & self.values)
-        raise InvalidFeatureSet("dimension", "at least 1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "dimension", self.values, "at least 1", len(inputs & self.values)
+        )
 
     def validate_filters(self, keys: set[str]) -> None:
         if len(self.expd_keys & keys) > 0:
             return
 
-        common = len(keys & self.expd_keys)
-        raise InvalidFeatureSet("filter", "at least 1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "filter", self.values, "at least 1", len(keys & self.values)
+        )
 
 
 class Optional(abc.SetType, _CompareMixin):
-    def validate_dimensions(self, inputs: set[str]) -> None:
+    def validate_dimensions(self, _: set[str]) -> None:
         # No verifiction required.
         ...
 
-    def validate_filters(self, keys: set[str]) -> None:
+    def validate_filters(self, _: set[str]) -> None:
         # No verifiction required.
         ...
 
 
 class ZeroOrOne(abc.SetType, _CompareMixin):
     def validate_dimensions(self, inputs: set[str]) -> None:
         if len(self.values & inputs) < 2:
             return
 
-        common = len(inputs & self.values)
-        raise InvalidFeatureSet("dimension", "0 or 1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "dimension", self.values, "0 or 1", len(inputs & self.values)
+        )
 
     def validate_filters(self, keys: set[str]) -> None:
         if len(self.expd_keys & keys) < 2:
             return
 
-        common = len(keys & self.expd_keys)
-        raise InvalidFeatureSet("filter", "0 or 1", common, self.values)
+        raise InvalidRequest.invalid_set(
+            "filter", self.values, "0 or 1", len(keys & self.values)
+        )
 
 
 class ZeroOrMore(abc.SetType, _CompareMixin):
-    def validate_dimensions(self, inputs: set[str]) -> None:
+    def validate_dimensions(self, _: set[str]) -> None:
         # No verifiction required.
         ...
 
-    def validate_filters(self, keys: set[str]) -> None:
+    def validate_filters(self, _: set[str]) -> None:
         # No verifiction required.
         ...
```

### Comparing `analytix-4.2.0rc1/analytix/reports/interfaces.py` & `analytix-4.2.1/analytix/reports/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,61 +32,55 @@
 
 import json
 import logging
 import typing as t
 from dataclasses import dataclass
 from enum import Enum
 
-from analytix import errors
-from analytix.utils import process_path, requires
+import analytix
+from analytix.errors import DataFrameConversionError, MissingOptionalComponents
+from analytix.utils import process_path
 
 if t.TYPE_CHECKING:
     import pandas as pd
     import polars as pl
     import pyarrow as pa
 
     from analytix.abc import ReportType
-    from analytix.reports.plots import Plot
     from analytix.types import PathLikeT, ResponseT
 
 _log = logging.getLogger(__name__)
 
 
 class DataType(Enum):
     """An enum representing data types. Can be `STRING`, `INTEGER`,
     or `FLOAT`.
-
-    *New in version 3.0.0.*
     """
 
     STRING = "STRING"
     INTEGER = "INTEGER"
     FLOAT = "FLOAT"
 
 
 class ColumnType(Enum):
     """An enum representing column types. Can be `DIMENSION` or
     `METRIC`.
-
-    *New in version 3.0.0.*
     """
 
     DIMENSION = "DIMENSION"
     METRIC = "METRIC"
 
 
 @dataclass(frozen=True)
 class ColumnHeader:
     """A representation of a column header.
 
     Column headers contain various information about the columns in the
     report. You will never need to create one of these yourself.
 
-    *New in version 3.0.0.*
-
     Parameters
     ----------
     name : str
         The column name.
     data_type : DataType
         The data type of the column.
     column_type : ColumnType
@@ -108,16 +102,14 @@
     data_type: DataType
     column_type: ColumnType
 
     @property
     def data(self) -> ResponseT:
         """The raw data for this column header in JSON format.
 
-        *New in version 4.0.0.*
-
         Returns
         -------
         dict of str-Any
             The response data.
         """
 
         return {
@@ -130,16 +122,14 @@
 @dataclass(frozen=True)
 class ResultTable:
     """A representation of a resultTable resource.
 
     This is the resource type that gets sent from the YouTube Analytics
     API.
 
-    *New in version 4.0.0.*
-
     Parameters
     ----------
     kind : str
         The kind of resource this is. This will always be
         "youtubeAnalytics#resultTable".
     column_headers : list of ColumnHeader
         Information about the columns in the report, such as the name
@@ -167,16 +157,14 @@
     column_headers: list[ColumnHeader]
     rows: list[list[str | int | float]]
 
     @classmethod
     def from_json(cls, data: ResponseT) -> ResultTable:
         """Create a new `ResultTable` instance from JSON data.
 
-        *New in version 4.0.0.*
-
         Parameters
         ----------
         data : JSON object
             The raw JSON data from the API.
 
         Returns
         -------
@@ -197,16 +185,14 @@
             data["rows"],
         )
 
     @property
     def data(self) -> ResponseT:
         """The raw data for this result table in JSON format.
 
-        *New in version 4.0.0.*
-
         Returns
         -------
         dict of str-Any
             The response data.
         """
 
         return {
@@ -219,17 +205,14 @@
 class AnalyticsReport:
     """A representation of an analytics report.
 
     This does not represent a direct resultTable resource, but instead
     provides additional methods on top of one, largely designed to save
     the report data into different formats.
 
-    *Changed in version 4.0.0:* The `data` attribute no longer exists,
-    and the `resource` attribute has been added in its place.
-
     Parameters
     ----------
     data : JSON object
         The raw JSON data from the API.
     type : ReportType
         The report type.
 
@@ -237,16 +220,14 @@
     ----------
     resource : ResultTable
         An instance representing a resultTable resource.
     type : ReportType
         The report type.
     """
 
-    __slots__ = ("resource", "type", "_shape")
-
     def __init__(self, data: ResponseT, type: ReportType) -> None:
         self.resource = ResultTable.from_json(data)
         self.type = type
         self._shape = (len(data["rows"]), len(self.resource.column_headers))
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
@@ -262,16 +243,14 @@
 
     @property
     def shape(self) -> tuple[int, int]:
         """The shape of the report.
 
         This is presented in (rows, columns) format.
 
-        *New in version 2.0.0.*
-
         Returns
         -------
         tuple of two ints
             The shape of the report.
 
         ??? example "Basic example"
             ```py
@@ -288,18 +267,14 @@
 
         return self._shape
 
     @property
     def columns(self) -> list[str]:
         """A list of all columns names in the report.
 
-        *New in version 2.0.0.*
-
-        *Changed in version 3.5.0:* This is now a property.
-
         Returns
         -------
         list of str
             The column list.
 
         !!! info "See also"
             This does not return a list of column headers. If you want
@@ -308,19 +283,14 @@
 
         return [c.name for c in self.resource.column_headers]
 
     @property
     def dimensions(self) -> list[str]:
         """A list of all dimensions in the report.
 
-        *New in version 3.3.0.*
-
-        *Changed in version 4.0.0:* This now returns a list of ordered
-        dimensions.
-
         Returns
         -------
         list of str
             The dimension list.
         """
 
         return [
@@ -329,19 +299,14 @@
             if c.column_type == ColumnType.DIMENSION
         ]
 
     @property
     def metrics(self) -> list[str]:
         """A list of all metrics in the report.
 
-        *New in version 3.3.0.*
-
-        *Changed in version 4.0.0:* This now returns a list of ordered
-        metrics.
-
         Returns
         -------
         list of str
             The metric list.
         """
 
         return [
@@ -350,16 +315,14 @@
             if c.column_type == ColumnType.METRIC
         ]
 
     @property
     def numeric(self) -> list[str]:
         """A list of all numerical columns in the report.
 
-        *New in version 4.0.0.*
-
         Returns
         -------
         list of str
             The list of numerical columns.
         """
 
         return [
@@ -368,40 +331,39 @@
             if c.data_type != DataType.STRING
         ]
 
     @property
     def non_numeric(self) -> list[str]:
         """A list of all non-numerical columns in the report.
 
-        *New in version 4.0.0.*
-
         Returns
         -------
         list of str
             The list of non-numerical columns.
         """
 
         return [
             c.name
             for c in self.resource.column_headers
             if c.data_type == DataType.STRING
         ]
 
     def to_json(
-        self, path: PathLikeT, *, indent: int | None = 4, overwrite: bool = True
+        self,
+        path: PathLikeT,
+        *,
+        indent: int | None = 4,
+        overwrite: bool = True,
+        **kwargs: t.Any,
     ) -> ResponseT:
         """Save this report in JSON format.
 
         This saves the data as it arrived from the YouTube Analytics
         API.
 
-        *New in version 1.0.0.*
-
-        *Changed in version 4.0.0:* Added the `overwrite` parameter.
-
         Parameters
         ----------
         path : Path object or str
             The path to save the file to.
         indent : int, optional
             The number of spaces to indent each line of the data. To
             create a one-line file, pass `None`.
@@ -409,14 +371,19 @@
             Whether to overwrite an existing file.
 
         Returns
         -------
         dict of str-Any
             The raw JSON data.
 
+        Other Parameters
+        ----------------
+        **kwargs : mapping of Any
+            Additional arguments to pass to `json.dump()`.
+
         ??? example "Basic example"
             ```py
             >>> report.to_json("output.json")
             ```
 
         ??? example "Saving in a minimal format"
             ```py
@@ -426,34 +393,28 @@
             ```
         """
 
         path = process_path(path, ".json", overwrite)
         data = self.resource.data
 
         with open(path, "w") as f:
-            json.dump(data, f, indent=indent)
+            json.dump(data, f, indent=indent, **kwargs)
 
         _log.info(f"Saved report as JSON to {path.resolve()}")
         return data
 
     def to_csv(
         self, path: PathLikeT, *, delimiter: str = ",", overwrite: bool = True
     ) -> None:
         """Save this report as a CSV or TSV file.
 
         The filetype is dependent on the delimiter you provide — if you
         pass a tab character as a delimiter, the file will be saved as
         a TSV. It will be saved as a CSV in all other cases.
 
-        *New in version 1.0.0.*
-
-        *Changed in version 3.0.0:* Added TSV support.
-
-        *Changed in version 4.0.0:* Added the `overwrite` parameter.
-
         Parameters
         ----------
         path : Path object or str
             The path to save the file to.
         delimiter : int, optional
             The character to use as a delimiter.
         overwrite : bool, optional
@@ -481,24 +442,19 @@
             f.write(f"{delimiter.join(self.columns)}\n")
             for row in self.resource.rows:
                 line = delimiter.join(f"{v}" for v in row)
                 f.write(f"{line}\n")
 
         _log.info(f"Saved report as {extension[1:].upper()} to {path.resolve()}")
 
-    @requires("openpyxl")
     def to_excel(
         self, path: PathLikeT, *, sheet_name: str = "Analytics", overwrite: bool = True
     ) -> None:
         """Save this report as an Excel spreadsheet.
 
-        *New in version 3.1.0.*
-
-        *Changed in version 4.0.0:* Added the `overwrite` parameter.
-
         Parameters
         ----------
         path : Path object or str
             The path to save the spreadsheet to.
         sheet_name : str, optional
             The name to give the sheet the data will be inserted into.
         overwrite : bool, optional
@@ -524,40 +480,37 @@
 
         ??? example "Saving with a custom sheet name"
             ```py
             >>> report.to_excel("output.xlsx", sheet_name="My Sheet")
             ```
         """
 
+        if not analytix.can_use("openpyxl"):
+            raise MissingOptionalComponents("openpyxl")
+
         from openpyxl import Workbook
 
         path = process_path(path, ".xlsx", overwrite)
         wb = Workbook()
         ws = wb.active
         ws.title = sheet_name
 
         ws.append(self.columns)
         for row in self.resource.rows:
             ws.append(row)
 
         wb.save(str(path))
         _log.info(f"Saved report as spreadsheet to {path.resolve()}")
 
-    @requires("pandas")
     def to_pandas(self, *, skip_date_conversion: bool = False) -> pd.DataFrame:
         """Return this report as a pandas DataFrame.
 
-        *New in version 1.0.0.*
-
-        *Changed in version 3.0.0:* Added `skip_date_conversion`
-        parameter.
-
-        *Changed in version 3.1.0:* Added native Modin support.
-
-        *Changed in version 4.0.0:* Removed native Modin support.
+        If Modin is installed, it will automatically be used instead of
+        pandas. However, you will need to select and initialise your
+        preferred engine before calling this method.
 
         Parameters
         ----------
         skip_date_conversion : bool, optional
             Whether or not to skip the conversion of "day" and "month"
             columns into the `datetime64[ns]` format. If you choose to
             skip this, these columns will be left as strings.
@@ -580,38 +533,38 @@
             1 2022-06-21   1062     32         8         3.558
             2 2022-06-22    946     38         6         2.910
             3 2022-06-23   5107    199        15        24.428
             4 2022-06-24   2137     61         2         6.691
             ```
         """
 
-        import pandas as pd
+        if not analytix.can_use("pandas"):
+            raise MissingOptionalComponents("pandas")
 
         if not self._shape[0]:
-            raise errors.DataFrameConversionError(
+            raise DataFrameConversionError(
                 "cannot convert to DataFrame as the returned data has no rows"
             )
 
+        import pandas as pd
+
         df = pd.DataFrame(self.resource.rows, columns=self.columns)
 
         if not skip_date_conversion:
             s = {"day", "month"} & set(df.columns)
             if len(s):
                 col = next(iter(s))
                 df[col] = pd.to_datetime(df[col], format="%Y-%m-%d")
                 _log.info(f"Converted {col!r} column to datetime64[ns] format")
 
         return df
 
-    @requires("pyarrow")
     def to_arrow(self, *, skip_date_conversion: bool = False) -> pa.Table:
         """Return this report as a Apache Arrow table.
 
-        *New in version 3.2.0.*
-
         Parameters
         ----------
         skip_date_conversion : bool, optional
             Whether or not to skip the conversion of "day" and "month"
             columns into the `timestamp[ns]` format. If you choose to
             skip this, these columns will be left as strings.
 
@@ -639,14 +592,22 @@
             views: [[778,1062,946,5107,2137]]
             likes: [[8,32,38,199,61]]
             comments: [[0,8,6,15,2]]
             grossRevenue: [[2.249,3.558,2.91,24.428,6.691]]
             ```
         """
 
+        if not analytix.can_use("pyarrow"):
+            raise MissingOptionalComponents("pyarrow")
+
+        if not self._shape[0]:
+            raise DataFrameConversionError(
+                "cannot convert to Arrow table as the returned data has no rows"
+            )
+
         import pyarrow as pa
         import pyarrow.compute as pc
 
         table = pa.table(list(zip(*self.resource.rows)), names=self.columns)
 
         if not skip_date_conversion:
             s = {"day", "month"} & set(table.column_names)
@@ -655,20 +616,17 @@
                 fmt = {"day": "%Y-%m-%d", "month": "%Y-%m"}[col]
                 dt_series = pc.strptime(table.column(col), format=fmt, unit="ns")
                 table = table.set_column(0, "day", dt_series)
                 _log.info(f"Converted {col!r} column to timestamp[ns] format")
 
         return table
 
-    @requires("polars")
     def to_polars(self, *, skip_date_conversion: bool = False) -> pl.DataFrame:
         """Return the data as a Polars DataFrame.
 
-        *New in version 3.6.0.*
-
         Parameters
         ----------
         skip_date_conversion : bool, optional
             Whether or not to skip the conversion of "day" and "month"
             columns into the `date` format. If you choose to skip this,
             these columns will be left as strings.
 
@@ -700,43 +658,48 @@
             │ 2022-06-23 ┆ 5107  ┆ 199   ┆ 15       ┆ 24.428       │
             ├╌╌╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌┼╌╌╌╌╌╌╌╌╌╌╌╌╌╌┤
             │ 2022-06-24 ┆ 2137  ┆ 61    ┆ 2        ┆ 6.691        │
             └────────────┴───────┴───────┴──────────┴──────────────┘
             ```
         """
 
+        if not analytix.can_use("polars"):
+            raise MissingOptionalComponents("polars")
+
+        if not self._shape[0]:
+            raise DataFrameConversionError(
+                "cannot convert to DataFrame as the returned data has no rows"
+            )
+
         import polars as pl
 
-        df = pl.DataFrame(self.resource.rows, columns=self.columns)
+        df = pl.DataFrame(self.resource.rows, schema=self.columns)
 
         if not skip_date_conversion:
             s = {"day", "month"} & set(df.columns)
             if len(s):
                 col = next(iter(s))
                 fmt = {"day": "%Y-%m-%d", "month": "%Y-%m"}[col]
-                df = df.with_column(pl.col(col).str.strptime(pl.Date, fmt=fmt))
+                df = df.with_columns(pl.col(col).str.strptime(pl.Date, format=fmt))
                 _log.info(f"Converted {col!r} column to date format")
 
         return df
 
-    @requires("pyarrow")
     def to_feather(
         self,
         path: PathLikeT,
         *,
         skip_date_conversion: bool = False,
         overwrite: bool = True,
     ) -> pa.Table:
         """Save this report as an Apache Feather file.
 
         To do this, the data is first converted to an Apache Arrow
         table, which is returned from the method.
 
-        *New in version 3.2.0*.
-
         Parameters
         ----------
         path : Path object or str
             The path to save the file to.
         skip_date_conversion : bool, optional
             Whether or not to skip the conversion of "day" and "month"
             columns into the `timestamp[ns]` format. If you choose to
@@ -757,37 +720,37 @@
             ```py
             >>> table = report.to_feather("output.feather")
             >>> table.shape
             (7, 5)
             ```
         """
 
+        if not analytix.can_use("pyarrow"):
+            raise MissingOptionalComponents("pyarrow")
+
         import pyarrow.feather as pf
 
         path = process_path(path, ".feather", overwrite)
         table = self.to_arrow(skip_date_conversion=skip_date_conversion)
         pf.write_feather(table, path)
         _log.info(f"Saved report as Apache Feather file to {path.resolve()}")
         return table
 
-    @requires("pyarrow")
     def to_parquet(
         self,
         path: PathLikeT,
         *,
         skip_date_conversion: bool = False,
         overwrite: bool = True,
     ) -> pa.Table:
         """Save this report as an Apache Parquet file.
 
         To do this, the data is first converted to an Apache Arrow
         table, which is returned from the method.
 
-        *New in version 3.2.0*.
-
         Parameters
         ----------
         path : Path object or str
             The path to save the file to.
         skip_date_conversion : bool, optional
             Whether or not to skip the conversion of "day" and "month"
             columns into the `timestamp[ns]` format. If you choose to
@@ -808,108 +771,17 @@
             ```py
             >>> table = report.to_parquet("output.parquet")
             >>> table.shape
             (7, 5)
             ```
         """
 
+        if not analytix.can_use("pyarrow"):
+            raise MissingOptionalComponents("pyarrow")
+
         import pyarrow.parquet as pq
 
         path = process_path(path, ".parquet", overwrite)
         table = self.to_arrow(skip_date_conversion=skip_date_conversion)
         pq.write_table(table, path)
         _log.info(f"Saved report as Apache Parquet file to {path.resolve()}")
         return table
-
-    @requires("matplotlib")
-    def plot(
-        self,
-        metrics: t.Collection[str] | None = None,
-        *,
-        size: tuple[int, int] | None = None,
-    ) -> Plot:
-        """Plots report data.
-
-        This method is largely automatic in that analytix will
-        automatically select the most conventionally appropriate way to
-        represent the data. Many formatting options are abstracted away
-        from you, so you will need to do you own plotting if you need
-        more than what this method can do.
-
-        If a pie chart is created, only a maximum of 10 wedges are
-        included. The first 9 will represent the data with the largest
-        values, and the final wedge will represent the rest of the data.
-
-        *New in version 4.2.0.*
-
-        Parameters
-        ----------
-        metrics : Collection of str, optional
-            The metrics to plot. Each metric is plotted on it's own
-            subplot. If no metrics are provided, the first available
-            metric is used.
-        size : tuple of two ints, optional
-            The width and height of the figure in inches. If this is
-            not provided, Matplotlib determines the size automatically.
-
-        Returns
-        -------
-        Plot
-            The plot instance.
-
-        Raises
-        ------
-        PlottingError
-            Something went wrong during plotting.
-
-        !!! note
-            This requires `matplotlib` to be installed to use, which is
-            an optional dependency. It can be installed using `pip
-            install analytix[plots]`.
-
-        ??? example "Basic example"
-            ```py
-            >>> plot = report.plot()
-            ```
-
-        ??? example "Advanced example"
-            ```py
-            >>> plot = report.plot(("views", "likes"), size=(12, 6))
-            ```
-
-        ??? example "Showing the plot"
-            ```py
-            >>> plot = report.plot(("views",))
-            >>> plot.show()
-            ```
-
-        ??? example "Saving the plot"
-            ```py
-            >>> plot = report.plot(("views",))
-            >>> plot.save("figure.png")
-            ```
-        """
-
-        from analytix.reports import plots
-
-        if len(self.dimensions) != 1:
-            raise errors.PlottingError("the report must have exactly one dimension")
-
-        dimension = self.dimensions[0]
-        metrics = metrics or (self.metrics[0],)
-
-        diff = set(metrics) - set(self.metrics)
-        if diff:
-            raise errors.PlottingError(
-                f"cannot plot non-existent metrics: {', '.join(diff)}"
-            )
-
-        if dimension in ("day", "month"):
-            _log.info("Plotting line graph for time-series data")
-            return plots.TimeSeriesPlot(self.resource, str(self.type), metrics, size)
-
-        if dimension == "elapsedVideoTimeRatio":
-            _log.info("Plotting line graph for linear data")
-            return plots.LinearPlot(self.resource, str(self.type), metrics, size)
-
-        _log.info("Plotting pie chart for categorical data")
-        return plots.CategoricalPlot(self.resource, str(self.type), metrics, size)
```

### Comparing `analytix-4.2.0rc1/analytix/reports/types.py` & `analytix-4.2.1/analytix/reports/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "ViewerDemographicsPlaylist",
     "TopPlaylists",
     "AdPerformance",
 )
 
 import logging
 import typing as t
+import warnings
 
 from analytix.abc import DetailedReportType, ReportType
 from analytix.errors import InvalidRequest
 from analytix.reports import data
 from analytix.reports.features import (
     Dimensions,
     ExactlyOne,
@@ -89,14 +90,15 @@
     OneOrMore,
     Optional,
     Required,
     SortOptions,
     ZeroOrMore,
     ZeroOrOne,
 )
+from analytix.warnings import CityReportWarning
 
 _log = logging.getLogger(__name__)
 
 
 class BasicUserActivity(ReportType):
     def __init__(self) -> None:
         self.name = "Basic user activity"
@@ -206,17 +208,19 @@
         filters: dict[str, str],
         metrics: t.Collection[str],
         sort_options: t.Collection[str],
         max_results: int = 0,
         start_index: int = 1,
     ) -> None:
         if 25 < max_results <= 250:
-            _log.warning(
+            warnings.warn(
                 "While the documentation says city reports can have a maximum of 250 "
-                "results, the actual maximum the API accepts (currently) is 25"
+                "results, the actual maximum the API accepts (currently) is 25",
+                CityReportWarning,
+                stacklevel=5,
             )
 
         if "province" in dimensions:
             # Change the filters on the fly to confirm with special
             # rules for this report type.
             self.filters = Filters(Required("country==US"), ZeroOrOne("video", "group"))
 
@@ -451,17 +455,16 @@
     ) -> None:
         super().validate(
             dimensions, filters, metrics, sort_options, max_results, start_index
         )
 
         itst = filters["insightTrafficSourceType"]
         if itst not in data.VALID_FILTER_OPTIONS["insightTrafficSourceDetail"]:
-            raise InvalidRequest(
-                "dimensions and filters are incompatible with value "
-                f"{itst!r} for filter 'insightTrafficSourceType'"
+            raise InvalidRequest.incompatible_filter_value(
+                "insightTrafficSourceType", itst
             )
 
 
 class DeviceType(ReportType):
     def __init__(self) -> None:
         self.name = "Device types"
         self.dimensions = Dimensions(
@@ -816,17 +819,16 @@
     ) -> None:
         super().validate(
             dimensions, filters, metrics, sort_options, max_results, start_index
         )
 
         itst = filters["insightTrafficSourceType"]
         if itst not in data.VALID_FILTER_OPTIONS["insightTrafficSourceDetail"]:
-            raise InvalidRequest(
-                "dimensions and filters are incompatible with value "
-                f"{itst!r} for filter 'insightTrafficSourceType'"
+            raise InvalidRequest.incompatible_filter_value(
+                "insightTrafficSourceType", itst
             )
 
 
 class DeviceTypePlaylist(ReportType):
     def __init__(self) -> None:
         self.name = "Device types for playlists"
         self.dimensions = Dimensions(
```

### Comparing `analytix-4.2.0rc1/analytix/shard.py` & `analytix-4.2.1/analytix/shard.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,30 @@
 you.
 """
 
 from __future__ import annotations
 
 __all__ = ("Shard",)
 
-import datetime
 import logging
 import typing as t
+import warnings
 from dataclasses import dataclass
 
-from aiohttp import ClientSession
-
 from analytix import OAUTH_CHECK_URL, oidc
 from analytix.errors import APIError, RefreshTokenExpired
 from analytix.groups import GroupItemList, GroupList
 from analytix.queries import GroupItemQuery, GroupQuery, ReportQuery
 from analytix.reports import AnalyticsReport
+from analytix.warnings import ForbiddenWarning
+
+if t.TYPE_CHECKING:
+    import datetime
+
+    from aiohttp import ClientSession
 
 _log = logging.getLogger(__name__)
 
 
 @dataclass()
 class Shard:
     """A shard interface capable of interacting with the YouTube
@@ -68,19 +72,20 @@
 
     !!! info "See also"
         If you're building simple scripts or a desktop-based
         application, the `AsyncClient` performs shard management for
         you.
     """
 
-    __slots__ = ("_session", "_secrets", "_tokens")
+    __slots__ = ("_session", "_secrets", "_tokens", "_scopes")
 
     _session: ClientSession
     _secrets: oidc.Secrets
     _tokens: oidc.Tokens
+    _scopes: oidc.Scopes
 
     def __str__(self) -> str:
         return self._secrets.project_id
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(project_id={self._secrets.project_id!r})"
 
@@ -91,14 +96,22 @@
                 raise APIError(resp.status, str(resp.reason))
 
             data: dict[str, t.Any] = await resp.json()
             _log.debug(f"Response data: {data}")
 
         if next(iter(data)) == "error":
             error = data["error"]
+            if error["code"] == 403:
+                warnings.warn(
+                    "A 403 error may indicate a problem getting revenue data; if your "
+                    "channel is not partnered, configure your client to only use the "
+                    "Scopes.READONLY scope",
+                    ForbiddenWarning,
+                    stacklevel=4,
+                )
             raise APIError(error["code"], error["message"])
 
         return data
 
     async def token_refresh_required(self) -> bool:
         async with self._session.get(
             OAUTH_CHECK_URL + self._tokens.access_token
@@ -161,15 +174,15 @@
             start_date,
             end_date,
             currency,
             start_index,
             include_historical_data,
         )
 
-        query.validate()
+        query.validate(self._scopes)
         assert query.rtype is not None
         data = await self._request(query.url)
         report = AnalyticsReport(data, query.rtype)
         _log.info(f"Created report of shape {report.shape}!")
         return report
 
     async def fetch_groups(
```

### Comparing `analytix-4.2.0rc1/analytix/types.py` & `analytix-4.2.1/analytix/types.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/analytix/utils.py` & `analytix-4.2.1/analytix/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,73 +24,28 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
-__all__ = ("can_use", "requires", "warn", "warn_on_call", "process_path")
+__all__ = ("can_use", "process_path")
 
-import logging
 import typing as t
-import warnings
-from functools import wraps
 from pathlib import Path
 
 from pkg_resources import working_set
 
-from analytix.errors import MissingOptionalComponents
-
 if t.TYPE_CHECKING:
     from analytix.types import PathLikeT
 
-    _FuncT = t.Callable[..., t.Any]
-
-_log = logging.getLogger(__name__)
 
-
-def can_use(*packages: str, required: bool = False) -> bool:
+def can_use(*packages: str) -> bool:
     ws = [p.key for p in working_set]
-    can_use = all(p in ws for p in packages)
-
-    if required and not can_use:
-        raise MissingOptionalComponents(*packages)
-
-    return can_use
-
-
-def requires(*packages: str) -> t.Callable[[_FuncT], _FuncT]:
-    def decorator(func: _FuncT) -> _FuncT:
-        @wraps(func)
-        def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
-            can_use(*packages, required=True)
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorator
-
-
-def warn(message: str) -> None:
-    if _log.hasHandlers() and _log.getEffectiveLevel() <= 30:
-        _log.warning(message)
-    else:
-        warnings.warn(message)
-
-
-def warn_on_call(message: str) -> t.Callable[[_FuncT], _FuncT]:
-    def decorator(func: _FuncT) -> _FuncT:
-        @wraps(func)
-        def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
-            warn(message)
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    return decorator
+    return all(p in ws for p in packages)
 
 
 def process_path(path: PathLikeT, extension: str, overwrite: bool) -> Path:
     if not isinstance(path, Path):
         path = Path(path)
 
     if path.suffix != extension:
```

### Comparing `analytix-4.2.0rc1/analytix/ux.py` & `analytix-4.2.1/analytix/ux.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,33 +28,38 @@
 
 """User experience utilities for analytix."""
 
 from __future__ import annotations
 
 __all__ = ("display_splash", "enable_logging")
 
+import json
 import logging
+import os
 import platform
+import sys
 import typing as t
+import warnings
 from importlib.util import find_spec
+from urllib import request
 
 import analytix
 
 BANNER = r"""
 {r}            {o}             {y}            {g}88  {b}             {i}         {v}88
 {r}            {o}             {y}            {g}88  {b}             {i}  ,d     {v}""
 {r}            {o}             {y}            {g}88  {b}             {i}  88
 {r},adPPYYba,  {o}8b,dPPYba,   {y},adPPYYba,  {g}88  {b}8b       d8  {i}MM88MMM  {v}88  {l}8b,     ,d8
 {r}""     `Y8  {o}88P'   `"8a  {y}""     `Y8  {g}88  {b}`8b     d8'  {i}  88     {v}88  {l} `Y8, ,8P'
 {r},adPPPPP88  {o}88       88  {y},adPPPPP88  {g}88  {b} `8b   d8'   {i}  88     {v}88  {l}   )888(
 {r}88,    ,88  {o}88       88  {y}88,    ,88  {g}88  {b}  `8b,d8'    {i}  88,    {v}88  {l} ,d8" "8b,
 {r}`"8bbdP"Y8  {o}88       88  {y}`"8bbdP"Y8  {g}88  {b}    Y88'     {i}  "Y888  {v}88  {l}8P'     `Y8
 {r}            {o}             {y}            {g}    {b}    d8'
 {r}            {o}             {y}            {g}    {b}   d8' {x}
-""".format(
+""".format(  # noqa: E501
     r="\33[38;5;1m",
     o="\33[38;5;208m",
     y="\33[38;5;3m",
     g="\33[38;5;2m",
     b="\33[38;5;4m",
     i="\33[38;5;135m",
     v="\33[38;5;213m",
@@ -62,36 +67,54 @@
     x="\33[0m",
 )
 
 
 def _install_location() -> str:
     spec = find_spec("analytix")
 
-    if spec:
-        if spec.submodule_search_locations:
-            return spec.submodule_search_locations[0]
+    if spec and spec.submodule_search_locations:
+        return spec.submodule_search_locations[0]
 
     return "unknown"
 
 
 def display_splash() -> None:
-    print(
+    r = "\33[38;5;1m"
+    o = "\33[38;5;208m"
+    y = "\33[38;5;3m"
+    g = "\33[38;5;2m"
+    b = "\33[38;5;4m"
+    l = "\33[38;5;219m"  # noqa: E741
+
+    resp = request.urlopen(analytix.UPDATE_CHECK_URL)  # noqa: S310
+    if resp.status == 200:
+        data = json.loads(resp.read().decode("utf-8"))
+        latest = data["info"]["version"]
+        linfo = (
+            f"{g}latest\33[0m"
+            if latest == analytix.__version__
+            else f"{y}latest is {latest}\33[0m"
+        )
+    else:
+        linfo = f"{o}latest N/A\33[0m"
+
+    print(  # noqa: T201
         BANNER + "\n"
         "\33[3mA simple yet powerful wrapper for the YouTube Analytics API.\33[0m\n\n"
-        f"You're using version \33[1m\33[38;5;1m{analytix.__version__}\33[0m.\n\n"
-        f"\33[1m\33[38;5;4mInformation:\33[0m\n"
+        f"You're using version \33[1m{r}{analytix.__version__}\33[0m ({linfo}).\n\n"
+        f"\33[1m{b}Information:\33[0m\n"
         f" • Python version: {platform.python_version()} "
         f"({platform.python_implementation()})\n"
         f" • Operating system: {platform.system()} ({platform.release()})\n"
         f" • Installed in: {_install_location()}\n\n"
-        f"\33[1m\33[38;5;2mUseful links:\33[0m\n"
+        f"\33[1m{g}Useful links:\33[0m\n"
         f" • Documentation: \33[4m{analytix.__docs__}\33[0m\n"
         f" • Source: \33[4m{analytix.__url__}\33[0m\n"
         f" • Changelog: \33[4m{analytix.__changelog__}\33[0m\n\n"
-        f"\33[1m\33[38;5;219mThanks for using analytix!\33[0m"
+        f"\33[1m{l}Thanks for using analytix!\33[0m"
     )
 
 
 def enable_logging(level: int = logging.INFO) -> logging.StreamHandler[t.TextIO]:
     """Enable analytix's preconfigured logger.
 
     Parameters
@@ -106,31 +129,51 @@
 
     ??? example
         ```py
         analytix.enable_logging(logging.DEBUG)
         ```
     """
 
-    FMT = "{relativeCreated:>7,.0f}ms [ {levelname:<7} ] {name}: {message}"
-    FORMATS = {
-        logging.DEBUG: f"\33[38;5;244m{FMT}\33[0m",
-        logging.INFO: f"\33[38;5;248m{FMT}\33[0m",
-        logging.WARNING: f"\33[1m\33[38;5;178m{FMT}\33[0m",
-        logging.ERROR: f"\33[1m\33[38;5;196m{FMT}\33[0m",
-        logging.CRITICAL: f"\33[1m\33[48;5;196m{FMT}\33[0m",
+    fmt = "{relativeCreated:>7,.0f}ms [ {levelname:<7} ] {name}: {message}"
+    formats = {
+        logging.DEBUG: f"\33[38;5;244m{fmt}\33[0m",
+        logging.INFO: f"\33[38;5;248m{fmt}\33[0m",
+        logging.WARNING: f"\33[1m\33[38;5;178m{fmt}\33[0m",
+        logging.ERROR: f"\33[1m\33[38;5;196m{fmt}\33[0m",
+        logging.CRITICAL: f"\33[1m\33[48;5;196m{fmt}\33[0m",
     }
 
     class CustomFormatter(logging.Formatter):
         def format(self, record: logging.LogRecord) -> str:
-            log_fmt = FORMATS[record.levelno]
+            log_fmt = formats[record.levelno]
             formatter = logging.Formatter(log_fmt, style="{")
             return formatter.format(record)
 
     handler = logging.StreamHandler()
     handler.setFormatter(CustomFormatter())
-    logging.basicConfig(
-        level=level,
-        handlers=[handler],
-    )
+    logging.basicConfig(level=level, handlers=[handler])
+    logging._srcfile = None
+    logging.logThreads = False
+    logging.logProcesses = False
+    logging.logMultiprocessing = False
+
+    def showwarning(
+        message: Warning | str,
+        category: type[Warning],
+        filename: str,
+        lineno: int,
+        file: t.TextIO | None = None,
+        line: str | None = None,
+    ) -> None:
+        for _module_name, module in sys.modules.items():
+            module_path = getattr(module, "__file__", None)
+            if module_path and os.path.samefile(module_path, filename):
+                break
+        else:
+            _module_name = os.path.splitext(os.path.split(filename)[1])[0]
+        log = logging.getLogger(_module_name)
+        log.warning(message)
+
+    warnings.simplefilter("always", DeprecationWarning)
+    warnings.showwarning = showwarning
 
-    logging.getLogger("matplotlib.font_manager").setLevel(logging.WARNING)
     return handler
```

### Comparing `analytix-4.2.0rc1/analytix.egg-info/PKG-INFO` & `analytix-4.2.1/analytix.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: analytix
-Version: 4.2.0rc1
+Version: 4.2.1
 Summary: A simple yet powerful wrapper for the YouTube Analytics API.
 Home-page: https://github.com/parafoxia/analytix
 Author: Ethan Henderson
 Author-email: ethan.henderson.1998@gmail.com
 License: BSD 3-Clause 'New' or 'Revised' License
-Project-URL: Documentation, https://parafoxia.github.io/analytix/
+Project-URL: Documentation, https://parafoxia.github.io/analytix
 Project-URL: Source, https://github.com/parafoxia/analytix
 Project-URL: Bug Tracker, https://github.com/parafoxia/analytix/issues
 Project-URL: CI, https://github.com/parafoxia/analytix/actions
 Project-URL: Changelog, https://github.com/parafoxia/analytix/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
@@ -100,25 +100,30 @@
 You may need to prefix these commands with a call to the Python interpreter depending on your OS and Python configuration.
 
 ## Additional support
 
 You can also install analytix with additional libraries to provide extra functionality:
 
 * `analytix[excel]` — support for exporting reports to Excel spreadsheets
-* `analytix[plots]` — support for plotting graphs for reports
 * `analytix[types]` — type stubs for type-hinted projects
 
 To install multiple at once, use commas:
 
 ```sh
-pip install "analytix[excel,plots,types]"
+pip install "analytix[excel,types]"
 ```
 
-Note that while analytix includes native support for DataFrame and Arrow table conversions, these libraries are not installed automatically.
-You will need to install these libraries yourself to use these features.
+Support for DataFrame and Arrow table conversions is also present.
+analytix supports these libraries natively:
+
+* `pandas` >= 0.23.2
+* `pyarrow` >= 2.0.0
+* `polars` >= 0.17.3
+
+Note: You will need to install your library of choice manually to be able to use it.
 
 ## OAuth authentication
 
 All requests to the YouTube Analytics API need to be authorised through OAuth 2.
 In order to do this, you will need a Google Developers project with the YouTube Analytics API enabled.
 You can find instructions on how to do that in the [API setup guide](https://parafoxia.github.io/analytix/starting/googleapp/), or on [this video](https://www.youtube.com/watch?v=1Xday10ZWeg).
 
@@ -140,14 +145,16 @@
 analytix.enable_logging()
 ```
 
 If anything is going wrong, or analytix appears to be taking a long time to fetch data, try enabling the logger in DEBUG mode.
 
 ## Usage
 
+### Retrieving reports
+
 Retrieving reports from the YouTube Analytics API is easy.
 The below example loads credentials from a secrets file, and gets day-by-day data on views, likes, and comments from the US over the last 28 days:
 
 ```py
 from analytix import Client  # or AsyncClient
 
 client = Client("./secrets.json")
@@ -155,33 +162,23 @@
     dimensions=("day",),
     filters={"country": "US"},
     metrics=("views", "likes", "comments"),
 )
 report.to_csv("./analytics.csv")
 ```
 
-If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame:
+If you want to analyse this data using additional tools such as *pandas*, you can directly export the report as a DataFrame or table.
 
 ```py
-# Return as a pandas DataFrame:
 df = report.to_pandas()
-
-# Return as an Apache Arrow table:
 table = report.to_arrow()
-
-# Return as a Polars DataFrame:
 df = report.to_polars()
 ```
 
-If you want to quickly plot the data, you can use the in-built plotter:
-
-```py
-plot = report.plot(("views",), size=(12, 6))
-plot.save("figure.png")
-```
+### Fetching group information
 
 You can also fetch groups and group items:
 
 ```py
 from analytix import Client
 
 client = Client("./secrets.json")
```

### Comparing `analytix-4.2.0rc1/analytix.egg-info/SOURCES.txt` & `analytix-4.2.1/analytix.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 analytix/oidc.py
 analytix/py.typed
 analytix/queries.py
 analytix/shard.py
 analytix/types.py
 analytix/utils.py
 analytix/ux.py
+analytix/warnings.py
 analytix.egg-info/PKG-INFO
 analytix.egg-info/SOURCES.txt
 analytix.egg-info/dependency_links.txt
 analytix.egg-info/requires.txt
 analytix.egg-info/top_level.txt
 analytix/groups/__init__.py
 analytix/groups/groups.py
 analytix/reports/__init__.py
 analytix/reports/data.py
 analytix/reports/features.py
 analytix/reports/interfaces.py
-analytix/reports/plots.py
 analytix/reports/types.py
 requirements/base.txt
 requirements/dev.txt
 requirements/docs.txt
 requirements/excel.txt
-requirements/plots.txt
+requirements/nox.txt
 requirements/types.txt
 tests/__init__.py
 tests/test_groups.py
 tests/test_oidc.py
 tests/test_shard.py
 tests/test_utils.py
```

### Comparing `analytix-4.2.0rc1/setup.py` & `analytix-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/tests/__init__.py` & `analytix-4.2.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/tests/test_groups.py` & `analytix-4.2.1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `analytix-4.2.0rc1/tests/test_oidc.py` & `analytix-4.2.1/tests/test_oidc.py`

 * *Files 17% similar despite different names*

```diff
@@ -158,30 +158,72 @@
         oidc.state_token()
         == "34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
     )
 
 
 @pytest.mark.dependency(depends=["test_state_token"])
 @mock.patch("os.urandom", return_value=b"rickroll")
-def test_auth_uri(mock_urand, secrets, auth_params):
-    uri, params = oidc.auth_uri(secrets, 8080)
+def test_auth_uri_all_scopes(mock_urand, secrets, auth_params):
+    uri, params = oidc.auth_uri(secrets, 8080, oidc.Scopes.ALL)
     # We don't need to test Python's URL encoder.
     assert uri == (
         "https://accounts.google.com/o/oauth2/auth"
         "?client_id=a1b2c3d4e5"
         "&nonce=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
         "&response_type=code"
         "&redirect_uri=http%3A%2F%2Flocalhost%3A8080"
         "&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fyt-analytics.readonly+https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fyt-analytics-monetary.readonly"
         "&state=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
         "&access_type=offline"
     )
     assert params == auth_params
 
 
+@pytest.mark.dependency(depends=["test_state_token"])
+@mock.patch("os.urandom", return_value=b"rickroll")
+def test_auth_uri_readonly_scope(mock_urand, secrets, auth_params):
+    uri, params = oidc.auth_uri(secrets, 8080, oidc.Scopes.READONLY)
+    # We don't need to test Python's URL encoder.
+    assert uri == (
+        "https://accounts.google.com/o/oauth2/auth"
+        "?client_id=a1b2c3d4e5"
+        "&nonce=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
+        "&response_type=code"
+        "&redirect_uri=http%3A%2F%2Flocalhost%3A8080"
+        "&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fyt-analytics.readonly"
+        "&state=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
+        "&access_type=offline"
+    )
+    # Kind of a hack here, need to sort out the fixtures.
+    auth_params["scope"] = "https://www.googleapis.com/auth/yt-analytics.readonly"
+    assert params == auth_params
+
+
+@pytest.mark.dependency(depends=["test_state_token"])
+@mock.patch("os.urandom", return_value=b"rickroll")
+def test_auth_uri_monetary_readonly_scope(mock_urand, secrets, auth_params):
+    uri, params = oidc.auth_uri(secrets, 8080, oidc.Scopes.MONETARY_READONLY)
+    # We don't need to test Python's URL encoder.
+    assert uri == (
+        "https://accounts.google.com/o/oauth2/auth"
+        "?client_id=a1b2c3d4e5"
+        "&nonce=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
+        "&response_type=code"
+        "&redirect_uri=http%3A%2F%2Flocalhost%3A8080"
+        "&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fyt-analytics-monetary.readonly"
+        "&state=34c5f166f6abb229ee092be1e7e92ca71434bcb1a27ba0664cd2fea834d85927"
+        "&access_type=offline"
+    )
+    # Kind of a hack here, need to sort out the fixtures.
+    auth_params[
+        "scope"
+    ] = "https://www.googleapis.com/auth/yt-analytics-monetary.readonly"
+    assert params == auth_params
+
+
 def test_token_uri(secrets, auth_params):
     uri, data, headers = oidc.token_uri(secrets, "rickroll", auth_params)
     assert uri == "https://oauth2.googleapis.com/token"
     assert data == {
         "code": "rickroll",
         "client_id": "a1b2c3d4e5",
         "client_secret": "f6g7h8i9j0",
```

### Comparing `analytix-4.2.0rc1/tests/test_shard.py` & `analytix-4.2.1/tests/test_shard.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 import pytest
 import pytz
 from aiohttp import ClientSession
 
 from analytix.errors import APIError, RefreshTokenExpired
 from analytix.groups import Group, GroupItem, GroupItemList, GroupList
+from analytix.oidc import Scopes
 from analytix.reports import AnalyticsReport
 from analytix.reports.types import TimeBasedActivity
 from analytix.shard import Shard
 from tests import (
     MockResponse,
     create_group_item_data,
     create_group_item_list_data,
@@ -59,15 +60,18 @@
 
 ERROR_DATA = r"""{"error": {"code": 403, "message": "You ain't allowed, son."}}"""
 
 
 @pytest.fixture()
 async def shard():
     return Shard(
-        _session=ClientSession(), _secrets=create_secrets(), _tokens=create_tokens()
+        _session=ClientSession(),
+        _secrets=create_secrets(),
+        _tokens=create_tokens(),
+        _scopes=Scopes.ALL,
     )
 
 
 def test_shard_str(shard):
     assert str(shard) == "rickroll"
     assert f"{shard}" == "rickroll"
```


# Comparing `tmp/jupysql-0.7.5.tar.gz` & `tmp/jupysql-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.5.tar", last modified: Wed May 24 22:55:07 2023, max compression
+gzip compressed data, was "jupysql-0.7.6.tar", last modified: Mon May 29 17:52:44 2023, max compression
```

## Comparing `jupysql-0.7.5.tar` & `jupysql-0.7.6.tar`

### file list

```diff
@@ -1,45 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-24 22:54:48.000000 jupysql-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 22:54:48.000000 jupysql-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 22:55:07.356754 jupysql-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-24 22:54:48.000000 jupysql-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-24 22:54:48.000000 jupysql-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-24 22:55:07.356754 jupysql-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 22:54:48.000000 jupysql-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.344754 jupysql-0.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.348754 jupysql-0.7.5/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 22:55:06.000000 jupysql-0.7.5/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:55:07.356754 jupysql-0.7.5/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-24 22:54:48.000000 jupysql-0.7.5/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-24 22:54:49.000000 jupysql-0.7.5/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-29 17:52:29.000000 jupysql-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 17:52:29.000000 jupysql-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-29 17:52:44.252600 jupysql-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-29 17:52:29.000000 jupysql-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-29 17:52:29.000000 jupysql-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 17:52:44.252600 jupysql-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-29 17:52:29.000000 jupysql-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.248600 jupysql-0.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.7.5/LICENSE` & `jupysql-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/PKG-INFO` & `jupysql-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.5
+Version: 0.7.6
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.5 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.6 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.5/README.md` & `jupysql-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/pyproject.toml` & `jupysql-0.7.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,11 @@
     "--extend-ignore=E402",
     # jupysql notebooks might have "undefined name" errors
     # due to the << operator
     # W503, W504 ignore line break after/before 
     # binary operator since they are conflicting 
     "--ignore=F821, W503, W504",
 ]
+
+[tool.codespell]
+skip = '.git,_build,build,*.drawio,*.ipynb'
+ignore-words-list = 'whis'
```

### Comparing `jupysql-0.7.5/setup.py` & `jupysql-0.7.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "sqlparse",
     "ipython-genutils>=0.1.0",
     "sqlglot",
     "jinja2",
     "sqlglot>=11.3.7",
     "ploomber-core>=0.2.7",
     'importlib-metadata;python_version<"3.8"',
+    "psutil",
 ]
 
 DEV = [
     "flake8",
     "pytest",
     "pandas",
     "polars==0.17.2",  # 04/18/23 this breaks our CI
@@ -43,25 +44,28 @@
     "duckdb-engine",
     "pyodbc",
     # sql.plot module tests
     "matplotlib",
     "black",
     # for %%sql --interact
     "ipywidgets",
+    # for running tests for %sqlcmd explore --table
+    "js2py",
 ]
 
 # dependencies for running integration tests
 INTEGRATION = [
     "dockerctx",
     "pyarrow",
     "psycopg2-binary",
     "pymysql",
     "pgspecial==2.0.1",
     "pyodbc",
     "snowflake-sqlalchemy",
+    "oracledb",
 ]
 
 setup(
     name="jupysql",
     version=VERSION,
     description="Better SQL in Jupyter",
     long_description=README,
```

### Comparing `jupysql-0.7.5/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.6/src/jupysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.5
+Version: 0.7.6
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.5 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.6 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.5/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.6/src/jupysql.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -31,8 +31,14 @@
 src/sql/ggplot/__init__.py
 src/sql/ggplot/aes.py
 src/sql/ggplot/facet_wrap.py
 src/sql/ggplot/ggplot.py
 src/sql/ggplot/geom/__init__.py
 src/sql/ggplot/geom/geom.py
 src/sql/ggplot/geom/geom_boxplot.py
-src/sql/ggplot/geom/geom_histogram.py
+src/sql/ggplot/geom/geom_histogram.py
+src/sql/widgets/__init__.py
+src/sql/widgets/utils.py
+src/sql/widgets/table_widget/__init__.py
+src/sql/widgets/table_widget/table_widget.py
+src/sql/widgets/table_widget/css/tableWidget.css
+src/sql/widgets/table_widget/js/tableWidget.js
```

### Comparing `jupysql-0.7.5/src/jupysql.egg-info/requires.txt` & `jupysql-0.7.6/src/jupysql.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 sqlalchemy
 sqlparse
 ipython-genutils>=0.1.0
 sqlglot
 jinja2
 sqlglot>=11.3.7
 ploomber-core>=0.2.7
+psutil
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [:python_version <= "3.8"]
 ipython<=8.12.0
 
@@ -24,14 +25,15 @@
 twine
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
+js2py
 
 [integration]
 flake8
 pytest
 pandas
 polars==0.17.2
 invoke
@@ -39,13 +41,15 @@
 twine
 duckdb<0.8.0
 duckdb-engine
 pyodbc
 matplotlib
 black
 ipywidgets
+js2py
 dockerctx
 pyarrow
 psycopg2-binary
 pymysql
 pgspecial==2.0.1
 snowflake-sqlalchemy
+oracledb
```

### Comparing `jupysql-0.7.5/src/sql/_patch.py` & `jupysql-0.7.6/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/_testing.py` & `jupysql-0.7.6/src/sql/_testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from contextlib import contextmanager
 import sys
 import time
 import docker
 from docker import errors
 from sqlalchemy.engine import URL
 import os
-
+import sqlalchemy
 
 TMP_DIR = "tmp"
 
 
 class DatabaseConfigHelper:
     @staticmethod
     def get_database_config(database):
@@ -123,14 +123,33 @@
         "alias": "snowflakeTest",
         "docker_ct": None,
         "query": {
             "warehouse": "COMPUTE_WH",
             "role": "SYSADMIN",
         },
     },
+    "oracle": {
+        "drivername": "oracle+oracledb",
+        "username": "ploomber_app",
+        "password": "ploomber_app_password",
+        "admin_password": "ploomber_app_admin_password",
+        # database/schema
+        "host": "localhost",
+        "port": "1521",
+        "alias": "oracle",
+        "database": None,
+        "docker_ct": {
+            "name": "oracle",
+            "image": "gvenzl/oracle-xe",
+            "ports": {1521: 1521},
+        },
+        "query": {
+            "service_name": "XEPDB1",
+        },
+    },
 }
 
 
 # SQLAlchmey URL: https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls
 def _get_database_url(database):
     return URL.create(
         drivername=databaseConfig[database]["drivername"],
@@ -155,45 +174,51 @@
 
 
     :type host: str
     :type port: int
     :type timeout: float
     :type poll_freq: float
     """
-    import sqlalchemy
-
     errors = []
 
     t0 = time.time()
     while time.time() - t0 < timeout:
         try:
             eng = sqlalchemy.create_engine(_get_database_url(database)).connect()
             eng.close()
+            print(f"{database} is initialized successfully")
             return True
         except Exception as e:
+            print(type(e))
             errors.append(str(e))
 
         time.sleep(poll_freq)
 
-    # print all the errors so we know what's goin on since failing to connect might be
+    # print all the errors so we know what's going on since failing to connect might be
     # to some misconfiguration error
     errors_ = "\n".join(errors)
     print(f"ERRORS: {errors_}")
 
-    return False
+    return True
+
+
+def get_docker_client():
+    return docker.from_env(
+        version="auto", environment={"DOCKER_HOST": os.getenv("DOCKER_HOST")}
+    )
 
 
 @contextmanager
 def postgres(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("postgreSQL")
     try:
-        client = docker.from_env(version="auto")
+        client = get_docker_client()
         container = client.containers.get(db_config["docker_ct"]["name"])
         yield container
     except errors.NotFound:
         print("Creating new container: postgreSQL")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
@@ -217,15 +242,15 @@
 @contextmanager
 def mysql(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("mySQL")
     try:
-        client = docker.from_env(version="auto")
+        client = get_docker_client()
         container = client.containers.get(db_config["docker_ct"]["name"])
         yield container
     except errors.NotFound:
         print("Creating new container: mysql")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
@@ -257,15 +282,15 @@
 @contextmanager
 def mariadb(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("mariaDB")
     try:
-        client = docker.from_env(version="auto")
+        client = get_docker_client()
         curr = client.containers.get(db_config["docker_ct"]["name"])
         yield curr
     except errors.NotFound:
         print("Creating new container: mariaDB")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
@@ -297,15 +322,15 @@
 @contextmanager
 def mssql(is_bypass_init=False):
     if is_bypass_init:
         yield None
         return
     db_config = DatabaseConfigHelper.get_database_config("MSSQL")
     try:
-        client = docker.from_env(version="auto")
+        client = get_docker_client()
         curr = client.containers.get(db_config["docker_ct"]["name"])
         yield curr
     except errors.NotFound:
         print("Creating new container: MSSQL")
         with new_container(
             new_container_name=db_config["docker_ct"]["name"],
             image_name=db_config["docker_ct"]["image"],
@@ -323,18 +348,44 @@
                 "-Q 'select 1' -b -o /dev/null",
                 "timeout": 5000000000,
             },
         ) as container:
             yield container
 
 
+@contextmanager
+def oracle(is_bypass_init=False):
+    if is_bypass_init:
+        yield None
+        return
+    db_config = DatabaseConfigHelper.get_database_config("oracle")
+    try:
+        client = get_docker_client()
+        curr = client.containers.get(db_config["docker_ct"]["name"])
+        yield curr
+    except errors.NotFound:
+        print("Creating new container: oracle")
+        with new_container(
+            new_container_name=db_config["docker_ct"]["name"],
+            image_name=db_config["docker_ct"]["image"],
+            ports=db_config["docker_ct"]["ports"],
+            environment={
+                "APP_USER": db_config["username"],
+                "APP_USER_PASSWORD": db_config["password"],
+                "ORACLE_PASSWORD": db_config["admin_password"],
+            },
+            # Oracle takes more time to initialize
+            ready_test=lambda: database_ready(database="oracle"),
+        ) as container:
+            yield container
+
+
 def main():
     print("Starting test containers...")
-
-    with postgres(), mysql(), mariadb(), mssql():
+    with oracle():
         print("Press CTRL+C to exit")
         try:
             while True:
                 time.sleep(5)
         except KeyboardInterrupt:
             print("Exit, containers will be killed")
             sys.exit()
```

### Comparing `jupysql-0.7.5/src/sql/column_guesser.py` & `jupysql-0.7.6/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/command.py` & `jupysql-0.7.6/src/sql/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Encapsulates the parsing logic (arguments, SQL code, connection string, etc.)
 
     """
 
     def __init__(self, magic, user_ns, line, cell) -> None:
         self.args = parse.magic_args(magic.execute, line)
         # self.args.line (everything that appears after %sql/%%sql in the first line)
-        # is splited in tokens (delimited by spaces), this checks if we have one arg
+        # is split in tokens (delimited by spaces), this checks if we have one arg
         one_arg = len(self.args.line) == 1
 
         is_custom_connection_ = (
             Connection.is_custom_connection(user_ns.get(self.args.line[0], False))
             if len(self.args.line) > 0
             else False
         )
@@ -92,9 +92,14 @@
         return self.parsed["connection"]
 
     @property
     def result_var(self):
         """Returns the result_var"""
         return self.parsed["result_var"]
 
+    @property
+    def return_result_var(self):
+        """Returns the return_result_var"""
+        return self.parsed["return_result_var"]
+
     def _var_expand(self, sql, user_ns, magic):
         return Template(sql).render(user_ns)
```

### Comparing `jupysql-0.7.5/src/sql/connection.py` & `jupysql-0.7.6/src/sql/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,27 @@
     # MSSQL
     "pyodbc": "pyodbc",
     "pymssql": "pymssql",
 }
 
 DIALECT_NAME_SQLALCHEMY_TO_SQLGLOT_MAPPING = {"postgresql": "postgres", "mssql": "tsql"}
 
+# All the DBs and their respective documentation links
+DB_DOCS_LINKS = {
+    "duckdb": "https://jupysql.ploomber.io/en/latest/integrations/duckdb.html",
+    "mysql": "https://jupysql.ploomber.io/en/latest/integrations/mysql.html",
+    "mssql": "https://jupysql.ploomber.io/en/latest/integrations/mssql.html",
+    "mariadb": "https://jupysql.ploomber.io/en/latest/integrations/mariadb.html",
+    "clickhouse": "https://jupysql.ploomber.io/en/latest/integrations/clickhouse.html",
+    "postgresql": (
+        "https://jupysql.ploomber.io/en/latest/integrations/postgres-connect.html"
+    ),
+    "questdb": "https://jupysql.ploomber.io/en/latest/integrations/questdb.html",
+}
+
 
 def extract_module_name_from_ModuleNotFoundError(e):
     return e.name
 
 
 def extract_module_name_from_NoSuchModuleError(e):
     return str(e).split(":")[-1].split(".")[-1]
@@ -106,14 +119,37 @@
     sought = sought.split("@")
     for key, val in dct.items():
         if not any(s.lower() not in key.lower() for s in sought):
             return val
     return default
 
 
+def is_pep249_compliant(conn):
+    """
+    Checks if given connection object complies with PEP 249
+    """
+    pep249_methods = [
+        "close",
+        "commit",
+        # "rollback",
+        # "cursor",
+        # PEP 249 doesn't require the connection object to have
+        # a cursor method strictly
+        # ref: https://peps.python.org/pep-0249/#id52
+    ]
+
+    for method_name in pep249_methods:
+        # Checking whether the connection object has the method
+        # and if it is callable
+        if not hasattr(conn, method_name) or not callable(getattr(conn, method_name)):
+            return False
+
+    return True
+
+
 class Connection:
     """Manages connections to databases
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         The SQLAlchemy engine to use
@@ -176,28 +212,40 @@
     @classmethod
     def _suggest_fix(cls, env_var, connect_str=None):
         """
         Returns an error message that we can display to the user
         to tell them how to pass the connection string
         """
         DEFAULT_PREFIX = "\n\n"
+        prefix = ""
 
         if connect_str:
             matches = get_close_matches(connect_str, list(cls.connections), n=1)
+            matches_db = get_close_matches(
+                connect_str.lower(), list(DB_DOCS_LINKS.keys()), cutoff=0.3, n=1
+            )
 
             if matches:
-                prefix = (
+                prefix = prefix + (
                     "\n\nPerhaps you meant to use the existing "
-                    f"connection: %sql {matches[0]!r}?\n\n"
+                    f"connection: %sql {matches[0]!r}?"
                 )
 
-            else:
+            if matches_db:
+                prefix = prefix + (
+                    f"\n\nPerhaps you meant to use the {matches_db[0]!r} db \n"
+                    f"To find more information regarding connection: "
+                    f"{DB_DOCS_LINKS[matches_db[0]]}\n\n"
+                )
+
+            if not matches and not matches_db:
                 prefix = DEFAULT_PREFIX
         else:
             matches = None
+            matches_db = None
             prefix = DEFAULT_PREFIX
 
         connection_string = (
             "Pass a valid connection string:\n    "
             "Example: %sql postgresql://username:password@hostname/dbname"
         )
 
@@ -389,22 +437,17 @@
                 raise exceptions.RuntimeError("No active connection")
             else:
                 conn = Connection.current.session
 
         if isinstance(conn, (CustomConnection, CustomSession)):
             is_custom_connection_ = True
         else:
-            # TODO: Better check when user passes a custom
-            # connection
-            if (
-                isinstance(
-                    conn, (sqlalchemy.engine.base.Connection, Connection, str, bool)
-                )
-                or conn.__class__.__name__ == "DataFrame"
-            ):
+            if isinstance(
+                conn, (sqlalchemy.engine.base.Connection, Connection)
+            ) or not (is_pep249_compliant(conn)):
                 is_custom_connection_ = False
             else:
                 is_custom_connection_ = True
 
         return is_custom_connection_
 
     def _get_curr_sqlalchemy_connection_info(self):
```

### Comparing `jupysql-0.7.5/src/sql/error_message.py` & `jupysql-0.7.6/src/sql/error_message.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/exceptions.py` & `jupysql-0.7.6/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.6/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.6/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/ggplot/ggplot.py` & `jupysql-0.7.6/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/inspect.py` & `jupysql-0.7.6/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/magic.py` & `jupysql-0.7.6/src/sql/magic.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     from pandas.core.frame import DataFrame, Series
 except ModuleNotFoundError:
     DataFrame = None
     Series = None
 
 from sql.telemetry import telemetry
 
+
 SUPPORT_INTERACTIVE_WIDGETS = ["Checkbox", "Text", "IntSlider", ""]
 
 
 @magics_class
 class RenderMagic(Magics):
     """
     %sqlrender magic which prints composed queries
@@ -199,14 +200,20 @@
     @argument(
         "-p",
         "--persist",
         action="store_true",
         help="create a table name in the database from the named DataFrame",
     )
     @argument(
+        "-P",
+        "--persist-replace",
+        action="store_true",
+        help="replace the DataFrame if it exists, otherwise perform --persist",
+    )
+    @argument(
         "-n",
         "--no-index",
         action="store_true",
         help="Do not store Data Frame index when persisting",
     )
     @argument(
         "--append",
@@ -363,19 +370,42 @@
             connect_arg,
             displaycon=self.displaycon,
             connect_args=args.connection_arguments,
             creator=args.creator,
             alias=args.alias,
         )
         payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
-        if args.persist:
+        if args.persist_replace and args.append:
+            raise exceptions.UsageError(
+                """You cannot simultaneously persist and append data to a dataframe;
+                  please choose to utilize either one or the other."""
+            )
+        if args.persist and args.persist_replace:
+            warnings.warn("Please use either --persist or --persist-replace")
+            return self._persist_dataframe(
+                command.sql,
+                conn,
+                user_ns,
+                append=False,
+                index=not args.no_index,
+                replace=True,
+            )
+        elif args.persist:
             return self._persist_dataframe(
                 command.sql, conn, user_ns, append=False, index=not args.no_index
             )
-
+        elif args.persist_replace:
+            return self._persist_dataframe(
+                command.sql,
+                conn,
+                user_ns,
+                append=False,
+                index=not args.no_index,
+                replace=True,
+            )
         if args.append:
             return self._persist_dataframe(
                 command.sql, conn, user_ns, append=True, index=not args.no_index
             )
 
         if not command.sql:
             return
@@ -419,14 +449,16 @@
 
                 self.shell.user_ns.update(result)
 
                 return None
             else:
                 if command.result_var:
                     self.shell.user_ns.update({command.result_var: result})
+                    if command.return_result_var:
+                        return result
                     return None
 
                 # Return results into the default ipython _ variable
                 return result
 
         # JA: added DatabaseError for MySQL
         except (ProgrammingError, OperationalError, DatabaseError) as e:
@@ -443,15 +475,17 @@
                     print(detailed_msg)
                 e.modify_exception = True
                 raise e
 
     legal_sql_identifier = re.compile(r"^[A-Za-z0-9#_$]+")
 
     @modify_exceptions
-    def _persist_dataframe(self, raw, conn, user_ns, append=False, index=True):
+    def _persist_dataframe(
+        self, raw, conn, user_ns, append=False, index=True, replace=False
+    ):
         """Implements PERSIST, which writes a DataFrame to the RDBMS"""
         if not DataFrame:
             raise exceptions.MissingPackageError(
                 "You must install pandas to persist results: pip install pandas"
             )
 
         frame_name = raw.strip(";")
@@ -482,22 +516,30 @@
                 f"{frame_name!r} is not a Pandas DataFrame or Series"
             )
 
         # Make a suitable name for the resulting database table
         table_name = frame_name.lower()
         table_name = self.legal_sql_identifier.search(table_name).group(0)
 
-        if_exists = "append" if append else "fail"
+        if replace:
+            if_exists = "replace"
+        elif append:
+            if_exists = "append"
+        else:
+            if_exists = "fail"
 
         try:
             frame.to_sql(
                 table_name, conn.session.engine, if_exists=if_exists, index=index
             )
-        except ValueError as e:
-            raise exceptions.ValueError(e) from e
+        except ValueError:
+            raise exceptions.ValueError(
+                f"""Table {table_name!r} already exists. Consider using \
+--persist-replace to drop the table before persisting the data frame"""
+            )
 
         return "Persisted %s" % table_name
 
 
 def load_ipython_extension(ip):
     """Load the extension in IPython."""
```

### Comparing `jupysql-0.7.5/src/sql/magic_cmd.py` & `jupysql-0.7.6/src/sql/magic_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 import sql.connection
 from sql import inspect
 import sql.run
 from sql.util import sanitize_identifier
 from sql import exceptions
 
+from sql.widgets import TableWidget
+from IPython.display import display
+
 
 class CmdParser(argparse.ArgumentParser):
     def exit(self, status=0, message=None):
         if message:
             self._print_message(message, sys.stderr)
 
     def error(self, message):
@@ -40,18 +43,18 @@
     @argument("line", type=str, help="Command name")
     def _validate_execute_inputs(self, line):
         """
         Function to validate %sqlcmd inputs.
         Raises UsageError in case of an invalid input, executes command otherwise.
         """
 
-        # We relly on SQLAlchemy when inspecting tables
+        # We rely on SQLAlchemy when inspecting tables
         util.support_only_sql_alchemy_connection("%sqlcmd")
 
-        AVAILABLE_SQLCMD_COMMANDS = ["tables", "columns", "test", "profile"]
+        AVAILABLE_SQLCMD_COMMANDS = ["tables", "columns", "test", "profile", "explore"]
 
         if line == "":
             raise exceptions.UsageError(
                 "Missing argument for %sqlcmd. "
                 "Valid commands are: {}".format(", ".join(AVAILABLE_SQLCMD_COMMANDS))
             )
         else:
@@ -206,14 +209,24 @@
 
             if args.output:
                 with open(args.output, "w") as f:
                     f.write(report._repr_html_())
 
             return report
 
+        elif cmd_name == "explore":
+            parser = CmdParser()
+            parser.add_argument(
+                "-t", "--table", type=str, help="Table name", required=True
+            )
+            args = parser.parse_args(others)
+
+            table_widget = TableWidget(args.table)
+            display(table_widget)
+
 
 def return_test_results(args, conn, query):
     try:
         columns = []
         column_data = conn.execute(text(query)).cursor.description
         res = conn.execute(text(query)).fetchall()
         for column in column_data:
```

### Comparing `jupysql-0.7.5/src/sql/magic_plot.py` & `jupysql-0.7.6/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/parse.py` & `jupysql-0.7.6/src/sql/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,28 +34,38 @@
     special parsing.
     Instead, add @arguments to SqlMagic.execute.
 
     We're grandfathering the
     connection string and `<<` operator in.
     """
 
-    result = {"connection": "", "sql": "", "result_var": None}
+    result = {
+        "connection": "",
+        "sql": "",
+        "result_var": None,
+        "return_result_var": False,
+    }
 
     pieces = cell.split(None, 1)
     if not pieces:
         return result
     result["connection"] = _connection_string(pieces[0], config)
     if result["connection"]:
         if len(pieces) == 1:
             return result
         cell = pieces[1]
 
     pieces = cell.split(None, 2)
     if len(pieces) > 1 and pieces[1] == "<<":
-        result["result_var"] = pieces[0]
+        if pieces[0].endswith("="):
+            result["result_var"] = pieces[0][:-1]
+            result["return_result_var"] = True
+        else:
+            result["result_var"] = pieces[0]
+
         if len(pieces) == 2:
             return result
         cell = pieces[2]
 
     result["sql"] = cell
     return result
```

### Comparing `jupysql-0.7.5/src/sql/plot.py` & `jupysql-0.7.6/src/sql/plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/run.py` & `jupysql-0.7.6/src/sql/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 
 def _nonbreaking_spaces(match_obj):
     """
     Make spaces visible in HTML by replacing all `` `` with ``&nbsp;``
 
     Call with a ``re`` match object.  Retain group 1, replace group 2
-    with nonbreaking speaces.
+    with nonbreaking spaces.
     """
     spaces = "&nbsp;" * len(match_obj.group(2))
     return "%s%s" % (match_obj.group(1), spaces)
 
 
 _cell_with_spaces_pattern = re.compile(r"(<td>)( {2,})")
 
@@ -251,15 +251,15 @@
 
         Parameters
         ----------
         key_word_sep: string used to separate column values
                       from each other in pie labels
         title: Plot title, defaults to name of value column
 
-        Any additional keyword arguments will be passsed
+        Any additional keyword arguments will be passed
         through to ``matplotlib.pylab.pie``.
         """
         self.guess_pie_columns(xlabel_sep=key_word_sep)
         import matplotlib.pylab as plt
 
         ax = plt.gca()
 
@@ -279,15 +279,15 @@
         The first and last columns are taken as the X and Y
         values.  Any columns between are ignored.
 
         Parameters
         ----------
         title: Plot title, defaults to names of Y value columns
 
-        Any additional keyword arguments will be passsed
+        Any additional keyword arguments will be passed
         through to ``matplotlib.pylab.plot``.
         """
         import matplotlib.pylab as plt
 
         self.guess_plot_columns()
         self.x = self.x or range(len(self.ys[0]))
 
@@ -320,15 +320,15 @@
 
         Parameters
         ----------
         title: Plot title, defaults to names of Y value columns
         key_word_sep: string used to separate column values
                       from each other in labels
 
-        Any additional keyword arguments will be passsed
+        Any additional keyword arguments will be passed
         through to ``matplotlib.pylab.bar``.
         """
         import matplotlib.pylab as plt
 
         ax = plt.gca()
 
         self.guess_pie_columns(xlabel_sep=key_word_sep)
```

### Comparing `jupysql-0.7.5/src/sql/store.py` & `jupysql-0.7.6/src/sql/store.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.5/src/sql/util.py` & `jupysql-0.7.6/src/sql/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import sql
 from sql import inspect
 import difflib
 from sql.connection import Connection
 from sql.store import store
 from sql import exceptions
+import json
 
 SINGLE_QUOTE = "'"
 DOUBLE_QUOTE = '"'
 
 
 def sanitize_identifier(identifier):
     if (identifier[0] == SINGLE_QUOTE and identifier[-1] == SINGLE_QUOTE) or (
@@ -246,7 +248,60 @@
 
 def support_only_sql_alchemy_connection(command):
     """
     Throws a sql.exceptions.RuntimeError if connection is not SQLAlchemy
     """
     if Connection.is_custom_connection():
         raise exceptions.RuntimeError(f"{command} is not supported for a custom engine")
+
+
+def fetch_sql_with_pagination(
+    table, offset, n_rows, sort_column=None, sort_order=None
+) -> tuple:
+    """
+    Returns next n_rows and columns from table starting at the offset
+
+    Parameters
+    ----------
+    table : str
+        Table name
+
+    offset : int
+        Specifies the number of rows to skip before
+        it starts to return rows from the query expression.
+
+    n_rows : int
+        Number of rows to return.
+
+    sort_column : str, default None
+        Sort by column
+
+    sort_order : 'DESC' or 'ASC', default None
+        Order list
+    """
+    is_table_exists(table)
+
+    order_by = "" if not sort_column else f"ORDER BY {sort_column} {sort_order}"
+
+    query = f"""
+    SELECT * FROM {table} {order_by}
+    OFFSET {offset} ROWS FETCH NEXT {n_rows} ROWS ONLY"""
+
+    rows = Connection.current.execute(query).fetchall()
+
+    columns = sql.run.raw_run(
+        Connection.current, f"SELECT * FROM {table} WHERE 1=0"
+    ).keys()
+
+    return rows, columns
+
+
+def parse_sql_results_to_json(rows, columns) -> str:
+    """
+    Serializes sql rows to a JSON formatted ``str``
+    """
+    dicts = [dict(zip(list(columns), row)) for row in rows]
+    rows_json = json.dumps(dicts, indent=4, sort_keys=True, default=str).replace(
+        "null", '"None"'
+    )
+
+    return rows_json
```


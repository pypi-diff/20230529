# Comparing `tmp/dbt-clickzetta-0.0.9.tar.gz` & `tmp/dbt-clickzetta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.0.9.tar", last modified: Sat May 27 20:14:51 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.1.0.tar", last modified: Mon May 29 06:35:04 2023, max compression
```

## Comparing `dbt-clickzetta-0.0.9.tar` & `dbt-clickzetta-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.746954 dbt-clickzetta-0.0.9/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.9/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 20:14:51.746831 dbt-clickzetta-0.0.9/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 06:42:15.000000 dbt-clickzetta-0.0.9/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.739414 dbt-clickzetta-0.0.9/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.9/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.738730 dbt-clickzetta-0.0.9/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.740613 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-26 10:45:40.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-26 13:43:40.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1179 2023-05-27 19:40:23.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7394 2023-05-27 18:40:18.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7075 2023-05-27 19:24:21.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1164 2023-05-27 19:52:27.000000 dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.738818 dbt-clickzetta-0.0.9/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.741205 dbt-clickzetta-0.0.9/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-25 08:45:33.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-26 12:03:31.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.741395 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 13:59:58.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.742262 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.743341 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.746041 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-26 13:10:00.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-26 12:08:15.000000 dbt-clickzetta-0.0.9/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:14:51.746683 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-27 20:14:51.000000 dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-27 20:14:51.746989 dbt-clickzetta-0.0.9/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-27 20:14:38.000000 dbt-clickzetta-0.0.9/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.522340 dbt-clickzetta-0.1.0/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 06:35:04.522223 dbt-clickzetta-0.1.0/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.517353 dbt-clickzetta-0.1.0/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.516652 dbt-clickzetta-0.1.0/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.518371 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7138 2023-05-29 03:50:21.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6709 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1184 2023-05-28 14:31:37.000000 dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.516744 dbt-clickzetta-0.1.0/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.518778 dbt-clickzetta-0.1.0/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.518978 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14278 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.519440 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.519916 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2651 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.521525 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.1.0/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:35:04.522074 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-05-29 06:35:04.000000 dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 06:35:04.522375 dbt-clickzetta-0.1.0/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-05-29 06:34:44.000000 dbt-clickzetta-0.1.0/setup.py
```

### Comparing `dbt-clickzetta-0.0.9/PKG-INFO` & `dbt-clickzetta-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.0.9
+Version: 0.1.0
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/column.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 @dataclass
 class ClickZettaColumn(dbtClassMixin, Column):  # type: ignore
     table_database: Optional[str] = None
     table_schema: Optional[str] = None
     table_name: Optional[str] = None
 
+    @classmethod
+    def translate_type(cls, dtype: str) -> str:
+        return dtype
+
     def is_integer(self) -> bool:
         return self.dtype.lower() in [
             "int8",
             "int16",
             "int32",
             "int64",
         ]
@@ -25,14 +29,22 @@
         return self.dtype.lower() in [
             "float32",
             "float64",
             # TODO(hanmiao.li): decimal is a subclass of float, but we don't want to treat it
             # "decimal",
         ]
 
+    @property
+    def quoted(self) -> str:
+        return "`{}`".format(self.column)
+
+    @property
+    def data_type(self) -> str:
+        return self.dtype
+
     def is_string(self) -> bool:
         return self.dtype.lower() in [
             "string",
             "varchar",
             "char",
         ]
```

### Comparing `dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -168,30 +168,19 @@
     def clear_transaction(self):
         pass
 
     @classmethod
     def _split_queries(cls, sql):
         pass
 
-    @classmethod
-    def process_results(cls, column_names, rows):
-        fixed = []
-        for row in rows:
-            fixed_row = []
-            for col in row:
-                fixed_row.append(col)
-
-            fixed.append(fixed_row)
-
-        return super().process_results(column_names, fixed)
-
     def execute(
             self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[AdapterResponse, agate.Table]:
         _, cursor = self.add_query(sql, auto_begin)
+        logger.info(f"dbt_execute_sql: {sql}")
         response = self.get_response(cursor)
         if fetch:
             table = self.get_result_from_cursor(cursor)
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
```

### Comparing `dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,29 +57,32 @@
         ConstraintType.unique: ConstraintSupport.NOT_ENFORCED,
         ConstraintType.primary_key: ConstraintSupport.NOT_ENFORCED,
         ConstraintType.foreign_key: ConstraintSupport.NOT_SUPPORTED,
     }
 
     @classmethod
     def date_function(cls):
-        return "CURRENT_TIMESTAMP()"
+        return "current_timestamp()"
 
     @classmethod
     def _catalog_filter_table(cls, table: agate.Table, manifest: Manifest) -> agate.Table:
         lowered = table.rename(column_names=[c.lower() for c in table.column_names])
         return super()._catalog_filter_table(lowered, manifest)
 
     @classmethod
     def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
-        return 'FLOAT' if decimals else 'INT'
+        return 'float64' if decimals else 'int64'
 
     @classmethod
     def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        return 'DATE'
+        return 'date'
+
+    def quote(self, identifier):
+        return "`{}`".format(identifier)
 
     def parse_describe_extended(
             self, relation: BaseRelation, raw_rows: AttrDict
     ) -> List[ClickZettaColumn]:
         # Convert the Row to a dict
         dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
 
@@ -111,31 +114,19 @@
             else:
                 raise e
 
         # strip hudi metadata columns.
         columns = [x for x in columns]
         return columns
 
-    def list_schemas(self, database: str) -> List[str]:
-        try:
-            results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
-        except DbtDatabaseError as exc:
-            msg = f"Database error while listing schemas in database " f'"{database}"\n{exc}'
-            raise DbtRuntimeError(msg)
-
-        return [row["schema_name"] for row in results]
+    def check_schema_exists(self, database, schema):
+        results = self.execute_macro(LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database})
 
-    def get_columns_in_relation(self, relation):
-        try:
-            return super().get_columns_in_relation(relation)
-        except DbtDatabaseError as exc:
-            if "does not exist or not authorized" in str(exc):
-                return []
-            else:
-                raise
+        exists = True if schema in [row[0] for row in results] else False
+        return exists
 
     def list_relations_without_caching(self, schema_relation: ClickZettaRelation) \
             -> List[ClickZettaRelation]:  # type: ignore
         kwargs = {"schema_relation": schema_relation}
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
         except DbtDatabaseError as exc:
```

### Comparing `dbt-clickzetta-0.0.9/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.1.0/dbt/adapters/clickzetta/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 class ClickZettaRelation(BaseRelation):
     quote_policy: ClickZettaQuotePolicy = field(default_factory=lambda: ClickZettaQuotePolicy())
     include_policy: ClickZettaIncludePolicy = field(default_factory=lambda: ClickZettaIncludePolicy())
     quote_character = "`"
 
     def __post_init__(self):
         if self.database != self.schema and self.database:
-            raise DbtRuntimeError("Cannot set database in spark!")
+            raise DbtRuntimeError("Cannot set database in clickzetta!")
 
     def render(self):
-        if self.include_policy.database and self.include_policy.schema:
-            raise DbtRuntimeError(
-                "Got a spark relation with schema and database set to "
-                "include, but only one can be set"
-            )
+        # if self.include_policy.database and self.include_policy.schema:
+        #     raise DbtRuntimeError(
+        #         "Got a clickzetta relation with schema and database set to "
+        #         "include, but only one can be set"
+        #     )
         return super().render()
```

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.1.0/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/PKG-INFO` & `dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickzetta
-Version: 0.0.9
+Version: 0.1.0
 Summary: The ClickZetta adapter plugin for dbt
 Home-page: 
 Author: clickzetta
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `dbt-clickzetta-0.0.9/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.1.0/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.0.9/setup.py` & `dbt-clickzetta-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.0.9"
+package_version = "0.1.0"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -64,15 +64,15 @@
     author="clickzetta",
     author_email="",
     url="",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "clickzetta-connector~=0.7.5",
+        "clickzetta-connector~=0.7.7",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```


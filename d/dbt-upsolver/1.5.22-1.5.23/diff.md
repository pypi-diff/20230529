# Comparing `tmp/dbt-upsolver-1.5.22.tar.gz` & `tmp/dbt-upsolver-1.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-1.5.22.tar", last modified: Tue May 23 13:07:01 2023, max compression
+gzip compressed data, was "dbt-upsolver-1.5.23.tar", last modified: Mon May 29 13:34:32 2023, max compression
```

## Comparing `dbt-upsolver-1.5.22.tar` & `dbt-upsolver-1.5.23.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.366083 dbt-upsolver-1.5.22/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.366083 dbt-upsolver-1.5.22/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/target_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.013711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-29 13:34:31.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:34:31.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 13:34:32.000000 dbt-upsolver-1.5.23/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:34:32.017711 dbt-upsolver-1.5.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-29 13:34:22.000000 dbt-upsolver-1.5.23/setup.py
```

### Comparing `dbt-upsolver-1.5.22/LICENSE` & `dbt-upsolver-1.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/PKG-INFO` & `dbt-upsolver-1.5.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.22
+Version: 1.5.23
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-1.5.22/README.md` & `dbt-upsolver-1.5.23/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,37 +69,37 @@
     @available
     def separate_options(self, config_options, source):
         job_options = self.enrich_options(config_options, source, 'job_options')
         source_options = self.enrich_options(config_options, source, 'source_options')
         return job_options, source_options
 
     def render_option_from_dict(self, option_value):
-        res = []
         try:
+            res = []
             for key, value in option_value.items():
                 item = [f'{key}=']
                 if isinstance(value, list):
                     item.append('(')
                     item.append(' ,'.join(value))
                     item.append(')')
                 else:
                     item.append(value)
                 res.append(''.join(item))
             return f"({' ,'.join(res)})"
         except Exception:
-            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}")
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}. Expected type: dictionary")
 
     def render_option_from_list(self, option_value):
         try:
-            if not isinstance(option_value, str):
+            if isinstance(option_value, list) and len(option_value) > 1:
                 return tuple(i for i in option_value)
             else:
-                return f"('{option_value}')"
+                return f"('{''.join(option_value)}')"
         except Exception:
-            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}")
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}. Expected type: list of strings")
 
     @available
     def enrich_options(self, config_options, source, options_type):
         options = self.get_options(source, options_type)
         enriched_options = {}
         for option, value in config_options.items():
             find_value = options.get(option.lower(), None)
```

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/target_options.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/target_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-1.5.23/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 {% macro get_create_copy_job_sql(job_identifier, sql, into_relation, sync, options, source, target_type) -%}
 
-    {% set connection_identifier = adapter.get_connection_from_sql(sql) %}
-    {% set job_options, source_options = adapter.separate_options(options, source) %}
+    {%- set connection_identifier = adapter.get_connection_from_sql(sql) -%}
+    {%- set job_options, source_options = adapter.separate_options(options, source) -%}
     {%- if target_type != 'datalake' -%}
-      {% set target_options = adapter.enrich_options(options, target_type, 'target_options') %}
-      {% set target_type = target_type %}
+      {%- set target_options = adapter.enrich_options(options, target_type, 'target_options') -%}
+      {%- set target_type = target_type -%}
     {%- else -%}
-      {% set target_options = {} %}
-      {% set target_type = '' %}
+      {%- set target_options = {} -%}
+      {%- set target_type = '' -%}
     {%- endif -%}
 
-    CREATE
-    {% if sync %}
-      SYNC
-    {% endif %}
+    CREATE {{''}}
+    {%- if sync -%}
+      SYNC {{''}}
+    {%- endif -%}
     JOB {{job_identifier}}
     {{ render_options(job_options, 'create') }}
     {{ render_options(target_options, 'create') }}
     AS COPY FROM {{source}} {{connection_identifier}}
     {{ render_options(source_options, 'create') }}
     INTO {{target_type}} {{into_relation}}
```

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 {% macro get_create_merge_job_sql(job_identifier, into_relation, sync, options, primary_key, delete_condition, target_type) -%}
 
   {% set enriched_options = adapter.enrich_options(options, target_type, 'transformation_options') %}
 
   {%- if target_type == 'datalake' -%}
-    {% set target_type = '' %}
+    {%- set target_type = '' -%}
   {%- endif -%}
 
-  CREATE
-  {% if sync %}
-    SYNC
-  {% endif %}
+  CREATE {{''}}
+  {%- if sync -%}
+    SYNC {{''}}
+  {%- endif -%}
   JOB {{ job_identifier }}
     {{ render_options(enriched_options, 'create') }}
   AS MERGE INTO {{ target_type }} {{ into_relation }} AS target
-  USING (
-  {{ sql }}
-  )
-  {% if primary_key %}
+  USING ( {{- sql }} )
+  {% if primary_key -%}
     source ON (
-      {% for item in primary_key %}
+      {%- for item in primary_key %}
         target.{{ item['field'] }} = source.{{ item['field'] }}
-      {% endfor %}
+      {%- endfor -%}
     )
-  {% endif %}
+  {%- endif -%}
   {% if delete_condition %}
-    WHEN MATCHED AND {{ delete_condition}} THEN DELETE
-  {% endif %}
+  WHEN MATCHED AND {{ delete_condition}} THEN DELETE
+  {%- endif %}
   WHEN MATCHED THEN REPLACE
   WHEN NOT MATCHED THEN INSERT MAP_COLUMNS_BY_NAME
 {%- endmacro %}
```

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 {% materialization incremental, adapter='upsolver' %}
 
   {%- set identifier = model['alias'] -%}
   {%- set model_config = model['config'] -%}
-  {% set incremental_strategy = adapter.get(model_config, 'incremental_strategy', False) %}
-  {% set sync = adapter.get(model_config, 'sync', False) %}
-  {% set options = adapter.get(model_config, 'options', {}) %}
-  {% set source = adapter.get(model_config, 'source') %}
-  {% set target_type = adapter.get(model_config, 'target_type', 'datalake').lower() %}
-  {% set target_schema = adapter.get(model_config, 'target_schema', schema) %}
-  {% set delete_condition = adapter.get(model_config, 'delete_condition', False) %}
-  {% set partition_by = adapter.get(model_config, 'partition_by', []) %}
-  {% set primary_key = adapter.get(model_config, 'primary_key', []) %}
-  {% set map_columns_by_name = adapter.get(model_config, 'map_columns_by_name', False) %}
-  {% set job_identifier = identifier + '_job' %}
+  {%- set incremental_strategy = adapter.get(model_config, 'incremental_strategy', False) -%}
+  {%- set sync = adapter.get(model_config, 'sync', False) -%}
+  {%- set options = adapter.get(model_config, 'options', {}) -%}
+  {%- set source = adapter.get(model_config, 'source') -%}
+  {%- set target_type = adapter.get(model_config, 'target_type', 'datalake').lower() -%}
+  {%- set target_schema = adapter.get(model_config, 'target_schema', schema) -%}
+  {%- set target_table_alias = adapter.get(model_config, 'target_table_alias', identifier) -%}
+  {%- set delete_condition = adapter.get(model_config, 'delete_condition', False) -%}
+  {%- set partition_by = adapter.get(model_config, 'partition_by', []) -%}
+  {%- set primary_key = adapter.get(model_config, 'primary_key', []) -%}
+  {%- set map_columns_by_name = adapter.get(model_config, 'map_columns_by_name', False) -%}
+  {%- set job_identifier = identifier + '_job' %}
 
   {%- set old_relation = adapter.get_relation(identifier=job_identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=job_identifier,
                                                 schema=schema,
                                                 database=database,
@@ -25,56 +26,56 @@
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
   {{ log("model[config]: " ~ model['config'] ) }}
 
 
   {% if target_type  == 'datalake' %}
-    {%- set table_relation = api.Relation.create(identifier=identifier,
+    {%- set table_relation = api.Relation.create(identifier=target_table_alias,
                                                  schema=schema,
                                                  database=database,
                                                  type='table') -%}
     {%- set into_relation = table_relation -%}
     {%- call statement('create_table_if_not_exists') -%}
       {{ get_create_table_if_not_exists_sql(table_relation, partition_by, primary_key, options) }}
     {%- endcall -%}
   {%- else -%}
     {% set target_connection = adapter.require(model_config, 'target_connection') %}
-    {%- set into_relation = target_connection + '.' + target_schema + '.' + identifier -%}
+    {%- set into_relation = target_connection + '.' + target_schema + '.' + target_table_alias -%}
   {%- endif %}
 
-  {% if old_relation %}
-    {% call statement('main') -%}
+  {%- if old_relation -%}
+    {%- call statement('main') -%}
       {{ get_alter_job_sql(job_identifier, options, incremental_strategy, source) }}
     {%- endcall %}
-  {% else %}
-    {% call statement('main') -%}
-      {% if incremental_strategy == 'merge' %}
+  {%- else -%}
+    {%- call statement('main') -%}
+      {%- if incremental_strategy == 'merge' -%}
         {{ get_create_merge_job_sql(job_identifier, into_relation, sync,
                                     options, primary_key, delete_condition,
                                     target_type) }}
-      {% elif incremental_strategy == 'insert' %}
+      {%- elif incremental_strategy == 'insert' -%}
         {{ get_create_insert_job_sql(job_identifier,
                                     into_relation, sync, options,
                                     map_columns_by_name, target_type) }}
 
-      {% else  %}
+      {%- else  -%}
         {{ get_create_copy_job_sql(job_identifier, sql,
                                    into_relation, sync, options, source,
                                    target_type) }}
 
-      {% endif %}
-    {%- endcall %}
-  {%- endif %}
+      {%- endif -%}
+    {%- endcall -%}
+  {%- endif -%}
 
-  {% do persist_docs(target_relation, model) %}
-  {% do persist_docs(table_relation, model) %}
+  {%- do persist_docs(target_relation, model) -%}
+  {%- do persist_docs(table_relation, model) -%}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
-  {% if target_type  == 'datalake' %}
+  {%- if target_type  == 'datalake' -%}
     {{ return({'relations': [target_relation, table_relation]}) }}
-  {% else  %}
+  {%- else  -%}
     {{ return({'relations': [target_relation]}) }}
-  {%- endif %}
-{% endmaterialization %}
+  {%- endif -%}
+{%- endmaterialization -%}
```

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-1.5.23/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% macro get_alter_job_sql(job_identifier, options, incremental_strategy, source) -%}
 
-  {% if incremental_strategy %}
-    {% set enriched_options = adapter.enrich_options(options, 'datalake', 'transformation_options') %}
-  {% else  %}
-    {% set enriched_options, _ = adapter.separate_options(options, source) %}
-  {% endif %}
-  {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
+  {%- if incremental_strategy -%}
+    {%- set enriched_options = adapter.enrich_options(options, 'datalake', 'transformation_options') -%}
+  {%- else  -%}
+    {%- set enriched_options, _ = adapter.separate_options(options, source) -%}
+  {%- endif -%}
+  {%- set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') -%}
 
   ALTER JOB {{job_identifier}}
     {{ render_options(enriched_editable_options, 'alter') }}
 
 {%- endmacro %}
```

### Comparing `dbt-upsolver-1.5.22/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-1.5.23/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.22
+Version: 1.5.23
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-1.5.22/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-1.5.23/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.22/setup.py` & `dbt-upsolver-1.5.23/setup.py`

 * *Files identical despite different names*


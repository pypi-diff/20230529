# Comparing `tmp/gn2pg_client-1.5.0.tar.gz` & `tmp/gn2pg_client-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gn2pg_client-1.5.0.tar", max compression
+gzip compressed data, was "gn2pg_client-1.5.1.tar", max compression
```

## Comparing `gn2pg_client-1.5.0.tar` & `gn2pg_client-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2023-05-03 12:49:34.878197 gn2pg_client-1.5.0/LICENSE
--rw-r--r--   0        0        0     7798 2023-05-03 12:49:34.878197 gn2pg_client-1.5.0/README.rst
--rw-r--r--   0        0        0     1059 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/__init__.py
--rw-r--r--   0        0        0     7124 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/api.py
--rw-r--r--   0        0        0        0 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/__init__.py
--rw-r--r--   0        0        0     1041 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/admin_views.py
--rw-r--r--   0        0        0     1391 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/app.py
--rw-r--r--   0        0        0     1942 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/config.py
--rw-r--r--   0        0        0      456 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/database.py
--rw-r--r--   0        0        0      240 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/env.py
--rw-r--r--   0        0        0      202 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/index.py
--rw-r--r--   0        0        0     1953 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/models.py
--rw-r--r--   0        0        0      216 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/static/css/custom_flaks_admin.css
--rw-r--r--   0        0        0    30240 2023-05-03 12:49:34.882197 gn2pg_client-1.5.0/gn2pg/app/static/img/src_gn2pg.png
--rw-r--r--   0        0        0      185 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/templates/admin/master.html
--rw-r--r--   0        0        0      353 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/templates/index.html
--rw-r--r--   0        0        0        0 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/utils/__init__.py
--rw-r--r--   0        0        0      582 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/app/utils/admin_views.py
--rw-r--r--   0        0        0    11145 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/check_conf.py
--rw-r--r--   0        0        0     1835 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/data/gn2pgconfig.toml
--rw-r--r--   0        0        0    78873 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/data/to_gnsynthese.sql
--rw-r--r--   0        0        0     8944 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/download.py
--rw-r--r--   0        0        0      241 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/env.py
--rw-r--r--   0        0        0     3968 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/helpers.py
--rw-r--r--   0        0        0     4100 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
--rw-r--r--   0        0        0    10575 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
--rw-r--r--   0        0        0    10307 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
--rwxr-xr-x   0        0        0     6063 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/main.py
--rw-r--r--   0        0        0      765 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/metadata.py
--rw-r--r--   0        0        0    20834 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/store_postgresql.py
--rw-r--r--   0        0        0     1387 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/gn2pg/utils.py
--rw-r--r--   0        0        0     3169 2023-05-03 12:49:34.886197 gn2pg_client-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     9874 1970-01-01 00:00:00.000000 gn2pg_client-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-29 15:15:48.180848 gn2pg_client-1.5.1/LICENSE
+-rw-r--r--   0        0        0     7798 2023-05-29 15:15:48.180848 gn2pg_client-1.5.1/README.rst
+-rw-r--r--   0        0        0     1059 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/__init__.py
+-rw-r--r--   0        0        0     7124 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/api.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/admin_views.py
+-rw-r--r--   0        0        0     1391 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/app.py
+-rw-r--r--   0        0        0     1942 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/config.py
+-rw-r--r--   0        0        0      456 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/database.py
+-rw-r--r--   0        0        0      240 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/env.py
+-rw-r--r--   0        0        0      202 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/index.py
+-rw-r--r--   0        0        0     1953 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/models.py
+-rw-r--r--   0        0        0      216 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/static/css/custom_flaks_admin.css
+-rw-r--r--   0        0        0    30240 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/static/img/src_gn2pg.png
+-rw-r--r--   0        0        0      185 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/templates/admin/master.html
+-rw-r--r--   0        0        0      353 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/templates/index.html
+-rw-r--r--   0        0        0        0 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/utils/__init__.py
+-rw-r--r--   0        0        0      582 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/app/utils/admin_views.py
+-rw-r--r--   0        0        0    11145 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/check_conf.py
+-rw-r--r--   0        0        0     1835 2023-05-29 15:15:48.184848 gn2pg_client-1.5.1/gn2pg/data/gn2pgconfig.toml
+-rw-r--r--   0        0        0    42462 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/data/to_gnsynthese.sql
+-rw-r--r--   0        0        0     8944 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/download.py
+-rw-r--r--   0        0        0      241 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/env.py
+-rw-r--r--   0        0        0     3968 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/helpers.py
+-rw-r--r--   0        0        0     4100 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po
+-rw-r--r--   0        0        0    10575 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po
+-rw-r--r--   0        0        0    10307 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~
+-rwxr-xr-x   0        0        0     6063 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/main.py
+-rw-r--r--   0        0        0      765 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/metadata.py
+-rw-r--r--   0        0        0    20834 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/store_postgresql.py
+-rw-r--r--   0        0        0     1387 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/gn2pg/utils.py
+-rw-r--r--   0        0        0     3169 2023-05-29 15:15:48.188848 gn2pg_client-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9874 1970-01-01 00:00:00.000000 gn2pg_client-1.5.1/PKG-INFO
```

### Comparing `gn2pg_client-1.5.0/LICENSE` & `gn2pg_client-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/README.rst` & `gn2pg_client-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/__init__.py` & `gn2pg_client-1.5.1/gn2pg/__init__.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/api.py` & `gn2pg_client-1.5.1/gn2pg/api.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/admin_views.py` & `gn2pg_client-1.5.1/gn2pg/app/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/app.py` & `gn2pg_client-1.5.1/gn2pg/app/app.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/config.py` & `gn2pg_client-1.5.1/gn2pg/app/config.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/models.py` & `gn2pg_client-1.5.1/gn2pg/app/models.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/static/img/src_gn2pg.png` & `gn2pg_client-1.5.1/gn2pg/app/static/img/src_gn2pg.png`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/app/utils/admin_views.py` & `gn2pg_client-1.5.1/gn2pg/app/utils/admin_views.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/check_conf.py` & `gn2pg_client-1.5.1/gn2pg/check_conf.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/data/gn2pgconfig.toml` & `gn2pg_client-1.5.1/gn2pg/data/gn2pgconfig.toml`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/download.py` & `gn2pg_client-1.5.1/gn2pg/download.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/helpers.py` & `gn2pg_client-1.5.1/gn2pg/helpers.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po` & `gn2pg_client-1.5.1/gn2pg/locale/en_US/LC_MESAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po` & `gn2pg_client-1.5.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~` & `gn2pg_client-1.5.1/gn2pg/locale/fr_FR/LC_MESSAGES/gn2pg.po~`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/main.py` & `gn2pg_client-1.5.1/gn2pg/main.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/metadata.py` & `gn2pg_client-1.5.1/gn2pg/metadata.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/store_postgresql.py` & `gn2pg_client-1.5.1/gn2pg/store_postgresql.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/gn2pg/utils.py` & `gn2pg_client-1.5.1/gn2pg/utils.py`

 * *Files identical despite different names*

### Comparing `gn2pg_client-1.5.0/pyproject.toml` & `gn2pg_client-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gn2pg_client"
 packages = [{ include = "gn2pg" }]
-version = "1.5.0"
+version = "1.5.1"
 description = "Import tool from GeoNature to a PostgreSQL database through Export module API (client side)"
 authors = ["lpofredc <frederic.cloitre@lpo.fr>"]
 maintainers = ["lpofredc <frederic.cloitre@lpo.fr>"]
 license = "AGPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/lpoaura/gn2gn_client/"
 keywords = ["GeoNature", "Export", "SINP", "opendata", "biodiversity"]
```

### Comparing `gn2pg_client-1.5.0/PKG-INFO` & `gn2pg_client-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gn2pg-client
-Version: 1.5.0
+Version: 1.5.1
 Summary: Import tool from GeoNature to a PostgreSQL database through Export module API (client side)
 Home-page: https://github.com/lpoaura/gn2gn_client/
 License: AGPL-3.0-or-later
 Keywords: GeoNature,Export,SINP,opendata,biodiversity
 Author: lpofredc
 Author-email: frederic.cloitre@lpo.fr
 Maintainer: lpofredc
```


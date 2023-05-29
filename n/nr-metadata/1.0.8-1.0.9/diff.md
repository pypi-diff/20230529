# Comparing `tmp/nr-metadata-1.0.8.tar.gz` & `tmp/nr-metadata-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nr-metadata-1.0.8.tar", last modified: Tue Mar 14 19:26:56 2023, max compression
+gzip compressed data, was "nr-metadata-1.0.9.tar", last modified: Tue Mar 14 20:06:28 2023, max compression
```

## Comparing `nr-metadata-1.0.8.tar` & `nr-metadata-1.0.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.364326 nr-metadata-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-14 19:26:56.364326 nr-metadata-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.340326 nr-metadata-1.0.8/nr_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/nr_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.344326 nr-metadata-1.0.8/nr_metadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:11.000000 nr-metadata-1.0.8/nr_metadata/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-14 19:26:12.000000 nr-metadata-1.0.8/nr_metadata/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-14 19:26:12.000000 nr-metadata-1.0.8/nr_metadata/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-14 19:26:12.000000 nr-metadata-1.0.8/nr_metadata/common/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.344326 nr-metadata-1.0.8/nr_metadata/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:12.000000 nr-metadata-1.0.8/nr_metadata/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   314317 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)   140677 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:13.000000 nr-metadata-1.0.8/nr_metadata/common/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39345 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/jsonschemas/common-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41922 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-14 19:26:14.000000 nr-metadata-1.0.8/nr_metadata/common/records/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-14 19:26:15.000000 nr-metadata-1.0.8/nr_metadata/common/records/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:15.000000 nr-metadata-1.0.8/nr_metadata/common/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:15.000000 nr-metadata-1.0.8/nr_metadata/common/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-14 19:26:15.000000 nr-metadata-1.0.8/nr_metadata/common/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-14 19:26:15.000000 nr-metadata-1.0.8/nr_metadata/common/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-14 19:26:16.000000 nr-metadata-1.0.8/nr_metadata/common/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.348326 nr-metadata-1.0.8/nr_metadata/common/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:16.000000 nr-metadata-1.0.8/nr_metadata/common/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.352326 nr-metadata-1.0.8/nr_metadata/common/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:16.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-14 19:26:16.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-03-14 19:26:17.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-14 19:26:17.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/i18nStr_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-14 19:26:17.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-14 19:26:17.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-03-14 19:26:42.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-03-14 19:26:18.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-14 19:26:18.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-03-14 19:26:42.000000 nr-metadata-1.0.8/nr_metadata/common/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 19:26:19.000000 nr-metadata-1.0.8/nr_metadata/common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-14 19:26:19.000000 nr-metadata-1.0.8/nr_metadata/common/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.352326 nr-metadata-1.0.8/nr_metadata/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:42.000000 nr-metadata-1.0.8/nr_metadata/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-14 19:26:43.000000 nr-metadata-1.0.8/nr_metadata/documents/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-14 19:26:43.000000 nr-metadata-1.0.8/nr_metadata/documents/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-14 19:26:43.000000 nr-metadata-1.0.8/nr_metadata/documents/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.352326 nr-metadata-1.0.8/nr_metadata/documents/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:43.000000 nr-metadata-1.0.8/nr_metadata/documents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   340447 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)   152319 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:44.000000 nr-metadata-1.0.8/nr_metadata/documents/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42540 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-14 19:26:45.000000 nr-metadata-1.0.8/nr_metadata/documents/records/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-14 19:26:46.000000 nr-metadata-1.0.8/nr_metadata/documents/records/multilingual_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.356326 nr-metadata-1.0.8/nr_metadata/documents/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:46.000000 nr-metadata-1.0.8/nr_metadata/documents/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.360326 nr-metadata-1.0.8/nr_metadata/documents/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:46.000000 nr-metadata-1.0.8/nr_metadata/documents/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-14 19:26:46.000000 nr-metadata-1.0.8/nr_metadata/documents/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-14 19:26:47.000000 nr-metadata-1.0.8/nr_metadata/documents/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-14 19:26:47.000000 nr-metadata-1.0.8/nr_metadata/documents/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.360326 nr-metadata-1.0.8/nr_metadata/documents/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:47.000000 nr-metadata-1.0.8/nr_metadata/documents/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.360326 nr-metadata-1.0.8/nr_metadata/documents/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:47.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-14 19:26:47.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-03-14 19:26:48.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-14 19:26:48.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/i18nStr_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-14 19:26:48.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-14 19:26:49.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-14 19:26:49.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-03-14 19:26:49.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 19:26:50.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-03-14 19:26:50.000000 nr-metadata-1.0.8/nr_metadata/documents/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 19:26:50.000000 nr-metadata-1.0.8/nr_metadata/documents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-14 19:26:50.000000 nr-metadata-1.0.8/nr_metadata/documents/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.360326 nr-metadata-1.0.8/nr_metadata/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/nr_metadata/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/nr_metadata/schema/identifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.364326 nr-metadata-1.0.8/nr_metadata/ui_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/nr_metadata/ui_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/nr_metadata/ui_schema/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 19:26:56.344326 nr-metadata-1.0.8/nr_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 19:26:56.000000 nr-metadata-1.0.8/nr_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-14 19:25:29.000000 nr-metadata-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-14 19:26:56.364326 nr-metadata-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 19:26:50.000000 nr-metadata-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.693524 nr-metadata-1.0.9/nr_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/nr_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.697523 nr-metadata-1.0.9/nr_metadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:46.000000 nr-metadata-1.0.9/nr_metadata/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314313 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)   140693 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:47.000000 nr-metadata-1.0.9/nr_metadata/common/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39345 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/jsonschemas/common-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:48.000000 nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41922 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/records/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.701524 nr-metadata-1.0.9/nr_metadata/common/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.705524 nr-metadata-1.0.9/nr_metadata/common/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:49.000000 nr-metadata-1.0.9/nr_metadata/common/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-14 20:05:50.000000 nr-metadata-1.0.9/nr_metadata/common/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-14 20:05:50.000000 nr-metadata-1.0.9/nr_metadata/common/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-14 20:05:50.000000 nr-metadata-1.0.9/nr_metadata/common/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.705524 nr-metadata-1.0.9/nr_metadata/common/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:50.000000 nr-metadata-1.0.9/nr_metadata/common/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.705524 nr-metadata-1.0.9/nr_metadata/common/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:50.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-14 20:05:51.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-03-14 20:05:51.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-14 20:05:51.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/i18nStr_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-14 20:05:52.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-14 20:05:52.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-03-14 20:06:16.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-03-14 20:05:53.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-14 20:05:53.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-03-14 20:06:16.000000 nr-metadata-1.0.9/nr_metadata/common/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 20:05:53.000000 nr-metadata-1.0.9/nr_metadata/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-14 20:05:54.000000 nr-metadata-1.0.9/nr_metadata/common/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.709524 nr-metadata-1.0.9/nr_metadata/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:16.000000 nr-metadata-1.0.9/nr_metadata/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.709524 nr-metadata-1.0.9/nr_metadata/documents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   340443 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)   152335 2023-03-14 20:06:17.000000 nr-metadata-1.0.9/nr_metadata/documents/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-14 20:06:18.000000 nr-metadata-1.0.9/nr_metadata/documents/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.709524 nr-metadata-1.0.9/nr_metadata/documents/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:18.000000 nr-metadata-1.0.9/nr_metadata/documents/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-03-14 20:06:18.000000 nr-metadata-1.0.9/nr_metadata/documents/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-14 20:06:18.000000 nr-metadata-1.0.9/nr_metadata/documents/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.709524 nr-metadata-1.0.9/nr_metadata/documents/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:18.000000 nr-metadata-1.0.9/nr_metadata/documents/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42540 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.709524 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.713523 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.713523 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-14 20:06:19.000000 nr-metadata-1.0.9/nr_metadata/documents/records/multilingual_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.713523 nr-metadata-1.0.9/nr_metadata/documents/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.713523 nr-metadata-1.0.9/nr_metadata/documents/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.713523 nr-metadata-1.0.9/nr_metadata/documents/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:20.000000 nr-metadata-1.0.9/nr_metadata/documents/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/nr_metadata/documents/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:21.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-14 20:06:21.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-03-14 20:06:21.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-14 20:06:22.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/i18nStr_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-14 20:06:22.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-14 20:06:22.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-03-14 20:06:22.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-03-14 20:06:23.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-14 20:06:23.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-03-14 20:06:23.000000 nr-metadata-1.0.9/nr_metadata/documents/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-14 20:06:23.000000 nr-metadata-1.0.9/nr_metadata/documents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-14 20:06:24.000000 nr-metadata-1.0.9/nr_metadata/documents/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/nr_metadata/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/nr_metadata/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/nr_metadata/schema/identifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/nr_metadata/ui_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/nr_metadata/ui_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/nr_metadata/ui_schema/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 20:06:28.697523 nr-metadata-1.0.9/nr_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-14 20:06:28.000000 nr-metadata-1.0.9/nr_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-14 20:05:07.000000 nr-metadata-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-14 20:06:28.717524 nr-metadata-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 20:06:24.000000 nr-metadata-1.0.9/setup.py
```

### Comparing `nr-metadata-1.0.8/PKG-INFO` & `nr-metadata-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-metadata
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Generated metadata files for the Czech National Repository"
 Home-page: https://github.com/Narodni-repozitar/ne-metadata
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR
 Platform: any
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/cli.py` & `nr-metadata-1.0.9/nr_metadata/common/cli.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/ext.py` & `nr-metadata-1.0.9/nr_metadata/common/ext.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/models/model.json` & `nr-metadata-1.0.9/nr_metadata/common/models/model.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999982633454%*

 * *Differences: {"'model'": "{'properties': {'metadata': {'properties': {'creators': {'items': {'properties': "*

 * *            "{'affiliations': {'items': {'relation-args': {'pid_field': "*

 * *            '\'Vocabulary.pid.with_type_ctx("institutions")\'}, \'pid-field\': '*

 * *            '\'Vocabulary.pid.with_type_ctx("institutions")\'}}}}}, \'contributors\': {\'items\': '*

 * *            "{'marshmallow': {'schema-class': "*

 * *            "'nr_metadata.common.services.records.schema.NRContributorSchema', 'imports': {0: "*

 * *            "{'im […]*

```diff
@@ -651,18 +651,18 @@
                     },
                     "contributors": {
                         "items": {
                             "marshmallow": {
                                 "field-class": "ma_fields.Nested",
                                 "imports": [
                                     {
-                                        "import": "nr_metadata.common.services.records.schema.NRAuthoritySchema"
+                                        "import": "nr_metadata.common.services.records.schema.NRContributorSchema"
                                     }
                                 ],
-                                "schema-class": "nr_metadata.common.services.records.schema.NRAuthoritySchema",
+                                "schema-class": "nr_metadata.common.services.records.schema.NRContributorSchema",
                                 "validators": []
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
                                         "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
                                         "imports": [
@@ -703,15 +703,15 @@
                                             ],
                                             "schema-class": "nr_metadata.common.services.records.schema.NRAffiliationVocabularySchema",
                                             "validators": []
                                         },
                                         "model": "vocabularies",
                                         "model-class": "Vocabulary",
                                         "name": "affiliations_item",
-                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor_affiliations\")",
+                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
                                             "@v": {
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.String",
                                                     "field-name": "_version",
                                                     "imports": [],
                                                     "validators": []
@@ -789,15 +789,15 @@
                                                         "validators": []
                                                     }
                                                 }
                                             }
                                         },
                                         "relation-args": {
                                             "keys": "['id', 'title']",
-                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"contributor_affiliations\")"
+                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"institutions\")"
                                         },
                                         "relation-class": "PIDRelation",
                                         "sample": {
                                             "faker": "company",
                                             "skip": false
                                         },
                                         "schema-prefix": "AffiliationsItem",
@@ -1020,18 +1020,18 @@
                                     ],
                                     "label.cs": "Role p\u0159isp\u011bvatele",
                                     "label.en": "Contributor's role",
                                     "marshmallow": {
                                         "field-class": "ma_fields.Nested",
                                         "imports": [
                                             {
-                                                "import": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema"
+                                                "import": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema"
                                             }
                                         ],
-                                        "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema",
+                                        "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema",
                                         "validators": []
                                     },
                                     "model": "vocabularies",
                                     "model-class": "Vocabulary",
                                     "name": "role",
                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
                                     "properties": {
@@ -1126,33 +1126,33 @@
                                     "type": "relation",
                                     "ui": {
                                         "detail": "authority",
                                         "marshmallow": {
                                             "field-class": "ma_fields.Nested",
                                             "imports": [
                                                 {
-                                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                 }
                                             ],
-                                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                         }
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "contributor",
                                 "marshmallow": {
                                     "field-class": "ma_fields.Nested",
                                     "imports": [
                                         {
-                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                            "import": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                         }
                                     ],
-                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                 }
                             }
                         },
                         "marshmallow": {
                             "field-class": "ma_fields.List",
                             "imports": [],
                             "validators": []
@@ -1219,15 +1219,15 @@
                                             ],
                                             "schema-class": "nr_metadata.common.services.records.schema.NRAffiliationVocabularySchema",
                                             "validators": []
                                         },
                                         "model": "vocabularies",
                                         "model-class": "Vocabulary",
                                         "name": "affiliations_item",
-                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"creator_affiliations\")",
+                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
                                             "@v": {
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.String",
                                                     "field-name": "_version",
                                                     "imports": [],
                                                     "validators": []
@@ -1305,15 +1305,15 @@
                                                         "validators": []
                                                     }
                                                 }
                                             }
                                         },
                                         "relation-args": {
                                             "keys": "['id', 'title']",
-                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"creator_affiliations\")"
+                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"institutions\")"
                                         },
                                         "relation-class": "PIDRelation",
                                         "sample": {
                                             "faker": "company",
                                             "skip": false
                                         },
                                         "schema-prefix": "AffiliationsItem",
@@ -3194,18 +3194,18 @@
                                                 ],
                                                 "label.cs": "Role p\u0159isp\u011bvatele",
                                                 "label.en": "Contributor's role",
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.Nested",
                                                     "imports": [
                                                         {
-                                                            "import": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema"
+                                                            "import": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema"
                                                         }
                                                     ],
-                                                    "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema",
+                                                    "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema",
                                                     "validators": []
                                                 },
                                                 "model": "vocabularies",
                                                 "model-class": "Vocabulary",
                                                 "name": "role",
                                                 "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
                                                 "properties": {
@@ -3300,18 +3300,18 @@
                                                 "type": "relation",
                                                 "ui": {
                                                     "detail": "authority",
                                                     "marshmallow": {
                                                         "field-class": "ma_fields.Nested",
                                                         "imports": [
                                                             {
-                                                                "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                                "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                             }
                                                         ],
-                                                        "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                        "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                     }
                                                 }
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
                                             "detail": "contributor",
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/models/ui.json` & `nr-metadata-1.0.9/nr_metadata/common/models/ui.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999998566267723%*

 * *Differences: {"'children'": "{'metadata': {'children': {'contributors': {'child': {'marshmallow': "*

 * *               "{'schema-class': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRContributorUISchema', 'imports': "*

 * *               "{0: {'import': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRContributorUISchema'}}}, "*

 * *               "'children': {'role': {'marshmallow': {'schema-class': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISch […]*

```diff
@@ -445,31 +445,31 @@
                                 "hint": "metadata/contributors/role.hint",
                                 "input": "relation",
                                 "label": "metadata/contributors/role.label",
                                 "marshmallow": {
                                     "field-class": "ma_fields.Nested",
                                     "imports": [
                                         {
-                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                         }
                                     ],
-                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                 }
                             }
                         },
                         "detail": "contributor",
                         "input": "contributor",
                         "marshmallow": {
                             "field-class": "ma_fields.Nested",
                             "imports": [
                                 {
-                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                    "import": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                 }
                             ],
-                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                         }
                     },
                     "detail": "array",
                     "help": "metadata/contributors.help",
                     "hint": "metadata/contributors.hint",
                     "input": "array",
                     "label": "metadata/contributors.label",
@@ -1432,18 +1432,18 @@
                                             "hint": "metadata/relatedItems/itemContributors/role.hint",
                                             "input": "relation",
                                             "label": "metadata/relatedItems/itemContributors/role.label",
                                             "marshmallow": {
                                                 "field-class": "ma_fields.Nested",
                                                 "imports": [
                                                     {
-                                                        "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                        "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                     }
                                                 ],
-                                                "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                             }
                                         }
                                     },
                                     "detail": "contributor",
                                     "input": "itemcontributor",
                                     "marshmallow": {
                                         "field-class": "ma_fields.Nested",
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/records/api.py` & `nr-metadata-1.0.9/nr_metadata/common/records/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     dumper_extensions = [MultilingualDumper()]
     dumper = CommonDumper(extensions=dumper_extensions)
 
     relations = RelationsField(
         affiliations_item=PIDRelation(
             "metadata.creators.affiliations",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("creator_affiliations"),
+            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         role=PIDRelation(
             "metadata.contributors.role",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
         ),
         affiliations_item_1=PIDRelation(
             "metadata.contributors.affiliations",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor_affiliations"),
+            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         resourceType=PIDRelation(
             "metadata.resourceType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("resource-types"),
         ),
         subjectCategories_item=PIDRelation(
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/records/jsonschemas/common-1.0.0.json` & `nr-metadata-1.0.9/nr_metadata/common/records/jsonschemas/common-1.0.0.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,49 +1,55 @@
 {
     "type": "object",
     "properties": {
         "metadata": {
+            "type": "object",
             "properties": {
                 "title": {
                     "type": "string"
                 },
                 "additionalTitles": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "title": {
+                                "type": "object",
                                 "properties": {
                                     "lang": {
                                         "type": "string"
                                     },
                                     "value": {
                                         "type": "string"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "titleType": {
-                                "type": "string",
                                 "enum": [
                                     "translatedTitle",
                                     "alternativeTitle",
                                     "subtitle",
                                     "other"
-                                ]
+                                ],
+                                "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "creators": {
+                    "type": "array",
+                    "minItems": 1,
                     "items": {
+                        "type": "object",
                         "properties": {
                             "affiliations": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "id": {
                                             "type": "string"
                                         },
                                         "title": {
                                             "propertyNames": {
                                                 "pattern": "^[a-z]{2}$"
@@ -52,68 +58,66 @@
                                                 "type": "string"
                                             },
                                             "type": "object"
                                         },
                                         "@v": {
                                             "type": "string"
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             },
                             "nameType": {
-                                "type": "string",
                                 "enum": [
                                     "Organizational",
                                     "Personal"
-                                ]
+                                ],
+                                "type": "string"
                             },
                             "fullName": {
                                 "type": "string"
                             },
                             "authorityIdentifiers": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
-                                            "type": "string",
                                             "enum": [
                                                 "orcid",
                                                 "scopusID",
                                                 "researcherID",
                                                 "czenasAutID",
                                                 "vedidk",
                                                 "institutionalID",
                                                 "ISNI",
                                                 "ROR",
                                                 "ICO",
                                                 "DOI"
-                                            ]
+                                            ],
+                                            "type": "string"
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
-                    "minItems": 1,
                     "uniqueItems": true
                 },
                 "contributors": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "role": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "propertyNames": {
                                             "pattern": "^[a-z]{2}$"
@@ -122,19 +126,20 @@
                                             "type": "string"
                                         },
                                         "type": "object"
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "affiliations": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "id": {
                                             "type": "string"
                                         },
                                         "title": {
                                             "propertyNames": {
                                                 "pattern": "^[a-z]{2}$"
@@ -143,64 +148,61 @@
                                                 "type": "string"
                                             },
                                             "type": "object"
                                         },
                                         "@v": {
                                             "type": "string"
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             },
                             "nameType": {
-                                "type": "string",
                                 "enum": [
                                     "Organizational",
                                     "Personal"
-                                ]
+                                ],
+                                "type": "string"
                             },
                             "fullName": {
                                 "type": "string"
                             },
                             "authorityIdentifiers": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
-                                            "type": "string",
                                             "enum": [
                                                 "orcid",
                                                 "scopusID",
                                                 "researcherID",
                                                 "czenasAutID",
                                                 "vedidk",
                                                 "institutionalID",
                                                 "ISNI",
                                                 "ROR",
                                                 "ICO",
                                                 "DOI"
-                                            ]
+                                            ],
+                                            "type": "string"
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "resourceType": {
+                    "type": "object",
                     "properties": {
                         "id": {
                             "type": "string"
                         },
                         "title": {
                             "propertyNames": {
                                 "pattern": "^[a-z]{2}$"
@@ -209,64 +211,65 @@
                                 "type": "string"
                             },
                             "type": "object"
                         },
                         "@v": {
                             "type": "string"
                         }
-                    },
-                    "type": "object"
+                    }
                 },
                 "dateAvailable": {
                     "type": "string"
                 },
                 "dateModified": {
                     "type": "string"
                 },
                 "subjects": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "subjectScheme": {
                                 "type": "string"
                             },
                             "subject": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "lang": {
                                             "type": "string"
                                         },
                                         "value": {
                                             "type": "string"
                                         }
-                                    },
-                                    "type": "object"
-                                },
-                                "type": "array"
+                                    }
+                                }
                             },
                             "valueURI": {
                                 "type": "string"
                             },
                             "classificationCode": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "publishers": {
+                    "type": "array",
                     "items": {
                         "type": "string"
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "subjectCategories": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "propertyNames": {
                                     "pattern": "^[a-z]{2}$"
@@ -275,22 +278,24 @@
                                     "type": "string"
                                 },
                                 "type": "object"
                             },
                             "@v": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "languages": {
+                    "type": "array",
+                    "minItems": 1,
                     "items": {
+                        "required": true,
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "propertyNames": {
                                     "pattern": "^[a-z]{2}$"
@@ -299,73 +304,71 @@
                                     "type": "string"
                                 },
                                 "type": "object"
                             },
                             "@v": {
                                 "type": "string"
                             }
-                        },
-                        "required": true,
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
-                    "minItems": 1,
                     "uniqueItems": true
                 },
                 "notes": {
+                    "type": "array",
                     "items": {
                         "type": "string"
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "abstract": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "lang": {
                                 "type": "string"
                             },
                             "value": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 },
                 "methods": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "lang": {
                                 "type": "string"
                             },
                             "value": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 },
                 "technicalInfo": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "lang": {
                                 "type": "string"
                             },
                             "value": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 },
                 "rights": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "propertyNames": {
                                     "pattern": "^[a-z]{2}$"
@@ -374,21 +377,20 @@
                                     "type": "string"
                                 },
                                 "type": "object"
                             },
                             "@v": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "accessRights": {
+                    "type": "object",
                     "properties": {
                         "id": {
                             "type": "string"
                         },
                         "title": {
                             "propertyNames": {
                                 "pattern": "^[a-z]{2}$"
@@ -397,28 +399,33 @@
                                 "type": "string"
                             },
                             "type": "object"
                         },
                         "@v": {
                             "type": "string"
                         }
-                    },
-                    "type": "object"
+                    }
                 },
                 "relatedItems": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "itemTitle": {
                                 "type": "string"
                             },
                             "itemCreators": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "affiliations": {
+                                            "type": "array",
                                             "items": {
+                                                "type": "object",
                                                 "properties": {
                                                     "id": {
                                                         "type": "string"
                                                     },
                                                     "title": {
                                                         "propertyNames": {
                                                             "pattern": "^[a-z]{2}$"
@@ -427,67 +434,66 @@
                                                             "type": "string"
                                                         },
                                                         "type": "object"
                                                     },
                                                     "@v": {
                                                         "type": "string"
                                                     }
-                                                },
-                                                "type": "object"
+                                                }
                                             },
-                                            "type": "array",
                                             "uniqueItems": true
                                         },
                                         "nameType": {
-                                            "type": "string",
                                             "enum": [
                                                 "Organizational",
                                                 "Personal"
-                                            ]
+                                            ],
+                                            "type": "string"
                                         },
                                         "fullName": {
                                             "type": "string"
                                         },
                                         "authorityIdentifiers": {
+                                            "type": "array",
                                             "items": {
+                                                "type": "object",
                                                 "properties": {
                                                     "identifier": {
                                                         "type": "string"
                                                     },
                                                     "scheme": {
-                                                        "type": "string",
                                                         "enum": [
                                                             "orcid",
                                                             "scopusID",
                                                             "researcherID",
                                                             "czenasAutID",
                                                             "vedidk",
                                                             "institutionalID",
                                                             "ISNI",
                                                             "ROR",
                                                             "ICO",
                                                             "DOI"
-                                                        ]
+                                                        ],
+                                                        "type": "string"
                                                     }
-                                                },
-                                                "type": "object"
+                                                }
                                             },
-                                            "type": "array",
                                             "uniqueItems": true
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             },
                             "itemContributors": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "role": {
+                                            "type": "object",
                                             "properties": {
                                                 "id": {
                                                     "type": "string"
                                                 },
                                                 "title": {
                                                     "propertyNames": {
                                                         "pattern": "^[a-z]{2}$"
@@ -496,19 +502,20 @@
                                                         "type": "string"
                                                     },
                                                     "type": "object"
                                                 },
                                                 "@v": {
                                                     "type": "string"
                                                 }
-                                            },
-                                            "type": "object"
+                                            }
                                         },
                                         "affiliations": {
+                                            "type": "array",
                                             "items": {
+                                                "type": "object",
                                                 "properties": {
                                                     "id": {
                                                         "type": "string"
                                                     },
                                                     "title": {
                                                         "propertyNames": {
                                                             "pattern": "^[a-z]{2}$"
@@ -517,83 +524,79 @@
                                                             "type": "string"
                                                         },
                                                         "type": "object"
                                                     },
                                                     "@v": {
                                                         "type": "string"
                                                     }
-                                                },
-                                                "type": "object"
+                                                }
                                             },
-                                            "type": "array",
                                             "uniqueItems": true
                                         },
                                         "nameType": {
-                                            "type": "string",
                                             "enum": [
                                                 "Organizational",
                                                 "Personal"
-                                            ]
+                                            ],
+                                            "type": "string"
                                         },
                                         "fullName": {
                                             "type": "string"
                                         },
                                         "authorityIdentifiers": {
+                                            "type": "array",
                                             "items": {
+                                                "type": "object",
                                                 "properties": {
                                                     "identifier": {
                                                         "type": "string"
                                                     },
                                                     "scheme": {
-                                                        "type": "string",
                                                         "enum": [
                                                             "orcid",
                                                             "scopusID",
                                                             "researcherID",
                                                             "czenasAutID",
                                                             "vedidk",
                                                             "institutionalID",
                                                             "ISNI",
                                                             "ROR",
                                                             "ICO",
                                                             "DOI"
-                                                        ]
+                                                        ],
+                                                        "type": "string"
                                                     }
-                                                },
-                                                "type": "object"
+                                                }
                                             },
-                                            "type": "array",
                                             "uniqueItems": true
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             },
                             "itemPIDs": {
+                                "type": "array",
                                 "items": {
+                                    "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
-                                            "type": "string",
                                             "enum": [
                                                 "DOI",
                                                 "Handle",
                                                 "ISBN",
                                                 "ISSN",
                                                 "RIV"
-                                            ]
+                                            ],
+                                            "type": "string"
                                         }
-                                    },
-                                    "type": "object"
+                                    }
                                 },
-                                "type": "array",
                                 "uniqueItems": true
                             },
                             "itemURL": {
                                 "type": "string"
                             },
                             "itemYear": {
                                 "type": "integer"
@@ -610,14 +613,15 @@
                             "itemEndPage": {
                                 "type": "string"
                             },
                             "itemPublisher": {
                                 "type": "string"
                             },
                             "itemRelationType": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "propertyNames": {
                                             "pattern": "^[a-z]{2}$"
@@ -626,18 +630,18 @@
                                             "type": "string"
                                         },
                                         "type": "object"
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "itemResourceType": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "propertyNames": {
                                             "pattern": "^[a-z]{2}$"
@@ -646,36 +650,36 @@
                                             "type": "string"
                                         },
                                         "type": "object"
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "fundingReferences": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "projectID": {
                                 "type": "string"
                             },
                             "projectName": {
                                 "type": "string"
                             },
                             "fundingProgram": {
                                 "type": "string"
                             },
                             "funder": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "propertyNames": {
                                             "pattern": "^[a-z]{2}$"
@@ -684,160 +688,161 @@
                                             "type": "string"
                                         },
                                         "type": "object"
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "version": {
                     "type": "string"
                 },
                 "geoLocations": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "geoLocationPlace": {
                                 "type": "string"
                             },
                             "geoLocationPoint": {
+                                "type": "object",
                                 "properties": {
                                     "pointLongitude": {
-                                        "type": "number",
                                         "minimum": -180.0,
+                                        "type": "number",
                                         "maximum": 180.0
                                     },
                                     "pointLatitude": {
-                                        "type": "number",
                                         "minimum": -90.0,
+                                        "type": "number",
                                         "maximum": 90.0
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "accessibility": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "lang": {
                                 "type": "string"
                             },
                             "value": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 },
                 "series": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "seriesTitle": {
                                 "type": "string"
                             },
                             "seriesVolume": {
                                 "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "externalLocation": {
+                    "type": "object",
                     "properties": {
                         "externalLocationURL": {
                             "type": "string"
                         },
                         "externalLocationNote": {
                             "type": "string"
                         }
-                    },
-                    "type": "object"
+                    }
                 },
                 "originalRecord": {
                     "type": "string"
                 },
                 "objectIdentifiers": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "string"
                             },
                             "scheme": {
-                                "type": "string",
                                 "enum": [
                                     "DOI",
                                     "Handle",
                                     "ISBN",
                                     "ISSN",
                                     "RIV"
-                                ]
+                                ],
+                                "type": "string"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
-                    "type": "array",
                     "uniqueItems": true
                 },
                 "systemIdentifiers": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "string"
                             },
                             "scheme": {
-                                "type": "string",
                                 "enum": [
                                     "nusl",
                                     "nuslOAI",
                                     "originalRecordOAI",
                                     "catalogueSysNo",
                                     "nrOAI"
-                                ]
+                                ],
+                                "type": "string"
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 },
                 "events": {
+                    "type": "array",
                     "items": {
+                        "type": "object",
                         "properties": {
                             "eventNameOriginal": {
                                 "type": "string"
                             },
                             "eventNameAlternate": {
+                                "type": "array",
                                 "items": {
                                     "type": "string"
-                                },
-                                "type": "array"
+                                }
                             },
                             "eventDate": {
                                 "type": "string"
                             },
                             "eventLocation": {
+                                "type": "object",
                                 "properties": {
                                     "place": {
                                         "type": "string"
                                     },
                                     "country": {
+                                        "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "string"
                                             },
                                             "title": {
                                                 "propertyNames": {
                                                     "pattern": "^[a-z]{2}$"
@@ -846,27 +851,22 @@
                                                     "type": "string"
                                                 },
                                                 "type": "object"
                                             },
                                             "@v": {
                                                 "type": "string"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
-                    },
-                    "type": "array"
+                        }
+                    }
                 }
-            },
-            "type": "object"
+            }
         },
         "id": {
             "type": "string"
         },
         "created": {
             "type": "string",
             "format": "date"
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json` & `nr-metadata-1.0.9/nr_metadata/common/records/mappings/os-v2/common/common-1.0.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,21 +1,23 @@
 {
     "mappings": {
         "properties": {
             "metadata": {
+                "type": "object",
                 "properties": {
                     "title": {
                         "type": "text",
                         "fields": {
                             "keyword": {
                                 "type": "keyword"
                             }
                         }
                     },
                     "additionalTitles": {
+                        "type": "object",
                         "properties": {
                             "title": {
                                 "type": "object",
                                 "properties": {
                                     "lang": {
                                         "type": "keyword"
                                     },
@@ -56,172 +58,172 @@
                                         "type": "keyword"
                                     }
                                 }
                             },
                             "titleType": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "creators": {
+                        "type": "object",
                         "properties": {
                             "affiliations": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "nameType": {
                                 "type": "keyword"
                             },
                             "fullName": {
                                 "type": "keyword"
                             },
                             "authorityIdentifiers": {
+                                "type": "object",
                                 "properties": {
                                     "identifier": {
                                         "type": "keyword"
                                     },
                                     "scheme": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "contributors": {
+                        "type": "object",
                         "properties": {
                             "role": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "affiliations": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "nameType": {
                                 "type": "keyword"
                             },
                             "fullName": {
                                 "type": "keyword"
                             },
                             "authorityIdentifiers": {
+                                "type": "object",
                                 "properties": {
                                     "identifier": {
                                         "type": "keyword"
                                     },
                                     "scheme": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "resourceType": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "keyword",
                                 "fields": {
                                     "text": {
                                         "type": "search_as_you_type"
                                     }
                                 }
                             },
                             "title": {
                                 "type": "object",
+                                "dynamic": true,
                                 "properties": {
                                     "en": {
                                         "type": "search_as_you_type"
                                     }
                                 },
-                                "dynamic": true,
                                 "enabled": false
                             },
                             "@v": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "dateAvailable": {
                         "type": "date"
                     },
                     "dateModified": {
                         "type": "date"
                     },
                     "subjects": {
+                        "type": "object",
                         "properties": {
                             "subjectScheme": {
                                 "type": "keyword"
                             },
                             "subject": {
                                 "type": "object",
                                 "properties": {
@@ -268,71 +270,70 @@
                             },
                             "valueURI": {
                                 "type": "keyword"
                             },
                             "classificationCode": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "publishers": {
                         "type": "text"
                     },
                     "subjectCategories": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "keyword",
                                 "fields": {
                                     "text": {
                                         "type": "search_as_you_type"
                                     }
                                 }
                             },
                             "title": {
                                 "type": "object",
+                                "dynamic": true,
                                 "properties": {
                                     "en": {
                                         "type": "search_as_you_type"
                                     }
                                 },
-                                "dynamic": true,
                                 "enabled": false
                             },
                             "@v": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "languages": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "keyword",
                                 "fields": {
                                     "text": {
                                         "type": "search_as_you_type"
                                     }
                                 }
                             },
                             "title": {
                                 "type": "object",
+                                "dynamic": true,
                                 "properties": {
                                     "en": {
                                         "type": "search_as_you_type"
                                     }
                                 },
-                                "dynamic": true,
                                 "enabled": false
                             },
                             "@v": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "notes": {
                         "type": "text"
                     },
                     "abstract": {
                         "type": "object",
                         "properties": {
@@ -462,202 +463,203 @@
                         "fields": {
                             "keyword": {
                                 "type": "keyword"
                             }
                         }
                     },
                     "rights": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "keyword",
                                 "fields": {
                                     "text": {
                                         "type": "search_as_you_type"
                                     }
                                 }
                             },
                             "title": {
                                 "type": "object",
+                                "dynamic": true,
                                 "properties": {
                                     "en": {
                                         "type": "search_as_you_type"
                                     }
                                 },
-                                "dynamic": true,
                                 "enabled": false
                             },
                             "@v": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "accessRights": {
+                        "type": "object",
                         "properties": {
                             "id": {
                                 "type": "keyword",
                                 "fields": {
                                     "text": {
                                         "type": "search_as_you_type"
                                     }
                                 }
                             },
                             "title": {
                                 "type": "object",
+                                "dynamic": true,
                                 "properties": {
                                     "en": {
                                         "type": "search_as_you_type"
                                     }
                                 },
-                                "dynamic": true,
                                 "enabled": false
                             },
                             "@v": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "relatedItems": {
+                        "type": "object",
                         "properties": {
                             "itemTitle": {
                                 "type": "text"
                             },
                             "itemCreators": {
+                                "type": "object",
                                 "properties": {
                                     "affiliations": {
+                                        "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "keyword",
                                                 "fields": {
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 }
                                             },
                                             "title": {
                                                 "type": "object",
+                                                "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
-                                                "dynamic": true,
                                                 "enabled": false
                                             },
                                             "@v": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     },
                                     "nameType": {
                                         "type": "keyword"
                                     },
                                     "fullName": {
                                         "type": "keyword"
                                     },
                                     "authorityIdentifiers": {
+                                        "type": "object",
                                         "properties": {
                                             "identifier": {
                                                 "type": "keyword"
                                             },
                                             "scheme": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "itemContributors": {
+                                "type": "object",
                                 "properties": {
                                     "role": {
+                                        "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "keyword",
                                                 "fields": {
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 }
                                             },
                                             "title": {
                                                 "type": "object",
+                                                "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
-                                                "dynamic": true,
                                                 "enabled": false
                                             },
                                             "@v": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     },
                                     "affiliations": {
+                                        "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "keyword",
                                                 "fields": {
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 }
                                             },
                                             "title": {
                                                 "type": "object",
+                                                "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
-                                                "dynamic": true,
                                                 "enabled": false
                                             },
                                             "@v": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     },
                                     "nameType": {
                                         "type": "keyword"
                                     },
                                     "fullName": {
                                         "type": "keyword"
                                     },
                                     "authorityIdentifiers": {
+                                        "type": "object",
                                         "properties": {
                                             "identifier": {
                                                 "type": "keyword"
                                             },
                                             "scheme": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "itemPIDs": {
+                                "type": "object",
                                 "properties": {
                                     "identifier": {
                                         "type": "keyword"
                                     },
                                     "scheme": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "itemURL": {
                                 "type": "keyword"
                             },
                             "itemYear": {
                                 "type": "integer"
                             },
@@ -673,129 +675,128 @@
                             "itemEndPage": {
                                 "type": "keyword"
                             },
                             "itemPublisher": {
                                 "type": "keyword"
                             },
                             "itemRelationType": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             },
                             "itemResourceType": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "fundingReferences": {
+                        "type": "object",
                         "properties": {
                             "projectID": {
                                 "type": "keyword"
                             },
                             "projectName": {
                                 "type": "text"
                             },
                             "fundingProgram": {
                                 "type": "text"
                             },
                             "funder": {
+                                "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "keyword",
                                         "fields": {
                                             "text": {
                                                 "type": "search_as_you_type"
                                             }
                                         }
                                     },
                                     "title": {
                                         "type": "object",
+                                        "dynamic": true,
                                         "properties": {
                                             "en": {
                                                 "type": "search_as_you_type"
                                             }
                                         },
-                                        "dynamic": true,
                                         "enabled": false
                                     },
                                     "@v": {
                                         "type": "keyword"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "version": {
                         "type": "keyword"
                     },
                     "geoLocations": {
+                        "type": "object",
                         "properties": {
                             "geoLocationPlace": {
                                 "type": "keyword"
                             },
                             "geoLocationPoint": {
+                                "type": "object",
                                 "properties": {
                                     "pointLongitude": {
                                         "type": "double"
                                     },
                                     "pointLatitude": {
                                         "type": "double"
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "accessibility": {
                         "type": "object",
                         "properties": {
                             "lang": {
                                 "type": "keyword"
                             },
@@ -834,110 +835,109 @@
                         "fields": {
                             "keyword": {
                                 "type": "keyword"
                             }
                         }
                     },
                     "series": {
+                        "type": "object",
                         "properties": {
                             "seriesTitle": {
                                 "type": "keyword"
                             },
                             "seriesVolume": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "externalLocation": {
+                        "type": "object",
                         "properties": {
                             "externalLocationURL": {
                                 "type": "keyword"
                             },
                             "externalLocationNote": {
                                 "type": "text"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "originalRecord": {
                         "type": "keyword"
                     },
                     "objectIdentifiers": {
+                        "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "keyword"
                             },
                             "scheme": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "systemIdentifiers": {
+                        "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "keyword"
                             },
                             "scheme": {
                                 "type": "keyword"
                             }
-                        },
-                        "type": "object"
+                        }
                     },
                     "events": {
+                        "type": "object",
                         "properties": {
                             "eventNameOriginal": {
                                 "type": "text"
                             },
                             "eventNameAlternate": {
                                 "type": "text"
                             },
                             "eventDate": {
                                 "type": "date_range"
                             },
                             "eventLocation": {
+                                "type": "object",
                                 "properties": {
                                     "place": {
                                         "type": "keyword"
                                     },
                                     "country": {
+                                        "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "keyword",
                                                 "fields": {
                                                     "text": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 }
                                             },
                                             "title": {
                                                 "type": "object",
+                                                "dynamic": true,
                                                 "properties": {
                                                     "en": {
                                                         "type": "search_as_you_type"
                                                     }
                                                 },
-                                                "dynamic": true,
                                                 "enabled": false
                                             },
                                             "@v": {
                                                 "type": "keyword"
                                             }
-                                        },
-                                        "type": "object"
+                                        }
                                     }
-                                },
-                                "type": "object"
+                                }
                             }
-                        },
-                        "type": "object"
+                        }
                     }
-                },
-                "type": "object"
+                }
             },
             "id": {
                 "type": "keyword"
             },
             "created": {
                 "type": "date"
             },
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/records/multilingual_dumper.py` & `nr-metadata-1.0.9/nr_metadata/common/records/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/resources/records/config.py` & `nr-metadata-1.0.9/nr_metadata/common/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/resources/records/ui.py` & `nr-metadata-1.0.9/nr_metadata/common/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/config.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/facets.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/i18nStr_schema.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/i18nStr_schema.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/multilingual_schema.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/schema.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,22 +46,36 @@
     nameType = ma_fields.String()
     fullName = ma_fields.String()
     authorityIdentifiers = ma_fields.List(
         ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
     )
 
 
-class NRAuthorityVocabularySchema(ma.Schema):
-    """NRAuthorityVocabularySchema schema."""
+class NRAuthorityRoleVocabularySchema(ma.Schema):
+    """NRAuthorityRoleVocabularySchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
     title = i18n_strings
     _version = ma_fields.String(data_key="@v", attribute="@v")
 
 
+class NRContributorSchema(ma.Schema):
+    """NRContributorSchema schema."""
+
+    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularySchema())
+    affiliations = ma_fields.List(
+        ma_fields.Nested(lambda: NRAffiliationVocabularySchema())
+    )
+    nameType = ma_fields.String()
+    fullName = ma_fields.String()
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NRAuthorityIdentifierSchema())
+    )
+
+
 class NRResourceTypeVocabularySchema(ma.Schema):
     """NRResourceTypeVocabularySchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
     title = i18n_strings
     _version = ma_fields.String(data_key="@v", attribute="@v")
 
@@ -204,15 +218,15 @@
     """NRCommonMetadataSchema schema."""
 
     title = ma_fields.String()
     additionalTitles = ma_fields.List(
         ma_fields.Nested(lambda: AdditionalTitlesSchema())
     )
     creators = ma_fields.List(ma_fields.Nested(lambda: NRAuthoritySchema()))
-    contributors = ma_fields.List(ma_fields.Nested(lambda: NRAuthoritySchema()))
+    contributors = ma_fields.List(ma_fields.Nested(lambda: NRContributorSchema()))
     resourceType = ma_fields.Nested(lambda: NRResourceTypeVocabularySchema())
     dateAvailable = ma_fields.String(
         validate=[mu_fields_edtf.EDTFValidator(types=(EDTFDate,))]
     )
     dateModified = ma_fields.String(
         validate=[mu_fields_edtf.EDTFValidator(types=(EDTFDate,))]
     )
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/search.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/search.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/common/services/records/ui_schema.py` & `nr-metadata-1.0.9/nr_metadata/common/services/records/ui_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,36 @@
     nameType = l10n.LocalizedEnum(value_prefix="nr_metadata.documents")
     fullName = ma_fields.String()
     authorityIdentifiers = ma_fields.List(
         ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
     )
 
 
-class NRAuthorityVocabularyUISchema(ma.Schema):
-    """NRAuthorityVocabularyUISchema schema."""
+class NRAuthorityRoleVocabularyUISchema(ma.Schema):
+    """NRAuthorityRoleVocabularyUISchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
     title = i18n_strings
     _version = ma_fields.String(data_key="@v", attribute="@v")
 
 
+class NRContributorUISchema(ma.Schema):
+    """NRContributorUISchema schema."""
+
+    role = ma_fields.Nested(lambda: NRAuthorityRoleVocabularyUISchema())
+    affiliations = ma_fields.List(
+        ma_fields.Nested(lambda: NRAffiliationVocabularyUISchema())
+    )
+    nameType = l10n.LocalizedEnum(value_prefix="nr_metadata.documents")
+    fullName = ma_fields.String()
+    authorityIdentifiers = ma_fields.List(
+        ma_fields.Nested(lambda: NRAuthorityIdentifierUISchema())
+    )
+
+
 class NRResourceTypeVocabularyUISchema(ma.Schema):
     """NRResourceTypeVocabularyUISchema schema."""
 
     _id = ma_fields.String(data_key="id", attribute="id")
     title = i18n_strings
     _version = ma_fields.String(data_key="@v", attribute="@v")
 
@@ -198,15 +212,15 @@
     """NRCommonMetadataUISchema schema."""
 
     title = ma_fields.String()
     additionalTitles = ma_fields.List(
         ma_fields.Nested(lambda: AdditionalTitlesUISchema())
     )
     creators = ma_fields.List(ma_fields.Nested(lambda: NRAuthorityUIUISchema()))
-    contributors = ma_fields.List(ma_fields.Nested(lambda: NRAuthorityUIUISchema()))
+    contributors = ma_fields.List(ma_fields.Nested(lambda: NRContributorUISchema()))
     resourceType = ma_fields.Nested(lambda: NRResourceTypeVocabularyUISchema())
     dateAvailable = l10n.LocalizedEDTF()
     dateModified = l10n.LocalizedEDTF()
     subjects = ma_fields.List(ma_fields.Nested(lambda: NRSubjectUISchema()))
     publishers = ma_fields.List(ma_fields.String())
     subjectCategories = ma_fields.List(
         ma_fields.Nested(lambda: NRSubjectCategoryVocabularyUISchema())
```

### Comparing `nr-metadata-1.0.8/nr_metadata/common/views.py` & `nr-metadata-1.0.9/nr_metadata/common/views.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/cli.py` & `nr-metadata-1.0.9/nr_metadata/documents/cli.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/config.py` & `nr-metadata-1.0.9/nr_metadata/documents/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/ext.py` & `nr-metadata-1.0.9/nr_metadata/documents/ext.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/models/model.json` & `nr-metadata-1.0.9/nr_metadata/documents/models/model.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999983791225%*

 * *Differences: {"'model'": "{'properties': {'metadata': {'properties': {'creators': {'items': {'properties': "*

 * *            "{'affiliations': {'items': {'pid-field': "*

 * *            '\'Vocabulary.pid.with_type_ctx("institutions")\', \'relation-args\': {\'pid_field\': '*

 * *            '\'Vocabulary.pid.with_type_ctx("institutions")\'}}}}}}, \'contributors\': {\'items\': '*

 * *            "{'marshmallow': {'schema-class': "*

 * *            "'nr_metadata.common.services.records.schema.NRContributorSchema', 'imports': {0: "*

 * *            "{' […]*

```diff
@@ -666,18 +666,18 @@
                     },
                     "contributors": {
                         "items": {
                             "marshmallow": {
                                 "field-class": "ma_fields.Nested",
                                 "imports": [
                                     {
-                                        "import": "nr_metadata.common.services.records.schema.NRAuthoritySchema"
+                                        "import": "nr_metadata.common.services.records.schema.NRContributorSchema"
                                     }
                                 ],
-                                "schema-class": "nr_metadata.common.services.records.schema.NRAuthoritySchema",
+                                "schema-class": "nr_metadata.common.services.records.schema.NRContributorSchema",
                                 "validators": []
                             },
                             "properties": {
                                 "affiliations": {
                                     "items": {
                                         "hint.cs": "Uve\u010fte instituci/instituce, pod jej\u00ed\u017e z\u00e1\u0161titou jste se na tvorb\u011b objektu pod\u00edleli.",
                                         "imports": [
@@ -718,15 +718,15 @@
                                             ],
                                             "schema-class": "nr_metadata.common.services.records.schema.NRAffiliationVocabularySchema",
                                             "validators": []
                                         },
                                         "model": "vocabularies",
                                         "model-class": "Vocabulary",
                                         "name": "affiliations_item",
-                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor_affiliations\")",
+                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
                                             "@v": {
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.String",
                                                     "field-name": "_version",
                                                     "imports": [],
                                                     "validators": []
@@ -804,15 +804,15 @@
                                                         "validators": []
                                                     }
                                                 }
                                             }
                                         },
                                         "relation-args": {
                                             "keys": "['id', 'title']",
-                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"contributor_affiliations\")"
+                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"institutions\")"
                                         },
                                         "relation-class": "PIDRelation",
                                         "sample": {
                                             "faker": "company",
                                             "skip": false
                                         },
                                         "schema-prefix": "AffiliationsItem",
@@ -1035,18 +1035,18 @@
                                     ],
                                     "label.cs": "Role p\u0159isp\u011bvatele",
                                     "label.en": "Contributor's role",
                                     "marshmallow": {
                                         "field-class": "ma_fields.Nested",
                                         "imports": [
                                             {
-                                                "import": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema"
+                                                "import": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema"
                                             }
                                         ],
-                                        "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema",
+                                        "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema",
                                         "validators": []
                                     },
                                     "model": "vocabularies",
                                     "model-class": "Vocabulary",
                                     "name": "role",
                                     "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
                                     "properties": {
@@ -1141,33 +1141,33 @@
                                     "type": "relation",
                                     "ui": {
                                         "detail": "authority",
                                         "marshmallow": {
                                             "field-class": "ma_fields.Nested",
                                             "imports": [
                                                 {
-                                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                 }
                                             ],
-                                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                         }
                                     }
                                 }
                             },
                             "type": "object",
                             "ui": {
                                 "detail": "contributor",
                                 "marshmallow": {
                                     "field-class": "ma_fields.Nested",
                                     "imports": [
                                         {
-                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                            "import": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                         }
                                     ],
-                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                 }
                             }
                         },
                         "marshmallow": {
                             "field-class": "ma_fields.List",
                             "imports": [],
                             "validators": []
@@ -1234,15 +1234,15 @@
                                             ],
                                             "schema-class": "nr_metadata.common.services.records.schema.NRAffiliationVocabularySchema",
                                             "validators": []
                                         },
                                         "model": "vocabularies",
                                         "model-class": "Vocabulary",
                                         "name": "affiliations_item",
-                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"creator_affiliations\")",
+                                        "pid-field": "Vocabulary.pid.with_type_ctx(\"institutions\")",
                                         "properties": {
                                             "@v": {
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.String",
                                                     "field-name": "_version",
                                                     "imports": [],
                                                     "validators": []
@@ -1320,15 +1320,15 @@
                                                         "validators": []
                                                     }
                                                 }
                                             }
                                         },
                                         "relation-args": {
                                             "keys": "['id', 'title']",
-                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"creator_affiliations\")"
+                                            "pid_field": "Vocabulary.pid.with_type_ctx(\"institutions\")"
                                         },
                                         "relation-class": "PIDRelation",
                                         "sample": {
                                             "faker": "company",
                                             "skip": false
                                         },
                                         "schema-prefix": "AffiliationsItem",
@@ -3209,18 +3209,18 @@
                                                 ],
                                                 "label.cs": "Role p\u0159isp\u011bvatele",
                                                 "label.en": "Contributor's role",
                                                 "marshmallow": {
                                                     "field-class": "ma_fields.Nested",
                                                     "imports": [
                                                         {
-                                                            "import": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema"
+                                                            "import": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema"
                                                         }
                                                     ],
-                                                    "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityVocabularySchema",
+                                                    "schema-class": "nr_metadata.common.services.records.schema.NRAuthorityRoleVocabularySchema",
                                                     "validators": []
                                                 },
                                                 "model": "vocabularies",
                                                 "model-class": "Vocabulary",
                                                 "name": "role",
                                                 "pid-field": "Vocabulary.pid.with_type_ctx(\"contributor-roles\")",
                                                 "properties": {
@@ -3315,18 +3315,18 @@
                                                 "type": "relation",
                                                 "ui": {
                                                     "detail": "authority",
                                                     "marshmallow": {
                                                         "field-class": "ma_fields.Nested",
                                                         "imports": [
                                                             {
-                                                                "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                                "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                             }
                                                         ],
-                                                        "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                        "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                     }
                                                 }
                                             }
                                         },
                                         "type": "object",
                                         "ui": {
                                             "detail": "contributor",
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/models/ui.json` & `nr-metadata-1.0.9/nr_metadata/documents/models/ui.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999998661849875%*

 * *Differences: {"'children'": "{'metadata': {'children': {'contributors': {'child': {'marshmallow': "*

 * *               "{'schema-class': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRContributorUISchema', 'imports': "*

 * *               "{0: {'import': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRContributorUISchema'}}}, "*

 * *               "'children': {'role': {'marshmallow': {'schema-class': "*

 * *               "'nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISch […]*

```diff
@@ -455,31 +455,31 @@
                                 "hint": "metadata/contributors/role.hint",
                                 "input": "relation",
                                 "label": "metadata/contributors/role.label",
                                 "marshmallow": {
                                     "field-class": "ma_fields.Nested",
                                     "imports": [
                                         {
-                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                            "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                         }
                                     ],
-                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                    "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                 }
                             }
                         },
                         "detail": "contributor",
                         "input": "contributor",
                         "marshmallow": {
                             "field-class": "ma_fields.Nested",
                             "imports": [
                                 {
-                                    "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                                    "import": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                                 }
                             ],
-                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityUIUISchema"
+                            "schema-class": "nr_metadata.common.services.records.ui_schema.NRContributorUISchema"
                         }
                     },
                     "detail": "array",
                     "help": "metadata/contributors.help",
                     "hint": "metadata/contributors.hint",
                     "input": "array",
                     "label": "metadata/contributors.label",
@@ -1442,18 +1442,18 @@
                                             "hint": "metadata/relatedItems/itemContributors/role.hint",
                                             "input": "relation",
                                             "label": "metadata/relatedItems/itemContributors/role.label",
                                             "marshmallow": {
                                                 "field-class": "ma_fields.Nested",
                                                 "imports": [
                                                     {
-                                                        "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                        "import": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                                     }
                                                 ],
-                                                "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityVocabularyUISchema"
+                                                "schema-class": "nr_metadata.common.services.records.ui_schema.NRAuthorityRoleVocabularyUISchema"
                                             }
                                         }
                                     },
                                     "detail": "contributor",
                                     "input": "itemcontributor",
                                     "marshmallow": {
                                         "field-class": "ma_fields.Nested",
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/records/api.py` & `nr-metadata-1.0.9/nr_metadata/documents/records/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,25 @@
             "metadata.thesis.degreeGrantor",
             keys=["id", "title", "hierarchy"],
             pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         affiliations_item=PIDRelation(
             "metadata.creators.affiliations",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("creator_affiliations"),
+            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         role=PIDRelation(
             "metadata.contributors.role",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("contributor-roles"),
         ),
         affiliations_item_1=PIDRelation(
             "metadata.contributors.affiliations",
             keys=["id", "title"],
-            pid_field=Vocabulary.pid.with_type_ctx("contributor_affiliations"),
+            pid_field=Vocabulary.pid.with_type_ctx("institutions"),
         ),
         resourceType=PIDRelation(
             "metadata.resourceType",
             keys=["id", "title"],
             pid_field=Vocabulary.pid.with_type_ctx("resource-types"),
         ),
         subjectCategories_item=PIDRelation(
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json` & `nr-metadata-1.0.9/nr_metadata/documents/records/jsonschemas/documents-1.0.0.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -18,19 +18,19 @@
                             "type": "object",
                             "properties": {
                                 "id": {
                                     "type": "string"
                                 },
                                 "title": {
                                     "type": "object",
-                                    "propertyNames": {
-                                        "pattern": "^[a-z]{2}$"
-                                    },
                                     "additionalProperties": {
                                         "type": "string"
+                                    },
+                                    "propertyNames": {
+                                        "pattern": "^[a-z]{2}$"
                                     }
                                 },
                                 "hierarchy": {
                                     "type": "object",
                                     "properties": {
                                         "parent": {
                                             "type": "string"
@@ -38,19 +38,19 @@
                                         "level": {
                                             "type": "integer"
                                         },
                                         "title": {
                                             "type": "array",
                                             "items": {
                                                 "type": "object",
-                                                "propertyNames": {
-                                                    "pattern": "^[a-z]{2}$"
-                                                },
                                                 "additionalProperties": {
                                                     "type": "string"
+                                                },
+                                                "propertyNames": {
+                                                    "pattern": "^[a-z]{2}$"
                                                 }
                                             }
                                         },
                                         "ancestors": {
                                             "type": "array",
                                             "items": {
                                                 "type": "string"
@@ -74,15 +74,14 @@
                 "collection": {
                     "type": "string"
                 },
                 "title": {
                     "type": "string"
                 },
                 "additionalTitles": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "title": {
                                 "type": "object",
                                 "properties": {
@@ -91,214 +90,214 @@
                                     },
                                     "value": {
                                         "type": "string"
                                     }
                                 }
                             },
                             "titleType": {
+                                "type": "string",
                                 "enum": [
                                     "translatedTitle",
                                     "alternativeTitle",
                                     "subtitle",
                                     "other"
-                                ],
-                                "type": "string"
+                                ]
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "creators": {
-                    "uniqueItems": true,
                     "type": "array",
+                    "minItems": 1,
                     "items": {
                         "type": "object",
                         "properties": {
                             "affiliations": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "id": {
                                             "type": "string"
                                         },
                                         "title": {
                                             "type": "object",
-                                            "propertyNames": {
-                                                "pattern": "^[a-z]{2}$"
-                                            },
                                             "additionalProperties": {
                                                 "type": "string"
+                                            },
+                                            "propertyNames": {
+                                                "pattern": "^[a-z]{2}$"
                                             }
                                         },
                                         "@v": {
                                             "type": "string"
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             },
                             "nameType": {
+                                "type": "string",
                                 "enum": [
                                     "Organizational",
                                     "Personal"
-                                ],
-                                "type": "string"
+                                ]
                             },
                             "fullName": {
                                 "type": "string"
                             },
                             "authorityIdentifiers": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
+                                            "type": "string",
                                             "enum": [
                                                 "orcid",
                                                 "scopusID",
                                                 "researcherID",
                                                 "czenasAutID",
                                                 "vedidk",
                                                 "institutionalID",
                                                 "ISNI",
                                                 "ROR",
                                                 "ICO",
                                                 "DOI"
-                                            ],
-                                            "type": "string"
+                                            ]
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             }
                         }
                     },
-                    "minItems": 1
+                    "uniqueItems": true
                 },
                 "contributors": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "role": {
                                 "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object",
-                                        "propertyNames": {
-                                            "pattern": "^[a-z]{2}$"
-                                        },
                                         "additionalProperties": {
                                             "type": "string"
+                                        },
+                                        "propertyNames": {
+                                            "pattern": "^[a-z]{2}$"
                                         }
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
                                 }
                             },
                             "affiliations": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "id": {
                                             "type": "string"
                                         },
                                         "title": {
                                             "type": "object",
-                                            "propertyNames": {
-                                                "pattern": "^[a-z]{2}$"
-                                            },
                                             "additionalProperties": {
                                                 "type": "string"
+                                            },
+                                            "propertyNames": {
+                                                "pattern": "^[a-z]{2}$"
                                             }
                                         },
                                         "@v": {
                                             "type": "string"
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             },
                             "nameType": {
+                                "type": "string",
                                 "enum": [
                                     "Organizational",
                                     "Personal"
-                                ],
-                                "type": "string"
+                                ]
                             },
                             "fullName": {
                                 "type": "string"
                             },
                             "authorityIdentifiers": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
+                                            "type": "string",
                                             "enum": [
                                                 "orcid",
                                                 "scopusID",
                                                 "researcherID",
                                                 "czenasAutID",
                                                 "vedidk",
                                                 "institutionalID",
                                                 "ISNI",
                                                 "ROR",
                                                 "ICO",
                                                 "DOI"
-                                            ],
-                                            "type": "string"
+                                            ]
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "resourceType": {
                     "type": "object",
                     "properties": {
                         "id": {
                             "type": "string"
                         },
                         "title": {
                             "type": "object",
-                            "propertyNames": {
-                                "pattern": "^[a-z]{2}$"
-                            },
                             "additionalProperties": {
                                 "type": "string"
+                            },
+                            "propertyNames": {
+                                "pattern": "^[a-z]{2}$"
                             }
                         },
                         "@v": {
                             "type": "string"
                         }
                     }
                 },
                 "dateAvailable": {
                     "type": "string"
                 },
                 "dateModified": {
                     "type": "string"
                 },
                 "subjects": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "subjectScheme": {
                                 "type": "string"
                             },
@@ -319,79 +318,80 @@
                             "valueURI": {
                                 "type": "string"
                             },
                             "classificationCode": {
                                 "type": "string"
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "publishers": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "string"
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "subjectCategories": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "type": "object",
-                                "propertyNames": {
-                                    "pattern": "^[a-z]{2}$"
-                                },
                                 "additionalProperties": {
                                     "type": "string"
+                                },
+                                "propertyNames": {
+                                    "pattern": "^[a-z]{2}$"
                                 }
                             },
                             "@v": {
                                 "type": "string"
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "languages": {
-                    "uniqueItems": true,
                     "type": "array",
+                    "minItems": 1,
                     "items": {
                         "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "type": "object",
-                                "propertyNames": {
-                                    "pattern": "^[a-z]{2}$"
-                                },
                                 "additionalProperties": {
                                     "type": "string"
+                                },
+                                "propertyNames": {
+                                    "pattern": "^[a-z]{2}$"
                                 }
                             },
                             "@v": {
                                 "type": "string"
                             }
                         },
                         "required": true
                     },
-                    "minItems": 1
+                    "uniqueItems": true
                 },
                 "notes": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "string"
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "abstract": {
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "lang": {
@@ -428,247 +428,246 @@
                             "value": {
                                 "type": "string"
                             }
                         }
                     }
                 },
                 "rights": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "id": {
                                 "type": "string"
                             },
                             "title": {
                                 "type": "object",
-                                "propertyNames": {
-                                    "pattern": "^[a-z]{2}$"
-                                },
                                 "additionalProperties": {
                                     "type": "string"
+                                },
+                                "propertyNames": {
+                                    "pattern": "^[a-z]{2}$"
                                 }
                             },
                             "@v": {
                                 "type": "string"
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "accessRights": {
                     "type": "object",
                     "properties": {
                         "id": {
                             "type": "string"
                         },
                         "title": {
                             "type": "object",
-                            "propertyNames": {
-                                "pattern": "^[a-z]{2}$"
-                            },
                             "additionalProperties": {
                                 "type": "string"
+                            },
+                            "propertyNames": {
+                                "pattern": "^[a-z]{2}$"
                             }
                         },
                         "@v": {
                             "type": "string"
                         }
                     }
                 },
                 "relatedItems": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "itemTitle": {
                                 "type": "string"
                             },
                             "itemCreators": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "affiliations": {
-                                            "uniqueItems": true,
                                             "type": "array",
                                             "items": {
                                                 "type": "object",
                                                 "properties": {
                                                     "id": {
                                                         "type": "string"
                                                     },
                                                     "title": {
                                                         "type": "object",
-                                                        "propertyNames": {
-                                                            "pattern": "^[a-z]{2}$"
-                                                        },
                                                         "additionalProperties": {
                                                             "type": "string"
+                                                        },
+                                                        "propertyNames": {
+                                                            "pattern": "^[a-z]{2}$"
                                                         }
                                                     },
                                                     "@v": {
                                                         "type": "string"
                                                     }
                                                 }
-                                            }
+                                            },
+                                            "uniqueItems": true
                                         },
                                         "nameType": {
+                                            "type": "string",
                                             "enum": [
                                                 "Organizational",
                                                 "Personal"
-                                            ],
-                                            "type": "string"
+                                            ]
                                         },
                                         "fullName": {
                                             "type": "string"
                                         },
                                         "authorityIdentifiers": {
-                                            "uniqueItems": true,
                                             "type": "array",
                                             "items": {
                                                 "type": "object",
                                                 "properties": {
                                                     "identifier": {
                                                         "type": "string"
                                                     },
                                                     "scheme": {
+                                                        "type": "string",
                                                         "enum": [
                                                             "orcid",
                                                             "scopusID",
                                                             "researcherID",
                                                             "czenasAutID",
                                                             "vedidk",
                                                             "institutionalID",
                                                             "ISNI",
                                                             "ROR",
                                                             "ICO",
                                                             "DOI"
-                                                        ],
-                                                        "type": "string"
+                                                        ]
                                                     }
                                                 }
-                                            }
+                                            },
+                                            "uniqueItems": true
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             },
                             "itemContributors": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "role": {
                                             "type": "object",
                                             "properties": {
                                                 "id": {
                                                     "type": "string"
                                                 },
                                                 "title": {
                                                     "type": "object",
-                                                    "propertyNames": {
-                                                        "pattern": "^[a-z]{2}$"
-                                                    },
                                                     "additionalProperties": {
                                                         "type": "string"
+                                                    },
+                                                    "propertyNames": {
+                                                        "pattern": "^[a-z]{2}$"
                                                     }
                                                 },
                                                 "@v": {
                                                     "type": "string"
                                                 }
                                             }
                                         },
                                         "affiliations": {
-                                            "uniqueItems": true,
                                             "type": "array",
                                             "items": {
                                                 "type": "object",
                                                 "properties": {
                                                     "id": {
                                                         "type": "string"
                                                     },
                                                     "title": {
                                                         "type": "object",
-                                                        "propertyNames": {
-                                                            "pattern": "^[a-z]{2}$"
-                                                        },
                                                         "additionalProperties": {
                                                             "type": "string"
+                                                        },
+                                                        "propertyNames": {
+                                                            "pattern": "^[a-z]{2}$"
                                                         }
                                                     },
                                                     "@v": {
                                                         "type": "string"
                                                     }
                                                 }
-                                            }
+                                            },
+                                            "uniqueItems": true
                                         },
                                         "nameType": {
+                                            "type": "string",
                                             "enum": [
                                                 "Organizational",
                                                 "Personal"
-                                            ],
-                                            "type": "string"
+                                            ]
                                         },
                                         "fullName": {
                                             "type": "string"
                                         },
                                         "authorityIdentifiers": {
-                                            "uniqueItems": true,
                                             "type": "array",
                                             "items": {
                                                 "type": "object",
                                                 "properties": {
                                                     "identifier": {
                                                         "type": "string"
                                                     },
                                                     "scheme": {
+                                                        "type": "string",
                                                         "enum": [
                                                             "orcid",
                                                             "scopusID",
                                                             "researcherID",
                                                             "czenasAutID",
                                                             "vedidk",
                                                             "institutionalID",
                                                             "ISNI",
                                                             "ROR",
                                                             "ICO",
                                                             "DOI"
-                                                        ],
-                                                        "type": "string"
+                                                        ]
                                                     }
                                                 }
-                                            }
+                                            },
+                                            "uniqueItems": true
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             },
                             "itemPIDs": {
-                                "uniqueItems": true,
                                 "type": "array",
                                 "items": {
                                     "type": "object",
                                     "properties": {
                                         "identifier": {
                                             "type": "string"
                                         },
                                         "scheme": {
+                                            "type": "string",
                                             "enum": [
                                                 "DOI",
                                                 "Handle",
                                                 "ISBN",
                                                 "ISSN",
                                                 "RIV"
-                                            ],
-                                            "type": "string"
+                                            ]
                                         }
                                     }
-                                }
+                                },
+                                "uniqueItems": true
                             },
                             "itemURL": {
                                 "type": "string"
                             },
                             "itemYear": {
                                 "type": "integer"
                             },
@@ -691,19 +690,19 @@
                                 "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object",
-                                        "propertyNames": {
-                                            "pattern": "^[a-z]{2}$"
-                                        },
                                         "additionalProperties": {
                                             "type": "string"
+                                        },
+                                        "propertyNames": {
+                                            "pattern": "^[a-z]{2}$"
                                         }
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
                                 }
                             },
@@ -711,31 +710,31 @@
                                 "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object",
-                                        "propertyNames": {
-                                            "pattern": "^[a-z]{2}$"
-                                        },
                                         "additionalProperties": {
                                             "type": "string"
+                                        },
+                                        "propertyNames": {
+                                            "pattern": "^[a-z]{2}$"
                                         }
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
                                 }
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "fundingReferences": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "projectID": {
                                 "type": "string"
                             },
@@ -749,58 +748,59 @@
                                 "type": "object",
                                 "properties": {
                                     "id": {
                                         "type": "string"
                                     },
                                     "title": {
                                         "type": "object",
-                                        "propertyNames": {
-                                            "pattern": "^[a-z]{2}$"
-                                        },
                                         "additionalProperties": {
                                             "type": "string"
+                                        },
+                                        "propertyNames": {
+                                            "pattern": "^[a-z]{2}$"
                                         }
                                     },
                                     "@v": {
                                         "type": "string"
                                     }
                                 }
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "version": {
                     "type": "string"
                 },
                 "geoLocations": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "geoLocationPlace": {
                                 "type": "string"
                             },
                             "geoLocationPoint": {
                                 "type": "object",
                                 "properties": {
                                     "pointLongitude": {
-                                        "minimum": -180.0,
                                         "type": "number",
+                                        "minimum": -180.0,
                                         "maximum": 180.0
                                     },
                                     "pointLatitude": {
-                                        "minimum": -90.0,
                                         "type": "number",
+                                        "minimum": -90.0,
                                         "maximum": 90.0
                                     }
                                 }
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "accessibility": {
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "lang": {
@@ -809,27 +809,27 @@
                             "value": {
                                 "type": "string"
                             }
                         }
                     }
                 },
                 "series": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "seriesTitle": {
                                 "type": "string"
                             },
                             "seriesVolume": {
                                 "type": "string"
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "externalLocation": {
                     "type": "object",
                     "properties": {
                         "externalLocationURL": {
                             "type": "string"
                         },
@@ -838,52 +838,52 @@
                         }
                     }
                 },
                 "originalRecord": {
                     "type": "string"
                 },
                 "objectIdentifiers": {
-                    "uniqueItems": true,
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "string"
                             },
                             "scheme": {
+                                "type": "string",
                                 "enum": [
                                     "DOI",
                                     "Handle",
                                     "ISBN",
                                     "ISSN",
                                     "RIV"
-                                ],
-                                "type": "string"
+                                ]
                             }
                         }
-                    }
+                    },
+                    "uniqueItems": true
                 },
                 "systemIdentifiers": {
                     "type": "array",
                     "items": {
                         "type": "object",
                         "properties": {
                             "identifier": {
                                 "type": "string"
                             },
                             "scheme": {
+                                "type": "string",
                                 "enum": [
                                     "nusl",
                                     "nuslOAI",
                                     "originalRecordOAI",
                                     "catalogueSysNo",
                                     "nrOAI"
-                                ],
-                                "type": "string"
+                                ]
                             }
                         }
                     }
                 },
                 "events": {
                     "type": "array",
                     "items": {
@@ -911,19 +911,19 @@
                                         "type": "object",
                                         "properties": {
                                             "id": {
                                                 "type": "string"
                                             },
                                             "title": {
                                                 "type": "object",
-                                                "propertyNames": {
-                                                    "pattern": "^[a-z]{2}$"
-                                                },
                                                 "additionalProperties": {
                                                     "type": "string"
+                                                },
+                                                "propertyNames": {
+                                                    "pattern": "^[a-z]{2}$"
                                                 }
                                             },
                                             "@v": {
                                                 "type": "string"
                                             }
                                         }
                                     }
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json` & `nr-metadata-1.0.9/nr_metadata/documents/records/mappings/os-v2/documents/documents-1.0.0.json`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/records/multilingual_dumper.py` & `nr-metadata-1.0.9/nr_metadata/documents/records/multilingual_dumper.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/resources/records/config.py` & `nr-metadata-1.0.9/nr_metadata/documents/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/resources/records/ui.py` & `nr-metadata-1.0.9/nr_metadata/documents/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/config.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/config.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/facets.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/i18nStr_schema.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/i18nStr_schema.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/multilingual_schema.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/schema.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from oarepo_runtime.validation import validate_date
 from oarepo_vocabularies.services.schemas import HierarchySchema
 
 from nr_metadata.common.services.records.schema import (
     AdditionalTitlesSchema,
     NRAccessRightsVocabularySchema,
     NRAffiliationVocabularySchema,
+    NRAuthorityRoleVocabularySchema,
     NRAuthoritySchema,
-    NRAuthorityVocabularySchema,
+    NRContributorSchema,
     NRCountryVocabularySchema,
     NREventSchema,
     NRExternalLocationSchema,
     NRFunderVocabularySchema,
     NRFundingReferenceSchema,
     NRGeoLocationPointSchema,
     NRGeoLocationSchema,
@@ -69,15 +70,15 @@
     thesis = ma_fields.Nested(lambda: NRThesisSchema())
     collection = ma_fields.String()
     title = ma_fields.String()
     additionalTitles = ma_fields.List(
         ma_fields.Nested(lambda: AdditionalTitlesSchema())
     )
     creators = ma_fields.List(ma_fields.Nested(lambda: NRAuthoritySchema()))
-    contributors = ma_fields.List(ma_fields.Nested(lambda: NRAuthoritySchema()))
+    contributors = ma_fields.List(ma_fields.Nested(lambda: NRContributorSchema()))
     resourceType = ma_fields.Nested(lambda: NRResourceTypeVocabularySchema())
     dateAvailable = ma_fields.String(
         validate=[mu_fields_edtf.EDTFValidator(types=(EDTFDate,))]
     )
     dateModified = ma_fields.String(
         validate=[mu_fields_edtf.EDTFValidator(types=(EDTFDate,))]
     )
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/search.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/search.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/services/records/ui_schema.py` & `nr-metadata-1.0.9/nr_metadata/documents/services/records/ui_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from oarepo_runtime.validation import validate_date
 from oarepo_vocabularies.services.ui_schemas import HierarchyUISchema
 
 from nr_metadata.common.services.records.ui_schema import (
     AdditionalTitlesUISchema,
     NRAccessRightsVocabularyUISchema,
     NRAffiliationVocabularyUISchema,
+    NRAuthorityRoleVocabularyUISchema,
     NRAuthorityUIUISchema,
-    NRAuthorityVocabularyUISchema,
+    NRContributorUISchema,
     NRCountryVocabularyUISchema,
     NREventUISchema,
     NRExternalLocationUISchema,
     NRFunderVocabularyUISchema,
     NRFundingReferenceUISchema,
     NRGeoLocationPointUISchema,
     NRGeoLocationUISchema,
@@ -69,15 +70,15 @@
     thesis = ma_fields.Nested(lambda: NRThesisUISchema())
     collection = ma_fields.String()
     title = ma_fields.String()
     additionalTitles = ma_fields.List(
         ma_fields.Nested(lambda: AdditionalTitlesUISchema())
     )
     creators = ma_fields.List(ma_fields.Nested(lambda: NRAuthorityUIUISchema()))
-    contributors = ma_fields.List(ma_fields.Nested(lambda: NRAuthorityUIUISchema()))
+    contributors = ma_fields.List(ma_fields.Nested(lambda: NRContributorUISchema()))
     resourceType = ma_fields.Nested(lambda: NRResourceTypeVocabularyUISchema())
     dateAvailable = l10n.LocalizedEDTF()
     dateModified = l10n.LocalizedEDTF()
     subjects = ma_fields.List(ma_fields.Nested(lambda: NRSubjectUISchema()))
     publishers = ma_fields.List(ma_fields.String())
     subjectCategories = ma_fields.List(
         ma_fields.Nested(lambda: NRSubjectCategoryVocabularyUISchema())
```

### Comparing `nr-metadata-1.0.8/nr_metadata/documents/views.py` & `nr-metadata-1.0.9/nr_metadata/documents/views.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/schema/identifiers.py` & `nr-metadata-1.0.9/nr_metadata/schema/identifiers.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata/ui_schema/identifier.py` & `nr-metadata-1.0.9/nr_metadata/ui_schema/identifier.py`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata.egg-info/PKG-INFO` & `nr-metadata-1.0.9/nr_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nr-metadata
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Generated metadata files for the Czech National Repository"
 Home-page: https://github.com/Narodni-repozitar/ne-metadata
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR
 Platform: any
```

### Comparing `nr-metadata-1.0.8/nr_metadata.egg-info/SOURCES.txt` & `nr-metadata-1.0.9/nr_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/nr_metadata.egg-info/requires.txt` & `nr-metadata-1.0.9/nr_metadata.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nr-metadata-1.0.8/setup.cfg` & `nr-metadata-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nr-metadata
-version = 1.0.8
+version = 1.0.9
 description = "Generated metadata files for the Czech National Repository"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio Czech NR
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```


# Comparing `tmp/housekeeper-4.4.0.tar.gz` & `tmp/housekeeper-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.4.0.tar", last modified: Tue May 16 11:18:43 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.5.0.tar", last modified: Mon May 29 14:16:59 2023, max compression
```

## Comparing `housekeeper-4.4.0.tar` & `housekeeper-4.5.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 11:18:33.000000 housekeeper-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 11:18:33.000000 housekeeper-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 11:18:43.000000 housekeeper-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-16 11:18:33.000000 housekeeper-4.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 11:18:33.000000 housekeeper-4.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:18:33.000000 housekeeper-4.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 11:18:43.000000 housekeeper-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-16 11:18:33.000000 housekeeper-4.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/lane1.spring
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/lane2.spring
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_archive_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_version_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_createhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_readhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_updatehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-29 14:16:47.000000 housekeeper-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 14:16:47.000000 housekeeper-4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 14:16:59.000000 housekeeper-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-29 14:16:47.000000 housekeeper-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/handlers/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-29 14:16:47.000000 housekeeper-4.5.0/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 14:16:59.000000 housekeeper-4.5.0/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-29 14:16:47.000000 housekeeper-4.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 14:16:47.000000 housekeeper-4.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 14:16:59.000000 housekeeper-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-29 14:16:47.000000 housekeeper-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/lane1.spring
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/sequencing_files/lane2.spring
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/filters/test_version_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:16:59.000000 housekeeper-4.5.0/tests/store/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_createhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_readhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/handlers/test_updatehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/store/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-29 14:16:47.000000 housekeeper-4.5.0/tests/test_include.py
```

### Comparing `housekeeper-4.4.0/LICENSE` & `housekeeper-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/PKG-INFO` & `housekeeper-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.4.0
+Version: 4.5.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.4.0/README.md` & `housekeeper-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/cli/add.py` & `housekeeper-4.5.0/housekeeper/cli/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Module for adding via CLI"""
 import datetime as dt
 import logging
 from logging import Logger
 from pathlib import Path
-from typing import List, Dict, Generator
+from typing import Dict, Generator, List
 
 import click
-
+from housekeeper.constants import ROOT
 from housekeeper.date import get_date
 from housekeeper.files import load_json, validate_input
+from housekeeper.include import link_to_relative_path, relative_path
 from housekeeper.store import Store
-from housekeeper.store.models import Bundle, Version, File, Tag
+from housekeeper.store.models import Bundle, Tag, Version
 
 LOG: Logger = logging.getLogger(__name__)
 
 
 def validate_args(arg: str, json: str, arg_name: str) -> None:
     """Check if input is valid
 
@@ -73,43 +74,59 @@
     LOG.info("new bundle added: %s (%s)", new_bundle.name, new_bundle.id)
 
 
 @add.command("file")
 @click.option("-t", "--tag", "tags", multiple=True, help="tag to associate the file by")
 @click.option("-b", "--bundle-name", help="name of bundle that file should be added to")
 @click.option("-j", "--json", help="json formatted input")
+@click.option(
+    "-kip",
+    "--keep-input-path",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="Flag to use the input path in Housekeeper",
+)
 @click.argument("path", required=False)
 @click.pass_context
 def file_cmd(
-    context: click.Context, tags: List[str], bundle_name: str, json: str, path: str
+    context: click.Context,
+    tags: List[str],
+    bundle_name: str,
+    json: str,
+    keep_input_path: bool,
+    path: str,
 ):
     """Add a file to the latest version of a bundle."""
     LOG.info("Running add file")
     store: Store = context.obj["store"]
     validate_args(arg=path, json=json, arg_name="path")
 
     data: Dict = {}
     if json:
         data: Dict = load_json(json)
         validate_input(data, input_type="file")
 
-    file_path = Path(data.get("path", path))
+    file_path: Path = Path(data.get("path", path))
     if not file_path.exists():
         LOG.warning("File: %s does not exist", file_path)
         raise click.Abort
 
     bundle_name = data.get("bundle", bundle_name)
     bundle = store.get_bundle_by_name(bundle_name=bundle_name)
 
     if bundle is None:
         LOG.warning("unknown bundle: %s", bundle_name)
         raise click.Abort
 
     tags = data.get("tags", tags)
-
+    if not keep_input_path:
+        version: Version = bundle.versions[0]
+        link_to_relative_path(version=version, file_path=file_path, root_path=context.obj[ROOT])
+        file_path: Path = relative_path(version=version, file=file_path)
     new_file = store.add_file(file_path=file_path, bundle=bundle, tags=tags)
     store.session.add(new_file)
     store.session.commit()
     LOG.info("new file added: %s (%s)", new_file.path, new_file.id)
 
 
 @add.command("version")
@@ -154,15 +171,15 @@
 @click.option("-f", "--file-id", type=int)
 @click.pass_context
 def tag_cmd(context: click.Context, tags: List[str], file_id: int):
     """Add tags to housekeeper. Use `--file-id` to add tags to existing file"""
     LOG.info("Running add tag")
     store: Store = context.obj["store"]
     file = None
-    if len(tags) == 0:
+    if not tags:
         LOG.warning("No tags provided")
         raise click.Abort
 
     if file_id:
         file = store.get_file_by_id(file_id=file_id)
 
         if not file:
```

### Comparing `housekeeper-4.4.0/housekeeper/cli/core.py` & `housekeeper-4.5.0/housekeeper/cli/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for base CLI"""
 import logging
 from typing import Optional
 
 import click
 import coloredlogs
-import yaml
-
 import housekeeper
+import yaml
+from housekeeper.constants import ROOT
 from housekeeper.store import Store
 
 from . import add, delete, get, include, init
 
 LOG = logging.getLogger(__name__)
 
 
@@ -31,15 +31,15 @@
     """Housekeeper - Access your files!"""
     coloredlogs.install(level=log_level)
     config_values = {}
     if config:
         config_values = yaml.full_load(config)
     context.obj = config_values
     db_path = database or context.obj.get("database")
-    root_path = context.obj["root"] = root or context.obj.get("root")
+    root_path = context.obj[ROOT] = root or context.obj.get(ROOT)
     if not db_path:
         LOG.error("Please point to a database")
         raise click.Abort
     if not root_path:
         LOG.error("Please specify a root dir")
         raise click.Abort
     context.obj["database"] = db_path
```

### Comparing `housekeeper-4.4.0/housekeeper/cli/delete.py` & `housekeeper-4.5.0/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/cli/get.py` & `housekeeper-4.5.0/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/cli/include.py` & `housekeeper-4.5.0/housekeeper/cli/include.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for including files via CLI"""
 import datetime as dt
 import logging
 
 import click
-
+from housekeeper.constants import ROOT
 from housekeeper.exc import VersionIncludedError
 from housekeeper.include import include_version
 from housekeeper.store.api.core import Store
 
 LOG = logging.getLogger(__name__)
 
 
@@ -43,15 +43,15 @@
             LOG.error("Could not find any versions for bundle %s", bundle_name)
             raise click.Abort
 
         LOG.info("Including latest version for %s", bundle_name)
         version_obj = bundle.versions[0]
 
     try:
-        include_version(context.obj["root"], version_obj)
+        include_version(context.obj[ROOT], version_obj)
     except VersionIncludedError as error:
         LOG.warning(error.message)
         raise click.Abort
 
     version_obj.included_at = dt.datetime.now()
     store.session.commit()
     click.echo(click.style("included all files!", fg="green"))
```

### Comparing `housekeeper-4.4.0/housekeeper/cli/init.py` & `housekeeper-4.5.0/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/cli/tables.py` & `housekeeper-4.5.0/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/date.py` & `housekeeper-4.5.0/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/files.py` & `housekeeper-4.5.0/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/include.py` & `housekeeper-4.5.0/housekeeper/include.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for code to include files in housekeeper"""
 import hashlib
 import logging
 import os
 from pathlib import Path
 
 from housekeeper.exc import VersionIncludedError
-from housekeeper.store import models
+from housekeeper.store.models import Version
 
 BLOCKSIZE = 65536
 EMPTY_STR = ""
 LOG = logging.getLogger(__name__)
 
 
 def link_file(file_path: Path, new_path: Path, hardlink: bool = True) -> None:
@@ -19,15 +19,15 @@
         os.link(file_path.resolve(), new_path)
     else:
         LOG.debug("Creating softlink")
         new_path.symlink_to(file_path)
     LOG.info("linked file: %s -> %s", file_path, new_path)
 
 
-def include_version(global_root: str, version_obj: models.Version, hardlink: bool = True):
+def include_version(global_root: str, version_obj: Version, hardlink: bool = True):
     """Include files in existing bundle version.
 
     Including a file means to link them into a folder in the root directory
     """
     LOG.info("Use global root path %s", global_root)
     global_root_dir = Path(global_root)
     if version_obj.included_at:
@@ -51,7 +51,17 @@
     hasher = hashlib.sha1()
     with open(path, "rb") as stream:
         buf = stream.read(BLOCKSIZE)
         while len(buf) > 0:
             hasher.update(buf)
             buf = stream.read(BLOCKSIZE)
     return hasher.hexdigest()
+
+
+def link_to_relative_path(file_path: Path, root_path: Path, version: Version) -> None:
+    """Link the given absolute path to its path when included in the given version and return the relative path."""
+    housekeeper_path: Path = Path(root_path, version.relative_root_dir, file_path.name)
+    link_file(file_path=file_path, new_path=housekeeper_path, hardlink=True)
+
+
+def relative_path(version: Version, file: Path) -> Path:
+    return Path(version.relative_root_dir, file.name)
```

### Comparing `housekeeper-4.4.0/housekeeper/store/api/core.py` & `housekeeper-4.5.0/housekeeper/store/api/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/api/handlers/base.py` & `housekeeper-4.5.0/housekeeper/store/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/api/handlers/create.py` & `housekeeper-4.5.0/housekeeper/store/api/handlers/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module handles adding things to the store"""
 
 import datetime as dt
 import logging
 from pathlib import Path
 from typing import Dict, List, Tuple
-from sqlalchemy.orm import Session
 
-from housekeeper.store.models import Archive, Bundle, File, Tag, Version
 from housekeeper.store.api.handlers.base import BaseHandler
 from housekeeper.store.api.handlers.read import ReadHandler
+from housekeeper.store.models import Archive, Bundle, File, Tag, Version
+from sqlalchemy.orm import Session
 
 LOG = logging.getLogger(__name__)
 
 
 class CreateHandler(BaseHandler):
     """Handles adding things to the store"""
 
@@ -106,24 +106,25 @@
     def add_file(
         self,
         file_path: Path,
         bundle: Bundle,
         to_archive: bool = False,
         tags: List[str] = None,
     ) -> File:
-        """Build a new file object and add it to the latest version of an existing bundle"""
-        version_obj = bundle.versions[0]
+        """Build a new file object and add it to the latest version of an existing bundle."""
+        version = bundle.versions[0]
         tags = tags or []
         tag_objs = [tag_obj for tag_name, tag_obj in self._build_tags(tags).items()]
+        file_path_to_use: str = str(file_path)
         new_file = self.new_file(
-            path=str(file_path.absolute()),
+            path=file_path_to_use,
             to_archive=to_archive,
             tags=tag_objs,
         )
-        new_file.version = version_obj
+        new_file.version = version
         return new_file
 
     def _build_tags(self, tag_names: List[str]) -> Dict[str, Tag]:
         """Build a list of tag objects.
 
         Take a list of tags, if a tag does not exist create a new tag object.
         Map the tag name to a tag object and return a list of those
```

### Comparing `housekeeper-4.4.0/housekeeper/store/api/handlers/read.py` & `housekeeper-4.5.0/housekeeper/store/api/handlers/read.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/api/handlers/update.py` & `housekeeper-4.5.0/housekeeper/store/api/handlers/update.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/api/schema.py` & `housekeeper-4.5.0/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/archive_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/file_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/filters/version_filters.py` & `housekeeper-4.5.0/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper/store/models.py` & `housekeeper-4.5.0/housekeeper/store/models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.5.0/housekeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.4.0
+Version: 4.5.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.4.0/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.5.0/housekeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/setup.py` & `housekeeper-4.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.4.0",
+    version="4.5.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.4.0/tests/cli/add/conftest.py` & `housekeeper-4.5.0/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.5.0/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.5.0/tests/cli/add/test_cli_add_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Tests foe adding files via CLI"""
 import logging
 from pathlib import Path
 
 from click import Context
 from click.testing import CliRunner
-
 from housekeeper.cli.add import file_cmd
+from housekeeper.store import Store
+from housekeeper.store.models import Bundle, Version
 
 
 def test_add_file_non_existing_bundle(
     base_context: Context,
     cli_runner: CliRunner,
     case_id: str,
     second_sample_vcf: Path,
     caplog,
 ):
     """Test to add a file to a non existing bundle"""
     caplog.set_level(logging.DEBUG)
+
     # GIVEN a context with a empty store and a cli runner
     unknown_bundle_name = case_id
-
     # WHEN trying to add a bundle
     result = cli_runner.invoke(
         file_cmd, [str(second_sample_vcf), "-b", unknown_bundle_name], obj=base_context
     )
 
     # THEN assert it fails
     assert result.exit_code == 1
@@ -79,41 +80,82 @@
 
     # THEN assert it fails since there is no valid input
     assert result.exit_code == 1
     # THEN check that the proper information is displayed
     assert f"File: {non_existing} does not exist" in caplog.text
 
 
-def test_add_file_existing_bundle(
-    populated_context: CliRunner,
+def test_add_file_existing_bundle_with_include(
+    populated_context: Context,
     cli_runner: CliRunner,
     case_id: str,
     second_sample_vcf: Path,
     caplog,
+    housekeeper_version_dir: Path,
+    project_dir: Path,
 ):
     """Test to add a file to a existing bundle"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
     bundle_name = case_id
 
+    store: Store = populated_context["store"]
+    bundle_obj: Bundle = store.bundles().first()
+    version_obj: Version = bundle_obj.versions[0]
+
     # WHEN trying to add the file to a bundle
     result = cli_runner.invoke(
-        file_cmd, [str(second_sample_vcf), "-b", bundle_name], obj=populated_context
+        file_cmd,
+        [str(second_sample_vcf), "-b", bundle_name],
+        obj=populated_context,
     )
 
     # THEN assert it succedes
     assert result.exit_code == 0
     # THEN check that the proper information is displayed
     assert "new file added" in caplog.text
+    # THEN check that the file has been included in the version and that the relative path is given
+    assert Path(housekeeper_version_dir, second_sample_vcf.name).exists()
+    assert Path(housekeeper_version_dir, second_sample_vcf.name).is_file()
+    assert Path(version_obj.files[2].path) == Path(
+        version_obj.relative_root_dir, second_sample_vcf.name
+    )
+
+
+def test_add_file_existing_bundle_without_include(
+    populated_context: Context,
+    cli_runner: CliRunner,
+    case_id: str,
+    second_sample_vcf: Path,
+    caplog,
+    housekeeper_version_dir: Path,
+):
+    """Test to add a file to a existing bundle"""
+    caplog.set_level(logging.DEBUG)
+    # GIVEN a context with a populated store and a cli runner
+    bundle_name = case_id
+
+    # WHEN trying to add the file to a bundle
+    result = cli_runner.invoke(
+        file_cmd,
+        [str(second_sample_vcf), "-b", bundle_name, "-kip"],
+        obj=populated_context,
+    )
+
+    # THEN assert the program exits with success
+    assert result.exit_code == 0
+    # THEN check that the proper information is displayed
+    assert "new file added" in caplog.text
 
 
 def test_add_file_json(
     populated_context: Context,
     cli_runner: CliRunner,
     file_data_json: str,
+    housekeeper_version_dir: Path,
     caplog,
 ):
     """Test to add a file in json format to a non existing bundle"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a populated store and a cli runner
 
     # WHEN trying to add a bundle
```

### Comparing `housekeeper-4.4.0/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.5.0/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.5.0/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/conftest.py` & `housekeeper-4.5.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.5.0/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/get/test_get_bundle.py` & `housekeeper-4.5.0/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/get/test_get_files.py` & `housekeeper-4.5.0/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/get/test_get_tag.py` & `housekeeper-4.5.0/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/get/test_get_version.py` & `housekeeper-4.5.0/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/test_cli_core.py` & `housekeeper-4.5.0/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/cli/test_cli_include.py` & `housekeeper-4.5.0/tests/cli/test_cli_include.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """Tests for include cli command"""
 import logging
 from datetime import datetime
+from pathlib import Path
+
 from click import Context
 from click.testing import CliRunner
-
-from housekeeper.cli.include import include
 from housekeeper.cli.add import bundle_cmd
+from housekeeper.cli.include import include
+from housekeeper.constants import ROOT
 from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle, Version
 
 
-def test_include_files_creates_bundle_dir(
-    populated_context: Context, cli_runner: CliRunner
-):
+def test_include_files_creates_bundle_dir(populated_context: Context, cli_runner: CliRunner):
     """Test to include the files of a version for a bundle_name
 
     The bundle should not exist before and after command is run it should have been created
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert bundle.versions[0].included_at is None
     # GIVEN that no folder has been created since case is not included
-    bundle_path = populated_context["root"] / bundle.name
+    bundle_path = Path(populated_context[ROOT], bundle.name)
     assert not bundle_path.exists()
 
     # WHEN running the include files command
     result = cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
     # THEN assert that the bundle path was created
     assert bundle_path.exists()
@@ -45,16 +45,16 @@
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
-    version_path = (
-        populated_context["root"] / bundle.name / str(version_obj.created_at.date())
+    version_path: Path = Path(
+        populated_context[ROOT], bundle.name, str(version_obj.created_at.date())
     )
     assert not version_path.exists()
 
     # WHEN running the include files command
     cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
     # THEN assert that the version path was created
@@ -72,48 +72,44 @@
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
-    version_path = (
-        populated_context["root"] / bundle.name / str(version_obj.created_at.date())
-    )
+    version_path = populated_context[ROOT] / bundle.name / str(version_obj.created_at.date())
     assert not version_path.exists()
 
     # WHEN running the include files command
     cli_runner.invoke(include, [bundle_name], obj=populated_context)
 
     # THEN assert that files are included in the folder
     files_included = []
     for file_path in version_path.iterdir():
         files_included.append(file_path)
 
     assert files_included
     assert len(files_included) == len(version_obj.files)
 
 
-def test_include_files_specific_version(
-    populated_context: Context, cli_runner: CliRunner
-):
+def test_include_files_specific_version(populated_context: Context, cli_runner: CliRunner):
     """Test to include the files of a version by specifying the version id
 
     The folder should have been created
     """
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     version_id = version_obj.id
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
-    version_path = (
-        populated_context["root"] / bundle.name / str(version_obj.created_at.date())
+    version_path: Path = Path(
+        populated_context[ROOT], bundle.name, str(version_obj.created_at.date())
     )
     assert not version_path.exists()
 
     # WHEN running the include files command
     cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # THEN assert that the folder was created
@@ -124,17 +120,15 @@
     for file_path in version_path.iterdir():
         files_included.append(file_path)
 
     assert files_included
     assert len(files_included) == len(version_obj.files)
 
 
-def test_include_version_no_args(
-    populated_context: Context, cli_runner: CliRunner, caplog
-):
+def test_include_version_no_args(populated_context: Context, cli_runner: CliRunner, caplog):
     """Test to include the files of a version without specifying bundle name or version
 
     The command should exit since it needs to be specified
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
 
@@ -143,32 +137,28 @@
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that arguments are needed
     assert "use bundle name or version-id" in caplog.text
 
 
-def test_include_non_existing_version(
-    populated_context: Context, cli_runner: CliRunner, caplog
-):
+def test_include_non_existing_version(populated_context: Context, cli_runner: CliRunner, caplog):
     """Test to include the files of a version that does not exist
 
     The command should exit since a valid version is needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
     store: Store = populated_context["store"]
     # GIVEN a version that does not exists
     version_id = 10
     assert not store.get_version_by_id(version_id=version_id)
 
     # WHEN running the include files specifying the non existing version
-    result = cli_runner.invoke(
-        include, ["--version-id", version_id], obj=populated_context
-    )
+    result = cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that version did not exist
     assert "version not found" in caplog.text
 
 
@@ -230,20 +220,16 @@
     The command should exit since the version can not be included again
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated and a version that is already included
     store: Store = populated_context["store"]
     version_obj = store._get_query(table=Version).first()
     version_id = version_obj.id
-    result = cli_runner.invoke(
-        include, ["--version-id", version_id], obj=populated_context
-    )
+    result = cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # WHEN trying to include the version again
-    result = cli_runner.invoke(
-        include, ["--version-id", version_id], obj=populated_context
-    )
+    result = cli_runner.invoke(include, ["--version-id", version_id], obj=populated_context)
 
     # THEN assert that the command exists with zero code 1
     assert result.exit_code == 1
     # THEN assert it was communicated that version did not exist
     assert "version included on" in caplog.text
```

### Comparing `housekeeper-4.4.0/tests/conftest.py` & `housekeeper-4.5.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 import shutil
 from copy import deepcopy
 from pathlib import Path
 from typing import List
 
 import pytest
 import yaml
-
 from housekeeper.date import get_date
 from housekeeper.store import Store
 from housekeeper.store.models import Archive, Bundle, Tag, Version
 
 from .helper_functions import Helpers
 
-
 # basic fixtures
 
 
 @pytest.fixture(scope="function", name="helpers")
 def fixture_helpers() -> Helpers:
     """Return a test helper object."""
     return Helpers()
@@ -346,14 +344,22 @@
 def fixture_project_dir(tmpdir_factory) -> Path:
     """Path to a temporary working directory."""
     my_tmpdir = Path(tmpdir_factory.mktemp("workdir"))
     yield my_tmpdir
     shutil.rmtree(str(my_tmpdir))
 
 
+@pytest.fixture(scope="function", name="housekeeper_version_dir")
+def fixture_housekeeper_version_dir(project_dir: Path, case_id: str, timestamp_string: str) -> Path:
+    """Path to a created directory with case and version."""
+    hk_version_tmpdir: Path = Path(project_dir, case_id, timestamp_string)
+    hk_version_tmpdir.mkdir(parents=True)
+    return hk_version_tmpdir
+
+
 @pytest.fixture(scope="function", name="config_dir")
 def fixture_config_dir(tmpdir_factory) -> Path:
     """Path to a temporary directory for config files."""
     my_tmpdir = Path(tmpdir_factory.mktemp("confdir"))
     yield my_tmpdir
     shutil.rmtree(str(my_tmpdir))
```

### Comparing `housekeeper-4.4.0/tests/helper_functions.py` & `housekeeper-4.5.0/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/conftest.py` & `housekeeper-4.5.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_archive_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_archive_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_bundle_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_file_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_tag_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_version_bundle_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/filters/test_version_filters.py` & `housekeeper-4.5.0/tests/store/filters/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/handlers/test_createhandler.py` & `housekeeper-4.5.0/tests/store/handlers/test_createhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Tests for store core functions."""
 from pathlib import Path
 from typing import List
 
 import pytest
-from sqlalchemy.exc import IntegrityError
-
 from housekeeper.store.api import schema
 from housekeeper.store.api.core import Store
-from housekeeper.store.models import Bundle, File, Tag, Version, Archive
+from housekeeper.store.models import Archive, Bundle, File, Tag, Version
+from sqlalchemy.exc import IntegrityError
 
 
 def test_schema_with_invalid_input(bundle_data_json):
     """Tests that errors are thrown when validating incorrect input data."""
     # GIVEN input data with missing name of the bundle
     del bundle_data_json["name"]
     # WHEN validating it against the schema
@@ -160,38 +159,51 @@
     populated_store.session.add(new_archive)
 
     # THEN an SQLAlchemy error should be thrown
     with pytest.raises(IntegrityError):
         populated_store.session.commit()
 
 
-def test_add_file(populated_store: Store, second_family_vcf: Path, family_tag_names: List[str]):
+def test_add_file(
+    populated_store: Store,
+    second_family_vcf: Path,
+    family_tag_names: List[str],
+    housekeeper_version_dir: Path,
+    project_dir: Path,
+):
     """Test to create a file with the add file method."""
     # GIVEN the path and the tags for a file
 
     # GIVEN a store populated with a bundle
     bundle: Bundle = populated_store.bundles().first()
     assert isinstance(bundle, Bundle)
 
     # WHEN using the add file method to create a new file object
     new_file: File = populated_store.add_file(
-        file_path=second_family_vcf, bundle=bundle, tags=family_tag_names
+        file_path=second_family_vcf,
+        bundle=bundle,
+        tags=family_tag_names,
     )
 
     # THEN assert that the file is a file object
     assert isinstance(new_file, File)
     # THEN assert that the file is added to the latest version of the bundle
     assert new_file.version == bundle.versions[0]
     # THEN assert that the tags are added to the new file
     assert len(new_file.tags) == len(family_tag_names)
     for tag_obj in new_file.tags:
         assert isinstance(tag_obj, Tag)
 
 
-def test_add_file_no_tags(populated_store: Store, second_family_vcf: Path):
+def test_add_file_no_tags(
+    populated_store: Store,
+    second_family_vcf: Path,
+    housekeeper_version_dir: Path,
+    project_dir: Path,
+):
     """Test to create a file with the add file method without tags."""
     # GIVEN a path for a file
 
     # GIVEN a store populated with a bundle
     bundle: Bundle = populated_store.bundles().first()
     assert isinstance(bundle, Bundle)
```

### Comparing `housekeeper-4.4.0/tests/store/handlers/test_readhandler.py` & `housekeeper-4.5.0/tests/store/handlers/test_readhandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/handlers/test_updatehandler.py` & `housekeeper-4.5.0/tests/store/handlers/test_updatehandler.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/store/test_models.py` & `housekeeper-4.5.0/tests/store/test_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/test_date.py` & `housekeeper-4.5.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.4.0/tests/test_include.py` & `housekeeper-4.5.0/tests/test_include.py`

 * *Files identical despite different names*


# Comparing `tmp/dataherb-0.1.5.tar.gz` & `tmp/dataherb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataherb-0.1.5.tar", last modified: Thu Aug 12 00:26:05 2021, max compression
+gzip compressed data, was "dataherb-0.1.8.tar", last modified: Mon May 29 14:10:03 2023, max compression
```

## Comparing `dataherb-0.1.5.tar` & `dataherb-0.1.8.tar`

### file list

```diff
@@ -1,58 +1,69 @@
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/
--rwxr-xr-x   0 leima      (501) staff       (20)       54 2021-08-07 09:33:23.000000 dataherb-0.1.5/MANIFEST.in
--rw-r--r--   0 leima      (501) staff       (20)     5245 2021-08-12 00:26:05.000000 dataherb-0.1.5/PKG-INFO
--rw-r--r--   0 leima      (501) staff       (20)     3743 2021-08-05 22:14:16.000000 dataherb-0.1.5/README.md
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/
--rwxr-xr-x   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.5/dataherb/__init__.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/cmd/
--rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.5/dataherb/cmd/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     1534 2021-08-07 14:59:55.000000 dataherb-0.1.5/dataherb/cmd/configs.py
--rw-r--r--   0 leima      (501) staff       (20)     3902 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/cmd/create.py
--rw-r--r--   0 leima      (501) staff       (20)     1303 2021-08-07 14:59:55.000000 dataherb-0.1.5/dataherb/cmd/search.py
--rw-r--r--   0 leima      (501) staff       (20)     2108 2021-08-07 14:59:55.000000 dataherb-0.1.5/dataherb/cmd/sync_git.py
--rw-r--r--   0 leima      (501) staff       (20)      211 2021-08-05 18:06:50.000000 dataherb-0.1.5/dataherb/cmd/sync_s3.py
--rw-r--r--   0 leima      (501) staff       (20)    15598 2021-08-12 00:09:07.000000 dataherb-0.1.5/dataherb/command.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/core/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.5/dataherb/core/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)    11617 2021-08-07 14:59:55.000000 dataherb-0.1.5/dataherb/core/base.py
--rw-r--r--   0 leima      (501) staff       (20)     1594 2021-08-07 13:38:27.000000 dataherb-0.1.5/dataherb/core/search.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/fetch/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.5/dataherb/fetch/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     4464 2021-08-06 20:07:51.000000 dataherb-0.1.5/dataherb/fetch/remote.py
--rw-r--r--   0 leima      (501) staff       (20)     7718 2021-08-11 23:49:04.000000 dataherb-0.1.5/dataherb/flora.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/parse/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.5/dataherb/parse/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)      207 2021-08-06 20:07:51.000000 dataherb-0.1.5/dataherb/parse/csv.py
--rw-r--r--   0 leima      (501) staff       (20)     3482 2021-08-07 14:59:55.000000 dataherb-0.1.5/dataherb/parse/model_json.py
--rw-r--r--   0 leima      (501) staff       (20)    11340 2021-08-06 20:07:51.000000 dataherb-0.1.5/dataherb/parse/model_yaml.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/serve/
--rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.5/dataherb/serve/__init__.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/herbs/
--rw-r--r--   0 leima      (501) staff       (20)      122 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/herbs/index.md
--rw-r--r--   0 leima      (501) staff       (20)      624 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/mkdocs.yml
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/
--rw-r--r--   0 leima      (501) staff       (20)     1309 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/home.html
--rw-r--r--   0 leima      (501) staff       (20)      936 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/main.html
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/partials/
--rw-r--r--   0 leima      (501) staff       (20)     1688 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html
--rw-r--r--   0 leima      (501) staff       (20)     1532 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/partials/metadata.html
--rw-r--r--   0 leima      (501) staff       (20)      704 2021-08-05 20:55:33.000000 dataherb-0.1.5/dataherb/serve/mkdocs_templates.py
--rw-r--r--   0 leima      (501) staff       (20)     1218 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/models.py
--rw-r--r--   0 leima      (501) staff       (20)     5069 2021-08-07 09:33:23.000000 dataherb-0.1.5/dataherb/serve/save_mkdocs.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb/utils/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.5/dataherb/utils/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     1590 2021-08-05 22:14:16.000000 dataherb-0.1.5/dataherb/utils/awscli.py
--rw-r--r--   0 leima      (501) staff       (20)     3247 2021-08-11 23:55:30.000000 dataherb-0.1.5/dataherb/utils/configs.py
--rw-r--r--   0 leima      (501) staff       (20)      821 2021-08-05 18:06:50.000000 dataherb-0.1.5/dataherb/utils/data.py
--rwxr-xr-x   0 leima      (501) staff       (20)       65 2021-08-12 00:25:55.000000 dataherb-0.1.5/dataherb/version.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/
--rw-r--r--   0 leima      (501) staff       (20)     5245 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/PKG-INFO
--rw-r--r--   0 leima      (501) staff       (20)     1248 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/SOURCES.txt
--rw-r--r--   0 leima      (501) staff       (20)        1 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/dependency_links.txt
--rw-r--r--   0 leima      (501) staff       (20)       56 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/entry_points.txt
--rw-r--r--   0 leima      (501) staff       (20)        1 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/not-zip-safe
--rw-r--r--   0 leima      (501) staff       (20)      332 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/requires.txt
--rw-r--r--   0 leima      (501) staff       (20)        9 2021-08-12 00:26:05.000000 dataherb-0.1.5/dataherb.egg-info/top_level.txt
--rw-r--r--   0 leima      (501) staff       (20)       38 2021-08-12 00:26:05.000000 dataherb-0.1.5/setup.cfg
--rwxr-xr-x   0 leima      (501) staff       (20)     1487 2021-08-05 18:06:50.000000 dataherb-0.1.5/setup.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.031005 dataherb-0.1.8/
+-rw-r--r--   0 leima      (501) staff       (20)     1063 2022-05-11 19:32:34.000000 dataherb-0.1.8/LICENSE
+-rwxr-xr-x   0 leima      (501) staff       (20)       55 2022-05-11 19:32:34.000000 dataherb-0.1.8/MANIFEST.in
+-rw-r--r--   0 leima      (501) staff       (20)     4084 2023-05-29 14:10:03.030617 dataherb-0.1.8/PKG-INFO
+-rw-r--r--   0 leima      (501) staff       (20)     3744 2022-05-11 19:32:34.000000 dataherb-0.1.8/README.md
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.990674 dataherb-0.1.8/dataherb/
+-rwxr-xr-x   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.998148 dataherb-0.1.8/dataherb/cmd/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/cmd/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     2061 2022-05-11 20:38:31.000000 dataherb-0.1.8/dataherb/cmd/create.py
+-rw-r--r--   0 leima      (501) staff       (20)     1597 2022-05-12 19:03:51.000000 dataherb-0.1.8/dataherb/cmd/search.py
+-rw-r--r--   0 leima      (501) staff       (20)     3223 2022-05-12 22:48:08.000000 dataherb-0.1.8/dataherb/cmd/sync_git.py
+-rw-r--r--   0 leima      (501) staff       (20)      295 2022-05-12 20:03:04.000000 dataherb-0.1.8/dataherb/cmd/sync_s3.py
+-rw-r--r--   0 leima      (501) staff       (20)    18581 2023-05-28 14:16:32.000000 dataherb-0.1.8/dataherb/command.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.000869 dataherb-0.1.8/dataherb/core/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/core/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     8719 2023-05-29 13:53:16.000000 dataherb-0.1.8/dataherb/core/base.py
+-rw-r--r--   0 leima      (501) staff       (20)     1621 2023-05-29 13:53:12.000000 dataherb-0.1.8/dataherb/core/search.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.002792 dataherb-0.1.8/dataherb/deprecation/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-11 20:30:23.000000 dataherb-0.1.8/dataherb/deprecation/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.006389 dataherb-0.1.8/dataherb/deprecation/cmd/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-11 20:30:20.000000 dataherb-0.1.8/dataherb/deprecation/cmd/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     1587 2022-05-11 20:29:52.000000 dataherb-0.1.8/dataherb/deprecation/cmd/configs.py
+-rw-r--r--   0 leima      (501) staff       (20)     2079 2022-05-11 20:38:31.000000 dataherb-0.1.8/dataherb/deprecation/cmd/create.py
+-rw-r--r--   0 leima      (501) staff       (20)     8475 2022-05-11 20:23:30.000000 dataherb-0.1.8/dataherb/deprecation/command.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.008060 dataherb-0.1.8/dataherb/deprecation/core/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-12 20:32:56.000000 dataherb-0.1.8/dataherb/deprecation/core/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     3673 2022-05-12 22:19:15.000000 dataherb-0.1.8/dataherb/deprecation/core/base.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.010381 dataherb-0.1.8/dataherb/fetch/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/fetch/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     4470 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/fetch/remote.py
+-rw-r--r--   0 leima      (501) staff       (20)     8552 2023-05-29 13:54:24.000000 dataherb-0.1.8/dataherb/flora.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.015461 dataherb-0.1.8/dataherb/parse/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/parse/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)      167 2022-05-12 21:02:37.000000 dataherb-0.1.8/dataherb/parse/csv.py
+-rw-r--r--   0 leima      (501) staff       (20)     2705 2022-05-11 20:17:04.000000 dataherb-0.1.8/dataherb/parse/model_json.py
+-rw-r--r--   0 leima      (501) staff       (20)    11335 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/parse/model_yaml.py
+-rw-r--r--   0 leima      (501) staff       (20)      421 2022-05-11 20:09:44.000000 dataherb-0.1.8/dataherb/parse/utils.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.019726 dataherb-0.1.8/dataherb/serve/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/serve/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.020981 dataherb-0.1.8/dataherb/serve/mkdocs_template/
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.021950 dataherb-0.1.8/dataherb/serve/mkdocs_template/herbs/
+-rw-r--r--   0 leima      (501) staff       (20)      123 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/herbs/index.md
+-rw-r--r--   0 leima      (501) staff       (20)      622 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/mkdocs.yml
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.023949 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/
+-rw-r--r--   0 leima      (501) staff       (20)     1310 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/home.html
+-rw-r--r--   0 leima      (501) staff       (20)      937 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/main.html
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.027024 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/
+-rw-r--r--   0 leima      (501) staff       (20)     1689 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html
+-rw-r--r--   0 leima      (501) staff       (20)     1533 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/metadata.html
+-rw-r--r--   0 leima      (501) staff       (20)      704 2021-08-05 20:55:33.000000 dataherb-0.1.8/dataherb/serve/mkdocs_templates.py
+-rw-r--r--   0 leima      (501) staff       (20)     1266 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/serve/models.py
+-rw-r--r--   0 leima      (501) staff       (20)     5064 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/serve/save_mkdocs.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.029596 dataherb-0.1.8/dataherb/utils/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/utils/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     1591 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/utils/awscli.py
+-rw-r--r--   0 leima      (501) staff       (20)     3145 2023-05-29 13:45:34.000000 dataherb-0.1.8/dataherb/utils/configs.py
+-rw-r--r--   0 leima      (501) staff       (20)      821 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/utils/data.py
+-rwxr-xr-x   0 leima      (501) staff       (20)       65 2022-05-12 21:08:37.000000 dataherb-0.1.8/dataherb/version.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.994529 dataherb-0.1.8/dataherb.egg-info/
+-rw-r--r--   0 leima      (501) staff       (20)     4084 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/PKG-INFO
+-rw-r--r--   0 leima      (501) staff       (20)     1501 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/SOURCES.txt
+-rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/dependency_links.txt
+-rw-r--r--   0 leima      (501) staff       (20)       55 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/entry_points.txt
+-rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-28 14:07:27.000000 dataherb-0.1.8/dataherb.egg-info/not-zip-safe
+-rw-r--r--   0 leima      (501) staff       (20)      351 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/requires.txt
+-rw-r--r--   0 leima      (501) staff       (20)        9 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/top_level.txt
+-rw-r--r--   0 leima      (501) staff       (20)       38 2023-05-29 14:10:03.031163 dataherb-0.1.8/setup.cfg
+-rwxr-xr-x   0 leima      (501) staff       (20)     1410 2022-05-11 19:32:34.000000 dataherb-0.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dataherb-0.1.5/README.md` & `dataherb-0.1.8/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,8 @@
 ## Documentation
 
 The source of the documentation for this package is located at `docs`.
 
 
 ## References and Acknolwedgement
 
-- `dataherb` uses `datapackage` in the core. `datapackage` is a python library for the [data-package standard](https://specs.frictionlessdata.io/data-package/). The core schema of the dataset is essentially the data-package standard.
+- `dataherb` uses `datapackage` in the core. `datapackage` is a python library for the [data-package standard](https://specs.frictionlessdata.io/data-package/). The core schema of the dataset is essentially the data-package standard.
```

### Comparing `dataherb-0.1.5/dataherb/cmd/configs.py` & `dataherb-0.1.8/dataherb/deprecation/cmd/configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from loguru import logger
 import json
 import sys
 from pathlib import Path
 
+from loguru import logger
+
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
 def load_dataherb_config(config_path=None, no_config_error=True):
-    """[Deprecated]
+    """
+
+    [Deprecated] Use `dataherb.utils.configs.Config` instead.
+
     Loads the dataherb config file.
 
     Load the content from the specified file as the config. The config file has to be json.
     """
 
     if config_path is None:
         home = Path.home()
```

### Comparing `dataherb-0.1.5/dataherb/cmd/search.py` & `dataherb-0.1.8/dataherb/cmd/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
+from rich.panel import Panel
 from rich.table import Table
 from rich.tree import Tree
-from rich.panel import Panel
+from dataherb.core.base import Herb
+from typing import Dict
 
 
 class HerbTable:
-    """Format search result
+    """Format a herb object as a table.
+
+    For example, a flora search result can be formatted
+    as a table for the user to read easily.
 
-    A flora search result has the following structure:
-    ```
+    :param herb: an Herb object
     """
 
-    def __init__(self, herb):
+    def __init__(self, herb: Herb):
         self.herb = herb
 
-    def panel(self):
+    def panel(self) -> Dict[str, Panel]:
+        """Create a panel with all the information"""
 
-        self.table()
-        self.resource_tree()
+        return {
+            "table": self.table(),
+            "tree": self.resource_tree(),
+        }
 
-    def table(self):
+    def table(self) -> Panel:
         """Summary Table"""
         table = Table(title=f"DataHerb: {self.herb.name}", show_lines=True)
 
         table.add_column("key", justify="right", style="cyan", no_wrap=False)
         table.add_column("value", style="magenta", no_wrap=False)
 
         table.add_row(f"ID", f"{self.herb.id}")
@@ -32,15 +39,15 @@
         table.add_row(f"URI", f"{self.herb.uri}")
         table.add_row(f"Metadata", f"{self.herb.metadata_uri}")
 
         pl = Panel(table, title=f"Summary of {self.herb.id}")
 
         return pl
 
-    def resource_tree(self):
+    def resource_tree(self) -> Panel:
         """Show list of resources"""
 
         tree = Tree(f"{self.herb.id}")
         for r in self.herb.resources:
             tree.add(f'{r.descriptor.get("path")}')
 
         pl = Panel(tree, title=f"Resources of {self.herb.id}")
```

### Comparing `dataherb-0.1.5/dataherb/command.py` & `dataherb-0.1.8/dataherb/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,62 +7,80 @@
 import git
 import inquirer
 from datapackage import Package
 from loguru import logger
 from mkdocs.commands.serve import serve as _serve
 from rich.console import Console
 
+
+from dataherb.version import __version__
 from dataherb.cmd.create import describe_dataset
 from dataherb.cmd.search import HerbTable
-from dataherb.cmd.sync_git import upload_dataset_to_git
+from dataherb.cmd.sync_git import remote_git_repo, upload_dataset_to_git
 from dataherb.cmd.sync_s3 import upload_dataset_to_s3
 from dataherb.core.base import Herb
+from dataherb.fetch.remote import get_data_from_url
 from dataherb.flora import Flora
-from dataherb.parse.model_json import STATUS_CODE, MetaData
+from dataherb.parse.model_json import MetaData
+from dataherb.parse.utils import STATUS_CODE
 from dataherb.serve.save_mkdocs import SaveMkDocs
 from dataherb.utils.configs import Config
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 console = Console()
 
 
-__CWD__ = os.getcwd()
+__CWD__ = Path(__file__).parent.resolve()
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def dataherb(ctx):
     if ctx.invoked_subcommand is None:
         click.echo("Hello {}".format(os.environ.get("USER", "")))
-        click.echo("Welcome to DataHerb.")
+        click.echo(f"Welcome to DataHerb (version {__version__}).")
     else:
-        # click.echo("Loading Service: %s" % ctx.invoked_subcommand)
-        pass
+        click.echo("Loading Service: %s" % ctx.invoked_subcommand)
+
+
+@dataherb.command()
+def version():
+    """
+    Print out the version of the tool.
+    """
+    click.echo(f"dataherb version {__version__}")
 
 
 @dataherb.command()
 @click.option(
     "--show/--no-show", "-s/ ", default=False, help="Show the current configuration"
 )
 @click.option(
     "--locate/--no-locate",
     "-l/ ",
     default=False,
     help="Locate the folder that contains the configuration",
 )
 def configure(show, locate):
     """
-    Configure dataherb; inspect, or lcoate the current configurations.
+    Configure dataherb; inspect, or locate the current configurations.
+
+    :param show: if flag is given, will show the current configuration instead of starting
+        the configuration process.
+    :param locate: if flag is given, will locate the configuration folder
+        and open in filesystem.
     """
 
     home = Path.home()
     config_path = home / ".dataherb" / "config.json"
 
-    if not show:
+    if locate:
+        click.launch(config_path.parent)
+    elif not show:
         if config_path.exists():
             is_overwite = click.confirm(
                 click.style(
                     f"Config file ({config_path}) already exists. Overwrite?", fg="red"
                 ),
                 default=False,
             )
@@ -94,26 +112,30 @@
 
         answers = inquirer.prompt(questions)
 
         config = {
             "workdir": answers.get("workdir"),
             "default": {
                 "flora": answers.get("default_flora"),
-                "aggregrated": False # if false, we will use folders for each herb.
+                "aggregrated": False,  # if false, we will use folders for each herb.
             },
         }
 
         flora_path_workdir = answers.get("workdir", "")
         if flora_path_workdir.startswith("~"):
             home = Path.home()
             flora_path_workdir = str(home / flora_path_workdir[2:])
 
-        flora_path = Path(flora_path_workdir) / "flora" / f"{answers.get('default_flora')}"
+        flora_path = (
+            Path(flora_path_workdir) / "flora" / f"{answers.get('default_flora')}"
+        )
         if not flora_path.exists():
-            click.secho(f"{flora_path} doesn't exist. Creating {flora_path}...", fg="red")
+            click.secho(
+                f"{flora_path} doesn't exist. Creating {flora_path}...", fg="red"
+            )
             flora_path.mkdir(parents=True)
         else:
             click.secho(f"{flora_path} exists, using the folder directly.", fg="green")
 
         logger.debug(f"config: {config}")
 
         with open(config_path, "w") as f:
@@ -127,39 +149,49 @@
             c = Config()
             click.secho(f"The current config for dataherb is:")
             click.secho(
                 json.dumps(c.config, indent=2, sort_keys=True, ensure_ascii=False)
             )
             click.secho(f"The above config is extracted from {config_path}")
 
-    if locate:
-        click.launch(str(config_path.parent))
-
 
 @dataherb.command()
 @click.option(
     "--flora",
     "-f",
     default=None,
     help="Path to the flora file; Defaults to the default flora in the configuration.",
 )
 @click.option("--id", "-i", required=False, help="The id of the dataset to describe.")
 @click.argument("keywords", required=False)
 @click.option(
     "--full/--summary", default=False, help="Whether to show the full json result"
 )
-def search(flora, id, keywords, full):
+@click.option(
+    "--locate/--no-locate",
+    "-l/ ",
+    default=False,
+    help="Locate the folder that contains the dataset, only works for --id mode",
+)
+def search(flora, id, keywords, full, locate):
     """
     search datasets on DataHerb by keywords or id
+
+    :param flora: the path to the flora file. If not given,
+        will use the default flora in the configuration.
+    :param id: the id of the dataset to find.
+    :param keywords: the keywords to search.
+    :param full: whether to show the full json result.
+    :param locate: if flag is given, will locate the dataset folder.
     """
     if flora is None:
         c = Config()
         flora = c.flora_path
 
-    fl = Flora(flora=flora)
+    fl = Flora(flora_path=flora)
     if not id:
         click.echo("Searching Herbs in DataHerb Flora ...")
         results = fl.search(keywords)
         click.echo(f"Found {len(results)} results")
         if not results:
             click.echo(f"Could not find dataset related to {keywords}")
         else:
@@ -189,14 +221,17 @@
                 console.print(ht.table())
                 console.print(ht.resource_tree())
             else:
                 console.rule(title=f"{result.id}", characters="||")
                 click.secho(f"DataHerb ID: {result.id}")
                 click.echo(json.dumps(result_metadata, indent=2, sort_keys=True))
 
+            if locate:
+                click.launch(str(result.base_path))
+
 
 @dataherb.command()
 @click.option(
     "--flora",
     "-f",
     default=None,
     help="Specify the path to the flora; defaults to default flora in configuration.",
@@ -219,34 +254,40 @@
     "-r",
     default=False,
     required=False,
     help="Whether to recreate the website. Recreation will delete all the current generated pages and rebuild the whole website.",
 )
 def serve(flora, workdir, dev_addr, recreate):
     """
-    create a dataherb server and view the flora in your browser
+    create a dataherb server and view the flora in your browser.
+
+    :param flora: the path to the flora file. If not given,
+        will use the default flora in the configuration.
+    :param workdir: the path to the work directory. If not given,
+        will use the workdir in the configuration.
+    :param dev_addr: the address of the dev server.
+    :param recreate: whether to recreate the website.
     """
 
     if flora is None:
         c = Config()
         flora = c.flora_path
 
     if workdir is None:
         c = Config()
         workdir = c.workdir
 
-    fl = Flora(flora=flora)
-    mk = SaveMkDocs(flora=fl, workdir=workdir)
-    mk.save_all(recreate=recreate)
+    fl = Flora(flora_path=flora)
 
-    mkdocs_config = str(Path(workdir) / "serve" / "mkdocs.yml")
+    mk = SaveMkDocs(flora=fl, workdir=workdir, folder=".serve")
+    mk.save_all(recreate=recreate)
 
     click.echo(f"Open http://{dev_addr}")
     click.launch(f"http://{dev_addr}")
-    _serve(config_file=mkdocs_config, dev_addr=dev_addr)
+    _serve(config_file=str(mk.mkdocs_config), dev_addr=dev_addr)
 
 
 @dataherb.command()
 @click.argument("id", required=True)
 @click.option(
     "--flora",
     "-f",
@@ -257,52 +298,58 @@
     "--workdir",
     "-w",
     default=None,
     help="Specify the path to the work directory; defaults to the workdir in configuration.",
 )
 def download(id, flora, workdir):
     """
-    Download dataset using id
+    Download dataset using id.
+
+    :param id: the id of the dataset to download.
+    :param flora: the path to the flora file. If not given,
+        will use the default flora in the configuration.
+    :param workdir: the path to the work directory. If not given,
+        will use the workdir in the configuration.
     """
 
     if flora is None:
         c = Config()
         flora = c.flora_path
 
     if workdir is None:
         c = Config()
         workdir = c.workdir
 
-    fl = Flora(flora=flora)
+    fl = Flora(flora_path=flora)
     click.echo(f"Fetching Herbs {id} in DataHerb Flora ...")
     result = fl.herb(id)
     if not result:
         click.echo(f"Could not find dataset with id {id}")
     else:
         result_metadata = result.metadata
-        click.echo(f'Downloading DataHerb ID: {result_metadata.get("id")}')
         result_uri = result_metadata.get("uri")
         result_id = result_metadata.get("id")
-        dest_folder = str(Path(workdir) / result_id)
-        if os.path.exists(dest_folder):
+        dest_folder = Path(workdir) / result_id
+        click.echo(
+            f'Downloading DataHerb ID: {result_metadata.get("id")} into {dest_folder}'
+        )
+        if dest_folder.exists():
             click.echo(f"Can not download dataset to {dest_folder}: folder exists.\n")
 
             is_pull = click.confirm(f"Would you like to pull from remote?")
             if is_pull:
                 repo = git.Repo(dest_folder)
                 repo.git.pull()
             else:
                 click.echo(
                     f"Please go to the folder {dest_folder} and sync your repo manually."
                 )
         else:
-            # dest_folder_parent = f"./{result_repository.split('/')[0]}"
-            os.makedirs(dest_folder)
+            dest_folder.mkdir(parents=True, exist_ok=False)
             repo = git.repo.base.Repo.clone_from(result_uri, to_path=dest_folder)
-            # git.Git(dest_folder).clone(result_uri)
 
 
 @dataherb.command()
 @click.confirmation_option(
     prompt=f"Your current working directory is {__CWD__}\n"
     "A dataherb.json file will be created right here.\n"
     "Are you sure this is the correct path?"
@@ -312,30 +359,33 @@
     "-f",
     default=None,
     help="Specify the path to the flora; defaults to default flora in configuration.",
 )
 def create(flora):
     """
     creates metadata for current dataset
+
+    :param flora: the path to the flora file. If not given,
+        will use the default flora in the configuration.
     """
     if flora is None:
         c = Config()
         flora = c.flora_path
 
     use_existing_dpkg = False
 
-    if (Path(__CWD__) / "dataherb.json").exists():
+    if (__CWD__ / "dataherb.json").exists():
         use_existing_dpkg = click.confirm(
             f"A dataherb.json file already exists in {__CWD__}. "
             f"Shall we use the existing dataherb.json?",
             default=True,
             show_default=True,
         )
 
-    fl = Flora(flora=flora)
+    fl = Flora(flora_path=flora)
     md = MetaData(folder=__CWD__)
 
     if use_existing_dpkg:
         logger.debug("Using existing dataherb.json ...")
         md.load()
     else:
         dataset_basics = describe_dataset()
@@ -344,15 +394,15 @@
 
         pkg = Package()
         pkg.infer("**/*.csv")
         pkg_descriptor = {"datapackage": pkg.descriptor}
 
         md.metadata.update(pkg_descriptor)
 
-        if (Path(__CWD__) / "dataherb.json").exists():
+        if (__CWD__ / "dataherb.json").exists():
             is_overwrite = click.confirm(
                 "Replace the current dataherb.json file?", default=False
             )
             if is_overwrite:
                 md.create(overwrite=is_overwrite)
 
                 click.echo(
@@ -388,15 +438,15 @@
     """
     remove herb from flora
     """
     if flora is None:
         c = Config()
         flora = c.flora_path
 
-    fl = Flora(flora=flora)
+    fl = Flora(flora_path=flora)
     herb = fl.herb(herb_id)
     if not herb:
         click.echo(click.style(f"Could not find herb with id {herb_id}", fg="red"))
         click.echo("We did nothing.")
         sys.exit()
 
     to_remove = click.confirm(f"Remove {herb_id} from the flora?", default=False)
@@ -494,10 +544,52 @@
         "The .dataherb folder and metadata.yml file \n"
         f"{__CWD__}\n"
         " has been validated. Please read the summary and fix the errors.",
         bold=True,
     )
 
 
-if __name__ == "__main__":
-    fl = Flora()
-    pass
+@dataherb.command()
+@click.option(
+    "--flora",
+    "-f",
+    default=None,
+    help="Specify the path to the flora; defaults to default flora in configuration.",
+)
+@click.option(
+    "--source",
+    "-s",
+    type=click.Choice(["github"], case_sensitive=False),
+    default="github",
+    help="Source of remote data.",
+)
+@click.argument("uri", required=True)
+def add(flora, source, uri):
+    """
+    add herb to flora from a remote source
+
+    :param flora: path to flora
+    :param source: source of remote data
+    :param uri: uri to the remote dataset metadata file
+    """
+
+    if flora is None:
+        c = Config()
+        flora = c.flora_path
+
+    if not source:
+        raise ValueError("Please specify a supported source.")
+
+    if source == "github":
+        parsed = remote_git_repo(uri)
+        metadata_request = get_data_from_url(parsed["metadata_uri"])
+
+        if not metadata_request.status_code == 200:
+            raise Exception(
+                "Could not download metadata from remote. status code: {}".format(
+                    metadata_request.status_code
+                )
+            )
+        else:
+            metadata = metadata_request.json()
+
+        # TODO: save content to file
```

### Comparing `dataherb-0.1.5/dataherb/core/base.py` & `dataherb-0.1.8/dataherb/core/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 import io
+import sys
 from pathlib import Path
 
 import click
 import pandas as pd
-from dataherb.cmd.configs import load_dataherb_config
-from dataherb.fetch.remote import get_data_from_url as _get_data_from_url
-from dataherb.parse.model_json import MetaData
-from dataherb.utils.data import flatten_dict as _flatten_dict
 from datapackage import Package, Resource
 from loguru import logger
 from rapidfuzz import fuzz
-import sys
+
+from dataherb.utils.configs import Config
+from dataherb.fetch.remote import get_data_from_url
+from dataherb.parse.model_json import MetaData
+from dataherb.utils.data import flatten_dict as _flatten_dict
+from typing import Optional, List, Tuple, Set, Union
+
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
-class Herb(object):
+class Herb:
     """
     Herb is a collection of the dataset.
+
+    :param meta_dict: the dictionary that specifies the herb.
+    :param base_path: the path to the dataset.
+    :param with_resources: whether to load the resources, i.e., data files.
     """
 
-    def __init__(self, meta_dict, base_path=None, with_resources=True):
-        """
-        :param herb_meta_json: the dictionary that specifies the herb
-        :type herb_meta_json: dict
+    def __init__(
+        self, meta_dict: dict, base_path: Optional[Path] = None, with_resources=True
+    ):
+        """
+        :param meta_dict: the dictionary that specifies the herb
+        :type meta_dict: dict
+        :param base_path: the path to the dataset
+        :type base_path: pathlib.Path
+        :param with_resources: whether to load the resources, i.e., data files
+        :type with_resources: bool
         """
         if base_path is None:
-            CONFIG = load_dataherb_config()
-            self.base_path = CONFIG["workdir"]
+            c = Config()
+            self.base_path = c.workdir
         else:
             self.base_path = base_path
         if isinstance(self.base_path, str):
             self.base_path = Path(self.base_path)
 
         self.with_resources = with_resources
 
@@ -47,42 +60,48 @@
                 f"input meta type ({type(meta_dict)}) is not supported.",
                 param=meta_dict,
             )
 
         self._from_meta_dict(self.herb_meta_json)
 
     @property
-    def is_local(self):
+    def is_local(self) -> bool:
         is_local = False
         if self.base_path.exists():
             is_local = True
 
         return is_local
 
-    def _from_meta_dict(self, meta_dict):
+    def _from_meta_dict(self, meta_dict: dict) -> None:
         """Build properties from meta dict"""
         self.name = meta_dict.get("name")
         self.description = meta_dict.get("description")
         self.repository = meta_dict.get("repository")  # Deprecated
-        self.id = meta_dict.get("id")
+        self.id = meta_dict.get("id", "")
 
         self.source = meta_dict.get("source")
-        self.metadata_uri = meta_dict.get("metadata_uri")
+        self.metadata_uri = meta_dict.get("metadata_uri", "")
         self.uri = meta_dict.get("uri")
         self.datapackage = Package(meta_dict.get("datapackage"))
         if not self.datapackage:
             self.update_datapackage()
 
         if self.with_resources:
             self.resources = [
                 self.get_resource(i, source_only=False)
                 for i in range(len(self.datapackage.resources))
             ]
 
-    def get_resource(self, idx=None, path=None, name=None, source_only=True):
+    def get_resource(
+        self,
+        idx: Optional[int] = None,
+        path: Optional[str] = None,
+        name: Optional[str] = None,
+        source_only: bool = True,
+    ) -> Resource:
         if idx is None:
             if path:
                 all_paths = [
                     r.descriptor.get("path") for r in self.datapackage.resources
                 ]
                 if path in all_paths:
                     idx = all_paths.index(path)
@@ -133,25 +152,25 @@
             resource = self.datapackage.resources[idx]
 
         if source_only:
             return resource.source
         else:
             return resource
 
-    def update_datapackage(self):
+    def update_datapackage(self) -> None:
         """
         update_datapackage gets the datapackage metadata from the metadata_uri
         """
 
         if self.source == "git":
-            file_content = _get_data_from_url(self.metadata_uri)
+            file_content = get_data_from_url(self.metadata_uri)
 
             if not file_content.status_code == 200:
                 file_error_msg = "Could not fetch remote file: {}; {}".format(
-                    self.url, file_content.status_code
+                    self.metadata_uri, file_content.status_code
                 )
                 click.ClickException(file_error_msg)
                 # file_content = json.dumps([{"url": self.url, "error": file_error_msg}])
             else:
                 file_content = file_content.json()  # .decode(self.decode)
         elif self.source == "s3":
             raise NotImplementedError(
@@ -162,20 +181,24 @@
 
         self.herb_meta_json["datapackage"] = self.datapackage_meta
 
         self.datapackage = Package(self.datapackage_meta)
 
         return self.datapackage
 
-    def search_score(self, keywords, keys=None):
+    def search_score(
+        self,
+        keywords: Union[List[str], Tuple[str], Set[str]],
+        keys: Optional[List[str]] = None,
+    ) -> float:
         """
         search_score calcualtes the matching score of the herb for any given keyword
 
-        :param key_word: keyword for the search
-        :type key_word: list
+        :param keywords: keywords for the search
+        :type keywords: list
         :param keys: list of keys in the dictionary to look into.
         :type keys: list, optional
         """
 
         if keys is None:
             keys = ["name", "id", "repository", "tags", "description"]
 
@@ -197,15 +220,15 @@
         max_score = 0
         if keywords_scores:
             max_score = max(keywords_scores)
 
         return max_score
 
     @property
-    def metadata(self, keys=None):
+    def metadata(self):
         """
         metadata formats the metadata of the herb
         """
 
         return self.herb_meta_json.copy()
 
     def download(self):
@@ -229,114 +252,7 @@
         authors = ", ".join([author.get("name") for author in authors])
         return (
             f"DataHerb ID: {meta.get('id')}\n"
             f"name: {meta.get('name')}"
             f"description: {meta.get('description')}\n"
             f"contributors: {authors}"
         )
-
-
-class Leaf(object):
-    """
-    Deprecated
-
-    Leaf is a data file of the Herb.
-    """
-
-    def __init__(self, leaf_meta_json, herb):
-        self.leaf_meta_json = leaf_meta_json
-        self.herb = herb
-
-        self.url = "https://raw.githubusercontent.com/{}/master/{}".format(
-            self.herb.repository, self.leaf_meta_json.get("path")
-        )
-        self.format = self.leaf_meta_json.get("format")
-        # decode the file content using decode
-        self.decode = self.leaf_meta_json.get("decode", "utf-8")
-        self.name = self.leaf_meta_json.get("name")
-        self.description = self.leaf_meta_json.get("description")
-        self.path = self.leaf_meta_json.get("path")
-        self.downloaded = {}
-
-    def download(self):
-        """
-        download downloads the data
-        """
-
-        # Fetch data from remote
-        file_content = _get_data_from_url(self.url)
-        if not file_content.status_code == 200:
-            file_error_msg = "Could not fetch remote file: {}; {}".format(
-                self.url, file_content.status_code
-            )
-            click.ClickException(file_error_msg)
-            # file_content = json.dumps([{"url": self.url, "error": file_error_msg}])
-        else:
-            file_content = file_content.content
-
-        if self.format.lower() == "csv":
-            if isinstance(file_content, bytes):
-                file_string_io = io.StringIO(file_content.decode(self.decode))
-            else:
-                file_string_io = file_content
-            # csv files may have comment rows
-            file_comment = self.leaf_meta_json.get("comment")
-            # csv files may have different separators
-            file_separator = self.leaf_meta_json.get("seperator", ",")
-            try:
-                data = pd.read_csv(
-                    file_string_io, comment=file_comment, sep=file_separator
-                )
-            except Exception as e:
-                logger.error(f"Error loading remote file: {self.url}")
-                data = file_string_io
-        elif self.format.lower() == "json":
-            if isinstance(file_content, bytes):
-                file_string_io = io.StringIO(file_content.decode(self.decode))
-            else:
-                file_string_io = file_content
-
-            try:
-                data = pd.read_json(self.url)
-            except Exception as e:
-                logger.error(f"Error loading remote file: {self.url}")
-                data = file_string_io
-        else:
-            logger.error(f"data file format {self.format} is not supported!")
-
-        self.downloaded = {"data": data, "content": file_content}
-
-    @property
-    def data(self):
-        if not self.downloaded:
-            self.download()
-
-        return self.downloaded.get("data")
-
-    @property
-    def content(self):
-        if not self.downloaded:
-            self.download()
-
-        return self.downloaded.get("content")
-
-    def metadata(self, format=None):
-        """
-        metadata formats the metadata of the herb
-        """
-        if format is None:
-            format = "json"
-
-        if format == "json":
-            return self.leaf_meta_json
-        else:
-            logger.error(f"format {format} is not support for metadata!")
-
-    def __str__(self):
-        return """{} from {} with size {}, the remote file is located at {};\n\n{}
-        """.format(
-            self.leaf_meta_json.get("path"),
-            self.herb.id,
-            self.leaf_meta_json.get("size"),
-            self.path,
-            self.metadata(),
-        )
```

### Comparing `dataherb-0.1.5/dataherb/core/search.py` & `dataherb-0.1.8/dataherb/core/search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,60 @@
-def search_by_keywords_in_flora(flora, keywords, keys=None, min_score=50):
+from typing import Sequence, Union, List, Sequence, Optional
+
+from dataherb.core.base import Herb
+
+
+def search_by_keywords_in_flora(
+    flora: List[Herb],
+    keywords: List[str],
+    keys: Optional[List[str]] = None,
+    min_score: float = 50,
+) -> List[dict]:
     """
     search_in_flora calculates the match score of each herb and returns the top 10.
 
     :param flora: list of herbs
-    :type flora: list
     :param keywords: search keywords
-    :type keywords: list
     :param keys: list of dictionary keys to look into
-    :type keys: list, optional
     :param min_score: minimum score of the dataset, default to 50
-    :type min_score: float, optional
-    :return: herbs that matches the requirements
-    :rtype: list
     """
 
-    if not isinstance(keywords, (list, tuple, set)):
+    if not isinstance(keywords, List):
         keywords = [keywords]
 
     herb_scores = []
 
     for herb in flora:
         herb_search_score = {
             "id": herb.id,
             "herb": herb,
             "score": herb.search_score(keywords),
         }
         herb_scores.append(herb_search_score)
 
     ranked_herbs = sorted(herb_scores, key=lambda i: i["score"], reverse=True)
 
-    ranked_herbs = [i for i in ranked_herbs if i.get("score") >= min_score]
+    ranked_herbs = [i for i in ranked_herbs if i.get("score", 0) >= min_score]
 
     return ranked_herbs
 
 
-def search_by_ids_in_flora(flora, ids):
+def search_by_ids_in_flora(flora: List[Herb], ids: Sequence[str]) -> List[dict]:
     """
     search_in_flora finds the herb with the corresponding ids
 
     :param flora: list of herbs
     :type flora: list
     :param ids: ids of the herbs to be located
     :type ids: list
     :return: herbs that matches the id
     :rtype: list
     """
 
-    if not isinstance(ids, (list, tuple, set)):
+    if not isinstance(ids, Sequence):
         ids = [ids]
 
     herbs = []
     for herb in flora:
         if herb.id in ids:
             herb_matched = {"herb": herb, "id": herb.id}
             herbs.append(herb_matched)
```

### Comparing `dataherb-0.1.5/dataherb/fetch/remote.py` & `dataherb-0.1.8/dataherb/fetch/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from loguru import logger
-import os, sys
+import os
 import random
+import sys
 
 import requests
+from loguru import logger
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
```

### Comparing `dataherb-0.1.5/dataherb/flora.py` & `dataherb-0.1.8/dataherb/flora.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,212 @@
 import json
 import shutil
 import sys
+import validators
 from pathlib import Path
+from yarl import URL
 
 from loguru import logger
 
 from dataherb.core.base import Herb
-from dataherb.core.search import \
-    search_by_ids_in_flora as _search_by_ids_in_flora
-from dataherb.core.search import \
-    search_by_keywords_in_flora as _search_by_keywords_in_flora
-from dataherb.fetch.remote import get_data_from_url as _get_data_from_url
+from dataherb.core.search import search_by_ids_in_flora as _search_by_ids_in_flora
+from dataherb.core.search import search_by_keywords_in_flora
+from dataherb.fetch.remote import get_data_from_url
 from dataherb.parse.model_json import MetaData
+from typing import List, Union, Optional
+from dataherb.core.base import Herb
+
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
-class Flora(object):
+class Flora:
     """
-    DataHerb is the container of datasets.
+    A container of datasets. It loads a local folder of dataset metadata and
+    forms a list of dataset objects.
+
+    The provided local path or remote resource will then be converted to a list
+    of dataherb objects.
+
+    :param flora: path to the flora database. Either an URL or a local path.
+    :param is_aggregated: if True, the flora is aggregated into one json file.
     """
 
-    def __init__(self, flora, is_aggregated=False):
-        """
-        :param flora: API of the DataHerb service, defaults to dataherb official or list of Herbs, defaults to everything from the API
-        """
+    def __init__(self, flora_path: Union[Path, URL], is_aggregated: bool = False):
         self.is_aggregated = is_aggregated
 
-        if isinstance(flora, str):
-            if flora.endswith(".json"):
+        if not isinstance(flora_path, (Path, URL)):
+            raise Exception(f"flora must be a path or a url. ({flora_path})")
+
+        if isinstance(flora_path, URL):
+            self.flora = self._get_remote_flora(flora_path)
+
+        if isinstance(flora_path, Path):
+            if flora_path.suffix == ".json":
                 self.is_aggregated = True
-            self.workdir = Path(flora).parent.parent
-            self.flora_config = flora
-            flora = self._get_flora(flora)
-        else:
-            raise Exception(f"flora must be a json file or a url. ({flora})")
+            self.workdir = flora_path.parent.parent
+            self.flora_path = flora_path
+            self.flora = self._get_local_flora(flora_path)
+
+        if is_aggregated != self.is_aggregated:
+            logger.warning(
+                f"flora has is_aggregated={self.is_aggregated}, "
+                "but was specified as is_aggregated={is_aggregated}."
+            )
 
         logger.debug(f"flora workdir {self.workdir}")
 
-        self.flora = flora
-
-    def _get_flora(self, flora_config):
+    def _get_local_flora(self, flora_config: Path) -> List[Herb]:
         """
-        _get_flora fetch flora from the provided API.
+        _get_local_flora fetch flora from the local folder or file.
+
+        There are two scenarios:
+
+        - The flora is one aggregated local json file.
+        - The flora is a folder that contains folders of dataset ids.
         """
-        if Path(flora_config).exists():
-            if self.is_aggregated:
-                with open(flora_config, "r") as f:
-                    flora = json.load(f)
-            else:
-                # We do not have aggregated flora
-                # read dataherb.json from all the folders here
-                flora_folder = Path(flora_config)
-                herb_paths = [f for f in flora_folder.iterdir() if f.is_dir()]
-                flora = [
-                    json.load(open(f.joinpath("dataherb.json"), "r"))
-                    for f in herb_paths
-                ]
+        if self.is_aggregated:
+            with open(flora_config, "r") as f:
+                json_flora = json.load(f)
         else:
-            # assuming the config is a url if the local file does not exist
-            flora_request = _get_data_from_url(flora_config)
+            flora_folder = Path(flora_config)
+            herb_paths = [f for f in flora_folder.iterdir() if f.is_dir()]
+            json_flora = [
+                json.load(open(f.joinpath("dataherb.json"), "r")) for f in herb_paths
+            ]
 
-            if not flora_request.status_code == 200:
-                raise Exception(
-                    "Could not download dataherb flora from remote. status code: {}".format(
-                        flora_request.status_code
-                    )
+        return [
+            Herb(herb, base_path=self.workdir / f'{herb.get("id", "")}')
+            for herb in json_flora
+        ]
+
+    def _get_remote_flora(self, flora_config: URL) -> List[Herb]:
+        """
+        _get_remote_flora fetch flora from the remote API.
+
+        !!! warning
+            Currently, this mode only works for aggregated json flora.
+        """
+        flora_request = get_data_from_url(flora_config)
+
+        if not flora_request.status_code == 200:
+            raise Exception(
+                "Could not download dataherb flora from remote. status code: {}".format(
+                    flora_request.status_code
                 )
-            else:
-                flora = flora_request.json()
+            )
+        else:
+            json_flora = flora_request.json()
 
-        # Convert herbs to objects
-        flora = [
+        return [
             Herb(herb, base_path=self.workdir / f'{herb.get("id", "")}')
-            for herb in flora
+            for herb in json_flora
         ]
 
-        return flora
-
-    def add(self, herb):
+    def add(self, herb: Union[Herb, dict, MetaData]) -> None:
         """
-        add add a herb to the flora
+        Add a herb to the flora.
         """
+
+        herb = self._convert_to_herb(herb)
+
+        logger.debug(f"adding herb with metadata: {herb.metadata}")
+
+        for h_exist in self.flora:
+            if herb.id == h_exist.id:
+                raise Exception(f"herb id = {herb.id} already exists")
+
+        self.flora.append(herb)
+        if self.is_aggregated:
+            self.save(path=self.flora_path)
+        else:
+            self.save(herb=herb)
+
+    def _convert_to_herb(self, herb: Union[Herb, dict, MetaData]) -> Herb:
         if isinstance(herb, MetaData):
             herb = Herb(herb.metadata)
         elif isinstance(herb, dict):
             herb = Herb(herb)
         elif isinstance(herb, Herb):
             pass
         else:
             raise Exception(f"Input herb type ({type(herb)}) is not supported.")
 
-        logger.debug(f"metadata: {herb.metadata}")
-
-        for id in [i.id for i in self.flora]:
-            if id == herb.id:
-                raise Exception(f"herb id = {herb.id} already exists")
-
-        self.flora.append(herb)
-        if self.is_aggregated:
-            self.save()
-        else:
-            self.save(herb=herb)
+        return herb
 
-    def remove(self, herb_id):
+    def remove(self, herb_id: str) -> None:
         """
-        add add a herb to the flora
+        Removes a herb from the flora.
         """
         for id in [i.id for i in self.flora]:
             if id == herb_id:
                 logger.debug(f"found herb id = {herb_id}")
 
         self.flora = [h for h in self.flora if h.id != herb_id]
 
         if self.is_aggregated:
-            self.save()
+            self.save(path=self.flora_path)
         else:
             self.remove_herb_from_flora(herb_id)
 
-    def save(self, path=None, id=None, herb=None):
+    def save(
+        self,
+        path: Optional[Path] = None,
+        id: Optional[str] = None,
+        herb: Optional[Herb] = None,
+    ) -> None:
         """save flora metadata to json file"""
 
         if path is None:
-            path = self.flora_config
-
-        if isinstance(path, str):
-            path = Path(path)
+            path = self.flora_path
 
         logger.debug(
             f"type of a herb in flora: {type(self.flora[0])}\n{self.flora[0].metadata}"
         )
 
         if self.is_aggregated:
             serialized_flora = []
             for h in self.flora:
                 logger.debug(f"herb (type {type(h)}): {h}")
                 serialized_flora.append(h.metadata)
 
             with open(path, "w") as fp:
                 json.dump(
-                    serialized_flora, fp, sort_keys=True, indent=4, separators=(",", ": ")
+                    serialized_flora,
+                    fp,
+                    sort_keys=True,
+                    indent=4,
+                    separators=(",", ": "),
                 )
         else:
             if (not id) and (not herb):
                 raise Exception("dataherb id must be provided")
             elif herb:
                 logger.debug(f"Saving herb using herb object")
-                self.save_herb_meta(herb.id, path / f"{herb.id}")
+                self.save_herb_meta(id=herb.id, path=path / f"{herb.id}")
             elif id:
                 logger.debug(f"Saving herb using herb id")
                 self.save_herb_meta(id, path / f"{id}")
 
-
-    def save_herb_meta(self, id, path=None):
+    def save_herb_meta(self, id: str, path: Optional[Path] = None) -> None:
         """Save a herb metadata to json file"""
         if path is None:
             path = self.workdir / f"{id}"
 
         if not path.exists():
             path.mkdir(parents=True)
 
         logger.debug(f"Will replace dataherb id {id}")
         with open(path / "dataherb.json", "w") as fp:
             json.dump(
-                self.herb_meta(id), fp,
-                sort_keys=True, indent=4, separators=(",", ": ")
+                self.herb_meta(id), fp, sort_keys=True, indent=4, separators=(",", ": ")
             )
 
-    def remove_herb_from_flora(self, id, path=None):
+    def remove_herb_from_flora(self, id: str, path: Optional[Path] = None) -> None:
         """Remove a herb metadata to json file"""
         if path is None:
             path = self.workdir / f"{id}"
 
         if not path.exists():
             logger.debug(f"dataherb {id} doesn't exist")
             return
@@ -180,86 +214,58 @@
             try:
                 shutil.rmtree(path)
             except OSError as e:
                 logger.error(
                     f"Can not remove herb id {id}: {e.filename} - {e.strerror}."
                 )
 
-    def search(self, keywords):
+    def search(self, keywords: Union[str, List[str]]) -> List[dict]:
         """
         search finds the datasets that matches the keywords
 
-        :param keywords: [description]
-        :type keywords: [type]
-        :return: [description]
-        :rtype: [type]
+        :param keywords: keywords to be searched
         """
         if isinstance(keywords, str):
             keywords = [keywords]
 
-        return _search_by_keywords_in_flora(self.flora, keywords)
+        return search_by_keywords_in_flora(flora=self.flora, keywords=keywords)
 
-    def herb_meta(self, id):
+    def herb_meta(self, id: str) -> Optional[dict]:
         """
         herb loads the dataset
 
         :param id: herb id of the dataset
-        :type id: str
         """
 
         herbs = _search_by_ids_in_flora(self.flora, id)
 
         if herbs:
-            herb = herbs[0]
-
-            herb = herb.get("herb")
-
-            return herb.metadata
+            herb = herbs[0].get("herb")
+            if herb:
+                return herb.metadata
+            else:
+                return None
         else:
-            return
+            return None
 
-    def herb(self, id):
+    def herb(self, id: str) -> Optional[Herb]:
         """
         herb loads the dataset as dataframes.
 
         :param id: herb id
-        :type id: str
         """
 
         herbs = _search_by_ids_in_flora(self.flora, id)
         if len(herbs) > 1:
             logger.error(
                 f"Found multiple datasets with id {id}, please fix this in your flora data json file, e.g, WORKDIRECTORY/flora/flora.json."
             )
 
         if herbs:
-            herb = herbs[0]
-            herb = herb.get("herb")
-            return herb
+            herb = herbs[0].get("herb")
+            if herb:
+                return herb
+            else:
+                return None
         else:
             logger.error(f"Could not find herb {id}")
-            return
-
-
-if __name__ == "__main__":
-
-    from datapackage import Resource
-
-    fl = Flora(flora="/Users/leima/dataherb/flora/flora.json")
-
-    hb = fl.herb("git-data-science-job")
-
-    print(f"herb base_path: {hb.base_path}")
-
-    rs = hb.resources[0]
-
-    rs_1 = Resource(rs.descriptor, base_path=str(hb.base_path))
-
-    print(f"{rs.tabular}")
-
-    # rs_2.read()
-
-    rs.read()
-
-    print(hb.get_resource(path="dataset/stackoverflow_job_listing.csv"))
-
-    logger.debug("End of Game")
+            return None
```

### Comparing `dataherb-0.1.5/dataherb/parse/model_yaml.py` & `dataherb-0.1.8/dataherb/parse/model_yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import csv
-import os, sys
+import os
+import sys
 from collections import OrderedDict
 from pathlib import Path
 
 import ruamel.yaml
 from loguru import logger
 from ruamel.yaml.representer import RoundTripRepresenter
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 IGNORED_FOLDERS_AND_FILES = [".git", ".dataherb", ".vscode"]
 
+
 # Add representer to ruamel.yaml for OrderedDict
 class MyRepresenter(RoundTripRepresenter):
     pass
 
 
 ruamel.yaml.add_representer(
     OrderedDict, MyRepresenter.represent_dict, representer=MyRepresenter
@@ -35,30 +37,29 @@
     "UNKNOWN": "unknown",
     "SUCCESS": "success",
     "WARNING": "warning",
     "ERROR": "error",
 }
 
 
-class MetaData(object):
+class MetaData:
     def __init__(self):
         self.dataherb_folder = ".dataherb"
         self.metadata_file = "metadata.yml"
         self.template = OrderedDict(
             {
                 "name": "",
                 "description": "",
                 "contributors": [{"name": "", "github": ""}],
                 "data": [],
                 "references": [{"name": "", "link": ""}],
             }
         )
 
     def parse_structure(self, folder=None):
-
         if folder is None:
             folder = "."
 
         tree_f = []
         tree_d = []
         for root, dirs, files in os.walk(folder):
             for d in dirs:
@@ -83,15 +84,14 @@
         fields = []
         for col in columns:
             fields.append({"name": col, "description": ""})
 
         return fields
 
     def _generate_leaf(self, path, meta_input):
-
         name = meta_input.get("name", "")
         description = meta_input.get("description", "")
         updated_at = meta_input.get("updated_at", "")
 
         file_format = path.split(".")[-1]
         if len(file_format) >= 10:
             logger.error(f"The format of file {path} could not be determined!")
@@ -113,28 +113,26 @@
             "updated_at": updated_at,
             "fields": fields,
         }
 
         return res
 
     def append_leaf(self, dataset_file, meta_input):
-
         existing_leaves = self.template["data"]
         existing_leaves.append(self._generate_leaf(dataset_file, meta_input))
         self.template.update(data=existing_leaves)
 
     def _parse_leaves(self, loaded_meta):
         """_parse_leaf loads the leaves from the metadata."""
 
         existing_leaves = loaded_meta["data"]
 
         return existing_leaves
 
     def create(self):
-
         # create .dataherb folder
         dataherb_folder = self.dataherb_folder
         try:
             os.mkdir(dataherb_folder)
             logger.info("Created ", dataherb_folder)
         except FileExistsError:
             logger.info(
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_template/mkdocs.yml` & `dataherb-0.1.8/dataherb/serve/mkdocs_template/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,7 @@
 markdown_extensions:
   - meta
   - admonition
 
 plugins:
   - search
   - macros
-
-
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/home.html` & `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/home.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
             </a>
           </div>
         </div>
       </div>
     </section>
   {% endblock %}
   {% block content %}asdasfdasfasfas{% endblock %}
-  {% block footer %}{% endblock %}
+  {% block footer %}{% endblock %}
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/main.html` & `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/main.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 {% if page and page.meta %}
 {% if page.meta.git_revision_date_localized or
         page.meta.revision_date
   %}
 {% include "partials/source-file.html" %}
 {% endif %}
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html` & `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
                 {% endfor %}
             </tbody>
         </table>
     </div>
 </div>
 {% endif %}
 
-{% endfor %}
+{% endfor %}
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_template/overrides/partials/metadata.html` & `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/metadata.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
                     <td>
                         {{ page.meta.tags }}
                     </td>
                 </tr>
             </tbody>
         </table>
     </div>
-</div>
+</div>
```

### Comparing `dataherb-0.1.5/dataherb/serve/mkdocs_templates.py` & `dataherb-0.1.8/dataherb/serve/mkdocs_templates.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.5/dataherb/serve/models.py` & `dataherb-0.1.8/dataherb/serve/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-from abc import abstractclassmethod
 import sys
+from abc import abstractclassmethod, abstractmethod
+from typing import List
+
 from loguru import logger
+
 from dataherb.flora import Flora
 
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
 class SourceModel:
     """
     Model is the base class for
     """
 
     def __init__(self, path_to_datasets: str) -> None:
         self.path_to_datasets = path_to_datasets
-        self.metas = []
+        self.metas: List[dict] = []
 
     @abstractclassmethod
     def fetch_metadata(self):
         raise NotImplementedError(f"Please implement this method")
 
 
 class SaveModel:
     """
     SaveModel take the models and save them as files to serve as the database.
     """
 
     def __init__(self, flora, workdir, **kargs) -> None:
-
         if isinstance(flora, str):
             flora = Flora(flora)
 
         self.flora = flora
         self.workdir = workdir
         self.kargs = kargs
 
-    @abstractclassmethod
+    @abstractmethod
     def save_json(self) -> None:
         raise NotImplementedError("Please implement save_json method")
 
-    @abstractclassmethod
+    @abstractmethod
     def save_markdown(self) -> None:
         raise NotImplementedError("Please implement save_markdown method")
 
-    @abstractclassmethod
-    def save_all(self) -> None:
+    @abstractmethod
+    def save_all(self, recreate) -> None:
         raise NotImplementedError("Please implement save_all method")
```

### Comparing `dataherb-0.1.5/dataherb/serve/save_mkdocs.py` & `dataherb-0.1.8/dataherb/serve/save_mkdocs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import json
-from distutils.dir_util import copy_tree
-import os, sys
-import click
-from pathlib import Path
+import os
+import sys
 import time
-import yaml
-
-from dataherb.serve.models import SaveModel
-from dataherb.serve.mkdocs_templates import site_config as _site_config
-from dataherb.serve.mkdocs_templates import index_template as _index_template
+from pathlib import Path
 
+import click
+import yaml
+from distutils.dir_util import copy_tree
 from loguru import logger
 from slugify import slugify
 
+from dataherb.serve.mkdocs_templates import index_template as _index_template
+from dataherb.serve.mkdocs_templates import site_config as _site_config
+from dataherb.serve.models import SaveModel
+
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
 class SaveMkDocs(SaveModel):
     """
     SaveMkDocs saves the dataset files from source as MkDocs files
     """
 
-    def __init__(self, flora, workdir):
-
+    def __init__(self, flora, workdir, folder):
         super().__init__(flora, workdir)
+        if folder is None:
+            folder = ".serve"
+        self.folder = folder
+        self.mkdocs_folder = Path(self.workdir) / self.folder
+        self.mkdocs_config = self.mkdocs_folder / "mkdocs.yml"
 
     @staticmethod
     def _generate_markdown_list_meta(dic_lists, name) -> str:
         """
         _markdown_metadata_entry
         """
 
@@ -97,45 +102,39 @@
             fp.write(metadata_mkdocs)
 
         logger.info(f"Saved {herb_metadata} to {path}")
 
     def create_mkdocs_theme(self):
         """copies the prepared theme to the serve dir"""
 
-        mkdocs_folder = Path(self.workdir) / "serve"
-
         mkdocs_template_path = Path(__file__).parent / "mkdocs_template"
 
-        copy_tree(str(mkdocs_template_path), str(mkdocs_folder))
+        copy_tree(str(mkdocs_template_path), str(self.mkdocs_folder))
 
     def create_mkdocs_yaml(self):
         """creates mkdocs.yaml from mkdocs_templates.py"""
 
-        mkdocs_folder = Path(self.workdir) / "serve"
-        mkdocs_yaml_path = mkdocs_folder / "mkdocs.yml"
-
-        with open(mkdocs_yaml_path, "w") as fp:
+        with open(self.mkdocs_config, "w") as fp:
             fp.write(_site_config)
 
     def create_mkdocs_index(self):
         """creates herbs/index.md from mkdocs_templates.py"""
 
-        mkdocs_folder = Path(self.workdir) / "serve"
-        mkdocs_index_path = mkdocs_folder / "herbs" / "index.md"
+        mkdocs_index_path = self.mkdocs_folder / "herbs" / "index.md"
 
         with open(mkdocs_index_path, "w") as fp:
             fp.write(_index_template)
 
     def save_all(self, recreate=False) -> None:
         """
         save_all saves all files necessary
         """
 
         # attach working directory to all paths
-        md_folder = Path(self.workdir) / "serve" / "herbs"
+        md_folder = self.mkdocs_folder / "herbs"
 
         # create folders if necessary
         if md_folder.exists():
             if not recreate:
                 is_remove = click.confirm(
                     f"{md_folder} exists, remove it and create new?",
                     default=True,
@@ -154,17 +153,16 @@
                 md_folder.mkdir(parents=True)
         else:
             md_folder.mkdir(parents=True)
 
         for herb in self.flora.flora:
             herb_id = slugify(herb.id)
 
-            herb_md_path = os.path.join(md_folder, f"{herb_id}.md")
+            herb_md_path = md_folder / f"{herb_id}.md"
             # generate markdown files
             self.save_one_markdown(herb, herb_md_path)
 
         self.create_mkdocs_theme()
 
 
 if __name__ == "__main__":
-
     pass
```

### Comparing `dataherb-0.1.5/dataherb/utils/awscli.py` & `dataherb-0.1.8/dataherb/utils/awscli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 import click
 
 try:
     from awscli.clidriver import create_clidriver
 except ImportError as e:
     click.echo(f"Please install awscli and config awscli first.")
```

### Comparing `dataherb-0.1.5/dataherb/utils/configs.py` & `dataherb-0.1.8/dataherb/utils/configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from loguru import logger
 import json
 import sys
 from pathlib import Path
 
+from loguru import logger
+from typing import cast, Optional
+
 logger.remove()
 logger.add(sys.stderr, level="INFO", enqueue=True)
 
 
 class Config:
     """Config system for Dataherb"""
 
-    def __init__(self, is_aggregated=None, config_path=None, no_config_error=False):
-
-        if is_aggregated is None:
-            is_aggregated = False
-
+    def __init__(
+        self,
+        is_aggregated: bool = False,
+        config_path: Optional[Path] = None,
+        no_config_error: bool = False,
+    ):
         self.is_aggregated = is_aggregated
 
         self.config_path = config_path
         self.no_config_error = no_config_error
         if self.config_path is None:
             home = Path.home()
             self.config_path = home / ".dataherb/config.json"
@@ -28,47 +31,46 @@
                 logger.error(
                     f"Config file {self.config_path} does not exist.\n"
                     f"If this is the first time you use dataherb, please run `dataherb configure` to config dataherb."
                 )
 
         # self.config = self.get_config(no_config_error=self.no_config_error)
 
-    def _flora_path(self, flora, workdir=None):
+    def _flora_path(self, flora, workdir: Optional[str] = None) -> Path:
         """Get the full path to the specified flora"""
 
         if workdir is None:
             workdir = self.config["WD"]
 
         if self.is_aggregated:
             which_flora_path = Path(workdir) / "flora" / Path(flora + ".json")
         else:
             which_flora_path = Path(workdir) / "flora" / Path(flora)
         logger.debug(f"Using flora path: {which_flora_path}")
         if not which_flora_path.exists():
             raise Exception(f"flora config {which_flora_path} does not exist")
 
-        return str(which_flora_path)
+        return which_flora_path
 
     @property
     def config(self):
         """Loads the dataherb config file.
 
         Load the content from the specified file as the config. The config file has to be json.
         """
         return self._config()
 
-    def _config(self, config_path=None):
+    def _config(self) -> dict:
         """Loads the dataherb config file."""
 
-        if config_path is None:
-            config_path = self.config_path
+        config_path = cast(Path, self.config_path)
 
         logger.debug(f"Using {config_path} as config file for dataherb")
         try:
-            with open(config_path, "r") as f:
+            with config_path.open(mode="r") as f:
                 conf = json.load(f)
 
             if not conf.get("workdir"):
                 logger.error(
                     f"Please specify working directory in the config file using the key workdir"
                 )
             elif conf.get("workdir", "").startswith("~"):
@@ -92,16 +94,7 @@
         return self._flora_path(
             self.config.get("default", {}).get("flora"), self.config["workdir"]
         )
 
     @property
     def flora(self):
         return self.config.get("default", {}).get("flora")
-
-
-if __name__ == "__main__":
-    c = Config()
-
-    print(c.config)
-    print(c.flora_path)
-    print(c.workdir)
-    print(c.flora)
```

### Comparing `dataherb-0.1.5/dataherb/utils/data.py` & `dataherb-0.1.8/dataherb/utils/data.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.5/dataherb.egg-info/SOURCES.txt` & `dataherb-0.1.8/dataherb.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 dataherb/__init__.py
 dataherb/command.py
 dataherb/flora.py
 dataherb/version.py
@@ -9,28 +10,35 @@
 dataherb.egg-info/SOURCES.txt
 dataherb.egg-info/dependency_links.txt
 dataherb.egg-info/entry_points.txt
 dataherb.egg-info/not-zip-safe
 dataherb.egg-info/requires.txt
 dataherb.egg-info/top_level.txt
 dataherb/cmd/__init__.py
-dataherb/cmd/configs.py
 dataherb/cmd/create.py
 dataherb/cmd/search.py
 dataherb/cmd/sync_git.py
 dataherb/cmd/sync_s3.py
 dataherb/core/__init__.py
 dataherb/core/base.py
 dataherb/core/search.py
+dataherb/deprecation/__init__.py
+dataherb/deprecation/command.py
+dataherb/deprecation/cmd/__init__.py
+dataherb/deprecation/cmd/configs.py
+dataherb/deprecation/cmd/create.py
+dataherb/deprecation/core/__init__.py
+dataherb/deprecation/core/base.py
 dataherb/fetch/__init__.py
 dataherb/fetch/remote.py
 dataherb/parse/__init__.py
 dataherb/parse/csv.py
 dataherb/parse/model_json.py
 dataherb/parse/model_yaml.py
+dataherb/parse/utils.py
 dataherb/serve/__init__.py
 dataherb/serve/mkdocs_templates.py
 dataherb/serve/models.py
 dataherb/serve/save_mkdocs.py
 dataherb/serve/mkdocs_template/mkdocs.yml
 dataherb/serve/mkdocs_template/herbs/index.md
 dataherb/serve/mkdocs_template/overrides/home.html
```

### Comparing `dataherb-0.1.5/setup.py` & `dataherb-0.1.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from os import path
-from setuptools import setup as _setup
+
 from setuptools import find_packages as _find_packages
+from setuptools import setup as _setup
+
 from dataherb.version import __version__
 
 # read the contents of your README file
 __CWD__ = path.abspath(path.dirname(__file__))
 with open(path.join(__CWD__, "README.md"), encoding="utf-8") as fp:
     PACKAGE_LONG_DESCRIPTION = fp.read()
 
@@ -29,15 +31,14 @@
         url=PACKAGE_URL,
         author="Lei Ma",
         author_email="hi@leima.is",
         license="MIT",
         packages=_find_packages(exclude=("tests",)),
         install_requires=_requirements(),
         include_package_data=True,
-        extras_require={"docs": ["sphinx>=2.4.1", "sphinx-rtd-theme>=0.4.3"]},
         entry_points={"console_scripts": ["dataherb=dataherb.command:dataherb"]},
         test_suite="nose.collector",
         tests_require=["nose"],
         zip_safe=False,
     )
```


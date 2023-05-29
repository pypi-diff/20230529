# Comparing `tmp/dataherb-0.1.8.tar.gz` & `tmp/dataherb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataherb-0.1.8.tar", last modified: Mon May 29 14:10:03 2023, max compression
+gzip compressed data, was "dist/dataherb-0.1.9.tar", last modified: Mon May 29 14:16:21 2023, max compression
```

## Comparing `dataherb-0.1.8.tar` & `dataherb-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.031005 dataherb-0.1.8/
--rw-r--r--   0 leima      (501) staff       (20)     1063 2022-05-11 19:32:34.000000 dataherb-0.1.8/LICENSE
--rwxr-xr-x   0 leima      (501) staff       (20)       55 2022-05-11 19:32:34.000000 dataherb-0.1.8/MANIFEST.in
--rw-r--r--   0 leima      (501) staff       (20)     4084 2023-05-29 14:10:03.030617 dataherb-0.1.8/PKG-INFO
--rw-r--r--   0 leima      (501) staff       (20)     3744 2022-05-11 19:32:34.000000 dataherb-0.1.8/README.md
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.990674 dataherb-0.1.8/dataherb/
--rwxr-xr-x   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/__init__.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.998148 dataherb-0.1.8/dataherb/cmd/
--rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/cmd/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     2061 2022-05-11 20:38:31.000000 dataherb-0.1.8/dataherb/cmd/create.py
--rw-r--r--   0 leima      (501) staff       (20)     1597 2022-05-12 19:03:51.000000 dataherb-0.1.8/dataherb/cmd/search.py
--rw-r--r--   0 leima      (501) staff       (20)     3223 2022-05-12 22:48:08.000000 dataherb-0.1.8/dataherb/cmd/sync_git.py
--rw-r--r--   0 leima      (501) staff       (20)      295 2022-05-12 20:03:04.000000 dataherb-0.1.8/dataherb/cmd/sync_s3.py
--rw-r--r--   0 leima      (501) staff       (20)    18581 2023-05-28 14:16:32.000000 dataherb-0.1.8/dataherb/command.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.000869 dataherb-0.1.8/dataherb/core/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/core/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     8719 2023-05-29 13:53:16.000000 dataherb-0.1.8/dataherb/core/base.py
--rw-r--r--   0 leima      (501) staff       (20)     1621 2023-05-29 13:53:12.000000 dataherb-0.1.8/dataherb/core/search.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.002792 dataherb-0.1.8/dataherb/deprecation/
--rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-11 20:30:23.000000 dataherb-0.1.8/dataherb/deprecation/__init__.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.006389 dataherb-0.1.8/dataherb/deprecation/cmd/
--rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-11 20:30:20.000000 dataherb-0.1.8/dataherb/deprecation/cmd/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     1587 2022-05-11 20:29:52.000000 dataherb-0.1.8/dataherb/deprecation/cmd/configs.py
--rw-r--r--   0 leima      (501) staff       (20)     2079 2022-05-11 20:38:31.000000 dataherb-0.1.8/dataherb/deprecation/cmd/create.py
--rw-r--r--   0 leima      (501) staff       (20)     8475 2022-05-11 20:23:30.000000 dataherb-0.1.8/dataherb/deprecation/command.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.008060 dataherb-0.1.8/dataherb/deprecation/core/
--rw-r--r--   0 leima      (501) staff       (20)        0 2022-05-12 20:32:56.000000 dataherb-0.1.8/dataherb/deprecation/core/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     3673 2022-05-12 22:19:15.000000 dataherb-0.1.8/dataherb/deprecation/core/base.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.010381 dataherb-0.1.8/dataherb/fetch/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/fetch/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     4470 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/fetch/remote.py
--rw-r--r--   0 leima      (501) staff       (20)     8552 2023-05-29 13:54:24.000000 dataherb-0.1.8/dataherb/flora.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.015461 dataherb-0.1.8/dataherb/parse/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/parse/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)      167 2022-05-12 21:02:37.000000 dataherb-0.1.8/dataherb/parse/csv.py
--rw-r--r--   0 leima      (501) staff       (20)     2705 2022-05-11 20:17:04.000000 dataherb-0.1.8/dataherb/parse/model_json.py
--rw-r--r--   0 leima      (501) staff       (20)    11335 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/parse/model_yaml.py
--rw-r--r--   0 leima      (501) staff       (20)      421 2022-05-11 20:09:44.000000 dataherb-0.1.8/dataherb/parse/utils.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.019726 dataherb-0.1.8/dataherb/serve/
--rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/serve/__init__.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.020981 dataherb-0.1.8/dataherb/serve/mkdocs_template/
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.021950 dataherb-0.1.8/dataherb/serve/mkdocs_template/herbs/
--rw-r--r--   0 leima      (501) staff       (20)      123 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/herbs/index.md
--rw-r--r--   0 leima      (501) staff       (20)      622 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/mkdocs.yml
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.023949 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/
--rw-r--r--   0 leima      (501) staff       (20)     1310 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/home.html
--rw-r--r--   0 leima      (501) staff       (20)      937 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/main.html
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.027024 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/
--rw-r--r--   0 leima      (501) staff       (20)     1689 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html
--rw-r--r--   0 leima      (501) staff       (20)     1533 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/metadata.html
--rw-r--r--   0 leima      (501) staff       (20)      704 2021-08-05 20:55:33.000000 dataherb-0.1.8/dataherb/serve/mkdocs_templates.py
--rw-r--r--   0 leima      (501) staff       (20)     1266 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/serve/models.py
--rw-r--r--   0 leima      (501) staff       (20)     5064 2023-05-29 13:43:13.000000 dataherb-0.1.8/dataherb/serve/save_mkdocs.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:03.029596 dataherb-0.1.8/dataherb/utils/
--rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.8/dataherb/utils/__init__.py
--rw-r--r--   0 leima      (501) staff       (20)     1591 2022-05-11 19:32:34.000000 dataherb-0.1.8/dataherb/utils/awscli.py
--rw-r--r--   0 leima      (501) staff       (20)     3145 2023-05-29 13:45:34.000000 dataherb-0.1.8/dataherb/utils/configs.py
--rw-r--r--   0 leima      (501) staff       (20)      821 2021-08-05 18:06:50.000000 dataherb-0.1.8/dataherb/utils/data.py
--rwxr-xr-x   0 leima      (501) staff       (20)       65 2022-05-12 21:08:37.000000 dataherb-0.1.8/dataherb/version.py
-drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:10:02.994529 dataherb-0.1.8/dataherb.egg-info/
--rw-r--r--   0 leima      (501) staff       (20)     4084 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/PKG-INFO
--rw-r--r--   0 leima      (501) staff       (20)     1501 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/SOURCES.txt
--rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/dependency_links.txt
--rw-r--r--   0 leima      (501) staff       (20)       55 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/entry_points.txt
--rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-28 14:07:27.000000 dataherb-0.1.8/dataherb.egg-info/not-zip-safe
--rw-r--r--   0 leima      (501) staff       (20)      351 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/requires.txt
--rw-r--r--   0 leima      (501) staff       (20)        9 2023-05-29 14:10:02.000000 dataherb-0.1.8/dataherb.egg-info/top_level.txt
--rw-r--r--   0 leima      (501) staff       (20)       38 2023-05-29 14:10:03.031163 dataherb-0.1.8/setup.cfg
--rwxr-xr-x   0 leima      (501) staff       (20)     1410 2022-05-11 19:32:34.000000 dataherb-0.1.8/setup.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/
+-rw-r--r--   0 leima      (501) staff       (20)     1063 2023-05-29 14:14:29.000000 dataherb-0.1.9/LICENSE
+-rwxr-xr-x   0 leima      (501) staff       (20)       55 2023-05-29 14:14:29.000000 dataherb-0.1.9/MANIFEST.in
+-rw-r--r--   0 leima      (501) staff       (20)     5233 2023-05-29 14:16:21.000000 dataherb-0.1.9/PKG-INFO
+-rw-r--r--   0 leima      (501) staff       (20)     3744 2023-05-29 14:14:29.000000 dataherb-0.1.9/README.md
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/
+-rwxr-xr-x   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.9/dataherb/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/cmd/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.9/dataherb/cmd/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     2061 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/cmd/create.py
+-rw-r--r--   0 leima      (501) staff       (20)     1597 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/cmd/search.py
+-rw-r--r--   0 leima      (501) staff       (20)     3223 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/cmd/sync_git.py
+-rw-r--r--   0 leima      (501) staff       (20)      295 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/cmd/sync_s3.py
+-rw-r--r--   0 leima      (501) staff       (20)    18581 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/command.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/core/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.9/dataherb/core/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     8719 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/core/base.py
+-rw-r--r--   0 leima      (501) staff       (20)     1621 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/core/search.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/deprecation/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/deprecation/cmd/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/cmd/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     1587 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/cmd/configs.py
+-rw-r--r--   0 leima      (501) staff       (20)     2079 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/cmd/create.py
+-rw-r--r--   0 leima      (501) staff       (20)     8475 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/command.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/deprecation/core/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/core/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     3673 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/deprecation/core/base.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/fetch/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.9/dataherb/fetch/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     4470 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/fetch/remote.py
+-rw-r--r--   0 leima      (501) staff       (20)     8552 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/flora.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/parse/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.9/dataherb/parse/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)      167 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/parse/csv.py
+-rw-r--r--   0 leima      (501) staff       (20)     2705 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/parse/model_json.py
+-rw-r--r--   0 leima      (501) staff       (20)    11335 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/parse/model_yaml.py
+-rw-r--r--   0 leima      (501) staff       (20)      421 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/parse/utils.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/serve/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2021-08-05 18:06:50.000000 dataherb-0.1.9/dataherb/serve/__init__.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/herbs/
+-rw-r--r--   0 leima      (501) staff       (20)      123 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/herbs/index.md
+-rw-r--r--   0 leima      (501) staff       (20)      622 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/mkdocs.yml
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/
+-rw-r--r--   0 leima      (501) staff       (20)     1310 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/home.html
+-rw-r--r--   0 leima      (501) staff       (20)      937 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/main.html
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/partials/
+-rw-r--r--   0 leima      (501) staff       (20)     1689 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html
+-rw-r--r--   0 leima      (501) staff       (20)     1533 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/partials/metadata.html
+-rw-r--r--   0 leima      (501) staff       (20)      704 2021-08-05 20:55:33.000000 dataherb-0.1.9/dataherb/serve/mkdocs_templates.py
+-rw-r--r--   0 leima      (501) staff       (20)     1266 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/models.py
+-rw-r--r--   0 leima      (501) staff       (20)     5064 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/serve/save_mkdocs.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb/utils/
+-rw-r--r--   0 leima      (501) staff       (20)        0 2020-09-25 20:14:36.000000 dataherb-0.1.9/dataherb/utils/__init__.py
+-rw-r--r--   0 leima      (501) staff       (20)     1591 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/utils/awscli.py
+-rw-r--r--   0 leima      (501) staff       (20)     3145 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/utils/configs.py
+-rw-r--r--   0 leima      (501) staff       (20)      821 2021-08-05 18:06:50.000000 dataherb-0.1.9/dataherb/utils/data.py
+-rwxr-xr-x   0 leima      (501) staff       (20)       65 2023-05-29 14:14:29.000000 dataherb-0.1.9/dataherb/version.py
+drwxr-xr-x   0 leima      (501) staff       (20)        0 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/
+-rw-r--r--   0 leima      (501) staff       (20)     5233 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/PKG-INFO
+-rw-r--r--   0 leima      (501) staff       (20)     1501 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/SOURCES.txt
+-rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/dependency_links.txt
+-rw-r--r--   0 leima      (501) staff       (20)       56 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/entry_points.txt
+-rw-r--r--   0 leima      (501) staff       (20)        1 2023-05-28 14:07:27.000000 dataherb-0.1.9/dataherb.egg-info/not-zip-safe
+-rw-r--r--   0 leima      (501) staff       (20)      351 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/requires.txt
+-rw-r--r--   0 leima      (501) staff       (20)        9 2023-05-29 14:16:21.000000 dataherb-0.1.9/dataherb.egg-info/top_level.txt
+-rw-r--r--   0 leima      (501) staff       (20)       38 2023-05-29 14:16:21.000000 dataherb-0.1.9/setup.cfg
+-rwxr-xr-x   0 leima      (501) staff       (20)     1410 2023-05-29 14:14:29.000000 dataherb-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dataherb-0.1.8/LICENSE` & `dataherb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/PKG-INFO` & `dataherb-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: dataherb
-Version: 0.1.8
-Summary: Get clean datasets from DataHerb to boost your data science and data analysis projects
-Home-page: https://github.com/DataHerb/dataherb-python
-Author: Lei Ma
-Author-email: hi@leima.is
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
   <br>
   <a href="https://dataherb.github.io"><img src="https://raw.githubusercontent.com/DataHerb/dataherb.github.io/master/assets/favicon/ms-icon-310x310.png" alt="Markdownify" width="200"></a>
   <br>
   The Python Package for DataHerb
   <br>
 </h1>
@@ -151,9 +139,7 @@
 
 The source of the documentation for this package is located at `docs`.
 
 
 ## References and Acknolwedgement
 
 - `dataherb` uses `datapackage` in the core. `datapackage` is a python library for the [data-package standard](https://specs.frictionlessdata.io/data-package/). The core schema of the dataset is essentially the data-package standard.
-
-
```

#### html2text {}

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1 Name: dataherb Version: 0.1.8 Summary: Get clean datasets
-from DataHerb to boost your data science and data analysis projects Home-page:
-https://github.com/DataHerb/dataherb-python Author: Lei Ma Author-email:
-hi@leima.is License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown License-File: LICENSE
                                     ******
                                 [Markdownify]
                        The Python Package for DataHerb
                                      ******
          *** A DataHerb Core Service to Create and Load Datasets. ***
 ## Install ``` pip install dataherb ``` Documentation: [dataherb.github.io/
 dataherb-python](https://dataherb.github.io/dataherb-python) ## The DataHerb
```

### Comparing `dataherb-0.1.8/dataherb/cmd/create.py` & `dataherb-0.1.9/dataherb/cmd/create.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/cmd/search.py` & `dataherb-0.1.9/dataherb/cmd/search.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/cmd/sync_git.py` & `dataherb-0.1.9/dataherb/cmd/sync_git.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/command.py` & `dataherb-0.1.9/dataherb/command.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/core/base.py` & `dataherb-0.1.9/dataherb/core/base.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/core/search.py` & `dataherb-0.1.9/dataherb/core/search.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/deprecation/cmd/configs.py` & `dataherb-0.1.9/dataherb/deprecation/cmd/configs.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/deprecation/cmd/create.py` & `dataherb-0.1.9/dataherb/deprecation/cmd/create.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/deprecation/command.py` & `dataherb-0.1.9/dataherb/deprecation/command.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/deprecation/core/base.py` & `dataherb-0.1.9/dataherb/deprecation/core/base.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/fetch/remote.py` & `dataherb-0.1.9/dataherb/fetch/remote.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/flora.py` & `dataherb-0.1.9/dataherb/flora.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/parse/model_json.py` & `dataherb-0.1.9/dataherb/parse/model_json.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/parse/model_yaml.py` & `dataherb-0.1.9/dataherb/parse/model_yaml.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_template/mkdocs.yml` & `dataherb-0.1.9/dataherb/serve/mkdocs_template/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/home.html` & `dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/home.html`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/main.html` & `dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/main.html`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html` & `dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/partials/datapackage.html`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_template/overrides/partials/metadata.html` & `dataherb-0.1.9/dataherb/serve/mkdocs_template/overrides/partials/metadata.html`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/mkdocs_templates.py` & `dataherb-0.1.9/dataherb/serve/mkdocs_templates.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/models.py` & `dataherb-0.1.9/dataherb/serve/models.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/serve/save_mkdocs.py` & `dataherb-0.1.9/dataherb/serve/save_mkdocs.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/utils/awscli.py` & `dataherb-0.1.9/dataherb/utils/awscli.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/utils/configs.py` & `dataherb-0.1.9/dataherb/utils/configs.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb/utils/data.py` & `dataherb-0.1.9/dataherb/utils/data.py`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/dataherb.egg-info/SOURCES.txt` & `dataherb-0.1.9/dataherb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataherb-0.1.8/setup.py` & `dataherb-0.1.9/setup.py`

 * *Files identical despite different names*


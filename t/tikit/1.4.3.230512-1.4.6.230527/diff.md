# Comparing `tmp/tikit-1.4.3.230512.tar.gz` & `tmp/tikit-1.4.6.230527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tikit-1.4.3.230512.tar", last modified: Mon May 15 07:26:37 2023, max compression
+gzip compressed data, was "tikit-1.4.6.230527.tar", last modified: Mon May 29 03:25:25 2023, max compression
```

## Comparing `tikit-1.4.3.230512.tar` & `tikit-1.4.6.230527.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/
--rw-r--r--   0 kaihuang   (501) staff       (20)       71 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/MANIFEST.in
--rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/PKG-INFO
--rw-r--r--   0 kaihuang   (501) staff       (20)      499 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/README.md
--rw-r--r--   0 kaihuang   (501) staff       (20)      413 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/requirements.txt
--rw-r--r--   0 kaihuang   (501) staff       (20)       38 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/setup.cfg
--rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 03:33:34.000000 tikit-1.4.3.230512/setup.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/
--rw-r--r--   0 kaihuang   (501) staff       (20)      185 2023-01-05 02:27:12.000000 tikit-1.4.3.230512/tikit/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     7896 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/cli.py
--rw-r--r--   0 kaihuang   (501) staff       (20)   195907 2023-05-15 04:30:12.000000 tikit-1.4.3.230512/tikit/client.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     3976 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/default_client.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/display_optimize/
--rw-r--r--   0 kaihuang   (501) staff       (20)      133 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     3820 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/dataset.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     1628 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/resource_group.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     3951 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/training_model.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     4973 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/display_optimize/training_task.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     1779 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/hdfs.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    35661 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/hive.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    19526 2023-05-05 11:53:57.000000 tikit-1.4.3.230512/tikit/models.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/templates/
--rw-r--r--   0 kaihuang   (501) staff       (20)     7622 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/templates/service_config.yaml
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/
--rw-r--r--   0 kaihuang   (501) staff       (20)      630 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    16473 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     2337 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     2002 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    12338 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/
--rw-r--r--   0 kaihuang   (501) staff       (20)      741 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)      760 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     5071 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     1657 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     1857 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     1574 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     6015 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     3465 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    33848 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    12419 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 kaihuang   (501) staff       (20)   747496 2023-05-05 11:53:57.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 kaihuang   (501) staff       (20)   260703 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 kaihuang   (501) staff       (20)        0 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 kaihuang   (501) staff       (20)      819 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 kaihuang   (501) staff       (20)    19834 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 kaihuang   (501) staff       (20)     4802 2022-12-16 08:10:47.000000 tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 kaihuang   (501) staff       (20)      893 2023-04-17 06:40:50.000000 tikit-1.4.3.230512/tikit/util.py
-drwxr-xr-x   0 kaihuang   (501) staff       (20)        0 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/
--rw-r--r--   0 kaihuang   (501) staff       (20)      858 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/PKG-INFO
--rw-r--r--   0 kaihuang   (501) staff       (20)     1883 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 kaihuang   (501) staff       (20)        1 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 kaihuang   (501) staff       (20)       41 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/entry_points.txt
--rw-r--r--   0 kaihuang   (501) staff       (20)      413 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/requires.txt
--rw-r--r--   0 kaihuang   (501) staff       (20)        6 2023-05-15 07:26:37.000000 tikit-1.4.3.230512/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.792013 tikit-1.4.6.230527/
+-rw-r--r--   0 liuliu     (501) staff       (20)       71 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/MANIFEST.in
+-rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-29 03:25:25.791171 tikit-1.4.6.230527/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)      499 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/README.md
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/requirements.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       38 2023-05-29 03:25:25.792302 tikit-1.4.6.230527/setup.cfg
+-rw-r--r--   0 liuliu     (501) staff       (20)      858 2023-05-29 03:23:07.000000 tikit-1.4.6.230527/setup.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.752086 tikit-1.4.6.230527/tikit/
+-rw-r--r--   0 liuliu     (501) staff       (20)      185 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     7896 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/cli.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   196654 2023-05-29 03:23:07.000000 tikit-1.4.6.230527/tikit/client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3976 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/default_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.760276 tikit-1.4.6.230527/tikit/display_optimize/
+-rw-r--r--   0 liuliu     (501) staff       (20)      133 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/display_optimize/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3820 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/display_optimize/dataset.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1628 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/display_optimize/resource_group.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3951 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/display_optimize/training_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4973 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/display_optimize/training_task.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1779 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/hdfs.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    35661 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/hive.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    20234 2023-05-29 03:23:07.000000 tikit-1.4.6.230527/tikit/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.761024 tikit-1.4.6.230527/tikit/templates/
+-rw-r--r--   0 liuliu     (501) staff       (20)     7622 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/templates/service_config.yaml
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.762030 tikit-1.4.6.230527/tikit/tencentcloud/
+-rw-r--r--   0 liuliu     (501) staff       (20)      630 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.767253 tikit-1.4.6.230527/tikit/tencentcloud/common/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    16473 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2337 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2002 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/common_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12338 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/credential.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.768988 tikit-1.4.6.230527/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 liuliu     (501) staff       (20)      741 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      760 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.770048 tikit-1.4.6.230527/tikit/tencentcloud/common/http/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     5071 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/http/request.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.771783 tikit-1.4.6.230527/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1657 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1857 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1574 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.772778 tikit-1.4.6.230527/tikit/tencentcloud/emr/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.775331 tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     6015 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3465 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    33848 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.776954 tikit-1.4.6.230527/tikit/tencentcloud/tione/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.783861 tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12419 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   748604 2023-05-29 03:23:07.000000 tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   260703 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.786633 tikit-1.4.6.230527/tikit/tencentcloud/wedata/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.790223 tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      819 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    19834 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4802 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      893 2023-04-06 06:58:27.000000 tikit-1.4.6.230527/tikit/util.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2023-05-29 03:25:25.756433 tikit-1.4.6.230527/tikit.egg-info/
+-rw-r--r--   0 liuliu     (501) staff       (20)      700 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)     1883 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        1 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       40 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/requires.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        6 2023-05-29 03:25:25.000000 tikit-1.4.6.230527/tikit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tikit-1.4.3.230512/PKG-INFO` & `tikit-1.4.6.230527/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.3.230512
+Version: 1.4.6.230527
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-Description: TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
-        Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
-        
-        # 发布
-        '''bash
-        # 公网
-        make publish
-        '''
-        
-        # 开发
-        '''bash
-        yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
-        pip install -r requirements.txt
-        '''
-        # 公网
-        pip install tikit -U -i https://pypi.org/simple
-        '''
-Platform: UNKNOWN
+
+TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
+Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
+
+# 发布
+'''bash
+# 公网
+make publish
+'''
+
+# 开发
+'''bash
+yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
+pip install -r requirements.txt
+'''
+# 公网
+pip install tikit -U -i https://pypi.org/simple
+'''
```

### Comparing `tikit-1.4.3.230512/setup.py` & `tikit-1.4.6.230527/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.4.3.230512',
+    version='1.4.6.230527',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.4.3.230512/tikit/cli.py` & `tikit-1.4.6.230527/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/client.py` & `tikit-1.4.6.230527/tikit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -840,14 +840,21 @@
             if input_data_config.DataSource == "GooseFS":
                 data_config = models.DataConfig()
                 data_config.DataSourceType = input_data_config.DataSource
                 data_config.MappingPath = input_data_config.TargetPath
                 data_config.GooseFSSource = models.GooseFSSource()
                 data_config.GooseFSSource.Id = input_data_config.GooseFSId
                 data_configs.append(data_config)
+            if input_data_config.DataSource == "CFSTurbo":
+                data_config = models.DataConfig()
+                data_config.DataSourceType = input_data_config.DataSource
+                data_config.MappingPath = input_data_config.TargetPath
+                data_config.CFSTurboSource = models.CFSTurboSource()
+                data_config.CFSTurboSource.Id = input_data_config.CFSTurboId
+                data_configs.append(data_config)
             return data_configs, input_data_config.DataSource
 
         for input_data_item in input_data_config:
             data_config = models.DataConfig()
             data_config.DataSourceType = input_data_item.DataSource
             data_config.MappingPath = input_data_item.TargetPath
             if input_data_item.DataSource == "COS":
@@ -869,15 +876,19 @@
                 data_config.WeDataHDFSSource.Path = input_data_item.HdfsPath
             elif input_data_item.DataSource == "AIMarket_Algo_PreModel":
                 data_config.AIMarketAlgoPreModelSource = models.AIMarketAlgoPreModelSource()
                 data_config.AIMarketAlgoPreModelSource.Id = input_data_item.AIMarketAlgoId
             elif input_data_item.DataSource == "GooseFS":
                 data_config.GooseFSSource = models.GooseFSSource()
                 data_config.GooseFSSource.Id = input_data_item.GooseFSId
-
+            elif input_data_item.DataSource == "CFSTurbo":
+                data_config.CFSTurboSource = models.CFSTurboSource()
+                data_config.CFSTurboSource.Id = input_data_item.CFSTurboId
+                data_config.CFSTurboSource.Path = input_data_item.CFSTurboPath
+                
             data_configs.append(data_config)
             data_type = input_data_item.DataSource
             if data_type == "AIMarket_Algo_PreModel":
                 data_type = "COS"
         return data_configs, data_type
 
     def stop_training_task(self, task_id):
```

### Comparing `tikit-1.4.3.230512/tikit/default_client.py` & `tikit-1.4.6.230527/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/display_optimize/dataset.py` & `tikit-1.4.6.230527/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/display_optimize/resource_group.py` & `tikit-1.4.6.230527/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/display_optimize/training_model.py` & `tikit-1.4.6.230527/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/display_optimize/training_task.py` & `tikit-1.4.6.230527/tikit/display_optimize/training_task.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/hdfs.py` & `tikit-1.4.6.230527/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/hive.py` & `tikit-1.4.6.230527/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/models.py` & `tikit-1.4.6.230527/tikit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,16 @@
         self.CfsId = None
         self.CfsPath = None
         self.HdfsId = None
         self.HdfsPath = None
         self.WedataId = None
         self.AIMarketAlgoId = None
         self.GooseFSId = None
+        self.CFSTurboId = None
+        self.CFSTurboPath = None
 
     @staticmethod
     def new_mount_cos(cos_str, target_path):
         """一个cos类型的训练数据
 
         :param cos_str:      cos存储，格式： <bucket>/<cos path>/
         :type cos_str: str
@@ -386,15 +388,34 @@
         :rtype:
         """
         ret = TrainingDataConfig()
         ret.TargetPath = target_path
         ret.DataSource = "GooseFS"
         ret.GooseFSId = goosefs_id
         return ret
+    
+    @staticmethod
+    def new_mount_cfs_turbofs(cfs_turbofs_id, source_path, target_path):
+        """新建一个goosefs类型的训练数据集配置
 
+        :param cfs_turbofs_id: cfs_turbofs实例id
+        :type cfs_turbofs_id: str
+        :param  source_path: CFS的路径
+        :type source_path: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = TrainingDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "CFSTurbo"
+        ret.CFSTurboId = cfs_turbofs_id
+        ret.CFSTurboPath= source_path
+        return ret
 
 class ReasoningEnvironment:
     def __init__(self, source, image_key=None, image_type=None, image_url=None, registry_region=None, registry_id=None):
         self.Source = source
         self.ImageKey = image_key
         self.ImageType = image_type
         self.ImageUrl = image_url
```

### Comparing `tikit-1.4.3.230512/tikit/templates/service_config.yaml` & `tikit-1.4.6.230527/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/__init__.py` & `tikit-1.4.6.230527/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/common_client.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/credential.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/http/request.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/common/sign.py` & `tikit-1.4.6.230527/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.4.6.230527/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3700,24 +3700,28 @@
         :type WeDataHDFSSource: :class:`tencentcloud.tione.v20211111.models.WeDataHDFSConfig`
         :param AIMarketAlgoPreModelSource: 来自AIMarket 算法的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type AIMarketAlgoPreModelSource: :class:`tencentcloud.tione.v20211111.models.AIMarketAlgoPreModelSource`
         :param GooseFSSource: 来自GooseFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type GooseFSSource: :class:`tencentcloud.tione.v20211111.models.GooseFSSource`
+        :param CFSTurboSource: 来自CFSTurbo的数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CFSTurboSource: :class:`tencentcloud.tione.v20211111.models.CFSTurboSource`
         """
         self.MappingPath = None
         self.DataSourceType = None
         self.DataSetSource = None
         self.COSSource = None
         self.CFSSource = None
         self.HDFSSource = None
         self.WeDataHDFSSource = None
         self.AIMarketAlgoPreModelSource = None
         self.GooseFSSource = None
+        self.CFSTurboSource = None
 
 
     def _deserialize(self, params):
         self.MappingPath = params.get("MappingPath")
         self.DataSourceType = params.get("DataSourceType")
         if params.get("DataSetSource") is not None:
             self.DataSetSource = DataSetConfig()
@@ -3736,14 +3740,17 @@
             self.WeDataHDFSSource._deserialize(params.get("WeDataHDFSSource"))
         if params.get("AIMarketAlgoPreModelSource") is not None:
             self.AIMarketAlgoPreModelSource = AIMarketAlgoPreModelSource()
             self.AIMarketAlgoPreModelSource._deserialize(params.get("AIMarketAlgoPreModelSource"))
         if params.get("GooseFSSource") is not None:
             self.GooseFSSource = GooseFSSource()
             self.GooseFSSource._deserialize(params.get("GooseFSSource"))
+        if params.get("CFSTurboSource") is not None:
+            self.CFSTurboSource = CFSTurboSource()
+            self.CFSTurboSource._deserialize(params.get("CFSTurboSource"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -21131,14 +21138,39 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
+class CFSTurboSource(AbstractModel):
+    """CFSTurbo的配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: CFSTurbo实例ID
+        :type Id: string
+        :param Path: string CFSTurbo路径
+        :type Path: str
+        """
+        self.Id = None
+        self.Path = None
+
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.Path = params.get("Path")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
 class WeightEntry(AbstractModel):
     """服务版本的权重
 
     """
 
     def __init__(self):
```

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.4.6.230527/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.4.6.230527/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit/util.py` & `tikit-1.4.6.230527/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.4.3.230512/tikit.egg-info/PKG-INFO` & `tikit-1.4.6.230527/tikit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: tikit
-Version: 1.4.3.230512
+Version: 1.4.6.230527
 Summary: Kit for TI PLATFORM
 Home-page: https://cloud.tencent.com/
 Author: TI PLATFORM TEAM
 Author-email: TI_Platform@tencent.com
 License: MIT
-Description: TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
-        Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
-        
-        # 发布
-        '''bash
-        # 公网
-        make publish
-        '''
-        
-        # 开发
-        '''bash
-        yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
-        pip install -r requirements.txt
-        '''
-        # 公网
-        pip install tikit -U -i https://pypi.org/simple
-        '''
-Platform: UNKNOWN
+
+TiKit是一套对接腾讯云TI平台各模块的python SDK工具。 
+Tikit的核心作用是为了让算法类研发人员在使用Notebook功能时，能够更好地进行交互，打通Notebook和本地环境访问平台的路径，进行从训练到推理的闭环。
+
+# 发布
+'''bash
+# 公网
+make publish
+'''
+
+# 开发
+'''bash
+yum install -y cyrus-sasl cyrus-sasl-devel cyrus-sasl-lib krb5-devel
+pip install -r requirements.txt
+'''
+# 公网
+pip install tikit -U -i https://pypi.org/simple
+'''
```

### Comparing `tikit-1.4.3.230512/tikit.egg-info/SOURCES.txt` & `tikit-1.4.6.230527/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*


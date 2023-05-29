# Comparing `tmp/nsj_rest_lib-0.2.0.tar.gz` & `tmp/nsj_rest_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-0.2.0.tar", last modified: Thu May 25 14:19:51 2023, max compression
+gzip compressed data, was "nsj_rest_lib-0.2.1.tar", last modified: Mon May 29 16:56:00 2023, max compression
```

## Comparing `nsj_rest_lib-0.2.0.tar` & `nsj_rest_lib-0.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.988175 nsj_rest_lib-0.2.0/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-05-25 14:19:50.992175 nsj_rest_lib-0.2.0/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      130 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/README.md
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/pyproject.toml
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      888 2023-05-25 14:19:50.992175 nsj_rest_lib-0.2.0/setup.cfg
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.852174 nsj_rest_lib-0.2.0/src/
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.888174 nsj_rest_lib-0.2.0/src/nsj_rest_lib/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.940175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       75 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3131 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      944 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3700 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4349 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3742 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4152 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4664 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.944175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    16639 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1223 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.944175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3987 2023-02-01 14:54:52.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.968175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     8870 2023-03-30 14:16:13.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7563 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5408 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      195 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2295 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.968175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7290 2023-04-17 15:08:09.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.976175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      772 2023-04-17 15:08:09.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      322 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      483 2022-12-09 11:46:59.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2856 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      825 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.976175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    23200 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      582 2023-03-30 14:16:13.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.988175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4196 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      527 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.904174 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1609 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      113 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       13 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2022-09-08 22:15:46.000000 nsj_rest_lib-0.2.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-01-06 22:06:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3131 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3700 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4349 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3684 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4094 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    16639 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2022-12-19 18:04:42.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-03-20 12:54:19.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9033 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-01-02 23:27:01.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      195 2022-12-27 22:14:24.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.335509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      772 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2022-12-27 22:14:24.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2022-11-30 20:09:08.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-01-05 22:38:04.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2022-12-19 17:39:11.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    23200 2023-05-29 16:55:39.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      582 2023-04-18 17:42:31.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.339509 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2022-11-30 19:49:52.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-05-29 16:56:00.331509 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1609 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-05-29 16:56:00.000000 nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-0.2.0/PKG-INFO` & `nsj_rest_lib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.2.0/setup.cfg` & `nsj_rest_lib-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 0.2.0
+version = 0.2.1
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         """
         Tratando requisições HTTP Post para inserir uma instância de uma entidade.
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os dados do corpo da rquisição
-                data = request.get_data(as_text=True)
-                data = json_loads(data)
+                data = request.json
 
                 # Convertendo os dados para o DTO
                 data = self._dto_class(**data)
 
                 # Construindo os objetos
                 service = self._get_service(factory)
```

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         """
         Tratando requisições HTTP Put para inserir uma instância de uma entidade.
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os dados do corpo da rquisição
-                data = request.get_data(as_text=True)
-                data = json_loads(data)
+                data = request.json
 
                 # Convertendo os dados para o DTO
                 data = self._dto_class(**data)
 
                 # Montando os filtros de particao de dados
                 partition_filters = {}
```

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,20 @@
             try:
                 value = float(value)
             except:
                 erro_tipo = True
         elif self.expected_type is Decimal:
             # Int
             try:
+                value = str(value)
+            except:
+                erro_tipo = True
+        elif self.expected_type is str:
+            # Int
+            try:
                 value = Decimal(value)
             except:
                 erro_tipo = True
         else:
             erro_tipo = True
 
         if erro_tipo:
```

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/service/service_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-0.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


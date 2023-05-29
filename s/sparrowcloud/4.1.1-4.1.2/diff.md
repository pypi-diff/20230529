# Comparing `tmp/sparrowcloud-4.1.1.tar.gz` & `tmp/sparrowcloud-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparrowcloud-4.1.1.tar", last modified: Tue May  9 06:42:44 2023, max compression
+gzip compressed data, was "dist/sparrowcloud-4.1.2.tar", last modified: Mon May 29 06:26:01 2023, max compression
```

## Comparing `sparrowcloud-4.1.1.tar` & `sparrowcloud-4.1.2.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.915218 sparrowcloud-4.1.1/
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1068 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/LICENSE
--rw-r--r--   0 tigerlittle   (501) staff       (20)    22407 2023-05-09 06:42:44.915043 sparrowcloud-4.1.1/PKG-INFO
--rw-r--r--   0 tigerlittle   (501) staff       (20)    21898 2023-05-09 06:41:20.000000 sparrowcloud-4.1.1/README.md
--rw-r--r--   0 tigerlittle   (501) staff       (20)       38 2023-05-09 06:42:44.915261 sparrowcloud-4.1.1/setup.cfg
--rwxr-xr-x   0 tigerlittle   (501) staff       (20)     2431 2023-05-09 06:41:57.000000 sparrowcloud-4.1.1/setup.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.884825 sparrowcloud-4.1.1/sparrow_cloud/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.885843 sparrowcloud-4.1.1/sparrow_cloud/access_control/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/access_control/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1119 2020-10-27 08:32:03.000000 sparrowcloud-4.1.1/sparrow_cloud/access_control/access_verify.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      199 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/access_control/base_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4570 2021-06-23 07:33:41.000000 sparrowcloud-4.1.1/sparrow_cloud/access_control/decorators.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.886128 sparrowcloud-4.1.1/sparrow_cloud/app_message/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-11-18 06:15:22.000000 sparrowcloud-4.1.1/sparrow_cloud/app_message/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1837 2021-02-07 06:05:50.000000 sparrowcloud-4.1.1/sparrow_cloud/app_message/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.886303 sparrowcloud-4.1.1/sparrow_cloud/apps/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.887874 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      896 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/example_access_control.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.888046 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.888307 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1679 2020-10-27 10:00:56.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/commands/register_access_control.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.888496 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.889457 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/admin.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.890267 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/
--rw-r--r--   0 tigerlittle   (501) staff       (20)      940 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1341 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      845 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14094 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      117 2023-03-07 08:29:29.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.890423 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.891081 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14060 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/_controller.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2943 2020-11-10 08:04:05.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      643 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.891241 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.892704 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      129 2023-03-07 09:09:03.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    21443 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/generators_django_1.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    17804 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/generators_django_2.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.892866 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.893303 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1614 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/_api.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     8069 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.893476 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      474 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      855 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      694 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      456 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.894574 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2023-03-07 08:30:32.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.894744 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      165 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      277 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/ping/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.895789 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      121 2023-03-07 08:30:15.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/apps.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      954 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/contributor.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.896012 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/__init__.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.896257 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/commands/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/commands/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1659 2020-10-28 07:54:35.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.896436 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/models.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.897826 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/
--rw-r--r--   0 tigerlittle   (501) staff       (20)      272 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1353 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/compat.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    14532 2023-03-29 03:35:53.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/generators.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      148 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/incompatible_settings.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)    17462 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/inspectors.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7418 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/patch.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1035 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/utils.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.899092 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/admin.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      143 2023-03-07 09:21:53.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/apps.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.899266 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/migrations/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/migrations/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      268 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/models.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      190 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/serializers.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/tests.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      130 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/urls.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1180 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/views.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.899655 sparrowcloud-4.1.1/sparrow_cloud/auth/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/auth/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      467 2021-06-18 03:25:54.000000 sparrowcloud-4.1.1/sparrow_cloud/auth/user.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2149 2021-07-29 06:08:19.000000 sparrowcloud-4.1.1/sparrow_cloud/auth/user_id_authentication.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.901379 sparrowcloud-4.1.1/sparrow_cloud/authorization/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/authorization/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      541 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/authorization/token.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.901791 sparrowcloud-4.1.1/sparrow_cloud/cache/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/cache/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1425 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/cache/cache_manager.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.902138 sparrowcloud-4.1.1/sparrow_cloud/dingtalk/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/dingtalk/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1263 2020-10-28 07:54:06.000000 sparrowcloud-4.1.1/sparrow_cloud/dingtalk/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.902456 sparrowcloud-4.1.1/sparrow_cloud/distributed_lock/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2021-02-07 06:05:50.000000 sparrowcloud-4.1.1/sparrow_cloud/distributed_lock/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2440 2021-02-07 06:05:50.000000 sparrowcloud-4.1.1/sparrow_cloud/distributed_lock/lock_op.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.902780 sparrowcloud-4.1.1/sparrow_cloud/filter/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:40:21.000000 sparrowcloud-4.1.1/sparrow_cloud/filter/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      281 2023-05-08 07:07:12.000000 sparrowcloud-4.1.1/sparrow_cloud/filter/log_filters.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.903457 sparrowcloud-4.1.1/sparrow_cloud/message_service/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/message_service/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4200 2020-10-28 07:54:22.000000 sparrowcloud-4.1.1/sparrow_cloud/message_service/sender.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2320 2020-10-27 06:12:38.000000 sparrowcloud-4.1.1/sparrow_cloud/message_service/sender_controller.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.904945 sparrowcloud-4.1.1/sparrow_cloud/middleware/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2023-05-08 07:06:50.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1730 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/acl_middleware.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.905254 sparrowcloud-4.1.1/sparrow_cloud/middleware/base/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/base/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      528 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/base/base_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      841 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/exception.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1530 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/jwt_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2432 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/lock_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1031 2023-05-09 02:50:33.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/log_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      651 2020-10-30 09:30:11.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/methodconvert.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3433 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/middleware/tracing_middleware.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.905699 sparrowcloud-4.1.1/sparrow_cloud/registry/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/registry/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2333 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/registry/service_configuration.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3405 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/registry/service_discovery.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.906326 sparrowcloud-4.1.1/sparrow_cloud/restclient/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/restclient/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      593 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/restclient/exception.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3112 2021-07-29 06:08:19.000000 sparrowcloud-4.1.1/sparrow_cloud/restclient/requests_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4190 2021-07-29 06:08:19.000000 sparrowcloud-4.1.1/sparrow_cloud/restclient/rest_client.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.906595 sparrowcloud-4.1.1/sparrow_cloud/service_log/
--rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/service_log/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1010 2020-10-30 06:33:49.000000 sparrowcloud-4.1.1/sparrow_cloud/service_log/sender.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.908818 sparrowcloud-4.1.1/sparrow_cloud/utils/
--rw-r--r--   0 tigerlittle   (501) staff       (20)      181 2023-05-08 07:07:01.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/__init__.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      394 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/build_url.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      283 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/common_exceptions.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      685 2021-06-18 03:25:54.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/decode_jwt.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      341 2021-01-08 06:07:37.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/get_cm_value.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      692 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/get_hash_key.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      700 2020-10-27 08:08:15.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/get_settings_value.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      917 2020-10-27 09:57:27.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/get_user.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      374 2020-10-27 09:57:47.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/normalize_url.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      837 2020-10-27 10:01:08.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/resource_cls_attribute.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2063 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/send_alert.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1240 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/sparrow_cloud/utils/validation_acl.py
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.909849 sparrowcloud-4.1.1/sparrowcloud.egg-info/
--rw-r--r--   0 tigerlittle   (501) staff       (20)    22407 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/PKG-INFO
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7208 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/SOURCES.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/dependency_links.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/not-zip-safe
--rw-r--r--   0 tigerlittle   (501) staff       (20)      155 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/requires.txt
--rw-r--r--   0 tigerlittle   (501) staff       (20)       14 2023-05-09 06:42:44.000000 sparrowcloud-4.1.1/sparrowcloud.egg-info/top_level.txt
-drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:42:44.914792 sparrowcloud-4.1.1/tests/
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2820 2021-07-29 06:08:19.000000 sparrowcloud-4.1.1/tests/test_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2481 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_acl_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     7264 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/tests/test_api_permission.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2332 2023-03-31 03:34:52.000000 sparrowcloud-4.1.1/tests/test_app_message.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3021 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_consul_service.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1960 2023-03-31 03:34:52.000000 sparrowcloud-4.1.1/tests/test_ding_talk.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2663 2021-02-07 06:05:50.000000 sparrowcloud-4.1.1/tests/test_distributed_lock.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1663 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/tests/test_exception_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     4670 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/tests/test_get_token_sdk.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      820 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_hash_key.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     5470 2023-03-07 09:49:19.000000 sparrowcloud-4.1.1/tests/test_jwtmiddleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3230 2021-06-03 09:44:22.000000 sparrowcloud-4.1.1/tests/test_lock_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)      750 2023-05-08 07:07:30.000000 sparrowcloud-4.1.1/tests/test_log_filter.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1773 2020-10-28 05:14:21.000000 sparrowcloud-4.1.1/tests/test_message_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     8219 2022-05-30 04:53:46.000000 sparrowcloud-4.1.1/tests/test_rabbitmq_consumer_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2178 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/tests/test_register_access_control.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2221 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_register_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2013 2020-10-28 06:20:10.000000 sparrowcloud-4.1.1/tests/test_register_schema_command.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1344 2023-05-08 07:07:37.000000 sparrowcloud-4.1.1/tests/test_requestid_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     3419 2020-10-28 05:11:47.000000 sparrowcloud-4.1.1/tests/test_requests_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     5741 2020-10-28 05:12:06.000000 sparrowcloud-4.1.1/tests/test_rest_client.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2182 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_service_configuration.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2710 2020-10-30 06:34:59.000000 sparrowcloud-4.1.1/tests/test_service_log.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1450 2020-09-29 03:48:09.000000 sparrowcloud-4.1.1/tests/test_table_api.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     1702 2020-10-26 04:41:02.000000 sparrowcloud-4.1.1/tests/test_tracing_middleware.py
--rw-r--r--   0 tigerlittle   (501) staff       (20)     2989 2021-07-29 06:08:19.000000 sparrowcloud-4.1.1/tests/test_user_id_authentication.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.353028 sparrowcloud-4.1.2/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1068 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/LICENSE
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    22407 2023-05-29 06:26:01.352857 sparrowcloud-4.1.2/PKG-INFO
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    21898 2023-05-09 06:41:20.000000 sparrowcloud-4.1.2/README.md
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       38 2023-05-29 06:26:01.353073 sparrowcloud-4.1.2/setup.cfg
+-rwxr-xr-x   0 tigerlittle   (501) staff       (20)     2431 2023-05-29 06:25:58.000000 sparrowcloud-4.1.2/setup.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.325677 sparrowcloud-4.1.2/sparrow_cloud/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.326455 sparrowcloud-4.1.2/sparrow_cloud/access_control/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/access_control/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1119 2020-10-27 08:32:03.000000 sparrowcloud-4.1.2/sparrow_cloud/access_control/access_verify.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      199 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/access_control/base_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4570 2021-06-23 07:33:41.000000 sparrowcloud-4.1.2/sparrow_cloud/access_control/decorators.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.326710 sparrowcloud-4.1.2/sparrow_cloud/app_message/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-11-18 06:15:22.000000 sparrowcloud-4.1.2/sparrow_cloud/app_message/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1837 2021-02-07 06:05:50.000000 sparrowcloud-4.1.2/sparrow_cloud/app_message/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.326839 sparrowcloud-4.1.2/sparrow_cloud/apps/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.328499 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      896 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/example_access_control.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.328652 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.328897 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1679 2020-10-27 10:00:56.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/commands/register_access_control.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.329063 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.329996 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/admin.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.330671 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      940 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1341 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      845 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14094 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      117 2023-03-07 08:29:29.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.330824 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.331538 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14170 2023-05-29 06:20:34.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/_controller.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2943 2020-11-10 08:04:05.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      643 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.331693 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.333118 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      129 2023-03-07 09:09:03.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    21443 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/generators_django_1.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    17804 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/generators_django_2.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.333291 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.333716 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1614 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/_api.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     8069 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.333877 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      474 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      855 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      694 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      456 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.334892 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      102 2023-03-07 08:30:32.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.335041 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      165 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      277 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/ping/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.336049 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      121 2023-03-07 08:30:15.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/apps.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      954 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/contributor.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.336254 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/__init__.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.336490 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/commands/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/commands/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1659 2020-10-28 07:54:35.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.336620 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       57 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/models.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.337937 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      272 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1353 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/compat.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    14532 2023-03-29 03:35:53.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/generators.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      148 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/incompatible_settings.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    17462 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/inspectors.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7418 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/patch.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1035 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/utils.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       60 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.339199 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       63 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/admin.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      143 2023-03-07 09:21:53.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/apps.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.339394 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/migrations/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/migrations/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      268 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/models.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      190 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/serializers.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/tests.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      130 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/urls.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1180 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/views.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.339805 sparrowcloud-4.1.2/sparrow_cloud/auth/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/auth/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      467 2021-06-18 03:25:54.000000 sparrowcloud-4.1.2/sparrow_cloud/auth/user.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2149 2021-07-29 06:08:19.000000 sparrowcloud-4.1.2/sparrow_cloud/auth/user_id_authentication.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.340096 sparrowcloud-4.1.2/sparrow_cloud/authorization/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/authorization/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      541 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/sparrow_cloud/authorization/token.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.340365 sparrowcloud-4.1.2/sparrow_cloud/cache/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/cache/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1425 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/cache/cache_manager.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.340624 sparrowcloud-4.1.2/sparrow_cloud/dingtalk/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/dingtalk/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1263 2020-10-28 07:54:06.000000 sparrowcloud-4.1.2/sparrow_cloud/dingtalk/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.340879 sparrowcloud-4.1.2/sparrow_cloud/distributed_lock/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2021-02-07 06:05:50.000000 sparrowcloud-4.1.2/sparrow_cloud/distributed_lock/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2440 2021-02-07 06:05:50.000000 sparrowcloud-4.1.2/sparrow_cloud/distributed_lock/lock_op.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.341143 sparrowcloud-4.1.2/sparrow_cloud/filter/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2023-05-09 06:40:21.000000 sparrowcloud-4.1.2/sparrow_cloud/filter/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      281 2023-05-08 07:07:12.000000 sparrowcloud-4.1.2/sparrow_cloud/filter/log_filters.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.341723 sparrowcloud-4.1.2/sparrow_cloud/message_service/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/message_service/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4200 2020-10-28 07:54:22.000000 sparrowcloud-4.1.2/sparrow_cloud/message_service/sender.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2320 2020-10-27 06:12:38.000000 sparrowcloud-4.1.2/sparrow_cloud/message_service/sender_controller.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.343129 sparrowcloud-4.1.2/sparrow_cloud/middleware/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2023-05-08 07:06:50.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1730 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/acl_middleware.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.343609 sparrowcloud-4.1.2/sparrow_cloud/middleware/base/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/base/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      528 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/base/base_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      841 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/exception.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1530 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/jwt_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2432 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/lock_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1031 2023-05-09 02:50:33.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/log_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      651 2020-10-30 09:30:11.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/methodconvert.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3433 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/middleware/tracing_middleware.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.344040 sparrowcloud-4.1.2/sparrow_cloud/registry/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/registry/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2333 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/registry/service_configuration.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3405 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/registry/service_discovery.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.344628 sparrowcloud-4.1.2/sparrow_cloud/restclient/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/restclient/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      593 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/restclient/exception.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3112 2021-07-29 06:08:19.000000 sparrowcloud-4.1.2/sparrow_cloud/restclient/requests_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4190 2021-07-29 06:08:19.000000 sparrowcloud-4.1.2/sparrow_cloud/restclient/rest_client.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.344951 sparrowcloud-4.1.2/sparrow_cloud/service_log/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        0 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/service_log/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1010 2020-10-30 06:33:49.000000 sparrowcloud-4.1.2/sparrow_cloud/service_log/sender.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.347100 sparrowcloud-4.1.2/sparrow_cloud/utils/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      181 2023-05-08 07:07:01.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/__init__.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      394 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/build_url.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      283 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/common_exceptions.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      685 2021-06-18 03:25:54.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/decode_jwt.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      341 2021-01-08 06:07:37.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/get_cm_value.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      692 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/get_hash_key.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      700 2020-10-27 08:08:15.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/get_settings_value.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      917 2020-10-27 09:57:27.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/get_user.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      374 2020-10-27 09:57:47.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/normalize_url.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      837 2020-10-27 10:01:08.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/resource_cls_attribute.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2063 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/send_alert.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1240 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/sparrow_cloud/utils/validation_acl.py
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.348099 sparrowcloud-4.1.2/sparrowcloud.egg-info/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)    22407 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/PKG-INFO
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7208 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)        1 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/not-zip-safe
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      155 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/requires.txt
+-rw-r--r--   0 tigerlittle   (501) staff       (20)       14 2023-05-29 06:26:01.000000 sparrowcloud-4.1.2/sparrowcloud.egg-info/top_level.txt
+drwxr-xr-x   0 tigerlittle   (501) staff       (20)        0 2023-05-29 06:26:01.352614 sparrowcloud-4.1.2/tests/
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2820 2021-07-29 06:08:19.000000 sparrowcloud-4.1.2/tests/test_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2481 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_acl_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     7264 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/tests/test_api_permission.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2332 2023-03-31 03:34:52.000000 sparrowcloud-4.1.2/tests/test_app_message.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3021 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_consul_service.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1960 2023-03-31 03:34:52.000000 sparrowcloud-4.1.2/tests/test_ding_talk.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2663 2021-02-07 06:05:50.000000 sparrowcloud-4.1.2/tests/test_distributed_lock.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1663 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/tests/test_exception_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     4670 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/tests/test_get_token_sdk.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      820 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_hash_key.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     5470 2023-03-07 09:49:19.000000 sparrowcloud-4.1.2/tests/test_jwtmiddleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3230 2021-06-03 09:44:22.000000 sparrowcloud-4.1.2/tests/test_lock_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)      750 2023-05-08 07:07:30.000000 sparrowcloud-4.1.2/tests/test_log_filter.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1773 2020-10-28 05:14:21.000000 sparrowcloud-4.1.2/tests/test_message_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     8219 2022-05-30 04:53:46.000000 sparrowcloud-4.1.2/tests/test_rabbitmq_consumer_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2178 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/tests/test_register_access_control.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2221 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_register_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2013 2020-10-28 06:20:10.000000 sparrowcloud-4.1.2/tests/test_register_schema_command.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1344 2023-05-08 07:07:37.000000 sparrowcloud-4.1.2/tests/test_requestid_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     3419 2020-10-28 05:11:47.000000 sparrowcloud-4.1.2/tests/test_requests_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     5741 2020-10-28 05:12:06.000000 sparrowcloud-4.1.2/tests/test_rest_client.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2182 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_service_configuration.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2710 2020-10-30 06:34:59.000000 sparrowcloud-4.1.2/tests/test_service_log.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1450 2020-09-29 03:48:09.000000 sparrowcloud-4.1.2/tests/test_table_api.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     1702 2020-10-26 04:41:02.000000 sparrowcloud-4.1.2/tests/test_tracing_middleware.py
+-rw-r--r--   0 tigerlittle   (501) staff       (20)     2989 2021-07-29 06:08:19.000000 sparrowcloud-4.1.2/tests/test_user_id_authentication.py
```

### Comparing `sparrowcloud-4.1.1/LICENSE` & `sparrowcloud-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/PKG-INFO` & `sparrowcloud-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrowcloud
-Version: 4.1.1
+Version: 4.1.2
 Summary: 基础Django和drf的微服务框架扩展
 Home-page: https://gitee.com/sparrow614/sparrow_cloud
 Author: sparrow
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `sparrowcloud-4.1.1/README.md` & `sparrowcloud-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/setup.py` & `sparrowcloud-4.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # import io
 import os
 import sys
 import shutil
 from setuptools import find_packages, setup
 
-version = "v4.1.1"
+version = "v4.1.2"
 
 
 def read(f):
     return open(f, 'r', encoding='utf-8').read()
 
 
 if sys.argv[-1] == 'publish':
```

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/access_control/access_verify.py` & `sparrowcloud-4.1.2/sparrow_cloud/access_control/access_verify.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/access_control/decorators.py` & `sparrowcloud-4.1.2/sparrow_cloud/access_control/decorators.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/app_message/sender.py` & `sparrowcloud-4.1.2/sparrow_cloud/app_message/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/example_access_control.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/example_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/access_control/management/commands/register_access_control.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/access_control/management/commands/register_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider2.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/AliyunCredentialsProvider3.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/connection.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/aliyun_amqp/receiver.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/_controller.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 from pika.exceptions import AMQPConnectionError as BrokerConnectonException
 from datetime import datetime
 from sparrow_cloud.restclient import rest_client
+from django.db import close_old_connections
 
 import base64, decimal, collections
 import importlib
 import json
 import logging
 import os
 import pika
@@ -233,14 +234,17 @@
             logger.error(fm2)
         logger.info(
             ' [*] {0} Finished task_id {1}.'.format(datetime.now(), task_id))
 
         cb = functools.partial(self.ack_message, channel, delivery_tag)
         connection.add_callback_threadsafe(cb)
 
+        # 关闭数据库连接 
+        close_old_connections()
+
     def on_message(self, channel, method_frame, header_frame, body, args):
         (connection, threads) = args
         t = threading.Thread(target=self.do_work, args=(
             connection, channel, method_frame, header_frame, body))
         t.start()
         threads.append(t)
```

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/_sparrow_rabbitmq_consumer.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/message_service/management/commands/rabbitmq_consumer.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/generators_django_1.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/generators_django_1.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/generators_django_2.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/generators_django_2.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/_api.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/_api.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/management/commands/register_api_permission.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/tests.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/tests.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/permission_command/urls.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/permission_command/urls.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/contributor.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/contributor.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/management/commands/register_api_schema.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/compat.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/compat.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/generators.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/generators.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/inspectors.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/inspectors.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/patch.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/patch.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/schema_command/schemas/utils.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/schema_command/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/apps/table_api/views.py` & `sparrowcloud-4.1.2/sparrow_cloud/apps/table_api/views.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/auth/user_id_authentication.py` & `sparrowcloud-4.1.2/sparrow_cloud/auth/user_id_authentication.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/authorization/token.py` & `sparrowcloud-4.1.2/sparrow_cloud/authorization/token.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/cache/cache_manager.py` & `sparrowcloud-4.1.2/sparrow_cloud/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/dingtalk/sender.py` & `sparrowcloud-4.1.2/sparrow_cloud/dingtalk/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/distributed_lock/lock_op.py` & `sparrowcloud-4.1.2/sparrow_cloud/distributed_lock/lock_op.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/message_service/sender.py` & `sparrowcloud-4.1.2/sparrow_cloud/message_service/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/message_service/sender_controller.py` & `sparrowcloud-4.1.2/sparrow_cloud/message_service/sender_controller.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/acl_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/acl_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/base/base_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/base/base_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/exception.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/jwt_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/jwt_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/lock_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/lock_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/log_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/log_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/methodconvert.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/methodconvert.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/middleware/tracing_middleware.py` & `sparrowcloud-4.1.2/sparrow_cloud/middleware/tracing_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/registry/service_configuration.py` & `sparrowcloud-4.1.2/sparrow_cloud/registry/service_configuration.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/registry/service_discovery.py` & `sparrowcloud-4.1.2/sparrow_cloud/registry/service_discovery.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/restclient/exception.py` & `sparrowcloud-4.1.2/sparrow_cloud/restclient/exception.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/restclient/requests_client.py` & `sparrowcloud-4.1.2/sparrow_cloud/restclient/requests_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/restclient/rest_client.py` & `sparrowcloud-4.1.2/sparrow_cloud/restclient/rest_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/service_log/sender.py` & `sparrowcloud-4.1.2/sparrow_cloud/service_log/sender.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/decode_jwt.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/decode_jwt.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/get_hash_key.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/get_hash_key.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/get_settings_value.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/get_settings_value.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/get_user.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/get_user.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/resource_cls_attribute.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/resource_cls_attribute.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/send_alert.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/send_alert.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrow_cloud/utils/validation_acl.py` & `sparrowcloud-4.1.2/sparrow_cloud/utils/validation_acl.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/sparrowcloud.egg-info/PKG-INFO` & `sparrowcloud-4.1.2/sparrowcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparrowcloud
-Version: 4.1.1
+Version: 4.1.2
 Summary: 基础Django和drf的微服务框架扩展
 Home-page: https://gitee.com/sparrow614/sparrow_cloud
 Author: sparrow
 Author-email: 
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `sparrowcloud-4.1.1/sparrowcloud.egg-info/SOURCES.txt` & `sparrowcloud-4.1.2/sparrowcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_access_control.py` & `sparrowcloud-4.1.2/tests/test_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_acl_middleware.py` & `sparrowcloud-4.1.2/tests/test_acl_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_api_permission.py` & `sparrowcloud-4.1.2/tests/test_api_permission.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_app_message.py` & `sparrowcloud-4.1.2/tests/test_app_message.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_consul_service.py` & `sparrowcloud-4.1.2/tests/test_consul_service.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_ding_talk.py` & `sparrowcloud-4.1.2/tests/test_ding_talk.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_distributed_lock.py` & `sparrowcloud-4.1.2/tests/test_distributed_lock.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_exception_middleware.py` & `sparrowcloud-4.1.2/tests/test_exception_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_get_token_sdk.py` & `sparrowcloud-4.1.2/tests/test_get_token_sdk.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_hash_key.py` & `sparrowcloud-4.1.2/tests/test_hash_key.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_jwtmiddleware.py` & `sparrowcloud-4.1.2/tests/test_jwtmiddleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_lock_middleware.py` & `sparrowcloud-4.1.2/tests/test_lock_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_log_filter.py` & `sparrowcloud-4.1.2/tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_message_client.py` & `sparrowcloud-4.1.2/tests/test_message_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_rabbitmq_consumer_command.py` & `sparrowcloud-4.1.2/tests/test_rabbitmq_consumer_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_register_access_control.py` & `sparrowcloud-4.1.2/tests/test_register_access_control.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_register_command.py` & `sparrowcloud-4.1.2/tests/test_register_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_register_schema_command.py` & `sparrowcloud-4.1.2/tests/test_register_schema_command.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_requestid_middleware.py` & `sparrowcloud-4.1.2/tests/test_requestid_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_requests_client.py` & `sparrowcloud-4.1.2/tests/test_requests_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_rest_client.py` & `sparrowcloud-4.1.2/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_service_configuration.py` & `sparrowcloud-4.1.2/tests/test_service_configuration.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_service_log.py` & `sparrowcloud-4.1.2/tests/test_service_log.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_table_api.py` & `sparrowcloud-4.1.2/tests/test_table_api.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_tracing_middleware.py` & `sparrowcloud-4.1.2/tests/test_tracing_middleware.py`

 * *Files identical despite different names*

### Comparing `sparrowcloud-4.1.1/tests/test_user_id_authentication.py` & `sparrowcloud-4.1.2/tests/test_user_id_authentication.py`

 * *Files identical despite different names*


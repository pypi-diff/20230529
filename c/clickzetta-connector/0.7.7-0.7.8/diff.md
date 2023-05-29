# Comparing `tmp/clickzetta-connector-0.7.7.tar.gz` & `tmp/clickzetta-connector-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.7.7.tar", last modified: Mon May 29 06:31:09 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.7.8.tar", last modified: Mon May 29 08:36:03 2023, max compression
```

## Comparing `clickzetta-connector-0.7.7.tar` & `clickzetta-connector-0.7.8.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699878 clickzetta-connector-0.7.7/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 06:31:09.699737 clickzetta-connector-0.7.7/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.686217 clickzetta-connector-0.7.7/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.686923 clickzetta-connector-0.7.7/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    38181 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.7/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.687813 clickzetta-connector-0.7.7/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4544 2023-05-29 06:30:58.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.683874 clickzetta-connector-0.7.7/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.695682 clickzetta-connector-0.7.7/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699037 clickzetta-connector-0.7.7/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8775 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.7/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 06:30:58.000000 clickzetta-connector-0.7.7/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699581 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      646 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 06:31:09.699925 clickzetta-connector-0.7.7/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2906 2023-05-29 06:12:31.000000 clickzetta-connector-0.7.7/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.703093 clickzetta-connector-0.7.8/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 08:36:03.702955 clickzetta-connector-0.7.8/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.689029 clickzetta-connector-0.7.8/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.689557 clickzetta-connector-0.7.8/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    21554 2023-05-29 08:34:50.000000 clickzetta-connector-0.7.8/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.690272 clickzetta-connector-0.7.8/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3299 2023-05-29 08:34:50.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.687336 clickzetta-connector-0.7.8/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.698432 clickzetta-connector-0.7.8/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.701887 clickzetta-connector-0.7.8/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7365 2023-05-29 08:34:50.000000 clickzetta-connector-0.7.8/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.8/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 08:35:58.000000 clickzetta-connector-0.7.8/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:36:03.702767 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      646 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 08:36:03.000000 clickzetta-connector-0.7.8/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 08:36:03.703136 clickzetta-connector-0.7.8/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2906 2023-05-29 06:39:42.000000 clickzetta-connector-0.7.8/setup.py
```

### Comparing `clickzetta-connector-0.7.7/clickzetta/_helpers.py` & `clickzetta-connector-0.7.8/clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_stream.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.7.8/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.7.8/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.7.8/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.7.8/clickzetta/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.7.8/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/dbapi/types.py` & `clickzetta-connector-0.7.8/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/enums.py` & `clickzetta-connector-0.7.8/clickzetta/enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.7.8/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/ingestion.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.7.8/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/query_result.py` & `clickzetta-connector-0.7.8/clickzetta/query_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,21 +52,20 @@
         self.length = length
 
     def set_nullable(self, nullable):
         self.nullable = nullable
 
 
 class QueryResult(object):
-    def __init__(self, total_msg: string, query_type: str):
+    def __init__(self, total_msg):
         self.data = None
         self.state = None
         self.total_row_count = 0
         self.total_msg = total_msg
         self.schema = []
-        self.query_type = query_type
         self._parse_result_data()
 
     def _parse_field(self, field: str, schema_field: Field):
         schema_field.set_name(field['name'])
         if field['type'].__contains__('charTypeInfo'):
             schema_field.set_type(field['type']['category'])
             schema_field.set_nullable(str(field['type']['nullable']) != 'False')
@@ -80,26 +79,17 @@
             schema_field.set_type(field['type']['category'])
             schema_field.set_nullable(str(field['type']['nullable']) == 'true')
 
     def get_result_state(self) -> string:
         return self.total_msg['status']['state']
 
     def _parse_result_data(self):
-        if self.query_type == 'anon':
-            field = Field()
-            field.set_name('RESULT_MESSAGE')
-            field.set_type("STRING")
-            self.schema.append(field)
-            self.total_row_count = 1
-            result_data = [['OPERATION SUCCEED']]
-            self.data = QueryData(result_data)
-            return
         self.state = self.total_msg['status']['state']
         if self.state != 'FAILED':
-            if self.query_type == 'create' or self.query_type == 'alter' or self.query_type == 'drop' or self.query_type == 'truncate' or self.query_type == 'insert':
+            if 'data' not in self.total_msg['resultSet']:
                 field = Field()
                 field.set_name('RESULT_MESSAGE')
                 field.set_type("STRING")
                 self.schema.append(field)
                 self.total_row_count = 1
                 result_data = [['OPERATION SUCCEED']]
                 self.data = QueryData(result_data)
@@ -128,70 +118,58 @@
                     self._parse_field(field, schema_field)
                     self.schema.append(schema_field)
                 result_data = []
                 csv.register_dialect('cz_dialect', delimiter=',', escapechar='\\')
                 for row in data_list:
                     data_list = []
                     has_null = False
-                    if self.query_type == 'select' or self.query_type == 'desc':
-                        if "\\N" in row:
-                            has_null = True
-                        reader = csv.reader(io.StringIO(row), dialect='cz_dialect')
-                        for line in reader:
-                            for i in range(len(line)):
-                                if self.schema[i].field_type.startswith('DECIMAL') or \
-                                        self.schema[i].field_type.startswith('decimal'):
-                                    if line[i] == "N" and has_null:
-                                        data_list.append(None)
-                                    else:
-                                        decimal_value = decimal.Decimal(line[i]).to_eng_string()
-                                        data_list.append(decimal_value)
-                                elif self.schema[i].field_type.startswith('INT') or \
-                                        self.schema[i].field_type.startswith('int'):
-                                    if line[i] == "N" and has_null:
-                                        data_list.append(None)
-                                    else:
-                                        data_list.append(int(line[i]))
-                                elif self.schema[i].field_type.startswith('FLOAT') or \
-                                        self.schema[i].field_type.startswith('float'):
-                                    if line[i] == "N" and has_null:
-                                        data_list.append(None)
-                                    else:
-                                        data_list.append(float(line[i]))
-                                elif self.schema[i].field_type == "STRING" or self.schema[i].field_type.startswith(
-                                        "VARCHAR") or \
-                                        self.schema[i].field_type.startswith("CHAR") or self.schema[
-                                    i].field_type == "string" or \
-                                        self.schema[i].field_type.startswith("varchar") or self.schema[
-                                    i].field_type.startswith("CHAR") or \
-                                        self.schema[i].field_type.startswith("TIMESTAMP"):
-                                    if line[i] == "N" and has_null:
-                                        data_list.append(None)
-                                    else:
-                                        data_list.append(line[i])
-
+                    if "\\N" in row:
+                        has_null = True
+                    reader = csv.reader(io.StringIO(row), dialect='cz_dialect')
+                    for line in reader:
+                        for i in range(len(line)):
+                            if self.schema[i].field_type.startswith('DECIMAL') or \
+                                    self.schema[i].field_type.startswith('decimal'):
+                                if line[i] == "N" and has_null:
+                                    data_list.append(None)
+                                else:
+                                    decimal_value = decimal.Decimal(line[i]).to_eng_string()
+                                    data_list.append(decimal_value)
+                            elif self.schema[i].field_type.startswith('INT') or \
+                                    self.schema[i].field_type.startswith('int'):
+                                if line[i] == "N" and has_null:
+                                    data_list.append(None)
+                                else:
+                                    data_list.append(int(line[i]))
+                            elif self.schema[i].field_type.startswith('FLOAT') or \
+                                    self.schema[i].field_type.startswith('float'):
+                                if line[i] == "N" and has_null:
+                                    data_list.append(None)
+                                else:
+                                    data_list.append(float(line[i]))
+                            elif self.schema[i].field_type == "STRING" or self.schema[i].field_type.startswith(
+                                    "VARCHAR") or \
+                                    self.schema[i].field_type.startswith("CHAR") or self.schema[
+                                i].field_type == "string" or \
+                                    self.schema[i].field_type.startswith("varchar") or self.schema[
+                                i].field_type.startswith("CHAR") or \
+                                    self.schema[i].field_type.startswith("TIMESTAMP"):
+                                if line[i] == "N" and has_null:
+                                    data_list.append(None)
                                 else:
                                     data_list.append(line[i])
-                        if len(data_list) > len(self.schema):
-                            data_list = data_list[0:len(self.schema)]
-                    elif self.query_type == 'show':
-                        if len(self.schema) == 1:
-                            data_list.append(row)
-                        else:
-                            for value in row.split(','):
-                                data_list.append(value)
-                            if len(data_list) > len(self.schema):
-                                data_list = data_list[0:len(self.schema)]
-                    elif self.query_type == 'other':
-                        for value in row.split(','):
-                            data_list.append(value)
-                    else:
-                        data_list.append(row)
+
+                            else:
+                                data_list.append(line[i])
+                    if len(data_list) > len(self.schema):
+                        data_list = data_list[0:len(self.schema)]
+
                     result_data.append(data_list)
                 self.data = QueryData(result_data)
+
         else:
             field = Field()
             field.set_name('ERROR_MESSAGE')
             field.set_type("STRING")
             self.schema.append(field)
             self.total_row_count = 1
             result_data = [[self.total_msg['status']['message'].split('\n')[0]]]
```

### Comparing `clickzetta-connector-0.7.7/clickzetta/schema.py` & `clickzetta-connector-0.7.8/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/session.py` & `clickzetta-connector-0.7.8/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/standard_sql.py` & `clickzetta-connector-0.7.8/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta/table.py` & `clickzetta-connector-0.7.8/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.7.8/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.7.8/clickzetta_connector.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.7/setup.py` & `clickzetta-connector-0.7.8/setup.py`

 * *Files identical despite different names*


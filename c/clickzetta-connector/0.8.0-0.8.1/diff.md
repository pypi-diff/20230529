# Comparing `tmp/clickzetta-connector-0.8.0.tar.gz` & `tmp/clickzetta-connector-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.8.0.tar", last modified: Mon May 29 08:59:22 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.8.1.tar", last modified: Mon May 29 09:32:35 2023, max compression
```

## Comparing `clickzetta-connector-0.8.0.tar` & `clickzetta-connector-0.8.1.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.737225 clickzetta-connector-0.8.0/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 08:59:22.737080 clickzetta-connector-0.8.0/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.721245 clickzetta-connector-0.8.0/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.721783 clickzetta-connector-0.8.0/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    21554 2023-05-29 08:34:50.000000 clickzetta-connector-0.8.0/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.722587 clickzetta-connector-0.8.0/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2974 2023-05-29 08:59:14.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.718724 clickzetta-connector-0.8.0/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.731241 clickzetta-connector-0.8.0/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.736304 clickzetta-connector-0.8.0/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7365 2023-05-29 08:34:50.000000 clickzetta-connector-0.8.0/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.0/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 08:59:14.000000 clickzetta-connector-0.8.0/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 08:59:22.736914 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      630 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 08:59:22.000000 clickzetta-connector-0.8.0/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 08:59:22.737268 clickzetta-connector-0.8.0/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2881 2023-05-29 08:59:14.000000 clickzetta-connector-0.8.0/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.242589 clickzetta-connector-0.8.1/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 09:32:35.242458 clickzetta-connector-0.8.1/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.227383 clickzetta-connector-0.8.1/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.227897 clickzetta-connector-0.8.1/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    21726 2023-05-29 09:29:09.000000 clickzetta-connector-0.8.1/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.229118 clickzetta-connector-0.8.1/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2974 2023-05-29 09:04:51.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.225126 clickzetta-connector-0.8.1/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.238346 clickzetta-connector-0.8.1/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 09:32:34.000000 clickzetta-connector-0.8.1/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.241767 clickzetta-connector-0.8.1/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7365 2023-05-29 09:04:51.000000 clickzetta-connector-0.8.1/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.1/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 09:32:26.000000 clickzetta-connector-0.8.1/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 09:32:35.242312 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      630 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 09:32:35.000000 clickzetta-connector-0.8.1/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 09:32:35.242630 clickzetta-connector-0.8.1/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2881 2023-05-29 09:04:51.000000 clickzetta-connector-0.8.1/setup.py
```

### Comparing `clickzetta-connector-0.8.0/clickzetta/_helpers.py` & `clickzetta-connector-0.8.1/clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_stream.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.8.1/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/client.py` & `clickzetta-connector-0.8.1/clickzetta/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,33 +281,38 @@
 
         HEADERS['instanceName'] = self.instance_name
         HEADERS['X-ClickZetta-Token'] = self.token
         try:
             api_response = requests.post(self.base_url + path, data=MessageToJson(gate_way_request), headers=HEADERS)
             result = api_response.text
             result_dict = json.loads(result)
+            if api_response.status_code != 200:
+                raise requests.exceptions.RequestException(
+                    'gate_way_call return failed code.Error message:' + result_dict['message'])
             result_status = ParseDict(result_dict['status'], ingestion_pb2.GateWayResponseStatus)
             if result_status.code == ingestion_pb2.Code.SUCCESS:
                 message_json = json.loads(result_dict['message'])
                 internal_result_status = message_json['status']
                 if internal_result_status["code"] == "SUCCESS":
                     return json.loads(result_dict['message'])
                 else:
                     raise requests.exceptions.RequestException(
                         'gate_way_call return failed code.Error message:' + internal_result_status["error_message"])
             else:
                 raise requests.exceptions.RequestException(
                     'gate_way_call return failed code.Error message:' + result_status.message)
 
-        except requests.exceptions.RequestException:
-            logging.error('gate_way_request error:{}, reqeust body:{}'.format(result_status['message'],
-                                                                              MessageToJson(gate_way_request)))
+        except requests.exceptions.RequestException as request_exception:
+            logging.error('gate_way_request error:{}'.format(request_exception))
+            raise requests.exceptions.RequestException(
+                'gate_way_request error:{}'.format(request_exception))
+        except Exception as e:
+            logging.error('gate_way_request error:{}'.format(e))
             raise requests.exceptions.RequestException(
-                'gate_way_request error:{}, reqeust body:{}'.format(result_status['message'],
-                                                                    MessageToJson(gate_way_request)))
+                'gate_way_request error:{}'.format(e))
 
     def submit_sql_job(self, token: str, sql: str, parameters=None, schema=None) -> QueryResult:
         path = "/lh/submitJob"
         if 'test plain returns' in sql or 'test unicode returns' in sql:
             return QueryResult({})
         table = Table(self.workspace, '', self.instance_name, self.vc_name)
         vc = table.vc_name
```

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/cursor.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/dbapi/types.py` & `clickzetta-connector-0.8.1/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/enums.py` & `clickzetta-connector-0.8.1/clickzetta/enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.8.1/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/ingestion.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.8.1/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/query_result.py` & `clickzetta-connector-0.8.1/clickzetta/query_result.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/schema.py` & `clickzetta-connector-0.8.1/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/session.py` & `clickzetta-connector-0.8.1/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/standard_sql.py` & `clickzetta-connector-0.8.1/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta/table.py` & `clickzetta-connector-0.8.1/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.8.1/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.8.1/clickzetta_connector.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.0/setup.py` & `clickzetta-connector-0.8.1/setup.py`

 * *Files identical despite different names*


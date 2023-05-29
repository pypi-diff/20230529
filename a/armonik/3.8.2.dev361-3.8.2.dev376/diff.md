# Comparing `tmp/armonik-3.8.2.dev361.tar.gz` & `tmp/armonik-3.8.2.dev376.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev361.tar", last modified: Wed May 24 09:33:21 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev376.tar", last modified: Mon May 29 04:54:09 2023, max compression
```

## Comparing `armonik-3.8.2.dev361.tar` & `armonik-3.8.2.dev376.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.387677 armonik-3.8.2.dev361/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:33:21.383677 armonik-3.8.2.dev361/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:33:21.387677 armonik-3.8.2.dev361/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.375676 armonik-3.8.2.dev361/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/tasks_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/versions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/versions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/client/versions_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.383677 armonik-3.8.2.dev361/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/versions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/versions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/versions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.383677 armonik-3.8.2.dev361/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-24 09:33:13.000000 armonik-3.8.2.dev361/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.383677 armonik-3.8.2.dev361/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-24 09:32:58.000000 armonik-3.8.2.dev361/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:21.371676 armonik-3.8.2.dev361/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 09:33:21.000000 armonik-3.8.2.dev361/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-24 09:33:21.000000 armonik-3.8.2.dev361/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:21.000000 armonik-3.8.2.dev361/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 09:33:21.000000 armonik-3.8.2.dev361/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 09:33:21.000000 armonik-3.8.2.dev361/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.461414 armonik-3.8.2.dev376/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.461414 armonik-3.8.2.dev376/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.465414 armonik-3.8.2.dev376/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.465414 armonik-3.8.2.dev376/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.461414 armonik-3.8.2.dev376/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.465414 armonik-3.8.2.dev376/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/versions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/versions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/client/versions_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sort_direction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sort_direction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/sort_direction_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/versions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/versions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/versions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-29 04:54:01.000000 armonik-3.8.2.dev376/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.473414 armonik-3.8.2.dev376/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-29 04:53:48.000000 armonik-3.8.2.dev376/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:54:09.465414 armonik-3.8.2.dev376/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-29 04:54:09.000000 armonik-3.8.2.dev376/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-29 04:54:09.000000 armonik-3.8.2.dev376/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:54:09.000000 armonik-3.8.2.dev376/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 04:54:09.000000 armonik-3.8.2.dev376/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 04:54:09.000000 armonik-3.8.2.dev376/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev361/PKG-INFO` & `armonik-3.8.2.dev376/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev361
+Version: 3.8.2.dev376
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev361/README.md` & `armonik-3.8.2.dev376/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/pyproject.toml` & `armonik-3.8.2.dev376/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/client/submitter.py` & `armonik-3.8.2.dev376/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/client/tasks.py` & `armonik-3.8.2.dev376/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev376/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/common/helpers.py` & `armonik-3.8.2.dev376/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/common/objects.py` & `armonik-3.8.2.dev376/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/results_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/versions_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/versions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/client/versions_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/client/versions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import objects_pb2 as objects__pb2
+from . import sort_direction_pb2 as sort__direction__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x61pplications_common.proto\x12 armonik.api.grpc.v1.applications\x1a\robjects.proto\"S\n\x0e\x41pplicationRaw\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\"\xeb\x05\n\x17ListApplicationsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12P\n\x06\x66ilter\x18\x03 \x01(\x0b\x32@.armonik.api.grpc.v1.applications.ListApplicationsRequest.Filter\x12L\n\x04sort\x18\x04 \x01(\x0b\x32>.armonik.api.grpc.v1.applications.ListApplicationsRequest.Sort\x1aK\n\x06\x46ilter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\x1a\xbb\x01\n\x04Sort\x12V\n\x06\x66ields\x18\x01 \x03(\x0e\x32\x46.armonik.api.grpc.v1.applications.ListApplicationsRequest.OrderByField\x12[\n\tdirection\x18\x02 \x01(\x0e\x32H.armonik.api.grpc.v1.applications.ListApplicationsRequest.OrderDirection\"\x9d\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x01\x12\x1a\n\x16ORDER_BY_FIELD_VERSION\x10\x02\x12\x1c\n\x18ORDER_BY_FIELD_NAMESPACE\x10\x03\x12\x1a\n\x16ORDER_BY_FIELD_SERVICE\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x92\x01\n\x18ListApplicationsResponse\x12\x46\n\x0c\x61pplications\x18\x01 \x03(\x0b\x32\x30.armonik.api.grpc.v1.applications.ApplicationRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\":\n\x19\x43ountTasksByStatusRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB#\xaa\x02 ArmoniK.Api.gRPC.V1.Applicationsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x61pplications_common.proto\x12 armonik.api.grpc.v1.applications\x1a\robjects.proto\x1a\x14sort_direction.proto\"S\n\x0e\x41pplicationRaw\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\"o\n\x10\x41pplicationField\x12R\n\x11\x61pplication_field\x18\x01 \x01(\x0e\x32\x35.armonik.api.grpc.v1.applications.ApplicationRawFieldH\x00\x42\x07\n\x05\x66ield\"\xba\x03\n\x17ListApplicationsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12P\n\x06\x66ilter\x18\x03 \x01(\x0b\x32@.armonik.api.grpc.v1.applications.ListApplicationsRequest.Filter\x12L\n\x04sort\x18\x04 \x01(\x0b\x32>.armonik.api.grpc.v1.applications.ListApplicationsRequest.Sort\x1aK\n\x06\x46ilter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\x1a\x90\x01\n\x04Sort\x12\x42\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x32.armonik.api.grpc.v1.applications.ApplicationField\x12\x44\n\tdirection\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.sort_direction.SortDirection\"\x92\x01\n\x18ListApplicationsResponse\x12\x46\n\x0c\x61pplications\x18\x01 \x03(\x0b\x32\x30.armonik.api.grpc.v1.applications.ApplicationRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\":\n\x19\x43ountTasksByStatusRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount*\xc7\x01\n\x13\x41pplicationRawField\x12%\n!APPLICATION_RAW_FIELD_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x41PPLICATION_RAW_FIELD_NAME\x10\x01\x12!\n\x1d\x41PPLICATION_RAW_FIELD_VERSION\x10\x02\x12#\n\x1f\x41PPLICATION_RAW_FIELD_NAMESPACE\x10\x03\x12!\n\x1d\x41PPLICATION_RAW_FIELD_SERVICE\x10\x04\x42#\xaa\x02 ArmoniK.Api.gRPC.V1.Applicationsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'applications_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002 ArmoniK.Api.gRPC.V1.Applications'
-  _APPLICATIONRAW._serialized_start=78
-  _APPLICATIONRAW._serialized_end=161
-  _LISTAPPLICATIONSREQUEST._serialized_start=164
-  _LISTAPPLICATIONSREQUEST._serialized_end=911
-  _LISTAPPLICATIONSREQUEST_FILTER._serialized_start=384
-  _LISTAPPLICATIONSREQUEST_FILTER._serialized_end=459
-  _LISTAPPLICATIONSREQUEST_SORT._serialized_start=462
-  _LISTAPPLICATIONSREQUEST_SORT._serialized_end=649
-  _LISTAPPLICATIONSREQUEST_ORDERBYFIELD._serialized_start=652
-  _LISTAPPLICATIONSREQUEST_ORDERBYFIELD._serialized_end=809
-  _LISTAPPLICATIONSREQUEST_ORDERDIRECTION._serialized_start=811
-  _LISTAPPLICATIONSREQUEST_ORDERDIRECTION._serialized_end=911
-  _LISTAPPLICATIONSRESPONSE._serialized_start=914
-  _LISTAPPLICATIONSRESPONSE._serialized_end=1060
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=1062
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=1120
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=1122
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=1200
+  _APPLICATIONRAWFIELD._serialized_start=1033
+  _APPLICATIONRAWFIELD._serialized_end=1232
+  _APPLICATIONRAW._serialized_start=100
+  _APPLICATIONRAW._serialized_end=183
+  _APPLICATIONFIELD._serialized_start=185
+  _APPLICATIONFIELD._serialized_end=296
+  _LISTAPPLICATIONSREQUEST._serialized_start=299
+  _LISTAPPLICATIONSREQUEST._serialized_end=741
+  _LISTAPPLICATIONSREQUEST_FILTER._serialized_start=519
+  _LISTAPPLICATIONSREQUEST_FILTER._serialized_end=594
+  _LISTAPPLICATIONSREQUEST_SORT._serialized_start=597
+  _LISTAPPLICATIONSREQUEST_SORT._serialized_end=741
+  _LISTAPPLICATIONSRESPONSE._serialized_start=744
+  _LISTAPPLICATIONSRESPONSE._serialized_end=890
+  _COUNTTASKSBYSTATUSREQUEST._serialized_start=892
+  _COUNTTASKSBYSTATUSREQUEST._serialized_end=950
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=952
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=1030
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 from . import objects_pb2 as _objects_pb2
+from . import sort_direction_pb2 as _sort_direction_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
+APPLICATION_RAW_FIELD_NAME: ApplicationRawField
+APPLICATION_RAW_FIELD_NAMESPACE: ApplicationRawField
+APPLICATION_RAW_FIELD_SERVICE: ApplicationRawField
+APPLICATION_RAW_FIELD_UNSPECIFIED: ApplicationRawField
+APPLICATION_RAW_FIELD_VERSION: ApplicationRawField
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class ApplicationField(_message.Message):
+    __slots__ = ["application_field"]
+    APPLICATION_FIELD_FIELD_NUMBER: _ClassVar[int]
+    application_field: ApplicationRawField
+    def __init__(self, application_field: _Optional[_Union[ApplicationRawField, str]] = ...) -> None: ...
+
 class ApplicationRaw(_message.Message):
     __slots__ = ["name", "namespace", "service", "version"]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     name: str
@@ -31,18 +43,14 @@
     __slots__ = ["status"]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     status: _containers.RepeatedCompositeFieldContainer[_objects_pb2.StatusCount]
     def __init__(self, status: _Optional[_Iterable[_Union[_objects_pb2.StatusCount, _Mapping]]] = ...) -> None: ...
 
 class ListApplicationsRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort"]
-    class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     class Filter(_message.Message):
         __slots__ = ["name", "namespace", "service", "version"]
         NAMESPACE_FIELD_NUMBER: _ClassVar[int]
         NAME_FIELD_NUMBER: _ClassVar[int]
         SERVICE_FIELD_NUMBER: _ClassVar[int]
         VERSION_FIELD_NUMBER: _ClassVar[int]
         name: str
@@ -50,26 +58,18 @@
         service: str
         version: str
         def __init__(self, name: _Optional[str] = ..., version: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "fields"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELDS_FIELD_NUMBER: _ClassVar[int]
-        direction: ListApplicationsRequest.OrderDirection
-        fields: _containers.RepeatedScalarFieldContainer[ListApplicationsRequest.OrderByField]
-        def __init__(self, fields: _Optional[_Iterable[_Union[ListApplicationsRequest.OrderByField, str]]] = ..., direction: _Optional[_Union[ListApplicationsRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: _sort_direction_pb2.SortDirection
+        fields: _containers.RepeatedCompositeFieldContainer[ApplicationField]
+        def __init__(self, fields: _Optional[_Iterable[_Union[ApplicationField, _Mapping]]] = ..., direction: _Optional[_Union[_sort_direction_pb2.SortDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_NAME: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_NAMESPACE: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_SERVICE: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListApplicationsRequest.OrderByField
-    ORDER_BY_FIELD_VERSION: ListApplicationsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListApplicationsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListApplicationsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListApplicationsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     filter: ListApplicationsRequest.Filter
     page: int
     page_size: int
     sort: ListApplicationsRequest.Sort
@@ -82,7 +82,10 @@
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     applications: _containers.RepeatedCompositeFieldContainer[ApplicationRaw]
     page: int
     page_size: int
     total: int
     def __init__(self, applications: _Optional[_Iterable[_Union[ApplicationRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
+
+class ApplicationRawField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from . import sort_direction_pb2 as sort__direction__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17partitions_common.proto\x12\x1e\x61rmonik.api.grpc.v1.partitions\"\xa8\x02\n\x0cPartitionRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1c\n\x14parent_partition_ids\x18\x02 \x03(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x03\x12\x0f\n\x07pod_max\x18\x04 \x01(\x03\x12]\n\x11pod_configuration\x18\x07 \x03(\x0b\x32\x42.armonik.api.grpc.v1.partitions.PartitionRaw.PodConfigurationEntry\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x03\x12\x10\n\x08priority\x18\x06 \x01(\x03\x1a\x37\n\x15PodConfigurationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xec\x06\n\x15ListPartitionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12L\n\x06\x66ilter\x18\x03 \x01(\x0b\x32<.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Filter\x12H\n\x04sort\x18\x04 \x01(\x0b\x32:.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Sort\x1a\x89\x01\n\x06\x46ilter\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1b\n\x13parent_partition_id\x18\x02 \x01(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x05\x12\x0f\n\x07pod_max\x18\x04 \x01(\x05\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x05\x12\x10\n\x08priority\x18\x06 \x01(\x05\x1a\xb2\x01\n\x04Sort\x12Q\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x42.armonik.api.grpc.v1.partitions.ListPartitionsRequest.OrderByField\x12W\n\tdirection\x18\x02 \x01(\x0e\x32\x44.armonik.api.grpc.v1.partitions.ListPartitionsRequest.OrderDirection\"\xf2\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x15\n\x11ORDER_BY_FIELD_ID\x10\x01\x12\'\n#ORDER_BY_FIELD_PARENT_PARTITION_IDS\x10\x02\x12\x1f\n\x1bORDER_BY_FIELD_POD_RESERVED\x10\x03\x12\x1a\n\x16ORDER_BY_FIELD_POD_MAX\x10\x04\x12(\n$ORDER_BY_FIELD_PREEMPTION_PERCENTAGE\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_PRIORITY\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x8a\x01\n\x16ListPartitionsResponse\x12@\n\npartitions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x13GetPartitionRequest\x12\n\n\x02id\x18\x01 \x01(\t\"W\n\x14GetPartitionResponse\x12?\n\tpartition\x18\x01 \x01(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRawB!\xaa\x02\x1e\x41rmonik.Api.Grpc.V1.Partitionsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17partitions_common.proto\x12\x1e\x61rmonik.api.grpc.v1.partitions\x1a\x14sort_direction.proto\"\xa8\x02\n\x0cPartitionRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1c\n\x14parent_partition_ids\x18\x02 \x03(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x03\x12\x0f\n\x07pod_max\x18\x04 \x01(\x03\x12]\n\x11pod_configuration\x18\x07 \x03(\x0b\x32\x42.armonik.api.grpc.v1.partitions.PartitionRaw.PodConfigurationEntry\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x03\x12\x10\n\x08priority\x18\x06 \x01(\x03\x1a\x37\n\x15PodConfigurationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"k\n\x0ePartitionField\x12P\n\x13partition_raw_field\x18\x01 \x01(\x0e\x32\x31.armonik.api.grpc.v1.partitions.PartitionRawFieldH\x00\x42\x07\n\x05\x66ield\"\xea\x03\n\x15ListPartitionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12L\n\x06\x66ilter\x18\x03 \x01(\x0b\x32<.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Filter\x12H\n\x04sort\x18\x04 \x01(\x0b\x32:.armonik.api.grpc.v1.partitions.ListPartitionsRequest.Sort\x1a\x89\x01\n\x06\x46ilter\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1b\n\x13parent_partition_id\x18\x02 \x01(\t\x12\x14\n\x0cpod_reserved\x18\x03 \x01(\x05\x12\x0f\n\x07pod_max\x18\x04 \x01(\x05\x12\x1d\n\x15preemption_percentage\x18\x05 \x01(\x05\x12\x10\n\x08priority\x18\x06 \x01(\x05\x1a\x8b\x01\n\x04Sort\x12=\n\x05\x66ield\x18\x01 \x01(\x0b\x32..armonik.api.grpc.v1.partitions.PartitionField\x12\x44\n\tdirection\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.sort_direction.SortDirection\"\x8a\x01\n\x16ListPartitionsResponse\x12@\n\npartitions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x13GetPartitionRequest\x12\n\n\x02id\x18\x01 \x01(\t\"W\n\x14GetPartitionResponse\x12?\n\tpartition\x18\x01 \x01(\x0b\x32,.armonik.api.grpc.v1.partitions.PartitionRaw*\x9a\x02\n\x11PartitionRawField\x12#\n\x1fPARTITION_RAW_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16PARTITION_RAW_FIELD_ID\x10\x01\x12,\n(PARTITION_RAW_FIELD_PARENT_PARTITION_IDS\x10\x02\x12$\n PARTITION_RAW_FIELD_POD_RESERVED\x10\x03\x12\x1f\n\x1bPARTITION_RAW_FIELD_POD_MAX\x10\x04\x12-\n)PARTITION_RAW_FIELD_PREEMPTION_PERCENTAGE\x10\x05\x12 \n\x1cPARTITION_RAW_FIELD_PRIORITY\x10\x06\x42!\xaa\x02\x1e\x41rmonik.Api.Grpc.V1.Partitionsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'partitions_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\036Armonik.Api.Grpc.V1.Partitions'
   _PARTITIONRAW_PODCONFIGURATIONENTRY._options = None
   _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_options = b'8\001'
-  _PARTITIONRAW._serialized_start=60
-  _PARTITIONRAW._serialized_end=356
-  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_start=301
-  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_end=356
-  _LISTPARTITIONSREQUEST._serialized_start=359
-  _LISTPARTITIONSREQUEST._serialized_end=1235
-  _LISTPARTITIONSREQUEST_FILTER._serialized_start=570
-  _LISTPARTITIONSREQUEST_FILTER._serialized_end=707
-  _LISTPARTITIONSREQUEST_SORT._serialized_start=710
-  _LISTPARTITIONSREQUEST_SORT._serialized_end=888
-  _LISTPARTITIONSREQUEST_ORDERBYFIELD._serialized_start=891
-  _LISTPARTITIONSREQUEST_ORDERBYFIELD._serialized_end=1133
-  _LISTPARTITIONSREQUEST_ORDERDIRECTION._serialized_start=1135
-  _LISTPARTITIONSREQUEST_ORDERDIRECTION._serialized_end=1235
-  _LISTPARTITIONSRESPONSE._serialized_start=1238
-  _LISTPARTITIONSRESPONSE._serialized_end=1376
-  _GETPARTITIONREQUEST._serialized_start=1378
-  _GETPARTITIONREQUEST._serialized_end=1411
-  _GETPARTITIONRESPONSE._serialized_start=1413
-  _GETPARTITIONRESPONSE._serialized_end=1500
+  _PARTITIONRAWFIELD._serialized_start=1248
+  _PARTITIONRAWFIELD._serialized_end=1530
+  _PARTITIONRAW._serialized_start=82
+  _PARTITIONRAW._serialized_end=378
+  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_start=323
+  _PARTITIONRAW_PODCONFIGURATIONENTRY._serialized_end=378
+  _PARTITIONFIELD._serialized_start=380
+  _PARTITIONFIELD._serialized_end=487
+  _LISTPARTITIONSREQUEST._serialized_start=490
+  _LISTPARTITIONSREQUEST._serialized_end=980
+  _LISTPARTITIONSREQUEST_FILTER._serialized_start=701
+  _LISTPARTITIONSREQUEST_FILTER._serialized_end=838
+  _LISTPARTITIONSREQUEST_SORT._serialized_start=841
+  _LISTPARTITIONSREQUEST_SORT._serialized_end=980
+  _LISTPARTITIONSRESPONSE._serialized_start=983
+  _LISTPARTITIONSRESPONSE._serialized_end=1121
+  _GETPARTITIONREQUEST._serialized_start=1123
+  _GETPARTITIONREQUEST._serialized_end=1156
+  _GETPARTITIONRESPONSE._serialized_start=1158
+  _GETPARTITIONRESPONSE._serialized_end=1245
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+from . import sort_direction_pb2 as _sort_direction_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+PARTITION_RAW_FIELD_ID: PartitionRawField
+PARTITION_RAW_FIELD_PARENT_PARTITION_IDS: PartitionRawField
+PARTITION_RAW_FIELD_POD_MAX: PartitionRawField
+PARTITION_RAW_FIELD_POD_RESERVED: PartitionRawField
+PARTITION_RAW_FIELD_PREEMPTION_PERCENTAGE: PartitionRawField
+PARTITION_RAW_FIELD_PRIORITY: PartitionRawField
+PARTITION_RAW_FIELD_UNSPECIFIED: PartitionRawField
 
 class GetPartitionRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: str
     def __init__(self, id: _Optional[str] = ...) -> None: ...
 
@@ -16,18 +24,14 @@
     __slots__ = ["partition"]
     PARTITION_FIELD_NUMBER: _ClassVar[int]
     partition: PartitionRaw
     def __init__(self, partition: _Optional[_Union[PartitionRaw, _Mapping]] = ...) -> None: ...
 
 class ListPartitionsRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort"]
-    class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     class Filter(_message.Message):
         __slots__ = ["id", "parent_partition_id", "pod_max", "pod_reserved", "preemption_percentage", "priority"]
         ID_FIELD_NUMBER: _ClassVar[int]
         PARENT_PARTITION_ID_FIELD_NUMBER: _ClassVar[int]
         POD_MAX_FIELD_NUMBER: _ClassVar[int]
         POD_RESERVED_FIELD_NUMBER: _ClassVar[int]
         PREEMPTION_PERCENTAGE_FIELD_NUMBER: _ClassVar[int]
@@ -39,28 +43,18 @@
         preemption_percentage: int
         priority: int
         def __init__(self, id: _Optional[str] = ..., parent_partition_id: _Optional[str] = ..., pod_reserved: _Optional[int] = ..., pod_max: _Optional[int] = ..., preemption_percentage: _Optional[int] = ..., priority: _Optional[int] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "field"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListPartitionsRequest.OrderDirection
-        field: ListPartitionsRequest.OrderByField
-        def __init__(self, field: _Optional[_Union[ListPartitionsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListPartitionsRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: _sort_direction_pb2.SortDirection
+        field: PartitionField
+        def __init__(self, field: _Optional[_Union[PartitionField, _Mapping]] = ..., direction: _Optional[_Union[_sort_direction_pb2.SortDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_ID: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PARENT_PARTITION_IDS: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_POD_MAX: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_POD_RESERVED: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PREEMPTION_PERCENTAGE: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_PRIORITY: ListPartitionsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListPartitionsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListPartitionsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListPartitionsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListPartitionsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     filter: ListPartitionsRequest.Filter
     page: int
     page_size: int
     sort: ListPartitionsRequest.Sort
@@ -74,14 +68,20 @@
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     page: int
     page_size: int
     partitions: _containers.RepeatedCompositeFieldContainer[PartitionRaw]
     total: int
     def __init__(self, partitions: _Optional[_Iterable[_Union[PartitionRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
+class PartitionField(_message.Message):
+    __slots__ = ["partition_raw_field"]
+    PARTITION_RAW_FIELD_FIELD_NUMBER: _ClassVar[int]
+    partition_raw_field: PartitionRawField
+    def __init__(self, partition_raw_field: _Optional[_Union[PartitionRawField, str]] = ...) -> None: ...
+
 class PartitionRaw(_message.Message):
     __slots__ = ["id", "parent_partition_ids", "pod_configuration", "pod_max", "pod_reserved", "preemption_percentage", "priority"]
     class PodConfigurationEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
@@ -98,7 +98,10 @@
     parent_partition_ids: _containers.RepeatedScalarFieldContainer[str]
     pod_configuration: _containers.ScalarMap[str, str]
     pod_max: int
     pod_reserved: int
     preemption_percentage: int
     priority: int
     def __init__(self, id: _Optional[str] = ..., parent_partition_ids: _Optional[_Iterable[str]] = ..., pod_reserved: _Optional[int] = ..., pod_max: _Optional[int] = ..., pod_configuration: _Optional[_Mapping[str, str]] = ..., preemption_percentage: _Optional[int] = ..., priority: _Optional[int] = ...) -> None: ...
+
+class PartitionRawField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/results_common_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,70 +9,71 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import result_status_pb2 as result__status__pb2
+from . import sort_direction_pb2 as sort__direction__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14results_common.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13result_status.proto\"\xb0\x02\n\tResultRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10wait_for_data_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x08 \x01(\t\"\x90\t\n\x12ListResultsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x46\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x36.armonik.api.grpc.v1.results.ListResultsRequest.Filter\x12\x42\n\x04sort\x18\x04 \x01(\x0b\x32\x34.armonik.api.grpc.v1.results.ListResultsRequest.Sort\x1a\xda\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x31\n\rcreated_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63ompleted_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63ompleted_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13wait_for_data_after\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14wait_for_data_before\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x0b \x01(\t\x1a\xa6\x01\n\x04Sort\x12K\n\x05\x66ield\x18\x01 \x01(\x0e\x32<.armonik.api.grpc.v1.results.ListResultsRequest.OrderByField\x12Q\n\tdirection\x18\x02 \x01(\x0e\x32>.armonik.api.grpc.v1.results.ListResultsRequest.OrderDirection\"\xe0\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x17\n\x13ORDER_BY_FIELD_NAME\x10\x02\x12 \n\x1cORDER_BY_FIELD_OWNER_TASK_ID\x10\x03\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x05\x12\x1c\n\x18ORDER_BY_FIELD_RESULT_ID\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"~\n\x13ListResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"%\n\x10GetResultRequest\x12\x11\n\tresult_id\x18\x01 \x01(\t\"K\n\x11GetResultResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\">\n\x15GetOwnerTaskIdRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"\xb9\x01\n\x16GetOwnerTaskIdResponse\x12V\n\x0bresult_task\x18\x01 \x03(\x0b\x32\x41.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse.MapResultTask\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x33\n\rMapResultTask\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\xa9\x01\n\x1c\x43reateResultsMetaDataRequest\x12W\n\x07results\x18\x01 \x03(\x0b\x32\x46.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"X\n\x1d\x43reateResultsMetaDataResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xa7\x01\n\x14\x43reateResultsRequest\x12O\n\x07results\x18\x01 \x03(\x0b\x32>.armonik.api.grpc.v1.results.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"P\n\x15\x43reateResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xc7\x01\n\x17UploadResultDataRequest\x12S\n\x02id\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.results.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"R\n\x18UploadResultDataResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"B\n#ResultsServiceConfigurationResponse\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"B\n\x19\x44ownloadResultDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"0\n\x1a\x44ownloadResultDataResponse\x12\x12\n\ndata_chunk\x18\x01 \x01(\x0c\"A\n\x18\x44\x65leteResultsDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"B\n\x19\x44\x65leteResultsDataResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\tB\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14results_common.proto\x12\x1b\x61rmonik.api.grpc.v1.results\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x13result_status.proto\x1a\x14sort_direction.proto\"\xfa\x01\n\tResultRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x08 \x01(\t\"_\n\x0bResultField\x12G\n\x10result_raw_field\x18\x01 \x01(\x0e\x32+.armonik.api.grpc.v1.results.ResultRawFieldH\x00\x42\x07\n\x05\x66ield\"\xa6\x06\n\x12ListResultsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x46\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x36.armonik.api.grpc.v1.results.ListResultsRequest.Filter\x12\x42\n\x04sort\x18\x04 \x01(\x0b\x32\x34.armonik.api.grpc.v1.results.ListResultsRequest.Sort\x1a\xda\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rowner_task_id\x18\x03 \x01(\t\x12?\n\x06status\x18\x04 \x01(\x0e\x32/.armonik.api.grpc.v1.result_status.ResultStatus\x12\x31\n\rcreated_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63ompleted_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63ompleted_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x13wait_for_data_after\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14wait_for_data_before\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tresult_id\x18\x0b \x01(\t\x1a\x85\x01\n\x04Sort\x12\x37\n\x05\x66ield\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.results.ResultField\x12\x44\n\tdirection\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.sort_direction.SortDirection\"~\n\x13ListResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"%\n\x10GetResultRequest\x12\x11\n\tresult_id\x18\x01 \x01(\t\"K\n\x11GetResultResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\">\n\x15GetOwnerTaskIdRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"\xb9\x01\n\x16GetOwnerTaskIdResponse\x12V\n\x0bresult_task\x18\x01 \x03(\x0b\x32\x41.armonik.api.grpc.v1.results.GetOwnerTaskIdResponse.MapResultTask\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x33\n\rMapResultTask\x12\x11\n\tresult_id\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\t\"\xa9\x01\n\x1c\x43reateResultsMetaDataRequest\x12W\n\x07results\x18\x01 \x03(\x0b\x32\x46.armonik.api.grpc.v1.results.CreateResultsMetaDataRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a\x1c\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\"X\n\x1d\x43reateResultsMetaDataResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xa7\x01\n\x14\x43reateResultsRequest\x12O\n\x07results\x18\x01 \x03(\x0b\x32>.armonik.api.grpc.v1.results.CreateResultsRequest.ResultCreate\x12\x12\n\nsession_id\x18\x02 \x01(\t\x1a*\n\x0cResultCreate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"P\n\x15\x43reateResultsResponse\x12\x37\n\x07results\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"\xc7\x01\n\x17UploadResultDataRequest\x12S\n\x02id\x18\x01 \x01(\x0b\x32\x45.armonik.api.grpc.v1.results.UploadResultDataRequest.ResultIdentifierH\x00\x12\x14\n\ndata_chunk\x18\x02 \x01(\x0cH\x00\x1a\x39\n\x10ResultIdentifier\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\tB\x06\n\x04type\"R\n\x18UploadResultDataResponse\x12\x36\n\x06result\x18\x01 \x01(\x0b\x32&.armonik.api.grpc.v1.results.ResultRaw\"B\n#ResultsServiceConfigurationResponse\x12\x1b\n\x13\x64\x61ta_chunk_max_size\x18\x01 \x01(\x05\"B\n\x19\x44ownloadResultDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x01(\t\"0\n\x1a\x44ownloadResultDataResponse\x12\x12\n\ndata_chunk\x18\x01 \x01(\x0c\"A\n\x18\x44\x65leteResultsDataRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t\"B\n\x19\x44\x65leteResultsDataResponse\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tresult_id\x18\x02 \x03(\t*\x93\x02\n\x0eResultRawField\x12 \n\x1cRESULT_RAW_FIELD_UNSPECIFIED\x10\x00\x12\x1f\n\x1bRESULT_RAW_FIELD_SESSION_ID\x10\x01\x12\x19\n\x15RESULT_RAW_FIELD_NAME\x10\x02\x12\"\n\x1eRESULT_RAW_FIELD_OWNER_TASK_ID\x10\x03\x12\x1b\n\x17RESULT_RAW_FIELD_STATUS\x10\x04\x12\x1f\n\x1bRESULT_RAW_FIELD_CREATED_AT\x10\x05\x12!\n\x1dRESULT_RAW_FIELD_COMPLETED_AT\x10\x06\x12\x1e\n\x1aRESULT_RAW_FIELD_RESULT_ID\x10\x07\x42\x1e\xaa\x02\x1b\x41rmoniK.Api.gRPC.V1.Resultsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'results_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\033ArmoniK.Api.gRPC.V1.Results'
-  _RESULTRAW._serialized_start=108
-  _RESULTRAW._serialized_end=412
-  _LISTRESULTSREQUEST._serialized_start=415
-  _LISTRESULTSREQUEST._serialized_end=1583
-  _LISTRESULTSREQUEST_FILTER._serialized_start=611
-  _LISTRESULTSREQUEST_FILTER._serialized_end=1085
-  _LISTRESULTSREQUEST_SORT._serialized_start=1088
-  _LISTRESULTSREQUEST_SORT._serialized_end=1254
-  _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_start=1257
-  _LISTRESULTSREQUEST_ORDERBYFIELD._serialized_end=1481
-  _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_start=1483
-  _LISTRESULTSREQUEST_ORDERDIRECTION._serialized_end=1583
-  _LISTRESULTSRESPONSE._serialized_start=1585
-  _LISTRESULTSRESPONSE._serialized_end=1711
-  _GETRESULTREQUEST._serialized_start=1713
-  _GETRESULTREQUEST._serialized_end=1750
-  _GETRESULTRESPONSE._serialized_start=1752
-  _GETRESULTRESPONSE._serialized_end=1827
-  _GETOWNERTASKIDREQUEST._serialized_start=1829
-  _GETOWNERTASKIDREQUEST._serialized_end=1891
-  _GETOWNERTASKIDRESPONSE._serialized_start=1894
-  _GETOWNERTASKIDRESPONSE._serialized_end=2079
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_start=2028
-  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_end=2079
-  _CREATERESULTSMETADATAREQUEST._serialized_start=2082
-  _CREATERESULTSMETADATAREQUEST._serialized_end=2251
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=2223
-  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=2251
-  _CREATERESULTSMETADATARESPONSE._serialized_start=2253
-  _CREATERESULTSMETADATARESPONSE._serialized_end=2341
-  _CREATERESULTSREQUEST._serialized_start=2344
-  _CREATERESULTSREQUEST._serialized_end=2511
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2469
-  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2511
-  _CREATERESULTSRESPONSE._serialized_start=2513
-  _CREATERESULTSRESPONSE._serialized_end=2593
-  _UPLOADRESULTDATAREQUEST._serialized_start=2596
-  _UPLOADRESULTDATAREQUEST._serialized_end=2795
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=2730
-  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=2787
-  _UPLOADRESULTDATARESPONSE._serialized_start=2797
-  _UPLOADRESULTDATARESPONSE._serialized_end=2879
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_start=2881
-  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_end=2947
-  _DOWNLOADRESULTDATAREQUEST._serialized_start=2949
-  _DOWNLOADRESULTDATAREQUEST._serialized_end=3015
-  _DOWNLOADRESULTDATARESPONSE._serialized_start=3017
-  _DOWNLOADRESULTDATARESPONSE._serialized_end=3065
-  _DELETERESULTSDATAREQUEST._serialized_start=3067
-  _DELETERESULTSDATAREQUEST._serialized_end=3132
-  _DELETERESULTSDATARESPONSE._serialized_start=3134
-  _DELETERESULTSDATARESPONSE._serialized_end=3200
+  _RESULTRAWFIELD._serialized_start=2906
+  _RESULTRAWFIELD._serialized_end=3181
+  _RESULTRAW._serialized_start=130
+  _RESULTRAW._serialized_end=380
+  _RESULTFIELD._serialized_start=382
+  _RESULTFIELD._serialized_end=477
+  _LISTRESULTSREQUEST._serialized_start=480
+  _LISTRESULTSREQUEST._serialized_end=1286
+  _LISTRESULTSREQUEST_FILTER._serialized_start=676
+  _LISTRESULTSREQUEST_FILTER._serialized_end=1150
+  _LISTRESULTSREQUEST_SORT._serialized_start=1153
+  _LISTRESULTSREQUEST_SORT._serialized_end=1286
+  _LISTRESULTSRESPONSE._serialized_start=1288
+  _LISTRESULTSRESPONSE._serialized_end=1414
+  _GETRESULTREQUEST._serialized_start=1416
+  _GETRESULTREQUEST._serialized_end=1453
+  _GETRESULTRESPONSE._serialized_start=1455
+  _GETRESULTRESPONSE._serialized_end=1530
+  _GETOWNERTASKIDREQUEST._serialized_start=1532
+  _GETOWNERTASKIDREQUEST._serialized_end=1594
+  _GETOWNERTASKIDRESPONSE._serialized_start=1597
+  _GETOWNERTASKIDRESPONSE._serialized_end=1782
+  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_start=1731
+  _GETOWNERTASKIDRESPONSE_MAPRESULTTASK._serialized_end=1782
+  _CREATERESULTSMETADATAREQUEST._serialized_start=1785
+  _CREATERESULTSMETADATAREQUEST._serialized_end=1954
+  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_start=1926
+  _CREATERESULTSMETADATAREQUEST_RESULTCREATE._serialized_end=1954
+  _CREATERESULTSMETADATARESPONSE._serialized_start=1956
+  _CREATERESULTSMETADATARESPONSE._serialized_end=2044
+  _CREATERESULTSREQUEST._serialized_start=2047
+  _CREATERESULTSREQUEST._serialized_end=2214
+  _CREATERESULTSREQUEST_RESULTCREATE._serialized_start=2172
+  _CREATERESULTSREQUEST_RESULTCREATE._serialized_end=2214
+  _CREATERESULTSRESPONSE._serialized_start=2216
+  _CREATERESULTSRESPONSE._serialized_end=2296
+  _UPLOADRESULTDATAREQUEST._serialized_start=2299
+  _UPLOADRESULTDATAREQUEST._serialized_end=2498
+  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_start=2433
+  _UPLOADRESULTDATAREQUEST_RESULTIDENTIFIER._serialized_end=2490
+  _UPLOADRESULTDATARESPONSE._serialized_start=2500
+  _UPLOADRESULTDATARESPONSE._serialized_end=2582
+  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_start=2584
+  _RESULTSSERVICECONFIGURATIONRESPONSE._serialized_end=2650
+  _DOWNLOADRESULTDATAREQUEST._serialized_start=2652
+  _DOWNLOADRESULTDATAREQUEST._serialized_end=2718
+  _DOWNLOADRESULTDATARESPONSE._serialized_start=2720
+  _DOWNLOADRESULTDATARESPONSE._serialized_end=2768
+  _DELETERESULTSDATAREQUEST._serialized_start=2770
+  _DELETERESULTSDATAREQUEST._serialized_end=2835
+  _DELETERESULTSDATARESPONSE._serialized_start=2837
+  _DELETERESULTSDATARESPONSE._serialized_end=2903
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from . import result_status_pb2 as _result_status_pb2
+from . import sort_direction_pb2 as _sort_direction_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+RESULT_RAW_FIELD_COMPLETED_AT: ResultRawField
+RESULT_RAW_FIELD_CREATED_AT: ResultRawField
+RESULT_RAW_FIELD_NAME: ResultRawField
+RESULT_RAW_FIELD_OWNER_TASK_ID: ResultRawField
+RESULT_RAW_FIELD_RESULT_ID: ResultRawField
+RESULT_RAW_FIELD_SESSION_ID: ResultRawField
+RESULT_RAW_FIELD_STATUS: ResultRawField
+RESULT_RAW_FIELD_UNSPECIFIED: ResultRawField
 
 class CreateResultsMetaDataRequest(_message.Message):
     __slots__ = ["results", "session_id"]
     class ResultCreate(_message.Message):
         __slots__ = ["name"]
         NAME_FIELD_NUMBER: _ClassVar[int]
         name: str
@@ -111,18 +120,14 @@
     __slots__ = ["result"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     result: ResultRaw
     def __init__(self, result: _Optional[_Union[ResultRaw, _Mapping]] = ...) -> None: ...
 
 class ListResultsRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort"]
-    class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     class Filter(_message.Message):
         __slots__ = ["completed_after", "completed_before", "created_after", "created_before", "name", "owner_task_id", "result_id", "session_id", "status", "wait_for_data_after", "wait_for_data_before"]
         COMPLETED_AFTER_FIELD_NUMBER: _ClassVar[int]
         COMPLETED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         NAME_FIELD_NUMBER: _ClassVar[int]
@@ -144,28 +149,18 @@
         wait_for_data_after: _timestamp_pb2.Timestamp
         wait_for_data_before: _timestamp_pb2.Timestamp
         def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "field"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListResultsRequest.OrderDirection
-        field: ListResultsRequest.OrderByField
-        def __init__(self, field: _Optional[_Union[ListResultsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListResultsRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: _sort_direction_pb2.SortDirection
+        field: ResultField
+        def __init__(self, field: _Optional[_Union[ResultField, _Mapping]] = ..., direction: _Optional[_Union[_sort_direction_pb2.SortDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CREATED_AT: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_NAME: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_OWNER_TASK_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_RESULT_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListResultsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListResultsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListResultsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListResultsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     filter: ListResultsRequest.Filter
     page: int
     page_size: int
     sort: ListResultsRequest.Sort
@@ -179,33 +174,37 @@
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     page: int
     page_size: int
     results: _containers.RepeatedCompositeFieldContainer[ResultRaw]
     total: int
     def __init__(self, results: _Optional[_Iterable[_Union[ResultRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
+class ResultField(_message.Message):
+    __slots__ = ["result_raw_field"]
+    RESULT_RAW_FIELD_FIELD_NUMBER: _ClassVar[int]
+    result_raw_field: ResultRawField
+    def __init__(self, result_raw_field: _Optional[_Union[ResultRawField, str]] = ...) -> None: ...
+
 class ResultRaw(_message.Message):
-    __slots__ = ["completed_at", "created_at", "name", "owner_task_id", "result_id", "session_id", "status", "wait_for_data_at"]
+    __slots__ = ["completed_at", "created_at", "name", "owner_task_id", "result_id", "session_id", "status"]
     COMPLETED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     OWNER_TASK_ID_FIELD_NUMBER: _ClassVar[int]
     RESULT_ID_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
-    WAIT_FOR_DATA_AT_FIELD_NUMBER: _ClassVar[int]
     completed_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
     name: str
     owner_task_id: str
     result_id: str
     session_id: str
     status: _result_status_pb2.ResultStatus
-    wait_for_data_at: _timestamp_pb2.Timestamp
-    def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., wait_for_data_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ..., name: _Optional[str] = ..., owner_task_id: _Optional[str] = ..., status: _Optional[_Union[_result_status_pb2.ResultStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., completed_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., result_id: _Optional[str] = ...) -> None: ...
 
 class ResultsServiceConfigurationResponse(_message.Message):
     __slots__ = ["data_chunk_max_size"]
     DATA_CHUNK_MAX_SIZE_FIELD_NUMBER: _ClassVar[int]
     data_chunk_max_size: int
     def __init__(self, data_chunk_max_size: _Optional[int] = ...) -> None: ...
 
@@ -225,7 +224,10 @@
     def __init__(self, id: _Optional[_Union[UploadResultDataRequest.ResultIdentifier, _Mapping]] = ..., data_chunk: _Optional[bytes] = ...) -> None: ...
 
 class UploadResultDataResponse(_message.Message):
     __slots__ = ["result"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     result: ResultRaw
     def __init__(self, result: _Optional[_Union[ResultRaw, _Mapping]] = ...) -> None: ...
+
+class ResultRawField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,44 +11,45 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import session_status_pb2 as session__status__pb2
+from . import sort_direction_pb2 as sort__direction__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15sessions_common.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x14session_status.proto\"\xbc\x02\n\nSessionRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12\x15\n\rpartition_ids\x18\x03 \x03(\t\x12\x31\n\x07options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x8a\x08\n\x13ListSessionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12H\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x38.armonik.api.grpc.v1.sessions.ListSessionsRequest.Filter\x12\x44\n\x04sort\x18\x04 \x01(\x0b\x32\x36.armonik.api.grpc.v1.sessions.ListSessionsRequest.Sort\x12\x19\n\x11with_task_options\x18\x05 \x01(\x08\x1a\xe8\x02\n\x06\x46ilter\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x02 \x01(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x31\n\rcreated_after\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63\x61ncelled_after\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63\x61ncelled_before\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x08 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x1a\xaa\x01\n\x04Sort\x12M\n\x05\x66ield\x18\x01 \x01(\x0e\x32>.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderByField\x12S\n\tdirection\x18\x02 \x01(\x0e\x32@.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderDirection\"\xa8\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x02\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x03\x12\x1f\n\x1bORDER_BY_FIELD_CANCELLED_AT\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x82\x01\n\x14ListSessionsResponse\x12:\n\x08sessions\x18\x01 \x03(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"\'\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"O\n\x12GetSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"*\n\x14\x43\x61ncelSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"R\n\x15\x43\x61ncelSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"/\n\x19\x43ountTasksByStatusRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15sessions_common.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x14session_status.proto\x1a\x14sort_direction.proto\"\xbc\x02\n\nSessionRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12\x15\n\rpartition_ids\x18\x03 \x03(\t\x12\x31\n\x07options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\"c\n\x0cSessionField\x12J\n\x11session_raw_field\x18\x01 \x01(\x0e\x32-.armonik.api.grpc.v1.sessions.SessionRawFieldH\x00\x42\x07\n\x05\x66ield\"\xd6\x05\n\x13ListSessionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12H\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x38.armonik.api.grpc.v1.sessions.ListSessionsRequest.Filter\x12\x44\n\x04sort\x18\x04 \x01(\x0b\x32\x36.armonik.api.grpc.v1.sessions.ListSessionsRequest.Sort\x12\x19\n\x11with_task_options\x18\x05 \x01(\x08\x1a\xe8\x02\n\x06\x46ilter\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x02 \x01(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x31\n\rcreated_after\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63\x61ncelled_after\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63\x61ncelled_before\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x08 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x1a\x87\x01\n\x04Sort\x12\x39\n\x05\x66ield\x18\x01 \x01(\x0b\x32*.armonik.api.grpc.v1.sessions.SessionField\x12\x44\n\tdirection\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.sort_direction.SortDirection\"\x82\x01\n\x14ListSessionsResponse\x12:\n\x08sessions\x18\x01 \x03(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"\'\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"O\n\x12GetSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"*\n\x14\x43\x61ncelSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"R\n\x15\x43\x61ncelSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"/\n\x19\x43ountTasksByStatusRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount*\x9e\x02\n\x0fSessionRawField\x12!\n\x1dSESSION_RAW_FIELD_UNSPECIFIED\x10\x00\x12 \n\x1cSESSION_RAW_FIELD_SESSION_ID\x10\x01\x12\x1c\n\x18SESSION_RAW_FIELD_STATUS\x10\x02\x12#\n\x1fSESSION_RAW_FIELD_PARTITION_IDS\x10\x03\x12\x1d\n\x19SESSION_RAW_FIELD_OPTIONS\x10\x04\x12 \n\x1cSESSION_RAW_FIELD_CREATED_AT\x10\x05\x12\"\n\x1eSESSION_RAW_FIELD_CANCELLED_AT\x10\x06\x12\x1e\n\x1aSESSION_RAW_FIELD_DURATION\x10\x07\x42\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\034ArmoniK.Api.gRPC.V1.Sessions'
-  _SESSIONRAW._serialized_start=158
-  _SESSIONRAW._serialized_end=474
-  _LISTSESSIONSREQUEST._serialized_start=477
-  _LISTSESSIONSREQUEST._serialized_end=1511
-  _LISTSESSIONSREQUEST_FILTER._serialized_start=705
-  _LISTSESSIONSREQUEST_FILTER._serialized_end=1065
-  _LISTSESSIONSREQUEST_SORT._serialized_start=1068
-  _LISTSESSIONSREQUEST_SORT._serialized_end=1238
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_start=1241
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_end=1409
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_start=1411
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_end=1511
-  _LISTSESSIONSRESPONSE._serialized_start=1514
-  _LISTSESSIONSRESPONSE._serialized_end=1644
-  _GETSESSIONREQUEST._serialized_start=1646
-  _GETSESSIONREQUEST._serialized_end=1685
-  _GETSESSIONRESPONSE._serialized_start=1687
-  _GETSESSIONRESPONSE._serialized_end=1766
-  _CANCELSESSIONREQUEST._serialized_start=1768
-  _CANCELSESSIONREQUEST._serialized_end=1810
-  _CANCELSESSIONRESPONSE._serialized_start=1812
-  _CANCELSESSIONRESPONSE._serialized_end=1894
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=1896
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=1943
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=1945
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=2023
+  _SESSIONRAWFIELD._serialized_start=1841
+  _SESSIONRAWFIELD._serialized_end=2127
+  _SESSIONRAW._serialized_start=180
+  _SESSIONRAW._serialized_end=496
+  _SESSIONFIELD._serialized_start=498
+  _SESSIONFIELD._serialized_end=597
+  _LISTSESSIONSREQUEST._serialized_start=600
+  _LISTSESSIONSREQUEST._serialized_end=1326
+  _LISTSESSIONSREQUEST_FILTER._serialized_start=828
+  _LISTSESSIONSREQUEST_FILTER._serialized_end=1188
+  _LISTSESSIONSREQUEST_SORT._serialized_start=1191
+  _LISTSESSIONSREQUEST_SORT._serialized_end=1326
+  _LISTSESSIONSRESPONSE._serialized_start=1329
+  _LISTSESSIONSRESPONSE._serialized_end=1459
+  _GETSESSIONREQUEST._serialized_start=1461
+  _GETSESSIONREQUEST._serialized_end=1500
+  _GETSESSIONRESPONSE._serialized_start=1502
+  _GETSESSIONRESPONSE._serialized_end=1581
+  _CANCELSESSIONREQUEST._serialized_start=1583
+  _CANCELSESSIONREQUEST._serialized_end=1625
+  _CANCELSESSIONRESPONSE._serialized_start=1627
+  _CANCELSESSIONRESPONSE._serialized_end=1709
+  _COUNTTASKSBYSTATUSREQUEST._serialized_start=1711
+  _COUNTTASKSBYSTATUSREQUEST._serialized_end=1758
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=1760
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=1838
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from . import objects_pb2 as _objects_pb2
 from . import session_status_pb2 as _session_status_pb2
+from . import sort_direction_pb2 as _sort_direction_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+SESSION_RAW_FIELD_CANCELLED_AT: SessionRawField
+SESSION_RAW_FIELD_CREATED_AT: SessionRawField
+SESSION_RAW_FIELD_DURATION: SessionRawField
+SESSION_RAW_FIELD_OPTIONS: SessionRawField
+SESSION_RAW_FIELD_PARTITION_IDS: SessionRawField
+SESSION_RAW_FIELD_SESSION_ID: SessionRawField
+SESSION_RAW_FIELD_STATUS: SessionRawField
+SESSION_RAW_FIELD_UNSPECIFIED: SessionRawField
 
 class CancelSessionRequest(_message.Message):
     __slots__ = ["session_id"]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     session_id: str
     def __init__(self, session_id: _Optional[str] = ...) -> None: ...
 
@@ -44,18 +53,14 @@
     __slots__ = ["session"]
     SESSION_FIELD_NUMBER: _ClassVar[int]
     session: SessionRaw
     def __init__(self, session: _Optional[_Union[SessionRaw, _Mapping]] = ...) -> None: ...
 
 class ListSessionsRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort", "with_task_options"]
-    class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     class Filter(_message.Message):
         __slots__ = ["application_name", "application_version", "cancelled_after", "cancelled_before", "created_after", "created_before", "session_id", "status"]
         APPLICATION_NAME_FIELD_NUMBER: _ClassVar[int]
         APPLICATION_VERSION_FIELD_NUMBER: _ClassVar[int]
         CANCELLED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CANCELLED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
@@ -71,26 +76,18 @@
         session_id: str
         status: _session_status_pb2.SessionStatus
         def __init__(self, application_name: _Optional[str] = ..., application_version: _Optional[str] = ..., session_id: _Optional[str] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "field"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListSessionsRequest.OrderDirection
-        field: ListSessionsRequest.OrderByField
-        def __init__(self, field: _Optional[_Union[ListSessionsRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListSessionsRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: _sort_direction_pb2.SortDirection
+        field: SessionField
+        def __init__(self, field: _Optional[_Union[SessionField, _Mapping]] = ..., direction: _Optional[_Union[_sort_direction_pb2.SortDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CANCELLED_AT: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_CREATED_AT: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListSessionsRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListSessionsRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListSessionsRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListSessionsRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListSessionsRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     WITH_TASK_OPTIONS_FIELD_NUMBER: _ClassVar[int]
     filter: ListSessionsRequest.Filter
     page: int
     page_size: int
@@ -106,14 +103,20 @@
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     page: int
     page_size: int
     sessions: _containers.RepeatedCompositeFieldContainer[SessionRaw]
     total: int
     def __init__(self, sessions: _Optional[_Iterable[_Union[SessionRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
+class SessionField(_message.Message):
+    __slots__ = ["session_raw_field"]
+    SESSION_RAW_FIELD_FIELD_NUMBER: _ClassVar[int]
+    session_raw_field: SessionRawField
+    def __init__(self, session_raw_field: _Optional[_Union[SessionRawField, str]] = ...) -> None: ...
+
 class SessionRaw(_message.Message):
     __slots__ = ["cancelled_at", "created_at", "duration", "options", "partition_ids", "session_id", "status"]
     CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     DURATION_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
@@ -123,7 +126,10 @@
     created_at: _timestamp_pb2.Timestamp
     duration: _duration_pb2.Duration
     options: _objects_pb2.TaskOptions
     partition_ids: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
     status: _session_status_pb2.SessionStatus
     def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
+
+class SessionRawField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,46 @@
 from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from . import objects_pb2 as _objects_pb2
+from . import sort_direction_pb2 as _sort_direction_pb2
 from . import task_status_pb2 as _task_status_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
+TASK_OPTION_FIELD_APPLICATION_NAME: TaskOptionField
+TASK_OPTION_FIELD_APPLICATION_NAMESPACE: TaskOptionField
+TASK_OPTION_FIELD_APPLICATION_SERVICE: TaskOptionField
+TASK_OPTION_FIELD_APPLICATION_VERSION: TaskOptionField
+TASK_OPTION_FIELD_ENGINE_TYPE: TaskOptionField
+TASK_OPTION_FIELD_MAX_DURATION: TaskOptionField
+TASK_OPTION_FIELD_MAX_RETRIES: TaskOptionField
+TASK_OPTION_FIELD_PARTITION_ID: TaskOptionField
+TASK_OPTION_FIELD_PRIORITY: TaskOptionField
+TASK_OPTION_FIELD_UNSPECIFIED: TaskOptionField
+TASK_SUMMARY_FIELD_ACQUIRED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_CREATED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_CREATION_TO_END_DURATION: TaskSummaryField
+TASK_SUMMARY_FIELD_ENDED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_ERROR: TaskSummaryField
+TASK_SUMMARY_FIELD_INITIAL_TASK_ID: TaskSummaryField
+TASK_SUMMARY_FIELD_OWNER_POD_ID: TaskSummaryField
+TASK_SUMMARY_FIELD_POD_HOSTNAME: TaskSummaryField
+TASK_SUMMARY_FIELD_POD_TTL: TaskSummaryField
+TASK_SUMMARY_FIELD_PROCESSING_TO_END_DURATION: TaskSummaryField
+TASK_SUMMARY_FIELD_RECEIVED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_SESSION_ID: TaskSummaryField
+TASK_SUMMARY_FIELD_STARTED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_STATUS: TaskSummaryField
+TASK_SUMMARY_FIELD_SUBMITTED_AT: TaskSummaryField
+TASK_SUMMARY_FIELD_TASK_ID: TaskSummaryField
+TASK_SUMMARY_FIELD_UNSPECIFIED: TaskSummaryField
 
 class CancelTasksRequest(_message.Message):
     __slots__ = ["task_ids"]
     TASK_IDS_FIELD_NUMBER: _ClassVar[int]
     task_ids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, task_ids: _Optional[_Iterable[str]] = ...) -> None: ...
 
@@ -73,18 +101,14 @@
     page_size: int
     tasks: _containers.RepeatedCompositeFieldContainer[TaskRaw]
     total: int
     def __init__(self, tasks: _Optional[_Iterable[_Union[TaskRaw, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
 class ListTasksRequest(_message.Message):
     __slots__ = ["filter", "page", "page_size", "sort", "with_errors"]
-    class OrderByField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    class OrderDirection(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
     class Filter(_message.Message):
         __slots__ = ["created_after", "created_before", "ended_after", "ended_before", "session_id", "started_after", "started_before", "status"]
         CREATED_AFTER_FIELD_NUMBER: _ClassVar[int]
         CREATED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         ENDED_AFTER_FIELD_NUMBER: _ClassVar[int]
         ENDED_BEFORE_FIELD_NUMBER: _ClassVar[int]
         SESSION_ID_FIELD_NUMBER: _ClassVar[int]
@@ -100,28 +124,18 @@
         started_before: _timestamp_pb2.Timestamp
         status: _containers.RepeatedScalarFieldContainer[_task_status_pb2.TaskStatus]
         def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Iterable[_Union[_task_status_pb2.TaskStatus, str]]] = ..., created_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., created_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_after: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_before: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
     class Sort(_message.Message):
         __slots__ = ["direction", "field"]
         DIRECTION_FIELD_NUMBER: _ClassVar[int]
         FIELD_FIELD_NUMBER: _ClassVar[int]
-        direction: ListTasksRequest.OrderDirection
-        field: ListTasksRequest.OrderByField
-        def __init__(self, field: _Optional[_Union[ListTasksRequest.OrderByField, str]] = ..., direction: _Optional[_Union[ListTasksRequest.OrderDirection, str]] = ...) -> None: ...
+        direction: _sort_direction_pb2.SortDirection
+        field: TaskField
+        def __init__(self, field: _Optional[_Union[TaskField, _Mapping]] = ..., direction: _Optional[_Union[_sort_direction_pb2.SortDirection, str]] = ...) -> None: ...
     FILTER_FIELD_NUMBER: _ClassVar[int]
-    ORDER_BY_FIELD_CREATED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_ENDED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_SESSION_ID: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_STARTED_AT: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_STATUS: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_TASK_ID: ListTasksRequest.OrderByField
-    ORDER_BY_FIELD_UNSPECIFIED: ListTasksRequest.OrderByField
-    ORDER_DIRECTION_ASC: ListTasksRequest.OrderDirection
-    ORDER_DIRECTION_DESC: ListTasksRequest.OrderDirection
-    ORDER_DIRECTION_UNSPECIFIED: ListTasksRequest.OrderDirection
     PAGE_FIELD_NUMBER: _ClassVar[int]
     PAGE_SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     WITH_ERRORS_FIELD_NUMBER: _ClassVar[int]
     filter: ListTasksRequest.Filter
     page: int
     page_size: int
@@ -175,14 +189,30 @@
         payload_id: str
         task_id: str
         def __init__(self, task_id: _Optional[str] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     TASK_INFOS_FIELD_NUMBER: _ClassVar[int]
     task_infos: _containers.RepeatedCompositeFieldContainer[SubmitTasksResponse.TaskInfo]
     def __init__(self, task_infos: _Optional[_Iterable[_Union[SubmitTasksResponse.TaskInfo, _Mapping]]] = ...) -> None: ...
 
+class TaskField(_message.Message):
+    __slots__ = ["task_option_field", "task_option_generic_field", "task_summary_field"]
+    TASK_OPTION_FIELD_FIELD_NUMBER: _ClassVar[int]
+    TASK_OPTION_GENERIC_FIELD_FIELD_NUMBER: _ClassVar[int]
+    TASK_SUMMARY_FIELD_FIELD_NUMBER: _ClassVar[int]
+    task_option_field: TaskOptionField
+    task_option_generic_field: TaskOptionGenericField
+    task_summary_field: TaskSummaryField
+    def __init__(self, task_summary_field: _Optional[_Union[TaskSummaryField, str]] = ..., task_option_field: _Optional[_Union[TaskOptionField, str]] = ..., task_option_generic_field: _Optional[_Union[TaskOptionGenericField, _Mapping]] = ...) -> None: ...
+
+class TaskOptionGenericField(_message.Message):
+    __slots__ = ["field"]
+    FIELD_FIELD_NUMBER: _ClassVar[int]
+    field: str
+    def __init__(self, field: _Optional[str] = ...) -> None: ...
+
 class TaskRaw(_message.Message):
     __slots__ = ["acquired_at", "created_at", "creation_to_end_duration", "data_dependencies", "ended_at", "expected_output_ids", "id", "initial_task_id", "options", "output", "owner_pod_id", "parent_task_ids", "pod_hostname", "pod_ttl", "processing_to_end_duration", "received_at", "retry_of_ids", "session_id", "started_at", "status", "status_message", "submitted_at"]
     class Output(_message.Message):
         __slots__ = ["error", "success"]
         ERROR_FIELD_NUMBER: _ClassVar[int]
         SUCCESS_FIELD_NUMBER: _ClassVar[int]
         error: str
@@ -277,7 +307,13 @@
     received_at: _timestamp_pb2.Timestamp
     session_id: str
     started_at: _timestamp_pb2.Timestamp
     status: _task_status_pb2.TaskStatus
     status_message: str
     submitted_at: _timestamp_pb2.Timestamp
     def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., owner_pod_id: _Optional[str] = ..., initial_task_id: _Optional[str] = ..., count_parent_task_ids: _Optional[int] = ..., count_data_dependencies: _Optional[int] = ..., count_expected_output_ids: _Optional[int] = ..., count_retry_of_ids: _Optional[int] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., status_message: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., submitted_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., pod_ttl: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., error: _Optional[str] = ..., pod_hostname: _Optional[str] = ..., received_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., acquired_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+
+class TaskSummaryField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
+class TaskOptionField(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/versions_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/versions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/versions_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/versions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.2.dev376/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.2.dev376/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.2.dev376/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev376/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev376/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik/worker/worker.py` & `armonik-3.8.2.dev376/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev361/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev376/src/armonik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev361
+Version: 3.8.2.dev376
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev361/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev376/src/armonik.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 src/armonik/protogen/common/results_common_pb2_grpc.py
 src/armonik/protogen/common/session_status_pb2.py
 src/armonik/protogen/common/session_status_pb2.pyi
 src/armonik/protogen/common/session_status_pb2_grpc.py
 src/armonik/protogen/common/sessions_common_pb2.py
 src/armonik/protogen/common/sessions_common_pb2.pyi
 src/armonik/protogen/common/sessions_common_pb2_grpc.py
+src/armonik/protogen/common/sort_direction_pb2.py
+src/armonik/protogen/common/sort_direction_pb2.pyi
+src/armonik/protogen/common/sort_direction_pb2_grpc.py
 src/armonik/protogen/common/submitter_common_pb2.py
 src/armonik/protogen/common/submitter_common_pb2.pyi
 src/armonik/protogen/common/submitter_common_pb2_grpc.py
 src/armonik/protogen/common/task_status_pb2.py
 src/armonik/protogen/common/task_status_pb2.pyi
 src/armonik/protogen/common/task_status_pb2_grpc.py
 src/armonik/protogen/common/tasks_common_pb2.py
```


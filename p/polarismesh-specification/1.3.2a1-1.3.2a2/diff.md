# Comparing `tmp/polarismesh_specification-1.3.2a1.tar.gz` & `tmp/polarismesh_specification-1.3.2a2.tar.gz`

## Comparing `polarismesh_specification-1.3.2a1.tar` & `polarismesh_specification-1.3.2a2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8830 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    16020 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13179 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.2a2/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x06\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xaf\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf8\x04\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf9\x05\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc2\x03\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\x0cis_encrypted\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x08\x64\x61ta_key\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x06\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xac\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\tencrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf8\x04\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xf9\x05\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb0\x03\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x07 \x03(\x0b\x32\x11.v1.ConfigFileTag\x12-\n\tencrypted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\017ConfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
   _CONFIGFILEGROUP._serialized_start=58
   _CONFIGFILEGROUP._serialized_end=861
   _CONFIGFILE._serialized_start=864
-  _CONFIGFILE._serialized_end=1679
-  _CONFIGFILETAG._serialized_start=1681
-  _CONFIGFILETAG._serialized_end=1784
-  _CONFIGFILERELEASE._serialized_start=1787
-  _CONFIGFILERELEASE._serialized_end=2419
-  _CONFIGFILERELEASEHISTORY._serialized_start=2422
-  _CONFIGFILERELEASEHISTORY._serialized_end=3183
-  _CONFIGFILETEMPLATE._serialized_start=3186
-  _CONFIGFILETEMPLATE._serialized_end=3632
-  _CLIENTCONFIGFILEINFO._serialized_start=3635
-  _CLIENTCONFIGFILEINFO._serialized_end=4085
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_start=4088
-  _CLIENTWATCHCONFIGFILEREQUEST._serialized_end=4266
-  _CONFIGFILEEXPORTREQUEST._serialized_start=4269
-  _CONFIGFILEEXPORTREQUEST._serialized_end=4434
+  _CONFIGFILE._serialized_end=1676
+  _CONFIGFILETAG._serialized_start=1678
+  _CONFIGFILETAG._serialized_end=1781
+  _CONFIGFILERELEASE._serialized_start=1784
+  _CONFIGFILERELEASE._serialized_end=2416
+  _CONFIGFILERELEASEHISTORY._serialized_start=2419
+  _CONFIGFILERELEASEHISTORY._serialized_end=3180
+  _CONFIGFILETEMPLATE._serialized_start=3183
+  _CONFIGFILETEMPLATE._serialized_end=3629
+  _CLIENTCONFIGFILEINFO._serialized_start=3632
+  _CLIENTCONFIGFILEINFO._serialized_end=4064
+  _CLIENTWATCHCONFIGFILEREQUEST._serialized_start=4067
+  _CLIENTWATCHCONFIGFILEREQUEST._serialized_end=4245
+  _CONFIGFILEEXPORTREQUEST._serialized_start=4248
+  _CONFIGFILEEXPORTREQUEST._serialized_end=4413
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,82 +3,82 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ClientConfigFileInfo(_message.Message):
-    __slots__ = ["content", "data_key", "file_name", "group", "is_encrypted", "md5", "namespace", "public_key", "version"]
+    __slots__ = ["content", "encrypted", "file_name", "group", "md5", "namespace", "public_key", "tags", "version"]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
-    DATA_KEY_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
     FILE_NAME_FIELD_NUMBER: _ClassVar[int]
     GROUP_FIELD_NUMBER: _ClassVar[int]
-    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
     MD5_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
+    TAGS_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     content: _wrappers_pb2.StringValue
-    data_key: _wrappers_pb2.StringValue
+    encrypted: _wrappers_pb2.BoolValue
     file_name: _wrappers_pb2.StringValue
     group: _wrappers_pb2.StringValue
-    is_encrypted: _wrappers_pb2.BoolValue
     md5: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
     public_key: _wrappers_pb2.StringValue
+    tags: _containers.RepeatedCompositeFieldContainer[ConfigFileTag]
     version: _wrappers_pb2.UInt64Value
-    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., data_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., public_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., file_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., version: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., md5: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., public_key: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class ClientWatchConfigFileRequest(_message.Message):
     __slots__ = ["client_ip", "service_name", "watch_files"]
     CLIENT_IP_FIELD_NUMBER: _ClassVar[int]
     SERVICE_NAME_FIELD_NUMBER: _ClassVar[int]
     WATCH_FILES_FIELD_NUMBER: _ClassVar[int]
     client_ip: _wrappers_pb2.StringValue
     service_name: _wrappers_pb2.StringValue
     watch_files: _containers.RepeatedCompositeFieldContainer[ClientConfigFileInfo]
     def __init__(self, client_ip: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., service_name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., watch_files: _Optional[_Iterable[_Union[ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
 
 class ConfigFile(_message.Message):
-    __slots__ = ["comment", "content", "create_by", "create_time", "encrypt_algo", "format", "group", "id", "is_encrypted", "modify_by", "modify_time", "name", "namespace", "release_by", "release_time", "status", "tags"]
+    __slots__ = ["comment", "content", "create_by", "create_time", "encrypt_algo", "encrypted", "format", "group", "id", "modify_by", "modify_time", "name", "namespace", "release_by", "release_time", "status", "tags"]
     COMMENT_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     CREATE_BY_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
     ENCRYPT_ALGO_FIELD_NUMBER: _ClassVar[int]
     FORMAT_FIELD_NUMBER: _ClassVar[int]
     GROUP_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    IS_ENCRYPTED_FIELD_NUMBER: _ClassVar[int]
     MODIFY_BY_FIELD_NUMBER: _ClassVar[int]
     MODIFY_TIME_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     RELEASE_BY_FIELD_NUMBER: _ClassVar[int]
     RELEASE_TIME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TAGS_FIELD_NUMBER: _ClassVar[int]
     comment: _wrappers_pb2.StringValue
     content: _wrappers_pb2.StringValue
     create_by: _wrappers_pb2.StringValue
     create_time: _wrappers_pb2.StringValue
     encrypt_algo: _wrappers_pb2.StringValue
+    encrypted: _wrappers_pb2.BoolValue
     format: _wrappers_pb2.StringValue
     group: _wrappers_pb2.StringValue
     id: _wrappers_pb2.UInt64Value
-    is_encrypted: _wrappers_pb2.BoolValue
     modify_by: _wrappers_pb2.StringValue
     modify_time: _wrappers_pb2.StringValue
     name: _wrappers_pb2.StringValue
     namespace: _wrappers_pb2.StringValue
     release_by: _wrappers_pb2.StringValue
     release_time: _wrappers_pb2.StringValue
     status: _wrappers_pb2.StringValue
     tags: _containers.RepeatedCompositeFieldContainer[ConfigFileTag]
-    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., is_encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., encrypt_algo: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+    def __init__(self, id: _Optional[_Union[_wrappers_pb2.UInt64Value, _Mapping]] = ..., name: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., group: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., content: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., format: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., comment: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., tags: _Optional[_Iterable[_Union[ConfigFileTag, _Mapping]]] = ..., create_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., create_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., modify_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_time: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., release_by: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., encrypted: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., encrypt_algo: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
 
 class ConfigFileExportRequest(_message.Message):
     __slots__ = ["groups", "names", "namespace"]
     GROUPS_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     NAMES_FIELD_NUMBER: _ClassVar[int]
     groups: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
```

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.2a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/LICENSE.txt` & `polarismesh_specification-1.3.2a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/README.md` & `polarismesh_specification-1.3.2a2/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/pyproject.toml` & `polarismesh_specification-1.3.2a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.2a1/PKG-INFO` & `polarismesh_specification-1.3.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.2a1
+Version: 1.3.2a2
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```


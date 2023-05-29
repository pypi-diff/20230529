# Comparing `tmp/qwak_core-0.0.82.tar.gz` & `tmp/qwak_core-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.82.tar", max compression
+gzip compressed data, was "qwak_core-0.0.83.tar", max compression
```

## Comparing `qwak_core-0.0.82.tar` & `qwak_core-0.0.83.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-28 15:36:05.177009 qwak_core-0.0.82/README.md
--rw-r--r--   0        0        0        0 2023-05-28 15:37:48.837381 qwak_core-0.0.82/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-28 15:37:48.861382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-28 15:37:27.789306 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.861382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-28 15:37:48.857382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-28 15:37:27.421305 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.857382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-28 15:37:48.861382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-28 15:37:27.601305 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.861382 qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-28 15:37:48.849382 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-28 15:37:26.873303 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-28 15:37:48.853381 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 15:37:48.853381 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-28 15:37:27.057303 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.853381 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-28 15:37:48.857382 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-28 15:37:27.237304 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.857382 qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-28 15:37:48.837381 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-28 15:37:26.685302 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-28 15:37:48.841382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-05-28 15:37:48.841382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-05-28 15:37:27.973307 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.841382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-28 15:37:48.845382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-28 15:37:28.341308 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.845382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-28 15:37:48.845382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-28 15:37:28.529309 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-28 15:37:48.849382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-28 15:37:48.841382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-28 15:37:28.157307 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.845382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-28 15:37:48.849382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-28 15:37:28.717309 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.849382 qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-28 15:37:48.893382 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-28 15:37:31.329319 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.893382 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-28 15:37:48.893382 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-28 15:37:31.517320 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-28 15:37:48.897382 qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-28 15:37:49.045382 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-28 15:37:36.897339 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.045382 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-28 15:37:49.045382 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-28 15:37:37.081340 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-28 15:37:49.045382 qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-28 15:37:49.049382 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-28 15:37:38.021343 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-28 15:37:49.049382 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-28 15:37:49.049382 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-28 15:37:37.833342 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.049382 qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-28 15:37:49.053382 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-28 15:37:38.205344 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.053382 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-28 15:37:49.053382 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-28 15:37:38.385344 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-28 15:37:49.057382 qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-28 15:37:49.145383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-28 15:37:46.361373 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.145383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-28 15:37:49.141383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-28 15:37:45.981371 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.141383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-28 15:37:49.145383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-28 15:37:46.169372 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.145383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-28 15:37:49.137383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-28 15:37:45.597370 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-28 15:37:49.137383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-28 15:37:49.137383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-28 15:37:45.793371 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.141383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-28 15:37:49.153383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-28 15:37:46.921375 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.153383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-28 15:37:49.149383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-28 15:37:46.737374 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.149383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-28 15:37:49.149383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-28 15:37:46.553373 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.149383 qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-28 15:37:49.133383 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-28 15:37:45.405369 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.137383 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-28 15:37:49.129382 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-28 15:37:45.013368 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.129382 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-28 15:37:49.133383 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-28 15:37:45.213369 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-28 15:37:49.133383 qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-28 15:37:49.081382 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-28 15:37:40.289351 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-28 15:37:49.081382 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-28 15:37:49.077382 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-28 15:37:40.101350 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.081382 qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-28 15:37:49.069382 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-28 15:37:39.725349 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.069382 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-28 15:37:49.073382 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-28 15:37:39.909350 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.073382 qwak_core-0.0.82/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-28 15:37:49.073382 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-28 15:37:40.477352 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-28 15:37:49.073382 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-28 15:37:49.077382 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-28 15:37:40.885353 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-28 15:37:49.077382 qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-28 15:37:49.085382 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-28 15:37:41.273355 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.089383 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-28 15:37:49.089383 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 15:37:41.457355 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 15:37:49.089383 qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-28 15:37:49.061382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-28 15:37:39.165347 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.065382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-28 15:37:49.065382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-28 15:37:39.349348 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-28 15:37:49.065382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-28 15:37:49.057382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-28 15:37:38.773346 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.061382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-28 15:37:49.057382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-28 15:37:38.585345 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.057382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-28 15:37:49.061382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-28 15:37:38.977346 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-28 15:37:49.061382 qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-28 15:37:48.881382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-28 15:37:30.393315 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.881382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 15:37:48.881382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-28 15:37:30.581316 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.885382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-28 15:37:48.885382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-28 15:37:30.769317 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-28 15:37:48.885382 qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-28 15:37:49.025382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-28 15:37:35.769335 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.025382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-28 15:37:49.021382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-28 15:37:35.581334 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-28 15:37:49.021382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-28 15:37:49.001382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-28 15:37:33.893328 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.005382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-28 15:37:49.001382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-28 15:37:33.709328 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.001382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-28 15:37:48.993382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-28 15:37:33.125325 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.993382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-28 15:37:48.997382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-28 15:37:33.521327 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-28 15:37:48.997382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-28 15:37:49.005382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-28 15:37:34.081329 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.005382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-28 15:37:49.005382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-28 15:37:34.265330 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-28 15:37:49.009382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-05-28 15:37:48.997382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-05-28 15:37:33.321326 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.997382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-28 15:37:49.009382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-28 15:37:34.449330 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.009382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11277 2023-05-28 15:37:49.009382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    15070 2023-05-28 15:37:34.637331 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.013382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-28 15:37:49.025382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-28 15:37:48.265380 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.029382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-28 15:37:49.029382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-28 15:37:48.485380 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-28 15:37:49.029382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-28 15:37:49.029382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-28 15:37:36.329337 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.033382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-28 15:37:49.033382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-28 15:37:36.521338 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-28 15:37:49.033382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-28 15:37:49.033382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-28 15:37:36.705338 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.037382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-28 15:37:49.041382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-28 15:37:37.465341 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.041382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-28 15:37:49.037382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-28 15:37:37.273340 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-28 15:37:49.037382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-28 15:37:49.041382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-28 15:37:37.649342 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.041382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-28 15:37:49.013382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-28 15:37:34.829331 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.013382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-28 15:37:49.017382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-28 15:37:35.017332 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.017382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-28 15:37:49.017382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-28 15:37:35.209333 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-28 15:37:49.017382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-28 15:37:49.021382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-28 15:37:35.397334 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.021382 qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-28 15:37:49.153383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-28 15:37:47.105375 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.153383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-28 15:37:49.157383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-28 15:37:47.289376 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 15:37:49.157383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-28 15:37:49.157383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-28 15:37:47.477377 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.161383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-28 15:37:49.161383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-28 15:37:47.669377 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-28 15:37:49.161383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-28 15:37:49.161383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-28 15:37:47.865378 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-28 15:37:49.165383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-28 15:37:49.165383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-28 15:37:48.053379 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.165383 qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-28 15:37:49.093382 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-28 15:37:41.637356 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.093382 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-28 15:37:49.093382 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-28 15:37:41.825357 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-28 15:37:49.093382 qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-28 15:37:48.917382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-28 15:37:32.373323 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.929382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-28 15:37:48.941382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-28 15:37:32.557323 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.953382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-28 15:37:48.961382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-28 15:37:32.745324 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-28 15:37:48.969382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-28 15:37:48.981382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-28 15:37:32.933325 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.993382 qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-28 15:37:49.069382 qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-28 15:37:39.537348 qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-28 15:37:49.069382 qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-28 15:37:49.097382 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-28 15:37:42.009357 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.097382 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-28 15:37:49.097382 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-28 15:37:42.193358 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-28 15:37:49.097382 qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-28 15:37:49.109382 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-28 15:37:43.305362 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.113382 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-28 15:37:49.113382 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-28 15:37:43.485362 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.113382 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-28 15:37:49.113382 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-28 15:37:43.681363 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.117383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-28 15:37:49.117383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-28 15:37:43.873364 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.117383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-28 15:37:49.117383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-28 15:37:44.065364 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.121383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-28 15:37:49.121383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-28 15:37:44.269365 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-28 15:37:49.121383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-28 15:37:49.125383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-28 15:37:44.457366 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.125383 qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-28 15:37:49.101382 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-28 15:37:42.561359 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.101382 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-28 15:37:49.109382 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-28 15:37:43.121361 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.109382 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-28 15:37:49.105383 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-28 15:37:42.749360 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-28 15:37:49.105383 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-28 15:37:49.105383 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-28 15:37:42.937360 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.109382 qwak_core-0.0.82/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-28 15:37:49.085382 qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-28 15:37:41.089354 qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-28 15:37:49.085382 qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-28 15:37:48.877382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-28 15:37:31.953321 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-28 15:37:48.877382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-28 15:37:48.873382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-28 15:37:31.729320 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.877382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-28 15:37:48.877382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-28 15:37:32.173322 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-28 15:37:48.881382 qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-28 15:37:49.081382 qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-28 15:37:40.677353 qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-28 15:37:49.085382 qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-28 15:37:49.101382 qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-28 15:37:42.377359 qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-28 15:37:49.101382 qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-28 15:37:48.873382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-28 15:37:29.645313 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.873382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-28 15:37:48.869382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-28 15:37:29.457312 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-28 15:37:48.873382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-28 15:37:48.865382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-28 15:37:28.901310 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.865382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-28 15:37:48.865382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-28 15:37:29.085311 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.865382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-28 15:37:48.869382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-28 15:37:29.273311 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-28 15:37:48.869382 qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-28 15:37:49.129382 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-28 15:37:44.829367 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-28 15:37:49.129382 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-28 15:37:49.125383 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-28 15:37:44.645367 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:49.125383 qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-28 15:37:48.889382 qwak_core-0.0.82/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-28 15:37:30.957317 qwak_core-0.0.82/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.889382 qwak_core-0.0.82/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-28 15:37:48.889382 qwak_core-0.0.82/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-28 15:37:31.141318 qwak_core-0.0.82/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-28 15:37:48.889382 qwak_core-0.0.82/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-28 15:37:50.533388 qwak_core-0.0.82/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-28 15:37:50.533388 qwak_core-0.0.82/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-28 15:36:05.177009 qwak_core-0.0.82/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-28 15:36:05.181009 qwak_core-0.0.82/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-28 15:36:05.185009 qwak_core-0.0.82/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.82/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-29 07:00:39.130911 qwak_core-0.0.83/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 07:02:20.531242 qwak_core-0.0.83/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-29 07:02:20.559242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-29 07:01:59.339172 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.559242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-29 07:02:20.555242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-29 07:01:58.955171 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.555242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-29 07:02:20.555242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-29 07:01:59.139172 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.555242 qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-29 07:02:20.547242 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-29 07:01:58.399169 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-29 07:02:20.547242 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-29 07:02:20.547242 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-29 07:01:58.587170 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.551241 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-29 07:02:20.551241 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-29 07:01:58.775171 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.551241 qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-29 07:02:20.531242 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-29 07:01:58.211169 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-29 07:02:20.535241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-05-29 07:02:20.535241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-05-29 07:01:59.527173 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.535241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-29 07:02:20.539241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-29 07:01:59.899174 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.539241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-29 07:02:20.543242 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-29 07:02:00.091175 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-29 07:02:20.543242 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-29 07:02:20.539241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-29 07:01:59.711174 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.539241 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-29 07:02:20.543242 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-29 07:02:00.275175 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.547242 qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-29 07:02:20.631242 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-29 07:02:02.859184 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.631242 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-29 07:02:20.631242 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-29 07:02:03.047185 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-29 07:02:20.635242 qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-29 07:02:20.707242 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-29 07:02:08.339202 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.707242 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-29 07:02:20.707242 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-29 07:02:08.523202 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-29 07:02:20.707242 qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-29 07:02:20.711242 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-29 07:02:09.539206 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-29 07:02:20.715242 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-29 07:02:20.711242 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-29 07:02:09.339205 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.711242 qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-29 07:02:20.715242 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-29 07:02:09.751206 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.715242 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-29 07:02:20.715242 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-29 07:02:09.951207 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-29 07:02:20.719242 qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-29 07:02:20.843243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-29 07:02:18.163234 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.843243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-29 07:02:20.839243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-29 07:02:17.787232 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.839243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-29 07:02:20.843243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-29 07:02:17.975233 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.843243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-29 07:02:20.835243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-29 07:02:17.407231 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-29 07:02:20.835243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-29 07:02:20.839243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-29 07:02:17.599232 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.839243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-29 07:02:20.851243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-29 07:02:18.715236 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.851243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-29 07:02:20.847242 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-29 07:02:18.531235 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.851243 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-29 07:02:20.847242 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-29 07:02:18.347234 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.847242 qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-29 07:02:20.831242 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-29 07:02:17.215231 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.835243 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-29 07:02:20.827242 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-29 07:02:16.827229 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.827242 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-29 07:02:20.831242 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-29 07:02:17.027230 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-29 07:02:20.831242 qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-29 07:02:20.747242 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-29 07:02:12.079214 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-29 07:02:20.747242 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-29 07:02:20.743242 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-29 07:02:11.871213 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.743242 qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-29 07:02:20.735242 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-29 07:02:11.459212 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.735242 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-29 07:02:20.735242 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-29 07:02:11.663213 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.735242 qwak_core-0.0.83/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-29 07:02:20.739242 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-29 07:02:12.287215 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-29 07:02:20.739242 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-29 07:02:20.739242 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-29 07:02:12.707216 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-29 07:02:20.743242 qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-29 07:02:20.751242 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-29 07:02:13.095217 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.755242 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-29 07:02:20.755242 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-29 07:02:13.279218 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-29 07:02:20.755242 qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-29 07:02:20.727242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-29 07:02:10.795210 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.727242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-29 07:02:20.727242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-29 07:02:11.011211 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-29 07:02:20.731242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-29 07:02:20.723242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-29 07:02:10.371208 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.723242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-29 07:02:20.719242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-29 07:02:10.167208 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.719242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-29 07:02:20.723242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-29 07:02:10.587209 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-29 07:02:20.727242 qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-29 07:02:20.619242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-29 07:02:01.927181 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.619242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-29 07:02:20.623242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-29 07:02:02.111181 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.623242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-29 07:02:20.623242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-29 07:02:02.295182 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-29 07:02:20.623242 qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-29 07:02:20.687242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-29 07:02:07.231198 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.687242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-29 07:02:20.683242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-29 07:02:07.051198 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-29 07:02:20.683242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-29 07:02:20.663242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-29 07:02:05.371192 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.663242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-29 07:02:20.659242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-29 07:02:05.183191 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.663242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-29 07:02:20.655242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-29 07:02:04.611190 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.655242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-29 07:02:20.659242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-29 07:02:04.999191 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-29 07:02:20.659242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-29 07:02:20.663242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-29 07:02:05.555193 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.667242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-29 07:02:20.667242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-29 07:02:05.743193 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-29 07:02:20.667242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-29 07:02:20.655242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-29 07:02:04.803190 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.655242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-29 07:02:20.671242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-29 07:02:05.927194 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.671242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11277 2023-05-29 07:02:20.671242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-29 07:02:06.127195 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.671242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-29 07:02:20.687242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-29 07:02:20.055240 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.687242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-29 07:02:20.691242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-29 07:02:20.243240 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-29 07:02:20.691242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-29 07:02:20.691242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-29 07:02:07.787200 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.691242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-29 07:02:20.695242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-29 07:02:07.971201 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-29 07:02:20.695242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-29 07:02:20.695242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-29 07:02:08.155201 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.699242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-29 07:02:20.699242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-29 07:02:08.931204 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.703242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-29 07:02:20.699242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-29 07:02:08.711203 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-29 07:02:20.699242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-29 07:02:20.703242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-29 07:02:09.135204 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.703242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-29 07:02:20.675242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-29 07:02:06.315195 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.675242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-29 07:02:20.675242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-29 07:02:06.503196 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.679242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-29 07:02:20.679242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-29 07:02:06.687196 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-29 07:02:20.679242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-29 07:02:20.679242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-29 07:02:06.871197 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.683242 qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-29 07:02:20.851243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-29 07:02:18.899236 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.855243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-29 07:02:20.855243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-29 07:02:19.083237 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-29 07:02:20.855243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-29 07:02:20.859243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-29 07:02:19.263237 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.859243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-29 07:02:20.859243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-29 07:02:19.459238 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-29 07:02:20.863242 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-29 07:02:20.863242 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-29 07:02:19.651239 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-29 07:02:20.863242 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-29 07:02:20.863242 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-29 07:02:19.863239 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.867243 qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-29 07:02:20.759242 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-29 07:02:13.467218 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.759242 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-29 07:02:20.759242 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-29 07:02:13.655219 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-29 07:02:20.759242 qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-29 07:02:20.635242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-29 07:02:03.871187 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.639242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-29 07:02:20.639242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-29 07:02:04.055188 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.643242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-29 07:02:20.643242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-29 07:02:04.239188 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-29 07:02:20.647242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-29 07:02:20.651242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-29 07:02:04.423189 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.651242 qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-29 07:02:20.731242 qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-29 07:02:11.235211 qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-29 07:02:20.731242 qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-29 07:02:20.763242 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-29 07:02:13.839220 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.763242 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-29 07:02:20.763242 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-29 07:02:14.027220 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-29 07:02:20.767242 qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-29 07:02:20.779242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-29 07:02:15.131224 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.807242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-29 07:02:20.807242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-29 07:02:15.315225 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.807242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-29 07:02:20.811242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-29 07:02:15.503225 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.811242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-29 07:02:20.811242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-29 07:02:15.695226 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.815242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-29 07:02:20.815242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-29 07:02:15.887226 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.815242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-29 07:02:20.819242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-29 07:02:16.091227 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-29 07:02:20.819242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-29 07:02:20.819242 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-29 07:02:16.275228 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.823243 qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-29 07:02:20.771242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-29 07:02:14.395222 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.771242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-29 07:02:20.775242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-29 07:02:14.947223 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.779242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-29 07:02:20.771242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-29 07:02:14.579222 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-29 07:02:20.771242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-29 07:02:20.775242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-29 07:02:14.763223 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.775242 qwak_core-0.0.83/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-29 07:02:20.751242 qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-29 07:02:12.911217 qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-29 07:02:20.751242 qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-29 07:02:20.615242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-29 07:02:03.463186 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-29 07:02:20.615242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-29 07:02:20.611242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-29 07:02:03.247185 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.615242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-29 07:02:20.615242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-29 07:02:03.671187 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-29 07:02:20.619242 qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-29 07:02:20.747242 qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-29 07:02:12.499215 qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-29 07:02:20.747242 qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-29 07:02:20.767242 qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-29 07:02:14.211221 qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-29 07:02:20.767242 qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-29 07:02:20.611242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-29 07:02:01.199179 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.611242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-29 07:02:20.607242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-29 07:02:01.015178 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-29 07:02:20.607242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-29 07:02:20.559242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-29 07:02:00.459176 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.563242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-29 07:02:20.563242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-29 07:02:00.647177 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.563242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-29 07:02:20.563242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-29 07:02:00.831177 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-29 07:02:20.607242 qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-29 07:02:20.823243 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-29 07:02:16.647229 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-29 07:02:20.827242 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-29 07:02:20.823243 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-29 07:02:16.459228 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.823243 qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-29 07:02:20.627242 qwak_core-0.0.83/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-29 07:02:02.479183 qwak_core-0.0.83/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.627242 qwak_core-0.0.83/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-29 07:02:20.627242 qwak_core-0.0.83/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-29 07:02:02.671183 qwak_core-0.0.83/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 07:02:20.631242 qwak_core-0.0.83/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-29 07:02:22.139247 qwak_core-0.0.83/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-29 07:02:22.139247 qwak_core-0.0.83/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.134911 qwak_core-0.0.83/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-29 07:00:39.138911 qwak_core-0.0.83/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-29 07:00:39.142911 qwak_core-0.0.83/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.83/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.83/PKG-INFO
```

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.83/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.83/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/pyproject.toml` & `qwak_core-0.0.83/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.82"
+version = "0.0.83"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.82/qwak/automations/__init__.py` & `qwak_core-0.0.83/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/automations/automation_executions.py` & `qwak_core-0.0.83/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/automations/automations.py` & `qwak_core-0.0.83/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.83/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.83/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/automations/common.py` & `qwak_core-0.0.83/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.83/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.83/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.83/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.83/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.83/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/alert_management/client.py` & `qwak_core-0.0.83/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/analytics/client.py` & `qwak_core-0.0.83/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/audience/client.py` & `qwak_core-0.0.83/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/automation_management/client.py` & `qwak_core-0.0.83/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.83/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.83/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.83/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.83/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/build_management/client.py` & `qwak_core-0.0.83/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.83/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.83/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/deployment/client.py` & `qwak_core-0.0.83/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.83/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.83/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.83/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.83/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/instance_template/client.py` & `qwak_core-0.0.83/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.83/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/logging_client/client.py` & `qwak_core-0.0.83/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/model_management/client.py` & `qwak_core-0.0.83/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/project/client.py` & `qwak_core-0.0.83/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/secret_service/client.py` & `qwak_core-0.0.83/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.83/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.83/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.83/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.83/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.83/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.83/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.83/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.83/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.83/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.83/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/offline/client.py` & `qwak_core-0.0.83/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/feature_store/online/client.py` & `qwak_core-0.0.83/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/const.py` & `qwak_core-0.0.83/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.83/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.83/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.83/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.83/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/singleton_meta.py` & `qwak_core-0.0.83/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/tool/auth.py` & `qwak_core-0.0.83/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.83/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.83/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.83/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.83/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/__init__.py` & `qwak_core-0.0.83/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.83/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.83/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.83/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.83/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.83/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/base.py` & `qwak_core-0.0.83/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/decorators/api.py` & `qwak_core-0.0.83/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.83/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/experiment_tracking.py` & `qwak_core-0.0.83/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/schema.py` & `qwak_core-0.0.83/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/schema_entities.py` & `qwak_core-0.0.83/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.83/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.83/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.83/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.83/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.83/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.83/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.83/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.83/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/client.py` & `qwak_core-0.0.83/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.83/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/models/model.py` & `qwak_core-0.0.83/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.83/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.83/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/tools/logger/logger.py` & `qwak_core-0.0.83/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak/tools/logger/logging.yml` & `qwak_core-0.0.83/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.83/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/qwak_services_mock/services_mock.py` & `qwak_core-0.0.83/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.82/setup.py` & `qwak_core-0.0.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.82',
+    'version': '0.0.83',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.82/PKG-INFO` & `qwak_core-0.0.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.82
+Version: 0.0.83
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```


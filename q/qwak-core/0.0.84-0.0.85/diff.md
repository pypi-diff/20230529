# Comparing `tmp/qwak_core-0.0.84.tar.gz` & `tmp/qwak_core-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.84.tar", max compression
+gzip compressed data, was "qwak_core-0.0.85.tar", max compression
```

## Comparing `qwak_core-0.0.84.tar` & `qwak_core-0.0.85.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-29 12:14:07.042600 qwak_core-0.0.84/README.md
--rw-r--r--   0        0        0        0 2023-05-29 12:16:02.942882 qwak_core-0.0.84/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-29 12:16:02.990882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-29 12:15:40.630828 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.990882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-29 12:16:02.986882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-29 12:15:40.242828 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.986882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-29 12:16:02.986882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-29 12:15:40.434828 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.990882 qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-29 12:16:02.978882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-29 12:15:39.658826 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-29 12:16:02.982882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-29 12:16:02.982882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-29 12:15:39.850827 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.982882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-29 12:16:02.982882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-29 12:15:40.046827 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.986882 qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-29 12:16:02.942882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-29 12:15:39.462826 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-29 12:16:02.942882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-05-29 12:16:02.946882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-05-29 12:15:40.826829 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.970882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-29 12:16:02.974882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-29 12:15:41.214830 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.974882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-29 12:16:02.974882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-29 12:15:41.414830 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-29 12:16:02.974882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-29 12:16:02.970882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-29 12:15:41.018829 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.970882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-29 12:16:02.978882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-29 12:15:41.614831 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.978882 qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-29 12:16:03.022882 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-29 12:15:44.418838 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.022882 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-29 12:16:03.022882 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-29 12:15:44.618838 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-29 12:16:03.026882 qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-29 12:16:03.174882 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-29 12:15:50.330852 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.174882 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-29 12:16:03.178882 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-29 12:15:50.534852 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-29 12:16:03.178882 qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-29 12:16:03.182882 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-29 12:15:51.538854 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-29 12:16:03.182882 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-29 12:16:03.178882 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-29 12:15:51.338854 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.178882 qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-29 12:16:03.182882 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-29 12:15:51.734855 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.182882 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-29 12:16:03.186882 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-29 12:15:51.930855 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-29 12:16:03.186882 qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-29 12:16:03.278882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-29 12:16:00.394876 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.278882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-29 12:16:03.274882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-29 12:15:59.994875 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.274882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-29 12:16:03.274882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-29 12:16:00.190875 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.278882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-29 12:16:03.270882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-29 12:15:59.602874 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-29 12:16:03.270882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-29 12:16:03.270882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-29 12:15:59.802874 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.274882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-29 12:16:03.286882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-29 12:16:00.974877 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.286882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-29 12:16:03.282882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-29 12:16:00.782877 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.282882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-29 12:16:03.282882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-29 12:16:00.586876 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.282882 qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-29 12:16:03.266882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-29 12:15:59.394873 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.270882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-29 12:16:03.262882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-29 12:15:58.994872 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.262882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-29 12:16:03.266882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-29 12:15:59.198873 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-29 12:16:03.266882 qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-29 12:16:03.210882 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-29 12:15:53.958860 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-29 12:16:03.214882 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-29 12:16:03.210882 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-29 12:15:53.754860 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.210882 qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-29 12:16:03.202882 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-29 12:15:53.358859 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.202882 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-29 12:16:03.202882 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-29 12:15:53.550859 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.202882 qwak_core-0.0.84/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-29 12:16:03.206882 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-29 12:15:54.158861 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-29 12:16:03.206882 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-29 12:16:03.206882 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-29 12:15:54.594862 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-29 12:16:03.210882 qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-29 12:16:03.218882 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-29 12:15:55.010863 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.218882 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-29 12:16:03.222882 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-29 12:15:55.214863 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-29 12:16:03.222882 qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-29 12:16:03.194882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-29 12:15:52.762858 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.194882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-29 12:16:03.198882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-29 12:15:52.962858 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-29 12:16:03.198882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-29 12:16:03.190882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-29 12:15:52.354857 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.190882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-29 12:16:03.186882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-29 12:15:52.142856 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.190882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-29 12:16:03.190882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-29 12:15:52.562857 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-29 12:16:03.194882 qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-29 12:16:03.010882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-29 12:15:43.422835 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.010882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-29 12:16:03.014882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-29 12:15:43.622836 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.014882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-29 12:16:03.014882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-29 12:15:43.822836 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-29 12:16:03.014882 qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-29 12:16:03.154882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-29 12:15:49.106849 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.154882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-29 12:16:03.150882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-29 12:15:48.910848 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-29 12:16:03.154882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-29 12:16:03.130882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-29 12:15:47.102844 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.134882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-29 12:16:03.130882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-29 12:15:46.902844 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.130882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-29 12:16:03.122882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-29 12:15:46.286842 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.122882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-29 12:16:03.126882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-29 12:15:46.706843 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-29 12:16:03.130882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-29 12:16:03.134882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-29 12:15:47.302844 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.134882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-29 12:16:03.138882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-29 12:15:47.498845 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-29 12:16:03.138882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-05-29 12:16:03.126882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-05-29 12:15:46.494843 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.126882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-29 12:16:03.138882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-29 12:15:47.714846 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.138882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    11277 2023-05-29 12:16:03.142882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    15070 2023-05-29 12:15:47.914846 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.142882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-29 12:16:03.158882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-29 12:16:02.366880 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.158882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-29 12:16:03.158882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-29 12:16:02.582881 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-29 12:16:03.158882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-29 12:16:03.162882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-29 12:15:49.714850 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.162882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-29 12:16:03.162882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-29 12:15:49.918851 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-29 12:16:03.166882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-29 12:16:03.166882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-29 12:15:50.130851 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.166882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-29 12:16:03.170882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-29 12:15:50.938853 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.170882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-29 12:16:03.166882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-29 12:15:50.734853 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-29 12:16:03.170882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-29 12:16:03.170882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-29 12:15:51.138854 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.174882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-29 12:16:03.142882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-29 12:15:48.114846 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.142882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-29 12:16:03.146882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-29 12:15:48.314847 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.146882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-29 12:16:03.146882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-29 12:15:48.514847 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-29 12:16:03.150882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-29 12:16:03.150882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-29 12:15:48.710848 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.150882 qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-29 12:16:03.286882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-29 12:16:01.170877 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.286882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-29 12:16:03.290882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-29 12:16:01.366878 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-29 12:16:03.290882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-29 12:16:03.290882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-29 12:16:01.558878 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.294882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-29 12:16:03.294882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-29 12:16:01.762879 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-29 12:16:03.294882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-29 12:16:03.294882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-29 12:16:01.966879 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-29 12:16:03.298882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-29 12:16:03.298882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-29 12:16:02.158880 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.298882 qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-29 12:16:03.222882 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-29 12:15:55.414864 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.222882 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-29 12:16:03.226882 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-29 12:15:55.606864 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-29 12:16:03.226882 qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-29 12:16:03.026882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-29 12:15:45.426840 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.038882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-29 12:16:03.046882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-29 12:15:45.622841 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.062882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-29 12:16:03.086882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-29 12:15:45.834841 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-29 12:16:03.102882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-29 12:16:03.114882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-29 12:15:46.078842 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.122882 qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-29 12:16:03.198882 qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-29 12:15:53.158858 qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-29 12:16:03.198882 qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-29 12:16:03.226882 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-29 12:15:55.806865 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.230882 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-29 12:16:03.230882 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-29 12:15:56.030865 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-29 12:16:03.230882 qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-29 12:16:03.242882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-29 12:15:57.214868 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.242882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-29 12:16:03.246882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-29 12:15:57.406869 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.246882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-29 12:16:03.246882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-29 12:15:57.602869 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.246882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-29 12:16:03.250882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-29 12:15:57.798869 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.250882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-29 12:16:03.250882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-29 12:15:57.998870 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.254882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-29 12:16:03.254882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-29 12:15:58.214870 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-29 12:16:03.254882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-29 12:16:03.254882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-29 12:15:58.410871 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.258882 qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-29 12:16:03.234882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-29 12:15:56.438866 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.234882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-29 12:16:03.242882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-29 12:15:57.022868 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.242882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-29 12:16:03.234882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-29 12:15:56.638867 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-29 12:16:03.238882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-29 12:16:03.238882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-29 12:15:56.830867 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.238882 qwak_core-0.0.84/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-29 12:16:03.218882 qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-29 12:15:54.806862 qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-29 12:16:03.218882 qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-29 12:16:03.006882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-29 12:15:45.022839 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-29 12:16:03.006882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-29 12:16:03.002882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-29 12:15:44.822838 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.006882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-29 12:16:03.006882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-29 12:15:45.226839 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-29 12:16:03.010882 qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-29 12:16:03.214882 qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-29 12:15:54.378861 qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-29 12:16:03.214882 qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-29 12:16:03.230882 qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-29 12:15:56.230866 qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-29 12:16:03.234882 qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-29 12:16:03.002882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-29 12:15:42.622833 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.002882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-29 12:16:02.998882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-29 12:15:42.418833 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-29 12:16:03.002882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-29 12:16:02.994882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-29 12:15:41.810831 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.994882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-29 12:16:02.994882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-29 12:15:42.018832 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:02.994882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-29 12:16:02.998882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-29 12:15:42.214832 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-29 12:16:02.998882 qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-29 12:16:03.262882 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-29 12:15:58.802872 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-29 12:16:03.262882 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-29 12:16:03.258882 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-29 12:15:58.606871 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.258882 qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-29 12:16:03.018882 qwak_core-0.0.84/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-29 12:15:44.022837 qwak_core-0.0.84/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.018882 qwak_core-0.0.84/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-29 12:16:03.018882 qwak_core-0.0.84/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-29 12:15:44.218837 qwak_core-0.0.84/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-29 12:16:03.022882 qwak_core-0.0.84/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-29 12:16:04.738886 qwak_core-0.0.84/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-29 12:16:04.738886 qwak_core-0.0.84/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-29 12:14:07.046600 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-29 12:14:07.050601 qwak_core-0.0.84/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-29 12:14:07.054601 qwak_core-0.0.84/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.84/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.84/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-29 13:31:52.282055 qwak_core-0.0.85/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 13:33:39.754327 qwak_core-0.0.85/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-29 13:33:39.782328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-29 13:33:17.846271 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.782328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-29 13:33:39.778328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-29 13:33:17.458270 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.778328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-29 13:33:39.778328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-29 13:33:17.650271 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.782328 qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-29 13:33:39.770327 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-29 13:33:16.874269 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-29 13:33:39.770327 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-29 13:33:39.774328 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-29 13:33:17.070269 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.774328 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-29 13:33:39.774328 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-29 13:33:17.262270 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.774328 qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-29 13:33:39.758328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-29 13:33:16.678269 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-29 13:33:39.758328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-05-29 13:33:39.758328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-05-29 13:33:18.042272 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.762328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-29 13:33:39.762328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-29 13:33:18.430273 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.766327 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-29 13:33:39.766327 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-29 13:33:18.626273 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-29 13:33:39.766327 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-29 13:33:39.762328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-29 13:33:18.234273 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.762328 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-29 13:33:39.766327 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-29 13:33:18.822274 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.770327 qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-29 13:33:39.814328 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-29 13:33:21.622281 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.814328 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-29 13:33:39.814328 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-29 13:33:21.818282 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-29 13:33:39.814328 qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-29 13:33:39.882328 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-29 13:33:27.342296 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.886328 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-29 13:33:39.886328 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-29 13:33:27.538296 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-29 13:33:39.886328 qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-29 13:33:39.890328 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-29 13:33:28.526299 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-29 13:33:39.890328 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-29 13:33:39.890328 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-29 13:33:28.334298 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.890328 qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-29 13:33:39.894328 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-29 13:33:28.718299 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.894328 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-29 13:33:39.894328 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-29 13:33:28.914300 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-29 13:33:39.894328 qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-29 13:33:39.990328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-29 13:33:37.306321 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.990328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-29 13:33:39.986328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-29 13:33:36.910320 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.986328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-29 13:33:39.986328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-29 13:33:37.106321 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.990328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-29 13:33:39.982328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-29 13:33:36.498319 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-29 13:33:39.982328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-29 13:33:39.982328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-29 13:33:36.718320 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.986328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-29 13:33:39.998328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-29 13:33:37.890323 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.998328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-29 13:33:39.994328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-29 13:33:37.698322 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.994328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-29 13:33:39.990328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-29 13:33:37.502322 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.994328 qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-29 13:33:39.978328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-29 13:33:36.290319 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.978328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-29 13:33:39.974328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-29 13:33:35.878318 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.974328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-29 13:33:39.978328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-29 13:33:36.094318 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-29 13:33:39.978328 qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-29 13:33:39.922328 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-29 13:33:30.906305 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-29 13:33:39.922328 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-29 13:33:39.918328 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-29 13:33:30.702304 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.922328 qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-05-29 13:33:39.910328 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-05-29 13:33:30.310303 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.910328 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-29 13:33:39.914328 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-29 13:33:30.502304 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.914328 qwak_core-0.0.85/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-29 13:33:39.914328 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-29 13:33:31.102306 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-29 13:33:39.918328 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-29 13:33:39.918328 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-29 13:33:31.526306 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-29 13:33:39.918328 qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-29 13:33:39.930328 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-29 13:33:31.934307 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.930328 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-29 13:33:39.930328 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-29 13:33:32.122308 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-29 13:33:39.934328 qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-29 13:33:39.902328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-29 13:33:29.722302 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.906328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-29 13:33:39.906328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-29 13:33:29.914302 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-29 13:33:39.906328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-29 13:33:39.898328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-29 13:33:29.322301 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.902328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-29 13:33:39.898328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-29 13:33:29.122300 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.898328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-29 13:33:39.902328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-29 13:33:29.526301 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-29 13:33:39.902328 qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-29 13:33:39.802327 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-29 13:33:20.630279 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.802327 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-29 13:33:39.802327 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-29 13:33:20.830279 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.806328 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-29 13:33:39.806328 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-29 13:33:21.030280 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-29 13:33:39.806328 qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-29 13:33:39.862328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-29 13:33:26.166293 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.866328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-29 13:33:39.862328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-29 13:33:25.974292 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-29 13:33:39.862328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-29 13:33:39.842328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-29 13:33:24.202288 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.842328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-29 13:33:39.838328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-29 13:33:24.006287 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.838328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-29 13:33:39.830328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-29 13:33:23.394286 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.834328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-29 13:33:39.838328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-29 13:33:23.810287 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-29 13:33:39.838328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-29 13:33:39.842328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-29 13:33:24.398288 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.846328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-29 13:33:39.846328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-29 13:33:24.594289 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-29 13:33:39.846328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-29 13:33:39.834328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-29 13:33:23.602286 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.834328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-29 13:33:39.846328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-29 13:33:24.790289 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.850328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    11277 2023-05-29 13:33:39.850328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-29 13:33:24.990290 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.850328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-29 13:33:39.866328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-29 13:33:39.274326 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.866328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-29 13:33:39.866328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-29 13:33:39.470327 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-29 13:33:39.870328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-29 13:33:39.870328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-29 13:33:26.754294 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.870328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-29 13:33:39.874328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-29 13:33:26.950295 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-29 13:33:39.874328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-29 13:33:39.874328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-29 13:33:27.146295 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.874328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-29 13:33:39.878328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-29 13:33:27.938297 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.882328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-29 13:33:39.878328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-29 13:33:27.738297 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-29 13:33:39.878328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-29 13:33:39.882328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-29 13:33:28.134298 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.882328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-29 13:33:39.854328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-29 13:33:25.190290 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.854328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-29 13:33:39.854328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-29 13:33:25.386291 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.854328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-29 13:33:39.858328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-29 13:33:25.586291 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-29 13:33:39.858328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-29 13:33:39.858328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-29 13:33:25.782292 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.862328 qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-29 13:33:39.998328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-29 13:33:38.086323 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.998328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-29 13:33:40.002328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-29 13:33:38.282324 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-29 13:33:40.002328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-29 13:33:40.002328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-29 13:33:38.474324 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:40.006328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-29 13:33:40.006328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-29 13:33:38.678325 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-29 13:33:40.006328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-29 13:33:40.006328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-29 13:33:38.882325 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-29 13:33:40.010328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-29 13:33:40.010328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-29 13:33:39.078326 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:40.010328 qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-29 13:33:39.934328 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-29 13:33:32.322308 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.934328 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-29 13:33:39.934328 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-29 13:33:32.518309 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-29 13:33:39.938328 qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-29 13:33:39.818328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-29 13:33:22.606284 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.818328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-29 13:33:39.822328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-29 13:33:22.798284 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.822328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-29 13:33:39.826328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-29 13:33:22.994285 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-29 13:33:39.826328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-29 13:33:39.830328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-29 13:33:23.190285 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.830328 qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-29 13:33:39.910328 qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-29 13:33:30.110303 qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-29 13:33:39.910328 qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-29 13:33:39.938328 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-29 13:33:32.718309 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.938328 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-29 13:33:39.942328 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-29 13:33:32.938310 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-29 13:33:39.942328 qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-29 13:33:39.954328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-29 13:33:34.098313 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.954328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-29 13:33:39.954328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-29 13:33:34.290314 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.958328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-29 13:33:39.958328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-29 13:33:34.490314 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.958328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-29 13:33:39.962328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-29 13:33:34.686314 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.962328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-29 13:33:39.962328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-29 13:33:34.886315 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.962328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-29 13:33:39.966328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-29 13:33:35.098316 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-29 13:33:39.966328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-29 13:33:39.966328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-29 13:33:35.294316 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.970328 qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-29 13:33:39.946328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-29 13:33:33.330311 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.946328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-29 13:33:39.950328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-29 13:33:33.906313 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.954328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-29 13:33:39.946328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-29 13:33:33.526311 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-29 13:33:39.946328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-29 13:33:39.950328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-29 13:33:33.714312 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.950328 qwak_core-0.0.85/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-29 13:33:39.926328 qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-29 13:33:31.738307 qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-29 13:33:39.926328 qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-29 13:33:39.798328 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-29 13:33:22.214283 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-29 13:33:39.798328 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-29 13:33:39.794328 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-29 13:33:22.018282 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.794328 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-29 13:33:39.798328 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-29 13:33:22.410283 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-29 13:33:39.802327 qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-29 13:33:39.926328 qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-29 13:33:31.310306 qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-29 13:33:39.926328 qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-29 13:33:39.942328 qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-29 13:33:33.130311 qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-29 13:33:39.942328 qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-29 13:33:39.794328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-29 13:33:19.826277 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.794328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-29 13:33:39.790328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-29 13:33:19.630276 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-29 13:33:39.790328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-29 13:33:39.782328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-29 13:33:19.026275 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.786327 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-29 13:33:39.786327 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-29 13:33:19.222275 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.786327 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-29 13:33:39.786327 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-29 13:33:19.426276 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-29 13:33:39.790328 qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-29 13:33:39.970328 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-29 13:33:35.686317 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-29 13:33:39.974328 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-29 13:33:39.970328 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-29 13:33:35.490316 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.970328 qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-29 13:33:39.810328 qwak_core-0.0.85/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-29 13:33:21.230280 qwak_core-0.0.85/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.810328 qwak_core-0.0.85/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-29 13:33:39.810328 qwak_core-0.0.85/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-29 13:33:21.422281 qwak_core-0.0.85/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-29 13:33:39.810328 qwak_core-0.0.85/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-29 13:33:41.390332 qwak_core-0.0.85/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-29 13:33:41.390332 qwak_core-0.0.85/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-29 13:31:52.286055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-29 13:31:52.290055 qwak_core-0.0.85/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-29 13:31:52.294055 qwak_core-0.0.85/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.85/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.85/PKG-INFO
```

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\"\xff\x03\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12?\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesH\x00\x12?\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\tB\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\x8e\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\"\x8d\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"a\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*h\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\x1a/qwak/user_application/common/v0/resources.proto\"\xeb\x04\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12\x43\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesB\x02\x18\x01H\x00\x12\x43\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesB\x02\x18\x01H\x00\x12\x62\n\x1c\x63lient_pod_compute_resources\x18\r \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\tB\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\x8e\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\"\x8d\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"a\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*h\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _DATACOLUMNTYPE = DESCRIPTOR.enum_types_by_name['DataColumnType']
 DataColumnType = enum_type_wrapper.EnumTypeWrapper(_DATACOLUMNTYPE)
@@ -144,40 +145,44 @@
   })
 _sym_db.RegisterMessage(CsvFormat)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.qwak.ai.builds.orchestrator.apiP\001'
-  _MEMORYUNIT._serialized_start=1904
-  _MEMORYUNIT._serialized_end=1959
-  _GPUTYPE._serialized_start=1961
-  _GPUTYPE._serialized_end=2065
-  _DATACOLUMNTYPE._serialized_start=2067
-  _DATACOLUMNTYPE._serialized_end=2167
-  _REMOTEBUILDSPEC._serialized_start=54
-  _REMOTEBUILDSPEC._serialized_end=565
-  _BUILDPROPERTIESV1._serialized_start=567
-  _BUILDPROPERTIESV1._serialized_end=670
-  _BUILDPROPERTIES._serialized_start=673
-  _BUILDPROPERTIES._serialized_end=815
-  _MODELURISPEC._serialized_start=818
-  _MODELURISPEC._serialized_end=959
-  _BUILDENV._serialized_start=961
-  _BUILDENV._serialized_end=1085
-  _DOCKERENV._serialized_start=1087
-  _DOCKERENV._serialized_end=1184
-  _PYTHONENV._serialized_start=1186
-  _PYTHONENV._serialized_end=1310
-  _CPURESOURCES._serialized_start=1312
-  _CPURESOURCES._serialized_end=1422
-  _GPURESOURCES._serialized_start=1424
-  _GPURESOURCES._serialized_end=1511
-  _DATATABLEDEFINITION._serialized_start=1514
-  _DATATABLEDEFINITION._serialized_end=1659
-  _DATACOLUMNDEFINITION._serialized_start=1661
-  _DATACOLUMNDEFINITION._serialized_end=1753
-  _DATAFORMAT._serialized_start=1755
-  _DATAFORMAT._serialized_end=1829
-  _CSVFORMAT._serialized_start=1831
-  _CSVFORMAT._serialized_end=1902
+  _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._options = None
+  _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._serialized_options = b'\030\001'
+  _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._options = None
+  _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
+  _MEMORYUNIT._serialized_start=2061
+  _MEMORYUNIT._serialized_end=2116
+  _GPUTYPE._serialized_start=2118
+  _GPUTYPE._serialized_end=2222
+  _DATACOLUMNTYPE._serialized_start=2224
+  _DATACOLUMNTYPE._serialized_end=2324
+  _REMOTEBUILDSPEC._serialized_start=103
+  _REMOTEBUILDSPEC._serialized_end=722
+  _BUILDPROPERTIESV1._serialized_start=724
+  _BUILDPROPERTIESV1._serialized_end=827
+  _BUILDPROPERTIES._serialized_start=830
+  _BUILDPROPERTIES._serialized_end=972
+  _MODELURISPEC._serialized_start=975
+  _MODELURISPEC._serialized_end=1116
+  _BUILDENV._serialized_start=1118
+  _BUILDENV._serialized_end=1242
+  _DOCKERENV._serialized_start=1244
+  _DOCKERENV._serialized_end=1341
+  _PYTHONENV._serialized_start=1343
+  _PYTHONENV._serialized_end=1467
+  _CPURESOURCES._serialized_start=1469
+  _CPURESOURCES._serialized_end=1579
+  _GPURESOURCES._serialized_start=1581
+  _GPURESOURCES._serialized_end=1668
+  _DATATABLEDEFINITION._serialized_start=1671
+  _DATATABLEDEFINITION._serialized_end=1816
+  _DATACOLUMNDEFINITION._serialized_start=1818
+  _DATACOLUMNDEFINITION._serialized_end=1910
+  _DATAFORMAT._serialized_start=1912
+  _DATAFORMAT._serialized_end=1986
+  _CSVFORMAT._serialized_start=1988
+  _CSVFORMAT._serialized_end=2059
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
+import qwak.user_application.common.v0.resources_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -85,14 +86,15 @@
 class RemoteBuildSpec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUILD_PROPERTIES_FIELD_NUMBER: builtins.int
     BUILD_ENV_FIELD_NUMBER: builtins.int
     CPU_RESOURCES_FIELD_NUMBER: builtins.int
     GPU_RESOURCES_FIELD_NUMBER: builtins.int
+    CLIENT_POD_COMPUTE_RESOURCES_FIELD_NUMBER: builtins.int
     VERBOSE_FIELD_NUMBER: builtins.int
     BUILD_CODE_PATH_FIELD_NUMBER: builtins.int
     BUILD_CONFIG_FIELD_NUMBER: builtins.int
     BUILD_V1_FLAG_FIELD_NUMBER: builtins.int
     BUILD_PROPERTIES_V1_FIELD_NUMBER: builtins.int
     BUILD_STEPS_FIELD_NUMBER: builtins.int
     ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
@@ -103,14 +105,17 @@
     def build_env(self) -> global___BuildEnv: ...
     @property
     def cpu_resources(self) -> global___CpuResources:
         """CPU Properties"""
     @property
     def gpu_resources(self) -> global___GpuResources:
         """GPU Properties"""
+    @property
+    def client_pod_compute_resources(self) -> qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources:
+        """Build pod compute resources"""
     verbose: builtins.int
     """Logs verbose mode 0: warning, 1: info, 2: debug (by qwak.tools.logger.py VERBOSITY_LEVEL_MAPPING from qwak-sdk)"""
     build_code_path: builtins.str
     """The saved code path."""
     build_config: builtins.str
     """The build configuration yaml as json"""
     build_v1_flag: builtins.bool
@@ -128,26 +133,27 @@
     def __init__(
         self,
         *,
         build_properties: global___BuildProperties | None = ...,
         build_env: global___BuildEnv | None = ...,
         cpu_resources: global___CpuResources | None = ...,
         gpu_resources: global___GpuResources | None = ...,
+        client_pod_compute_resources: qwak.user_application.common.v0.resources_pb2.ClientPodComputeResources | None = ...,
         verbose: builtins.int = ...,
         build_code_path: builtins.str = ...,
         build_config: builtins.str = ...,
         build_v1_flag: builtins.bool = ...,
         build_properties_v1: global___BuildPropertiesV1 | None = ...,
         build_steps: collections.abc.Iterable[builtins.str] | None = ...,
         environment_id: builtins.str = ...,
         sdk_version: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_code_path", b"build_code_path", "build_config", b"build_config", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "build_steps", b"build_steps", "build_v1_flag", b"build_v1_flag", "cpu_resources", b"cpu_resources", "environment_id", b"environment_id", "gpu_resources", b"gpu_resources", "sdk_version", b"sdk_version", "verbose", b"verbose"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["Resources", b"Resources"]) -> typing_extensions.Literal["cpu_resources", "gpu_resources"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "client_pod_compute_resources", b"client_pod_compute_resources", "cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_code_path", b"build_code_path", "build_config", b"build_config", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "build_steps", b"build_steps", "build_v1_flag", b"build_v1_flag", "client_pod_compute_resources", b"client_pod_compute_resources", "cpu_resources", b"cpu_resources", "environment_id", b"environment_id", "gpu_resources", b"gpu_resources", "sdk_version", b"sdk_version", "verbose", b"verbose"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["Resources", b"Resources"]) -> typing_extensions.Literal["cpu_resources", "gpu_resources", "client_pod_compute_resources"] | None: ...
 
 global___RemoteBuildSpec = RemoteBuildSpec
 
 class BuildPropertiesV1(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUILD_CONFIG_URL_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.85/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.85/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/pyproject.toml` & `qwak_core-0.0.85/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.84"
+version = "0.0.85"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.84/qwak/automations/__init__.py` & `qwak_core-0.0.85/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/automations/automation_executions.py` & `qwak_core-0.0.85/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/automations/automations.py` & `qwak_core-0.0.85/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.85/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.85/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/automations/common.py` & `qwak_core-0.0.85/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.85/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.85/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.85/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.85/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.85/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/alert_management/client.py` & `qwak_core-0.0.85/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/analytics/client.py` & `qwak_core-0.0.85/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/audience/client.py` & `qwak_core-0.0.85/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/automation_management/client.py` & `qwak_core-0.0.85/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.85/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.85/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.85/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.85/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/build_management/client.py` & `qwak_core-0.0.85/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.85/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.85/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/deployment/client.py` & `qwak_core-0.0.85/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.85/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.85/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.85/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.85/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/instance_template/client.py` & `qwak_core-0.0.85/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.85/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/logging_client/client.py` & `qwak_core-0.0.85/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/model_management/client.py` & `qwak_core-0.0.85/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/project/client.py` & `qwak_core-0.0.85/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/secret_service/client.py` & `qwak_core-0.0.85/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.85/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.85/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.85/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.85/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.85/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.85/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.85/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.85/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.85/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.85/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/offline/client.py` & `qwak_core-0.0.85/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/feature_store/online/client.py` & `qwak_core-0.0.85/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/const.py` & `qwak_core-0.0.85/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.85/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.85/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.85/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.85/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/singleton_meta.py` & `qwak_core-0.0.85/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/tool/auth.py` & `qwak_core-0.0.85/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.85/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.85/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.85/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.85/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/__init__.py` & `qwak_core-0.0.85/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.85/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.85/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.85/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.85/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.85/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/base.py` & `qwak_core-0.0.85/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/decorators/api.py` & `qwak_core-0.0.85/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.85/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/experiment_tracking.py` & `qwak_core-0.0.85/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/schema.py` & `qwak_core-0.0.85/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/schema_entities.py` & `qwak_core-0.0.85/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.85/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.85/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.85/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.85/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.85/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.85/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.85/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.85/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/client.py` & `qwak_core-0.0.85/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.85/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/models/model.py` & `qwak_core-0.0.85/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.85/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.85/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/tools/logger/logger.py` & `qwak_core-0.0.85/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak/tools/logger/logging.yml` & `qwak_core-0.0.85/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.85/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/qwak_services_mock/services_mock.py` & `qwak_core-0.0.85/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.84/setup.py` & `qwak_core-0.0.85/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.84',
+    'version': '0.0.85',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.84/PKG-INFO` & `qwak_core-0.0.85/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.84
+Version: 0.0.85
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```


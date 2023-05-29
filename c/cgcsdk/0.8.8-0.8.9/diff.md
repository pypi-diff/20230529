# Comparing `tmp/cgcsdk-0.8.8.tar.gz` & `tmp/cgcsdk-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.8.tar", last modified: Mon May 29 15:00:35 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.9.tar", last modified: Mon May 29 15:08:51 2023, max compression
```

## Comparing `cgcsdk-0.8.8.tar` & `cgcsdk-0.8.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.144915 cgcsdk-0.8.8/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.8/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-05-29 15:00:35.143149 cgcsdk-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.902182 cgcsdk-0.8.8/cgc/
--rw-rw-rw-   0        0        0      234 2023-05-29 14:54:59.000000 cgcsdk-0.8.8/cgc/.env
--rw-rw-rw-   0        0        0     4114 2023-05-29 14:55:36.000000 cgcsdk-0.8.8/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.8.8/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.916392 cgcsdk-0.8.8/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.929061 cgcsdk-0.8.8/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.8.8/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.8.8/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.8.8/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.8.8/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.942778 cgcsdk-0.8.8/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.8.8/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.8/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.8.8/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.959104 cgcsdk-0.8.8/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.8/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.966629 cgcsdk-0.8.8/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.8/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.972492 cgcsdk-0.8.8/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.8/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.977364 cgcsdk-0.8.8/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:34.993508 cgcsdk-0.8.8/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.8/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.8/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.009961 cgcsdk-0.8.8/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.8/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.8/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2851 2023-05-29 14:58:18.000000 cgcsdk-0.8.8/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.016138 cgcsdk-0.8.8/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.8.8/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.022662 cgcsdk-0.8.8/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.8/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.051983 cgcsdk-0.8.8/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.8/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.8/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.092549 cgcsdk-0.8.8/cgc/utils/
--rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.8.8/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.8/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.8.8/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.100993 cgcsdk-0.8.8/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-05-18 13:48:23.000000 cgcsdk-0.8.8/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1218 2023-05-23 08:55:27.000000 cgcsdk-0.8.8/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.117828 cgcsdk-0.8.8/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.8/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.8/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.8.8/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.8.8/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-05-18 13:28:20.000000 cgcsdk-0.8.8/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.8.8/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.8/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.8/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:00:35.139052 cgcsdk-0.8.8/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 15:00:34.000000 cgcsdk-0.8.8/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 15:00:35.145358 cgcsdk-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.932999 cgcsdk-0.8.9/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-05-29 15:08:51.931951 cgcsdk-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.700304 cgcsdk-0.8.9/cgc/
+-rw-rw-rw-   0        0        0      234 2023-05-29 15:07:20.000000 cgcsdk-0.8.9/cgc/.env
+-rw-rw-rw-   0        0        0     4113 2023-05-29 15:07:13.000000 cgcsdk-0.8.9/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.8.9/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.717975 cgcsdk-0.8.9/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.729730 cgcsdk-0.8.9/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.8.9/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.8.9/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.8.9/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.8.9/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.741427 cgcsdk-0.8.9/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4061 2023-05-23 09:09:29.000000 cgcsdk-0.8.9/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.9/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.8.9/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.759374 cgcsdk-0.8.9/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.9/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.765427 cgcsdk-0.8.9/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.9/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.770844 cgcsdk-0.8.9/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.9/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.776939 cgcsdk-0.8.9/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.793866 cgcsdk-0.8.9/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.9/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.9/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.811945 cgcsdk-0.8.9/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.9/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.9/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2840 2023-05-29 15:06:35.000000 cgcsdk-0.8.9/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.818463 cgcsdk-0.8.9/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.8.9/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.825496 cgcsdk-0.8.9/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.9/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.855773 cgcsdk-0.8.9/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.9/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.9/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.887414 cgcsdk-0.8.9/cgc/utils/
+-rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.8.9/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.9/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-0.8.9/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.896595 cgcsdk-0.8.9/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-18 13:48:23.000000 cgcsdk-0.8.9/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-05-23 08:55:27.000000 cgcsdk-0.8.9/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.908591 cgcsdk-0.8.9/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.9/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.9/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1773 2023-05-23 09:05:26.000000 cgcsdk-0.8.9/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2488 2023-05-23 09:03:57.000000 cgcsdk-0.8.9/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-05-18 13:28:20.000000 cgcsdk-0.8.9/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.8.9/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.9/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.9/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:08:51.927923 cgcsdk-0.8.9/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 15:08:51.000000 cgcsdk-0.8.9/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:08:51.934060 cgcsdk-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.9/setup.py
```

### Comparing `cgcsdk-0.8.8/PKG-INFO` & `cgcsdk-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.8
+Version: 0.8.9
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.8/cgc/CHANGELOG.md` & `cgcsdk-0.8.9/cgc/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Change Log
 
-## 0.8.8
+## 0.8.8, 0.8.9
 
 Release on May 29, 2023.
 
-* hotfix: fixed typo in redis import in cgc.sdk
+* hotfix: fixed redis import in cgc.sdk
 
 ## 0.8.7
 
 Release on May 23, 2023.
 
 * hotfix: development changed .env file making it broken for new users
```

### Comparing `cgcsdk-0.8.8/cgc/cgc.py` & `cgcsdk-0.8.9/cgc/cgc.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.9/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.9/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.9/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.9/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.9/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.9/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.9/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.9/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.9/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/cgc_helpers.py` & `cgcsdk-0.8.9/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.9/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.9/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.9/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.9/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.9/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/resource/resource_cmd.py` & `cgcsdk-0.8.9/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.9/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.9/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.9/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.9/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/sdk/handlers.py` & `cgcsdk-0.8.9/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/sdk/mongodb.py` & `cgcsdk-0.8.9/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/sdk/postgresql.py` & `cgcsdk-0.8.9/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/sdk/redis.py` & `cgcsdk-0.8.9/cgc/sdk/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from redis.asyncio import Redis as redis_async
+import redis.asyncio as redis_async
 import redis
 
 
 class RedisConnector:
     redis_client_async = None
     redis_client = None
```

### Comparing `cgcsdk-0.8.8/cgc/server.crt` & `cgcsdk-0.8.9/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/telemetry/basic.py` & `cgcsdk-0.8.9/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/__init__.py` & `cgcsdk-0.8.9/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.9/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.9/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.9/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/tests/responses_tests.py` & `cgcsdk-0.8.9/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/__init__.py` & `cgcsdk-0.8.9/cgc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/click_group.py` & `cgcsdk-0.8.9/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/config_utils.py` & `cgcsdk-0.8.9/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.9/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.9/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.9/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.9/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.9/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.9/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/message_utils.py` & `cgcsdk-0.8.9/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.9/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/requests_helper.py` & `cgcsdk-0.8.9/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/response_utils.py` & `cgcsdk-0.8.9/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgc/utils/version_control.py` & `cgcsdk-0.8.9/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.9/cgcsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.8
+Version: 0.8.9
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.8/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.9/cgcsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.8/setup.py` & `cgcsdk-0.8.9/setup.py`

 * *Files identical despite different names*


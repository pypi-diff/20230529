# Comparing `tmp/oss2-2.9.0.tar.gz` & `tmp/oss2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oss2-2.9.0.tar", last modified: Sat Nov 16 04:00:05 2019, max compression
+gzip compressed data, was "dist/oss2-2.9.1.tar", last modified: Fri Dec 27 05:00:43 2019, max compression
```

## Comparing `oss2-2.9.0.tar` & `oss2-2.9.1.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/examples/
--rw-r--r--   0 root         (0) root         (0)     6202 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/bucket_website.py
--rw-r--r--   0 root         (0) root         (0)     2220 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/traffic_limit.py
--rw-r--r--   0 root         (0) root         (0)     7163 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_post.py
--rw-r--r--   0 root         (0) root         (0)     1176 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/bucket_user_qos.py
--rw-r--r--   0 root         (0) root         (0)     5175 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/custom_crypto.py
--rw-r--r--   0 root         (0) root         (0)     3330 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/image.py
--rw-r--r--   0 root         (0) root         (0)     2016 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/select_csv.py
--rw-r--r--   0 root         (0) root         (0)     1506 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_request_payment.py
--rw-r--r--   0 root         (0) root         (0)     5726 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/live_channel.py
--rw-r--r--   0 root         (0) root         (0)     3268 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_basic.py
--rw-r--r--   0 root         (0) root         (0)     2909 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_crypto.py
--rw-r--r--   0 root         (0) root         (0)     3710 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/sts.py
--rw-r--r--   0 root         (0) root         (0)     3974 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_progress.py
--rw-r--r--   0 root         (0) root         (0)     3889 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/bucket.py
--rw-r--r--   0 root         (0) root         (0)     1881 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_server_crypto.py
--rw-r--r--   0 root         (0) root         (0)     2944 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_extra.py
--rw-r--r--   0 root         (0) root         (0)     6069 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_check.py
--rw-r--r--   0 root         (0) root         (0)     3369 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/object_callback.py
--rw-r--r--   0 root         (0) root         (0)     2016 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/bucket_policy.py
--rw-r--r--   0 root         (0) root         (0)     3178 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/sign_v2.py
--rw-r--r--   0 root         (0) root         (0)     3263 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/qos_info.py
--rw-r--r--   0 root         (0) root         (0)     2517 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/download.py
--rw-r--r--   0 root         (0) root         (0)     3341 2019-11-16 03:56:17.000000 oss2-2.9.0/examples/upload.py
--rw-r--r--   0 root         (0) root         (0)     1595 2019-11-16 03:56:17.000000 oss2-2.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/oss2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6881 2019-11-16 04:00:04.000000 oss2-2.9.0/oss2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2145 2019-11-16 04:00:04.000000 oss2-2.9.0/oss2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        5 2019-11-16 04:00:04.000000 oss2-2.9.0/oss2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      110 2019-11-16 04:00:04.000000 oss2-2.9.0/oss2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-16 04:00:04.000000 oss2-2.9.0/oss2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     6050 2019-11-16 03:56:17.000000 oss2-2.9.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     1053 2019-11-16 03:56:17.000000 oss2-2.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      134 2019-11-16 03:56:17.000000 oss2-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6881 2019-11-16 04:00:05.000000 oss2-2.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4869 2019-11-16 03:56:17.000000 oss2-2.9.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/tests/
--rw-r--r--   0 root         (0) root         (0)    11722 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_live_channel.py
--rw-r--r--   0 root         (0) root         (0)    30866 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_object_request_payment.py
--rw-r--r--   0 root         (0) root         (0)    45267 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_mock_bucket.py
--rw-r--r--   0 root         (0) root         (0)    55250 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_object.py
--rw-r--r--   0 root         (0) root         (0)     7220 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_bucket_versioning.py
--rw-r--r--   0 root         (0) root         (0)     3899 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_image.py
--rw-r--r--   0 root         (0) root         (0)        0 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22026 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_select_csv_object.py
--rw-r--r--   0 root         (0) root         (0)     4579 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_sts.py
--rw-r--r--   0 root         (0) root         (0)    14222 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2530 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_crc64_combine.py
--rw-r--r--   0 root         (0) root         (0)     8176 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_mock_multipart.py
--rw-r--r--   0 root         (0) root         (0)     7136 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/common.py
--rw-r--r--   0 root         (0) root         (0)    36941 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_object_versioning.py
--rw-r--r--   0 root         (0) root         (0)     1046 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_headers.py
--rw-r--r--   0 root         (0) root         (0)     2512 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_chinese.py
--rw-r--r--   0 root         (0) root         (0)     3328 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_api_base.py
--rw-r--r--   0 root         (0) root         (0)      689 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_request_payment.py
--rw-r--r--   0 root         (0) root         (0)     7322 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_crypto.py
--rw-r--r--   0 root         (0) root         (0)    11066 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     5460 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_lifecycle_versioning.py
--rw-r--r--   0 root         (0) root         (0)     7307 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_qos_info.py
--rw-r--r--   0 root         (0) root         (0)    39913 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_mock_object.py
--rw-r--r--   0 root         (0) root         (0)    25691 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_website.py
--rw-r--r--   0 root         (0) root         (0)      825 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_init.py
--rw-r--r--   0 root         (0) root         (0)     7242 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_multipart.py
--rw-r--r--   0 root         (0) root         (0)    18283 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_select_json_object.py
--rw-r--r--   0 root         (0) root         (0)     3245 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_object_request_payment_versions.py
--rw-r--r--   0 root         (0) root         (0)    38728 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_bucket.py
--rw-r--r--   0 root         (0) root         (0)    10897 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_traffic_limit.py
--rw-r--r--   0 root         (0) root         (0)     6815 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_iterator.py
--rw-r--r--   0 root         (0) root         (0)    23802 2019-11-16 03:56:17.000000 oss2-2.9.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-11-16 04:00:05.000000 oss2-2.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/unittests/
--rw-r--r--   0 root         (0) root         (0)    20748 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_object.py
--rw-r--r--   0 root         (0) root         (0)      993 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_xml_utils.py
--rw-r--r--   0 root         (0) root         (0)       32 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13732 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/common.py
--rw-r--r--   0 root         (0) root         (0)    18195 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_select_object.py
--rw-r--r--   0 root         (0) root         (0)     6783 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_multipart.py
--rw-r--r--   0 root         (0) root         (0)     1257 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_resumable.py
--rw-r--r--   0 root         (0) root         (0)    27870 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_bucket.py
--rw-r--r--   0 root         (0) root         (0)     2723 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_task_queue.py
--rw-r--r--   0 root         (0) root         (0)    19642 2019-11-16 03:56:17.000000 oss2-2.9.0/unittests/test_iterator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-11-16 04:00:05.000000 oss2-2.9.0/oss2/
--rw-r--r--   0 root         (0) root         (0)     1210 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/select_params.py
--rw-r--r--   0 root         (0) root         (0)    52083 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/models.py
--rw-r--r--   0 root         (0) root         (0)     2456 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7916 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/exceptions.py
--rw-r--r--   0 root         (0) root         (0)   118866 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/api.py
--rw-r--r--   0 root         (0) root         (0)      887 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/defaults.py
--rw-r--r--   0 root         (0) root         (0)    22893 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/utils.py
--rw-r--r--   0 root         (0) root         (0)     4913 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/crc64_combine.py
--rw-r--r--   0 root         (0) root         (0)    14422 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/auth.py
--rw-r--r--   0 root         (0) root         (0)     9415 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/crypto.py
--rw-r--r--   0 root         (0) root         (0)     5484 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/http.py
--rw-r--r--   0 root         (0) root         (0)    10393 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/iterators.py
--rw-r--r--   0 root         (0) root         (0)    53646 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/xml_utils.py
--rw-r--r--   0 root         (0) root         (0)     2242 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/compat.py
--rw-r--r--   0 root         (0) root         (0)     1702 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/headers.py
--rw-r--r--   0 root         (0) root         (0)     2311 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/task_queue.py
--rw-r--r--   0 root         (0) root         (0)    10063 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/select_response.py
--rw-r--r--   0 root         (0) root         (0)    32944 2019-11-16 03:56:17.000000 oss2-2.9.0/oss2/resumable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/examples/
+-rw-r--r--   0 root         (0) root         (0)     6202 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/bucket_website.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/traffic_limit.py
+-rw-r--r--   0 root         (0) root         (0)     7163 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_post.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/bucket_user_qos.py
+-rw-r--r--   0 root         (0) root         (0)     5175 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/custom_crypto.py
+-rw-r--r--   0 root         (0) root         (0)     3330 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/image.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/select_csv.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_request_payment.py
+-rw-r--r--   0 root         (0) root         (0)     5726 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/live_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_basic.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_crypto.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/sts.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_progress.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_server_crypto.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_extra.py
+-rw-r--r--   0 root         (0) root         (0)     6069 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_check.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/object_callback.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/bucket_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/sign_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3263 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/qos_info.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/download.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2019-11-16 03:56:17.000000 oss2-2.9.1/examples/upload.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2019-12-27 04:58:52.000000 oss2-2.9.1/examples/async_fetch_task.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2019-12-27 04:58:52.000000 oss2-2.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7015 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2205 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     6403 2019-12-27 04:58:52.000000 oss2-2.9.1/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     1053 2019-11-16 03:56:17.000000 oss2-2.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      134 2019-11-16 03:56:17.000000 oss2-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7015 2019-12-27 05:00:43.000000 oss2-2.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4869 2019-11-16 03:56:17.000000 oss2-2.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/tests/
+-rw-r--r--   0 root         (0) root         (0)    11722 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_live_channel.py
+-rw-r--r--   0 root         (0) root         (0)    31810 2019-12-27 04:58:52.000000 oss2-2.9.1/tests/test_object_request_payment.py
+-rw-r--r--   0 root         (0) root         (0)    45267 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_mock_bucket.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2019-12-27 04:58:52.000000 oss2-2.9.1/tests/test_object.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_bucket_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_image.py
+-rw-r--r--   0 root         (0) root         (0)        0 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22026 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_select_csv_object.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_sts.py
+-rw-r--r--   0 root         (0) root         (0)    14222 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_crc64_combine.py
+-rw-r--r--   0 root         (0) root         (0)     8176 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_mock_multipart.py
+-rw-r--r--   0 root         (0) root         (0)     7136 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)    36941 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_object_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_headers.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_api_base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_request_payment.py
+-rw-r--r--   0 root         (0) root         (0)     7322 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_crypto.py
+-rw-r--r--   0 root         (0) root         (0)    12022 2019-12-27 04:58:52.000000 oss2-2.9.1/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     5460 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_lifecycle_versioning.py
+-rw-r--r--   0 root         (0) root         (0)     7307 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_qos_info.py
+-rw-r--r--   0 root         (0) root         (0)    39913 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_mock_object.py
+-rw-r--r--   0 root         (0) root         (0)    25691 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_website.py
+-rw-r--r--   0 root         (0) root         (0)      825 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_init.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2019-12-27 04:58:52.000000 oss2-2.9.1/tests/test_multipart.py
+-rw-r--r--   0 root         (0) root         (0)    18283 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_select_json_object.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_object_request_payment_versions.py
+-rw-r--r--   0 root         (0) root         (0)    38728 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_bucket.py
+-rw-r--r--   0 root         (0) root         (0)    10897 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_traffic_limit.py
+-rw-r--r--   0 root         (0) root         (0)     6815 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_iterator.py
+-rw-r--r--   0 root         (0) root         (0)    23802 2019-11-16 03:56:17.000000 oss2-2.9.1/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     6586 2019-12-27 04:58:52.000000 oss2-2.9.1/tests/test_async_fetch_task.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-12-27 05:00:43.000000 oss2-2.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/unittests/
+-rw-r--r--   0 root         (0) root         (0)    20748 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_object.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2019-12-27 04:58:52.000000 oss2-2.9.1/unittests/test_xml_utils.py
+-rw-r--r--   0 root         (0) root         (0)       32 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13732 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/common.py
+-rw-r--r--   0 root         (0) root         (0)    18195 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_select_object.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_multipart.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_resumable.py
+-rw-r--r--   0 root         (0) root         (0)    27870 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_task_queue.py
+-rw-r--r--   0 root         (0) root         (0)    19642 2019-11-16 03:56:17.000000 oss2-2.9.1/unittests/test_iterator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-27 05:00:43.000000 oss2-2.9.1/oss2/
+-rw-r--r--   0 root         (0) root         (0)     1210 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/select_params.py
+-rw-r--r--   0 root         (0) root         (0)    54787 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/models.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8006 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)   121570 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/api.py
+-rw-r--r--   0 root         (0) root         (0)      887 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    22893 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/crc64_combine.py
+-rw-r--r--   0 root         (0) root         (0)    17323 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/auth.py
+-rw-r--r--   0 root         (0) root         (0)     9415 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/crypto.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/http.py
+-rw-r--r--   0 root         (0) root         (0)    10393 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/iterators.py
+-rw-r--r--   0 root         (0) root         (0)    55679 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/xml_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/compat.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/headers.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/task_queue.py
+-rw-r--r--   0 root         (0) root         (0)    10063 2019-11-16 03:56:17.000000 oss2-2.9.1/oss2/select_response.py
+-rw-r--r--   0 root         (0) root         (0)    33999 2019-12-27 04:58:52.000000 oss2-2.9.1/oss2/resumable.py
```

### Comparing `oss2-2.9.0/examples/bucket_website.py` & `oss2-2.9.1/examples/bucket_website.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/traffic_limit.py` & `oss2-2.9.1/examples/traffic_limit.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_post.py` & `oss2-2.9.1/examples/object_post.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/bucket_user_qos.py` & `oss2-2.9.1/examples/bucket_user_qos.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/custom_crypto.py` & `oss2-2.9.1/examples/custom_crypto.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/image.py` & `oss2-2.9.1/examples/image.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/select_csv.py` & `oss2-2.9.1/examples/select_csv.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_request_payment.py` & `oss2-2.9.1/examples/object_request_payment.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/live_channel.py` & `oss2-2.9.1/examples/live_channel.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_basic.py` & `oss2-2.9.1/examples/object_basic.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_crypto.py` & `oss2-2.9.1/examples/object_crypto.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/sts.py` & `oss2-2.9.1/examples/sts.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_progress.py` & `oss2-2.9.1/examples/object_progress.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/bucket.py` & `oss2-2.9.1/examples/bucket.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_server_crypto.py` & `oss2-2.9.1/examples/object_server_crypto.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_extra.py` & `oss2-2.9.1/examples/object_extra.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_check.py` & `oss2-2.9.1/examples/object_check.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/object_callback.py` & `oss2-2.9.1/examples/object_callback.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/bucket_policy.py` & `oss2-2.9.1/examples/bucket_policy.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/sign_v2.py` & `oss2-2.9.1/examples/sign_v2.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/qos_info.py` & `oss2-2.9.1/examples/qos_info.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/download.py` & `oss2-2.9.1/examples/download.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/examples/upload.py` & `oss2-2.9.1/examples/upload.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/setup.py` & `oss2-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,10 +42,12 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5'
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7'
     ]
 )
```

### Comparing `oss2-2.9.0/oss2.egg-info/PKG-INFO` & `oss2-2.9.1/oss2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: oss2
-Version: 2.9.0
+Version: 2.9.1
 Summary: Aliyun OSS (Object Storage Service) SDK
 Home-page: http://oss.aliyun.com
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
+Description-Content-Type: UNKNOWN
 Description: Alibaba Cloud OSS SDK for Python
         ================================
         
         .. image:: https://badge.fury.io/py/oss2.svg
             :target: https://badge.fury.io/py/oss2
         .. image:: https://travis-ci.org/aliyun/aliyun-oss-python-sdk.svg?branch=master
             :target: https://travis-ci.org/aliyun/aliyun-oss-python-sdk
@@ -167,7 +168,9 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `oss2-2.9.0/oss2.egg-info/SOURCES.txt` & `oss2-2.9.1/oss2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
+examples/async_fetch_task.py
 examples/bucket.py
 examples/bucket_policy.py
 examples/bucket_user_qos.py
 examples/bucket_website.py
 examples/custom_crypto.py
 examples/download.py
 examples/image.py
@@ -48,14 +49,15 @@
 oss2.egg-info/SOURCES.txt
 oss2.egg-info/dependency_links.txt
 oss2.egg-info/requires.txt
 oss2.egg-info/top_level.txt
 tests/__init__.py
 tests/common.py
 tests/test_api_base.py
+tests/test_async_fetch_task.py
 tests/test_bucket.py
 tests/test_bucket_versioning.py
 tests/test_chinese.py
 tests/test_crc64_combine.py
 tests/test_crypto.py
 tests/test_download.py
 tests/test_headers.py
```

### Comparing `oss2-2.9.0/CHANGELOG.rst` & `oss2-2.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 OSS SDK for Python 版本记录
 ===========================
 
 Python SDK的版本号遵循 `Semantic Versioning <http://semver.org/>`_ 规则。
 
+Version 2.9.1
+-------------
+- 增加：异步fetch 接口
+- 增加：签名url支持访问者付费参数
+- 增加：分片上传支持sequential参数，支持分片上传的文件返回content-md5
+- 增加：支持python3.6 & python3.7
+- 优化：在python3下，支持传入bytes类型数据
+- 优化：GetBucketInfo api 兼容低版本后台服务
+
 Version 2.9.0
 -------------
 - 增加：面向用户的QOS查询设置接口
 - 增加：支持在创建bucket时设置容灾类型
 - 增加：GetVodPlaylist 接口，支持获取指定时间播放列表 
 - 增加：sign url接口新增 slash-safe参数，避免'/'转义成'%2F'
 - 增加：Storage Capacity 接口，支持设置Bucket容量
```

### Comparing `oss2-2.9.0/LICENSE` & `oss2-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/PKG-INFO` & `oss2-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: oss2
-Version: 2.9.0
+Version: 2.9.1
 Summary: Aliyun OSS (Object Storage Service) SDK
 Home-page: http://oss.aliyun.com
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
+Description-Content-Type: UNKNOWN
 Description: Alibaba Cloud OSS SDK for Python
         ================================
         
         .. image:: https://badge.fury.io/py/oss2.svg
             :target: https://badge.fury.io/py/oss2
         .. image:: https://travis-ci.org/aliyun/aliyun-oss-python-sdk.svg?branch=master
             :target: https://travis-ci.org/aliyun/aliyun-oss-python-sdk
@@ -167,7 +168,9 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
```

### Comparing `oss2-2.9.0/README.rst` & `oss2-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_live_channel.py` & `oss2-2.9.1/tests/test_live_channel.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_object_request_payment.py` & `oss2-2.9.1/tests/test_object_request_payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,11 +744,35 @@
 
         # PartIterator with payer setting, should be successful.
         headers = dict()
         headers[OSS_REQUEST_PAYER] = "requester"
         up_iter = oss2.PartIterator(self.payer_bucket, key, upload_id, headers=headers)
         for up in up_iter:
             pass
-    
+
+    def test_put_object_with_signed_url(self):
+        key = 'request-payment-test-put-object-signed-url'
+        file_name = self._prepare_temp_file_with_size(1024)
+
+        params = dict()
+        params[OSS_REQUEST_PAYER] = "requester" 
+        url = self.payer_bucket.sign_url('PUT', key, 60, params=params)
+        self.payer_bucket.put_object_with_url_from_file(url, file_name)
+
+    def test_get_object_with_signed_url(self):
+        key = 'request-payment-test-get-object-signed-url'
+        content = b'a' * 1024
+        file_name = key + '.txt'
+
+        result = self.bucket.put_object(key, content);
+        self.assertEqual(result.status, 200)
+
+        params = dict()
+        params[OSS_REQUEST_PAYER] = "requester"
+        url = self.payer_bucket.sign_url('GET', key, 60, params=params)
+        result = self.payer_bucket.get_object_with_url_to_file(url, file_name)
+
+        os.remove(file_name)
+        self.bucket.delete_object(key)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oss2-2.9.0/tests/test_mock_bucket.py` & `oss2-2.9.1/tests/test_mock_bucket.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_object.py` & `oss2-2.9.1/tests/test_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from oss2.exceptions import (ClientError, RequestError, NoSuchBucket, OpenApiServerError,
         NotFound, NoSuchKey, Conflict, PositionNotEqualToLength, ObjectNotAppendable)
 
 from oss2.compat import is_py2, is_py33
 from oss2.models import Tagging, TaggingRule
 from oss2.headers import OSS_OBJECT_TAGGING, OSS_OBJECT_TAGGING_COPY_DIRECTIVE
-from oss2.compat import urlunquote, urlquote
+from oss2.compat import urlunquote, urlquote, to_bytes, to_string
 
 from .common import *
 
 
 def now():
     return int(calendar.timegm(time.gmtime()))
 
@@ -1451,14 +1451,29 @@
 
         head_result = self.bucket.head_object(symlink)
         self.assertEqual(head_result.content_length, len(content))
         self.assertEqual(head_result.etag, '5D41402ABC4B2A76B9719D911017C592')
         self.assertEqual(head_result.headers['x-oss-meta-key1'], 'value1')
         self.assertEqual(head_result.headers['x-oss-meta-key2'], 'value2')
 
+    def test_put_object_with_unicode_header(self):
+        key = self.random_key()
+        value = '测试'
+        byte = to_bytes(value)
+        headers={'x-oss-meta-unicode': byte}
+        self.bucket.put_object(key, 'a novel', headers=headers)
+        result = self.bucket.head_object(key)
+        self.assertEqual(result.status, 200)
+        newstr = result.headers['x-oss-meta-unicode']
+        if is_py2:
+            b_str = newstr
+        else:
+            b_str = newstr.encode('iso-8859-1')
+        self.assertEqual(to_string(b_str), value)
+
     
 class TestSign(TestObject):
     """
         这个类主要是用来增加测试覆盖率，当环境变量为oss2.AUTH_VERSION_2，则重新设置为oss2.AUTH_VERSION_1再运行TestObject，反之亦然
     """
     def __init__(self, *args, **kwargs):
         super(TestSign, self).__init__(*args, **kwargs)
```

### Comparing `oss2-2.9.0/tests/test_bucket_versioning.py` & `oss2-2.9.1/tests/test_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_image.py` & `oss2-2.9.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_select_csv_object.py` & `oss2-2.9.1/tests/test_select_csv_object.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_sts.py` & `oss2-2.9.1/tests/test_sts.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_utils.py` & `oss2-2.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_crc64_combine.py` & `oss2-2.9.1/tests/test_crc64_combine.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_mock_multipart.py` & `oss2-2.9.1/tests/test_mock_multipart.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/common.py` & `oss2-2.9.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_object_versioning.py` & `oss2-2.9.1/tests/test_object_versioning.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_headers.py` & `oss2-2.9.1/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_chinese.py` & `oss2-2.9.1/tests/test_chinese.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_api_base.py` & `oss2-2.9.1/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_request_payment.py` & `oss2-2.9.1/tests/test_request_payment.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_crypto.py` & `oss2-2.9.1/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_upload.py` & `oss2-2.9.1/tests/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -306,10 +306,32 @@
         self.bucket.delete_object_tagging(key)
         
         result = self.bucket.get_object_tagging(key)
         
         self.assertEqual(0, result.tag_set.len())
         self.bucket.delete_object(key)
 
+    def test_upload_sequenial(self):
+        endpoint = "http://oss-cn-shanghai.aliyuncs.com"
+        auth = oss2.Auth(OSS_ID, OSS_SECRET)
+        bucket_name = OSS_BUCKET + "-test-upload-sequential"
+        bucket = oss2.Bucket(auth, endpoint, bucket_name)
+        bucket.create_bucket()
+
+        key = random_string(16)
+        content = random_bytes(5 * 100 * 1024)
+        pathname = self._prepare_temp_file(content)
+
+        oss2.resumable_upload(bucket, key, pathname, multipart_threshold=200 * 1024, part_size=None)
+        result = bucket.get_object(key)
+        self.assertIsNone(result.resp.headers.get('Content-MD5'))
+
+        params={'sequential' : ''}
+        oss2.resumable_upload(bucket, key, pathname, multipart_threshold=200 * 1024, part_size=None, params=params)
+        result = bucket.get_object(key)
+        self.assertIsNotNone(result.resp.headers.get('Content-MD5'))
+
+        bucket.delete_object(key)
+        bucket.delete_bucket()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oss2-2.9.0/tests/test_lifecycle_versioning.py` & `oss2-2.9.1/tests/test_lifecycle_versioning.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_qos_info.py` & `oss2-2.9.1/tests/test_qos_info.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_mock_object.py` & `oss2-2.9.1/tests/test_mock_object.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_website.py` & `oss2-2.9.1/tests/test_website.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_init.py` & `oss2-2.9.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_multipart.py` & `oss2-2.9.1/tests/test_multipart.py`

 * *Files 16% similar despite different names*

```diff
@@ -202,10 +202,43 @@
         result = self.bucket.get_object_tagging(key)
 
         self.assertEqual(2, result.tag_set.len())
         self.assertEqual('.-', result.tag_set.tagging_rule['+:/'])
         self.assertEqual('中文', result.tag_set.tagging_rule[' + '])
 
         result = self.bucket.delete_object_tagging(key)
-   
+
+    def test_multipart_sequential(self): 
+        endpoint = "http://oss-cn-shanghai.aliyuncs.com"
+        auth = oss2.Auth(OSS_ID, OSS_SECRET)
+        bucket_name = OSS_BUCKET + "-test-multipart-sequential"
+        bucket = oss2.Bucket(auth, endpoint, bucket_name)
+        bucket.create_bucket()
+
+        key = self.random_key()
+        content = random_bytes(128 * 1024)
+
+        parts = []
+        upload_id = bucket.init_multipart_upload(key).upload_id
+        result = bucket.upload_part(key, upload_id, 1, content)
+        parts.append(oss2.models.PartInfo(1, result.etag, size=len(content), part_crc=result.crc))
+        bucket.complete_multipart_upload(key, upload_id, parts)
+        
+        result = bucket.get_object(key)
+        self.assertIsNone(result.resp.headers.get('Content-MD5'))
+
+        parts = []
+        params = {'sequential':''}
+        upload_id = bucket.init_multipart_upload(key, params=params).upload_id
+        result = bucket.upload_part(key, upload_id, 1, content)
+        parts.append(oss2.models.PartInfo(1, result.etag, size=len(content), part_crc=result.crc))
+        bucket.complete_multipart_upload(key, upload_id, parts)
+
+        result = bucket.get_object(key)
+        self.assertIsNotNone(result.resp.headers.get('Content-MD5'))
+
+        bucket.delete_object(key)
+        bucket.delete_bucket()
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `oss2-2.9.0/tests/test_select_json_object.py` & `oss2-2.9.1/tests/test_select_json_object.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_object_request_payment_versions.py` & `oss2-2.9.1/tests/test_object_request_payment_versions.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_bucket.py` & `oss2-2.9.1/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_traffic_limit.py` & `oss2-2.9.1/tests/test_traffic_limit.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_iterator.py` & `oss2-2.9.1/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/tests/test_download.py` & `oss2-2.9.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_object.py` & `oss2-2.9.1/unittests/test_object.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/common.py` & `oss2-2.9.1/unittests/common.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_select_object.py` & `oss2-2.9.1/unittests/test_select_object.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_multipart.py` & `oss2-2.9.1/unittests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_resumable.py` & `oss2-2.9.1/unittests/test_resumable.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_bucket.py` & `oss2-2.9.1/unittests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_task_queue.py` & `oss2-2.9.1/unittests/test_task_queue.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/unittests/test_iterator.py` & `oss2-2.9.1/unittests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/select_params.py` & `oss2-2.9.1/oss2/select_params.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/models.py` & `oss2-2.9.1/oss2/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1510,7 +1510,85 @@
     def __init__(self, storage_capacity=None):
         self.storage_capacity = storage_capacity
 
 class GetBucketUserQosResult(RequestResult, BucketUserQos):
     def __init__(self, resp):
         RequestResult.__init__(self, resp)
         BucketUserQos.__init__(self)
+
+
+ASYNC_FETCH_TASK_STATE_RUNNING = 'Running'
+ASYNC_FETCH_TASK_STATE_RETRY = 'Retry'
+ASYNC_FETCH_TASK_STATE_FETCH_SUCCESS_CALLBACK_FAILED = 'FetchSuccessCallbackFailed'
+ASYNC_FETCH_TASK_STATE_FAILED= 'Failed'
+ASYNC_FETCH_TASK_STATE_SUCCESS = 'Success'
+
+class AsyncFetchTaskConfiguration(object):
+    """异步获取文件到bucket到任务配置项
+
+    :param url: 源文件url
+    :type url: str
+
+    :param object_name: 文件的名称。
+    :type task_state: str
+
+    :param host: 文件所在服务器的host，如果不指定则会根据url解析填充。
+    :type host: str
+
+    :param content_md5: 指定校验源文件的md5
+    :type content_md5: str
+
+    :param callback: 指定fetch成功知乎回调给用户的引用服务器，如果不指定则不回调。
+            callback格式与OSS上传回调的请求头callback一致，详情见官网。
+    :type callback: str
+
+    :param ignore_same_key: 默认为True表示如果文件已存在则忽略本次任务，api调用将会报错。如果为False，则会覆盖已存在的object。
+    :type ignore_same_key: bool
+    """
+    def __init__(self, 
+            url, 
+            object_name,
+            host = None,
+            content_md5 = None,
+            callback = None,
+            ignore_same_key = None):
+
+        self.url = url
+        self.object_name = object_name
+        self.host = host
+        self.content_md5 = content_md5
+        self.callback = callback
+        self.ignore_same_key = ignore_same_key
+
+class PutAsyncFetchTaskResult(RequestResult):
+    def __init__(self, resp, task_id=None):
+        RequestResult.__init__(self, resp)
+        self.task_id = task_id
+
+class GetAsyncFetchTaskResult(RequestResult):
+    """获取异步获取文件到bucket的任务的返回结果
+
+    :param task_id: 任务id
+    :type task_id: str
+
+    :param task_state: 取值范围：oss2.models.ASYNC_FETCH_TASK_STATE_RUNNING, oss2.models.ASYNC_FETCH_TASK_STATE_RETRY, 
+            oss2.models.ASYNC_FETCH_TASK_STATE_FETCH_SUCCESS_CALLBACK_FAILED, oss2.models.ASYNC_FETCH_TASK_STATE_FAILED, 
+            oss2.models.ASYNC_FETCH_TASK_STATE_SUCCESS。
+    :type task_state: str
+
+    :param error_msg: 错误信息
+    :type error_msg: str
+
+    :param task_config: 任务配置信息
+    :type task_config: class:`AsyncFetchTaskConfiguration <oss2.models.AsyncFetchTaskConfiguration>`
+    """
+    def __init__(self, resp, 
+            task_id=None, 
+            task_state=None, 
+            error_msg=None, 
+            task_config=None):
+
+        RequestResult.__init__(self, resp)
+        self.task_id = task_id
+        self.task_state = task_state
+        self.error_msg = error_msg
+        self.task_config = task_config
```

### Comparing `oss2-2.9.0/oss2/__init__.py` & `oss2-2.9.1/oss2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.9.0'
+__version__ = '2.9.1'
 
 from . import models, exceptions
 
 from .api import Service, Bucket, CryptoBucket
 from .auth import Auth, AuthV2, AnonymousAuth, StsAuth, AUTH_VERSION_1, AUTH_VERSION_2, make_auth
 from .http import Session, CaseInsensitiveDict
```

### Comparing `oss2-2.9.0/oss2/exceptions.py` & `oss2-2.9.1/oss2/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,17 @@
                 'message': self.message}
         return str(error)
 
 class SignatureDoesNotMatch(ServerError):
     status = 403
     code = 'SignatureDoesNotMatch'
 
+class ObjectAlreadyExists(ServerError):
+    status = 400
+    code = 'ObjectAlreadyExists'
 
 def make_exception(resp):
     status = resp.status
     headers = resp.headers
     body = resp.read(4096)
     details = _parse_error_body(body)
     code = details.get('Code', '')
```

### Comparing `oss2-2.9.0/oss2/api.py` & `oss2-2.9.1/oss2/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,16 @@
     VERSIONID = 'versionId'
     RESTORE = 'restore'
     OBJECTMETA = 'objectMeta'
     POLICY = 'policy'
     REQUESTPAYMENT  = 'requestPayment'
     QOS_INFO = 'qosInfo'
     USER_QOS = 'qos'
+    ASYNC_FETCH = 'asyncFetch'
+    SEQUENTIAL = 'sequential'
 
     def __init__(self, auth, endpoint, bucket_name,
                  is_cname=False,
                  session=None,
                  connect_timeout=None,
                  app_name='',
                  enable_crc=True):
@@ -1203,31 +1205,37 @@
         resp = self.__do_object('POST', '',
                                 data=data,
                                 params={'delete': '', 'encoding-type': 'url'},
                                 headers=headers)
         logger.debug("Delete object versions done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return self._parse_result(resp, xml_utils.parse_batch_delete_objects, BatchDeleteObjectsResult)
 
-    def init_multipart_upload(self, key, headers=None):
+    def init_multipart_upload(self, key, headers=None, params=None):
         """初始化分片上传。
 
         返回值中的 `upload_id` 以及Bucket名和Object名三元组唯一对应了此次分片上传事件。
 
         :param str key: 待上传的文件名
 
         :param headers: HTTP头部
         :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
 
         :return: :class:`InitMultipartUploadResult <oss2.models.InitMultipartUploadResult>`
         """
         headers = utils.set_content_type(http.CaseInsensitiveDict(headers), key)
 
-        logger.debug("Start to init multipart upload, bucket: {0}, keys: {1}, headers: {2}".format(
-            self.bucket_name, to_string(key), headers))
-        resp = self.__do_object('POST', key, params={'uploads': ''}, headers=headers)
+        if params is None:
+            tmp_params = dict()
+        else:
+            tmp_params = params.copy()
+
+        tmp_params['uploads'] = ''
+        logger.debug("Start to init multipart upload, bucket: {0}, keys: {1}, headers: {2}, params: {3}".format(
+            self.bucket_name, to_string(key), headers, tmp_params))
+        resp = self.__do_object('POST', key, params=tmp_params, headers=headers)
         logger.debug("Init multipart upload done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return self._parse_result(resp, xml_utils.parse_init_multipart_upload, InitMultipartUploadResult)
 
     def upload_part(self, key, upload_id, part_number, data, progress_callback=None, headers=None):
         """上传一个分片。
 
         :param str key: 待上传文件名，这个文件名要和 :func:`init_multipart_upload` 的文件名一致。
@@ -2059,60 +2067,59 @@
     def put_bucket_versioning(self, config, headers=None):
         """
 
         :param str operation: 设置bucket是否开启多版本特性，可取值为:[Enabled,Suspend] 
 
         :return: :class:`RequestResult <oss2.models.RequestResult>`
         """
-        logger.debug("Start to put object versioning, bucket: {0}".format(
-            self.bucket_name))
+        logger.debug("Start to put object versioning, bucket: {0}".format(self.bucket_name))
         data = self.__convert_data(BucketVersioningConfig, xml_utils.to_put_bucket_versioning, config) 
 
         headers = http.CaseInsensitiveDict(headers)
         headers['Content-MD5'] = utils.content_md5(data)
 
         resp = self.__do_bucket('PUT', data=data, params={Bucket.VERSIONING: ''}, headers=headers)
+        logger.debug("Put bucket versiong done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return RequestResult(resp)
 
     def get_bucket_versioning(self):
         """
         :return: :class:`GetBucketVersioningResult<oss2.models.GetBucketVersioningResult>` 
         """
-        logger.debug("Start to get bucket versioning, bucket: {0}".format(
-                    self.bucket_name))
-        
+        logger.debug("Start to get bucket versioning, bucket: {0}".format(self.bucket_name))
         resp = self.__do_bucket('GET', params={Bucket.VERSIONING: ''})
+        logger.debug("Get bucket versiong done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return self._parse_result(resp, xml_utils.parse_get_bucket_versioning, GetBucketVersioningResult)
 
     def put_bucket_policy(self, policy):
-        """设置bucket policy, 具体policy书写规则请参考官方文档
-        :param str policy: 
-        """
-
-        logger.debug("Start to put bucket policy, bucket: {0}, policy: {1}".format(
-            self.bucket_name, policy))
+        """设置bucket授权策略, 具体policy书写规则请参考官方文档
 
+        :param str policy: 授权策略
+        """
+        logger.debug("Start to put bucket policy, bucket: {0}, policy: {1}".format(self.bucket_name, policy))
         resp = self.__do_bucket('PUT', data=policy, params={Bucket.POLICY: ''}, headers={'Content-MD5': utils.content_md5(policy)})
         logger.debug("Put bucket policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
         return RequestResult(resp)
 
     def get_bucket_policy(self):
-        """
+        """获取bucket授权策略
+
         :return: :class:`GetBucketPolicyResult <oss2.models.GetBucketPolicyResult>`
         """
 
         logger.debug("Start to get bucket policy, bucket: {0}".format(self.bucket_name))
         resp = self.__do_bucket('GET', params={Bucket.POLICY:''})
         logger.debug("Get bucket policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return GetBucketPolicyResult(resp)
 
     def delete_bucket_policy(self):
-        """
+        """删除bucket授权策略
         :return: :class:`RequestResult <oss2.models.RequestResult>`
         """
         logger.debug("Start to delete bucket policy, bucket: {0}".format(self.bucket_name))
         resp = self.__do_bucket('DELETE', params={Bucket.POLICY: ''})
         logger.debug("Delete bucket policy done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
         return RequestResult(resp)
 
@@ -2147,14 +2154,15 @@
         """
         logger.debug("Start to put bucket qos info, bucket: {0}".format(self.bucket_name))
         data = self.__convert_data(BucketQosInfo, xml_utils.to_put_qos_info, bucket_qos_info) 
 
         headers = http.CaseInsensitiveDict()
         headers['Content-MD5'] = utils.content_md5(data)
         resp = self.__do_bucket('PUT', data=data, params={Bucket.QOS_INFO: ''}, headers=headers)
+        logger.debug("Get bucket qos info done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
 
         return RequestResult(resp)
 
     def get_bucket_qos_info(self):
         """获取bucket的QoSInfo
 
         :return: :class:`GetBucketQosInfoResult <oss2.models.GetBucketQosInfoResult>`
@@ -2177,26 +2185,61 @@
         return RequestResult(resp)
 
     def set_bucket_storage_capacity(self, user_qos):
         """设置Bucket的容量，单位GB
 
         :param user_qos :class:`BucketUserQos <oss2.models.BucketUserQos>`
         """
+        logger.debug("Start to set bucket storage capacity: {0}".format(self.bucket_name))
         data = xml_utils.to_put_bucket_user_qos(user_qos)
         resp = self.__do_bucket('PUT', data=data, params={Bucket.USER_QOS: ''})
+        logger.debug("Set bucket storage capacity done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
         return RequestResult(resp)
 
     def get_bucket_storage_capacity(self):
         """获取bucket的容量信息。
 
         :return: :class:`GetBucketUserQosResult <oss2.models.GetBucketUserQosResult>`
         """
+        logger.debug("Start to get bucket storage capacity, bucket:{0}".format(self.bucket_name))
         resp = self._Bucket__do_bucket('GET', params={Bucket.USER_QOS: ''})
+        logger.debug("Get bucket storage capacity done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
         return self._parse_result(resp, xml_utils.parse_get_bucket_user_qos, GetBucketUserQosResult)
 
+    def put_async_fetch_task(self, task_config):
+        """创建一个异步获取文件到bucket的任务。
+
+        :param task_config: 任务配置
+        :type task_config: class:`AsyncFetchTaskConfiguration <oss2.models.AsyncFetchTaskConfiguration>` 
+
+        :return: :class:`PutAsyncFetchTaskResult <oss2.models.PutAsyncFetchTaskResult>`
+        """
+        logger.debug("Start to put async fetch task, bucket:{0}".format(self.bucket_name))
+        data = xml_utils.to_put_async_fetch_task(task_config)
+        headers = http.CaseInsensitiveDict()
+        headers['Content-MD5'] = utils.content_md5(data)
+        resp = self._Bucket__do_bucket('POST', data=data, params={Bucket.ASYNC_FETCH: ''}, headers=headers)
+        logger.debug("Put async fetch task done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return self._parse_result(resp, xml_utils.parse_put_async_fetch_task_result, PutAsyncFetchTaskResult)
+
+    def get_async_fetch_task(self, task_id):
+        """获取一个异步获取文件到bucket的任务信息。
+
+        :param str task_id: 任务id
+        :return: :class:`GetAsyncFetchTaskResult <oss2.models.GetAsyncFetchTaskResult>`
+        """
+        logger.debug("Start to get async fetch task, bucket:{0}, task_id:{1}".format(self.bucket_name, task_id))
+        resp = self._Bucket__do_bucket('GET', headers={OSS_TASK_ID: task_id}, params={Bucket.ASYNC_FETCH: ''})
+        logger.debug("Put async fetch task done, req_id: {0}, status_code: {1}".format(resp.request_id, resp.status))
+
+        return self._parse_result(resp, xml_utils.parse_get_async_fetch_task_result, GetAsyncFetchTaskResult)
+
     def _get_bucket_config(self, config):
         """获得Bucket某项配置，具体哪种配置由 `config` 指定。该接口直接返回 `RequestResult` 对象。
         通过read()接口可以获得XML字符串。不建议使用。
 
         :param str config: 可以是 `Bucket.ACL` 、 `Bucket.LOGGING` 等。
 
         :return: :class:`RequestResult <oss2.models.RequestResult>`
```

### Comparing `oss2-2.9.0/oss2/defaults.py` & `oss2-2.9.1/oss2/defaults.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/utils.py` & `oss2-2.9.1/oss2/utils.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/crc64_combine.py` & `oss2-2.9.1/oss2/crc64_combine.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/auth.py` & `oss2-2.9.1/oss2/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import hmac
 import hashlib
 import time
 
 from . import utils
-from .compat import urlquote, to_bytes
+from .compat import urlquote, to_bytes, is_py2
 from .headers import *
 import logging
 
 AUTH_VERSION_1 = 'v1'
 AUTH_VERSION_2 = 'v2'
 
 logger = logging.getLogger(__name__)
@@ -69,15 +69,16 @@
          'response-cache-control', 'logging', 'response-content-encoding',
          'acl', 'uploadId', 'uploads', 'partNumber', 'group', 'link',
          'delete', 'website', 'location', 'objectInfo', 'objectMeta',
          'response-expires', 'response-content-disposition', 'cors', 'lifecycle',
          'restore', 'qos', 'referer', 'stat', 'bucketInfo', 'append', 'position', 'security-token',
          'live', 'comp', 'status', 'vod', 'startTime', 'endTime', 'x-oss-process',
          'symlink', 'callback', 'callback-var', 'tagging', 'encryption', 'versions',
-         'versioning', 'versionId', 'policy', 'requestPayment', 'x-oss-traffic-limit', 'qosInfo']
+         'versioning', 'versionId', 'policy', 'requestPayment', 'x-oss-traffic-limit', 'qosInfo', 'asyncFetch',
+         'x-oss-request-payer', 'sequential']
     )
 
     def _sign_request(self, req, bucket_name, key):
         req.headers['date'] = utils.http_date()
 
         signature = self.__make_signature(req, bucket_name, key)
         req.headers['authorization'] = "OSS {0}:{1}".format(self.id, signature)
@@ -91,15 +92,18 @@
         req.params['OSSAccessKeyId'] = self.id
         req.params['Expires'] = str(expiration_time)
         req.params['Signature'] = signature
 
         return req.url + '?' + '&'.join(_param_to_quoted_query(k, v) for k, v in req.params.items())
 
     def __make_signature(self, req, bucket_name, key):
-        string_to_sign = self.__get_string_to_sign(req, bucket_name, key)
+        if is_py2:
+            string_to_sign = self.__get_string_to_sign(req, bucket_name, key)
+        else:
+            string_to_sign = self.__get_bytes_to_sign(req, bucket_name, key)
 
         logger.debug('Make signature: string to be signed = {0}'.format(string_to_sign))
 
         h = hmac.new(to_bytes(self.secret), to_bytes(string_to_sign), hashlib.sha1)
         return utils.b64encode_as_string(h.digest())
 
     def __get_string_to_sign(self, req, bucket_name, key):
@@ -154,14 +158,41 @@
 
     def __param_to_query(self, k, v):
         if v:
             return k + '=' + v
         else:
             return k
 
+    def __get_bytes_to_sign(self, req, bucket_name, key):
+        resource_bytes = self.__get_resource_string(req, bucket_name, key).encode('utf-8')
+        headers_bytes = self.__get_headers_bytes(req)
+
+        content_md5 = req.headers.get('content-md5', '').encode('utf-8')
+        content_type = req.headers.get('content-type', '').encode('utf-8')
+        date = req.headers.get('date', '').encode('utf-8')
+        return b'\n'.join([req.method.encode('utf-8'),
+                          content_md5,
+                          content_type,
+                          date,
+                          headers_bytes + resource_bytes])
+
+    def __get_headers_bytes(self, req):
+        headers = req.headers
+        canon_headers = []
+        for k, v in headers.items():
+            lower_key = k.lower()
+            if lower_key.startswith('x-oss-'):
+                canon_headers.append((lower_key, v))
+
+        canon_headers.sort(key=lambda x: x[0])
+
+        if canon_headers:
+            return b'\n'.join(to_bytes(k) + b':' + to_bytes(v) for k, v in canon_headers) + b'\n'
+        else:
+            return b''
 
 class AnonymousAuth(object):
     """用于匿名访问。
 
     .. note::
         匿名用户只能读取public-read的Bucket，或只能读取、写入public-read-write的Bucket。
         不能进行Service、Bucket相关的操作，也不能罗列文件等。
@@ -295,15 +326,18 @@
         signature = self.__make_signature(req, bucket_name, key, additional_headers)
 
         req.params['x-oss-signature'] = signature
 
         return req.url + '?' + '&'.join(_param_to_quoted_query(k, v) for k, v in req.params.items())
 
     def __make_signature(self, req, bucket_name, key, additional_headers):
-        string_to_sign = self.__get_string_to_sign(req, bucket_name, key, additional_headers)
+        if is_py2:
+            string_to_sign = self.__get_string_to_sign(req, bucket_name, key, additional_headers)
+        else:
+            string_to_sign = self.__get_bytes_to_sign(req, bucket_name, key, additional_headers)
 
         logger.debug('Make signature: string to be signed = {0}'.format(string_to_sign))
 
         h = hmac.new(to_bytes(self.secret), to_bytes(string_to_sign), hashlib.sha256)
         return utils.b64encode_as_string(h.digest())
 
     def __get_additional_headers(self, req, in_additional_headers):
@@ -369,7 +403,40 @@
             lower_key = k.lower()
             if lower_key.startswith('x-oss-') or lower_key in additional_headers:
                 canon_headers.append((lower_key, v))
 
         canon_headers.sort(key=lambda x: x[0])
 
         return ''.join(v[0] + ':' + v[1] + '\n' for v in canon_headers)
+
+    def __get_bytes_to_sign(self, req, bucket_name, key, additional_header_list):
+        verb = req.method.encode('utf-8')
+        content_md5 = req.headers.get('content-md5', '').encode('utf-8')
+        content_type = req.headers.get('content-type', '').encode('utf-8')
+        date = req.headers.get('date', '').encode('utf-8')
+
+        canonicalized_oss_headers = self.__get_canonicalized_oss_headers_bytes(req, additional_header_list)
+        additional_headers = ';'.join(sorted(additional_header_list)).encode('utf-8')
+        canonicalized_resource = self.__get_resource_string(req, bucket_name, key).encode('utf-8')
+
+        return verb + b'\n' +\
+            content_md5 + b'\n' +\
+            content_type + b'\n' +\
+            date + b'\n' +\
+            canonicalized_oss_headers +\
+            additional_headers + b'\n' +\
+            canonicalized_resource
+    
+    def __get_canonicalized_oss_headers_bytes(self, req, additional_headers):
+        """
+        :param additional_headers: 小写的headers列表, 并且这些headers都不以'x-oss-'为前缀.
+        """
+        canon_headers = []
+
+        for k, v in req.headers.items():
+            lower_key = k.lower()
+            if lower_key.startswith('x-oss-') or lower_key in additional_headers:
+                canon_headers.append((lower_key, v))
+
+        canon_headers.sort(key=lambda x: x[0])
+
+        return b''.join(to_bytes(v[0]) + b':' + to_bytes(v[1]) + b'\n' for v in canon_headers)
```

### Comparing `oss2-2.9.0/oss2/crypto.py` & `oss2-2.9.1/oss2/crypto.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/http.py` & `oss2-2.9.1/oss2/http.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/iterators.py` & `oss2-2.9.1/oss2/iterators.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/xml_utils.py` & `oss2-2.9.1/oss2/xml_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,16 @@
                      RedirectMirrorHeaders,
                      MirrorHeadersSet,
                      REDIRECT_TYPE_MIRROR,
                      REDIRECT_TYPE_EXTERNAL,
                      REDIRECT_TYPE_INTERNAL,
                      REDIRECT_TYPE_ALICDN,
                      NoncurrentVersionStorageTransition,
-                     NoncurrentVersionExpiration)
+                     NoncurrentVersionExpiration,
+                     AsyncFetchTaskConfiguration)
 
 from .select_params import (SelectJsonTypes, SelectParameters)
 
 from .compat import urlunquote, to_unicode, to_string
 from .utils import iso8601_to_unixtime, date_to_iso8601, iso8601_to_date
 from . import utils
 import base64
@@ -291,28 +292,36 @@
     result.creation_date = _find_tag(root, 'Bucket/CreationDate')
     result.storage_class = _find_tag(root, 'Bucket/StorageClass')
     result.extranet_endpoint = _find_tag(root, 'Bucket/ExtranetEndpoint')
     result.intranet_endpoint = _find_tag(root, 'Bucket/IntranetEndpoint')
     result.location = _find_tag(root, 'Bucket/Location')
     result.owner = Owner(_find_tag(root, 'Bucket/Owner/DisplayName'), _find_tag(root, 'Bucket/Owner/ID'))
     result.acl = AccessControlList(_find_tag(root, 'Bucket/AccessControlList/Grant'))
-    result.data_redundancy_type = _find_tag(root, 'Bucket/DataRedundancyType')
     result.comment = _find_tag(root, 'Bucket/Comment')
 
     server_side_encryption = root.find("Bucket/ServerSideEncryptionRule")
 
-    result.bucket_encryption_rule = _parse_bucket_encryption_info(server_side_encryption)
+    if server_side_encryption is None:
+        result.bucket_encryption_rule = None
+    else:
+        result.bucket_encryption_rule = _parse_bucket_encryption_info(server_side_encryption)
 
     bucket_versioning = root.find('Bucket/Versioning')
     
     if bucket_versioning is None or bucket_versioning.text is None:
         result.versioning_status = None
     else:
         result.versioning_status = to_string(bucket_versioning.text)
 
+    data_redundancy_type = root.find('Bucket/DataRedundancyType')
+    if data_redundancy_type is None or data_redundancy_type.text is None:
+        result.data_redundancy_type = None
+    else:
+        result.data_redundancy_type = to_string(data_redundancy_type.text)
+
     return result
 
 def _parse_bucket_encryption_info(node):
 
     rule = ServerSideEncryptionRule()
 
     rule.sse_algorithm = _find_tag(node,"SSEAlgorithm")
@@ -1284,7 +1293,52 @@
 
 def to_put_bucket_user_qos(user_qos):
     root = ElementTree.Element('BucketUserQos')
 
     _add_text_child(root, 'StorageCapacity', str(user_qos.storage_capacity))
 
     return _node_to_string(root)
+
+
+def to_put_async_fetch_task(task_config):
+    root = ElementTree.Element('AsyncFetchTaskConfiguration')
+
+    _add_text_child(root, 'Url', task_config.url)
+    _add_text_child(root, 'Object', task_config.object_name)
+
+    if task_config.host is not None:    
+        _add_text_child(root, 'Host', task_config.host)
+    if task_config.content_md5 is not None:
+        _add_text_child(root, 'ContentMD5', task_config.content_md5)
+    if task_config.callback is not None:
+        _add_text_child(root, 'Callback', task_config.callback)
+    if task_config.ignore_same_key is not None:
+        _add_text_child(root, 'IgnoreSameKey', str(task_config.ignore_same_key).lower())
+
+    return _node_to_string(root)
+
+def parse_put_async_fetch_task_result(result, body):
+    root = ElementTree.fromstring(body)
+
+    result.task_id = _find_tag(root, 'TaskId')
+
+    return result
+
+def _parse_async_fetch_task_configuration(task_info_node):
+    url = _find_tag(task_info_node, 'Url')
+    object_name = _find_tag(task_info_node, 'Object')
+    host = _find_tag(task_info_node, 'Host')
+    content_md5 = _find_tag(task_info_node, 'ContentMD5')
+    callback = _find_tag(task_info_node, 'Callback')
+    ignore_same_key = _find_bool(task_info_node, 'IgnoreSameKey')
+
+    return AsyncFetchTaskConfiguration(url, object_name, host, content_md5, callback, ignore_same_key)
+
+def parse_get_async_fetch_task_result(result, body):
+    root = ElementTree.fromstring(body)
+
+    result.task_id = _find_tag(root, 'TaskId')
+    result.task_state = _find_tag(root, 'State')
+    result.error_msg = _find_tag(root, 'ErrorMsg')
+    result.task_config = _parse_async_fetch_task_configuration(root.find('TaskInfo'))
+
+    return result
```

### Comparing `oss2-2.9.0/oss2/compat.py` & `oss2-2.9.1/oss2/compat.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/headers.py` & `oss2-2.9.1/oss2/headers.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 OSS_OBJECT_TAGGING = "x-oss-tagging"
 OSS_OBJECT_TAGGING_COPY_DIRECTIVE = "x-oss-tagging-directive"
 
 OSS_REQUEST_PAYER = 'x-oss-request-payer'
 
 OSS_TRAFFIC_LIMIT = 'x-oss-traffic-limit'
 
+OSS_TASK_ID = 'x-oss-task-id'
+
 class RequestHeader(dict):
     def __init__(self, *arg, **kw): 
         super(RequestHeader, self).__init__(*arg, **kw)
 
     def set_server_side_encryption(self, algorithm=None, cmk_id=None):
         if OSS_SERVER_SIDE_ENCRYPTION in self:
             del self[OSS_SERVER_SIDE_ENCRYPTION]
```

### Comparing `oss2-2.9.0/oss2/task_queue.py` & `oss2-2.9.1/oss2/task_queue.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/select_response.py` & `oss2-2.9.1/oss2/select_response.py`

 * *Files identical despite different names*

### Comparing `oss2-2.9.0/oss2/resumable.py` & `oss2-2.9.1/oss2/resumable.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 def resumable_upload(bucket, key, filename,
                      store=None,
                      headers=None,
                      multipart_threshold=None,
                      part_size=None,
                      progress_callback=None,
-                     num_threads=None):
+                     num_threads=None,
+                     params=None):
     """断点上传本地文件。
 
     实现中采用分片上传方式上传本地文件，缺省的并发数是 `oss2.defaults.multipart_num_threads` ，并且在
     本地磁盘保存已经上传的分片信息。如果因为某种原因上传被中断，下次上传同样的文件，即源文件和目标文件路径都
     一样，就只会上传缺失的分片。
 
     缺省条件下，该函数会在用户 `HOME` 目录下保存断点续传的信息。当待上传的本地文件没有发生变化，
@@ -63,29 +64,35 @@
         # 调用外部函数complete_multipart_upload目前只传递OSS_REQUEST_PAYER
     :type headers: 可以是dict，建议是oss2.CaseInsensitiveDict
 
     :param multipart_threshold: 文件长度大于该值时，则用分片上传。
     :param part_size: 指定分片上传的每个分片的大小。如不指定，则自动计算。
     :param progress_callback: 上传进度回调函数。参见 :ref:`progress_callback` 。
     :param num_threads: 并发上传的线程数，如不指定则使用 `oss2.defaults.multipart_num_threads` 。
+
+    :param params: HTTP请求参数
+        # 只有'sequential'这个参数才会被传递到外部函数init_multipart_upload中。
+        # 其他参数视为无效参数不会往外部函数传递。
+    :type params: dict
     """
     logger.debug("Start to resumable upload, bucket: {0}, key: {1}, filename: {2}, headers: {3}, "
                 "multipart_threshold: {4}, part_size: {5}, num_threads: {6}".format(bucket.bucket_name, to_string(key),
                                                                                     filename, headers, multipart_threshold,
                                                                                     part_size, num_threads))
     size = os.path.getsize(filename)
     multipart_threshold = defaults.get(multipart_threshold, defaults.multipart_threshold)
 
     logger.debug("The size of file to upload is: {0}, multipart_threshold: {1}".format(size, multipart_threshold))
     if isinstance(bucket, Bucket) and size >= multipart_threshold:
         uploader = _ResumableUploader(bucket, key, filename, size, store,
                                       part_size=part_size,
                                       headers=headers,
                                       progress_callback=progress_callback,
-                                      num_threads=num_threads)
+                                      num_threads=num_threads,
+                                      params=params)
         result = uploader.upload()
     else:
         with open(to_unicode(filename), 'rb') as f:
             result = bucket.put_object(key, f, headers=headers, progress_callback=progress_callback)
 
     return result
 
@@ -234,14 +241,39 @@
             valid_headers[key] = headers[key]
 
     if len(valid_headers) == 0:
         valid_headers = None
 
     return valid_headers
 
+def _populate_valid_params(params=None, valid_keys=None):
+    """构建只包含有效keys的params
+
+    :param params: 需要过滤的params
+    :type params: dict
+
+    :param valid_keys: 有效的关键key列表
+    :type valid_keys: list
+
+    :return: 只包含有效keys的params
+    """
+    if params is None or valid_keys is None:
+        return None
+
+    valid_params = dict()
+
+    for key in valid_keys:
+        if params.get(key) is not None:
+            valid_params[key] = params[key]
+
+    if len(valid_params) == 0:
+        valid_params = None
+
+    return valid_params
+
 class _ResumableOperation(object):
     def __init__(self, bucket, key, filename, size, store,
                  progress_callback=None, versionid=None):
         self.bucket = bucket
         self.key = to_string(key)
         self.filename = filename
         self.size = size
@@ -481,29 +513,32 @@
     :param progress_callback: 上传进度回调函数。参见 :ref:`progress_callback` 。
     """
     def __init__(self, bucket, key, filename, size,
                  store=None,
                  headers=None,
                  part_size=None,
                  progress_callback=None,
-                 num_threads=None):
+                 num_threads=None,
+                 params=None):
         super(_ResumableUploader, self).__init__(bucket, key, filename, size,
                                                  store or ResumableStore(),
                                                  progress_callback=progress_callback)
 
         self.__headers = headers
 
         self.__part_size = defaults.get(part_size, defaults.part_size)
 
         self.__mtime = os.path.getmtime(filename)
 
         self.__num_threads = defaults.get(num_threads, defaults.multipart_num_threads)
 
         self.__upload_id = None
 
+        self.__params = params
+
         # protect below fields
         self.__lock = threading.Lock()
         self.__record = None
         self.__finished_size = 0
         self.__finished_parts = None
         logger.debug("Init _ResumableUploader, bucket: {0}, key: {1}, part_size: {2}, num_thread: {3}".format(
             bucket.bucket_name, to_string(key), self.__part_size, self.__num_threads))
@@ -579,15 +614,16 @@
             self._del_record()
             record = None
 
         if not record:
             part_size = determine_part_size(self.size, self.__part_size)
             logger.debug("Upload File size: {0}, User-specify part_size: {1}, Calculated part_size: {2}".format(
                 self.size, self.__part_size, part_size))
-            upload_id = self.bucket.init_multipart_upload(self.key, headers=self.__headers).upload_id
+            params = _populate_valid_params(self.__params, [Bucket.SEQUENTIAL])
+            upload_id = self.bucket.init_multipart_upload(self.key, headers=self.__headers, params=params).upload_id
             record = {'upload_id': upload_id, 'mtime': self.__mtime, 'size': self.size, 'parts': [],
                       'abspath': self._abspath, 'bucket': self.bucket.bucket_name, 'key': self.key,
                       'part_size': part_size}
 
             logger.debug('Add new record, bucket: {0}, key: {1}, upload_id: {2}, part_size: {3}'.format(
                 self.bucket.bucket_name, self.key, upload_id, part_size))
             self._put_record(record)
```


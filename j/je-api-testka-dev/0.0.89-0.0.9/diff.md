# Comparing `tmp/je_api_testka_dev-0.0.89.tar.gz` & `tmp/je_api_testka_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.89.tar", last modified: Mon May 29 03:07:01 2023, max compression
+gzip compressed data, was "dist\je_api_testka_dev-0.0.9.tar", last modified: Sat Mar 12 10:59:14 2022, max compression
```

## Comparing `je_api_testka_dev-0.0.89.tar` & `je_api_testka_dev-0.0.9.tar`

### file list

```diff
@@ -1,82 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.565712 je_api_testka_dev-0.0.89/
--rw-rw-rw-   0        0        0     3330 2023-05-29 03:07:01.564732 je_api_testka_dev-0.0.89/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2023-05-24 09:54:01.000000 je_api_testka_dev-0.0.89/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.347746 je_api_testka_dev-0.0.89/je_api_testka/
--rw-rw-rw-   0        0        0     2845 2023-04-21 07:30:34.000000 je_api_testka_dev-0.0.89/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.89/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.361353 je_api_testka_dev-0.0.89/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.89/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.89/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.364359 je_api_testka_dev-0.0.89/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.370702 je_api_testka_dev-0.0.89/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.381070 je_api_testka_dev-0.0.89/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-05-29 03:06:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.391593 je_api_testka_dev-0.0.89/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.400798 je_api_testka_dev-0.0.89/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-05-29 03:06:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.406798 je_api_testka_dev-0.0.89/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.421883 je_api_testka_dev-0.0.89/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.428870 je_api_testka_dev-0.0.89/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.441202 je_api_testka_dev-0.0.89/je_api_testka/utils/global_dict/
--rw-rw-rw-   0        0        0        0 2023-05-29 03:04:06.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/global_dict/__init__.py
--rw-rw-rw-   0        0        0     1495 2023-05-29 03:06:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/global_dict/event_dict.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.445203 je_api_testka_dev-0.0.89/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.452802 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.461203 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.468202 je_api_testka_dev-0.0.89/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.476727 je_api_testka_dev-0.0.89/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.483195 je_api_testka_dev-0.0.89/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.495795 je_api_testka_dev-0.0.89/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.508424 je_api_testka_dev-0.0.89/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.513971 je_api_testka_dev-0.0.89/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.517974 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.523524 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.529523 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.89/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:07:01.561715 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-05-29 03:07:01.000000 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2545 2023-05-29 03:07:01.000000 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:07:01.000000 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 03:07:01.000000 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-29 03:07:01.000000 je_api_testka_dev-0.0.89/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1150 2023-05-29 03:06:38.000000 je_api_testka_dev-0.0.89/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 03:07:01.566732 je_api_testka_dev-0.0.89/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      966 2022-03-12 10:59:10.000000 je_api_testka_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/
+-rw-rw-rw-   0        0        0     2866 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/record/
+-rw-rw-rw-   0        0        0        0 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/__init__.py
+-rw-rw-rw-   0        0        0      258 2022-03-07 01:22:48.000000 je_api_testka_dev-0.0.9/je_api_testka/record/record.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     3134 2022-03-11 09:34:19.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     1294 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/requests_wrapper/requests_data_structure.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/
+-rw-rw-rw-   0        0        0       35 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:52:53.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/assert_result/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     2754 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_eceptions_tag.py
+-rw-rw-rw-   0        0        0     1906 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/exception/api_test_exceptions.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/__init__.py
+-rw-rw-rw-   0        0        0     1159 2022-03-12 09:24:21.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/execute_action/action_executor.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1063 2022-03-11 13:13:40.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0       40 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1324 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1046 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/__init__.py
+-rw-rw-rw-   0        0        0     1084 2022-02-16 16:26:27.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_search/json_search.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2022-03-12 10:53:49.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2480 2022-03-02 15:06:29.000000 je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0      930 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1378 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-03-12 10:59:13.000000 je_api_testka_dev-0.0.9/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-03-12 10:59:14.000000 je_api_testka_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      958 2022-03-11 16:12:43.000000 je_api_testka_dev-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `je_api_testka_dev-0.0.89/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/json/json_file/json_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import json
 from pathlib import Path
 from threading import Lock
 
-from je_api_testka.utils.exception.exception_tags import cant_find_json_error
-from je_api_testka.utils.exception.exception_tags import cant_save_json_error
-from je_api_testka.utils.exception.exceptions import APITesterJsonException
+from je_api_testka.utils.exception.api_test_exceptions import APITesterJsonException
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_find_json_error
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_save_json_error
 
 lock = Lock()
 
 
-def read_action_json(json_file_path: str) -> dict:
+def read_action_json(json_file_path: str):
     """
-    read the action json
     :param json_file_path json file's path to read
     """
     try:
         lock.acquire()
         file_path = Path(json_file_path)
         if file_path.exists() and file_path.is_file():
             with open(json_file_path) as read_file:
-                return json.load(read_file)
+                return read_file.read()
     except APITesterJsonException:
-        raise APITesterJsonException(cant_find_json_error)
+        raise APITesterJsonException(api_test_cant_find_json_error)
     finally:
         lock.release()
 
 
-def write_action_json(json_save_path: str, action_json: list) -> None:
+def write_action_json(json_save_path: str, action_json: str):
     """
-    write action json
     :param json_save_path  json save path
     :param action_json the json str include action to write
     """
     try:
         lock.acquire()
         with open(json_save_path, "w+") as file_to_write:
-            file_to_write.write(json.dumps(action_json, indent=4))
+            file_to_write.write(action_json)
     except APITesterJsonException:
-        raise APITesterJsonException(cant_save_json_error)
+        raise APITesterJsonException(api_test_cant_save_json_error)
     finally:
         lock.release()
+
```

### Comparing `je_api_testka_dev-0.0.89/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.9/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,63 @@
 import xml.dom.minidom
 from xml.etree import ElementTree
-
-from je_api_testka.utils.exception.exception_tags import cant_read_xml_error
-from je_api_testka.utils.exception.exception_tags import xml_type_error
-from je_api_testka.utils.exception.exceptions import APITesterXMLException
-from je_api_testka.utils.exception.exceptions import APITesterXMLTypeException
+from xml.dom.minidom import parse
+from xml.dom.minidom import parseString
+from xml.dom import minidom
+
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_cant_read_xml_error
+from je_api_testka.utils.exception.api_test_eceptions_tag import api_test_xml_type_error
+from je_api_testka.utils.exception.api_test_exceptions import APITesterXMLException
+from je_api_testka.utils.exception.api_test_exceptions import APITesterXMLTypeException
 
 
 def reformat_xml_file(xml_string: str):
     dom = xml.dom.minidom.parseString(xml_string)
     return dom.toprettyxml()
 
 
 class XMLParser(object):
 
-    def __init__(self, xml_string: str, xml_type: str = "string"):
-        """
-        :param xml_string: full xml string
-        :param xml_type: file or string
-        """
+    def __init__(self, xml_string: str, xml_type: str):
         self.element_tree = ElementTree
         self.tree = None
         self.xml_root = None
         self.xml_from_type = "string"
         self.xml_string = xml_string.strip()
         xml_type = xml_type.lower()
         if xml_type not in ["file", "string"]:
-            raise APITesterXMLTypeException(xml_type_error)
+            raise APITesterXMLTypeException(api_test_xml_type_error)
         if xml_type == "string":
             self.xml_parser_from_string()
         else:
             self.xml_parser_from_file()
 
     def xml_parser_from_string(self, **kwargs):
-        """
-        :param kwargs: any another param
-        :return: xml root element tree
-        """
         try:
             self.xml_root = ElementTree.fromstring(self.xml_string, **kwargs)
         except APITesterXMLException:
-            raise APITesterXMLException(cant_read_xml_error)
+            raise APITesterXMLException(api_test_cant_read_xml_error)
         return self.xml_root
 
     def xml_parser_from_file(self, **kwargs):
-        """
-        :param kwargs: any another param
-        :return: xml root element tree
-        """
         try:
             self.tree = ElementTree.parse(self.xml_string, **kwargs)
         except APITesterXMLException:
-            raise APITesterXMLException(cant_read_xml_error)
+            raise APITesterXMLException(api_test_cant_read_xml_error)
         self.xml_root = self.tree.getroot()
         self.xml_from_type = "file"
         return self.xml_root
 
+    def find_tag(self, tag_name: [str, None] = None):
+        if self.xml_from_type == "string":
+            return self.xml_root.iter(tag_name)
+        else:
+            return self.tree.iter(tag_name)
+
+    def xml_iterparse(self, xml_string: str, **kwargs):
+        return self.element_tree.iterparse(xml_string, **kwargs)
+
     def write_xml(self, write_xml_filename: str, write_content: str):
-        """
-        :param write_xml_filename:  xml file name
-        :param write_content: content to write
-        """
         write_content = write_content.strip()
         content = self.element_tree.fromstring(write_content)
         tree = self.element_tree.ElementTree(content)
         tree.write(write_xml_filename, encoding="utf-8")
```


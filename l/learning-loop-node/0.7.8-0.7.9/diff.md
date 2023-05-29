# Comparing `tmp/learning_loop_node-0.7.8.tar.gz` & `tmp/learning_loop_node-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning_loop_node-0.7.8.tar", max compression
+gzip compressed data, was "learning_loop_node-0.7.9.tar", max compression
```

## Comparing `learning_loop_node-0.7.8.tar` & `learning_loop_node-0.7.9.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     4210 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/README.md
--rw-r--r--   0        0        0      481 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/.vscode/settings.json
--rw-r--r--   0        0        0      487 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/__init__.py
--rw-r--r--   0        0        0     3052 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/annotation_node/annotation_node.py
--rw-r--r--   0        0        0      611 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/annotation_node/annotation_tool.py
--rw-r--r--   0        0        0     1253 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/annotation_node/data_classes.py
--rw-r--r--   0        0        0     1453 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/annotation_node/tests/test_annotation_node.py
--rw-r--r--   0        0        0     1392 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/conftest.py
--rw-r--r--   0        0        0      103 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/context.py
--rw-r--r--   0        0        0     1714 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/converter/converter.py
--rw-r--r--   0        0        0     4300 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/converter/converter_node.py
--rw-r--r--   0        0        0     1689 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/converter/tests/test_converter.py
--rw-r--r--   0        0        0       45 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/data_classes/__init__.py
--rw-r--r--   0        0        0      142 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/data_classes/basic_data.py
--rw-r--r--   0        0        0      517 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/data_classes/category.py
--rw-r--r--   0        0        0      146 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/__init__.py
--rw-r--r--   0        0        0     1860 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/box_detection.py
--rw-r--r--   0        0        0      656 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/detections.py
--rw-r--r--   0        0        0     2002 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/detector.py
--rw-r--r--   0        0        0    10495 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/detector_node.py
--rw-r--r--   0        0        0     2412 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/outbox.py
--rw-r--r--   0        0        0     1015 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/point_detection.py
--rw-r--r--   0        0        0      885 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/rest/detect.py
--rw-r--r--   0        0        0     1251 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/rest/operation_mode.py
--rw-r--r--   0        0        0      435 2022-02-21 09:47:07.047708 learning_loop_node-0.7.8/learning_loop_node/detector/rest/upload.py
--rw-r--r--   0        0        0     2765 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/conftest.py
--rw-r--r--   0        0        0   161390 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/test.jpg
--rw-r--r--   0        0        0     2643 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_client_communication.py
--rw-r--r--   0        0        0     1419 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_outbox.py
--rw-r--r--   0        0        0      679 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_relevants_filter.py
--rw-r--r--   0        0        0      660 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/detector/tests/testing_detector.py
--rw-r--r--   0        0        0     1064 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/gdrive_downloader.py
--rw-r--r--   0        0        0      104 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/globals.py
--rw-r--r--   0        0        0      559 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/observation.py
--rw-r--r--   0        0        0     1134 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/relevants_filter.py
--rw-r--r--   0        0        0     2239 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/relevants_group.py
--rw-r--r--   0        0        0      969 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_observation.py
--rw-r--r--   0        0        0     4070 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_relevants_group.py
--rw-r--r--   0        0        0     1455 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_unexpected_observations_count.py
--rw-r--r--   0        0        0     4481 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/loop.py
--rw-r--r--   0        0        0      474 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/model_information.py
--rw-r--r--   0        0        0     4223 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/node.py
--rw-r--r--   0        0        0      592 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/node_helper.py
--rw-r--r--   0        0        0      184 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/pytest.ini
--rw-r--r--   0        0        0     1733 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/rest/downloader.py
--rw-r--r--   0        0        0     5238 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/rest/downloads.py
--rw-r--r--   0        0        0      762 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/rest/uploads.py
--rw-r--r--   0        0        0      294 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/singleton.py
--rw-r--r--   0        0        0     2058 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/socket_response.py
--rw-r--r--   0        0        0     1206 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/status.py
--rw-r--r--   0        0        0     1730 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/task_logger.py
--rw-r--r--   0        0        0        0 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/__init__.py
--rw-r--r--   0        0        0      195 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/mock_async_client.py
--rw-r--r--   0        0        0       19 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_data/file_1.txt
--rw-r--r--   0        0        0       19 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_data/file_2.txt
--rw-r--r--   0        0        0     3414 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_downloader.py
--rw-r--r--   0        0        0     1959 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_executor.py
--rw-r--r--   0        0        0     2513 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_helper.py
--rw-r--r--   0        0        0      697 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/tests/test_learning_loop_node.py
--rw-r--r--   0        0        0      147 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/__init__.py
--rw-r--r--   0        0        0     1770 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/downloader.py
--rw-r--r--   0        0        0      270 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/error_configuration.py
--rw-r--r--   0        0        0     1902 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/executor.py
--rw-r--r--   0        0        0      153 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/helper.py
--rw-r--r--   0        0        0      493 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/model.py
--rw-r--r--   0        0        0      611 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/tests/trainer_test_helper.py
--rw-r--r--   0        0        0     6850 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/trainer.py
--rw-r--r--   0        0        0     9136 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/trainer_node.py
--rw-r--r--   0        0        0      403 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/training.py
--rw-r--r--   0        0        0      525 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/training_data.py
--rw-r--r--   0        0        0      489 2022-02-21 09:47:07.051708 learning_loop_node-0.7.8/learning_loop_node/trainer/training_status.py
--rw-r--r--   0        0        0      939 2022-02-21 09:47:18.383058 learning_loop_node-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     6126 2022-02-21 09:47:19.433404 learning_loop_node-0.7.8/setup.py
--rw-r--r--   0        0        0     5686 2022-02-21 09:47:19.434265 learning_loop_node-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     4210 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/README.md
+-rw-r--r--   0        0        0      481 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/.vscode/settings.json
+-rw-r--r--   0        0        0      487 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/__init__.py
+-rw-r--r--   0        0        0     3052 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/annotation_node/annotation_node.py
+-rw-r--r--   0        0        0      611 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/annotation_node/annotation_tool.py
+-rw-r--r--   0        0        0     1253 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/annotation_node/data_classes.py
+-rw-r--r--   0        0        0     1453 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/annotation_node/tests/test_annotation_node.py
+-rw-r--r--   0        0        0     1392 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/conftest.py
+-rw-r--r--   0        0        0      103 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/context.py
+-rw-r--r--   0        0        0     1714 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/converter/converter.py
+-rw-r--r--   0        0        0     4300 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/converter/converter_node.py
+-rw-r--r--   0        0        0     1689 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/converter/tests/test_converter.py
+-rw-r--r--   0        0        0       45 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/data_classes/__init__.py
+-rw-r--r--   0        0        0      142 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/data_classes/basic_data.py
+-rw-r--r--   0        0        0      517 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/data_classes/category.py
+-rw-r--r--   0        0        0      146 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/__init__.py
+-rw-r--r--   0        0        0     1860 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/box_detection.py
+-rw-r--r--   0        0        0      656 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/detections.py
+-rw-r--r--   0        0        0     2002 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/detector.py
+-rw-r--r--   0        0        0    10495 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/detector_node.py
+-rw-r--r--   0        0        0     2412 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/outbox.py
+-rw-r--r--   0        0        0     1015 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/point_detection.py
+-rw-r--r--   0        0        0      885 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/rest/detect.py
+-rw-r--r--   0        0        0     1251 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/rest/operation_mode.py
+-rw-r--r--   0        0        0      435 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/rest/upload.py
+-rw-r--r--   0        0        0     2765 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/conftest.py
+-rw-r--r--   0        0        0   161390 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/test.jpg
+-rw-r--r--   0        0        0     2643 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_client_communication.py
+-rw-r--r--   0        0        0     1419 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_outbox.py
+-rw-r--r--   0        0        0      679 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_relevants_filter.py
+-rw-r--r--   0        0        0      660 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/detector/tests/testing_detector.py
+-rwxr-xr-x   0        0        0     1182 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/gdrive_downloader.py
+-rw-r--r--   0        0        0      104 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/globals.py
+-rw-r--r--   0        0        0      559 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/observation.py
+-rw-r--r--   0        0        0     1134 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/relevants_filter.py
+-rw-r--r--   0        0        0     2239 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/relevants_group.py
+-rw-r--r--   0        0        0      969 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_observation.py
+-rw-r--r--   0        0        0     4070 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_relevants_group.py
+-rw-r--r--   0        0        0     1455 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_unexpected_observations_count.py
+-rw-r--r--   0        0        0     4481 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/loop.py
+-rw-r--r--   0        0        0      474 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/model_information.py
+-rw-r--r--   0        0        0     4223 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/node.py
+-rw-r--r--   0        0        0      592 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/node_helper.py
+-rw-r--r--   0        0        0      184 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/pytest.ini
+-rw-r--r--   0        0        0     1733 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/rest/downloader.py
+-rw-r--r--   0        0        0     5238 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/rest/downloads.py
+-rw-r--r--   0        0        0      762 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/rest/uploads.py
+-rw-r--r--   0        0        0      294 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/singleton.py
+-rw-r--r--   0        0        0     2058 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/socket_response.py
+-rw-r--r--   0        0        0     1206 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/status.py
+-rw-r--r--   0        0        0     1730 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/task_logger.py
+-rw-r--r--   0        0        0        0 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/__init__.py
+-rw-r--r--   0        0        0      195 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/mock_async_client.py
+-rw-r--r--   0        0        0       19 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_data/file_1.txt
+-rw-r--r--   0        0        0       19 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_data/file_2.txt
+-rw-r--r--   0        0        0     3414 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_downloader.py
+-rw-r--r--   0        0        0     1959 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_executor.py
+-rw-r--r--   0        0        0     2752 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_helper.py
+-rw-r--r--   0        0        0      697 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_learning_loop_node.py
+-rw-r--r--   0        0        0     1319 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/tests/test_loop.py
+-rw-r--r--   0        0        0      147 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/__init__.py
+-rw-r--r--   0        0        0     1770 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/downloader.py
+-rw-r--r--   0        0        0      270 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/error_configuration.py
+-rw-r--r--   0        0        0     1902 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/executor.py
+-rw-r--r--   0        0        0      153 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/helper.py
+-rw-r--r--   0        0        0      493 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/model.py
+-rw-r--r--   0        0        0      611 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/tests/trainer_test_helper.py
+-rw-r--r--   0        0        0     9848 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/trainer.py
+-rw-r--r--   0        0        0     9784 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/trainer_node.py
+-rw-r--r--   0        0        0      403 2022-02-28 09:16:29.282878 learning_loop_node-0.7.9/learning_loop_node/trainer/training.py
+-rw-r--r--   0        0        0      525 2022-02-28 09:16:29.286878 learning_loop_node-0.7.9/learning_loop_node/trainer/training_data.py
+-rw-r--r--   0        0        0      489 2022-02-28 09:16:29.286878 learning_loop_node-0.7.9/learning_loop_node/trainer/training_status.py
+-rw-r--r--   0        0        0      939 2022-02-28 09:16:37.982983 learning_loop_node-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     6126 2022-02-28 09:16:38.884663 learning_loop_node-0.7.9/setup.py
+-rw-r--r--   0        0        0     5686 2022-02-28 09:16:38.885128 learning_loop_node-0.7.9/PKG-INFO
```

### Comparing `learning_loop_node-0.7.8/README.md` & `learning_loop_node-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/annotation_node/annotation_node.py` & `learning_loop_node-0.7.9/learning_loop_node/annotation_node/annotation_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/annotation_node/annotation_tool.py` & `learning_loop_node-0.7.9/learning_loop_node/annotation_node/annotation_tool.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/annotation_node/data_classes.py` & `learning_loop_node-0.7.9/learning_loop_node/annotation_node/data_classes.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/annotation_node/tests/test_annotation_node.py` & `learning_loop_node-0.7.9/learning_loop_node/annotation_node/tests/test_annotation_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/conftest.py` & `learning_loop_node-0.7.9/learning_loop_node/conftest.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/converter/converter.py` & `learning_loop_node-0.7.9/learning_loop_node/converter/converter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/converter/converter_node.py` & `learning_loop_node-0.7.9/learning_loop_node/converter/converter_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/converter/tests/test_converter.py` & `learning_loop_node-0.7.9/learning_loop_node/converter/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/data_classes/category.py` & `learning_loop_node-0.7.9/learning_loop_node/data_classes/category.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/box_detection.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/box_detection.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/detections.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/detections.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/detector.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/detector.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/detector_node.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/detector_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/outbox.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/outbox.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/point_detection.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/point_detection.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/rest/detect.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/rest/detect.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/rest/operation_mode.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/rest/operation_mode.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/conftest.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/test.jpg` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/test.jpg`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_client_communication.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_client_communication.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_outbox.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_outbox.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/test_relevants_filter.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/test_relevants_filter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/detector/tests/testing_detector.py` & `learning_loop_node-0.7.9/learning_loop_node/detector/tests/testing_detector.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/gdrive_downloader.py` & `learning_loop_node-0.7.9/learning_loop_node/gdrive_downloader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python3
 import requests
-
+from icecream import ic
 # https://stackoverflow.com/a/39225272/4082686
 
 
-def download(id, destination):
+def g_download(id, destination):
     URL = "https://docs.google.com/uc?export=download"
 
     session = requests.Session()
 
-    response = session.get(URL, params={'id': id}, stream=True)
+    response = session.get(URL, params={
+        'id': id,
+        'confirm': 't'},  # e.g. large file warning.
+        stream=True)
+    ic(str(response))
     token = get_confirm_token(response)
 
     if token:
         params = {'id': id, 'confirm': token}
         response = session.get(URL, params=params, stream=True)
 
     save_response_content(response, destination)
@@ -33,10 +37,10 @@
     with open(destination, "wb") as f:
         for chunk in response.iter_content(CHUNK_SIZE):
             if chunk:  # filter out keep-alive new chunks
                 f.write(chunk)
 
 
 if __name__ == "__main__":
-    file_id = '1jNgQDqQeaZhIWFCxV1eKeuLzXHYhXAQv'
+    file_id = '1q8nT-CTHt1eZuNjPMbdaavyFnMtDRT-L'
     destination = 'test.zip'
-    download(file_id, destination)
+    g_download(file_id, destination)
```

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/observation.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/observation.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/relevants_filter.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/relevants_filter.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/relevants_group.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/relevants_group.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_observation.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_relevants_group.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_relevants_group.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/inbox_filter/tests/test_unexpected_observations_count.py` & `learning_loop_node-0.7.9/learning_loop_node/inbox_filter/tests/test_unexpected_observations_count.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/loop.py` & `learning_loop_node-0.7.9/learning_loop_node/loop.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/node.py` & `learning_loop_node-0.7.9/learning_loop_node/node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/node_helper.py` & `learning_loop_node-0.7.9/learning_loop_node/node_helper.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/rest/downloader.py` & `learning_loop_node-0.7.9/learning_loop_node/rest/downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/rest/downloads.py` & `learning_loop_node-0.7.9/learning_loop_node/rest/downloads.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/rest/uploads.py` & `learning_loop_node-0.7.9/learning_loop_node/rest/uploads.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/socket_response.py` & `learning_loop_node-0.7.9/learning_loop_node/socket_response.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/status.py` & `learning_loop_node-0.7.9/learning_loop_node/status.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/task_logger.py` & `learning_loop_node-0.7.9/learning_loop_node/task_logger.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/tests/test_downloader.py` & `learning_loop_node-0.7.9/learning_loop_node/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/tests/test_executor.py` & `learning_loop_node-0.7.9/learning_loop_node/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/tests/test_helper.py` & `learning_loop_node-0.7.9/learning_loop_node/tests/test_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from glob import glob
 import os
 from typing import List, Optional
+import zipfile
 from learning_loop_node.loop import loop
 from urllib.parse import urljoin
 from requests import Session
 import aiohttp
 import logging
 from icecream import ic
+import shutil
 
 
 class LiveServerSession(Session):
     """https://stackoverflow.com/a/51026159/364388"""
 
     def __init__(self, *args, **kwargs):
         super(LiveServerSession, self).__init__(*args, **kwargs)
@@ -63,7 +65,14 @@
         file_paths = [f'{module_path}/test_data/file_1.txt',
                       f'{module_path}/test_data/file_2.txt']
     data = [('files', open(path, 'rb')) for path in file_paths]
     data = aiohttp.FormData()
     for path in file_paths:
         data.add_field('files',  open(path, 'rb'))
     return data
+
+
+def unzip(file_path, target_folder):
+    shutil.rmtree(target_folder, ignore_errors=True)
+    os.makedirs(target_folder)
+    with zipfile.ZipFile(file_path, 'r') as zip:
+        zip.extractall(target_folder)
```

### Comparing `learning_loop_node-0.7.8/learning_loop_node/tests/test_learning_loop_node.py` & `learning_loop_node-0.7.9/learning_loop_node/tests/test_learning_loop_node.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/downloader.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/downloader.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/executor.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/executor.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/tests/trainer_test_helper.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/tests/trainer_test_helper.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/trainer.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/trainer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from abc import abstractmethod
 import asyncio
 import os
 from typing import Dict, List, Optional, Union
 from uuid import uuid4
+from learning_loop_node.rest.downloader import DataDownloader
+from learning_loop_node.loop import loop
+from ..model_information import ModelInformation
 from .executor import Executor
 from .training import Training
 from .model import BasicModel, PretrainedModel
 from ..context import Context
 from ..node import Node
 from .downloader import TrainingsDownloader
 from ..rest import downloads, uploads
 from .. import node_helper
 import logging
 from icecream import ic
 from .helper import is_valid_uuid4
-
+from glob import glob
+import json
+from fastapi.encoders import jsonable_encoder
+import shutil
 
 class Trainer():
 
     def __init__(self, model_format: str) -> None:
         self.model_format: str = model_format
         self.training: Optional[Training] = None
         self.executor: Optional[Executor] = None
@@ -30,14 +36,15 @@
         self.training.data = await downloader.download_training_data(self.training.images_folder)
         self.executor = Executor(self.training.training_folder)
 
         self.source_model_id = source_model['id']
         if not is_valid_uuid4(self.source_model_id):
             if self.source_model_id in [m.name for m in self.provided_pretrained_models]:
                 logging.debug('Should start with pretrained model')
+                self.ensure_model_json()
                 await self.start_training_from_scratch(self.source_model_id)
             else:
                 raise ValueError(f'Pretrained model {self.source_model_id} is not supported')
         else:
             logging.debug('Should start with loop model')
             logging.info(f'downloading model {self.source_model_id} as {self.model_format}')
             await downloads.download_model(self.training.training_folder, context, self.source_model_id, self.model_format)
@@ -106,14 +113,59 @@
         a dictionary mapping format -> list of files can be returned.
         Each format should contain a model.json in the file list. 
         This file contains the trained resolution, categories including their learning loop ids to be robust about renamings etc.
         Example: {"resolution": 832, "categories":[{"name": "A", "id": "<a uuid>", "type": "box"}]}
         '''
         raise NotImplementedError()
 
+    async def do_detections(self, context: Context, model_id: str, model_format: str):
+        tmp_folder = f'/tmp/model_for_auto_detections_{model_id}_{model_format}'
+        
+        shutil.rmtree(tmp_folder, ignore_errors=True)
+        os.makedirs(tmp_folder)
+        logging.info('downloading model for detecting')
+        try:
+            await downloads.download_model(tmp_folder, context, model_id, model_format)
+        except:
+            logging.exception('download error')
+        with open(f'{tmp_folder}/model.json', 'r') as f:
+            content = json.load(f)
+            model_information = ModelInformation.parse_obj(content)
+
+        project_folder = Node.create_project_folder(context)
+        image_folder = node_helper.create_image_folder(project_folder)
+        downloader = DataDownloader(context)
+        image_ids = []
+        for state in ['inbox', 'annotate', 'review', 'complete']:
+            basic_data = await downloader.download_basic_data(query_params=f'state={state}')
+            image_ids += basic_data.image_ids
+            await downloader.download_images(basic_data.image_ids, image_folder)
+        images = [img for img in glob(f'{image_folder}/**/*.*', recursive=True) if os.path.splitext(os.path.basename(img))[0] in image_ids]
+        logging.info(f'running detections on {len(images)} images')
+        detections = await self._detect(model_information, images, tmp_folder, model_id, 'some_model_version')
+        logging.info(f'uploading {len(detections)} detections')
+        await self._upload_detections(context, jsonable_encoder(detections))
+        return detections
+
+    async def _detect(self, model_information: ModelInformation, images:  List[str], model_folder: str, model_id: str, model_version: str) -> List:
+        raise NotImplementedError()
+
+    async def _upload_detections(self, context: Context, detections: List[dict]):
+        logging.info('uploading detections')
+        try:
+            data = json.dumps(detections)
+            logging.info(f'uploading detections. File size : {len(data)}')
+            async with loop.post(f'api/{context.organization}/projects/{context.project}/detections', data=data) as response:
+                if response.status != 200:
+                    logging.error(f'could not upload detections. {str(response)}')
+                else:
+                    logging.info('successfully uploaded detections')
+        except:
+            logging.exception('error uploading detections.')
+
     async def clear_training_data(self, training_folder: str) -> None:
         '''Called after a training has finished. Deletes all data that is not needed anymore after a training run. This can be old
         weightfiles or any additional files.
         '''
         raise NotImplementedError()
 
     @property
@@ -134,7 +186,13 @@
         )
 
     @staticmethod
     def create_training_folder(project_folder: str, trainings_id: str) -> str:
         training_folder = f'{project_folder}/trainings/{trainings_id}'
         os.makedirs(training_folder, exist_ok=True)
         return training_folder
+
+    def ensure_model_json(self):
+        modeljson_path = f'{self.training.training_folder}/model.json'
+        if not os.path.exists(modeljson_path):
+            with open(modeljson_path, 'w') as f:
+                f.write('{}')
```

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/trainer_node.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/trainer_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,19 @@
                 await self.check_state()
             except:
                 logging.exception('could not check state')
 
         @self.on_event("shutdown")
         async def shutdown():
             logging.info('shutdown detected, stopping training')
-            await self.stop_training()
+            try:
+                self.trainer.training.excecutor.stop()
+            except:
+                logging.exception('could not kill training.')
+                pass
 
     async def begin_training(self, context: Context, source_model: dict):
         self.status.reset_error('start_training')
         await self.update_state(State.Preparing)
         try:
             await self.trainer.begin_training(context, source_model)
         except Exception as e:
@@ -81,15 +85,20 @@
             result = self.trainer.stop_training()
             if self.latest_known_model_id and self.trainer.source_model_id != self.latest_known_model_id:
                 if save_latest_model:
                     await self.update_state(State.Uploading)
                     await self.save_model(self.trainer.training.context, self.latest_known_model_id)
                 if do_detections:
                     await self.update_state(State.Detecting)
-                    await asyncio.sleep(1)
+                    try:
+                        await self.trainer.do_detections(context=self.trainer.training.context,
+                                                         model_id=self.latest_known_model_id,
+                                                         model_format=self.trainer.model_format)
+                    except Exception as e:
+                        logging.exception(f'Could not predict detections: {str(e)}')
 
             await self.clear_training_data(self.trainer.training.training_folder)
             self.trainer.training = None
             self.latest_known_model_id = None
             await self.update_state(State.Idle)
             if not result:
                 raise Exception('No Training is running')
@@ -209,13 +218,14 @@
 
         if not response.success:
             logging.error(f'Error for updating: Response from loop was : {response.__dict__}')
             logging.error('Going to kill training. ')
             logging.exception('update trainer failed')
 
             if status.state != State.Idle:
+                # TODO was soll passieren, wenn wir z.B. Stopping sind, und das Event von der Loop abgelehnt wird?
                 await self.stop_training(do_detections=False, save_latest_model=False)
 
     def get_state(self):
         if self.trainer.executor is not None and self.trainer.executor.is_process_running():
             return State.Running
         return State.Idle
```

### Comparing `learning_loop_node-0.7.8/learning_loop_node/trainer/training_data.py` & `learning_loop_node-0.7.9/learning_loop_node/trainer/training_data.py`

 * *Files identical despite different names*

### Comparing `learning_loop_node-0.7.8/pyproject.toml` & `learning_loop_node-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "learning_loop_node"
-version = "v0.7.8"
+version = "v0.7.9"
 description = "Python Library for Nodes which connect to the Zauberzeug Learning Loop"
 authors = ["Zauberzeug GmbH <info@zauberzeug.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/zauberzeug/learning_loop_node"
 
 [tool.poetry.dependencies]
```

### Comparing `learning_loop_node-0.7.8/setup.py` & `learning_loop_node-0.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'requests>=2.25.1,<3.0.0',
  'simplejson>=3.17.2,<4.0.0',
  'uvicorn>=0.13.3,<0.14.0',
  'werkzeug>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'learning-loop-node',
-    'version': '0.7.8',
+    'version': '0.7.9',
     'description': 'Python Library for Nodes which connect to the Zauberzeug Learning Loop',
     'long_description': '# Learning Loop Node\n\nThis Python library helps you to write your own Detection Nodes, Training Nodes and Converter Nodes for the Zauberzeug Learning Loop.\n\n## General Usage\n\nYou can configure connection to our Learning Loop by specifying the following environment variables before starting:\n\n- LOOP_HOST=learning-loop.ai\n- LOOP_USERNAME=<your username>\n- LOOP_PASSWORD=<your password>\n\n## Detector Node\n\nDetector Nodes are normally deployed on edge devices like robots or machinery but can also run in the cloud to provide backend services for an app or similar. These nodes register themself at the Learning Loop to make model deployments very easy. They also provide REST and Socket.io APIs to run inferences. By default the images will automatically used for active learning: high uncertain predictions will be submitted to the Learning Loop inbox.\n\n#### Additinal environment variables\n\n- LOOP_ORGANIZATION=<your organization>\n- LOOP_PROJECT=<your project>\n\n## Trainer Node\n\nTrainers fetch the images and anntoations from the Learning Loop to generate new and improved models.\n\n- if the command line tool "jpeginfo" is installed, the downloader will drop corrupted images automatically\n\n## Converter Node\n\nA Conveter Node converts models from one format into another.\n\n### How to test the operability?\n\nAssumend there is a Converter Node which converts models of format \'format_a\' into \'format_b\'.\nUpload a model with\n`curl --request POST -F \'files=@my_model.zip\' https://learning-loop.ai/api/zauberzeug/projects/demo/format_a`\nThe model should now be available for the format \'format_a\'\n`curl "https://learning-loop.ai/api/zauberzeug/projects/demo/models?format=format_a"`\n\n```\n{\n  "models": [\n    {\n      "id": "3c20d807-f71c-40dc-a996-8a8968aa5431",\n      "version": "4.0",\n      "formats": [\n        "format_a"\n      ],\n      "created": "2021-06-01T06:28:21.289092",\n      "comment": "uploaded at 2021-06-01 06:28:21.288442",\n      ...\n    }\n  ]\n}\n\n```\n\nbut not in the format_b\n`curl "https://learning-loop.ai/api/zauberzeug/projects/demo/models?format=format_b"`\n\n```\n{\n  "models": []\n}\n```\n\nConnect the Node to the Learning Loop by simply starting the container.\nAfter a short time the converted model should be available as well.\n`curl https://learning-loop.ai/api/zauberzeug/projects/demo/models?format=format_b`\n\n```\n{\n  "models": [\n    {\n      "id": "3c20d807-f71c-40dc-a996-8a8968aa5431",\n      "version": "4.0",\n      "formats": [\n        "format_a",\n        "format_b",\n      ],\n      "created": "2021-06-01T06:28:21.289092",\n      "comment": "uploaded at 2021-06-01 06:28:21.288442",\n      ...\n    }\n  ]\n}\n```\n\n## About Models (the currency between Nodes)\n\n- Models are packed in zips and saved on the Learning Loop (one for each format)\n- Nodes and users can upload and download models with which they want to work\n- In each zip there is a file called `model.json` which contains the metadata to interpret the other files in the package\n- for base models (pretrained models from external sources) no `model.json` has to be sent, ie. these models should simply be zipped in such a way that the respective trainer can work with them.\n- the loop adds or corrects the following properties in the `model.json` after receiving; it also creates the file if it is missing:\n  - `host`: uri to the loop\n  - `organization`: the ID of the organization\n  - `project`: the id of the project\n  - `version`: the version number that the loop assigned for this model (e.g. 1.3)\n  - `id`: the model UUID (currently not needed by anyone, since host, org, project, version clearly identify the model)\n  - `format`: the format e.g. yolo, tkdnn, yolor etc.\n- Nodes add properties to `model.json`, which contains all the information which are needed by subsequent nodes. These are typically the properties:\n  - `resolution`: resolution in which the model expects images (as `int`, since the resolution is mostly square - later, ` resolution_x`` resolution_y ` would also be conceivable or `resolutions` to give a list of possible resolutions)\n  - `categories`: list of categories with name, id, (later also type), in the order in which they are used by the model -- this is neccessary to be robust about renamings\n',
     'author': 'Zauberzeug GmbH',
     'author_email': 'info@zauberzeug.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/zauberzeug/learning_loop_node',
```

### Comparing `learning_loop_node-0.7.8/PKG-INFO` & `learning_loop_node-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning-loop-node
-Version: 0.7.8
+Version: 0.7.9
 Summary: Python Library for Nodes which connect to the Zauberzeug Learning Loop
 Home-page: https://github.com/zauberzeug/learning_loop_node
 License: MIT
 Author: Zauberzeug GmbH
 Author-email: info@zauberzeug.com
 Requires-Python: >=3.6.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


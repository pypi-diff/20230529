# Comparing `tmp/coretex-1.0.0.tar.gz` & `tmp/coretex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.0.tar", last modified: Fri May 26 00:03:11 2023, max compression
+gzip compressed data, was "coretex-1.0.1.tar", last modified: Mon May 29 15:22:49 2023, max compression
```

## Comparing `coretex-1.0.0.tar` & `coretex-1.0.1.tar`

### file list

```diff
@@ -1,179 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.304675 coretex-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-05-26 00:02:58.000000 coretex-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-26 00:03:11.304675 coretex-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-26 00:02:58.000000 coretex-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-26 00:02:58.000000 coretex-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:03:11.304675 coretex-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.272674 coretex-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.280674 coretex-1.0.0/src/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.284674 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/network_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/executing_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.288674 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/experiment/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.292675 coretex-1.0.0/src/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.296675 coretex-1.0.0/src/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.300675 coretex-1.0.0/src/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.304675 coretex-1.0.0/src/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-26 00:02:58.000000 coretex-1.0.0/src/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:03:11.276674 coretex-1.0.0/src/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 00:03:11.000000 coretex-1.0.0/src/coretex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.247695 coretex-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-05-29 15:22:34.000000 coretex-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-29 15:22:49.247695 coretex-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-29 15:22:34.000000 coretex-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-29 15:22:34.000000 coretex-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:22:49.247695 coretex-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.207694 coretex-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.219694 coretex-1.0.1/src/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.219694 coretex-1.0.1/src/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.219694 coretex-1.0.1/src/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.219694 coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.223694 coretex-1.0.1/src/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.223694 coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.223694 coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.227694 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.227694 coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/network_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.227694 coretex-1.0.1/src/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/executing_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.227694 coretex-1.0.1/src/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.231695 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/experiment/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.231695 coretex-1.0.1/src/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.231695 coretex-1.0.1/src/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.235695 coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.235695 coretex-1.0.1/src/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.235695 coretex-1.0.1/src/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.235695 coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.239695 coretex-1.0.1/src/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.239695 coretex-1.0.1/src/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.239695 coretex-1.0.1/src/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.239695 coretex-1.0.1/src/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.243695 coretex-1.0.1/src/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.243695 coretex-1.0.1/src/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.243695 coretex-1.0.1/src/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.243695 coretex-1.0.1/src/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.247695 coretex-1.0.1/src/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 15:22:34.000000 coretex-1.0.1/src/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:22:49.215694 coretex-1.0.1/src/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-29 15:22:49.000000 coretex-1.0.1/src/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-29 15:22:49.000000 coretex-1.0.1/src/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:22:49.000000 coretex-1.0.1/src/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 15:22:49.000000 coretex-1.0.1/src/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 15:22:49.000000 coretex-1.0.1/src/coretex.egg-info/top_level.txt
```

### Comparing `coretex-1.0.0/LICENSE` & `coretex-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/PKG-INFO` & `coretex-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>, Igor Perić <igor@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Linter code check](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml/badge.svg?branch=develop)](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml)
+
 ![](https://coretex.ai/images/coretex_logo_new.svg)
 
 <h1 style="text-align: center;">Coretex.ai Python library</h1>
 
 Manage the complete lifecycle of your experiments and complex workloads, from project inception to production deployment and monitoring.
 
 ## What is Coretex.ai?
```

### Comparing `coretex-1.0.0/README.md` & `coretex-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+[![Linter code check](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml/badge.svg?branch=develop)](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml)
+
 ![](https://coretex.ai/images/coretex_logo_new.svg)
 
 <h1 style="text-align: center;">Coretex.ai Python library</h1>
 
 Manage the complete lifecycle of your experiments and complex workloads, from project inception to production deployment and monitoring.
 
 ## What is Coretex.ai?
```

### Comparing `coretex-1.0.0/pyproject.toml` & `coretex-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coretex"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
   { name="Darko Zarić", email="dzaric@coretex.ai" },
```

### Comparing `coretex-1.0.0/src/coretex/__init__.py` & `coretex-1.0.1/src/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/_configuration.py` & `coretex-1.0.1/src/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/_logger.py` & `coretex-1.0.1/src/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/cache/__init__.py` & `coretex-1.0.1/src/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/cache/cache_module.py` & `coretex-1.0.1/src/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/codable/__init__.py` & `coretex-1.0.1/src/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/codable/codable.py` & `coretex-1.0.1/src/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/codable/descriptor.py` & `coretex-1.0.1/src/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/__init__.py` & `coretex-1.0.1/src/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/annotation/__init__.py` & `coretex-1.0.1/src/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.1/src/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.1/src/coretex/coretex/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.1/src/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.1/src/coretex/coretex/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/__init__.py` & `coretex-1.0.1/src/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.1/src/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/__init__.py` & `coretex-1.0.1/src/coretex/coretex/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.1/src/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/dataset/utils.py` & `coretex-1.0.1/src/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/__init__.py` & `coretex-1.0.1/src/coretex/coretex/experiment/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -15,8 +15,8 @@
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .artifact import Artifact
 from .experiment import Experiment
 from .status import ExperimentStatus
 from .executing_experiment import ExecutingExperiment
-from .metrics import MetricType
+from .metrics import Metric, MetricType
```

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/artifact.py` & `coretex-1.0.1/src/coretex/coretex/experiment/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/executing_experiment.py` & `coretex-1.0.1/src/coretex/coretex/experiment/executing_experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/experiment.py` & `coretex-1.0.1/src/coretex/coretex/experiment/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -24,15 +24,15 @@
 import os
 import time
 import logging
 import zipfile
 
 from .artifact import Artifact
 from .status import ExperimentStatus
-from .metrics import Metric, getClassForMetric, MetricType
+from .metrics import Metric
 from ..space import SpaceTask
 from ...codable import KeyDescriptor
 from ...networking import networkManager, NetworkObject, RequestType, NetworkRequestError
 from ...folder_management import FolderManager
 
 
 class Experiment(NetworkObject):
@@ -203,58 +203,59 @@
                 if response.hasFailed():
                     logging.getLogger("coretexpylib").error(">> [Coretex] Error while updating experiment status")
 
                 return not response.hasFailed()
 
             return True
 
-    def createMetrics(self, values: List[Tuple[str, str, MetricType, str, MetricType]]) -> List[Metric]:
+    def createMetrics(self, metrics: List[Metric]) -> None:
         """
             Creates specified metrics for the experiment
 
             Parameters
             ----------
-            values : List[Tuple[str, str, MetricType, str, MetricType]]
-                Metric meta in this format ("name", "x_label", "x_type", "y_label", "y_type")
+            values : List[Metric]]
+                List of Metric meta objects in this format
+                Metric("name", "x_label", "x_type", "y_label", "y_type", "x_range", "y_range")
 
             Returns
             -------
             List[Metric] -> List of Metric objects
 
+            Raises
+            ------
+            NetworkRequestError -> if the request failed
+
             Example
             -------
             >>> from coretex import ExecutingExperiment, MetricType
             \b
             >>> metrics = ExecutingExperiment.current().createMetrics([
-                    ("loss", "epoch", MetricType.int, "value", MetricType.float),
-                    ("accuracy", "epoch", MetricType.int, "value", MetricType.float)
+                    Metric.create("loss", "epoch", MetricType.int, "value", MetricType.float, None, [0, 100]),
+                    Metric.create("accuracy", "epoch", MetricType.int, "value", MetricType.float, None, [0, 100])
                 ])
             >>> if len(metrics) == 0:
                     print("Failed to create metrics")
         """
 
-        if not Metric.createMetrics(self.id, values):
-            logging.getLogger("coretexpylib").info(">> [Coretex] Failed to create metrics!")
-            return []
-
-        metrics: List[Metric] = []
-        for name, xLabel, xType, yLabel, yType in values:
-            clazz = getClassForMetric(name)
-
-            if clazz is not None:
-                metric = clazz.create(name, xLabel, xType, yLabel, yType)
-                metrics.append(metric)
-
-            else:
-                metric = Metric.create(name, xLabel, xType, yLabel, yType)
-                metrics.append(metric)
+        parameters: Dict[str, Any] = {
+            "experiment_id": self.id,
+            "metrics": [metric.encode() for metric in metrics]
+        }
 
-        self.metrics.extend(metrics)
+        response = networkManager.genericJSONRequest(
+            "model-queue/metrics-meta",
+            RequestType.post,
+            parameters
+        )
 
-        return self.metrics
+        if response.hasFailed():
+            raise NetworkRequestError(response, ">> [Coretex] Failed to create metrics!")
+
+        self.metrics.extend(metrics)
 
 
     def submitMetrics(self, metricValues: Dict[str, Tuple[float, float]]) -> bool:
         """
             Appends metric values for the provided metrics
 
             Parameters
@@ -272,28 +273,28 @@
                 })
             >>> print(result)
             True
         """
 
         metrics = [{
             "timestamp": time.time(),
-            "metric": k,
-            "x": v[0],
-            "y": v[1]} for k, v in metricValues.items()]
+            "metric": key,
+            "x": value[0],
+            "y": value[1]
+        } for key, value in metricValues.items()]
 
         parameters: Dict[str, Any] = {
             "experiment_id": self.id,
             "metrics": metrics
         }
 
-        endpoint =  "model-queue/metrics"
         response = networkManager.genericJSONRequest(
-            endpoint = endpoint,
-            requestType = RequestType.post,
-            parameters = parameters
+            "model-queue/metrics",
+            RequestType.post,
+            parameters
         )
 
         return not response.hasFailed()
 
     def getLastStatusMessage(self) -> Optional[str]:
         return self.__lastStatusMessage
```

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -12,10 +12,9 @@
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .metric import Metric
-from .metric_factory import getClassForMetric
 from .utils import getNetworkUsage
 from .metric_type import MetricType
```

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Type, Optional
+from typing import Type, Optional, List
 
-from .metric import Metric
+from .metric import Metric, MetricType
 from .predefined_metrics import *
 
 
 def getClassForMetric(name: str) -> Optional[Type[Metric]]:
     if name == "disk_read":
         return MetricDiskRead
 
@@ -30,20 +30,40 @@
 
     if name == "cpu_usage":
         return MetricCPUUsage
 
     if name == "ram_usage":
         return MetricRAMUsage
 
+    if name == "swap_usage":
+        return MetricSwapUsage
+
     if name == "gpu_usage":
         return MetricGPUUsage
 
     if name == "gpu_temperature":
         return MetricGPUTemperature
 
     if name == "upload_speed":
         return MetricUploadSpeed
 
     if name == "download_speed":
         return MetricDownloadSpeed
 
     return None
+
+
+def createMetric(
+    name: str,
+    xLabel: str,
+    xType: MetricType,
+    yLabel: str,
+    yType: MetricType,
+    xRange: Optional[List[float]] = None,
+    yRange: Optional[List[float]] = None
+) -> Metric:
+
+    metric = getClassForMetric(name)
+    if metric is None:
+        raise ValueError(f"[Coretex] Failed to create {name} metric")
+
+    return metric.create(name, xLabel, xType, yLabel, yType, xRange, yRange)
```

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -19,7 +19,8 @@
 from .disk_read import MetricDiskRead
 from .disk_write import MetricDiskWrite
 from .download_speed import MetricDownloadSpeed
 from .gpu_temperature import MetricGPUTemperature
 from .gpu_usage import MetricGPUUsage
 from .ram_usage import MetricRAMUsage
 from .upload_speed import MetricUploadSpeed
+from .swap_usage import MetricSwapUsage
```

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.1/src/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/parameters.py` & `coretex-1.0.1/src/coretex/coretex/experiment/parameters.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/experiment/status.py` & `coretex-1.0.1/src/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/model/__init__.py` & `coretex-1.0.1/src/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/model/model.py` & `coretex-1.0.1/src/coretex/coretex/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/__init__.py` & `coretex-1.0.1/src/coretex/coretex/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.1/src/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.1/src/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/local_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/network_sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/sample/sample.py` & `coretex-1.0.1/src/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/space/__init__.py` & `coretex-1.0.1/src/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/space/base.py` & `coretex-1.0.1/src/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/space/project.py` & `coretex-1.0.1/src/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/space/space.py` & `coretex-1.0.1/src/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/coretex/space/space_task.py` & `coretex-1.0.1/src/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/folder_management/__init__.py` & `coretex-1.0.1/src/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/folder_management/folder_manager.py` & `coretex-1.0.1/src/coretex/folder_management/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/logging/__init__.py` & `coretex-1.0.1/src/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/logging/log.py` & `coretex-1.0.1/src/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/logging/log_severity.py` & `coretex-1.0.1/src/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/logging/logger.py` & `coretex-1.0.1/src/coretex/logging/logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/__init__.py` & `coretex-1.0.1/src/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/chunk_upload_session.py` & `coretex-1.0.1/src/coretex/networking/chunk_upload_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -102,15 +102,15 @@
             "end": end - 1  # API expects start/end to be inclusive
         }
 
         response = networkManager.genericUpload("upload/chunk", files, parameters)
         if response.hasFailed():
             raise NetworkRequestError(response, f"Failed to upload file chunk with byte range \"{start}-{end}\"")
 
-        logging.getLogger("coretexpylib").info(f">> [Coretex] Uploaded chunk with range \"{start}-{end}\"")
+        logging.getLogger("coretexpylib").debug(f">> [Coretex] Uploaded chunk with range \"{start}-{end}\"")
 
     def run(self) -> str:
         """
             Uploads the file to Coretex.ai
 
             Returns
             -------
@@ -130,15 +130,15 @@
             \b
             >>> try:
                     uploadId = uploadSession.run()
                     print(uploadId)
                 except NetworkRequestError, ValueError:
                     print("Failed to upload file")
         """
-        logging.getLogger("coretexpylib").info(f">> [Coretex] Starting upload for \"{self.filePath}\"")
+        logging.getLogger("coretexpylib").debug(f">> [Coretex] Starting upload for \"{self.filePath}\"")
 
         uploadId = self.__start()
 
         chunkCount = self.fileSize // self.chunkSize
         if self.fileSize % self.chunkSize != 0:
             chunkCount += 1
```

### Comparing `coretex-1.0.0/src/coretex/networking/network_manager.py` & `coretex-1.0.1/src/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/network_manager_base.py` & `coretex-1.0.1/src/coretex/networking/network_manager_base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/network_object.py` & `coretex-1.0.1/src/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/network_response.py` & `coretex-1.0.1/src/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/request_type.py` & `coretex-1.0.1/src/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/requests_manager.py` & `coretex-1.0.1/src/coretex/networking/requests_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/networking/user_data.py` & `coretex-1.0.1/src/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/__init__.py` & `coretex-1.0.1/src/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/text.py` & `coretex-1.0.1/src/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/token.py` & `coretex-1.0.1/src/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/transcriber.py` & `coretex-1.0.1/src/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/transcription.py` & `coretex-1.0.1/src/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/nlp/utils.py` & `coretex-1.0.1/src/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/project/__init__.py` & `coretex-1.0.1/src/coretex/project/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU Affero General Public License for more details.
 
 #     You should have received a copy of the GNU Affero General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Callable, Optional, Type, TypeVar, Tuple, List
+from typing import Callable, Optional, Type, TypeVar, List
 from enum import IntEnum
 
 import logging
 import sys
 
 from .remote import processRemote
 from .local import processLocal
-from ..coretex import ExperimentStatus, NetworkDataset, ExecutingExperiment, MetricType
+from ..coretex import ExperimentStatus, NetworkDataset, ExecutingExperiment, Metric
 from ..logging import LogHandler, initializeLogger, LogSeverity
 from ..networking import RequestFailedError
 from ..folder_management import FolderManager
 
 
 DatasetType = TypeVar("DatasetType", bound = "NetworkDataset")
 
@@ -38,28 +38,29 @@
      local = 1
      remote = 2
 
 
 def _prepareForExecution(
      experimentId: int,
      datasetType: Optional[Type[DatasetType]] = None,
-     metrics: Optional[List[Tuple[str, str, MetricType, str, MetricType]]] = None
+     metrics: Optional[List[Metric]] = None
 ) -> None:
+
      experiment = ExecutingExperiment.startExecuting(experimentId, datasetType)
 
      logPath = FolderManager.instance().logs / f"{experimentId}.log"
      customLogHandler = LogHandler.instance()
      customLogHandler.currentExperimentId = experimentId
 
-     # if logLevel exists apply it, otherwise default to info
+     # enable/disable verbose mode for experiments
      severity = LogSeverity.info
-     logLevel = experiment.parameters.get("logLevel")
+     verbose = experiment.parameters.get("verbose", False)
 
-     if logLevel is not None:
-          severity = LogSeverity(logLevel)
+     if verbose:
+          severity = LogSeverity.debug
 
      initializeLogger(severity, logPath)
 
      experiment.updateStatus(
           status = ExperimentStatus.inProgress,
           message = "Executing project."
      )
@@ -70,29 +71,30 @@
           if len(ExecutingExperiment.current().metrics) > 0:
                logging.getLogger("coretexpylib").info(">> [Coretex] Metrics successfully created.")
 
 
 def initializeProject(
      mainFunction: Callable[[ExecutingExperiment], None],
      datasetType: Optional[Type[DatasetType]] = None,
-     metrics: Optional[List[Tuple[str, str, MetricType, str, MetricType]]] = None,
+     metrics: Optional[List[Metric]] = None,
      args: Optional[List[str]] = None
 ) -> None:
+
      """
           Initializes and starts the python project as
           Coretex experiment
 
           Parameters
           ----------
           mainFunction : Callable[[ExecutingExperiment], None]
                entry point function
           datasetType : Optional[Type[DatasetType]]
                Custom dataset if there is any (Not required)
-          metrics : Optional[List[Tuple[str, str, MetricType, str, MetricType]]]
-               list of metrics that will be created for executing Experiment
+          metrics : Optional[List[Metric]]
+               list of metric objects that will be created for executing Experiment
           args : Optional[List[str]]
                list of command line arguments, if None sys.argv will be used
      """
 
      try:
           experimentId, callback = processRemote(args)
      except:
```

### Comparing `coretex-1.0.0/src/coretex/project/base.py` & `coretex-1.0.1/src/coretex/project/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/project/calculate_metrics.py` & `coretex-1.0.1/src/coretex/project/calculate_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -17,25 +17,27 @@
 
 from typing import Tuple, Dict
 from multiprocessing.connection import Connection
 
 import time
 
 from ..coretex import MetricType
-from ..networking import networkManager
-from ..coretex.experiment.experiment import Experiment
+from ..networking import networkManager, NetworkRequestError
+from ..coretex.experiment import Experiment
+from ..coretex.experiment.metrics.metric_factory import createMetric
 
 
 METRICS = [
-    ("cpu_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent),
-    ("ram_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent),
-    ("download_speed", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
-    ("upload_speed", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
-    ("disk_read", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
-    ("disk_write", "time (s)", MetricType.interval, "bytes", MetricType.bytes)
+    createMetric("cpu_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent, None, [0, 100]),
+    createMetric("ram_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent, None, [0, 100]),
+    createMetric("swap_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent, None, [0, 100]),
+    createMetric("download_speed", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
+    createMetric("upload_speed", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
+    createMetric("disk_read", "time (s)", MetricType.interval, "bytes", MetricType.bytes),
+    createMetric("disk_write", "time (s)", MetricType.interval, "bytes", MetricType.bytes)
 ]
 
 
 def sendSuccess(conn: Connection, message: str) -> None:
     conn.send({
         "code": 0,
         "message": message
@@ -56,16 +58,16 @@
     # automatically be performed
 
     try:
         from py3nvml import py3nvml
         py3nvml.nvmlInit()
 
         METRICS.extend([
-            ("gpu_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent),
-            ("gpu_temperature", "time (s)", MetricType.interval, "usage (%)", MetricType.percent)
+            createMetric("gpu_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent, None, [0, 100]),
+            createMetric("gpu_temperature", "time (s)", MetricType.interval, "usage (%)", MetricType.percent)
         ])
     except:
         pass
 
 
 def uploadMetricsWorker(outputStream: Connection, refreshToken: str, experimentId: int) -> None:
     setupGPUMetrics()
@@ -76,18 +78,18 @@
         return
 
     experiment = Experiment.fetchById(experimentId)
     if experiment is None:
         sendFailure(outputStream, f"Failed to fetch experiment with id: {experimentId}")
         return
 
-    createdMetrics = experiment.createMetrics(METRICS)
-    if len(createdMetrics) == 0:
-        sendFailure(outputStream, "Failed to create metrics list")
-        return
+    try:
+        experiment.createMetrics(METRICS)
+    except NetworkRequestError:
+        sendFailure(outputStream, "Failed to create metrics")
 
     sendSuccess(outputStream, "Metrics worker succcessfully started")
 
     while True:
         startTime = time.time()
         metricValues: Dict[str, Tuple[float, float]] = {}
```

### Comparing `coretex-1.0.0/src/coretex/project/heartbeat.py` & `coretex-1.0.1/src/coretex/project/heartbeat.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/project/local.py` & `coretex-1.0.1/src/coretex/project/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #     Copyright (C) 2023  BioMech LLC
 
-#     This file is part of Coretex.ai  
+#     This file is part of Coretex.ai
 
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU Affero General Public License as
 #     published by the Free Software Foundation, either version 3 of the
 #     License, or (at your option) any later version.
 
 #     This program is distributed in the hope that it will be useful,
@@ -120,16 +120,17 @@
     parameters = ExperimentParameter.readExperimentConfig()
 
     experiment = Experiment.startCustomExperiment(
         parser.projectId,
         # Dummy Local node ID, hardcoded as it is only a temporary solution,
         # backend will add a new ExperimentType (local) which does not require a specific
         # node to run
-        43,
+        -1,
         parser.name,
         parser.description,
         parameters = [parameter.encode() for parameter in parameters]
     )
 
+    logging.getLogger("coretexpylib").info(f">> [Coretex] Created local experiment with ID \"{experiment.id}\"")
     experiment.updateStatus(ExperimentStatus.preparingToStart)
 
     return experiment.id, LocalProjectCallback(experiment, response.json["refresh_token"])
```

### Comparing `coretex-1.0.0/src/coretex/project/remote.py` & `coretex-1.0.1/src/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/qiime2/__init__.py` & `coretex-1.0.1/src/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/qiime2/utils.py` & `coretex-1.0.1/src/coretex/qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/threading/__init__.py` & `coretex-1.0.1/src/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/threading/threaded_data_processor.py` & `coretex-1.0.1/src/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/utils/__init__.py` & `coretex-1.0.1/src/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/utils/console_progress_bar.py` & `coretex-1.0.1/src/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/utils/date.py` & `coretex-1.0.1/src/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/utils/file.py` & `coretex-1.0.1/src/coretex/utils/file.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex/utils/number.py` & `coretex-1.0.1/src/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.0/src/coretex.egg-info/PKG-INFO` & `coretex-1.0.1/src/coretex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>, Igor Perić <igor@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+[![Linter code check](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml/badge.svg?branch=develop)](https://github.com/coretex-ai/coretexpylib/actions/workflows/linter-code-check.yml)
+
 ![](https://coretex.ai/images/coretex_logo_new.svg)
 
 <h1 style="text-align: center;">Coretex.ai Python library</h1>
 
 Manage the complete lifecycle of your experiments and complex workloads, from project inception to production deployment and monitoring.
 
 ## What is Coretex.ai?
```

### Comparing `coretex-1.0.0/src/coretex.egg-info/SOURCES.txt` & `coretex-1.0.1/src/coretex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
 src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
 src/coretex/coretex/model/__init__.py
 src/coretex/coretex/model/model.py
 src/coretex/coretex/sample/__init__.py
 src/coretex/coretex/sample/any_local_sample.py
 src/coretex/coretex/sample/local_sample.py
 src/coretex/coretex/sample/network_sample.py
```


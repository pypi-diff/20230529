# Comparing `tmp/idtrackerai-5.1.3.tar.gz` & `tmp/idtrackerai-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idtrackerai-5.1.3.tar", last modified: Wed May  3 10:34:26 2023, max compression
+gzip compressed data, was "idtrackerai-5.1.4.tar", last modified: Mon May 29 18:55:03 2023, max compression
```

## Comparing `idtrackerai-5.1.3.tar` & `idtrackerai-5.1.4.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-04-19 16:31:58.000000 idtrackerai-5.1.3/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1597 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3079 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/pyproject.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/setup.cfg
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idmatcherai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idmatcherai/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     9092 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idmatcherai/main.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3678 2023-05-03 10:01:42.000000 idtrackerai-5.1.3/src/idmatcherai/matcher.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/__init__.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/animals_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/animals_detection.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15562 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/animals_detection/segmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    31737 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/blob.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/constants.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7524 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3144 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossings_detection.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7286 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5057 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/model_area.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.573556 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      761 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5415 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4174 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.573556 idtrackerai-5.1.3/src/idtrackerai/data/
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/data/test_A.avi
--rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/data/test_B.avi
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    26226 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/fragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/fragmentation/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/fragmentation/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5058 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/fragmentation/fragmentation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8913 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/globalfragment.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    15885 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    23949 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_fragments.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13045 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/list_of_global_fragments.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      456 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4271 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/network/evaluate.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3854 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/learners.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1878 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/network_params.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4509 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/train.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8886 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/network/utils.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.577556 idtrackerai-5.1.3/src/idtrackerai/postprocess/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    27568 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/assign_them_all.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/compute_velocity_model.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    21435 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3634 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/erosion.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8545 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/get_trajectories.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5113 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_creation.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_to_csv.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    36591 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8680 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/accumulator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4270 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/assigner.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3700 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataloader.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6666 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataset.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5432 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/identity_transfer.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/tracker/network/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1452 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/get_predictions.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8824 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/stop_training_criteria.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5035 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/network/trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     7147 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/pre_trainer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    34367 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/tracker/tracker.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai/utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1144 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/utils/check_PyPI_version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai/utils/confparams.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2990 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/init_logger.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12515 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/utils/py_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    33048 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai/video.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.569556 idtrackerai-5.1.3/src/idtrackerai.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2824 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5732 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      371 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-05-03 10:34:26.000000 idtrackerai-5.1.3/src/idtrackerai.egg-info/top_level.txt
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6154 2023-05-03 10:04:54.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/GUI_main_base.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/logo_256.png
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/themes.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5909 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-03 10:01:51.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_start_app/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4975 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/all_valid_parameters.dat
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/arg_parser.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5405 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/run_idtrackerai.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    16140 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5827 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6625 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_start_app/tooltips.toml
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.581556 idtrackerai-5.1.3/src/idtrackerai_validator/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/__main__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/tooltips.toml
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    30957 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validation_GUI.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      491 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1752 2023-05-03 10:06:36.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/additional_info.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/errors_explorer.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_groups.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1654 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_labels.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12940 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/interpolator.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6246 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/paint_blobs.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-05-03 10:02:02.000000 idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/setup_points.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-03 10:34:26.585556 idtrackerai-5.1.3/src/idtrackerai_video/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-02 13:56:50.000000 idtrackerai-5.1.3/src/idtrackerai_video/__init__.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5289 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/general_video.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4110 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/individual_videos.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-03 10:04:26.000000 idtrackerai-5.1.3/src/idtrackerai_video/main.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    35987 2023-02-10 16:03:19.000000 idtrackerai-5.1.4/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1601 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3050 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/pyproject.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/setup.cfg
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idmatcherai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idmatcherai/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9102 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idmatcherai/main.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3643 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idmatcherai/matcher.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      587 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/__init__.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/animals_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6157 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/animals_detection.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15527 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/animals_detection/segmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31625 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/blob.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3215 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/constants.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       96 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7497 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3115 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossings_detection.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3947 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7161 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4938 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/model_area.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      828 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5107 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3101 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.770815 idtrackerai-5.1.4/src/idtrackerai/data/
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5933626 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/data/test_A.avi
+-rwxrwxr-x   0 jordi     (1000) jordi     (1000)  5976882 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/data/test_B.avi
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    26172 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/fragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/fragmentation/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       78 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/fragmentation/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4529 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/fragmentation/fragmentation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8468 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/globalfragment.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    22092 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    20302 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3924 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5589 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3989 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    15642 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27145 2023-05-29 18:33:25.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_fragments.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12556 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/list_of_global_fragments.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      459 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2556 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/evaluate.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3172 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/learners.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6563 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai/network/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2046 2023-05-29 18:41:52.000000 idtrackerai-5.1.4/src/idtrackerai/network/network_params.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2818 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/train.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2419 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/network/utils.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/postprocess/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      292 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    27711 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/assign_them_all.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2725 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/compute_velocity_model.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    21299 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3602 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/erosion.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8671 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/get_trajectories.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2592 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5168 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_creation.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_to_csv.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/tracker/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    37146 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3151 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8802 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/accumulator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5742 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/assigner.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.778815 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3593 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataloader.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6107 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataset.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5561 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/identity_transfer.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai/tracker/network/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1536 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/get_predictions.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     7058 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/stop_training_criteria.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3175 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/network/trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6820 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/pre_trainer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    31972 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/tracker/tracker.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai/utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1180 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2151 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/check_PyPI_version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1143 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai/utils/confparams.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2954 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/init_logger.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/utils/py_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    32730 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai/video.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.762814 idtrackerai-5.1.4/src/idtrackerai.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2828 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5795 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      341 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      351 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      108 2023-05-29 18:55:03.000000 idtrackerai-5.1.4/src/idtrackerai.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6454 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/GUI_main_base.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      794 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2448 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    66516 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/logo_256.png
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10027 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/themes.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      619 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5484 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/canvas.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6069 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8204 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2870 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13532 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_player.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_start_app/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4959 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1515 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/all_valid_parameters.dat
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6826 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/arg_parser.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5403 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/run_idtrackerai.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    16111 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8406 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      482 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5790 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5715 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3534 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2368 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6800 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5007 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2713 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_start_app/tooltips.toml
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.782815 idtrackerai-5.1.4/src/idtrackerai_validator/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      672 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/__main__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      715 2023-05-16 10:39:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/tooltips.toml
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    33550 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validation_GUI.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      547 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1904 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/additional_info.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     8104 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/errors_explorer.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6073 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_groups.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1505 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_labels.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    12933 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/interpolator.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4494 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/mark_properties.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6695 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/paint_blobs.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4835 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/setup_points.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:55:03.786815 idtrackerai-5.1.4/src/idtrackerai_video/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        0 2023-05-29 18:15:16.000000 idtrackerai-5.1.4/src/idtrackerai_video/__init__.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5289 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_video/general_video.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4085 2023-05-29 18:22:31.000000 idtrackerai-5.1.4/src/idtrackerai_video/individual_videos.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2961 2023-05-29 18:19:35.000000 idtrackerai-5.1.4/src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.3/LICENSE` & `idtrackerai-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/PKG-INFO` & `idtrackerai-5.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.3
+Version: 5.1.4
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -36,12 +36,12 @@
 
 ``` bash
 pip install git+https://gitlab.com/polavieja_lab/idtrackerai[dev,docs]
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
-* Antonio Ortega (2021-)
+* Antonio Ortega (2021-2023)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
 * Ricardo Ribeiro (2018-2020)
 * Francisco J.H. Heras (2015-2022)
```

### Comparing `idtrackerai-5.1.3/README.md` & `idtrackerai-5.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 ``` bash
 pip install git+https://gitlab.com/polavieja_lab/idtrackerai[dev,docs]
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
-* Antonio Ortega (2021-)
+* Antonio Ortega (2021-2023)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
 * Ricardo Ribeiro (2018-2020)
 * Francisco J.H. Heras (2015-2022)
```

### Comparing `idtrackerai-5.1.3/pyproject.toml` & `idtrackerai-5.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "idtrackerai"
-version = "5.1.3"
+version = "5.1.4"
 authors = [
     { name = "Jordi Torrents", email = "jordi.torrentsm@gmail.com" },
     { name = "Francisco Romero Ferrero" },
     { name = "Mattia G. Bergomi" },
     { name = "Francisco J.H. Heras" },
     { name = "Ricardo Ribeiro" },
 ]
@@ -29,15 +29,14 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "numpy >= 1.24.2",
     "rich >= 13.3.1",
-    "scikit-learn >= 1.2.1",
     "h5py >= 3.8.0",
     "scipy >= 1.10.0",
     "opencv-python-headless >= 4.7.0",
     "pyqt6 >= 6.4.2",
     'superqt >= 0.4.1',
     'toml >= 0.10.2',
     "matplotlib >= 3.7.0",
```

### Comparing `idtrackerai-5.1.3/src/idmatcherai/main.py` & `idtrackerai-5.1.4/src/idmatcherai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,26 +59,26 @@
             master_session.session_folder.name
         )
         create_dir(results_path)
         create_dir(results_path / "csv")
         create_dir(results_path / "png")
 
         direct_matches = match(
-            matching_session.id_images_folder, master_session.accumulation_folder
+            matching_session.id_images_folder, master_session.auto_accumulation_folder
         )
         save_matrix(
             direct_matches,
             results_path,
             "direct_matches",
             xlabel=master_session.session_folder.name,
             ylabel=matching_session.session_folder.name,
         )
 
         indirect_matches = match(
-            master_session.id_images_folder, matching_session.accumulation_folder
+            master_session.id_images_folder, matching_session.auto_accumulation_folder
         ).T
         save_matrix(
             indirect_matches,
             results_path,
             "indirect_matches",
             xlabel=master_session.session_folder.name,
             ylabel=matching_session.session_folder.name,
```

### Comparing `idtrackerai-5.1.3/src/idmatcherai/matcher.py` & `idtrackerai-5.1.4/src/idmatcherai/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
     identification_network_params = NetworkParams(
         schedule=params["schedule"],
         number_of_classes=params["number_of_classes"],
         architecture="idCNN",
         restore_folder=model_folder,
         model_name=params["model_name"],
-        dataset=params["dataset"],
         image_size=params["image_size"],
         use_gpu=True,
     )
 
     identification_model = LearnerClassification.load_model(
         identification_network_params
     )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/__init__.py` & `idtrackerai-5.1.4/src/idtrackerai/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/animals_detection/animals_detection.py` & `idtrackerai-5.1.4/src/idtrackerai/animals_detection/animals_detection.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/animals_detection/segmentation.py` & `idtrackerai-5.1.4/src/idtrackerai/animals_detection/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     --------
     Video
     Blob
     _get_videoCapture
     segment_frame
     blob_extractor
     """
-    (episode, video_paths, segmentation_parameters, segmentation_data_folder) = inputs
+    episode, video_paths, segmentation_parameters, segmentation_data_folder = inputs
     # Set file path to store blobs segmentation image and blobs pixels
     bbox_images_path = segmentation_data_folder / f"episode_images_{episode.index}.hdf5"
     remove_file(bbox_images_path)
 
     # Read video for the episode
     video_path = video_paths[episode.video_path_index]
     cap = cv2.VideoCapture(str(video_path))
@@ -196,17 +196,16 @@
         )
 
     # Applying the mask
     if ROI_mask is not None:
         segmented_frame *= ROI_mask  # type: ignore
 
     # Extract blobs info
-    # TODO cv2.CHAIN_APPROX_TC89_L1
     contours = cv2.findContours(
-        segmented_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        segmented_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_TC89_KCOS
     )[0]
 
     # Filter contours by size
     areas = []
     good_contours = []
     for contour in contours:
         area = cv2.contourArea(contour)
@@ -338,22 +337,22 @@
             progress_bar.emit(i)
     return frame_stack
 
 
 def generate_background_from_frame_stack(
     frame_stack: np.ndarray | None, stat=None
 ) -> np.ndarray | None:
-    logging.info(f"Computing background from a frame stack using '{stat}'")
-
     if frame_stack is None:
         return None
 
     if stat is None:
         stat = conf.BACKGROUND_SUBTRACTION_STAT
 
+    logging.info(f"Computing background from a frame stack using '{stat}'")
+
     if stat == "median":
         bkg = np.median(frame_stack, axis=0, overwrite_input=True)
     elif stat == "mean":
         bkg = np.mean(frame_stack, axis=0)
     elif stat == "max":
         bkg = np.max(frame_stack, axis=0)
     elif stat == "min":
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/blob.py` & `idtrackerai-5.1.4/src/idtrackerai/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 from functools import cached_property
 from itertools import chain
 from math import atan2, sqrt
 from pathlib import Path
-from typing import Sequence
+from typing import Iterable, Sequence
 
 import cv2
 import h5py
 import numpy as np
 
 
 class Blob:
@@ -76,26 +76,21 @@
         Resolution reductio factor as defined by the user, by default 1.0.
     """
 
     episode: int
     id_image_index: int
     """Index of the identification image position in the hdf5 file"""
 
+    seems_like_individual: bool = False
+    """Unicity condition or not huge area"""
+
     is_an_individual: bool
     """Flag indicating the blob represents a single animal.
     Defined in crossing detection."""
 
-    accumulation_step: int | None = None
-    """Integer indicating the accumulation step at which the blob was
-    accumulated"""
-
-    used_for_training: bool = False
-    """Flag indicating if the blob has been used to train the
-    identification CNN"""
-
     used_for_training_crossings: bool = False
     """Flag indicating if the blob has been used to train the
     crossing CNN"""
 
     was_a_crossing: bool = False
     """Flag indicating whether the blob was created after splitting a
     crossing blob during the crossings interpolation process"""
@@ -106,14 +101,16 @@
     next: list["Blob"]
     previous: list["Blob"]
 
     fragment_identifier: int = -1
     """Indicates the index of the Fragment that contains the blob,
     -1 means no associated Fragment"""
 
+    pixels_are_from_eroded_blob: bool = False
+
     blob_index: int = None  # type: ignore
     """Blob index at the segmentation step (comes from the find contours
     function of OpenCV)"""
 
     user_generated_identities: list[int | None] = None  # type: ignore
     """List of identities of the blob some of which might have been give
     by a user during the validation process"""
@@ -122,48 +119,57 @@
     """This property is give during the correction of impossible velocity
     jumps. It has nothing to do with the manual validation."""
 
     user_generated_centroids: list[tuple[float, float] | None] = None  # type: ignore
     """List of centroids generated by the user during the validation
     processes"""
 
-    P2_vector: list | np.ndarray | None
-
     identity_corrected_solving_jumps: int | None = None
     """Identity of the blob after correcting impossible velocity jumps"""
 
     identities_corrected_closing_gaps: list | None = None
     """Identity of the blob after crossings interpolation"""
 
     interpolated_centroids: list | None = None
 
     centroid: tuple[float, float]
 
     added_by_user: bool = False
 
+    forced_crossing: bool = False
+    """Indicates if the crossing attribute has been forced by set_individual_with_identity_0_as_crossings()"""
+
     def __init__(
         self,
         contour: np.ndarray,
         frame_number: int = -1,
         bbox_img_id: str = "",
         pixels_are_from_eroded_blob: bool = False,
     ):
         self.set_contour(contour)
         self.frame_number = frame_number
         self.bbox_img_id = bbox_img_id
-        self.pixels_are_from_eroded_blob = pixels_are_from_eroded_blob
         if pixels_are_from_eroded_blob:
+            self.pixels_are_from_eroded_blob = pixels_are_from_eroded_blob
             # TODO fix this, some eroded blobs are not classified as
             # individuals/crossings and idtrackerai crashes
             self.is_an_individual = True
-            self.P2_vector = None
+            self.forced_crossing = True
 
         self.next = []
         self.previous = []
 
+    @property
+    def n_next(self):
+        return len(self.next)
+
+    @property
+    def n_previous(self):
+        return len(self.previous)
+
     @cached_property
     def convexHull(self) -> np.ndarray:
         return cv2.convexHull(self.contour)
 
     @cached_property
     def area(self) -> int:
         return cv2.contourArea(self.contour)
@@ -204,15 +210,15 @@
         together.
 
         This attribute is the negative of `is_an_individual` and is set at
         the same time as is an individual
         """
         return not self.is_an_individual
 
-    def check_for_multiple_previous(self) -> bool:
+    def has_multiple_previous(self) -> bool:
         """Flag indicating if the blob has multiple blobs in its past or future
         overlapping history
 
         This method is used to check whether the blob is a crossing.
 
         Returns
         -------
@@ -226,15 +232,15 @@
         while len(current.previous) == 1:
             current = current.previous[0]
             if len(current.previous) > 1:
                 return True
 
         return False
 
-    def check_for_multiple_next(self) -> bool:
+    def has_multiple_next(self) -> bool:
         """Flag indicating if the blob has multiple blobs in its past or future
         overlapping history
 
         This method is used to check whether the blob is a crossing.
 
         Returns
         -------
@@ -257,45 +263,41 @@
 
         Returns
         -------
         bool
             If True the blob has a crossing in its "future" history
         """
         current = self.next[0]
-        while len(current.next) == 1:
+        while current.n_next == 1:
             current = current.next[0]
-            if len(current.previous) > 1 and current.is_a_crossing:
+            if current.n_previous > 1 and not current.seems_like_individual:
                 return True
         return False
 
     def check_for_crossing_previous(self) -> bool:
         """Flag indicating if the blob has a crossing in its past overlapping history
 
         Returns
         -------
         bool
             If True the blob has a crossing in its "past" history
         """
         current = self.previous[0]
-        while len(current.previous) == 1:
+        while current.n_previous == 1:
             current = current.previous[0]
-            if len(current.next) > 1 and current.is_a_crossing:
+            if current.n_next > 1 and not current.seems_like_individual:
                 return True
         return False
 
     def is_a_sure_individual(self) -> bool:
         """Flag indicating that the blob is a sure individual according to
         some heuristics and it can be used to train the crossing detector CNN.
-
-        Returns
-        -------
-        bool
         """
         return (
-            self.is_an_individual  # assigned in _apply_area_and_unicity_heuristics
+            self.seems_like_individual
             and len(self.previous) == 1
             and len(self.next) == 1
             and len(self.next[0].previous) == 1
             and len(self.previous[0].next) == 1
             and self.check_for_crossing_previous()
             and self.check_for_crossing_next()
         )
@@ -304,22 +306,20 @@
         """Flag indicating that the blob is a sure crossing according to
         some heuristics and it can be used to train the crossing detector CNN.
 
         Returns
         -------
         bool
         """
-        if self.is_an_individual:
+        if self.seems_like_individual:
             return False
         if len(self.previous) > 1 or len(self.next) > 1:
             return True
         if len(self.previous) == 1 and len(self.next) == 1:
-            has_multiple_previous = self.check_for_multiple_previous()
-            has_multiple_next = self.check_for_multiple_next()
-            return has_multiple_previous and has_multiple_next
+            return self.has_multiple_previous() and self.has_multiple_next()
         return False
 
     def overlaps_with(self, other: "Blob") -> bool:
         """Computes whether the pixels in `self` intersect with the pixels in
         `other`
 
         Parameters
@@ -331,18 +331,18 @@
         -------
         bool
             True if the lists of pixels of both blobs have non-empty
             intersection
         """
 
         # Check bounding boxes
-        (S_xmin, S_ymin) = self.bbox_in_frame_coordinates[0]
-        (S_xmax, S_ymax) = self.bbox_in_frame_coordinates[1]
-        (O_xmin, O_ymin) = other.bbox_in_frame_coordinates[0]
-        (O_xmax, O_ymax) = other.bbox_in_frame_coordinates[1]
+        S_xmin, S_ymin = self.bbox_in_frame_coordinates[0]
+        S_xmax, S_ymax = self.bbox_in_frame_coordinates[1]
+        O_xmin, O_ymin = other.bbox_in_frame_coordinates[0]
+        O_xmax, O_ymax = other.bbox_in_frame_coordinates[1]
         if not S_xmax >= O_xmin and O_xmax >= S_xmin:  # x overlap
             return False
         if not S_ymax >= O_ymin and O_ymax >= S_ymin:  # y overlap
             return False
 
         # Check convex hull
         if not cv2.intersectConvexConvex(self.convexHull, other.convexHull)[0]:
@@ -468,15 +468,15 @@
         the default centroid during validation or generated more centroids.
 
         Returns
         -------
         list
             List of tuples (x, y) indicating the centroids of the blob.
         """
-        return list(filter(lambda c: c != (-1, -1), self.all_final_centroids))
+        return (c for c in self.all_final_centroids if c != (-1, -1))
 
     @property
     def all_final_centroids(self):
         if self.user_generated_centroids:
             # Note that sometimes len(user_generated_centroids) >
             # len(assigned_centroids)
             final_centroids = []
@@ -486,15 +486,15 @@
                 else:
                     final_centroids.append(self.assigned_centroids[i])
             return final_centroids
         return self.assigned_centroids
 
     @property
     def final_identities(self):
-        return list(filter(lambda id: id != -1, self.all_final_identities))
+        return (id for id in self.all_final_identities if id != -1)
 
     @property
     def all_final_identities(self):
         """Identities of the blob after the tracking process and after
         potential modifications by the users during the validation procedure.
         """
         if self.user_generated_identities:
@@ -509,15 +509,17 @@
                     final_identities.append(user_generated_identity)
                 else:
                     final_identities.append(self.assigned_identities[i])
             return final_identities
         return self.assigned_identities
 
     @property
-    def final_ids_and_centroids(self):
+    def final_ids_and_centroids(
+        self,
+    ) -> Iterable[tuple[int | None, tuple[float, float]]]:
         return zip(self.final_identities, self.final_centroids)
 
     @property
     def all_final_ids_and_centroids(self):
         return zip(self.all_final_identities, self.all_final_centroids)
 
     def get_image_for_identification(
@@ -651,15 +653,15 @@
                 - self.bbox_in_frame_coordinates[0][0]
                 + 2,  # 2 bbox_image_pads
             ),
             np.uint8,
         )
         return cv2.fillPoly(
             img=base,
-            pts=[self.contour],
+            pts=(self.contour,),
             color=1,
             offset=(
                 -self.bbox_in_frame_coordinates[0][0] + 1,  # bbox_image_pad
                 -self.bbox_in_frame_coordinates[0][1] + 1,  # bbox_image_pad
             ),
         )
 
@@ -691,17 +693,17 @@
         self.user_generated_centroids[index] = new_centroid
         self.user_generated_identities[index] = identity
 
     def init_validator_variables(self):
         if self.user_generated_centroids is None:
             self.user_generated_centroids: list[tuple[float, float] | None] = [
                 None
-            ] * len(self.final_centroids)
+            ] * len(list(self.final_centroids))
         if self.user_generated_identities is None:
-            self.user_generated_identities = [None] * len(self.final_identities)
+            self.user_generated_identities = [None] * len(list(self.final_identities))
 
     def index_and_centroid_closer_to(
         self, centroid: tuple, identity: int | None
     ) -> tuple[int, tuple, float]:
         candidates: list[tuple[int, tuple, float]] = []
         for indx, (_id, _centroid) in enumerate(self.all_final_ids_and_centroids):
             if identity not in (None, _id):
@@ -840,34 +842,34 @@
             first_frame_modified = current.frame_number
 
         return first_frame_modified, last_frame_modified
 
     @property
     def properties(self) -> Sequence[str]:
         return (
-            ("Individual" if self.is_an_individual else "Crossing")
-            + f" Blob ({hex(id(self))})",
+            (
+                (("Individual" if self.is_an_individual else "Crossing") + " Blob")
+                + (" (forced)" if self.forced_crossing else "")
+            ),
             f"{self.contour.shape[0]} vertices in contour of {self.area:.0f} px area",
-            ("Used" if self.used_for_training else "Not used") + " for training",
             f"In fragment {self.fragment_identifier}",
-            f"Linked to {len(self.previous)} previous blobs",
-            f"Linked to {len(self.next)} next blobs",
+            f"Linked to {self.n_previous} previous blobs",
+            f"Linked to {self.n_next} next blobs",
             ("Used" if self.used_for_training_crossings else "Not used")
             + " for training crossings",
-            ("Sure" if self.is_a_sure_individual() else "Not sure") + " individual",
-            ("Sure" if self.is_a_sure_crossing() else "Not sure") + " crossing",
-            "It was " + ("" if self.was_a_crossing else "not ") + "a crossing",
+            f"Seems like individual: {self.seems_like_individual}",
+            f"Pixels are from eroded blob: {self.pixels_are_from_eroded_blob}",
             f"Predicted identity: {self.identity}",
-            f"Id correcting jumps {self.identity_corrected_solving_jumps}",
-            f"Id correcting gaps: {self.identities_corrected_closing_gaps}",
+            f"Corrected solving jumps {self.identity_corrected_solving_jumps}",
+            f"Corrected solving gaps: {self.identities_corrected_closing_gaps}",
             f"assigned identities: {self.assigned_identities}",
             f"assigned centroids: {repr_of_list_of_points(self.assigned_centroids)}",
             f"user identities: {self.user_generated_identities}",
             f"user centroids: {repr_of_list_of_points(self.user_generated_centroids)}",
-            f"final identities: {self.final_identities}",
+            f"final identities: {list(self.final_identities)}",
             f"final centroids: {repr_of_list_of_points(self.final_centroids)}",
         )
 
 
 def repr_of_list_of_points(list_of_points) -> str:
     if list_of_points is None:
         return "None"
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/constants.toml` & `idtrackerai-5.1.4/src/idtrackerai/constants.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossing_detector.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossing_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 
 import torch
-from torch import nn
 from torch.backends import cudnn
+from torch.nn import CrossEntropyLoss
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import Blob, ListOfBlobs, Video
 from idtrackerai.network import (
     LearnerClassification,
     NetworkParams,
     weights_xavier_init,
 )
-from idtrackerai.utils import conf, create_dir
+from idtrackerai.utils import conf
 
 from .dataset.crossings_dataloader import get_training_data_loaders
 from .dataset.crossings_dataset import get_train_validation_and_eval_blobs
 from .model_area import ModelArea
 from .network.predictor_crossing_detector import get_predictions_crossigns
 from .network.stop_training_criteria_crossings import StopTraining
 from .network.trainer_crossing_detector import train_deep_crossing
@@ -65,15 +65,15 @@
     logging.info(
         "Classifying Blobs as individuals or crossings "
         "depending on their area and the number of blobs in the frame"
     )
     for blobs_in_frame in blobs_in_video:
         unicity_cond = len(blobs_in_frame) == number_of_animals
         for blob in blobs_in_frame:
-            blob.is_an_individual = unicity_cond or model_area(blob.area)
+            blob.seems_like_individual = unicity_cond or model_area(blob.area)
 
 
 def detect_crossings(list_of_blobs: ListOfBlobs, video: Video):
     """Classify all blobs in the video as being crossings or individuals.
 
     Parameters
     ----------
@@ -88,23 +88,21 @@
         individuals and crossings images. Otherwise only the model area is applied
 
     Returns
     -------
 
     trainer or list_of_blobs : TrainDeepCrossing or ListOfBlobs()
     """
-
-    create_dir(video.crossings_detector_folder)
-    model_area = ModelArea(list_of_blobs.blobs_in_video, video.number_of_animals)
+    model_area = ModelArea(list_of_blobs, video.number_of_animals)
 
     _apply_area_and_unicity_heuristics(
         list_of_blobs.blobs_in_video, video.number_of_animals, model_area
     )
 
-    (train_blobs, val_blobs, eval_blobs) = get_train_validation_and_eval_blobs(
+    train_blobs, val_blobs, eval_blobs = get_train_validation_and_eval_blobs(
         list_of_blobs.blobs_in_video, video.number_of_animals
     )
 
     if (
         len(train_blobs["crossings"])
         < conf.MINIMUM_NUMBER_OF_CROSSINGS_TO_TRAIN_CROSSING_DETECTOR
     ):
@@ -117,54 +115,56 @@
     logging.info("Setting crossing detector network parameters")
     network_params = NetworkParams(
         number_of_classes=2,
         architecture="DCD",
         save_folder=video.crossings_detector_folder,
         model_name="crossing_detector",
         image_size=video.id_image_size,
-        loss="CE",
         use_gpu=True,
         optimizer="Adam",
         schedule=[30, 60],
         optim_args={"lr": conf.LEARNING_RATE_DCD},
-        apply_mask=False,
-        dataset="supervised",
-        skip_eval=False,
         epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_DCD,
     )
+    network_params.save()
     logging.info("Setting training criterion")
-    criterion = nn.CrossEntropyLoss(weight=torch.tensor(train_blobs["weights"]))
+    criterion = CrossEntropyLoss(weight=torch.tensor(train_blobs["weights"]))
     crossing_detector_model = LearnerClassification.create_model(network_params)
     logging.info("Initialize networks params with Xavier initialization")
     crossing_detector_model.apply(weights_xavier_init)
 
     if network_params.use_gpu:
         torch.cuda.set_device(0)
         logging.info(
             'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
         )
         cudnn.benchmark = True  # make it train faster
         crossing_detector_model = crossing_detector_model.cuda()
         criterion = criterion.cuda()
 
-    logging.info("Setting optimizer")
-    optimizer = torch.optim.__dict__[network_params.optimizer](
-        crossing_detector_model.parameters(), **network_params.optim_args
-    )
+    logging.info(f"Setting {network_params.optimizer} optimizer")
+    if network_params.optimizer == "Adam":
+        optimizer = torch.optim.Adam(
+            crossing_detector_model.parameters(), **network_params.optim_args
+        )
+    elif network_params.optimizer == "SGD":
+        optimizer = torch.optim.SGD(
+            crossing_detector_model.parameters(), **network_params.optim_args
+        )
+    else:
+        raise AttributeError(network_params.optimizer)
+
     logging.info("Setting scheduler")
     scheduler = MultiStepLR(optimizer, milestones=network_params.schedule, gamma=0.1)
-    logging.info("Setting the learner")
+
     learner = LearnerClassification(
         crossing_detector_model, criterion, optimizer, scheduler
     )
-    logging.info("Setting the stopping criteria")
-    # set criteria to stop the training
-    stop_training = StopTraining(
-        check_for_loss_plateau=True, num_epochs=network_params.epochs
-    )
+
+    stop_training = StopTraining(network_params.epochs)
 
     model_diverged, best_model_path = train_deep_crossing(
         learner, train_loader, val_loader, network_params, stop_training
     )
 
     if model_diverged:
         logging.warning(
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/crossings_detection.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/crossings_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         frame i+1.
 
     NOTE: This crossing detector sets the identification images that will be
     used to identify the animals
     """
     video.crossing_detector_timer.start()
 
-    median_body_length = compute_body_length(
-        list_of_blobs.blobs_in_video, video.number_of_animals
-    )
+    median_body_length = compute_body_length(list_of_blobs, video.number_of_animals)
     video.set_id_image_size(median_body_length)
 
     create_dir(video.id_images_folder, remove_existing=True)
 
     list_of_blobs.set_images_for_identification(
         video.episodes,
         video.id_images_file_paths,
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataloader.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,86 +24,73 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
-
 import logging
-import os
-from pathlib import Path
 
 from torch.utils.data import DataLoader
 from torchvision import transforms
 
-from idtrackerai import Blob
-from idtrackerai.crossings_detection.dataset.crossings_dataset import CrossingDataset
-from idtrackerai.network import Normalize
+from idtrackerai.network import normalize
 from idtrackerai.utils import conf
 
-if os.name == "nt":  # windows
-    # Using multipricessing in Windows causes a
-    # recursion limit error difficut to debug
-    num_workers_train = 0
-    num_workers_val = 0
-else:
-    num_workers_train = 4
-    num_workers_val = 4
+from .identification_dataset import IdentificationDataset
+
+num_workers_train = 1
+num_workers_val = 1
 
 
 def get_training_data_loaders(
-    id_images_file_paths: list[Path],
-    train_blobs: dict[str, list[Blob]],
-    val_blobs: dict[str, list[Blob]],
-):
-    logging.info("Creating training and validation data loaders")
-    training_set = CrossingDataset(
-        train_blobs,
-        id_images_file_paths,
+    number_of_animals: int, train_data, val_data
+) -> tuple[DataLoader, DataLoader]:
+    logging.info("Creating training IdentificationDataset")
+    training_set = IdentificationDataset(
+        train_data,
         scope="training",
-        transform=transforms.Compose([transforms.ToTensor(), Normalize()]),
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
     )
     train_loader = DataLoader(
         training_set,
-        batch_size=conf.BATCH_SIZE_DCD,
-        shuffle=False,
+        batch_size=conf.BATCH_SIZE_IDCNN,
+        shuffle=True,
         num_workers=num_workers_train,
+        persistent_workers=num_workers_train > 0,
     )
-    train_loader.num_classes = 2
+    train_loader.num_classes = number_of_animals
     train_loader.image_shape = training_set[0][0].shape
 
-    logging.info("Creating validation CrossingDataset")
-    validation_set = CrossingDataset(
-        val_blobs,
-        id_images_file_paths,
+    logging.info("Creating validation IdentificationDataset")
+    validation_set = IdentificationDataset(
+        val_data,
         scope="validation",
-        transform=transforms.Compose([transforms.ToTensor(), Normalize()]),
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
     )
     val_loader = DataLoader(
         validation_set,
-        batch_size=conf.BATCH_SIZE_PREDICTIONS_DCD,
-        shuffle=False,
+        batch_size=conf.BATCH_SIZE_PREDICTIONS_IDCNN,
         num_workers=num_workers_val,
+        persistent_workers=num_workers_val > 0,
     )
-    val_loader.num_classes = 2
+    val_loader.num_classes = number_of_animals
     val_loader.image_shape = validation_set[0][0].shape
     return train_loader, val_loader
 
 
-def get_test_data_loader(id_images_file_paths: list[Path], test_blobs: list[Blob]):
-    logging.info("Creating test CrossingDataset")
-    test_set = CrossingDataset(
-        test_blobs,
-        id_images_file_paths,
-        scope="test",
-        transform=transforms.Compose([transforms.ToTensor(), Normalize()]),
+def get_test_data_loader(test_data, number_of_classes):
+    logging.debug("Creating test IdentificationDataset")
+    test_set = IdentificationDataset(
+        test_data,
+        scope="predict",
+        transform=transforms.Compose([transforms.ToTensor(), normalize]),
     )
     test_loader = DataLoader(
         test_set,
-        batch_size=conf.BATCH_SIZE_PREDICTIONS_DCD,
-        shuffle=False,
+        batch_size=conf.BATCH_SIZE_PREDICTIONS_IDCNN,
         num_workers=num_workers_val,
+        persistent_workers=num_workers_val > 0,
     )
-    test_loader.num_classes = 2
+    test_loader.num_classes = number_of_classes
     test_loader.image_shape = test_set[0][0].shape
     return test_loader
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/dataset/crossings_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,27 +36,28 @@
 
 from idtrackerai import Blob
 from idtrackerai.tracker.dataset.identification_dataset import duplicate_PCA_images
 from idtrackerai.utils import conf, load_id_images, track
 
 
 class CrossingDataset(VisionDataset):
+    images: np.ndarray
+    labels: np.ndarray
+
     def __init__(
         self,
         blobs_list: list[Blob] | dict[str, list[Blob]],
         id_images_file_paths: list[Path],
         scope,
         transform=None,
     ):
-        super().__init__(blobs_list, transform=transform)
+        super().__init__("", transform=transform)
         self.id_images_file_paths = id_images_file_paths
         self.blobs = blobs_list
         self.scope = scope
-        self.images = None
-        self.labels = None
         self.get_data()
 
     def get_data(self):
         if isinstance(self.blobs, dict):
             logging.info(f"Generating crossing {self.scope} set.")
             crossings_images = self.get_images_indices(image_type="crossings")
             crossing_labels = np.ones(len(crossings_images), int)
@@ -64,32 +65,27 @@
             logging.info(f"Generating single individual {self.scope} set")
             individual_images = self.get_images_indices(image_type="individuals")
             individual_labels = np.zeros(len(individual_images), int)
 
             logging.info("Preparing images and labels")
             images_indices = crossings_images + individual_images
             self.images = load_id_images(self.id_images_file_paths, images_indices)
-            self.images = np.expand_dims(np.asarray(self.images), axis=-1)
+            self.images = np.expand_dims(self.images, axis=-1)
 
             self.labels = np.concatenate([crossing_labels, individual_labels], axis=0)
 
             if self.scope == "training":
                 self.images, self.labels = duplicate_PCA_images(
                     self.images, self.labels
                 )
 
-            np.random.seed(0)
-            permutation = np.random.permutation(len(self.labels))
-            self.images = self.images[permutation]
-            self.labels = self.labels[permutation]
-
         elif isinstance(self.blobs, list):
             images_indices = self.get_images_indices()
             self.images = load_id_images(self.id_images_file_paths, images_indices)
-            self.images = np.expand_dims(np.asarray(self.images), axis=-1)
+            self.images = np.expand_dims(self.images, axis=-1)
             self.labels = np.zeros((self.images.shape[0]))
 
     def get_images_indices(self, image_type: str = "") -> list[tuple[int, int]]:
         if image_type:
             assert isinstance(self.blobs, dict)
             blobs = self.blobs[image_type]
         else:
@@ -127,31 +123,34 @@
     crossings = []
     toassign_blobs = []
     for blobs_in_frame in track(blobs_in_video, "First individual/crossing assignment"):
         in_a_global_fragment_core = len(blobs_in_frame) == number_of_animals
         for blob in blobs_in_frame:
             if in_a_global_fragment_core or blob.is_a_sure_individual():
                 blob.used_for_training_crossings = True
+                blob.is_an_individual = True
                 individuals.append(blob)
             elif blob.is_a_sure_crossing():
                 blob.used_for_training_crossings = True
+                blob.is_an_individual = False
                 crossings.append(blob)
             else:
                 blob.used_for_training_crossings = False
                 toassign_blobs.append(blob)
 
     logging.debug(
         f"{len(individuals)} individual, "
         f"{len(crossings)} crossing and "
         f"{len(toassign_blobs)} unknown blobs in total"
     )
 
     # Shuffle and make crossings and individuals even
-    np.random.shuffle(individuals)
-    np.random.shuffle(crossings)
+    rng = np.random.default_rng()
+    rng.shuffle(individuals)
+    rng.shuffle(crossings)
 
     crossings = crossings[: conf.MAX_IMAGES_PER_CLASS_CROSSING_DETECTOR]
     individuals = individuals[: conf.MAX_IMAGES_PER_CLASS_CROSSING_DETECTOR]
 
     n_blobs_crossings = len(crossings)
     n_blobs_individuals = len(individuals)
     n_individual_blobs_validation = int(n_blobs_individuals * ratio_validation)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/model_area.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/model_area.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 
 import numpy as np
 
-from idtrackerai import Blob
+from idtrackerai import ListOfBlobs
 from idtrackerai.utils import CustomError, conf
 
 
 class ModelArea:
     """Model of the area used to perform a first discrimination between blobs
     representing single individual and multiple touching animals (crossings)
 
@@ -57,33 +57,31 @@
 
     Methods
     -------
     __call__:
       some description
     """
 
-    def __init__(self, blobs_in_video: list[list[Blob]], number_of_animals: int):
+    def __init__(self, list_of_blobs: ListOfBlobs, number_of_animals: int):
         """computes the median and standard deviation of the area of all the blobs
         in the the video and the median of the the diagonal of the bounding box.
         """
         # areas are collected throughout the entire video inthe cores of the
         # global fragments
         logging.info(
             "Initializing ModelArea for individual/crossing blob initial classification"
         )
-        areas = []
         if number_of_animals > 0:
-            for blobs_in_frame in blobs_in_video:
+            areas = []
+            for blobs_in_frame in list_of_blobs.blobs_in_video:
                 if len(blobs_in_frame) == number_of_animals:
                     for blob in blobs_in_frame:
                         areas.append(blob.area)
         else:
-            for blobs_in_frame in blobs_in_video:
-                for blob in blobs_in_frame:
-                    areas.append(blob.area)
+            areas = [b.area for b in list_of_blobs.all_blobs]
         areas = np.asarray(areas)
 
         n_blobs = len(areas)
         if n_blobs == 0:
             raise CustomError(
                 "There is not part in the video where the "
                 f"{number_of_animals} animals are visible. "
@@ -101,28 +99,24 @@
             f"and std = {self.std:.1f} (in pixels)"
         )
 
     def __call__(self, area) -> bool:
         return (area - self.median) < self.tolerance
 
 
-def compute_body_length(
-    blobs_in_video: list[list[Blob]], number_of_animals: int
-) -> float:
+def compute_body_length(list_of_blobs: ListOfBlobs, number_of_animals: int) -> float:
     """computes the median of the the diagonal of the bounding box."""
     # areas are collected throughout the entire video in the cores of
     # the global fragments
-    body_lengths = []
     if number_of_animals > 0:
-        for blobs_in_frame in blobs_in_video:
+        body_lengths = []
+        for blobs_in_frame in list_of_blobs.blobs_in_video:
             if len(blobs_in_frame) == number_of_animals:
                 for blob in blobs_in_frame:
                     body_lengths.append(blob.estimated_body_length)
     else:
-        for blobs_in_frame in blobs_in_video:
-            for blob in blobs_in_frame:
-                body_lengths.append(blob.estimated_body_length)
+        body_lengths = [b.estimated_body_length for b in list_of_blobs.all_blobs]
 
     median = np.median(body_lengths)
     logging.info(f"Median body length: {median} pixels")
     return float(median)
     # return np.percentile(body_lengths, 80)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/predictor_crossing_detector.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import torch
 from torch.nn import Module
 
 from idtrackerai import Blob
 from idtrackerai.crossings_detection.dataset.crossings_dataloader import (
     get_test_data_loader,
 )
+from idtrackerai.utils import track
 
 
 def get_predictions_crossigns(
     id_images_file_paths: list[Path], model: Module, blobs: list[Blob], use_gpu: bool
 ):
     loader = get_test_data_loader(id_images_file_paths, blobs)
     predictions = []
 
     model.eval()
-    for input, _target in loader:
+    for input, _target in track(loader, "Predicting crossings"):
         # Prepare the inputs
         if use_gpu:
             with torch.no_grad():
                 input = input.cuda()
 
         # Inference
         output = model(input)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/stop_training_criteria_crossings.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,49 +35,41 @@
 import numpy as np
 from rich.status import Status
 
 from idtrackerai.utils import conf
 
 
 class StopTraining:
-    """Stops the training of the network according to the conditions specified
+    """CROSSING Stops the training of the network according to the conditions specified
     in __call__
     """
 
-    def __init__(
-        self,
-        epochs_before_checking_stopping_conditions=10,
-        check_for_loss_plateau: bool = True,
-        num_epochs=10,
-    ):
+    number_of_classes = 2
+    epochs_before_checking_stopping_conditions = 10
+
+    def __init__(self, num_epochs: int):
+        logging.info("Setting the stopping criteria", stacklevel=3)
         self.num_epochs = num_epochs  # maximal num of epochs
-        self.number_of_classes = 2
-        self.epochs_before_checking_stopping_conditions = (
-            epochs_before_checking_stopping_conditions
-        )
         self.overfitting_counter: int = 0
         """Number of epochs in which the network is overfitting before
         stopping the training"""
 
-        self.check_for_loss_plateau = check_for_loss_plateau
-        """if true the training is stopped if the loss is not decreasing enough"""
-
         self.epochs_completed = -1
 
     def __call__(
         self,
-        loss_training: list,
+        loss_training: float,
         loss_validation: list,
-        accuracy_validation: list,
+        accuracy_validation: float,
         status: Status,
     ):
         self.epochs_completed += 1
         # check that the model did not diverged (nan loss).
         if self.epochs_completed > 0 and (
-            np.isnan(loss_training[-1]) or np.isnan(loss_validation[-1])
+            np.isnan(loss_training) or np.isnan(loss_validation[-1])
         ):
             status.stop()
             logging.info(
                 "The model diverged with loss NaN, falling back "
                 "to detecting crossings with the model area"
             )
             return True
@@ -107,26 +99,26 @@
                 if self.overfitting_counter >= conf.OVERFITTING_COUNTER_THRESHOLD_DCD:
                     status.stop()
                     logging.info("Overfitting")
                     return True
             else:
                 self.overfitting_counter = 0
             # check if the error is not decreasing much
-            if self.check_for_loss_plateau and np.abs(
+            if np.abs(
                 losses_difference
             ) < conf.LEARNING_PERCENTAGE_DIFFERENCE_2_DCD * 10 ** (
                 int(np.log10(current_loss)) - 1
             ):
                 status.stop()
                 logging.info(
                     "The losses difference is very small, we stop the training"
                 )
                 return True
             # if the individual accuracies in validation are 1. for all the animals
-            if accuracy_validation[-1] == 1.0:
+            if accuracy_validation == 1.0:
                 status.stop()
                 logging.info("The accuracy in validation is 100%, we stop the training")
                 return True
             # if the validation loss is 0.
             if previous_loss == 0.0 or current_loss == 0.0:
                 status.stop()
                 logging.info("The validation loss is 0.0, we stop the training")
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py` & `idtrackerai-5.1.4/src/idtrackerai/crossings_detection/network/trainer_crossing_detector.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,73 +30,49 @@
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 from contextlib import suppress
 from pathlib import Path
 
 import numpy as np
 from rich.console import Console
+from torch.utils.data import DataLoader
 
 from idtrackerai.network import LearnerClassification, NetworkParams, evaluate, train
 
 from .stop_training_criteria_crossings import StopTraining
 
 
 def train_deep_crossing(
     learner: LearnerClassification,
-    train_loader,
-    val_loader,
+    train_loader: DataLoader,
+    val_loader: DataLoader,
     network_params: NetworkParams,
     stop_training: StopTraining,
 ) -> tuple[bool, Path]:
     logging.info("Training Deep Crossing Detector")
 
     # Initialize metric storage
-    train_losses = []
-    if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-        train_losses_CE = []
-        train_losses_MCL = []
-        val_losses_CE = []
-        val_losses_MCL = []
-    train_accs = []
+    train_loss = 0.0
     val_losses = []
-    val_accs = []
+    val_acc = 0.0
 
     logging.debug("Entering the epochs loop...")
     with Console().status("[red]Epochs loop...") as status:
-        while not stop_training(train_losses, val_losses, val_accs, status):
+        while not stop_training(train_loss, val_losses, val_acc, status):
             epoch = stop_training.epochs_completed
-            (loss, loss_CE, loss_MCL), train_acc = train(
-                epoch, train_loader, learner, network_params
-            )
-
-            train_losses.append(loss)
-            if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-                train_losses_CE.append(loss_CE)
-                train_losses_MCL.append(loss_MCL)
-            train_accs.append(train_acc)
-
-            if val_loader is not None and (
-                (not network_params.skip_eval) or (epoch == network_params.epochs - 1)
-            ):
-                loss, loss_CE, loss_MCL, val_acc = evaluate(
-                    val_loader, None, network_params, learner
-                )
-                val_losses.append(loss)
-                if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-                    val_losses_CE.append(loss_CE)
-                    val_losses_MCL.append(loss_MCL)
-                val_accs.append(val_acc)
-            # Save checkpoint at each LR steps and the end of optimization
-            best_model_path = learner.snapshot(
-                network_params.save_folder
-                / f"{network_params.dataset}_{network_params.model_name}"
-            )
+
+            train_loss, train_acc = train(epoch, train_loader, learner, network_params)
+            val_loss, val_acc = evaluate(val_loader, network_params, learner)
+
+            val_losses.append(val_loss)
+
             with suppress(IndexError):
                 status.update(
-                    f"[red]Epochs loop {epoch}: training loss ="
-                    f" {train_losses[-1]:.6f}, validation loss ="
-                    f" {val_losses[-1]:.6f} and accuracy = {val_accs[-1]:.4%}"
+                    f"[red]Epoch {epoch}: training loss ="
+                    f" {train_loss:.6f}, validation loss ="
+                    f" {val_loss:.6f} and accuracy = {val_acc:.4%}"
                 )
 
         logging.info("Last epoch loop: %s", status.status, extra={"markup": True})
 
-    return np.isnan(train_losses[-1]) or np.isnan(val_losses[-1]), best_model_path
+    learner.save_model(network_params.model_path)
+    return np.isnan(train_loss) or np.isnan(val_loss), network_params.model_path
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/data/test_A.avi` & `idtrackerai-5.1.4/src/idtrackerai/data/test_A.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/data/test_B.avi` & `idtrackerai-5.1.4/src/idtrackerai/data/test_B.avi`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/fragment.py` & `idtrackerai-5.1.4/src/idtrackerai/fragment.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
-import sys
-from typing import Sequence
+from typing import Literal, Sequence
 
 import numpy as np
 
 from .utils import conf
 
 
 class Fragment:
@@ -65,16 +64,14 @@
         equivalent image index.
     is_an_individual : bool
         Indicates whether the fragment corresponds to a collection of blobs
         that are all labelled as being an individual.
     is_a_crossing : bool
         Indicates whether the fragment corresponds to a collection of blobs
         that are all labelled as being a crossing.
-    number_of_animals : int
-        Number of animals to be tracked as defined by the user.
     """
 
     acceptable_for_training: bool | None
     """Boolean to indicate that the fragment was identified sufficiently
     well and can in principle be used for training. See also the
     accumulation_manager.py module."""
 
@@ -82,45 +79,42 @@
     """Integer indicating a temporary identity assigned to the fragment
     during the cascade of training and identification protocols."""
 
     is_certain: bool | None = None
     """Boolean indicating whether the fragment is certain enough to be
     accumulated. See also the accumulation_manager.py module."""
 
-    accumulable: bool | None
+    accumulable: bool | None = None
     """Boolean indicating whether the fragment can be accumulated, i.e. it
     can potentially be used for training."""
 
     is_in_a_global_fragment: bool = False
     """Indicates whether the fragment is part of a global fragment"""
 
     P1_vector: np.ndarray
     """Numpy array indicating the P1 probability of each of the possible
     identities"""
 
     certainty: float
     """Indicates the certainty of the identity"""
 
-    certainty_P2: float
-    """Indicating the certainty of the identity following the P2"""
-
-    P2_vector: np.ndarray | None
+    P2_vector: np.ndarray | None = None
     """Numpy array indicating the P2 probability of each of the possible
     identities. See also :meth:`compute_P2_vector`"""
 
     identity: int | None = None
     """Identity assigned to the fragment during the cascade of training
     and identification protocols or during the residual identification
     (see also the assigner.py module)"""
 
-    non_consistent: bool | None
+    non_consistent: bool = False
     """Boolean indicating whether the fragment identity is consistent with
     coexisting fragment"""
 
-    ambiguous_identities: np.ndarray | None
+    ambiguous_identities: np.ndarray | None = None
     """Identities that would be ambiguously assigned during the residual
     identification process. See also the assigner.py module"""
 
     used_for_training: bool = False
     """Boolean indicating whether the images in the fragment were used to
     train the identification network during the cascade of training and
     identification protocols. See also the accumulation_manager.py module.
@@ -161,77 +155,125 @@
     partial accumulation step of the cascade of training and identification
     protocols. See also the accumulation_manager.py module."""
 
     user_generated_identity: int | None = None
     """This property is give during the correction of impossible velocity
     jumps. It has nothing to do with the manual validation."""
 
+    coexisting_individual_fragments: list["Fragment"]
+    """list of fragment objects representing and individual (i.e.
+    not representing a crossing where two or more animals are touching) and
+    coexisting (in frame) with self"""
+
+    forced_crossing: bool = False
+    """Indicates if the crossing attribute has been forced by set_individual_with_identity_0_as_crossings()"""
+
+    frame_by_frame_velocity: np.ndarray
+    """Instant speed (in each frame) of the blob in the fragment"""
+
+    start_position: tuple[float, float]
+    """X and Y position of the blob's centroid at the start of the fragment"""
+
+    end_position: tuple[float, float]
+    """X and Y position of the blob's centroid at the end of the fragment"""
+
     def __init__(
         self,
         fragment_identifier: int,
         start_frame: int,
         end_frame: int,
         images: list[int],
-        centroids: list,
+        centroids: list[tuple[float, float]],
         episodes: list[int],
         is_an_individual: bool,
-        number_of_animals: int,
     ):
         self.identifier = fragment_identifier
         self.start_frame = start_frame
         self.end_frame = end_frame
         self.images = images
-        self.centroids = np.asarray(centroids)
         self.episodes = episodes
         self.is_an_individual = is_an_individual
-        self.number_of_animals = number_of_animals
-        self.distance_travelled = self.set_distance_travelled(self.centroids)
 
-    def reset(self, roll_back_to: str):
+        if len(centroids) > 1:
+            self.frame_by_frame_velocity = np.sqrt(
+                (np.diff(centroids, axis=0) ** 2).sum(axis=1)
+            )
+        else:
+            self.frame_by_frame_velocity = np.array([0])
+
+        self.start_position = centroids[0]
+        self.end_position = centroids[-1]
+
+    @property
+    def image_locations(self):
+        return zip(self.images, self.episodes)
+
+    @classmethod
+    def from_json(cls, json: dict):
+        fragment: cls = cls.__new__(cls)
+        fragment.__dict__ = json
+        if len(fragment.episodes) == 1:  # decompress
+            fragment.episodes = [fragment.episodes[0]] * len(fragment.images)
+        for key in (
+            "P1_vector",
+            "P2_vector",
+            "ambiguous_identities",
+            "frame_by_frame_velocity",
+        ):
+            if key in json:
+                setattr(fragment, key, np.asarray(json[key]))
+        return fragment
+
+    @property
+    def distance_travelled(self) -> float:
+        """The distance traveled by the individual in the fragment.
+        It is based on the position of the centroids in consecutive images.
+        """
+        return np.sum(self.frame_by_frame_velocity)
+
+    def reset(
+        self,
+        roll_back_to: Literal["fragmentation", "accumulation"],
+        number_of_animals: int,
+    ):
         """Reset attributes of the fragment to a specific part of the
         algorithm.
 
         Parameters
         ----------
         roll_back_to : str
             Reset all the attributes up to the process specified in input.
             'fragmentation', 'pretraining', 'accumulation', 'assignment'
         """
         #  This method was mainly used to resume the tracking from different
         # rocessing steps. Currently this function is not active, but this
         #  method might still be useful in the future.
-        if roll_back_to in ("fragmentation", "pretraining"):
+        self.identity_is_fixed = False
+        if roll_back_to == "fragmentation":
             self.used_for_training = False
-            if roll_back_to == "fragmentation":
-                self.used_for_pretraining = False
+            self.used_for_pretraining = False
             self.acceptable_for_training = None
             self.temporary_id = None
             self.identity = None
             self.identity_corrected_solving_jumps = None
-            self.identity_is_fixed = False
             self.accumulated_globally = False
             self.accumulated_partially = False
             self.accumulation_step = None
             self.is_certain = None
-            self.non_consistent = None
+            self.non_consistent = False
             self.certainty = 0.0
-            self.P1_vector = np.zeros(self.number_of_animals)
+            self.P1_vector = np.zeros(number_of_animals)
             self.P1_below_random = None
         elif roll_back_to == "accumulation":
-            self.identity_is_fixed = False
             if not self.used_for_training:
                 self.identity = None
                 self.identity_corrected_solving_jumps = None
-                self.P1_vector = np.zeros(self.number_of_animals)
+                self.P1_vector = np.zeros(number_of_animals)
             self.ambiguous_identities = None
-            self.certainty_P2 = 0.0
             self.P2_vector = None
-        elif roll_back_to == "assignment":
-            self.user_generated_identity = None
-            self.identity_corrected_solving_jumps = None
         else:
             raise ValueError(roll_back_to)
 
     @property
     def is_a_crossing(self) -> bool:
         return not self.is_an_individual
 
@@ -266,36 +308,14 @@
             sum(
                 fragment.used_for_training
                 for fragment in self.coexisting_individual_fragments
             )
             >= self.number_of_coexisting_individual_fragments / 2
         )
 
-    @staticmethod
-    def set_distance_travelled(centroids: np.ndarray | None) -> float:
-        """Computes the distance traveled by the individual in the fragment.
-        It is based on the position of the centroids in consecutive images. See
-        :attr:`blob.Blob.centroid`.
-
-        """
-        if centroids is not None and centroids.shape[0] > 1:
-            return np.sqrt((np.diff(centroids, axis=0) ** 2).sum(axis=1)).sum()
-        return 0.0
-
-    def frame_by_frame_velocity(self) -> np.ndarray:
-        """Instant speed (in each frame) of the blob in the fragment.
-
-        Returns
-        -------
-        ndarray
-            Frame by frame speed of the individual in the fragment
-
-        """
-        return np.sqrt((np.diff(self.centroids, axis=0) ** 2).sum(axis=1))
-
     def compute_border_velocity(self, other: "Fragment") -> float:
         """Velocity necessary to cover the space between two fragments.
 
         Note that these velocities are divided by the number of frames that
         separate self and other fragment.
 
         Parameters
@@ -307,17 +327,17 @@
         -------
         float
             Returns the speed at which an individual should travel to be
             present in both self and other fragments.
 
         """
         if self.start_frame > other.end_frame:
-            centroids = np.asarray([self.centroids[0], other.centroids[-1]])
+            centroids = np.asarray([self.start_position, other.end_position])
         else:
-            centroids = np.asarray([self.centroids[-1], other.centroids[0]])
+            centroids = np.asarray([self.end_position, other.start_position])
         return np.sqrt((np.diff(centroids, axis=0) ** 2).sum(axis=1))[0]
 
     def coexist_with(self, other: "Fragment"):
         """Boolean indicating whether the given fragment coexists in time with
         another fragment.
 
         Parameters
@@ -329,33 +349,14 @@
         -------
         bool
             True if self and other coexist in time in at least one frame.
 
         """
         return self.start_frame < other.end_frame and self.end_frame > other.start_frame
 
-    def get_coexisting_individual_fragments_indices(self, fragments: list["Fragment"]):
-        """Get the list of fragment objects representing and individual (i.e.
-        not representing a crossing where two or more animals are touching) and
-        coexisting (in frame) with self
-
-        Parameters
-        ----------
-        fragments : list
-            List of all the fragments in the video
-
-        """
-        self.coexisting_individual_fragments = [
-            fragment
-            for fragment in fragments
-            if fragment.is_an_individual
-            and self.coexist_with(fragment)
-            and fragment is not self
-        ]
-
     @property
     def number_of_coexisting_individual_fragments(self):
         return len(self.coexisting_individual_fragments)
 
     def check_consistency_with_coexistent_individual_fragments(self, temporary_id):
         """Check that the temporary identity assigned to the fragment is
         consistent with respect to the identities already assigned to the
@@ -375,15 +376,15 @@
         """
         return all(
             coexisting_fragment.temporary_id != temporary_id
             for coexisting_fragment in self.coexisting_individual_fragments
         )
 
     def compute_identification_statistics(
-        self, predictions: np.ndarray | list, softmax_probs, number_of_animals=None
+        self, predictions: np.ndarray | list, softmax_probs, number_of_animals: int
     ):
         """Computes the statistics necessary for the identification of the
         fragment.
 
         Parameters
         ----------
         predictions : numpy array
@@ -394,23 +395,20 @@
             whose rows are the result of applying the softmax function to the
             predictions outputted by the idCNN per image
         number_of_animals : int
             Description of parameter `number_of_animals`.
 
         See Also
         --------
-        :meth:`set_P1_from_frequencies`
         :meth:`compute_median_softmax`
         :meth:`compute_certainty_of_individual_fragment`
         """
         assert self.is_an_individual
-        number_of_animals = (
-            self.number_of_animals if number_of_animals is None else number_of_animals
-        )
-        self.set_P1_from_frequencies(
+
+        self.P1_vector = self.compute_P1_from_frequencies(
             np.bincount(predictions, minlength=number_of_animals + 1)[1:]
         )
         median_softmax = self.compute_median_softmax(softmax_probs, number_of_animals)
         self.certainty = self.compute_certainty_of_individual_fragment(
             self.P1_vector, median_softmax
         )
 
@@ -424,87 +422,85 @@
         self.P1_vector[self.temporary_id] = 1.0
 
     @staticmethod
     def get_possible_identities(P2_vector):
         """Returns the possible identities by the argmax of the P2 vector and
         the value of the maximum.
         """
-        max = np.max(P2_vector)
+        max = np.max(P2_vector)  # there can be two equal maximums
         return np.argwhere(P2_vector == max)[:, 0] + 1, max
 
-    def assign_identity(self):
+    def assign_identity(self, number_of_animals: int):
         """Assigns the identity to the fragment by considering the fragments
         coexisting with it.
 
         If the certainty of the identification is high enough it sets
         the identity of the fragment as fixed and it won't be modified during
         the postprocessing.
         """
         assert self.is_an_individual
-        if self.used_for_training and not self.identity_is_fixed:
+        if self.identity_is_fixed:
+            return
+        if self.used_for_training:
             self.identity_is_fixed = True
-        elif not self.identity_is_fixed:
-            possible_identities, max_P2 = self.get_possible_identities(self.P2_vector)
-            if len(possible_identities) > 1:  # TODO is it possible?
-                self.identity = 0
-                self.zero_identity_assigned_by_P2 = True
-                self.ambiguous_identities = possible_identities
-            else:
-                if max_P2 > conf.FIXED_IDENTITY_THRESHOLD:
-                    self.identity_is_fixed = True
-                self.identity = possible_identities[0]
-                self.P1_vector = np.zeros(len(self.P1_vector))
-                self.P1_vector[self.identity - 1] = 1.0
-                self.recompute_P2_of_coexisting_fragments()
-
-    def recompute_P2_of_coexisting_fragments(self):
-        """Updates the P2 of the fragments coexisting with self
-        (see :attr:`coexisting_individual_fragments`) if their identity is not
-        fixed (see :attr:`identity_is_fixed`)
-        """
-        # The P2 of fragments with fixed identity won't be recomputed
-        # due to the condition in assign_identity() (second line)
-        for fragment in self.coexisting_individual_fragments:
-            fragment.compute_P2_vector()
+            return
+
+        possible_identities, max_P2 = self.get_possible_identities(self.P2_vector)
+        if len(possible_identities) > 1:  # TODO is it possible?
+            self.identity = 0
+            self.zero_identity_assigned_by_P2 = True
+            self.ambiguous_identities = possible_identities
+        else:
+            if max_P2 > conf.FIXED_IDENTITY_THRESHOLD:
+                self.identity_is_fixed = True
+            self.identity = possible_identities[0]
+            self.P1_vector = np.zeros(len(self.P1_vector))
+            self.P1_vector[self.identity - 1] = 1.0
+            for fragment in self.coexisting_individual_fragments:
+                fragment.compute_P2_vector(number_of_animals)
 
-    def compute_P2_vector(self):
+    def compute_P2_vector(self, number_of_animals: int):
         """Computes the P2_vector of the fragment.
 
         It is based on :attr:`coexisting_individual_fragments`"""
         coexisting_P1_vectors = np.asarray(
             [fragment.P1_vector for fragment in self.coexisting_individual_fragments]
         )
-        numerator = np.asarray(self.P1_vector) * np.prod(
-            1.0 - coexisting_P1_vectors, axis=0
-        )
+        numerator = self.P1_vector * np.prod(1.0 - coexisting_P1_vectors, axis=0)
         denominator = numerator.sum()
         if denominator != 0:
             self.P2_vector = numerator / denominator
-            P2_vector_ordered = np.sort(self.P2_vector)
-            P2_first_max = P2_vector_ordered[-1]
-            P2_second_max = P2_vector_ordered[-2]
-            self.certainty_P2 = (
-                sys.float_info[0]
-                if P2_second_max == 0
-                else P2_first_max / P2_second_max
-            )
         else:
-            self.P2_vector = np.zeros(self.number_of_animals)
-            self.certainty_P2 = 0.0
+            self.P2_vector = np.zeros(number_of_animals)
 
-    def set_P1_from_frequencies(self, frequencies: np.ndarray):
+    @property
+    def certainty_P2(self) -> float:
+        """Indicating the certainty of the identity following the P2"""
+
+        if self.P2_vector is None or self.P2_vector.sum() < 0.001:
+            return 0.0
+
+        P2_vector_ordered = np.sort(self.P2_vector)
+        P2_first_max = P2_vector_ordered[-1]
+        P2_second_max = P2_vector_ordered[-2]
+
+        with np.errstate(divide="ignore"):
+            return P2_first_max / P2_second_max
+
+    @staticmethod
+    def compute_P1_from_frequencies(frequencies: np.ndarray):
         """Given the frequencies of a individual fragment
         computer the P1 vector.
 
         P1 is the softmax of the frequencies with base 2 for each identity.
         Numpy array indicating the number of images assigned with each of
         the possible identities
         """
         with np.errstate(over="ignore"):
-            self.P1_vector = 1.0 / (
+            return 1.0 / (
                 2.0
                 ** (
                     np.tile(frequencies, (len(frequencies), 1)).T
                     - np.tile(frequencies, (len(frequencies), 1))
                 )
             ).sum(axis=0)
 
@@ -537,15 +533,17 @@
         argmax_softmax_probs = np.argmax(softmax_probs, axis=1)
         softmax_median = np.zeros(number_of_animals)
         for i in np.unique(argmax_softmax_probs):
             softmax_median[i] = np.median(max_softmax_probs[argmax_softmax_probs == i])
         return softmax_median
 
     @staticmethod
-    def compute_certainty_of_individual_fragment(P1_vector: np.ndarray, median_softmax):
+    def compute_certainty_of_individual_fragment(
+        P1_vector: np.ndarray, median_softmax
+    ) -> float:
         """Computes the certainty given the P1_vector of the fragment by
         using the output of :meth:`compute_median_softmax`
 
         Parameters
         ----------
         P1_vector : numpy array
             Array with shape [1, number_of_animals] computed from frequencies
@@ -637,28 +635,35 @@
         if accumulation_strategy == "global":
             self.accumulated_globally = True
         elif accumulation_strategy == "partial":
             self.accumulated_partially = True
 
     @property
     def properties(self) -> Sequence[str]:
+        max_p1 = np.argmax(self.P1_vector)
         return (
             f"Fragment {self.identifier}",
-            f"Frames from {self.start_frame} to {self.end_frame}",
-            ("Individual" if self.is_an_individual else "Crossing") + " fragment",
+            (
+                f"Frames from {self.start_frame} to {self.end_frame} (length"
+                f" {self.end_frame-self.start_frame})"
+            ),
+            ("Individual" if self.is_an_individual else "Crossing")
+            + " fragment"
+            + (" (forced)" if self.forced_crossing else ""),
             ("Used" if self.used_for_training else "Not used") + " for training",
             ("Used" if self.used_for_pretraining else "Not used") + " for pretraining",
             ("Acceptable" if self.acceptable_for_training else "Not acceptable")
             + " for training",
-            f"{self.temporary_id}",
-            f"{self.identity}",
-            f"{self.identity_corrected_solving_jumps}",
-            f"{self.identity_is_fixed}",
-            f"{self.accumulated_globally}",
-            f"{self.accumulated_partially}",
-            f"{self.accumulation_step}",
-            f"{self.is_certain}",
+            f"Predicted identity: {self.identity}",
+            f"Corrected solving jumps: {self.identity_corrected_solving_jumps}",
+            f"Corrected solving gaps: {self.identities_corrected_closing_gaps}",
+            f"Fixed identity: {self.identity_is_fixed}",
+            f"Globally accumulated: {self.accumulated_globally}",
+            f"Partially accumulated: {self.accumulated_partially}",
+            f"Accumulable: {self.accumulable}",
+            f"Accumulated at step {self.accumulation_step}",
+            f"Is certain: {self.is_certain}",
             "Non consistent" if self.non_consistent else "Consistent",
+            f"Max P1 {max_p1+1} with value {self.P1_vector[max_p1]}",
             f"Certainty: {self.certainty}",
-            f"P1 vector: {self.P1_vector}",
             f"P1 below random: {self.P1_below_random}",
         )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/fragmentation/fragmentation.py` & `idtrackerai-5.1.4/src/idtrackerai/fragmentation/fragmentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,19 +34,14 @@
 from idtrackerai.utils import track
 
 
 def fragmentation_API(
     video: Video, list_of_blobs: ListOfBlobs
 ) -> tuple[ListOfFragments, ListOfGlobalFragments]:
     video.fragmentation_timer.start()
-    if video.single_animal:
-        # If there is only one animal there is no need to compute fragments
-        # as the trajectories are obtained directly from the list_of_blobs
-        video.fragmentation_timer.finish()
-        return ListOfFragments([], []), ListOfGlobalFragments([])
 
     compute_fragment_identifier_and_blob_index(
         list_of_blobs.blobs_in_video,
         max(video.number_of_animals, list_of_blobs.maximum_number_of_blobs),
     )
 
     list_of_fragments = ListOfFragments.from_fragmented_blobs(
@@ -54,26 +49,23 @@
     )
     logging.info(
         f"{list_of_fragments.number_of_fragments} Fragments in total, "
         f"{list_of_fragments.number_of_individual_fragments} individuals and "
         f"{list_of_fragments.number_of_crossing_fragments} crossings"
     )
 
-    if not video.track_wo_identities:
-        list_of_global_fragments = ListOfGlobalFragments.from_fragments(
-            list_of_blobs.blobs_in_video,
-            list_of_fragments.fragments,
-            video.number_of_animals,
-        )
-        list_of_fragments.manage_accumulable_non_accumulable_fragments(
-            list_of_global_fragments.global_fragments,
-            list_of_global_fragments.non_accumulable_global_fragments,
-        )
-    else:
-        list_of_global_fragments = ListOfGlobalFragments([])
+    list_of_global_fragments = ListOfGlobalFragments.from_fragments(
+        list_of_blobs.blobs_in_video,
+        list_of_fragments.fragments,
+        video.number_of_animals,
+    )
+    list_of_fragments.manage_accumulable_non_accumulable_fragments(
+        list_of_global_fragments.global_fragments,
+        list_of_global_fragments.non_accumulable_global_fragments,
+    )
 
     video.fragmentation_timer.finish()
     return list_of_fragments, list_of_global_fragments
 
 
 def compute_fragment_identifier_and_blob_index(
     blobs_in_video: list[list[Blob]], number_of_animals: int
@@ -88,39 +80,38 @@
     number_of_animals : int
         Number of animals to be tracked as defined by the user
     """
     frame_id = 0
     possible_blob_indices = set(range(number_of_animals))
 
     for blobs_in_frame in track(blobs_in_video, "Fragmenting blobs"):
-        used_blob_indices = [
-            blob.blob_index for blob in blobs_in_frame if blob.blob_index is not None
-        ]
-        missing_blob_indices = possible_blob_indices.difference(set(used_blob_indices))
+        missing_blob_indices = possible_blob_indices.difference(
+            blob.blob_index for blob in blobs_in_frame
+        )
 
         for blob in blobs_in_frame:
             if blob.fragment_identifier != -1:
                 continue
 
             blob.fragment_identifier = frame_id
             if blob.is_an_individual:
                 blob_index = missing_blob_indices.pop()
                 blob.blob_index = blob_index
                 while (
-                    len(blob.next) == 1
-                    and len(blob.next[0].previous) == 1
+                    blob.n_next == 1
+                    and blob.next[0].n_previous == 1
                     and blob.next[0].is_an_individual
                 ):
                     blob = blob.next[0]
                     blob.fragment_identifier = frame_id
                     blob.blob_index = blob_index
 
             elif blob.is_a_crossing:
                 while (
-                    len(blob.next) == 1
-                    and len(blob.next[0].previous) == 1
+                    blob.n_next == 1
+                    and blob.next[0].n_previous == 1
                     and blob.next[0].is_a_crossing
                 ):
                     blob = blob.next[0]
                     blob.fragment_identifier = frame_id
 
             frame_id += 1
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/globalfragment.py` & `idtrackerai-5.1.4/src/idtrackerai/globalfragment.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import numpy as np
 
 from . import Blob, Fragment
-from .utils import conf, load_id_images
+from .utils import load_id_images
 
 
 class GlobalFragment:
     """Representes a collection of :class:`fragment.Fragment` N different
     animals. Where N is the number of animals in the video as defined by the
     user.
 
@@ -53,69 +53,77 @@
         Number of animals to be tracked as defined by the user.
     """
 
     accumulation_step: int | None = None
     """Integer indicating the accumulation step at which the fragment was
     accumulated. See also the accumulation_manager.py module."""
 
+    duplicated_identities: set
+    first_frame_of_the_core: int
+    individual_fragments_identifiers: list[int]
+    individual_fragments: list[Fragment]
+    minimum_distance_travelled: float
+
     def __init__(
         self,
         blobs_in_video: list[list[Blob]],
         fragments: list[Fragment],
         first_frame_of_the_core: int,
-        number_of_animals: int,
     ):
         self.first_frame_of_the_core = first_frame_of_the_core
-        self.number_of_animals = number_of_animals
-        self.individual_fragments_identifiers: list[int] = [
+        self.individual_fragments_identifiers = [
             blob.fragment_identifier for blob in blobs_in_video[first_frame_of_the_core]
         ]
         self.set_individual_fragments(fragments)
 
-        number_of_images_per_individual_fragment: list[int] = []
         distance_travelled_per_individual_fragment: list[float] = []
 
         for fragment in self.individual_fragments:
-            assert fragment.is_an_individual
             fragment.is_in_a_global_fragment = True
-            number_of_images_per_individual_fragment.append(fragment.number_of_images)
             distance_travelled_per_individual_fragment.append(
                 fragment.distance_travelled
             )
 
         self.minimum_distance_travelled = min(
             distance_travelled_per_individual_fragment
         )
 
-        self.candidate_for_accumulation: bool = (
-            min(number_of_images_per_individual_fragment)
-            > conf.MINIMUM_NUMBER_OF_FRAMES_TO_BE_A_CANDIDATE_FOR_ACCUMULATION
-        )
         """Boolean indicating whether the global fragment is a candidate
         for accumulation in the cascade of training and identification
         protocols.
         """
 
-        # Initializes some attributes that will be used in other processes
-        # during the cascade of training and identification protocols
-        self._init_attributes()
+    @property
+    def min_n_images_per_fragment(self):
+        return min(fragment.number_of_images for fragment in self.individual_fragments)
+
+    @classmethod
+    def from_json(cls, data: dict, fragments: list[Fragment] | None):
+        global_fragment = cls.__new__(cls)
+        global_fragment.__dict__.update(data)
+        if "duplicated_identities" in data:
+            global_fragment.duplicated_identities = set(data["duplicated_identities"])
+
+        if fragments is not None:
+            global_fragment.set_individual_fragments(fragments)
+
+        return global_fragment
 
     @property
     def used_for_training(self):
         """Boolean indicating if all the fragments in the global fragment
         have been used for training the identification network"""
         return all(fragment.used_for_training for fragment in self.individual_fragments)
 
-    @property
-    def is_unique(self):
+    def is_unique(self, number_of_animals: int):
         """Boolean indicating that the global fragment has unique
         identities, i.e. it does not have duplications."""
         return (
             len(
-                set(range(self.number_of_animals))
+                set(range(number_of_animals))
                 - {fragment.temporary_id for fragment in self.individual_fragments}
             )
             == 0
         )
 
     @property
     def is_partially_unique(self):
@@ -130,31 +138,14 @@
         self.duplicated_identities = {
             x
             for x in identities_acceptable_for_training
             if identities_acceptable_for_training.count(x) > 1
         }
         return len(self.duplicated_identities) == 0
 
-    def _init_attributes(self):
-        """Initializes some attributes required for the cascade of
-        training and identification protocols"""
-        self.predictions = []
-
-    def reset(self, roll_back_to):
-        """Resets attributes to the fragmentation step in the algorithm,
-        allowing for example to start a new accumulation.
-
-        Parameters
-        ----------
-        roll_back_to : str
-            "fragmentation"
-        """
-        if roll_back_to == "fragmentation":
-            self._init_attributes()
-
     def set_individual_fragments(self, fragments: list[Fragment]):
         """Gets the list of instances of the class :class:`fragment.Fragment`
         that constitute the global fragment and sets an attribute with such
         list.
 
         Parameters
         ----------
@@ -223,11 +214,11 @@
         Tuple
             Tuple with two Numpy arrays with the images and their labels.
         """
         images = []
         labels = []
 
         for temporary_id, fragment in enumerate(self.individual_fragments):
-            images.extend(list(zip(fragment.images, fragment.episodes)))
+            images.extend(fragment.image_locations)
             labels.extend([temporary_id] * fragment.number_of_images)
 
         return load_id_images(id_images_file_paths, images), np.asarray(labels)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py` & `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py` & `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_groundtruth_statistics_general.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py` & `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/compute_individual_groundtruth_statistics.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_groundtruth.py` & `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py` & `idtrackerai-5.1.4/src/idtrackerai/groundtruth_utils/generate_individual_groundtruth.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/list_of_blobs.py` & `idtrackerai-5.1.4/src/idtrackerai/list_of_blobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from pathlib import Path
 from typing import Optional
 
 import h5py
 import numpy as np
 
 from . import Blob
-from .utils import Episode, conf, resolve_path, track
+from .utils import Episode, clean_attrs, conf, resolve_path, track
 
 
 class ListOfBlobs:
     """Contains all the instances of the class :class:`~blob.Blob` for all
     frames in the video.
 
     Notes
@@ -129,14 +129,18 @@
         path_to_save : str, optional
             Path where to save the object, by default None
         """
         path = resolve_path(path)
         logging.info(f"Saving ListOfBlobs at {path}")
         path.parent.mkdir(exist_ok=True)
         self.disconnect()
+
+        for blob in self.all_blobs:
+            clean_attrs(blob)
+
         with open(path, "wb") as file:
             pickle.dump(self, file, protocol=pickle.HIGHEST_PROTOCOL)
         self.reconnect()
 
     @classmethod
     def load(cls, path: Path | str) -> "ListOfBlobs":
         """Loads an instance of a class saved in a .npy file.
@@ -172,29 +176,23 @@
         logging.info("Loading from v4 file: %s", path)
         list_of_blobs: "ListOfBlobs" = np.load(path, allow_pickle=True).item()
 
         for blob in track(
             list_of_blobs.all_blobs, "Updating objects from an old idtracker.ai version"
         ):
             blob.is_an_individual = blob._is_an_individual  # type:ignore
-            blob.identity_corrected_solving_jumps = (
-                blob._identity_corrected_solving_jumps  # type:ignore
-            )
             blob.fragment_identifier = blob._fragment_identifier  # type:ignore
             blob.blob_index = blob._blob_index  # type:ignore
-            blob.used_for_training = blob._used_for_training  # type:ignore
             blob.identity = blob._identity  # type:ignore
             blob.identity_corrected_solving_jumps = (
                 blob._identity_corrected_solving_jumps  # type:ignore
             )
             blob.identities_corrected_closing_gaps = (
                 blob._identities_corrected_closing_gaps  # type:ignore
             )
-            if hasattr(blob, "_P2_vector"):
-                blob.P2_vector = blob._P2_vector  # type:ignore
         return list_of_blobs
 
     def disconnect(self):
         if self.blobs_are_connected:
             for blob in self.all_blobs:
                 blob.next.clear()
 
@@ -261,15 +259,15 @@
                     blobs_in_episode
                 )
 
     @staticmethod
     def set_id_images_per_episode(
         inputs: tuple[Path, int, Path, Episode, list[list[Blob]]]
     ) -> tuple[list[list[Blob]], Episode]:
-        (bbox_imgs_path, id_image_size, file_path, episode, blobs_in_episode) = inputs
+        bbox_imgs_path, id_image_size, file_path, episode, blobs_in_episode = inputs
 
         imgs_to_save = np.empty(
             (sum(map(len, blobs_in_episode)), id_image_size, id_image_size), np.uint8
         )
 
         for index, blob in enumerate(itertools.chain.from_iterable(blobs_in_episode)):
             imgs_to_save[index] = blob.get_image_for_identification(
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/list_of_fragments.py` & `idtrackerai-5.1.4/src/idtrackerai/list_of_fragments.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,87 +24,101 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
+import json
 import logging
 import pickle
+from itertools import combinations
+from math import comb
 from pathlib import Path
-from typing import Any, Iterable
+from typing import Any, Iterable, Literal
 
 import h5py
 import numpy as np
 
 from . import Blob, Fragment, GlobalFragment
-from .utils import load_id_images, resolve_path, track
+from .utils import clean_attrs, load_id_images, resolve_path, track
 
 
 class ListOfFragments:
     """Contains all the instances of the class :class:`fragment.Fragment`.
 
     Parameters
     ----------
     fragments : list
         List of instances of the class :class:`fragment.Fragment`.
     id_images_file_paths : list
         List of strings with the paths to the files where the identification
         images are stored.
     """
 
-    def __init__(self, fragments: list[Fragment], id_images_file_paths: list[Path]):
+    accumulable_individual_fragments: set[int]
+    not_accumulable_individual_fragments: set[int]
+
+    def __init__(
+        self,
+        fragments: list[Fragment],
+        id_images_file_paths: list[Path],
+        number_of_animals: int,
+    ):
         # Assert fragments are sorted
         for i, fragment in enumerate(fragments):
             assert i == fragment.identifier
-
+        self.number_of_animals = number_of_animals
         self.fragments = fragments
         self.id_images_file_paths = id_images_file_paths
         self.connect_coexisting_fragments()
 
     @property
     def number_of_fragments(self):
         return len(self.fragments)
 
+    @property
+    def individual_fragments(self):
+        return (frag for frag in self.fragments if frag.is_an_individual)
+
     # TODO: if the resume feature is not active, this does not make sense|
-    def reset(self, roll_back_to):
+    def reset(self, roll_back_to: Literal["fragmentation", "accumulation"]):
         """Resets all the fragment to a given processing step.
 
         Parameters
         ----------
         roll_back_to : str
             Name of the step at which the fragments should be reset.
             It can be 'fragmentation', 'pretraining', 'accumulation' or
             'assignment'
 
         See Also
         --------
         :meth:`fragment.Fragment.reset`
         """
-        logging.info(f"Resetting ListOfFragments to '{roll_back_to}'")
+        logging.info(f"Resetting ListOfFragments to '{roll_back_to}'", stacklevel=3)
         for fragment in self.fragments:
-            fragment.reset(roll_back_to)
+            fragment.reset(roll_back_to, self.number_of_animals)
 
     # TODO: maybe this should go to the accumulator manager
     def get_images_from_fragments_to_assign(self):
         """Take all the fragments that have not been used to train the idCNN
         and that are associated with an individual, and concatenates their
         images in order to feed them to the identification network.
 
         Returns
         -------
         ndarray
             [number_of_images, height, width, number_of_channels]
         """
-        images_lists = [
-            list(zip(fragment.images, fragment.episodes))
-            for fragment in self.fragments
-            if not fragment.used_for_training and fragment.is_an_individual
-        ]
-        images = [image for images in images_lists for image in images]
+        images: list[tuple[int, int]] = []
+        for fragment in self.individual_fragments:
+            if not fragment.used_for_training:
+                images.extend(fragment.image_locations)
+
         logging.info(
             f"Number of images to identify non-accumulated fragments: {len(images)}"
         )
         return load_id_images(self.id_images_file_paths, images)
 
     # TODO: The following methods could be properties.
     # TODO: The following methods depend on the identification strategy.
@@ -176,17 +190,16 @@
             / self.number_of_images_in_global_fragments
         )
 
     def compute_P2_vectors(self):
         """Computes the P2_vector associated to every individual fragment. See
         :meth:`fragment.Fragment.compute_P2_vector`
         """
-        for fragment in self.fragments:
-            if fragment.is_an_individual:
-                fragment.compute_P2_vector()
+        for fragment in self.individual_fragments:
+            fragment.compute_P2_vector(self.number_of_animals)
 
     def get_number_of_unidentified_individual_fragments(self):
         """Returns the number of individual fragments that have not been
         identified during the fingerprint protocols cascade
 
         Returns
         -------
@@ -206,21 +219,20 @@
         Returns
         -------
         :class:`fragment.Fragment`
             An instance of the class :class:`fragment.Fragment`
         """
         try:
             return max(
-                (
-                    fragment
-                    for fragment in self.fragments
-                    if fragment.is_an_individual
-                    and fragment.assigned_identities[0] is None
+                filter(
+                    lambda frag: frag.is_an_individual
+                    and frag.assigned_identities[0] is None,
+                    self.fragments,
                 ),
-                key=lambda x: x.certainty_P2,
+                key=lambda frag: frag.certainty_P2,
             )
         except ValueError:
             return None
 
     def update_id_images_dataset(self):
         """Updates the identification images files with the identity assigned
         to each fragment during the tracking process.
@@ -230,26 +242,26 @@
         identities = []
         for path in self.id_images_file_paths:
             with h5py.File(path, "r") as file:
                 identities.append(np.full(file["id_images"].shape[0], 0))  # type: ignore
 
         for fragment in self.fragments:
             if fragment.used_for_training:
-                for image, episode in zip(fragment.images, fragment.episodes):
+                for image, episode in fragment.image_locations:
                     identities[episode][image] = fragment.identity
 
         for path, identities_in_episode in zip(self.id_images_file_paths, identities):
             with h5py.File(path, "r+") as file:
                 dataset = file.require_dataset(
                     "identities", shape=len(identities_in_episode), dtype=int
                 )
                 dataset[:] = identities_in_episode
 
     def get_ordered_list_of_fragments(
-        self, scope: str, first_frame_first_global_fragment: int
+        self, scope: str, specific_frame: int
     ) -> list[Fragment]:
         """Sorts the fragments starting from the frame number
         `first_frame_first_global_fragment`. According to `scope` the sorting
         is done either "to the future" of "to the past" with respect to
         `first_frame_first_global_fragment`
 
         Parameters
@@ -264,94 +276,106 @@
         Returns
         -------
         list
             list of sorted fragments
 
         """
         if scope == "to_the_past":
-            fragments_subset = [
-                fragment
-                for fragment in self.fragments
-                if fragment.end_frame <= first_frame_first_global_fragment
-            ]
-            fragments_subset.sort(key=lambda x: x.end_frame, reverse=True)
+            fragments_to_the_past = filter(
+                lambda frag: frag.end_frame <= specific_frame, self.fragments
+            )
+            return sorted(
+                fragments_to_the_past, key=lambda x: x.end_frame, reverse=True
+            )
         elif scope == "to_the_future":
-            fragments_subset = [
-                fragment
-                for fragment in self.fragments
-                if fragment.start_frame >= first_frame_first_global_fragment
-            ]
-            fragments_subset.sort(key=lambda x: x.start_frame, reverse=False)
+            fragments_to_the_future = filter(
+                lambda frag: frag.start_frame >= specific_frame, self.fragments
+            )
+            return sorted(fragments_to_the_future, key=lambda x: x.start_frame)
         else:
             raise ValueError(scope)
-        return fragments_subset
 
     def save(self, path: Path | str):
         """Save an instance of the object in disk,
 
         Parameters
         ----------
         fragments_path : str
             Path where the instance of the object will be stored.
         """
         path = resolve_path(path)
         logging.info(f"Saving ListOfFragments as {path}")
         path.parent.mkdir(exist_ok=True)
 
-        # Avoid recursion when saving object on disk
-        for fragment in self.fragments:
-            fragment.coexisting_individual_fragments.clear()
-
-        with open(path, "wb") as file:
-            pickle.dump(self, file, protocol=pickle.HIGHEST_PROTOCOL)
+        json.dump(self, path.open("w"), cls=FragmentsEncoder, indent=4)
 
-        self.connect_coexisting_fragments()
-
-    @staticmethod
-    def load(path: Path | str) -> "ListOfFragments":
+    @classmethod
+    def load(cls, path: Path | str, reconnect=True) -> "ListOfFragments":
         """Loads a previously saved (see :meth:`save`) from the path
         `path_to_load`
         """
         path = resolve_path(path)
         logging.info(f"Loading ListOfFragments from {path}")
-        with open(path, "rb") as file:
-            list_of_fragments: "ListOfFragments" = pickle.load(file)
 
-        list_of_fragments.connect_coexisting_fragments()
+        if not path.is_file() and path.with_suffix(".pickle").is_file():
+            # <=5.1.3 compatibility
+            pickle.load(path.with_suffix(".pickle").open("rb")).save(path)
+
+        list_of_fragments = cls.__new__(cls)
+        json_data = json.load(path.with_suffix(".json").open("r"))
+
+        list_of_fragments.accumulable_individual_fragments = set(
+            json_data.get("accumulable_individual_fragments", [])
+        )
+        list_of_fragments.not_accumulable_individual_fragments = set(
+            json_data.get("not_accumulable_individual_fragments", [])
+        )
+        if "number_of_animals" in json_data:
+            list_of_fragments.number_of_animals = json_data["number_of_animals"]
+        list_of_fragments.id_images_file_paths = list(
+            map(Path, json_data["id_images_file_paths"])
+        )
+
+        list_of_fragments.fragments = [
+            Fragment.from_json(frag_data) for frag_data in json_data["fragments"]
+        ]
+
+        for fragment in list_of_fragments.fragments:
+            if (
+                fragment.identifier
+                in list_of_fragments.accumulable_individual_fragments
+            ):
+                fragment.accumulable = True
+            elif (
+                fragment.identifier
+                in list_of_fragments.not_accumulable_individual_fragments
+            ):
+                fragment.accumulable = False
+
+        if reconnect:
+            list_of_fragments.connect_coexisting_fragments()
 
         return list_of_fragments
 
     def connect_coexisting_fragments(self):
         logging.info("Connecting coexisting individual fragments")
         # Make it N (not N²) with, maybe, sets (not lists)
-        for fragment in track(self.fragments, "Connecting coexisting fragments"):
-            fragment.get_coexisting_individual_fragments_indices(self.fragments)
-
-    def get_new_images_and_labels_for_training(self):
-        """Extract images and creates labels from every individual fragment
-        that has not been used to train the network during the fingerprint
-        protocols cascade.
-
-        Returns
-        -------
-        list
-            List of numpy arrays with shape [width, height, num channels]
-        list
-            labels
-        """
-        images = []
-        labels = []
         for fragment in self.fragments:
-            if fragment.acceptable_for_training and not fragment.used_for_training:
-                assert fragment.is_an_individual
-                images.extend(list(zip(fragment.images, fragment.episodes)))
-                labels.extend([fragment.temporary_id] * fragment.number_of_images)
-        if len(images) != 0:
-            return np.asarray(images), np.asarray(labels)
-        return None, None
+            fragment.coexisting_individual_fragments = []
+
+        for fragment_A, fragment_B in track(
+            combinations(self.fragments, 2),
+            "Connecting coexisting fragments",
+            comb(len(self.fragments), 2),
+        ):
+            if fragment_A.coexist_with(fragment_B):
+                if fragment_A.is_an_individual:
+                    fragment_B.coexisting_individual_fragments.append(fragment_A)
+                if fragment_B.is_an_individual:
+                    fragment_A.coexisting_individual_fragments.append(fragment_B)
 
     def manage_accumulable_non_accumulable_fragments(
         self,
         accumulable_global_fragments: list[GlobalFragment],
         non_accumulable_global_fragments: list[GlobalFragment],
     ):
         """Gets the unique identifiers associated to individual fragments that
@@ -377,30 +401,28 @@
         } - self.accumulable_individual_fragments
 
         for fragment in self.fragments:
             if fragment.identifier in self.accumulable_individual_fragments:
                 fragment.accumulable = True
             elif fragment.identifier in self.not_accumulable_individual_fragments:
                 fragment.accumulable = False
-            else:
-                fragment.accumulable = None
 
     @property
     def number_of_crossing_fragments(self) -> int:
         return sum(fragment.is_a_crossing for fragment in self.fragments)
 
     @property
     def number_of_individual_fragments(self) -> int:
-        return sum(fragment.is_an_individual for fragment in self.fragments)
+        return sum(1 for _ in self.individual_fragments)
 
     @property
     def number_of_individual_fragments_not_in_a_glob_fragment(self) -> int:
         return sum(
-            not fragment.is_in_a_global_fragment and fragment.is_an_individual
-            for fragment in self.fragments
+            not fragment.is_in_a_global_fragment
+            for fragment in self.individual_fragments
         )
 
     @property
     def number_of_accumulable_individual_fragments(self) -> int:
         return len(self.accumulable_individual_fragments)
 
     @property
@@ -416,47 +438,41 @@
         return sum(
             fragment.is_a_crossing * fragment.number_of_images
             for fragment in self.fragments
         )
 
     @property
     def number_of_individual_blobs(self) -> int:
-        return sum(
-            fragment.is_an_individual * fragment.number_of_images
-            for fragment in self.fragments
-        )
+        return sum(fragment.number_of_images for fragment in self.individual_fragments)
 
     @property
     def number_of_individual_blobs_not_in_a_global_fragment(self) -> int:
         return sum(
-            (not fragment.is_in_a_global_fragment and fragment.is_an_individual)
-            * fragment.number_of_images
-            for fragment in self.fragments
+            not fragment.is_in_a_global_fragment * fragment.number_of_images
+            for fragment in self.individual_fragments
         )
 
     @property
     def fragments_not_accumulated(self) -> set[int]:
         return self.accumulable_individual_fragments & {
             fragment.identifier
             for fragment in self.fragments
             if not fragment.used_for_training
         }
 
     @property
     def number_of_globally_accumulated_individual_fragments(self) -> int:
         return sum(
-            fragment.accumulated_globally and fragment.is_an_individual
-            for fragment in self.fragments
+            fragment.accumulated_globally for fragment in self.individual_fragments
         )
 
     @property
     def number_of_partially_accumulated_individual_fragments(self) -> int:
         return sum(
-            fragment.accumulated_partially and fragment.is_an_individual
-            for fragment in self.fragments
+            fragment.accumulated_partially for fragment in self.individual_fragments
         )
 
     @property
     def number_of_accumulable_individual_blobs(self) -> int:
         return sum(
             bool(fragment.accumulable) * fragment.number_of_images
             for fragment in self.fragments
@@ -469,25 +485,23 @@
             for fragment in self.fragments
             if fragment.accumulable is not None
         )
 
     @property
     def number_of_globally_accumulated_individual_blobs(self) -> int:
         return sum(
-            (bool(fragment.accumulated_globally) and fragment.is_an_individual)
-            * fragment.number_of_images
-            for fragment in self.fragments
+            fragment.accumulated_globally * fragment.number_of_images
+            for fragment in self.individual_fragments
         )
 
     @property
     def number_of_partially_accumulated_individual_blobs(self) -> int:
         return sum(
-            (bool(fragment.accumulated_partially) and fragment.is_an_individual)
-            * fragment.number_of_images
-            for fragment in self.fragments
+            fragment.accumulated_partially * fragment.number_of_images
+            for fragment in self.individual_fragments
         )
 
     def get_stats(self) -> dict[str, Any]:
         """Collects the following counters from the fragments.
 
         * number_of_fragments
         * number_of_crossing_fragments
@@ -593,15 +607,15 @@
                 images = [blob.id_image_index]
                 centroids = [blob.centroid]
                 episodes = [blob.episode]
                 start = blob.frame_number
                 current = blob
 
                 while (
-                    len(current.next) > 0
+                    current.n_next > 0
                     and current.next[0].fragment_identifier
                     == current_fragment_identifier
                 ):
                     current = current.next[0]
                     images.append(current.id_image_index)
                     centroids.append(current.centroid)
                     episodes.append(current.episode)
@@ -612,19 +626,18 @@
                     current_fragment_identifier,
                     start,
                     end + 1,  # it is not inclusive
                     images,
                     centroids,
                     episodes,
                     blob.is_an_individual,
-                    number_of_animals,
                 )
                 used_fragment_identifiers.add(current_fragment_identifier)
                 fragments.append(fragment)
-        return cls(fragments, id_images_file_paths)
+        return cls(fragments, id_images_file_paths, number_of_animals)
 
     def update_blobs(self, all_blobs: Iterable[Blob]):
         """Updates the blobs objects generated from the video with the
         attributes computed for each fragment
 
         Parameters
         ----------
@@ -636,15 +649,77 @@
         :meth:`blob.Blob.compute_fragment_identifier_and_blob_index`
 
         """
         logging.info("Updating list of blobs from list of fragments")
         for blob in all_blobs:
             fragment = self.fragments[blob.fragment_identifier]
             blob.identity = fragment.identity
-            blob.used_for_training = fragment.used_for_training
-            blob.accumulation_step = fragment.accumulation_step
             blob.identity_corrected_solving_jumps = (
                 fragment.identity_corrected_solving_jumps
             )
-            blob.P2_vector = fragment.P2_vector
             blob.user_generated_identity = fragment.user_generated_identity
             blob.is_an_individual = fragment.is_an_individual
+            if fragment.forced_crossing:
+                blob.forced_crossing = True
+
+
+class FragmentsEncoder(json.JSONEncoder):
+    def default(self, obj):
+        match obj:
+            case Path():
+                return str(obj)
+
+            case ListOfFragments():
+                serial = obj.__dict__.copy()
+                serial["accumulable_individual_fragments"] = (
+                    f"NotString{json.dumps(list(serial.get('accumulable_individual_fragments',{})))}"
+                )
+                serial["not_accumulable_individual_fragments"] = (
+                    f"NotString{json.dumps(list(serial.get('not_accumulable_individual_fragments',{})))}"
+                )
+                return serial
+
+            case Fragment():
+                clean_attrs(obj)
+                serial = obj.__dict__.copy()
+                serial.pop("coexisting_individual_fragments", None)
+                serial.pop("centroids", None)  # v5.1.3 compatibility
+                serial.pop("accumulable", None)
+                serial["images"] = "NotString" + json.dumps(obj.images)
+                if len(set(obj.episodes)) == 1:
+                    # compress when all images are in the same episode
+                    serial["episodes"] = f"NotString{[obj.episodes[0]]}"
+                else:
+                    serial["episodes"] = "NotString" + json.dumps(obj.episodes)
+                if "frame_by_frame_velocity" in serial:
+                    serial["frame_by_frame_velocity"] = "NotString" + json.dumps(
+                        np.round(obj.frame_by_frame_velocity, 2).tolist()
+                    )
+                if "start_position" in serial:
+                    serial["start_position"] = "NotString" + json.dumps(
+                        np.round(obj.start_position, 2).tolist()
+                    )
+                if "end_position" in serial:
+                    serial["end_position"] = "NotString" + json.dumps(
+                        np.round(obj.end_position, 2).tolist()
+                    )
+                for key in ("P1_vector", "P2_vector", "ambiguous_identities"):
+                    if key in serial:
+                        serial[key] = "NotString" + json.dumps(serial[key].tolist())
+
+                return serial
+            case np.integer():
+                return int(obj)
+            case np.bool_():
+                return bool(obj)
+            case np.floating():
+                return float(obj)
+            case _:
+                return super().default(obj)
+
+    def iterencode(self, obj, **kwargs):
+        for encoded in super().iterencode(obj, **kwargs):
+            if encoded.startswith('"NotString'):
+                # remove first and final '"NoIndent..."' and remove indents,
+                yield encoded[10:-1]
+            else:
+                yield encoded
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/list_of_global_fragments.py` & `idtrackerai-5.1.4/src/idtrackerai/list_of_global_fragments.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
+import json
 import logging
 import pickle
-from itertools import chain
 from pathlib import Path
 
+import numpy as np
+
 from . import Blob, Fragment, GlobalFragment
-from .utils import resolve_path
+from .utils import conf, resolve_path
 
 
 class ListOfGlobalFragments:
     """Contains a list of instances of the class
     :class:`global_fragment.GlobalFragment`.
 
     It contains methods to retrieve information from these global fragments
@@ -48,32 +50,34 @@
 
     Parameters
     ----------
     global_fragments : list
         List of instances of :class:`global_fragment.GlobalFragment`.
     """
 
-    accumulation_step: int | None = None
-    """Integer indicating the accumulation step at which the fragment was
-    accumulated. See also the accumulation_manager.py module."""
+    non_accumulable_global_fragments: list[GlobalFragment]
+    """List of global fragments which are NOT candidate for accumulation"""
+
+    global_fragments: list[GlobalFragment]
+    """List of global fragments which are candidate for accumulation"""
+
+    first_global_fragment_for_accumulation: GlobalFragment
 
     def __init__(self, global_fragments: list[GlobalFragment]):
-        self.non_accumulable_global_fragments: list[GlobalFragment] = [
-            global_fragment
-            for global_fragment in global_fragments
-            if not global_fragment.candidate_for_accumulation
-        ]
-        """List of global fragments which are NOT candidate for accumulation"""
+        self.global_fragments = []
+        self.non_accumulable_global_fragments = []
 
-        self.global_fragments: list[GlobalFragment] = [
-            global_fragment
-            for global_fragment in global_fragments
-            if global_fragment.candidate_for_accumulation
-        ]
-        """List of global fragments which are candidate for accumulation"""
+        for global_fragment in global_fragments:
+            if (
+                global_fragment.min_n_images_per_fragment
+                > conf.MINIMUM_NUMBER_OF_FRAMES_TO_BE_A_CANDIDATE_FOR_ACCUMULATION
+            ):
+                self.global_fragments.append(global_fragment)
+            else:
+                self.non_accumulable_global_fragments.append(global_fragment)
 
     @classmethod
     def from_fragments(
         cls,
         blobs_in_video: list[list[Blob]],
         fragments: list[Fragment],
         num_animals: int,
@@ -93,52 +97,44 @@
 
         Returns
         -------
         list
             list of instances of the class :class:`~globalfragment.GlobalFragment`
 
         """
-        global_fragments_boolean_array = check_global_fragments(
-            blobs_in_video, num_animals
-        )
+        global_fragments_boolean_array = [
+            is_global_fragment_core(blobs_in_frame, blobs_in_video[i - 1], num_animals)
+            for i, blobs_in_frame in enumerate(blobs_in_video)
+        ]
+
         indices_beginning_of_fragment = detect_global_fragments_core_first_frame(
             global_fragments_boolean_array
         )
 
         global_fragments = [
-            GlobalFragment(blobs_in_video, fragments, i, num_animals)
+            GlobalFragment(blobs_in_video, fragments, i)
             for i in indices_beginning_of_fragment
         ]
         logging.info(f"Total number of global_fragments: {len(global_fragments)}")
         return cls(global_fragments)
 
     @property
     def number_of_global_fragments(self) -> int:
         return len(self.global_fragments)
 
     @property
     def single_global_fragment(self) -> bool:
         return self.number_of_global_fragments == 1
 
-    def reset(self, roll_back_to=None):
-        """Resets all the global fragment by calling recursively the method
-        :meth:`globalfragment.GlobalFragment.reset`.
-        """
-        logging.info(f"Resetting ListOfGlobalFragments to '{roll_back_to}'")
-        for global_fragment in self.global_fragments:
-            global_fragment.reset(roll_back_to)
-
     def order_by_distance_travelled(self):
         """Sorts the global fragments by the minimum distance travelled.
         See :attr:`global_fragment.GlobalFragment.minimum_distance_travelled`
         """
-        self.global_fragments = sorted(
-            self.global_fragments,
-            key=lambda x: x.minimum_distance_travelled,
-            reverse=True,
+        self.global_fragments.sort(
+            key=lambda x: x.minimum_distance_travelled, reverse=True
         )
 
     def set_first_global_fragment_for_accumulation(
         self, accumulation_trial: int
     ) -> GlobalFragment | None:
         """Sets the first global fragment that will be used during the
         accumulation in the cascade of training and identification protocols.
@@ -168,14 +164,15 @@
 
         Returns
         -------
         int
             A unique identifier of the global fragment that will be used as the
             first global fragment for training.
         """
+        logging.info("Setting #%d global fragment for accumulation", accumulation_trial)
         self.order_by_distance_travelled()
 
         try:
             self.first_global_fragment_for_accumulation = self.global_fragments[
                 accumulation_trial
             ]
         except IndexError:  # TODO what happens with this exception
@@ -193,71 +190,42 @@
         ----------
         video : :class:`video.Video`
             Instance of the class :class:`video.Video`.
         accumulation_trial : int
             accumulation number (protocol 2 performs a single accumulation
             attempt, and if used, protocol 3 will perform 3 other attempts)
         """
-        self.global_fragments = sorted(
-            self.global_fragments,
+        self.global_fragments.sort(
             key=lambda x: abs(
                 x.first_frame_of_the_core
                 - first_frame_first_global_fragment[accumulation_trial]
-            ),
-            reverse=False,
+            )
         )
 
-    def relink_fragments_to_global_fragments(self, fragments: list[Fragment]):
-        """Re-assigns the instances of :class:`fragment.Fragment` to each
-        global fragment in the list of `global_fragments`.
-
-        Parameters
-        ----------
-        fragments: list
-            List of instances of the class :class:`fragment.Fragment`.
-        """
-        for global_fragment in self.global_fragments:
-            global_fragment.set_individual_fragments(fragments)
-        for global_fragment in self.non_accumulable_global_fragments:
-            global_fragment.set_individual_fragments(fragments)
-
     def save(self, path: Path | str):
         """Saves an instance of the class.
 
         Before saving the instances of fragments associated to every global
         fragment are removed and reset them after saving. This
         prevents problems when pickling objects inside of objects.
 
         Parameters
         ----------
         global_fragments_path : str
             Path where the object will be stored
         """
         path = resolve_path(path)
         logging.info(f"Saving ListOfGlobalFragments at {path}")
-        tmp_fragments = []
-        for global_fragment in chain(
-            self.global_fragments, self.non_accumulable_global_fragments
-        ):
-            tmp_fragments.append(global_fragment.individual_fragments)
-            global_fragment.individual_fragments = []
-
         path.parent.mkdir(exist_ok=True)
-        with open(path, "wb") as file:
-            pickle.dump(self, file, protocol=pickle.HIGHEST_PROTOCOL)
 
-        for fragments, global_fragment in zip(
-            tmp_fragments,
-            chain(self.global_fragments, self.non_accumulable_global_fragments),
-        ):
-            global_fragment.individual_fragments = fragments
+        json.dump(self.__dict__, path.open("w"), cls=GlobalFragmentsEncoder, indent=4)
 
-    @staticmethod
+    @classmethod
     def load(
-        path: Path | str, fragments: list[Fragment] | None = None
+        cls, path: Path | str, fragments: list[Fragment] | None = None
     ) -> "ListOfGlobalFragments":
         """Loads an instance of the class saved with :meth:`save` and
         associates individual fragments to each global fragment by calling
         :meth:`~relink_fragments_to_global_fragments`
 
         Parameters
         ----------
@@ -266,19 +234,39 @@
             Path where the object to be loaded is stored.
         fragments : list
             List of all the instances of the class :class:`fragment.Fragment`
             in the video.
         """
         path = resolve_path(path)
         logging.info(f"Loading ListOfGlobalFragments from {path}")
-        with open(path, "rb") as file:
-            list_of_global_fragments: ListOfGlobalFragments = pickle.load(file)
 
-        if fragments is not None:
-            list_of_global_fragments.relink_fragments_to_global_fragments(fragments)
+        if not path.is_file():  # <=5.1.3 compatibility
+            if not path.with_suffix(".pickle").is_file():
+                raise FileNotFoundError(path)
+            pickle.load(path.with_suffix(".pickle").open("rb")).save(path)
+
+        list_of_global_fragments = cls.__new__(cls)
+        json_data = json.load(path.open("r"))
+
+        list_of_global_fragments.global_fragments = [
+            GlobalFragment.from_json(g_frag_data, fragments)
+            for g_frag_data in json_data["global_fragments"]
+        ]
+
+        list_of_global_fragments.non_accumulable_global_fragments = [
+            GlobalFragment.from_json(g_frag_data, fragments)
+            for g_frag_data in json_data["non_accumulable_global_fragments"]
+        ]
+
+        if "first_global_fragment_for_accumulation" in json_data:
+            list_of_global_fragments.first_global_fragment_for_accumulation = (
+                GlobalFragment.from_json(
+                    json_data["first_global_fragment_for_accumulation"], fragments
+                )
+            )
         return list_of_global_fragments
 
 
 def detect_global_fragments_core_first_frame(boolean_array: list[bool]) -> list[int]:
     """Detects the frame where the core of a global fragment starts.
 
     A core of a global fragment is the part of the global fragment where all
@@ -289,54 +277,57 @@
     """
     if all(boolean_array):
         return [0]
     return [
         i
         for i in range(len(boolean_array))
         if (boolean_array[i] and not boolean_array[i - 1])
-    ]
+    ]  # boolean_array[0] is always False
 
 
-def check_global_fragments(
-    blobs_in_video: list[list[Blob]], num_animals: int
-) -> list[bool]:
-    """Returns list of booleans indicating the frames where all animals are
-    visible.
+def is_global_fragment_core(
+    blobs_in_frame: list[Blob], blobs_in_frame_past: list[Blob], n_animals: int
+) -> bool:
+    """Return True if the set of fragments identifiers in the current frame
+    is the same as in the previous frame, otherwise returns false
+    """
+    all_in_frame = len(blobs_in_frame) == n_animals
 
-    The element of the array is True if.
+    same_fragment_identifiers = {b.fragment_identifier for b in blobs_in_frame} == {
+        b.fragment_identifier for b in blobs_in_frame_past
+    }
+    not_all_were_in_frame = len(blobs_in_frame_past) != n_animals
+    return all_in_frame and (same_fragment_identifiers or not_all_were_in_frame)
 
-    * each blob has a unique blob intersecting in the past and future.
-    * number of blobs equals num_animals.
 
-    Parameters
-    ----------
-    blobs_in_video : list
-        List of lists of instances of the class :class:`blob.Blob`.
+class GlobalFragmentsEncoder(json.JSONEncoder):
+    """Json encoder to serialize Global Fragments with styled indentation"""
 
-    Returns
-    -------
-    list
-        List of booleans with length the number of frames in the video. An
-        element is True if all the animals are visible in the frame.
-    """
+    def default(self, obj):
+        if isinstance(obj, set):
+            return list(obj)
 
-    def _same_fragment_identifier(
-        blobs_in_frame: list[Blob], blobs_in_frame_past: list[Blob]
-    ) -> bool:
-        """Return True if the set of fragments identifiers in the current frame
-        is the same as in the previous frame, otherwise returns false
-        """
-        same_fragment_identifier = {b.fragment_identifier for b in blobs_in_frame} == {
-            b.fragment_identifier for b in blobs_in_frame_past
-        }
-        condition_2 = (
-            all(b.is_an_individual for b in blobs_in_frame_past)
-            and len(blobs_in_frame_past) == num_animals
-        )
-        return same_fragment_identifier or not condition_2
+        if isinstance(obj, GlobalFragment):
+            serial = obj.__dict__.copy()
+            serial.pop("individual_fragments", None)  # remove connections
 
-    return [
-        all(b.is_an_individual for b in blobs_in_frame)
-        and len(blobs_in_frame) == num_animals
-        and _same_fragment_identifier(blobs_in_frame, blobs_in_video[i - 1])
-        for i, blobs_in_frame in enumerate(blobs_in_video)
-    ]
+            serial["individual_fragments_identifiers"] = (  # without indentation
+                f"NotString{json.dumps(obj.individual_fragments_identifiers)}"
+            )
+
+            return serial
+
+        if isinstance(obj, np.integer):
+            return int(obj)
+
+        if isinstance(obj, np.floating):
+            return float(obj)
+
+        return super().default(obj)
+
+    def iterencode(self, obj, **kwargs):
+        for encoded in super().iterencode(obj, **kwargs):
+            if encoded.startswith('"NotString'):
+                # remove colons and "NotString"
+                yield encoded[10:-1]
+            else:
+                yield encoded
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/network/learners.py` & `idtrackerai-5.1.4/src/idtrackerai/network/learners.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """This file provides the template Learner. The Learner is used in training/evaluation loop
 The Learner implements the training procedure for specific task.
 The default Learner is from classification task."""
 import logging
 from pathlib import Path
 
 import torch
-from torch import nn
+from torch.nn import CrossEntropyLoss, Module
+from torch.optim import Optimizer
+from torch.optim.lr_scheduler import MultiStepLR
 
 from . import NetworkParams, models
 
 
-class LearnerClassification(nn.Module):
-    def __init__(self, model: nn.Module, criterion, optimizer, scheduler):
+class LearnerClassification(Module):
+    def __init__(
+        self,
+        model: Module,
+        criterion: CrossEntropyLoss,
+        optimizer: Optimizer,
+        scheduler: MultiStepLR,
+    ):
         super().__init__()
+        logging.info("Setting the learner")
         self.model = model
         self.criterion = criterion
         self.optimizer = optimizer
         self.scheduler = scheduler
-        self.epoch = 0
-        self.model_path = None
+        self.epoch: int = 0
 
     @staticmethod
-    def create_model(learner_params: NetworkParams) -> nn.Module:
+    def create_model(learner_params: NetworkParams) -> Module:
         logging.info("Creating model")
         if learner_params.architecture == "DCD":
             model = models.DCD
         elif learner_params.architecture == "idCNN":
             model = models.idCNN
         elif learner_params.architecture == "idCNN_adaptive":
             model = models.idCNN_adaptive
@@ -34,69 +42,51 @@
 
         return model(
             out_dim=learner_params.number_of_classes,
             input_shape=learner_params.image_size,
         )
 
     @classmethod
-    def load_model(cls, learner_params: NetworkParams, scope=""):
+    def load_model(
+        cls, learner_params: NetworkParams, knowledge_transfer: bool = False
+    ):
         model = cls.create_model(learner_params)
-        if scope == "knowledge_transfer":
+        if knowledge_transfer:
             model_path = learner_params.knowledge_transfer_model_file
+            assert model_path is not None
         else:
             model_path = learner_params.load_model_path
-        assert model_path is not None
 
         logging.info("Load model weights from %s", model_path)
         # The path to model file (*.best_model.pth). Do NOT use checkpoint file here
         # model_state = torch.load(
         #     model_path, map_location=lambda storage, loc: storage
         # )  # Load to CPU as the default!
-        model_state = torch.load(model_path)
+        model_state: dict = torch.load(model_path)
+        model_state.pop("val_acc", None)
         # The pretrained state dict doesn't need to fit the model
         model.load_state_dict(model_state, strict=True)
         return model
 
     def forward(self, x):
         return self.model.forward(x)
 
-    def forward_with_criterion(self, inputs, targets, **kwargs):
+    def forward_with_criterion(self, inputs, targets):
         out = self.forward(inputs)
         targets = targets.long()
         return self.criterion(out, targets), out
 
-    def learn(self, inputs, targets, **kwargs):
+    def learn(self, inputs, targets):
         with torch.autograd.set_detect_anomaly(True):
-            loss, out = self.forward_with_criterion(inputs, targets, **kwargs)
+            loss, out = self.forward_with_criterion(inputs, targets)
             self.optimizer.zero_grad()
             loss.backward()
             self.optimizer.step()
         return loss, out
 
     def step_schedule(self, epoch):
         self.epoch = epoch
         self.scheduler.step()
-        # for param_group in self.optimizer.param_groups:
-        # print("LR:", param_group["lr"])
 
-    def save_model(self, savename: Path):
-        model_state = self.model.state_dict()
-        if isinstance(self.model, torch.nn.DataParallel):
-            # Get rid of 'module' before the name of states
-            model_state = self.model.module.state_dict()
-        for key in model_state.keys():  # Always save it to cpu
-            model_state[key] = model_state[key].cpu()
-        self.model_path = savename.parent / (savename.name + ".pth")
-        torch.save(model_state, self.model_path)
-
-    def snapshot(self, savename: Path) -> Path:
-        model_state = self.model.state_dict()
-        optim_state = self.optimizer.state_dict()
-        checkpoint = {
-            "epoch": self.epoch,
-            "model": model_state,
-            "optimizer": optim_state,
-        }
-        torch.save(checkpoint, savename.parent / (savename.name + ".checkpoint.pth"))
-        self.save_model(savename.parent / (savename.name + ".model"))
-        assert self.model_path is not None
-        return self.model_path
+    def save_model(self, savename: Path, **extra_data):
+        logging.info("Saving model at %s", savename)
+        torch.save(self.model.state_dict() | extra_data, savename)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/network/models.py` & `idtrackerai-5.1.4/src/idtrackerai/network/models.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/network/network_params.py` & `idtrackerai-5.1.4/src/idtrackerai/network/network_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,60 +3,61 @@
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import Optional
 
 from idtrackerai.utils import create_dir, json_default
 
 
-@dataclass
+@dataclass(slots=True)
 class NetworkParams:
     number_of_classes: int
     schedule: list[int]
     architecture: str
     model_name: str
-    dataset: str
     image_size: list[int]
     optim_args: dict = field(default_factory=dict)
     epochs: int = 0
     optimizer: str = "SGD"
     loss: str = "CE"
     use_gpu: bool = True
-    apply_mask: bool = False
-    skip_eval: bool = False
     save_folder: Path = Path("")
-
     scopes_layers_to_optimize: Optional[list[str]] = field(default_factory=list)
     knowledge_transfer_folder: Path | None = None
     use_adam_optimiser: bool = False
     return_store_objects: bool = False
     restore_folder: Path = Path()
 
     @property
     def load_model_path(self) -> Path:
         # v5.0.0 compatibility
-        v5_path = self.restore_folder / (self.model_file_name + "_.model.pth")
-        if v5_path.is_file():
-            return v5_path
-        return self.restore_folder / (self.model_file_name + ".model.pth")
+        for deprecated_name in (
+            self.model_name + "_.model.pth",
+            "supervised_" + self.model_name + ".model.pth",
+            "supervised_" + self.model_name + "_.model.pth",
+        ):
+            path = self.restore_folder / deprecated_name
+            if path.is_file():
+                return path
+
+        return self.restore_folder / (self.model_name + ".model.pth")
 
     @property
-    def save_model_path(self) -> Path:
-        return self.save_folder / self.model_file_name
+    def model_path(self) -> Path:
+        return (self.save_folder / self.model_name).with_suffix(".model.pth")
 
     @property
-    def model_file_name(self) -> str:
-        return f"{self.dataset}_{self.model_name}"
+    def penultimate_model_path(self) -> Path:
+        return (self.save_folder / (self.model_name + "_penultimate")).with_suffix(
+            ".model.pth"
+        )
 
     @property
     def knowledge_transfer_model_file(self) -> Path | None:
         if self.knowledge_transfer_folder is None:
             return None
-        return (
-            self.knowledge_transfer_folder
-            / "supervised_identification_network.model.pth"
-        )
+        return self.knowledge_transfer_folder / "identification_network.model.pth"
 
     def save(self) -> None:
         path = self.save_folder / "model_params.json"
         logging.info(f"Saving NetworkParams at {path}")
         create_dir(self.save_folder)
-        path.write_text(json.dumps(asdict(self), indent=4, default=json_default))
+        json.dump(asdict(self), path.open("w"), indent=4, default=json_default)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/network/train.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_to_csv.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,93 +24,93 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
-
-from statistics import fmean
+import json
+import logging
+from argparse import ArgumentParser
+from pathlib import Path
 
 import numpy as np
-import torch
-
-from .utils import Confusion, prepare_task_target
 
+from idtrackerai.utils import create_dir, wrap_exceptions
 
-def train(epoch, train_loader, learner, network_params):
-    """Trains trains a network using a learner, a given train_loader and a set of network_params
 
-    :param epoch: current epoch
-    :param train_loader: dataloader
-    :param learner: learner from learner.py
-    :param network_params: networks params from networks_params.py
-    :return: losses (tuple) and accuracy
-    """
-
-    # Initialize all meters
-    losses = []
-    if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-        losses_CE = []
-        losses_MCL = []
-    confusion = Confusion(network_params.number_of_classes)
-
-    # Setup learner's configuration
-    learner.train()
-
-    # The optimization loop
-    for input_, target in train_loader:
-        # mask
-        mask = None
-        if network_params.apply_mask:
-            mask = torch.from_numpy(~np.eye(len(target), dtype=bool))
-        # Prepare the inputs
-        if network_params.use_gpu:
-            input_ = input_.cuda()
-            target = target.cuda()
-            if mask is not None:
-                mask = mask.cuda()
-        train_target, eval_target = prepare_task_target(
-            target, network_params, mask=mask
+def save_array_to_csv(path: Path, array: np.ndarray, key: str):
+    array = np.squeeze(array)
+    if key == "id_probabilities":
+        fmt = "%.3e"
+    elif key == "trajectories":
+        fmt = "%.3f"
+    else:
+        fmt = "%.3f"
+
+    if array.ndim == 3:
+        array_header = ",".join(
+            coord + str(i) for i in range(1, array.shape[1] + 1) for coord in ("x", "y")
         )
-
-        # Optimization
-        if "weighted" in network_params.loss:
-            loss, output = learner.learn(
-                input_, train_target, w_MCL=network_params.w_MCL, mask=mask
-            )
-        else:
-            loss, output = learner.learn(input_, train_target, mask=mask)
-
-        with torch.no_grad():
-            # Update the performance meter
-            if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-                confusion.add(output[0], eval_target)
+        array = array.reshape((-1, array.shape[1] * array.shape[2]))
+    elif array.ndim == 2:
+        array_header = ",".join(f"{key}{i}" for i in range(1, array.shape[1] + 1))
+    else:
+        raise ValueError(array.shape)
+    np.savetxt(path, array, delimiter=",", header=array_header, fmt=fmt, comments="")
+
+
+def convert_trajectories_file_to_csv_and_json(npy_path: Path):
+    logging.info(f"Converting {npy_path} to .csv and .json")
+    output_dir = npy_path.with_suffix("")
+    create_dir(output_dir, remove_existing=True)
+    try:
+        trajectories_dict: dict = np.load(npy_path, allow_pickle=True).item()
+        attributes_dict = {}
+        for key, value in trajectories_dict.items():
+            if key in ("trajectories", "id_probabilities"):
+                save_array_to_csv(
+                    output_dir / npy_path.with_suffix(f".{key}.csv").name,
+                    value,
+                    key=key,
+                )
+            elif key == "areas":
+                np.savetxt(
+                    output_dir / npy_path.with_suffix(f".{key}.csv").name,
+                    np.asarray((value["mean"], value["median"], value["std"])).T,
+                    delimiter=",",
+                    header="mean, median, standard_deviation",
+                    fmt="%.1f",
+                    comments="",
+                )
             else:
-                confusion.add(output, eval_target)
+                attributes_dict[key] = value
 
-        # Mini-Logs
-        losses += [loss] * input_.size(0)
-        if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-            losses_CE += [output[1]] * input_.size(0)
-            losses_MCL += [output[2]] * input_.size(0)
-
-    learner.step_schedule(epoch)
-    # print loss avg
-    # print(losses.avg)
-    # Loss-specific information
-    if network_params.loss == "CE":
+        json_path = output_dir / npy_path.with_suffix(".attributes.json").name
+        json.dump(attributes_dict, json_path.open("w"), indent=4)
+    except Exception as e:
+        logging.error(e)
         pass
-        # print("[Train] ACC: ", confusion.acc())
-    elif network_params.loss in ("MCL", "CEMCL", "CEMCL_weighted"):
-        network_params.cluster2Class = tuple(
-            confusion.optimal_assignment(train_loader.num_classes)
-        )  # Save the mapping in network_params to use in eval
-        # print(network_params.cluster2Class)
-        if network_params.out_dim <= 20:  # Avoid to print a large confusion matrix
-            confusion.show()
-        # print("Clustering scores:", confusion.clusterscores())
-        # print("[Train] ACC: ", confusion.acc())
-
-    if network_params.loss in ("CEMCL", "CEMCL_weighted"):
-        return (fmean(losses), fmean(losses_CE), fmean(losses_MCL)), confusion.acc()
-    return (fmean(losses), None, None), confusion.acc()
+
+
+@wrap_exceptions
+def main():
+    logging.basicConfig(level=logging.DEBUG, format="%(message)s", datefmt="%H:%M:%S")
+
+    parser = ArgumentParser()
+
+    parser.add_argument(
+        "session", help="Session path to convert trajectories to CSV and JSON", type=str
+    )
+
+    args = parser.parse_args()
+    path = Path(args.session)
+
+    if path.name.startswith("session_"):
+        path /= "trajectories"
+
+    for file in path.glob("*.npy"):
+        convert_trajectories_file_to_csv_and_json(file)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/assign_them_all.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/assign_them_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 from idtrackerai.utils import track
 
 from .compute_velocity_model import compute_model_velocity
 from .erosion import compute_erosion_disk, get_eroded_blobs
 
 
 def set_individual_with_identity_0_as_crossings(list_of_fragments: ListOfFragments):
-    for fragment in list_of_fragments.fragments:
+    for fragment in list_of_fragments.individual_fragments:
         if (
-            fragment.is_an_individual
-            and len(fragment.assigned_identities) == 1
+            len(fragment.assigned_identities) == 1
             and fragment.assigned_identities[0] == 0
         ):
             fragment.is_an_individual = False
+            fragment.forced_crossing = True
             fragment.identity = None
             fragment.identity_corrected_solving_jumps = None
 
 
 def find_the_gap_interval(
     blobs_in_video: list[list[Blob]],
     possible_identities: set[int],
@@ -110,15 +110,15 @@
     previous_blob_to_the_gap: Blob,
     next_blob_to_the_gap: Blob,
     identity: int,
     border: str,
 ) -> tuple[float, float]:
     blobs_for_interpolation = [previous_blob_to_the_gap, next_blob_to_the_gap]
     centroids_to_interpolate = [
-        blob.final_centroids[blob.final_identities.index(identity)]
+        list(blob.final_centroids)[list(blob.final_identities).index(identity)]
         for blob in blobs_for_interpolation
     ]
     centroids_to_interpolate = np.asarray(centroids_to_interpolate).T
     argsort_x = np.argsort(centroids_to_interpolate[0])
     centroids_to_interpolate[0] = centroids_to_interpolate[0][argsort_x]
     centroids_to_interpolate[1] = centroids_to_interpolate[1][argsort_x]
     number_of_points = individual_gap_interval[1] - individual_gap_interval[0] + 1
@@ -249,20 +249,19 @@
 
 def centroid_is_inside_of_any_eroded_blob(
     candidate_eroded_blobs: list[Blob], candidate_centroid: tuple[float, float]
 ) -> list[Blob]:
     # logging.debug('Checking whether the centroids is inside of a blob')
     candidate_centroid = tuple(map(int, candidate_centroid))
     # logging.debug('Finished whether the centroids is inside of a blob')
-    return list(
-        filter(
-            lambda b: cv2.pointPolygonTest(b.contour, candidate_centroid, False) >= 0,
-            candidate_eroded_blobs,
-        )
-    )
+    return [
+        b
+        for b in candidate_eroded_blobs
+        if cv2.pointPolygonTest(b.contour, candidate_centroid, False) >= 0
+    ]
 
 
 def evaluate_candidate_blobs_and_centroid(
     velocity_threshold: float,
     candidate_eroded_blobs: list[Blob],
     candidate_centroid: tuple[float, float],
     blob_in_border_frame: Blob,
@@ -319,18 +318,19 @@
                 original_blob, candidate_tuples_to_close_gap
             )
         )
         if len(candidate_tuples_with_centroids_in_original_blob) == 1:
             # the gap is a single individual blob
             identity = candidate_tuples_with_centroids_in_original_blob[0][2]
             centroid = candidate_tuples_with_centroids_in_original_blob[0][1]
+            original_blob_final_identities = list(original_blob.final_identities)
             if (
                 original_blob.is_an_individual
-                and len(original_blob.final_identities) == 1
-                and original_blob.final_identities[0] == 0
+                and len(original_blob_final_identities) == 1
+                and original_blob_final_identities[0] == 0
             ):
                 original_blob.identities_corrected_closing_gaps = [identity]
                 # TODO loop over the fragment
                 for blobs_in_frame in blobs_in_video:
                     for blob in blobs_in_frame:
                         if (
                             blob.fragment_identifier
@@ -396,25 +396,27 @@
                 ) in candidate_tuples_with_centroids_in_original_blob:
                     if count_eroded_blobs[eroded_blob] == 1:
                         # split blob, single individual
                         eroded_blob.frame_number = original_blob.frame_number
                         eroded_blob.centroid = centroid
                         eroded_blob.identities_corrected_closing_gaps = [identity]
                         eroded_blob.is_an_individual = True
+                        eroded_blob.forced_crossing = True
                         eroded_blob.was_a_crossing = True
                         new_original_blobs.append(eroded_blob)
                     elif count_eroded_blobs[eroded_blob] > 1:
                         if eroded_blob.interpolated_centroids is None:
                             eroded_blob.interpolated_centroids = []
                         if eroded_blob.identities_corrected_closing_gaps is None:
                             eroded_blob.identities_corrected_closing_gaps = []
                         eroded_blob.frame_number = original_blob.frame_number
                         eroded_blob.interpolated_centroids.append(centroid)
                         eroded_blob.identities_corrected_closing_gaps.append(identity)
                         eroded_blob.is_an_individual = False
+                        eroded_blob.forced_crossing = True
                         new_original_blobs.append(eroded_blob)
 
         new_original_blobs.append(original_blob)
 
     new_original_blobs = list(set(new_original_blobs))
     blobs_in_video[original_blob.frame_number] = new_original_blobs
     return blobs_in_video, list_of_occluded_identities
@@ -558,21 +560,19 @@
                     # else:
                     #     logging.debug('next_blob_to_the_gap exists')
                     for i in range(
                         individual_gap_interval[0], individual_gap_interval[1]
                     ):
                         list_of_occluded_identities[i].add(identity)
 
-            (blobs_in_video, list_of_occluded_identities) = (
-                assign_identity_to_new_blobs(
-                    blobs_in_video,
-                    inner_blobs_in_frame,
-                    candidate_tuples_to_close_gap,
-                    list_of_occluded_identities,
-                )
+            blobs_in_video, list_of_occluded_identities = assign_identity_to_new_blobs(
+                blobs_in_video,
+                inner_blobs_in_frame,
+                candidate_tuples_to_close_gap,
+                list_of_occluded_identities,
             )
     return blobs_in_video, list_of_occluded_identities
 
 
 def reset_blobs_in_video_before_erosion_iteration(all_blobs: Iterable[Blob]):
     """Resets the identity of crossings and individual with multiple identities
     before starting a loop of interpolation
@@ -580,15 +580,15 @@
     Parameters
     ----------
     blobs_in_video : list of lists of `Blob` objects
     """
     for blob in all_blobs:
         if blob.is_a_crossing:
             blob.identity = None
-        elif blob.is_an_individual and len(blob.final_identities) > 1:
+        elif blob.is_an_individual and len(list(blob.final_identities)) > 1:
             blob.identities_corrected_closing_gaps = None
 
 
 def close_trajectories_gaps(
     video: Video, list_of_blobs: ListOfBlobs, list_of_fragments: ListOfFragments
 ):
     """This is the main function to close the gaps where animals have not been
@@ -624,27 +624,27 @@
     """
     set_individual_with_identity_0_as_crossings(list_of_fragments)
     list_of_fragments.update_blobs(list_of_blobs.all_blobs)
 
     if not hasattr(video, "erosion_kernel_size"):
         video.erosion_kernel_size = compute_erosion_disk(list_of_blobs.blobs_in_video)
     if not hasattr(video, "velocity_threshold"):
-        video.velocity_threshold = compute_model_velocity(list_of_fragments.fragments)
+        video.velocity_threshold = compute_model_velocity(list_of_fragments)
     possible_identities = set(range(1, video.number_of_animals + 1))
     list_of_occluded_identities: list[set[int]] = [
         set() for _ in range(video.number_of_frames)
     ]
 
     previous_number_of_non_split_crossings = list_of_blobs.number_of_crossing_blobs
     erosion_counter = 0
     continue_erosion_protocol = True
     # TODO why erosion_counter==1?
     while continue_erosion_protocol or erosion_counter == 1:
         reset_blobs_in_video_before_erosion_iteration(list_of_blobs.all_blobs)
-        (list_of_blobs.blobs_in_video, list_of_occluded_identities) = (
+        list_of_blobs.blobs_in_video, list_of_occluded_identities = (
             interpolate_trajectories_during_gaps(
                 video,
                 list_of_blobs.blobs_in_video,
                 list_of_occluded_identities,
                 possible_identities,
                 erosion_counter,
             )
@@ -657,10 +657,10 @@
             > current_number_of_non_split_crossings
         )
 
         previous_number_of_non_split_crossings = current_number_of_non_split_crossings
         erosion_counter += 1
 
     for blob in list_of_blobs.all_blobs:
-        if blob.is_an_individual and len(blob.final_identities) > 1:
+        if blob.is_an_individual and len(list(blob.final_identities)) > 1:
             blob.identities_corrected_closing_gaps = None
     return list_of_blobs
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/compute_velocity_model.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/compute_velocity_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,25 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
+
+
 import numpy as np
 
-from idtrackerai import Fragment
+from idtrackerai import ListOfFragments
 from idtrackerai.utils import conf, track
 
 
-def compute_model_velocity(fragments: list[Fragment], percentile=None) -> float:
+def compute_model_velocity(
+    list_of_fragments: ListOfFragments, percentile=None
+) -> float:
     """computes the 2 * (percentile) of the distribution of velocities of identified fish.
     params
     -----
     blobs_in_video: list of blob objects
         collection of blobs detected in the video.
     number_of_animals int
     percentile int
@@ -47,20 +51,21 @@
     -----
     float
     2 * np.max(distance_travelled_in_individual_fragments) if percentile is None
     2 * percentile(velocity distribution of identified animals) otherwise
     """
     if percentile is None:
         percentile = conf.VEL_PERCENTILE
-    distance_travelled_in_individual_fragments: list[np.ndarray] = []
+    distance_travelled_in_individual_fragments: list[float] = []
 
-    for fragment in track(fragments, "Computing velocity model"):
-        if fragment.is_an_individual:
-            distance_travelled_in_individual_fragments.extend(
-                fragment.frame_by_frame_velocity()
-            )
+    for fragment in track(
+        list_of_fragments.individual_fragments, "Computing velocity model"
+    ):
+        distance_travelled_in_individual_fragments.extend(
+            fragment.frame_by_frame_velocity
+        )
     return (
         2 * np.max(distance_travelled_in_individual_fragments)
         if percentile is None
         else 2.0
         * float(np.percentile(distance_travelled_in_individual_fragments, percentile))
     )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/correct_impossible_velocity_jumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from idtrackerai import Fragment, ListOfFragments, Video
 from idtrackerai.utils import track
 
 
 def get_candidate_identities_by_minimum_speed(
     fragment: Fragment,
     fragments: list[Fragment],
-    available_identities: set,
+    available_identities: list[int],
     impossible_velocity_threshold: float,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Computes the candidate identities for a given `fragment` taking into
     consideration the velocities needed to join the `fragment` with its neighbour
     fragments in the past and in the future
 
     Parameters
@@ -87,34 +87,35 @@
         neighbour_fragment_future = fragment.get_neighbour_fragment(
             fragments, "to_the_future"
         )
         velocities_between_fragments = compute_velocities_consecutive_fragments(
             neighbour_fragment_past, fragment, neighbour_fragment_future
         )
 
-        if all(np.isnan(velocities_between_fragments)):
+        if np.isnan(velocities_between_fragments).all():
             speed_of_candidate_identities.append(impossible_velocity_threshold)
         else:
             speed_of_candidate_identities.append(
                 np.nanmax(velocities_between_fragments)
             )
     fragment.user_generated_identity = None
     argsort_identities_by_speed = np.argsort(speed_of_candidate_identities)
     return (
-        np.asarray(list(available_identities))[argsort_identities_by_speed],
+        np.asarray(available_identities)[argsort_identities_by_speed],
         np.asarray(speed_of_candidate_identities)[argsort_identities_by_speed],
     )
 
 
 def get_candidate_identities_above_random_P2(
     fragment: Fragment,
     fragments: list[Fragment],
     non_available_identities: np.ndarray,
-    available_identities: set,
+    available_identities: list[int],
     impossible_velocity_threshold: float,
+    number_of_animals: int,
 ):
     """Computes the candidate identities of a `fragment` taking into
     consideration the probability of identification given by its
     `fragment.P2_vector`. An identity is a potential candidate if the
     probability of identification is above random.
 
     Parameters
@@ -148,34 +149,35 @@
 
     See Also
     --------
     Fragment
     get_candidate_identities_by_minimum_speed
 
     """
-    # TODO does it need a copy()?
     P2_vector = fragment.P2_vector
     assert P2_vector is not None
     if len(non_available_identities) > 0:
         P2_vector[non_available_identities - 1] = 0
     if all(P2_vector == 0):
-        (candidate_identities_speed, _) = get_candidate_identities_by_minimum_speed(
+        candidate_identities_speed, _ = get_candidate_identities_by_minimum_speed(
             fragment, fragments, available_identities, impossible_velocity_threshold
         )
         return candidate_identities_speed
 
     if fragment.number_of_images == 1:
-        random_threshold = 1 / fragment.number_of_animals
+        random_threshold = 1 / number_of_animals
     else:
         random_threshold = 1 / fragment.number_of_images
     return np.argwhere(P2_vector > random_threshold)[:, 0] + 1
 
 
 def reassign(
-    fragment: Fragment, fragments: list[Fragment], impossible_velocity_threshold: float
+    fragment: Fragment,
+    list_of_fragments: ListOfFragments,
+    impossible_velocity_threshold: float,
 ):
     """Reassigns the identity of a given `fragment` considering the identity of the
     `fragments` coexisting with it and the `impossible_velocity_threshold`
 
     Parameters
     ----------
     fragment : <Fragment object>
@@ -199,37 +201,43 @@
     """
 
     non_available_identities = {
         coexisting_fragment.assigned_identities[0]
         for coexisting_fragment in fragment.coexisting_individual_fragments
     }
     available_identities = (
-        set(range(1, fragment.number_of_animals + 1)) - non_available_identities
+        set(range(1, list_of_fragments.number_of_animals + 1))
+        - non_available_identities
     )
     if fragment.assigned_identities[0] not in (None, 0):
         available_identities.add(fragment.assigned_identities[0])
 
     if 0 in non_available_identities:
         non_available_identities.remove(0)
     non_available_identities = np.asarray(list(non_available_identities))
 
     if len(available_identities) == 1:
         candidate_id = available_identities.pop()
     else:
+        available_identities = list(available_identities)
         candidate_identities_speed, speed_of_candidate_identities = (
             get_candidate_identities_by_minimum_speed(
-                fragment, fragments, available_identities, impossible_velocity_threshold
+                fragment,
+                list_of_fragments.fragments,
+                available_identities,
+                impossible_velocity_threshold,
             )
         )
         candidate_identities_P2 = get_candidate_identities_above_random_P2(
             fragment,
-            fragments,
+            list_of_fragments.fragments,
             non_available_identities,
             available_identities,
             impossible_velocity_threshold,
+            list_of_fragments.number_of_animals,
         )
         candidate_identities: list[int] = []
         candidate_speeds: list[float] = []
         for candidate_id, candidate_speed in zip(
             candidate_identities_speed, speed_of_candidate_identities
         ):
             if candidate_id in candidate_identities_P2:
@@ -381,30 +389,26 @@
 
     See Also
     --------
     get_fragment_with_same_identity
     compute_velocities_consecutive_fragments
 
     """
-    (neighbour_fragment_past, number_of_frames_in_past) = (
-        get_fragment_with_same_identity(
-            number_of_frames, list_of_fragments, fragment, "to_the_past"
-        )
+    neighbour_fragment_past, n_frames_in_past = get_fragment_with_same_identity(
+        number_of_frames, list_of_fragments, fragment, "to_the_past"
     )
-    (neighbour_fragment_future, number_of_frames_in_future) = (
-        get_fragment_with_same_identity(
-            number_of_frames, list_of_fragments, fragment, "to_the_future"
-        )
+    neighbour_fragment_future, n_frames_in_future = get_fragment_with_same_identity(
+        number_of_frames, list_of_fragments, fragment, "to_the_future"
     )
 
     velocities = compute_velocities_consecutive_fragments(
         neighbour_fragment_past, fragment, neighbour_fragment_future
     )
     velocities_between_fragments = np.asarray(velocities) / np.asarray(
-        [number_of_frames_in_past, number_of_frames_in_future]
+        [n_frames_in_past, n_frames_in_future]
     )
 
     return (
         neighbour_fragment_past,
         neighbour_fragment_future,
         velocities_between_fragments,
     )
@@ -463,17 +467,15 @@
         if all(velocities_between_fragments > impossible_velocity_threshold):
             assert neighbour_fragment_future is not None
             assert neighbour_fragment_past is not None
             if (
                 neighbour_fragment_past.identity_is_fixed
                 or neighbour_fragment_future.identity_is_fixed
             ):
-                reassign(
-                    fragment, list_of_fragments.fragments, impossible_velocity_threshold
-                )
+                reassign(fragment, list_of_fragments, impossible_velocity_threshold)
             else:
                 neighbour_fragment_past_past = (
                     neighbour_fragment_past.get_neighbour_fragment(
                         list_of_fragments.fragments, "to_the_past"
                     )
                 )
                 velocity_in_past = compute_velocities_consecutive_fragments(
@@ -489,41 +491,33 @@
                     neighbour_fragment_future,
                     neighbour_fragment_future_future,
                 )[1]
                 if (
                     velocity_in_past < impossible_velocity_threshold
                     or velocity_in_future < impossible_velocity_threshold
                 ):
-                    reassign(
-                        fragment,
-                        list_of_fragments.fragments,
-                        impossible_velocity_threshold,
-                    )
+                    reassign(fragment, list_of_fragments, impossible_velocity_threshold)
         elif velocities_between_fragments[0] > impossible_velocity_threshold:
             assert neighbour_fragment_past is not None
             if neighbour_fragment_past.identity_is_fixed:
-                reassign(
-                    fragment, list_of_fragments.fragments, impossible_velocity_threshold
-                )
+                reassign(fragment, list_of_fragments, impossible_velocity_threshold)
             else:
                 reassign(
                     neighbour_fragment_past,
-                    list_of_fragments.fragments,
+                    list_of_fragments,
                     impossible_velocity_threshold,
                 )
         elif velocities_between_fragments[1] > impossible_velocity_threshold:
             assert neighbour_fragment_future is not None
             if neighbour_fragment_future.identity_is_fixed:
-                reassign(
-                    fragment, list_of_fragments.fragments, impossible_velocity_threshold
-                )
+                reassign(fragment, list_of_fragments, impossible_velocity_threshold)
             else:
                 reassign(
                     neighbour_fragment_future,
-                    list_of_fragments.fragments,
+                    list_of_fragments,
                     impossible_velocity_threshold,
                 )
 
 
 def correct_impossible_velocity_jumps(video: Video, list_of_fragments: ListOfFragments):
     """Corrects the parts of the video where the velocity of any individual is
     higher than a particular velocity threshold given by `video.velocity_threshold`.
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/erosion.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/erosion.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,25 +69,24 @@
 
 def get_eroded_blobs(
     video: Video, blobs_in_frame: list[Blob], frame_number: int
 ) -> list[Blob]:
     segmented_frame = np.zeros((video.height, video.width), np.uint8)
 
     for blob in blobs_in_frame:
-        segmented_frame = cv2.fillPoly(segmented_frame, [blob.contour], 255)
+        segmented_frame = cv2.fillPoly(segmented_frame, (blob.contour,), 255)
 
     segmented_eroded_frame = cv2.erode(
         src=segmented_frame,
         kernel=np.ones(video.erosion_kernel_size, np.uint8),
         iterations=1,
     )
 
     # Extract blobs info
-    # TODO cv2.CHAIN_APPROX_TC89_L1
     contours = cv2.findContours(
-        segmented_eroded_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
+        segmented_eroded_frame, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_TC89_KCOS
     )[0]
 
     return [
         Blob(contour, frame_number=frame_number, pixels_are_from_eroded_blob=True)
         for contour in contours
     ]
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/get_trajectories.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/get_trajectories.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,24 @@
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 from importlib import metadata
 from typing import Callable
 
 import numpy as np
 
-from idtrackerai import Blob, Video
+from idtrackerai import Blob, Fragment, Video
 from idtrackerai.utils import track
 
 
 def produce_trajectories(
     blobs_in_video: list[list[Blob]],
     number_of_animals: int,
     progress_bar=None,
     abort: Callable = lambda: False,
+    fragments: list[Fragment] | None = None,
 ):
     """Produce trajectories array from ListOfBlobs
 
     Parameters
     ----------
     blobs_in_video : <ListOfBlobs object>
         See :class:`list_of_blobs.ListOfBlobs`
@@ -65,40 +66,46 @@
     id_probabilities = np.full((number_of_frames, number_of_animals, 1), np.NaN)
     areas = np.full((number_of_frames, number_of_animals), np.NaN)
 
     for frame_number, blobs_in_frame in enumerate(
         track(blobs_in_video, "Producing trajectories")
     ):
         if abort():
-            return None
+            return None, None, {}
         if progress_bar:
             progress_bar.emit(frame_number)
         for blob in blobs_in_frame:
-            for identity, centroid in zip(blob.final_identities, blob.final_centroids):
+            for identity, centroid in blob.final_ids_and_centroids:
                 if identity not in (None, 0):
                     centroid_trajectories[blob.frame_number, identity - 1, :] = centroid
-            if (
-                blob.is_an_individual
-                and len(blob.final_identities) == 1
-                and blob.P2_vector is not None
-            ):
-                identity = blob.final_identities[0]
-                if identity not in (None, 0):
-                    id_probabilities[blob.frame_number, identity - 1, :] = np.max(
-                        blob.P2_vector
-                    )
-                    areas[blob.frame_number, identity - 1] = blob.area
-
-    return {
-        "centroid_trajectories": centroid_trajectories,
-        "id_probabilities": id_probabilities,
-        "mean_areas": np.nanmean(areas, axis=0),
-        "median_areas": np.nanmedian(areas, axis=0),
-        "std_areas": np.nanstd(areas, axis=0),
-    }
+            blob_final_identities = list(blob.final_identities)
+            if blob.is_an_individual and len(blob_final_identities) == 1:
+                identity = blob_final_identities[0]
+                if identity in (None, 0):
+                    continue
+
+                areas[blob.frame_number, identity - 1] = blob.area
+
+                if fragments is None:
+                    continue
+                P2_vector = fragments[blob.fragment_identifier].P2_vector
+
+                if P2_vector is None:
+                    continue
+                id_probabilities[blob.frame_number, identity - 1, :] = np.max(P2_vector)
+
+    return (
+        centroid_trajectories,
+        id_probabilities,
+        {
+            "mean": np.nanmean(areas, axis=0),
+            "median": np.nanmedian(areas, axis=0),
+            "std": np.nanstd(areas, axis=0),
+        },
+    )
 
 
 def produce_trajectories_wo_identification(
     blobs_in_video: list[list[Blob]],
     number_of_animals: int,
     progress_bar=None,
     abort: Callable = lambda: False,
@@ -108,15 +115,15 @@
     identifiers_prev = np.full(number_of_animals, np.nan)
     areas = np.full((number_of_frames, number_of_animals), np.nan)
 
     for frame_number, blobs_in_frame in enumerate(
         track(blobs_in_video, "Creating trajectories")
     ):
         if abort():
-            return None
+            return None, None, {}
         if progress_bar:
             progress_bar.emit(frame_number)
         try:
             identifiers_next = {
                 b.fragment_identifier for b in blobs_in_video[frame_number + 1]
             }
         except IndexError:  # last frame
@@ -130,31 +137,36 @@
                     ][0]
                 else:
                     column = np.argwhere(np.isnan(identifiers_prev))[0][0]
                     identifiers_prev[column] = blob.fragment_identifier
 
                 blob.identity = column + 1
                 # blobs that are individual only have one centroid
-                centroid_trajectories[frame_number, column, :] = blob.final_centroids[0]
+                centroid_trajectories[frame_number, column, :] = next(
+                    blob.final_centroids
+                )
                 areas[frame_number, column] = blob.area
 
                 if blob.fragment_identifier not in identifiers_next:
                     identifiers_prev[column] = np.nan
-    return {
-        "centroid_trajectories": centroid_trajectories,
-        "id_probabilities": None,
-        "mean_areas": np.nanmean(areas, axis=0),
-        "median_areas": np.nanmedian(areas, axis=0),
-        "std_areas": np.nanstd(areas, axis=0),
-    }
+    return (
+        centroid_trajectories,
+        None,
+        {
+            "mean": np.nanmean(areas, axis=0),
+            "median": np.nanmedian(areas, axis=0),
+            "std": np.nanstd(areas, axis=0),
+        },
+    )
 
 
 def produce_output_dict(
     blobs_in_video: list[list[Blob]],
     video: Video,
+    fragments: list[Fragment] | None = None,
     progress_bar=None,
     abort: Callable = lambda: False,
 ):
     """Outputs the dictionary with keys: trajectories, git_commit, video_path,
     frames_per_second
 
     Parameters
@@ -169,47 +181,47 @@
     -------
     dict
         Output dictionary containing trajectories as values
 
     """
     if video.track_wo_identities:
         video.number_of_animals = max(map(len, blobs_in_video))
-        trajectories_info_dict = produce_trajectories_wo_identification(
+
+    centroid_trajectories, id_probabilities, area_stats = (
+        produce_trajectories_wo_identification(
             blobs_in_video, video.number_of_animals, progress_bar, abort
         )
-    else:
-        trajectories_info_dict = produce_trajectories(
-            blobs_in_video, video.number_of_animals, progress_bar, abort
+        if video.track_wo_identities
+        else produce_trajectories(
+            blobs_in_video, video.number_of_animals, progress_bar, abort, fragments
         )
-    if trajectories_info_dict is None or abort():
+    )
+
+    if centroid_trajectories is None or abort():
         return None
 
     output_dict = {
-        "trajectories": (
-            trajectories_info_dict["centroid_trajectories"] / video.resolution_reduction
-        ),
+        "trajectories": centroid_trajectories / video.resolution_reduction,
         "version": metadata.version("idtrackerai"),
         "video_paths": list(map(str, video.video_paths)),
         "frames_per_second": video.frames_per_second,
         "body_length": video.median_body_length_full_resolution,
         "stats": {"estimated_accuracy": video.estimated_accuracy},
-        "areas": {
-            "mean": trajectories_info_dict["mean_areas"],
-            "median": trajectories_info_dict["median_areas"],
-            "std": trajectories_info_dict["std_areas"],
-        },
+        "areas": area_stats,
         "setup_points": video.setup_points,
-        "identities_labels": video.identities_labels,
+        "identities_labels": video.identities_labels or [
+            str(i + 1) for i in range(video.number_of_animals)
+        ],
         "identities_groups": {
             key: list(value) for key, value in video.identities_groups.items()
         },
     }
 
-    if trajectories_info_dict["id_probabilities"] is not None:
-        output_dict["id_probabilities"] = trajectories_info_dict["id_probabilities"]
+    if id_probabilities is not None and np.isfinite(id_probabilities).any():
+        output_dict["id_probabilities"] = id_probabilities
         # After the interpolation some identities that were 0 are assigned
         output_dict["stats"]["estimated_accuracy_after_interpolation"] = (
             1 if video.single_animal else np.nanmean(output_dict["id_probabilities"])
         )
         # Centroids with identity
         identified = ~np.isnan(output_dict["trajectories"][..., 0])
         output_dict["stats"]["percentage_identified"] = np.mean(identified)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/identify_non_assigned_with_interpolation.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/postprocess/trajectories_creation.py` & `idtrackerai-5.1.4/src/idtrackerai/postprocess/trajectories_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Iterable
 
 import numpy as np
 
-from idtrackerai import Blob, Fragment, ListOfBlobs, ListOfFragments, Video
+from idtrackerai import Blob, ListOfBlobs, ListOfFragments, Video
 from idtrackerai.utils import conf, create_dir
 
 from .assign_them_all import close_trajectories_gaps
 from .compute_velocity_model import compute_model_velocity
 from .correct_impossible_velocity_jumps import correct_impossible_velocity_jumps
 from .get_trajectories import produce_output_dict
 from .identify_non_assigned_with_interpolation import (
@@ -28,15 +28,17 @@
         and not single_global_fragment
     ):
         postprocess_impossible_jumps(video, list_of_fragments, list_of_blobs.all_blobs)
 
     video.create_trajectories_timer.start()
     create_dir(video.trajectories_folder, remove_existing=True)
 
-    trajectories = produce_output_dict(list_of_blobs.blobs_in_video, video)
+    trajectories = produce_output_dict(
+        list_of_blobs.blobs_in_video, video, list_of_fragments.fragments
+    )
 
     trajectories_file = video.trajectories_folder / (
         "trajectories_wo_identification.npy"
         if video.track_wo_identities
         else "trajectories.npy"
     )
 
@@ -60,38 +62,37 @@
     video.save()
 
 
 def postprocess_impossible_jumps(
     video: Video, list_of_fragments: ListOfFragments, all_blobs: Iterable[Blob]
 ):
     video.impossible_jumps_timer.start()
-    video.velocity_threshold = compute_model_velocity(list_of_fragments.fragments)
+    video.velocity_threshold = compute_model_velocity(list_of_fragments)
     correct_impossible_velocity_jumps(video, list_of_fragments)
 
     video.individual_fragments_stats = list_of_fragments.get_stats()
 
-    video.estimated_accuracy = compute_estimated_accuracy(list_of_fragments.fragments)
-    list_of_fragments.save(video.accumulation_folder / "list_of_fragments.pickle")
+    video.estimated_accuracy = compute_estimated_accuracy(list_of_fragments)
+    list_of_fragments.save(video.accumulation_folder / "list_of_fragments.json")
     list_of_fragments.update_blobs(all_blobs)
     video.impossible_jumps_timer.finish()
 
 
-def compute_estimated_accuracy(fragments: list[Fragment]) -> float:
+def compute_estimated_accuracy(list_of_fragments: ListOfFragments) -> float:
     weighted_P2 = 0
     number_of_individual_blobs = 0
 
-    for fragment in fragments:
-        if fragment.is_an_individual:
-            if fragment.assigned_identities[0] not in (0, None):
-                assert fragment.P2_vector is not None
-                weighted_P2 += (
-                    fragment.P2_vector[fragment.assigned_identities[0] - 1]
-                    * fragment.number_of_images
-                )
-            number_of_individual_blobs += fragment.number_of_images
+    for fragment in list_of_fragments.individual_fragments:
+        if fragment.assigned_identities[0] not in (0, None):
+            assert fragment.P2_vector is not None
+            weighted_P2 += (
+                fragment.P2_vector[fragment.assigned_identities[0] - 1]
+                * fragment.number_of_images
+            )
+        number_of_individual_blobs += fragment.number_of_images
     return weighted_P2 / number_of_individual_blobs
 
 
 def interpolate_crossings(video: Video, list_of_fragments: ListOfFragments):
     video.crossing_solver_timer.start()
     list_of_blobs_no_gaps = close_trajectories_gaps(
         video, ListOfBlobs.load(video.blobs_path), list_of_fragments
@@ -101,15 +102,15 @@
 
     trajectories_wo_gaps_file = video.trajectories_folder / "trajectories_wo_gaps.npy"
     logging.info(
         "Generating trajectories. The trajectories files are stored in "
         f"{trajectories_wo_gaps_file}"
     )
     trajectories_wo_gaps = produce_output_dict(
-        list_of_blobs_no_gaps.blobs_in_video, video
+        list_of_blobs_no_gaps.blobs_in_video, video, list_of_fragments.fragments
     )
 
     np.save(trajectories_wo_gaps_file, trajectories_wo_gaps)  # type: ignore
     if conf.CONVERT_TRAJECTORIES_TO_CSV_AND_JSON:
         convert_trajectories_file_to_csv_and_json(trajectories_wo_gaps_file)
 
     # Now, two ListOfBlobs will be loaded in RAM, we clean the heavier parts of
@@ -127,11 +128,13 @@
             del blob.convexHull
 
     logging.info("Saving trajectories")
     list_of_blobs = assign_zeros_with_interpolation_identities(
         list_of_blobs, list_of_blobs_no_gaps
     )
     trajectories_file = video.trajectories_folder / "trajectories.npy"
-    trajectories = produce_output_dict(list_of_blobs.blobs_in_video, video)
+    trajectories = produce_output_dict(
+        list_of_blobs.blobs_in_video, video, list_of_fragments.fragments
+    )
     np.save(trajectories_file, trajectories)  # type: ignore
     if conf.CONVERT_TRAJECTORIES_TO_CSV_AND_JSON:
         convert_trajectories_file_to_csv_and_json(trajectories_file)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 import random
 from pathlib import Path
 
 import numpy as np
+from torch.nn import Module
 
 from idtrackerai import Fragment, GlobalFragment, ListOfFragments, ListOfGlobalFragments
 from idtrackerai.utils import conf, load_id_images
 
 from .accumulation_manager_utils import (
     get_P1_array_and_argsort,
     p1_below_random,
@@ -98,15 +99,15 @@
             threshold_acceptable_accumulation = float(
                 conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
             )
         self.id_images_file_paths = id_images_file_paths
         self.number_of_animals = number_of_animals
         self.list_of_fragments = list_of_fragments
         self.list_of_global_fragments = list_of_global_fragments
-        self.counter = 0
+        self.current_step: int = 0
         self.certainty_threshold = certainty_threshold
         self.threshold_acceptable_accumulation = threshold_acceptable_accumulation
         self.accumulation_strategy = "global"
         self.individual_fragments_used: list[int] = []
         self.used_images = None
         self.used_labels = None
         self.new_images = None
@@ -136,34 +137,42 @@
             return True
         logging.info(
             "[bold]There are no more global fragments acceptable for training",
             extra={"markup": True},
         )
         return False
 
-    def update_counter(self):
-        """Update iteration counter"""
-        self.counter += 1
-
     def get_new_images_and_labels(self):
         """Get the images and labels of the new global fragments that are going
         to be used for training. This function checks whether the images of a individual
         fragment have been added before"""
-        n_images = 0
-        self.new_images, self.new_labels = (
-            self.list_of_fragments.get_new_images_and_labels_for_training()
-        )
-        if self.new_images is not None:
-            logging.info(f"{len(self.new_images)} new images for training")
-            n_images += len(self.new_images)
+
+        images = []
+        labels = []
+        for fragment in self.list_of_fragments.individual_fragments:
+            if fragment.acceptable_for_training and not fragment.used_for_training:
+                images.extend(fragment.image_locations)
+                labels.extend([fragment.temporary_id] * fragment.number_of_images)
+
+        if images:
+            self.new_images, self.new_labels = np.asarray(images), np.asarray(labels)
+        else:
+            self.new_images, self.new_labels = None, None
+
+        n_used_images = len(self.used_images) if self.used_images is not None else 0
+        n_new_images = len(self.new_images) if self.new_images is not None else 0
+        n_images = n_used_images + n_new_images
+
+        if n_new_images:
+            logging.info("%d new images for training", n_new_images)
         else:
             logging.info("There are no new images in this accumulation")
-        if self.used_images is not None:
-            n_images += len(self.used_images)
-            logging.info(f"{len(self.used_images)} old images for training")
+
+        if n_used_images:
+            logging.info("%d old images for training", n_used_images)
 
         ratio = n_images / self.list_of_fragments.number_of_images_in_global_fragments
         logging.info(
             f"{n_images} images in total, {ratio:.2%} of the total accumulable"
         )
 
     def get_images_and_labels_for_training(self):
@@ -252,15 +261,15 @@
                     images.extend(list(self.used_images[used_images_indices]))
                     labels.extend([i] * number_of_used_images)
         return load_id_images(self.id_images_file_paths, images), np.asarray(labels)
 
     def update_used_images_and_labels(self):
         """Sets as used the images already used for training"""
         logging.info("Update images and labels used for training")
-        if self.counter == 0:
+        if self.current_step == 0:
             self.used_images = self.new_images
             self.used_labels = self.new_labels
         elif self.new_images is not None:
             self.used_images = np.concatenate(
                 (self.used_images, self.new_images), axis=0
             )
             self.used_labels = np.concatenate(
@@ -274,15 +283,15 @@
         for fragment in self.list_of_fragments.fragments:
             if fragment.acceptable_for_training and not fragment.used_for_training:
                 fragment.used_for_training = True
                 fragment.acceptable_for_training = False
                 fragment.set_partially_or_globally_accumulated(
                     self.accumulation_strategy
                 )
-                fragment.accumulation_step = self.counter
+                fragment.accumulation_step = self.current_step
 
     def assign_identities_to_fragments_used_for_training(self):
         """Assign the identities to the global fragments used for training and
         their individual fragments.
         This function checks that the identities of the individual fragments in
         the global fragment
         are consistent with the previously assigned identities
@@ -324,15 +333,15 @@
         self.individual_fragments_used.extend(new_individual_fragments_identifiers)
 
     def split_predictions_after_network_assignment(
         self,
         predictions,
         softmax_probs,
         indices_to_split,
-        candidate_individual_fragments_identifiers,
+        candidate_individual_fragments_identifiers: list[int],
     ):
         """Gathers predictions relative to fragment images from the GPU and
         splits them according to their organization in fragments.
         """
         logging.debug("Computing fragment prediction statistics")
         individual_fragments_predictions = np.split(predictions, indices_to_split)
         individual_fragments_softmax_probs = np.split(softmax_probs, indices_to_split)
@@ -345,22 +354,24 @@
             individual_fragments_predictions,
             individual_fragments_softmax_probs,
             candidate_individual_fragments_identifiers,
         ):
             self.list_of_fragments.fragments[
                 candidate_individual_fragment_identifier
             ].compute_identification_statistics(
-                individual_fragment_predictions, individual_fragment_softmax_probs
+                individual_fragment_predictions,
+                individual_fragment_softmax_probs,
+                self.list_of_fragments.number_of_animals,
             )
 
     def reset_accumulation_variables(self):
         """After an accumulation is finished reinitialise the variables involved
         in the process.
         """
-        self.temporary_individual_fragments_used = []
+        self.temporary_individual_fragments_used: list[int] = []
         if self.accumulation_strategy == "global":
             self.number_of_noncertain_global_fragments = 0
             self.number_of_random_assigned_global_fragments = 0
             self.number_of_nonconsistent_global_fragments = 0
             self.number_of_nonunique_global_fragments = 0
         self.number_of_sparse_fragments = 0
         self.number_of_noncertain_fragments = 0
@@ -537,15 +548,15 @@
                 else:
                     logging.warning(
                         "Individual fragment not in candidates or in used, this should"
                         " not happen"
                     )
             # Compute identities if the global_fragment is certain
             if global_fragment.acceptable_for_training(self.accumulation_strategy):
-                (P1_array, index_individual_fragments_sorted_by_P1_max_to_min) = (
+                P1_array, index_individual_fragments_sorted_by_P1_max_to_min = (
                     get_P1_array_and_argsort(global_fragment)
                 )
                 # set to zero the P1 of the the identities of the individual
                 # fragments that have been already used
                 for index_individual_fragment, fragment in enumerate(
                     global_fragment.individual_fragments
                 ):
@@ -579,38 +590,39 @@
                         ):
                             self.reset_non_acceptable_global_fragment(global_fragment)
                             fragment.non_consistent = True
                             self.number_of_nonconsistent_global_fragments += 1
                             break
 
                         P1_array = set_fragment_temporary_id(
-                            fragment, temporary_id, P1_array, index_individual_fragment
+                            fragment,
+                            int(temporary_id),
+                            P1_array,
+                            index_individual_fragment,
                         )
 
                 # Check if the global fragment is unique after assigning the identities
                 if global_fragment.acceptable_for_training(self.accumulation_strategy):
-                    if not global_fragment.is_unique:
+                    if not global_fragment.is_unique(self.number_of_animals):
                         # set acceptable_for_training to False and temporary_id to
                         # None for all the individual_fragments
                         # that had not been accumulated before (i.e. not in
                         # temporary_individual_fragments_used or individual_fragments_used)
                         self.reset_non_acceptable_global_fragment(global_fragment)
                         self.number_of_nonunique_global_fragments += 1
                     else:
-                        global_fragment.accumulation_step = self.counter
-                        [
-                            self.temporary_individual_fragments_used.append(
-                                fragment.identifier
-                            )
+                        global_fragment.accumulation_step = self.current_step
+                        self.temporary_individual_fragments_used.extend(
+                            fragment.identifier
                             for fragment in global_fragment.individual_fragments
                             if fragment.identifier
                             not in self.temporary_individual_fragments_used
                             and fragment.identifier
                             not in self.individual_fragments_used
-                        ]
+                        )
         elif self.accumulation_strategy == "partial":
             for fragment in global_fragment.individual_fragments:
                 fragment.acceptable_for_training = False
 
             for fragment in global_fragment.individual_fragments:
                 # Check certainties of the individual fragme
                 if (
@@ -724,27 +736,27 @@
                 and fragment.acceptable_for_training
             ]
             self.number_of_acceptable_fragments += sum(
                 bool(fragment.acceptable_for_training)
                 and not fragment.used_for_training
                 for fragment in global_fragment.individual_fragments
             )
-            global_fragment.accumulation_step = self.counter
+            global_fragment.accumulation_step = self.current_step
         assert all(
             fragment.temporary_id is not None
             for fragment in global_fragment.individual_fragments
             if fragment.acceptable_for_training and fragment.is_an_individual
         )
 
 
 def get_predictions_of_candidates_fragments(
-    identification_model,
+    identification_model: Module,
     id_images_file_paths: list[Path],
     network_params,
-    fragments: list[Fragment],
+    list_of_fragments: ListOfFragments,
 ):
     """Get predictions of individual fragments that have been used to train the
     idCNN in an accumulation's iteration
 
     Parameters
     ----------
     net : ConvNetwork object
@@ -765,19 +777,19 @@
         (used to rebuild the collection of images per fragment after gathering
         predicions and softmax vectors from the gpu)
     candidate_individual_fragments_identifiers : list
         list of fragment identifiers
     """
     images = []
     lengths = []
-    candidate_individual_fragments_identifiers = []
+    candidate_individual_fragments_identifiers: list[int] = []
 
-    for fragment in fragments:
-        if fragment.is_an_individual and not fragment.used_for_training:
-            images.extend(list(zip(fragment.images, fragment.episodes)))
+    for fragment in list_of_fragments.individual_fragments:
+        if not fragment.used_for_training:
+            images.extend(fragment.image_locations)
             lengths.append(fragment.number_of_images)
             candidate_individual_fragments_identifiers.append(fragment.identifier)
 
     assert images
     images = load_id_images(id_images_file_paths, images)
 
     predictions, softmax_probs = get_predictions_identities(
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulation_manager_utils.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/accumulation_manager_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/accumulator.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/accumulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
+from shutil import copyfile
 
 import torch
-from torch import nn
 from torch.backends import cudnn
+from torch.nn import CrossEntropyLoss, Module
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import Video
 from idtrackerai.network import LearnerClassification, NetworkParams
 from idtrackerai.utils import conf
 
 from .accumulation_manager import (
@@ -48,104 +49,106 @@
 from .network.stop_training_criteria import StopTraining
 from .network.trainer import TrainIdentification
 
 
 def perform_one_accumulation_step(
     accumulation_manager: AccumulationManager,
     video: Video,
-    identification_model: nn.Module,
-    learner_class: type[LearnerClassification],
+    identification_model: Module,
     network_params: NetworkParams,
 ):
     logging.info(
-        f"[bold]Performing new accumulation, step {accumulation_manager.counter}",
+        f"[bold]Performing new accumulation, step {accumulation_manager.current_step}",
         extra={"markup": True},
     )
-    video.accumulation_step = accumulation_manager.counter
+    video.accumulation_step = accumulation_manager.current_step
 
     # Get images for training
     accumulation_manager.get_new_images_and_labels()
     images, labels = accumulation_manager.get_images_and_labels_for_training()
     train_data, val_data = split_data_train_and_validation(
         images, labels, validation_proportion=conf.VALIDATION_PROPORTION
     )
     assert images.shape[0] == labels.shape[0]
     logging.info(
-        f"Training with {len(train_data['images'])}, "
-        f"validating with {len(val_data['images'])}"
+        "Training with %d, validating with %d",
+        len(train_data["images"]),
+        len(val_data["images"]),
     )
     assert len(val_data["images"]) > 0
 
     # Set data loaders
     train_loader, val_loader = get_training_data_loaders(
         video.number_of_animals, train_data, val_data
     )
 
     # Set criterion
     logging.info("Setting training criterion")
-    criterion = nn.CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
+    criterion = CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
 
     # Send model and criterion to GPU
     if network_params.use_gpu:
         torch.cuda.set_device(0)
         logging.info(
             'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
         )
         cudnn.benchmark = True  # make it train faster
         identification_model = identification_model.cuda()
         criterion = criterion.cuda()
 
-    # Set optimizer
-    logging.info("Setting optimizer")
-    optimizer = torch.optim.__dict__[network_params.optimizer](
-        identification_model.parameters(), **network_params.optim_args
-    )
+    logging.info(f"Setting {network_params.optimizer} optimizer")
+    if network_params.optimizer == "Adam":
+        optimizer = torch.optim.Adam(
+            identification_model.parameters(), **network_params.optim_args
+        )
+    elif network_params.optimizer == "SGD":
+        optimizer = torch.optim.SGD(
+            identification_model.parameters(), **network_params.optim_args
+        )
+    else:
+        raise AttributeError(network_params.optimizer)
 
     # Set scheduler
     logging.info("Setting scheduler")
     scheduler = MultiStepLR(optimizer, milestones=network_params.schedule, gamma=0.1)
 
-    # Set learner
-    logging.info("Setting the learner")
-    learner = learner_class(identification_model, criterion, optimizer, scheduler)
-
-    # Set stopping criteria
-    logging.info("Setting the stopping criteria")
-    # set criteria to stop the training
+    learner = LearnerClassification(
+        identification_model, criterion, optimizer, scheduler
+    )
+
     stop_training = StopTraining(
         network_params.number_of_classes,
-        check_for_loss_plateau=True,
-        first_accumulation_flag=video is None or video.accumulation_step == 0,
+        is_first_accumulation=video.accumulation_step == 0,
     )
 
+    # keep a copy of the penultimate model
+    network_params.penultimate_model_path.unlink(missing_ok=True)
+    if network_params.model_path.is_file():
+        copyfile(network_params.model_path, network_params.penultimate_model_path)
+
     TrainIdentification(
-        learner,
-        train_loader,
-        val_loader,
-        network_params,
-        stop_training,
-        accumulation_manager=accumulation_manager,
+        learner, train_loader, val_loader, network_params, stop_training
     )
-    logging.info("Identification network trained")
 
+    accumulation_manager.update_fragments_used_for_training()
     accumulation_manager.update_used_images_and_labels()
     accumulation_manager.assign_identities_to_fragments_used_for_training()
     accumulation_manager.update_list_of_individual_fragments_used()
 
     # compute ratio of accumulated images and stop if it is above random
     accumulation_manager.ratio_accumulated_images = (
         accumulation_manager.list_of_fragments.compute_ratio_of_images_used_for_training()
     )
 
     if (
         accumulation_manager.ratio_accumulated_images
         > conf.THRESHOLD_EARLY_STOP_ACCUMULATION
     ):
         logging.debug("Stopping accumulation by early stopping criteria")
-        return accumulation_manager.ratio_accumulated_images
+        return
 
     # Set accumulation parameters for rest of the accumulation
     # take images from global fragments not used in training (in the remainder test global fragments)
     if any(
         not global_fragment.used_for_training
         for global_fragment in accumulation_manager.list_of_global_fragments.global_fragments
     ):
@@ -158,15 +161,15 @@
             softmax_probs,
             indices_to_split,
             candidate_individual_fragments_identifiers,
         ) = get_predictions_of_candidates_fragments(
             identification_model,
             video.id_images_file_paths,
             network_params,
-            accumulation_manager.list_of_fragments.fragments,
+            accumulation_manager.list_of_fragments,
         )
 
         accumulation_manager.split_predictions_after_network_assignment(
             predictions,
             softmax_probs,
             indices_to_split,
             candidate_individual_fragments_identifiers,
@@ -210,18 +213,16 @@
                 for global_fragment in accumulation_manager.list_of_global_fragments.global_fragments
             )
         )
         stats["ratio_of_accumulated_images"].append(
             accumulation_manager.ratio_accumulated_images
         )
 
-        accumulation_manager.update_counter()
+        accumulation_manager.current_step += 1
 
     accumulation_manager.ratio_accumulated_images = (
         accumulation_manager.list_of_fragments.compute_ratio_of_images_used_for_training()
     )
 
     video.accumulation_statistics_data[video.accumulation_trial] = (
         video.accumulation_statistics
     )
-
-    return accumulation_manager.ratio_accumulated_images
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/dataset/identification_dataset.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/dataset/identification_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,32 +32,29 @@
 from torchvision.datasets.folder import VisionDataset
 
 from idtrackerai.utils import conf
 
 
 class IdentificationDataset(VisionDataset):
     def __init__(self, data_dict, scope, transform=None):
-        super().__init__(data_dict, transform=transform)  # TODO this is wrong
+        super().__init__("", transform=transform)
         self.scope = scope
         self.images = data_dict["images"]
         if self.scope in ("training", "validation", "test"):
             self.labels = data_dict["labels"]
         else:
             self.labels = np.zeros((self.images.shape[0]))
         self.get_data()
 
     def get_data(self):
         if self.images.ndim <= 3:
             self.images = np.expand_dims(np.asarray(self.images), axis=-1)
 
         if self.scope == "training":
             self.images, self.labels = duplicate_PCA_images(self.images, self.labels)
-            self.images, self.labels = shuffle_images_and_labels(
-                self.images, self.labels
-            )
 
     def __len__(self):
         return len(self.images)
 
     def __getitem__(self, index):
         image = self.images[index]
         target = self.labels[index]
@@ -88,27 +85,25 @@
     validation_dataset : <DataSet object>
         Object containing the images and labels for validation
 
     See Also
     --------
     :class:`get_data.DataSet`
     :func:`get_data.duplicate_PCA_images`
-    :func:`get_data.shuffle_images_and_labels`
     """
 
     if validation_proportion is None:
         validation_proportion = conf.VALIDATION_PROPORTION
 
     # Init variables
     train_images = []
     train_labels = []
     validation_images = []
     validation_labels = []
 
-    images, labels = shuffle_images_and_labels(images, labels)
     for i in np.unique(labels):
         # Get images of this individual
         this_indiv_images = images[labels == i]
         this_indiv_labels = labels[labels == i]
         # Compute number of images for training and validation
         num_images = len(this_indiv_labels)
         num_images_validation = np.ceil(validation_proportion * num_images).astype(int)
@@ -134,24 +129,14 @@
         "labels": train_labels,
         "weights": training_weights,
     }
     val_dict = {"images": validation_images, "labels": validation_labels}
     return train_dict, val_dict
 
 
-def shuffle_images_and_labels(images, labels):
-    """Shuffles images and labels with a random
-    permutation, according to the number of examples"""
-    np.random.seed(0)
-    perm = np.random.permutation(len(labels))
-    images = images[perm]
-    labels = labels[perm]
-    return images, labels
-
-
 def duplicate_PCA_images(training_images, training_labels):
     """Creates a copy of every image in `training_images` by rotating 180 degrees
 
     Parameters
     ----------
     training_images : ndarray
         Array of shape [number of images, height, width, channels] containing
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/identity_transfer.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/identity_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 from .assigner import compute_identification_statistics_for_non_accumulated_fragments
 from .network.get_predictions import get_predictions_identities
 
 
 def identify_first_global_fragment_for_accumulation(
     first_global_fragment_for_accumulation: GlobalFragment,
     video: Video,
-    identification_model: Module,
+    identification_model: Module | None,
     network_params: NetworkParams,
     knowledge_transfer_info_dict: dict,
 ):
-    if video.identity_transfer:
+    if (
+        identification_model is not None and video.identity_transfer
+    ):  # identity transfer
         logging.info(f"Transferring identities from {video.knowledge_transfer_folder}")
         identities = get_transferred_identities(
             first_global_fragment_for_accumulation,
             video,
             identification_model,
             network_params,
             knowledge_transfer_info_dict,
@@ -61,25 +63,25 @@
     ):
         fragment.acceptable_for_training = True
         fragment.temporary_id = id
         frequencies = np.zeros(video.number_of_animals)
         frequencies[id] = fragment.number_of_images
         fragment.is_certain = True
         fragment.certainty = 1.0
-        fragment.set_P1_from_frequencies(frequencies)
+        fragment.P1_vector = fragment.compute_P1_from_frequencies(frequencies)
 
 
 def get_transferred_identities(
     first_global_fragment_for_accumulation: GlobalFragment,
     video: Video,
     identification_model: Module,
     network_params: NetworkParams,
     knowledge_transfer_info_dict: dict,
 ) -> list | None:
-    (images, _) = first_global_fragment_for_accumulation.get_images_and_labels(
+    images, _ = first_global_fragment_for_accumulation.get_images_and_labels(
         video.id_images_file_paths
     )
 
     predictions, softmax_probs = get_predictions_identities(
         identification_model, images, network_params
     )
 
@@ -126,15 +128,15 @@
             logging.error("The computed identities are not consistent")
             return None
         P1_array = set_fragment_temporary_id(
             fragment, temporary_id, P1_array, fragment_indx
         )
 
     # Check if the global fragment is unique after assigning the identities
-    if not first_global_fragment_for_accumulation.is_unique:
+    if not first_global_fragment_for_accumulation.is_unique(video.number_of_animals):
         logging.error("The computed identities are not unique")
         return None
 
     if video.number_of_animals != knowledge_transfer_info_dict["number_of_classes"]:
         logging.error(
             "The number of animals in the current video and the one "
             "transferring identities from are not the same"
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/network/get_predictions.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/network/get_predictions.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 import torch
 from torch.backends import cudnn
 
 from idtrackerai.network import NetworkParams
 from idtrackerai.tracker.dataset.identification_dataloader import get_test_data_loader
+from idtrackerai.utils import track
 
 
 def get_predictions_identities(
     model: torch.nn.Module, images: np.ndarray, network_params: NetworkParams
 ):
     logging.debug("Generating prediction data set with %d images", len(images))
     loader = get_test_data_loader({"images": images}, network_params.number_of_classes)
@@ -22,22 +23,22 @@
         logging.info(
             'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
         )
         cudnn.benchmark = True  # make it train faster
         model = model.cuda()
 
     model.eval()
-    for input_, _target in loader:
+    for input_, _target in track(loader, "Predicting identities"):
         # Prepare the inputs
         if network_params.use_gpu:
             with torch.no_grad():
                 input_ = input_.cuda()
 
         # Inference
         with torch.no_grad():
-            softmax = model.softmax_probs(input_)
+            softmax = model.softmax_probs(input_)  # type: ignore
             pred = softmax.argmax(1)  # find the predicted class
 
             predictions.extend(pred.cpu().numpy())
             softmax_probs.extend(softmax.cpu().numpy())
 
     return np.asarray(predictions) + 1, np.asarray(softmax_probs)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/network/stop_training_criteria.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/network/stop_training_criteria.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 # [1] Romero-Ferrero, F., Bergomi, M.G., Hinz, R.C., Heras, F.J.H.,
 # de Polavieja, G.G., Nature Methods, 2019.
 # idtracker.ai: tracking all individuals in small or large collectives of
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
-
 import logging
 import sys
 
 import numpy as np
 from rich.status import Status
 
 from idtrackerai.utils import conf
@@ -48,59 +47,36 @@
         Number of epochs before starting the training
     number_of_animals : int
         Number of animals in the video
     epochs_before_checking_stopping_conditions : int
         Number of epochs before starting to check the stopping conditions
     overfitting_counter : int
         Counts the number of consecutive overfitting epochs during training
-    check_for_loss_plateau : bool
-        Flag to check for a plateu in the loss of the validation
     first_accumulation_flag : bool
         Flag to indicate that it is the first step of the accumulation
 
     """
 
-    conf_variables = [
-        "MAXIMUM_NUMBER_OF_EPOCHS_IDCNN",
-        "OVERFITTING_COUNTER_THRESHOLD_IDCNN",
-        "OVERFITTING_COUNTER_THRESHOLD_IDCNN_FIRST_ACCUM",
-        "LEARNING_PERCENTAGE_DIFFERENCE_1_IDCNN",
-        "LEARNING_PERCENTAGE_DIFFERENCE_2_IDCNN",
-    ]
+    epochs_before_checking_stopping_conditions = 10
 
-    def __init__(
-        self,
-        number_of_animals,
-        epochs_before_checking_stopping_conditions=10,
-        check_for_loss_plateau=True,
-        first_accumulation_flag=False,
-        conf_dict=None,
-    ):
-        self.conf_dict = self.get_conf_dict(conf_dict)
-        self.num_epochs = self.conf_dict[
-            "MAXIMUM_NUMBER_OF_EPOCHS_IDCNN"
-        ]  # maximal num of epochs
+    def __init__(self, number_of_animals: int, is_first_accumulation: bool = False):
+        logging.info("Setting the stopping criteria", stacklevel=3)
+        self.num_epochs = conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN
         self.number_of_animals = number_of_animals
-        self.epochs_before_checking_stopping_conditions = (
-            epochs_before_checking_stopping_conditions
-        )
         # number of epochs in which the network is overfitting
         # before stopping the training
         self.overfitting_counter = 0
-        # bool: if true the training is stopped if the loss
-        # is not decreasing enough
-        self.check_for_loss_plateau = check_for_loss_plateau
-        self.first_accumulation_flag = first_accumulation_flag
+        self.is_first_accumulation = is_first_accumulation
         self.epochs_completed = -1
 
     def __call__(
         self,
-        loss_training: list,
+        loss_training: float,
         loss_validation: list,
-        accuracy_validation: list,
+        accuracy_validation: float,
         status: Status,
     ):
         """Returns True when one of the conditions to stop the training is
         satisfied, otherwise it returns False
 
         Parameters
         ----------
@@ -114,15 +90,15 @@
             Number of epochs completed before checking the conditions
 
         """
         # check that the model did not diverged (nan loss).
         self.epochs_completed += 1
 
         if self.epochs_completed > 0 and (
-            np.isnan(loss_training[-1]) or np.isnan(loss_validation[-1])
+            np.isnan(loss_training) or np.isnan(loss_validation[-1])
         ):
             status.stop()
             logging.error(
                 "The model diverged. Oops. Check the hyperparameters and "
                 "the architecture of the network."
             )
             return True
@@ -131,93 +107,81 @@
             status.stop()
             logging.warning(
                 "The number of epochs completed is larger than the number "
                 "of epochs set for training, we stop the training"
             )
             return True
 
+        if self.epochs_completed <= self.epochs_before_checking_stopping_conditions:
+            return False
+
         # check that the model is not overfitting or if it reached
         # a stable saddle (minimum)
-        if self.epochs_completed > self.epochs_before_checking_stopping_conditions:
-            current_loss = loss_validation[-1]
-            previous_loss = np.nanmean(
-                loss_validation[-self.epochs_before_checking_stopping_conditions : -1]
-            )
+        current_loss = loss_validation[-1]
+        previous_loss = np.nanmean(
+            loss_validation[-self.epochs_before_checking_stopping_conditions : -1]
+        )
 
-            # The validation loss in the first 10 epochs could have exploded
-            # but being decreasing.
-            if np.isnan(previous_loss):
-                previous_loss = sys.float_info[0]
-            losses_difference = previous_loss - current_loss
-
-            # check overfitting
-            if losses_difference < 0.0:
-                self.overfitting_counter += 1
-                if (
-                    self.overfitting_counter
-                    >= self.conf_dict["OVERFITTING_COUNTER_THRESHOLD_IDCNN"]
-                    and not self.first_accumulation_flag
-                ):
-                    status.stop()
-                    logging.info("Overfitting")
-                    return True
-                if (
-                    self.first_accumulation_flag
-                    and self.overfitting_counter
-                    > self.conf_dict["OVERFITTING_COUNTER_THRESHOLD_IDCNN_FIRST_ACCUM"]
-                ):
-                    # logging.info(f"Overfitting counter, {self.overfitting_counter}")
-                    status.stop()
-                    logging.info("Overfitting first accumulation")
-                    return True
-            else:
-                self.overfitting_counter = 0
-
-            # check if the error is not decreasing much
-            if self.check_for_loss_plateau:
-                if self.first_accumulation_flag and np.abs(
-                    losses_difference
-                ) < self.conf_dict["LEARNING_PERCENTAGE_DIFFERENCE_1_IDCNN"] * 10 ** (
-                    int(np.log10(current_loss)) - 1
-                ):
-                    status.stop()
-                    logging.info(
-                        "The losses difference is very small, we stop the training"
-                    )
-                    return True
-                if np.abs(losses_difference) < self.conf_dict[
-                    "LEARNING_PERCENTAGE_DIFFERENCE_2_IDCNN"
-                ] * 10 ** (int(np.log10(current_loss)) - 1):
-                    status.stop()
-                    logging.info(
-                        "The losses difference is very small, we stop the training"
-                    )
-                    return True
-
-            # if the individual accuracies in validation are 1.
-            # for all the animals
-            if accuracy_validation[-1] == 1.0:
+        # The validation loss in the first 10 epochs could have exploded
+        # but being decreasing.
+        if np.isnan(previous_loss):
+            previous_loss = sys.float_info[0]
+        losses_difference = previous_loss - current_loss
+
+        # check overfitting
+        if losses_difference < 0.0:
+            self.overfitting_counter += 1
+            if (
+                not self.is_first_accumulation
+                and self.overfitting_counter >= conf.OVERFITTING_COUNTER_THRESHOLD_IDCNN
+            ):
                 status.stop()
-                logging.info(
-                    "The individual accuracies in validation is 100% for "
-                    "all the individuals, we stop the training"
-                )
+                logging.info("Overfitting")
                 return True
-
-            # if the validation loss is 0.
-            if previous_loss == 0.0 or current_loss == 0.0:
+            if (
+                self.is_first_accumulation
+                and self.overfitting_counter
+                > conf.OVERFITTING_COUNTER_THRESHOLD_IDCNN_FIRST_ACCUM
+            ):
+                # logging.info(f"Overfitting counter, {self.overfitting_counter}")
                 status.stop()
-                logging.info("The validation loss is 0.0, we stop the training")
+                logging.info("Overfitting first accumulation")
                 return True
+        else:
+            self.overfitting_counter = 0
 
-        return False
+        # check if the error is not decreasing much
+
+        if self.is_first_accumulation and np.abs(
+            losses_difference
+        ) < conf.LEARNING_PERCENTAGE_DIFFERENCE_1_IDCNN * 10 ** (
+            int(np.log10(current_loss)) - 1
+        ):
+            status.stop()
+            logging.info("The losses difference is very small, we stop the training")
+            return True
+        if np.abs(
+            losses_difference
+        ) < conf.LEARNING_PERCENTAGE_DIFFERENCE_2_IDCNN * 10 ** (
+            int(np.log10(current_loss)) - 1
+        ):
+            status.stop()
+            logging.info("The losses difference is very small, we stop the training")
+            return True
+
+        # if the individual accuracies in validation are 1.
+        # for all the animals
+        if accuracy_validation == 1.0:
+            status.stop()
+            logging.info(
+                "The individual accuracies in validation is 100% for "
+                "all the individuals, we stop the training"
+            )
+            return True
+
+        # if the validation loss is 0.
+        if previous_loss == 0.0 or current_loss == 0.0:
+            status.stop()
+            logging.info("The validation loss is 0.0, we stop the training")
+            return True
 
-    def get_conf_dict(self, conf_dict):
-        if conf_dict is not None:
-            # Check that the conf_dict has the variables needed
-            for conf_variable in self.conf_variables:
-                if conf_variable not in conf_dict.keys():
-                    raise Exception(
-                        f"The conf_variable {conf_variable} is not in the conf_dict"
-                    )
-            return conf_dict
-        return {conf_var: getattr(conf, conf_var) for conf_var in self.conf_variables}
+        return False
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/pre_trainer.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/pre_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import logging
 
 import torch
-from torch import nn
 from torch.backends import cudnn
+from torch.nn import CrossEntropyLoss, Module
 from torch.optim.lr_scheduler import MultiStepLR
 
 from idtrackerai import GlobalFragment, ListOfFragments
 from idtrackerai.network import LearnerClassification, NetworkParams, fc_weights_reinit
 from idtrackerai.utils import conf
 
 from .dataset.identification_dataloader import get_training_data_loaders
@@ -44,16 +44,15 @@
 from .network.stop_training_criteria import StopTraining
 from .network.trainer import TrainIdentification
 
 
 def pre_train_global_fragment(
     number_of_animals: int,
     accumulation_step: int,
-    identification_model: nn.Module,
-    learner_class: type[LearnerClassification],
+    identification_model: Module,
     network_params: NetworkParams,
     pretraining_global_fragment: GlobalFragment,
     list_of_fragments: ListOfFragments,
 ):
     """Performs pretraining on a single global fragments
 
     Parameters
@@ -62,18 +61,14 @@
         an instance of the class :class:`~idCNN.ConvNetwork`
     pretraining_global_fragment : <GlobalFragment object>
         an instance of the class :class:`~globalfragment.GlobalFragment`
     list_of_fragments : <ListOfFragments object>
         an instance of the class :class:`~list_of_fragments.ListOfFragments`
     global_epoch : int
         global counter of the training epoch in pretraining
-    check_for_loss_plateau : bool
-        if True the stopping criteria (see :mod:`~stop_training_criteria`) will
-        automatically stop the training in case the loss functin computed for
-        the validation set of images reaches a plateau
     store_accuracy_and_error : bool
         if True the values of the loss function, accuracy and individual
         accuracy will be stored
     save_summaries : bool
         if True tensorflow summaries will be generated and stored to allow
         tensorboard visualisation of both loss and activity histograms
     store_training_accuracy_and_loss_data : <Store_Accuracy_and_Loss object>
@@ -113,59 +108,56 @@
     # Set data loaders
     train_loader, val_loader = get_training_data_loaders(
         number_of_animals, train_data, val_data
     )
 
     # Set criterion
     logging.info("Setting training criterion")
-    criterion = nn.CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
+    criterion = CrossEntropyLoss(weight=torch.tensor(train_data["weights"]))
 
     # Re-initialize fully-connected layers
     identification_model.apply(fc_weights_reinit)
 
     # Send model and criterion to GPU
     if network_params.use_gpu:
         torch.cuda.set_device(0)
         logging.info(
             'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
         )
         cudnn.benchmark = True  # make it train faster
         identification_model = identification_model.cuda()
         criterion = criterion.cuda()
 
-    # Set optimizer
-    logging.info("Setting optimizer")
-    optimizer = torch.optim.__dict__[network_params.optimizer](
-        identification_model.parameters(), **network_params.optim_args
-    )
-
+    logging.info(f"Setting {network_params.optimizer} optimizer")
+    if network_params.optimizer == "Adam":
+        optimizer = torch.optim.Adam(
+            identification_model.parameters(), **network_params.optim_args
+        )
+    elif network_params.optimizer == "SGD":
+        optimizer = torch.optim.SGD(
+            identification_model.parameters(), **network_params.optim_args
+        )
+    else:
+        raise AttributeError(network_params.optimizer)
     # Set scheduler
     logging.info("Setting scheduler")
     scheduler = MultiStepLR(optimizer, milestones=network_params.schedule, gamma=0.1)
 
-    # Set learner
-    logging.info("Setting the learner")
-    learner = learner_class(identification_model, criterion, optimizer, scheduler)
-
-    # Set stopping criteria
-    logging.info("Setting the stopping criteria")
-    # set criteria to stop the training
+    learner = LearnerClassification(
+        identification_model, criterion, optimizer, scheduler
+    )
+
     stop_training = StopTraining(
-        network_params.number_of_classes,
-        check_for_loss_plateau=True,
-        first_accumulation_flag=accumulation_step == 0,
+        network_params.number_of_classes, is_first_accumulation=accumulation_step == 0
     )
 
-    logging.info("Training identification network")
-    best_model_path = TrainIdentification(
+    TrainIdentification(
         learner, train_loader, val_loader, network_params, stop_training
     )
 
-    logging.info("Identification network trained")
-
     for fragment in pretraining_global_fragment.individual_fragments:
         fragment.used_for_pretraining = True
 
     ratio_of_pretrained_images = (
         list_of_fragments.compute_ratio_of_images_used_for_pretraining()
     )
     logging.debug(
@@ -174,9 +166,9 @@
         f"{conf.MAX_RATIO_OF_PRETRAINED_IMAGES:.2%} we stop pretraining)"
     )
 
     return (
         identification_model,
         ratio_of_pretrained_images,
         list_of_fragments,
-        best_model_path,
+        network_params.model_path,
     )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/tracker/tracker.py` & `idtrackerai-5.1.4/src/idtrackerai/tracker/tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 from .accumulator import perform_one_accumulation_step
 from .assigner import assign_remaining_fragments
 from .identity_transfer import identify_first_global_fragment_for_accumulation
 from .pre_trainer import pre_train_global_fragment
 
 
 class TrackerAPI:
+    identification_model: torch.nn.Module
+
     def __init__(
         self,
         video: Video,
         list_of_blobs: ListOfBlobs,
         list_of_fragments: ListOfFragments,
         list_of_global_fragments: ListOfGlobalFragments,
     ):
@@ -81,48 +83,34 @@
             self.knowledge_transfer_info_dict = {}
 
         # Old requirements for restoring
         self.processes_to_restore = {}
 
         self.accumulation_network_params: NetworkParams
         self.restoring_first_accumulation = False  # Flag restores first accumulation
-        self.accumulation_step_finished = False  # Flag accumulation step finished
 
     def track_single_animal(self):
         logging.debug("Assigning identity 1 to all blobs")
-        for bf in self.list_of_blobs.blobs_in_video:
-            for blob in bf:
-                blob.identity = 1
-                blob.P2_vector = [1.0]
+        for blob in self.list_of_blobs.all_blobs:
+            blob.identity = 1
 
     def track_single_global_fragment_video(self):
         logging.info("TRACKING SINGLE GLOBAL FRAGMENT")
 
-        def get_P2_vector(identity, number_of_animals):
-            P2_vector = np.zeros(number_of_animals)
-            P2_vector[identity - 1] = 1.0
-            return P2_vector
-
         fragment_identifier_to_id = {}
         identity = 1
         for fragment in self.list_of_fragments.fragments:
             if fragment.is_an_individual:
                 fragment_identifier_to_id[fragment.identifier] = identity
                 identity += 1
             else:
                 fragment_identifier_to_id[fragment.identifier] = None
 
-        for bf in self.list_of_blobs.blobs_in_video:
-            for b in bf:
-                if b.is_an_individual:
-                    b.identity = fragment_identifier_to_id[b.fragment_identifier]
-                    b.P2_vector = get_P2_vector(
-                        fragment_identifier_to_id[b.fragment_identifier],
-                        self.video.number_of_animals,
-                    )
+        for blob in (b for b in self.list_of_blobs.all_blobs if b.is_an_individual):
+            blob.identity = fragment_identifier_to_id[blob.fragment_identifier]
         self.video.first_frame_first_global_fragment = [0]  # in case
 
     def track_with_identities(self) -> ListOfFragments:
         """In protocol 3, list_of_fragments is loaded from accumulation
         folders so the reference from outside tracker_API is lost.
         That's why list_of_fragments has to be returned"""
         self.video.tracking_timer.start()
@@ -200,15 +188,15 @@
             #
             # self.create_trajectories()
 
         if self.processes_to_restore.get("protocol3_pretraining"):
             # TODO: bring restoring back to life
             raise NotImplementedError
             # logging.info("Restoring pretraining")
-            # logging.info("Initialising pretraining network")
+            # logging.info("Initializing pretraining network")
             # self.init_pretraining_net()
             # logging.info("Restoring pretraining")
             # self.accumulation_step_finished = True
             # self.restore_first_accumulation()
             # self.restore_pretraining()
             # self.accumulation_manager.ratio_accumulated_images =
             # self.video.percentage_of_accumulated_images[0]
@@ -253,43 +241,35 @@
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.accumulation_folder,
             knowledge_transfer_folder=self.video.knowledge_transfer_folder,
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
-            loss="CE",
             use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
             optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
-            apply_mask=False,
-            dataset="supervised",
-            skip_eval=False,
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
             return_store_objects=False,
         )
         # Save network params
         self.accumulation_network_params.save()
 
     def protocol1(self):
         self.video.protocol1_timer.start()
 
         # reset list of fragments and global fragments to fragmentation
         self.list_of_fragments.reset(roll_back_to="fragmentation")
-        self.list_of_global_fragments.reset(roll_back_to="fragmentation")
 
-        # Initialize idCNN
-        logging.info("Setting learner class")
-        self.learner_class = LearnerClassification
         logging.info("Creating idCNN")
         if self.video.knowledge_transfer_folder:
             try:
-                self.identification_model = self.learner_class.load_model(
-                    self.accumulation_network_params, scope="knowledge_transfer"
+                self.identification_model = LearnerClassification.load_model(
+                    self.accumulation_network_params, knowledge_transfer=True
                 )
                 logging.info("Tracking with knowledge transfer")
                 if not self.video.identity_transfer:
                     logging.info("Reinitializing fully connected layers")
                     self.identification_model.apply(fc_weights_reinit)
                 else:
                     logging.info(
@@ -298,21 +278,20 @@
                     )
             except RuntimeError:
                 logging.error(
                     f"Could not load model {self.accumulation_network_params} to"
                     " transfer knowledge, following without knowledge nor identity"
                     " transfer"
                 )
-                self.learner_class = LearnerClassification
-                self.identification_model = self.learner_class.create_model(
+                self.identification_model = LearnerClassification.create_model(
                     self.accumulation_network_params
                 )
                 self.identification_model.apply(weights_xavier_init)
         else:
-            self.identification_model = self.learner_class.create_model(
+            self.identification_model = LearnerClassification.create_model(
                 self.accumulation_network_params
             )
             self.identification_model.apply(weights_xavier_init)
 
         # Set first global fragment to start accumulation.
         # The network is passed in case of identity transfer.
         logging.info("Setting first global fragment for accumulation")
@@ -347,76 +326,71 @@
             self.video.number_of_animals,
             self.list_of_fragments,
             self.list_of_global_fragments,
         )
 
         # Selecting the first global fragment is considered as
         # the 0 accumulation step
-        self.accumulation_step_finished = True
-        self.init_and_accumulate()
-
-    def one_shot_accumulation(self):
-        self.accumulation_step_finished = False
-        assert self.identification_model is not None
-        self.accumulation_manager.ratio_accumulated_images = (
-            perform_one_accumulation_step(
-                self.accumulation_manager,
-                self.video,
-                self.identification_model,
-                self.learner_class,
-                network_params=self.accumulation_network_params,
-            )
-        )
-        self.accumulation_step_finished = True
+        self.video.init_accumulation_statistics_attributes()
+        self.accumulate()
 
     def accumulate(self):
-        new_global_fragments_for_training = (
-            self.accumulation_manager.new_global_fragments_for_training
-        )
-        if self.accumulation_step_finished and new_global_fragments_for_training:
+        logging.info("Entering accumulation loop")
+        if self.accumulation_manager.new_global_fragments_for_training:
             # Training and identification continues
             if (
-                self.accumulation_manager.counter == 1
+                self.accumulation_manager.current_step == 1
                 and self.video.accumulation_trial == 0
             ):
                 # first training finished
                 self.video.protocol1_timer.finish()
                 self.video.protocol2_timer.start()
 
             # Training and identification step
-            self.one_shot_accumulation()
+            perform_one_accumulation_step(
+                self.accumulation_manager,
+                self.video,
+                self.identification_model,
+                self.accumulation_network_params,
+            )
             # Re-enter the function for the next step of the accumulation
             self.accumulate()
 
         elif (
-            not new_global_fragments_for_training
-            and not self.video.protocol2_timer.finished
+            not self.video.protocol2_timer.finished
             and self.accumulation_manager.ratio_accumulated_images
             > conf.THRESHOLD_EARLY_STOP_ACCUMULATION
         ):
             # Accumulation stop because protocol 1 is successful
             self.save_after_first_accumulation()
             self.video.protocol1_timer.finish()
             logging.info("Protocol 1 successful")
-            self.identify()
+            assign_remaining_fragments(
+                self.list_of_fragments,
+                self.identification_model,
+                self.accumulation_network_params,
+                self.video.identify_timer,
+            )
 
-        elif (
-            not new_global_fragments_for_training
-            and not self.video.protocol3_pretraining_timer.finished
-        ):
-            logging.info("--------------------> No more new global fragments")
+        elif not self.video.protocol3_pretraining_timer.finished:
+            logging.info("No more new global fragments")
             self.save_after_first_accumulation()
 
             if (
                 self.accumulation_manager.ratio_accumulated_images
                 >= conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
             ):
                 self.video.protocol2_timer.finish()
                 logging.info("Protocol 2 successful")
-                self.identify()
+                assign_remaining_fragments(
+                    self.list_of_fragments,
+                    self.identification_model,
+                    self.accumulation_network_params,
+                    self.video.identify_timer,
+                )
 
             elif (
                 self.accumulation_manager.ratio_accumulated_images
                 < conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
             ):
                 self.video.protocol1_timer.finish()
                 self.video.protocol2_timer.finish(raise_if_not_started=False)
@@ -424,70 +398,58 @@
                     "[red]Protocol 2 failed, protocol 3 is going to start",
                     extra={"markup": True},
                 )
                 ask_about_protocol3(
                     self.video.protocol3_action, self.video.number_of_error_frames
                 )
 
-                logging.warning("Going to start protocol 3")
                 self.video.protocol3_pretraining_timer.start()
 
                 self.pretraining_counter = 0
                 self.protocol3()
 
         elif (
             self.video.protocol3_pretraining_timer.finished
             and self.video.accumulation_trial
             < conf.MAXIMUM_NUMBER_OF_PARACHUTE_ACCUMULATIONS
             and self.accumulation_manager.ratio_accumulated_images
             < conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
         ):
-            logging.info(
-                "--------------------> Accumulation Protocol 3 failed. Opening"
-                " parachute ..."
-            )
+            logging.warning("Accumulation Protocol 3 failed. Opening parachute ...")
             if self.video.accumulation_trial == 0:
                 self.video.protocol3_accumulation_timer.start()
             self.video.accumulation_trial += 1
-            if (
-                not new_global_fragments_for_training
-                and self.video.accumulation_trial > 1
-            ):
+            if self.video.accumulation_trial > 1:
                 self.save_and_update_accumulation_parameters_in_parachute()
             self.accumulation_parachute_init(self.video.accumulation_trial)
 
-            self.init_and_accumulate()
+            self.video.init_accumulation_statistics_attributes()
+            self.accumulate()
 
         elif self.video.protocol3_pretraining_timer.finished and (
             self.accumulation_manager.ratio_accumulated_images
             >= conf.THRESHOLD_ACCEPTABLE_ACCUMULATION
             or self.video.accumulation_trial
             >= conf.MAXIMUM_NUMBER_OF_PARACHUTE_ACCUMULATIONS
         ):
             logging.info("Accumulation after protocol 3 has been successful")
             self.video.protocol3_accumulation_timer.finish()
 
             self.save_after_second_accumulation()
-            logging.info("Start residual identification")
-            self.identify()
+            assign_remaining_fragments(
+                self.list_of_fragments,
+                self.identification_model,
+                self.accumulation_network_params,
+                self.video.identify_timer,
+            )
 
         # Whether to re-enter the function for the next accumulation step
         if self.accumulation_manager.new_global_fragments_for_training:
             self.accumulate()
 
-    def init_and_accumulate(self):
-        """
-        This is called in the first step of each accumulation trial
-        :param do_accumulate:
-        :return:
-        """
-        logging.info("Entering accumulation loop")
-        self.video.init_accumulation_statistics_attributes()
-        self.accumulate()
-
     def save_after_first_accumulation(self):
         """Set flags and save data"""
         logging.info("Saving first accumulation parameters")
 
         if not self.restoring_first_accumulation:
             self.video.ratio_accumulated_images = (
                 self.accumulation_manager.ratio_accumulated_images
@@ -523,22 +485,21 @@
         self.pretraining_loop()
 
     def init_pretraining_variables(self):
         self.init_pretraining_net()
         self.ratio_of_pretrained_images = 0
 
         # Initialize network
-        self.learner_class = LearnerClassification
         if self.video.knowledge_transfer_folder:
-            self.identification_model = self.learner_class.load_model(
-                self.pretrain_network_params, scope="knowledge_transfer"
+            self.identification_model = LearnerClassification.load_model(
+                self.pretrain_network_params, knowledge_transfer=True
             )
             self.identification_model.apply(fc_weights_reinit)
         else:
-            self.identification_model = self.learner_class.create_model(
+            self.identification_model = LearnerClassification.create_model(
                 self.pretrain_network_params
             )
             self.identification_model.apply(weights_xavier_init)
 
     def init_pretraining_net(self):
         delete = not self.processes_to_restore.get("protocol3_pretraining")
         create_dir(self.video.pretraining_folder, remove_existing=delete)
@@ -546,22 +507,18 @@
         self.pretrain_network_params = NetworkParams(
             number_of_classes=self.video.number_of_animals,
             architecture=conf.IDCNN_NETWORK_NAME,
             save_folder=self.video.pretraining_folder,
             model_name="identification_network",
             image_size=self.video.id_image_size,
             scopes_layers_to_optimize=conf.LAYERS_TO_OPTIMISE_PRETRAINING,
-            loss="CE",
             use_gpu=True,
             optimizer="SGD",
             schedule=[30, 60],
             optim_args={"lr": conf.LEARNING_RATE_IDCNN_ACCUMULATION, "momentum": 0.9},
-            apply_mask=False,
-            dataset="supervised",
-            skip_eval=False,
             epochs=conf.MAXIMUM_NUMBER_OF_EPOCHS_IDCNN,
             return_store_objects=False,
         )
 
     def pretraining_loop(self):
         self.list_of_fragments.reset(roll_back_to="fragmentation")
         self.list_of_global_fragments.order_by_distance_travelled()
@@ -569,25 +526,23 @@
         self.continue_pretraining()
 
     def one_shot_pretraining(self):
         self.pretraining_step_finished = False
         self.pretraining_global_fragment = (
             self.list_of_global_fragments.global_fragments[self.pretraining_counter]
         )
-        assert self.identification_model is not None
         (
             self.identification_model,
             self.ratio_of_pretrained_images,
             self.list_of_fragments,
             self.pretrained_model_path,
         ) = pre_train_global_fragment(
             self.video.number_of_animals,
             self.video.accumulation_step,
             self.identification_model,
-            self.learner_class,
             self.pretrain_network_params,
             self.pretraining_global_fragment,
             self.list_of_fragments,
         )
         self.pretraining_counter += 1
         self.pretraining_step_finished = True
 
@@ -605,54 +560,48 @@
             logging.warning("Calling accumulate from continue_pretraining")
             self.video.protocol3_pretraining_timer.finish()
             self.accumulate()
 
     """ parachute """
 
     def accumulation_parachute_init(self, iteration_number):
-        logging.debug("------------------------> accumulation_parachute_init")
+        logging.debug("Accumulation_parachute_init")
         logging.info("Starting accumulation %i" % iteration_number)
 
         delete = not self.processes_to_restore.get("protocol3_accumulation")
 
         self.video.create_accumulation_folder(
             iteration_number=iteration_number, delete=delete
         )
         self.video.accumulation_trial = iteration_number
         self.list_of_fragments.reset(roll_back_to="fragmentation")
-        self.list_of_global_fragments.reset(roll_back_to="fragmentation")
-
-        # Initialize network
-        if self.video.identity_transfer:
-            logging.info("Load model for identity transfer")
-            self.identification_model = self.learner_class.load_model(
-                self.accumulation_network_params
-            )
-        else:
-            self.identification_model = None
 
-        logging.info("Setting first global fragment for accumulation")
         first_global_fragment = (
             self.list_of_global_fragments.set_first_global_fragment_for_accumulation(
                 accumulation_trial=iteration_number - 1
             )
         )
 
         self.video.first_frame_first_global_fragment.append(
             first_global_fragment.first_frame_of_the_core
             if first_global_fragment is not None
             else None
         )
+
         if first_global_fragment is not None:
             identify_first_global_fragment_for_accumulation(
                 first_global_fragment,
                 self.video,
-                network_params=self.accumulation_network_params,
-                identification_model=self.identification_model,
-                knowledge_transfer_info_dict=self.knowledge_transfer_info_dict,
+                (
+                    LearnerClassification.load_model(self.accumulation_network_params)
+                    if self.video.identity_transfer
+                    else None
+                ),
+                self.accumulation_network_params,
+                self.knowledge_transfer_info_dict,
             )
 
         # Sort global fragments by distance
         self.list_of_global_fragments.order_by_distance_to_the_first_global_fragment_for_accumulation(
             self.video.first_frame_first_global_fragment,
             accumulation_trial=iteration_number - 1,
         )
@@ -672,18 +621,18 @@
         self.accumulation_network_params.restore_folder = self.video.pretraining_folder
 
         # TODO: allow to train only the fully connected layers
         self.accumulation_network_params.scopes_layers_to_optimize = [
             "fully-connected1",
             "fully_connected_pre_softmax",
         ]
-        logging.info("Initialising accumulation network")
+        logging.info("Initializing accumulation network")
 
         # Load pretrained network
-        self.identification_model = self.learner_class.load_model(
+        self.identification_model = LearnerClassification.load_model(
             self.accumulation_network_params
         )
 
         # Re-initialize fully-connected layers
         self.identification_model.apply(fc_weights_reinit)
 
         # Instantiate accumualtion manager
@@ -704,15 +653,15 @@
         self.video.ratio_accumulated_images = (
             self.accumulation_manager.ratio_accumulated_images
         )
         self.video.percentage_of_accumulated_images.append(
             self.video.ratio_accumulated_images
         )
         self.list_of_fragments.save(
-            self.video.accumulation_folder / "list_of_fragments.pickle"
+            self.video.accumulation_folder / "list_of_fragments.json"
         )
 
     def save_after_second_accumulation(self):
         logging.info("Saving second accumulation parameters")
         # Save accumulation parameters
         self.save_and_update_accumulation_parameters_in_parachute()
 
@@ -725,15 +674,15 @@
         self.video.ratio_accumulated_images = (
             self.video.percentage_of_accumulated_images[self.video.accumulation_trial]
         )
         self.video.create_accumulation_folder()
 
         # Load light list of fragments with identities of the best accumulation
         self.list_of_fragments = ListOfFragments.load(
-            self.video.auto_accumulation_folder / "list_of_fragments.pickle"
+            self.video.auto_accumulation_folder / "list_of_fragments.json"
         )
 
         # Save objects
         self.list_of_fragments.save(self.video.fragments_path)
         self.list_of_global_fragments.save(self.video.global_fragments_path)
 
         # set restoring folder
@@ -741,18 +690,18 @@
         self.accumulation_network_params.restore_folder = self.video.accumulation_folder
 
         # TODO: allow to train only the fully connected layers
         self.accumulation_network_params.scopes_layers_to_optimize = [
             "fully-connected1",
             "fully_connected_pre_softmax",
         ]
-        logging.info("Initialising accumulation network")
+        logging.info("Initializing accumulation network")
 
         # Load pretrained network
-        self.identification_model = self.learner_class.load_model(
+        self.identification_model = LearnerClassification.load_model(
             self.accumulation_network_params
         )
 
         # # Re-initialize fully-connected layers
         # self.identification_model.apply(fc_weights_reinit)
 
         # Send model and criterion to GPU
@@ -762,26 +711,14 @@
                 'Sending model and criterion to GPU: "%s"', torch.cuda.get_device_name()
             )
             cudnn.benchmark = True  # make it train faster
             self.identification_model = self.identification_model.cuda()
 
         self.video.save()
 
-    """ Residual identification """
-
-    def identify(self):
-        self.video.identify_timer.start()
-        assert self.identification_model is not None
-        assign_remaining_fragments(
-            self.list_of_fragments,
-            self.identification_model,
-            self.accumulation_network_params,
-        )
-        self.video.identify_timer.finish()
-
 
 def ask_about_protocol3(protocol3_action: str, n_error_frames: int) -> None:
     """Raises a CustomError if protocol3_action is abort or aks and user answers abortion"""
     logging.info("Protocol 3 action: %s", protocol3_action)
 
     if protocol3_action == "abort":
         raise CustomError(
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/utils/__init__.py` & `idtrackerai-5.1.4/src/idtrackerai/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 from .init_logger import CustomError, initLogger, wrap_exceptions
 from .py_utils import (
     Episode,
     Timer,
     assert_all_files_exist,
     build_ROI_mask_from_list,
     check_if_identity_transfer_is_possible,
+    clean_attrs,
     create_dir,
     delete_attributes_from_object,
     get_vertices_from_label,
     json_default,
     json_object_hook,
     load_id_images,
     pprint_dict,
     remove_dir,
     remove_file,
     resolve_path,
     track,
 )
 
 __all__ = [
+    "clean_attrs",
     "wrap_exceptions",
     "check_version",
     "check_version_on_console",
     "initLogger",
     "conf",
     "CustomError",
     "Episode",
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/utils/check_PyPI_version.py` & `idtrackerai-5.1.4/src/idtrackerai/utils/check_PyPI_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return False, "Could not reach PyPI website to check for updates"
 
     if not isinstance(out_text, str) or not out_text:
         return False, "Error getting web text"
 
     # TODO maybe use from html.parser import HTMLParser?
     no_yanked_versions = "\n".join(
-        filter(lambda line: "yanked" not in line, out_text.splitlines())
+        (line for line in out_text.splitlines() if "yanked" not in line)
     )
     versions: list[tuple[str, str]] = re.findall(
         ">idtrackerai-(.+?)(.tar.gz|-py3-none-any.whl)<", no_yanked_versions
     )
 
     current_version = idtrackerai.__version__
     for version, _file_extension in versions:
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/utils/confparams.py` & `idtrackerai-5.1.4/src/idtrackerai/utils/confparams.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai/utils/init_logger.py` & `idtrackerai-5.1.4/src/idtrackerai/utils/init_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                     width=logger_width_when_no_terminal,
                 )
             ),
         ],
     )
 
     logging.getLogger("PyQt6").setLevel(logging.INFO)
-    logging.info("Welcome to idtracker.ai %s", metadata.version("idtrackerai"))
+    logging.info("Welcome to idtracker.ai")
     logging.debug(
         f"Running idtracker.ai '{metadata.version('idtrackerai')}'"
         f" on Python '{sys.version.split(' ')[0]}'\nPlatform: '{platform(True)}'"
         "\nDate: "
         + str(datetime.now()).split(".")[0]
     )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/utils/py_utils.py` & `idtrackerai-5.1.4/src/idtrackerai/utils/py_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # unmarked animals.
 # (F.R.-F. and M.G.B. contributed equally to this work.
 # Correspondence should be addressed to G.G.d.P:
 # gonzalo.polavieja@neuro.fchampalimaud.org)
 import json
 import logging
 from dataclasses import dataclass
-from datetime import datetime
+from datetime import datetime, timedelta
 from pathlib import Path
 from shutil import rmtree
 from typing import Iterable, Optional, TypeVar
 
 import cv2
 import h5py
 import numpy as np
@@ -54,53 +54,65 @@
     """A custom interpretation of rich.progress.track"""
 
     progress = Progress(
         " " * 18 + desc,
         BarColumn(bar_width=None),
         TaskProgressColumn(show_speed=True),
         TimeRemainingColumn(elapsed_when_finished=True),
+        transient=True,
     )
 
     with progress:
         yield from progress.track(sequence, total, description=desc)
 
+    task = progress.tasks[0]
+
+    logging.info(
+        "[green]%s[/] (%s iterations). It took %s",
+        desc,
+        int(task.total) if task.total is not None else "unknown",
+        "--:--" if task.elapsed is None else timedelta(seconds=int(task.elapsed)),
+        stacklevel=3,
+        extra={"markup": True},
+    )
+
 
 def delete_attributes_from_object(object_to_modify, list_of_attributes):
     for attribute in list_of_attributes:
         if hasattr(object_to_modify, attribute):
             delattr(object_to_modify, attribute)
 
 
 def create_dir(path: Path, remove_existing=False):
     if path.is_dir():
         if remove_existing:
             rmtree(path)
             path.mkdir()
-            logging.info(f"Directory {path} has been cleaned")
+            logging.info(f"Directory {path} has been cleaned", stacklevel=3)
         else:
-            logging.info(f"Directory {path} already exists")
+            logging.info(f"Directory {path} already exists", stacklevel=3)
     else:
         if not path.parent.is_dir():
             path.parent.mkdir()
         path.mkdir()
-        logging.info(f"Directory {path} has been created")
+        logging.info(f"Directory {path} has been created", stacklevel=3)
 
 
 def remove_dir(path: Path):
     if path.is_dir():
         rmtree(path, ignore_errors=True)
-        logging.info(f"Directory {path} has been removed")
+        logging.info(f"Directory {path} has been removed", stacklevel=3)
     else:
-        logging.info(f"Directory {path} not found, can't remove")
+        logging.info(f"Directory {path} not found, can't remove", stacklevel=3)
 
 
 def remove_file(path: Path):
     if path.is_file():
         path.unlink()
-        logging.info(f"File {path} has been removed")
+        logging.info(f"File {path} has been removed", stacklevel=3)
 
 
 def assert_all_files_exist(paths: list[Path]):
     """Returns FileNotFoundError if any of the paths is not an existing file"""
     for path in paths:
         if not path.is_file():
             raise FileNotFoundError(f"File {path} not found")
@@ -148,17 +160,17 @@
         list_of_ROIs = list(list_of_ROIs)
 
     for line in list_of_ROIs:
         vertices = (get_vertices_from_label(line) * resolution_reduction + 0.5).astype(
             np.int32
         )
         if line[0] == "+":
-            cv2.fillPoly(ROI_mask, [vertices][::-1], color=1)
+            cv2.fillPoly(ROI_mask, (vertices,), color=1)
         elif line[0] == "-":
-            cv2.fillPoly(ROI_mask, [vertices][::-1], color=0)
+            cv2.fillPoly(ROI_mask, (vertices,), color=0)
         else:
             raise TypeError
     return ROI_mask.astype(bool)
 
 
 @dataclass
 class Episode:
@@ -194,25 +206,29 @@
         return self.start_time is not None
 
     @property
     def finished(self):
         return self.interval is not None
 
     def start(self):
-        logging.info("[blue bold]START %s", self.name, extra={"markup": True})
+        logging.info(
+            "[blue bold]START %s", self.name, extra={"markup": True}, stacklevel=3
+        )
         self.start_time = datetime.now()
 
     def finish(self, raise_if_not_started=True):
         if not self.started and raise_if_not_started:
             raise RuntimeError("Timer finish method called before start method")
 
         self.finish_time = datetime.now()
 
         logging.info(
-            f"[blue bold]FINISH {self.name}, it took {self}", extra={"markup": True}
+            f"[blue bold]FINISH {self.name}, it took {self}",
+            extra={"markup": True},
+            stacklevel=3,
         )
 
     def __str__(self) -> str:
         return str(self.interval or "Not finished").split(".")[0]
 
     @classmethod
     def from_dict(cls, d: dict):
@@ -304,15 +320,15 @@
                 s += f",\n{' '*pad}    {repr(item)}"
             s += "]"
             text += f"\n[bold]{key:>{pad}}[/] = {s}"
     return text
 
 
 def load_id_images(
-    id_images_file_paths: list[Path], images_indices: list[tuple[int, int]]
+    id_images_file_paths: list[Path], images_indices: Iterable[tuple[int, int]]
 ) -> np.ndarray:
     """Loads the identification images from disk.
 
     Parameters
     ----------
     id_images_file_paths : list
         List of strings with the paths to the files where the images are
@@ -322,14 +338,16 @@
         to be loaded
 
     Returns
     -------
     Numpy array
         Numpy array of shape [number of images, width, height]
     """
+    if isinstance(images_indices, zip):
+        images_indices = list(images_indices)
 
     img_indices, episodes = np.asarray(images_indices).T
 
     # Create entire output array
     with h5py.File(id_images_file_paths[0], "r") as file:
         test_dataset = file["id_images"]
         images = np.empty(
@@ -346,17 +364,15 @@
 
 def json_default(obj):
     """Encodes non JSON serializable object as dicts"""
     if isinstance(obj, Path):
         return {"py/object": "Path", "path": str(obj)}
 
     if isinstance(obj, (Timer, Episode)):
-        dic = {"py/object": obj.__class__.__name__}
-        dic.update(obj.__dict__)
-        return dic
+        return {"py/object": obj.__class__.__name__} | obj.__dict__
 
     if isinstance(obj, np.integer):
         return int(obj)
 
     if isinstance(obj, np.floating):
         return float(obj)
 
@@ -388,7 +404,24 @@
             return set(d["values"])
         raise ValueError(f"Could not read {d}")
     return d
 
 
 def resolve_path(path: Path | str) -> Path:
     return Path(path).expanduser().resolve()
+
+
+def clean_attrs(obj: object):
+    """Removes instances attributes if they are redundant
+    with the class attributes"""
+    class_attr = obj.__class__.__dict__
+
+    attributes_to_remove: list[str] = [
+        attr
+        for attr, value in obj.__dict__.items()
+        if attr in class_attr
+        and type(class_attr[attr]) == type(value)
+        and class_attr[attr] == value
+    ]
+
+    for attr in attributes_to_remove:
+        delattr(obj, attr)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai/video.py` & `idtrackerai-5.1.4/src/idtrackerai/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,17 @@
     number_of_error_frames: int = -1
     """The number of frames with more blobs than animals. Set on animals_detection."""
 
     accumulation_statistics: dict[str, list]
 
     accumulation_statistics_data: list[dict[str, list]]
 
+    identities_labels: list[str] | None = None
+    """A list with a name for every identity. Defined and used in validator"""
+
     def __init__(
         self,
         video_paths: list[Path | str],
         number_of_animals,
         intensity_ths,
         area_ths,
         output_dir: Path | None,
@@ -254,22 +257,14 @@
 
         This feature was coded because some users require indicating classes
         of individuals but we do not use it in the lab."""
 
         self.setup_points: dict[str, list[tuple[float, float]]] = {}
         """Setup points"""
 
-        self.identities_labels: list[str] = list(
-            map(str, range(1, number_of_animals + 1))
-        )
-        """A list with a name for every identity. Defined ans used in validator"""
-
-        # Flag to decide which type of interpolation is done. This flag
-        # is updated when we update a blob centroid
-
         # Processes timers
         self.general_timer = Timer("Tracking session")
         self.detect_animals_timer = Timer("Animal detection")
         self.crossing_detector_timer = Timer("Crossing detection")
         self.fragmentation_timer = Timer("Fragmentation")
         self.tracking_timer = Timer("Tracking")
         self.protocol1_timer = Timer("Protocol 1")
@@ -467,21 +462,21 @@
     def idmatcher_results_path(self) -> Path:
         return self.session_folder / "matching_results"
 
     @property
     def global_fragments_path(self) -> Path:
         """get the path to save the list of global fragments after
         fragmentation"""
-        return self.preprocessing_folder / "list_of_global_fragments.pickle"
+        return self.preprocessing_folder / "list_of_global_fragments.json"
 
     @property
     def fragments_path(self) -> Path:
         """get the path to save the list of global fragments after
         fragmentation"""
-        return self.preprocessing_folder / "list_of_fragments.pickle"
+        return self.preprocessing_folder / "list_of_fragments.json"
 
     @property
     def path_to_video_object(self) -> Path:
         return self.session_folder / "video_object.json"
 
     @property
     def ground_truth_path(self) -> Path:
@@ -528,15 +523,15 @@
             with open(path, "r", encoding="utf_8") as file:
                 video_dict = json.load(file, object_hook=json_object_hook)
 
         video = cls.__new__(cls)
         video.__dict__.update(video_dict)
         video.update_paths(path.parent, video_paths_dir)
         try:
-            (_, _, _, video.episodes) = video.get_processing_episodes(
+            _, _, _, video.episodes = video.get_processing_episodes(
                 video.video_paths, video.frames_per_episode, video.tracking_intervals
             )
         except AttributeError:
             logging.warning(
                 "Could not load video episodes probably due to loading an old version"
                 " session"
             )
@@ -572,17 +567,14 @@
         ]
         _dict["resolution_reduction"] = _dict["_user_defined_parameters"][
             "resolution_reduction"
         ]
         _dict["track_wo_identities"] = _dict["_user_defined_parameters"][
             "track_wo_identification"
         ]
-        _dict["identities_labels"] = list(
-            map(str, range(1, _dict["number_of_animals"] + 1))
-        )
         _dict["accumulation_folder"] = (
             path.parent / Path(_dict.pop("_accumulation_folder")).name
         )
         _dict["_user_defined_parameters"].pop("mask")
         return _dict
 
     def update_paths(
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai.egg-info/PKG-INFO` & `idtrackerai-5.1.4/src/idtrackerai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idtrackerai
-Version: 5.1.3
+Version: 5.1.4
 Summary: Idtracker.ai tracks up to 100 unmarked animals from videos recorded in laboratory conditions using artificial intelligence. Free and open source.
 Author: Francisco Romero Ferrero, Mattia G. Bergomi, Francisco J.H. Heras, Ricardo Ribeiro
 Author-email: Jordi Torrents <jordi.torrentsm@gmail.com>
 Project-URL: Homepage, https://idtracker.ai/
 Project-URL: Repository, https://gitlab.com/polavieja_lab/idtrackerai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -36,12 +36,12 @@
 
 ``` bash
 pip install git+https://gitlab.com/polavieja_lab/idtrackerai[dev,docs]
 ```
 
 ## Contributors
 * Jordi Torrents (2022-)
-* Antonio Ortega (2021-)
+* Antonio Ortega (2021-2023)
 * Francisco Romero-Ferrero (2015-2022)
 * Mattia G. Bergomi (2015-2018)
 * Ricardo Ribeiro (2018-2020)
 * Francisco J.H. Heras (2015-2022)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai.egg-info/SOURCES.txt` & `idtrackerai-5.1.4/src/idtrackerai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -111,13 +111,14 @@
 src/idtrackerai_validator/validation_GUI.py
 src/idtrackerai_validator/validator_widgets/__init__.py
 src/idtrackerai_validator/validator_widgets/additional_info.py
 src/idtrackerai_validator/validator_widgets/errors_explorer.py
 src/idtrackerai_validator/validator_widgets/id_groups.py
 src/idtrackerai_validator/validator_widgets/id_labels.py
 src/idtrackerai_validator/validator_widgets/interpolator.py
+src/idtrackerai_validator/validator_widgets/mark_properties.py
 src/idtrackerai_validator/validator_widgets/paint_blobs.py
 src/idtrackerai_validator/validator_widgets/setup_points.py
 src/idtrackerai_video/__init__.py
 src/idtrackerai_video/general_video.py
 src/idtrackerai_video/individual_videos.py
 src/idtrackerai_video/main.py
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/GUI_main_base.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/GUI_main_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,35 @@
         self.setStyleSheet("QToolTip { color: black;}")
 
         self.auto_check_updates = AutoCheckUpdatesThread()
         self.auto_check_updates.out_of_date.connect(
             lambda msg: QMessageBox.about(self, "Check for updates", msg)
         )
         QTimer.singleShot(100, self.auto_check_updates.start)
+        self.center_window()
 
     def check_updates(self):
         out_of_date, message = check_version()
         QMessageBox.about(self, "Check for updates", message)
 
     def open_docs(self):
         QDesktopServices.openUrl(QUrl(self.documentation_url))
 
     def center_window(self):
         w, h = 1000, 800
-        cp = QGuiApplication.screenAt(self.cursor().pos()).availableGeometry().center()
+        try:
+            cp = (
+                QGuiApplication.screenAt(self.cursor().pos())
+                .availableGeometry()
+                .center()
+            )
+        except AttributeError:
+            # in Fedora QGuiApplication.screenAt(self.cursor().pos()) is None
+            cp = QGuiApplication.primaryScreen().availableGeometry().center()
+
         self.setGeometry(cp.x() - w // 2, cp.y() - h // 2, w, h)
 
     def change_theme(self, dark_theme: bool):
         if dark_theme:
             QApplication.setPalette(dark)
         else:
             QApplication.setPalette(light)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/__init__.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/cmap_gist_rainbow.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/logo_256.png` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/logo_256.png`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/themes.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/themes.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/tooltips.toml` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/canvas.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/canvas.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/custom_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PyQt6.QtCore import QEvent, QSize, Qt, QTimer, pyqtSignal
-from PyQt6.QtGui import QColor, QPainter, QPixmap
+from PyQt6.QtGui import QColor, QFocusEvent, QPainter, QPixmap
 from PyQt6.QtWidgets import (
     QHBoxLayout,
     QLabel,
     QListWidget,
     QListWidgetItem,
     QToolButton,
     QWidget,
@@ -26,22 +26,24 @@
         self.model().rowsInserted.connect(self.ListChanged.emit)
         self.model().rowsRemoved.connect(self.ListChanged.emit)
         self.model().rowsMoved.connect(self.ListChanged.emit)
         self.itemPressed.connect(self.item_selected)
         self.currentItemChanged.connect(lambda x, y: self.item_selected(x))
         self.selected_item = None
 
-    def focusOutEvent(self, event):
+    def focusOutEvent(self, event: QFocusEvent):
+        super().focusOutEvent(event)
+        if event.reason() is Qt.FocusReason.ActiveWindowFocusReason:
+            return  # this fixes drag and drop errors on Wayland
         self.clearSelection()
         item = self.itemWidget(self.selected_item)
         if item:
             item.lost_focus()
         self.newItemSelected.emit(None)
         self.selected_item = None
-        super().focusOutEvent(event)
 
     def mousePressEvent(self, event):
         super().mousePressEvent(event)
         if not self.indexAt(event.pos()).isValid():
             self.clearFocus()
 
     def changeEvent(self, event: QEvent):
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_paths_holder.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_GUI_tools/widgets_utils/video_player.py` & `idtrackerai-5.1.4/src/idtrackerai_GUI_tools/widgets_utils/video_player.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/__main__.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     window = SegmentationGUI(params)
     window.show()
     app.exec()
 
 
 @wrap_exceptions
 def general_test():
-    from time import perf_counter
+    from datetime import datetime
 
     from .run_idtrackerai import RunIdTrackerAi
 
     COMPRESSED_VIDEO_PATH = Path(str(files("idtrackerai"))) / "data" / "test_B.avi"
 
     video_path = Path.cwd() / COMPRESSED_VIDEO_PATH.name
     shutil.copyfile(COMPRESSED_VIDEO_PATH, video_path)
@@ -149,21 +149,20 @@
             "ROI_list": None,
             "track_wo_identities": False,
             "use_bkg": False,
             "protocol3_action": "continue",
         }
     )
 
-    start = perf_counter()
+    start = datetime.now()
     success = RunIdTrackerAi(params).track_video()
-    minutes = (perf_counter() - start) / 60
     if success:
         logging.info(
-            "[green]Test passed successfully in %.2f min with version %s",
-            minutes,
+            "[green]Test passed successfully in %s with version %s",
+            str(datetime.now() - start).split(".")[0],
             version("idtrackerai"),
             extra={"markup": True},
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/all_valid_parameters.dat` & `idtrackerai-5.1.4/src/idtrackerai_start_app/all_valid_parameters.dat`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/arg_parser.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/run_idtrackerai.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/run_idtrackerai.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
             self.save()
 
             crossings_detection_API(self.video, self.list_of_blobs)
 
             self.save()
 
-            (self.list_of_fragments, self.list_of_global_fragments) = fragmentation_API(
+            self.list_of_fragments, self.list_of_global_fragments = fragmentation_API(
                 self.video, self.list_of_blobs
             )
             self.save()
 
             tracker = TrackerAPI(
                 self.video,
                 self.list_of_blobs,
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_GUI.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,14 @@
         self.centralWidget().layout().addWidget(main_splitter)
         self.list_of_widgets = self.get_list_of_widgets(left_layout)
         for widget in self.list_of_widgets:
             widget.setEnabled(False)
         self.right_splitter.setEnabled(False)
         self.enabled = False
         self.open_widget.setEnabled(True)
-        self.center_window()
 
         self.setTabOrder(self.resreduct, self.videoPlayer.canvas)
         self.setTabOrder(self.videoPlayer.canvas, self.resreduct)
         for widget in self.findChildren(QCheckBox):
             assert isinstance(widget, QWidget)
             widget.setFocusPolicy(Qt.FocusPolicy.NoFocus)
         QTimer.singleShot(0, lambda: self.load_parameters(self.user_params))
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/ROI_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/bkg_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,16 @@
                 " again the background subtraction if desired when finish editing the"
                 " video paths."
             ),
         )
         self.checkBox.setChecked(False)
 
     def view_bkg_clicked(self):
-        img = self.bkg_thread.bkg
-        assert img is not None
-        self.image_display.show((255 * img / img.max()).astype("uint8"))
+        if self.bkg_thread.bkg is not None:
+            self.image_display.show(self.bkg_thread.bkg)
 
     def CheckBox_changed(self, checked):
         if checked:
             if not hasattr(self, "video_paths"):
                 self.checkBox.setChecked(False)
                 return
             self.bkg_thread.set_parameters(self.video_paths, self.episodes)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/blob_info_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/frame_analyzer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/intensity_ths.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/open_video_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import Sequence
 
 from PyQt6.QtCore import Qt, pyqtSignal
+from PyQt6.QtGui import QFocusEvent
 from PyQt6.QtWidgets import (
     QFileDialog,
     QHBoxLayout,
     QListView,
     QListWidget,
     QMessageBox,
     QPushButton,
@@ -46,17 +47,18 @@
             super().keyPressEvent(event)
 
     def keyReleaseEvent(self, e):
         event = key_event_modifier(e)
         if event is not None:
             super().keyReleaseEvent(event)
 
-    def focusOutEvent(self, event):
-        self.clearSelection()
+    def focusOutEvent(self, event: QFocusEvent):
         super().focusOutEvent(event)
+        if event.reason() is not Qt.FocusReason.ActiveWindowFocusReason:
+            self.clearSelection()  # this IF fixes drag and drop errors on Wayland
 
 
 class OpenVideoWidget(QWidget):
     new_video_paths = pyqtSignal(list, tuple, int, int, list)
     path_clicked = pyqtSignal(int)
     video_paths_reordered = pyqtSignal(list)
     new_episodes = pyqtSignal(list, object)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py` & `idtrackerai-5.1.4/src/idtrackerai_start_app/segmentation_widgets/track_intervals_widget.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_start_app/tooltips.toml` & `idtrackerai-5.1.4/src/idtrackerai_start_app/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/__main__.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/tooltips.toml` & `idtrackerai-5.1.4/src/idtrackerai_validator/tooltips.toml`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validation_GUI.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validation_GUI.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 import logging
+import sys
 from enum import Enum
 from pathlib import Path
 
 import numpy as np
 import toml
 from PyQt6.QtCore import Qt, QThread, QTimer, pyqtSignal
 from PyQt6.QtGui import QAction, QCloseEvent, QColor, QKeyEvent
 from PyQt6.QtWidgets import (
+    QApplication,
     QCheckBox,
     QDialog,
     QFileDialog,
     QHBoxLayout,
     QLabel,
-    QListWidget,
     QMessageBox,
     QProgressDialog,
     QPushButton,
     QSpinBox,
     QSplitter,
     QTabWidget,
     QVBoxLayout,
     QWidget,
 )
 
-from idtrackerai import Blob, ListOfBlobs, Video, ListOfFragments
+from idtrackerai import Blob, Fragment, ListOfBlobs, ListOfFragments, Video
 from idtrackerai.postprocess import (
     convert_trajectories_file_to_csv_and_json,
     produce_output_dict,
 )
-from idtrackerai.utils import resolve_path, track
+from idtrackerai.utils import resolve_path
 from idtrackerai_GUI_tools import (
     CanvasMouseEvent,
     CanvasPainter,
     GUIBase,
     LabelRangeSlider,
     QHLine,
     VideoPlayer,
 )
 from idtrackerai_GUI_tools import __file__ as idtrackerai_GUI_tools_file
-from idtrackerai_GUI_tools import build_ROI_patches_from_list, key_event_modifier
+from idtrackerai_GUI_tools import build_ROI_patches_from_list
 
 from .validator_widgets import (
+    AdditionalInfo,
     ErrorsExplorer,
     IdGroups,
     IdLabels,
     Interpolator,
+    MarkBlobs,
     SetupPoints,
     find_selected_blob,
     paintBlobs,
     paintTrails,
-    AdditionalInfo,
 )
 
 parent_dir = Path(idtrackerai_GUI_tools_file).parent
 for file in parent_dir.glob("cmap_*"):
     general_cmap = np.loadtxt(parent_dir / file, dtype=np.uint8)
 assert general_cmap is not None
 
@@ -134,15 +136,57 @@
 
         new_id = self.spinbox.value()
         if new_id == -1:
             new_id = None
         return answer, new_id, self.propagate.isChecked()
 
 
+class LoadSessionObjects(QThread):
+    """Independent thread to load lists of Blobs/Fragments
+    because they take too long for large sessions."""
+
+    blobs: ListOfBlobs | None = None
+    fragments: list[Fragment] | None = None
+
+    def __init__(self, video: Video, parent: QWidget):
+        super().__init__(parent)
+        self.video = video
+        self.parienta = parent
+
+    def run(self):
+        for path in (
+            self.video.blobs_path_validated,
+            self.video.blobs_no_gaps_path,
+            self.video.blobs_path,
+        ):
+            try:
+                self.blobs = ListOfBlobs.load(path)
+                break
+            except FileNotFoundError:
+                pass
+        else:
+            self.blobs = None
+
+        try:
+            self.fragments = ListOfFragments.load(
+                self.video.fragments_path, reconnect=False
+            ).fragments
+            for index, fragment in enumerate(self.fragments):
+                if fragment.identifier != index:
+                    logging.warning(
+                        "Loading an old session, invalid list of fragments format"
+                    )
+                    raise FileExistsError
+        except FileNotFoundError:
+            self.fragments = None
+
+
 class ValidationGUI(GUIBase):
+    blobs: ListOfBlobs
+
     def __init__(self, session_path: Path | None = None):
         super().__init__()
 
         # TODO logging.getLogger().addHandler(WarningRedirector(self))
 
         self.setWindowTitle("idtracker.ai | Validation GUI")
         self.documentation_url = (
@@ -162,14 +206,17 @@
         self.id_groups = IdGroups(self)
         self.id_groups.needToDraw.connect(self.video_player.update)
         self.id_groups.unsaved_changes.connect(new_changes)
 
         self.errorsExplorer = ErrorsExplorer()
         self.errorsExplorer.go_to_error.connect(self.go_to_error)
 
+        self.mark_blobs = MarkBlobs(self)
+        self.mark_blobs.needToDraw.connect(self.video_player.update)
+
         self.interpolator = Interpolator()
         self.interpolator.neew_to_draw.connect(self.video_player.update)
         self.interpolator.update_trajectories.connect(self.update_trajectories_range)
         self.interpolator.go_to_frame.connect(self.video_player.setCurrentFrame)
         self.interpolator.preload_frames.connect(self.video_player.preload_frames)
         self.interpolator.interpolation_accepted.connect(
             self.errorsExplorer.accepted_interpolation
@@ -191,14 +238,16 @@
 
         self.additional_info = AdditionalInfo()
 
         tabs = QTabWidget()
         tabs.addTab(self.id_groups, "Groups")
         tabs.addTab(self.id_labels, "Labels")
         tabs.addTab(self.setup_points, "Setup Points")
+        tabs.addTab(self.mark_blobs, "Mark blobs")
+        tabs.setMinimumWidth(250)
         tabs.currentChanged.connect(self.video_player.update)
         right_splitter.addWidget(tabs)
         right_splitter.addWidget(self.additional_info)
         self.interpolator.enabled_changed.connect(
             lambda enabled: tabs.setEnabled(not enabled)
         )
 
@@ -210,17 +259,18 @@
         splitter = QSplitter(Qt.Orientation.Horizontal, self)
         self.video_player.layout().setContentsMargins(8, 0, 8, 0)
         left_widget = QWidget()
         left_widget.setLayout(left_splitter)
         splitter.addWidget(left_widget)
         splitter.addWidget(self.video_player)
         splitter.addWidget(right_splitter)
-        splitter.setStretchFactor(0, 1)
-        splitter.setStretchFactor(1, 3)
-        splitter.setStretchFactor(2, 1)
+        splitter.setStretchFactor(0, 0)
+        splitter.setStretchFactor(1, 1)
+        splitter.setStretchFactor(2, 0)
+        splitter.setSizes((1, 10, 1))
         self.centralWidget().layout().addWidget(splitter)
         self.centralWidget().setEnabled(False)
         self.centralWidget().layout().setContentsMargins(8, 0, 8, 8)
 
         self.selected_id: int | None = None
         self.selected_blob: Blob | None = None
         self.selection_last_location: tuple[float, float] | None = None
@@ -322,15 +372,14 @@
             tooltips["interpolation_order"]
         )
         for index in range(self.interpolator.input_size_row.count()):
             self.interpolator.input_size_row.itemAt(index).widget().setToolTip(
                 tooltips["input_size"]
             )
 
-        self.center_window()
         if session_path is not None:
             QTimer.singleShot(0, lambda: self.open_session(session_path))
         self.unsaved_changes = False
 
     def keyPressEvent(self, event: QKeyEvent):
         if event.key() in (Qt.Key.Key_Return, Qt.Key.Key_Enter):
             self.id_groups.uncheck_edit_buttons()
@@ -342,14 +391,20 @@
         start: int,
         length: int,
         where: np.ndarray | None,
         identity: int,
     ):
         if where is None:
             where = self.trajectories[start]
+            if kind == "No id":
+                for blob in self.blobs.blobs_in_video[start]:
+                    for blob_id, centroid in blob.final_ids_and_centroids:
+                        if blob_id in (None, 0):
+                            where = np.asarray(centroid)
+                            break
             assert where is not None
 
         if where.ndim == 2:
             # Set the zoom to capture all positions of 'where'
             xmax, ymax = np.nanmax(where, axis=0)
             xmin, ymin = np.nanmin(where, axis=0)
             zoom_scale = max(
@@ -390,20 +445,27 @@
         self.video.identities_labels = self.id_labels.get_labels()[1:]
         self.video.identities_groups = self.id_groups.get_groups()
         self.video.setup_points = self.setup_points.get_points()
         self.video.save()
         self.blobs.save(self.video.blobs_path_validated)
 
         progress = QProgressDialog(
-            "Computing trajectories", "Abort", 0, self.video.number_of_frames + 1, self
+            "Computing trajectories",
+            "Abort",
+            0,
+            self.video.number_of_frames + 1,
+            self,
+            Qt.WindowType.SplashScreen,
         )
         progress.setMinimumDuration(1500)
         progress.setModal(True)
 
-        self.save_thread = SaveTrajectoriesThread(self.blobs.blobs_in_video, self.video)
+        self.save_thread = SaveTrajectoriesThread(
+            self.blobs.blobs_in_video, self.video, self.fragments
+        )
         progress.canceled.connect(self.save_thread.quit)
         self.save_thread.finished.connect(self.finish_saving)
         self.save_thread.progress_changed.connect(progress.setValue)
         self.save_thread.start()
 
     def finish_saving(self):
         if self.save_thread.success:
@@ -429,41 +491,42 @@
                     " behavior can happen. Do you want to continue?"
                 ),
                 QMessageBox.StandardButton.Cancel | QMessageBox.StandardButton.Ok,
             )
             if answer != QMessageBox.StandardButton.Ok:
                 return
 
-        blobs_paths_candidates = [
-            video.blobs_path_validated,
-            video.blobs_no_gaps_path,
-            video.blobs_path,
-        ]
+        loading_thread = LoadSessionObjects(video, self)
+        progress_bar = QProgressDialog(
+            "Loading session, please wait...",
+            "Close app",
+            0,
+            0,
+            self,
+            Qt.WindowType.SplashScreen,
+        )
+        progress_bar.setMinimumDuration(100)
+        progress_bar.canceled.connect(loading_thread.terminate)
+        progress_bar.canceled.connect(sys.exit)
+        progress_bar.setModal(True)
+
+        loading_thread.start()
+        while loading_thread.isRunning():
+            QApplication.processEvents()
+        progress_bar.cancel()
 
-        for path in blobs_paths_candidates:
-            try:
-                self.blobs = ListOfBlobs.load(path)
-            except FileNotFoundError:
-                continue
-            else:
-                break
-        else:
+        if loading_thread.blobs is None:
             QMessageBox.warning(
-                self,
-                "Loading session error",
-                f"List of blobs not found on any of {blobs_paths_candidates}",
+                self, "Loading session error", "List of blobs not found"
             )
             return
+        self.blobs = loading_thread.blobs
+        self.fragments = loading_thread.fragments
 
-        if video.fragments_path.is_file():
-            self.additional_info.list_of_fragments = ListOfFragments.load(
-                video.fragments_path
-            )
-        else:
-            self.additional_info.list_of_fragments = None
+        self.additional_info.fragments = self.fragments
 
         self.video_player.update_video_paths(
             video.video_paths,
             video.number_of_frames,
             (video.original_width, video.original_height),
             video.frames_per_second,
             res_reduct=video.resolution_reduction,
@@ -480,20 +543,18 @@
         cmap = [(255, 255, 255)] + list(
             general_cmap[np.linspace(0, 255, video.number_of_animals, dtype=int)]
         )
         self.cmap = [QColor(*color) for color in cmap]
         self.cmap_alpha = [QColor(*color, alpha=77) for color in cmap]
 
         self.id_groups.load_groups(video.identities_groups)
-        if hasattr(video, "identities_labels") and video.identities_labels:
-            self.id_labels.load_labels(video.identities_labels)
-        else:
-            self.id_labels.load_labels(
-                list(map(str, range(1, video.number_of_animals + 1)))
-            )
+        self.id_labels.load_labels(
+            video.identities_labels
+            or [str(i + 1) for i in range(video.number_of_animals)]
+        )
 
         self.setup_points.load_points(video.setup_points)
         self.errorsExplorer.set_references(
             self.trajectories,
             self.unidentified,
             self.duplicated,
             video.tracking_intervals,
@@ -548,15 +609,17 @@
                 self.selected_blob.add_centroid(event.xy_data, new_id)
                 self.update_trajectories_range(self.current_frame_number)
             return
 
         # clicked on a blob with centroid
         assert self.selection_last_location is not None
         answer, new_id, propagate = self.dbl_click_dialog.exec_with_description(
-            self.selected_id
+            self.interpolator.animal_id + 1
+            if self.interpolator.isEnabled()
+            else self.selected_id
         )
         if answer == DblClickDialog.Answers.ChangeId:
             self.selected_blob.update_identity(
                 self.selected_id, new_id, self.selection_last_location
             )
             if propagate:
                 lower, upper = self.selected_blob.propagate_identity(
@@ -610,24 +673,25 @@
             painter,
             blobs_in_frame,
             cmap,
             cmap_alpha,
             self.selected_blob,
             self.selection_last_location,
             self.id_labels.get_labels(),
+            self.mark_blobs(blobs_in_frame, self.fragments),
         )
 
         if self.setup_points.isVisible():
             self.setup_points.paint_on_canvas(painter)
 
         if self.interpolator.isEnabled():
             self.interpolator.paint_on_canvas(painter, frame_number)
 
         if update_info_widget:
-            self.additional_info.set_data(self.selected_blob)
+            self.additional_info.set_data(self.selected_blob, len(blobs_in_frame))
 
     def closeEvent(self, event: QCloseEvent):
         if not self.unsaved_changes:
             return super().closeEvent(event)
 
         answer = QMessageBox.question(
             self,
@@ -652,17 +716,15 @@
         ids_in_frame = set()
         self.trajectories[start:finish] = np.nan
         self.duplicated[start:finish] = False
         self.unidentified[start:finish] = False
         for blobs_in_frame in self.blobs.blobs_in_video[start:finish]:
             ids_in_frame.clear()
             for blob in blobs_in_frame:
-                for identity, centroid in zip(
-                    blob.final_identities, blob.final_centroids
-                ):
+                for identity, centroid in blob.final_ids_and_centroids:
                     if identity not in (None, 0):
                         self.trajectories[blob.frame_number, identity - 1] = centroid
                         if identity in ids_in_frame:
                             self.duplicated[blob.frame_number, identity - 1] = True
                         ids_in_frame.add(identity)
                     else:
                         self.unidentified[blob.frame_number] = True
@@ -673,20 +735,32 @@
 
     def generate_trajectories(self, blobs_in_video: list[list[Blob]]):
         number_of_frames = len(blobs_in_video)
         self.trajectories = np.full((number_of_frames, self.n_animals, 2), np.NaN)
         self.unidentified = np.zeros((number_of_frames), bool)
         self.duplicated = np.zeros((number_of_frames, self.n_animals), bool)
         ids_in_frame: set[int] = set()
-        for blobs_in_frame in track(blobs_in_video, "Analyzing trajectories"):
+
+        progress_bar = QProgressDialog(
+            "Analyzing trajectories",
+            "Close app",
+            0,
+            number_of_frames - 1,
+            self,
+            Qt.WindowType.SplashScreen,
+        )
+        progress_bar.setMinimumDuration(1000)
+        progress_bar.canceled.connect(sys.exit)
+        progress_bar.setModal(True)
+
+        for index, blobs_in_frame in enumerate(blobs_in_video):
+            progress_bar.setValue(index)
             ids_in_frame.clear()
             for blob in blobs_in_frame:
-                for identity, centroid in zip(
-                    blob.final_identities, blob.final_centroids
-                ):
+                for identity, centroid in blob.final_ids_and_centroids:
                     if identity not in (None, 0):
                         self.trajectories[blob.frame_number, identity - 1] = centroid
                         if identity in ids_in_frame:
                             self.duplicated[blob.frame_number, identity - 1] = True
                         ids_in_frame.add(identity)
                     else:
                         self.unidentified[blob.frame_number] = True
@@ -697,54 +771,61 @@
 ) -> tuple[Blob | None, int | None, tuple[float, float] | None]:
     distances_to_centroids: list[
         tuple[Blob, int | None, tuple[float, float], float]
     ] = []
 
     for blob in blobs:
         if blob.contains_point(click.xy_data):
-            for identity, centroid in zip(blob.final_identities, blob.final_centroids):
+            for identity, centroid in blob.final_ids_and_centroids:
                 dist = click.sq_distance_to(centroid)
                 distances_to_centroids.append((blob, identity, centroid, dist))
             if not distances_to_centroids:  # blob with no centroids
                 return blob, -1, None
             break
 
     if distances_to_centroids:
         return min(distances_to_centroids, key=lambda x: x[-1])[:-1]
 
     for blob in blobs:
-        for identity, centroid in zip(blob.final_identities, blob.final_centroids):
+        for identity, centroid in blob.final_ids_and_centroids:
             dist = click.sq_distance_to(centroid)
             if dist < (SELECT_POINT_DIST * click.zoom):
                 distances_to_centroids.append((blob, identity, centroid, dist))
 
     if distances_to_centroids:
         return min(distances_to_centroids, key=lambda x: x[-1])[:-1]
 
     return None, -1, None
 
 
 class SaveTrajectoriesThread(QThread):
     progress_changed = pyqtSignal(int)
 
-    def __init__(self, blobs_in_video: list[list[Blob]], video: Video):
+    def __init__(
+        self,
+        blobs_in_video: list[list[Blob]],
+        video: Video,
+        list_of_fragments: list[Fragment] | None,
+    ):
         super().__init__()
         self.blobs_in_video = blobs_in_video
+        self.fragments = list_of_fragments
         self.video = video
         self.success = False
         self.finished.connect(
             lambda: self.progress_changed.emit(len(self.blobs_in_video) + 1)
         )
 
     def run(self):
         self.abort = False
 
         trajectories = produce_output_dict(
             self.blobs_in_video,
             self.video,
+            self.fragments,
             progress_bar=self.progress_changed,
             abort=lambda: self.abort,
         )
         if self.abort:
             return
         trajectories_file = (
             self.video.trajectories_folder / "trajectories_validated.npy"
@@ -759,14 +840,17 @@
         self.success = True
 
     def quit(self):
         self.abort = True
 
 
 class ResetSessionDialog(QDialog):
+    """Pop up to select the range of the user corrections reset.
+    Reset is activated in the menu bar / Session / Reset session"""
+
     class Answers(Enum):
         Cancel = 0
         RangeReset = 1
         AllReset = 2
 
     def __init__(self, parent, n_frames: int):
         super().__init__(parent)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/additional_info.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/additional_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt6.QtGui import QKeyEvent
 from PyQt6.QtWidgets import QLabel, QListWidget, QVBoxLayout, QWidget
 
-from idtrackerai import Blob, ListOfFragments
+from idtrackerai import Blob, Fragment
 from idtrackerai_GUI_tools import key_event_modifier
 
 
 class CustomListWidget(QListWidget):
     def __init__(self):
         super().__init__()
         self.setAlternatingRowColors(True)
@@ -18,36 +18,40 @@
     def keyReleaseEvent(self, e: QKeyEvent):
         event = key_event_modifier(e)
         if event is not None:
             super().keyReleaseEvent(event)
 
 
 class AdditionalInfo(QWidget):
-    list_of_fragments: ListOfFragments | None
+    fragments: list[Fragment] | None
 
     def __init__(self) -> None:
         super().__init__()
         self.setLayout(QVBoxLayout())
+        self.n_blobs_in_frame = QLabel("")
         self.blob_title = QLabel("Selected blob:")
         self.blob_properties = CustomListWidget()
-        # self.fragment_title = QLabel("Selected blob's fragment")
-        # self.fragment_properties = CustomListWidget()
+        self.fragment_title = QLabel("Selected blob's fragment")
+        self.fragment_properties = CustomListWidget()
         self.layout().setContentsMargins(0, 0, 0, 8)
+        self.layout().addWidget(self.n_blobs_in_frame)
         self.layout().addWidget(self.blob_title)
         self.layout().addWidget(self.blob_properties)
-        # self.layout().addWidget(self.fragment_title)
-        # self.layout().addWidget(self.fragment_properties)
+        self.layout().addWidget(self.fragment_title)
+        self.layout().addWidget(self.fragment_properties)
 
-    def set_data(self, blob: Blob | None):
+    def set_data(self, blob: Blob | None, n_blobs: int):
         self.blob_properties.clear()
-        # self.fragment_properties.clear()
+        self.fragment_properties.clear()
+        # add "All" blobs in frame
+        self.n_blobs_in_frame.setText(f"{n_blobs} blobs in frame")
         if blob is None:
             return
 
         self.blob_properties.addItems(blob.properties)
 
-        # if self.list_of_fragments is None:
-        #     return
+        if self.fragments is None:
+            return
 
-        # self.fragment_properties.addItems(
-        #     self.list_of_fragments.fragments[blob.fragment_identifier].properties
-        # )
+        self.fragment_properties.addItems(
+            self.fragments[blob.fragment_identifier].properties
+        )
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/errors_explorer.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/errors_explorer.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_groups.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_groups.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/id_labels.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/id_labels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from PyQt6.QtCore import pyqtSignal
+from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QFormLayout, QLineEdit, QScrollArea, QWidget
 
 
 class IdLabels(QScrollArea):
     needToDraw = pyqtSignal()
     labels: list[str]
 
     def __init__(self):
         super().__init__()
         self.form_layout = QFormLayout()
         self.setWidgetResizable(True)
         wid = QWidget()
         wid.setLayout(self.form_layout)
         self.setWidget(wid)
-
-        # To disable horizontal scrolling
-        self.setMinimumWidth(
-            self.widget().minimumSizeHint().width()
-            + self.verticalScrollBar().width()
-            + 2  # it works with this extra padding
-        )
+        self.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 
     def load_labels(self, labels: list[str]):
         for _ in range(self.form_layout.rowCount()):
             self.form_layout.removeRow(0)
 
         for indx, label in enumerate(labels, 1):
             edit = QLineEdit()
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/interpolator.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/interpolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         range_row = QHBoxLayout()
         range_row.setAlignment(Qt.AlignmentFlag.AlignLeft)
         self.start_btn = QToolButton()
         self.end_btn = QToolButton()
         self.start_btn.clicked.connect(lambda: self.go_to_frame.emit(self.start - 1))
         self.end_btn.clicked.connect(lambda: self.go_to_frame.emit(self.end))
-        range_row.addWidget(QLabel("Range: from"))
+        range_row.addWidget(QLabel("From"))
         range_row.addWidget(self.start_btn)
         range_row.addWidget(QLabel("to"))
         range_row.addWidget(self.end_btn)
         layout.addLayout(range_row)
 
         self.interpolation_order_box = CustomComboBox()
         self.interpolation_order_box.addItems(self.interpolation_kinds.keys())
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/paint_blobs.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/paint_blobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Iterable
+
 import numpy as np
 from PyQt6.QtCore import QPointF, QRectF, Qt
 from PyQt6.QtGui import QColor, QImage, QPainter, QPolygon
 
 from idtrackerai import Blob
 from idtrackerai_GUI_tools import CanvasPainter
 
@@ -39,37 +41,46 @@
     painter: CanvasPainter,
     blobs_in_frame: list[Blob],
     cmap: list[QColor],
     cmap_alpha: list[QColor],
     selected_blob: Blob | None,
     selected_centroid: tuple[float, float] | None,
     labels: list[str],
+    marked_blobs: Iterable[Blob],
 ):
     labels_to_draw: list[tuple[QColor, str, tuple]] = []
     polygon = QPolygon()
 
     if selected_blob is not None:
+        selected_blob_final_identities = list(selected_blob.final_identities)
         color_indx = (
-            selected_blob.final_identities[0]
-            if len(selected_blob.final_identities) == 1
-            and selected_blob.final_identities[0] is not None
+            selected_blob_final_identities[0]
+            if len(selected_blob_final_identities) == 1
+            and selected_blob_final_identities[0] is not None
             else 0
         )
         color_alpha = cmap_alpha[color_indx]
 
         painter.setPenColor(0xFFFFFF)
         polygon.setPoints(*selected_blob.contour.ravel())
         painter.setBrush(color_alpha)
         painter.drawPolygon(polygon)
         painter.setBrush(Qt.BrushStyle.NoBrush)
 
+    painter.setPen(Qt.PenStyle.NoPen)
+    painter.setBrush(QColor(255, 0, 0, 128))
+    for blob in marked_blobs:
+        polygon.setPoints(*blob.contour.ravel())
+        painter.drawPolygon(polygon)
+
     for blob in blobs_in_frame:
+        blob_final_identities = list(blob.final_identities)
         color_indx = (
-            blob.final_identities[0]
-            if len(blob.final_identities) == 1 and blob.final_identities[0] is not None
+            blob_final_identities[0]
+            if len(blob_final_identities) == 1 and blob_final_identities[0] is not None
             else 0
         )
         color = cmap[color_indx]
 
         painter.setPenColor(color)
 
         if draw_contours:
@@ -105,14 +116,15 @@
             color = cmap[0 if identity is None else identity]
             labels_to_draw.append((color, idstr, centroid))
 
     if selected_blob is not None and selected_centroid is not None:
         radius = 15 * painter.applied_zoom
         x, y = selected_centroid
         painter.setPenColor(0x000000)
+        painter.setBrush(Qt.BrushStyle.NoBrush)
         painter.drawEllipse(QRectF(x - radius / 2, y - radius / 2, radius, radius))
 
     # colored centroids
     if draw_centroids:
         painter.setPen(Qt.PenStyle.NoPen)
         for color, _idstr, (x, y) in labels_to_draw:
             painter.setBrush(color)
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_validator/validator_widgets/setup_points.py` & `idtrackerai-5.1.4/src/idtrackerai_validator/validator_widgets/setup_points.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_video/general_video.py` & `idtrackerai-5.1.4/src/idtrackerai_video/general_video.py`

 * *Files identical despite different names*

### Comparing `idtrackerai-5.1.3/src/idtrackerai_video/individual_videos.py` & `idtrackerai-5.1.4/src/idtrackerai_video/individual_videos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from pathlib import Path
 
 import cv2
 import numpy as np
 
 from idtrackerai import Video
 from idtrackerai.utils import create_dir, track
 from idtrackerai_GUI_tools import VideoPathHolder
```

### Comparing `idtrackerai-5.1.3/src/idtrackerai_video/main.py` & `idtrackerai-5.1.4/src/idtrackerai_video/main.py`

 * *Files identical despite different names*


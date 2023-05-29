# Comparing `tmp/Simba-UW-tf-dev-1.61.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.61.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.3.tar", last modified: Thu May 25 19:53:47 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.4.tar", last modified: Mon May 29 21:11:05 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.61.3.tar` & `Simba-UW-tf-dev-1.61.4.tar`

### file list

```diff
@@ -1,506 +1,507 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.61.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-23 15:41:51.000000 Simba-UW-tf-dev-1.61.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-25 14:55:02.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18214 2023-05-24 15:19:35.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.3/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.3/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10984 2023-05-24 16:55:20.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11410 2023-05-23 20:23:27.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.61.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.3/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.3/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18515 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.3/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.3/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5043 2023-05-25 14:14:27.000000 Simba-UW-tf-dev-1.61.3/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.3/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.3/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3972 2023-05-21 18:23:01.000000 Simba-UW-tf-dev-1.61.3/tests/test_thirdparty_appenders.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-25 19:53:39.000000 Simba-UW-tf-dev-1.61.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.61.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.4/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-29 21:05:41.000000 Simba-UW-tf-dev-1.61.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-25 14:55:02.000000 Simba-UW-tf-dev-1.61.4/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.4/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.61.4/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.4/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.61.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.4/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.4/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18654 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-29 21:11:04.000000 Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.4/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.4/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.61.4/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.4/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.61.4/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.4/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.61.4/tests/test_thirdparty_appenders.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-29 21:11:03.000000 Simba-UW-tf-dev-1.61.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-29 21:11:05.000000 Simba-UW-tf-dev-1.61.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.61.3/PKG-INFO` & `Simba-UW-tf-dev-1.61.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.3
+Version: 1.61.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.enums import Keys, Links, Formats, Paths
 from simba.ui.tkinter_functions import DropDownMenu, CreateLabelFrameWithIcon
 from simba.utils.read_write import get_file_name_info_in_directory
 from simba.utils.errors import AnimalNumberError
-from simba.plotting.Directing_animals_visualizer import DirectingOtherAnimalsVisualizer
-from simba.plotting.Directing_animals_visualizer_mp import DirectingOtherAnimalsVisualizerMultiprocess
+from simba.plotting.directing_animals_visualizer import DirectingOtherAnimalsVisualizer
+from simba.plotting.directing_animals_visualizer_mp import DirectingOtherAnimalsVisualizerMultiprocess
 
 class DirectingOtherAnimalsVisualizerPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str):
 
 
         ConfigReader.__init__(self, config_path=config_path)
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.61.4/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.61.4/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.61.4/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.61.4/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.61.4/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.61.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.61.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -99,38 +99,38 @@
 00000620: 0128 012a 012b 012d 0136 0137 0139 013a  .(.*.+.-.6.7.9.:
 00000630: 0143 0144 0145 0147 0150 0151 0153 0154  .C.D.E.G.P.Q.S.T
 00000640: 0156 015f 0160 0162 0163 0165 016e 016f  .V._.`.b.c.e.n.o
 00000650: 0171 0172 0174 017d 017e 0180 0181 0183  .q.r.t.}.~......
 00000660: 018c 018d 0190 0191 0193 0194 019d 01aa  ................
 00000670: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
 00000680: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00000690: 01b4 1024 2518 0a54 7369 7a65 1061 0809  ...$%..Tsize.a..
-000006a0: d40d 0e0f 1029 2a0a 0a54 6b69 6e64 1073  .....)*..Tkind.s
-000006b0: 0909 d40d 0e0f 102e 2f0a 1855 6c61 6265  ......../..Ulabe
-000006c0: 6c10 6409 08d4 0d0e 0f10 3334 0a18 5776  l.d.......34..Wv
-000006d0: 6572 7369 6f6e 104b 0908 d40d 0e0f 1038  ersion.K.......8
-000006e0: 390a 1858 636f 6d6d 656e 7473 1101 2c09  9..Xcomments..,.
-000006f0: 08d4 0d0e 0f10 3d3e 1818 5e64 6174 654c  ......=>..^dateL
-00000700: 6173 744f 7065 6e65 6410 c808 08d4 0d0e  astOpened.......
-00000710: 0f10 421c 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
-00000720: 0808 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
-00000730: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
-00000740: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-00000750: 6500 7000 7900 8c00 8e00 8f00 9b00 a400  e.p.y...........
-00000760: af00 b500 bf00 c700 cc00 cf00 d000 d100  ................
-00000770: da00 e300 e500 e600 e700 f000 fd00 ff01  ................
-00000780: 0001 0101 0a01 1601 1701 1801 2101 2601  ............!.&.
-00000790: 2801 2901 2a01 3301 3801 3a01 3b01 3c01  (.).*.3.8.:.;.<.
-000007a0: 4501 4b01 4d01 4e01 4f01 5801 6001 6201  E.K.M.N.O.X.`.b.
-000007b0: 6301 6401 6d01 7601 7901 7a01 7b01 8401  c.d.m.v.y.z.{...
-000007c0: 9301 9501 9601 9701 a001 aa01 ab01 ac01  ................
-000007d0: ad01 b601 c301 cc00 0000 0000 0002 0100  ................
-000007e0: 0000 0000 0000 4a00 0000 0000 0000 0000  ......J.........
-000007f0: 0000 0000 0001 cd00 0000 0c00 7500 6e00  ............u.n.
-00000800: 7300 7500 0000 0001 0000 0000 0000 080b  s.u.............
+00000690: 01b4 6564 0808 d40d 0e0f 1024 2518 0a54  ..ed.......$%..T
+000006a0: 7369 7a65 1061 0809 d40d 0e0f 1029 2a0a  size.a.......)*.
+000006b0: 0a54 6b69 6e64 1073 0909 d40d 0e0f 102e  .Tkind.s........
+000006c0: 2f0a 1855 6c61 6265 6c10 6409 08d4 0d0e  /..Ulabel.d.....
+000006d0: 0f10 3334 0a18 5776 6572 7369 6f6e 104b  ..34..Wversion.K
+000006e0: 0908 d40d 0e0f 1038 390a 1858 636f 6d6d  .......89..Xcomm
+000006f0: 656e 7473 1101 2c09 08d4 0d0e 0f10 3d3e  ents..,.......=>
+00000700: 1818 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00000710: 6410 c808 08d4 0d0e 0f10 421c 1818 5964  d.........B...Yd
+00000720: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
+00000730: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00000740: 6409 1001 0008 0019 0022 0034 003c 0050  d........".4.<.P
+00000750: 0059 0064 0077 008c 0095 0096 00a2 00ab  .Y.d.w..........
+00000760: 00b6 00bc 00c6 00ce 00d3 00d6 00d7 00d8  ................
+00000770: 00e1 00ea 00ec 00ed 00ee 00f7 00f8 00fa  ................
+00000780: 00fb 0108 0111 011d 011e 011f 0128 012d  .............(.-
+00000790: 012f 0130 0131 013a 013f 0141 0142 0143  ./.0.1.:.?.A.B.C
+000007a0: 014c 0152 0154 0155 0156 015f 0167 0169  .L.R.T.U.V._.g.i
+000007b0: 016a 016b 0174 017d 0180 0181 0182 018b  .j.k.t.}........
+000007c0: 019a 019c 019d 019e 01a7 01b1 01b2 01b3  ................
+000007d0: 01b4 01bd 01ca 01cb 0000 0000 0000 0201  ................
+000007e0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+000007f0: 0000 0000 0000 01cd 0000 000c 0075 006e  .............u.n
+00000800: 0073 0075 0000 0001 0000 0000 0000 080b  .s.u............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -254,55 +254,55 @@
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0002 0000 0005 0000 0007  ................
 00001010: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00001020: 006e 0067 6c73 7643 626c 6f62 0000 02b8  .n.glsvCblob....
 00001030: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00001040: 0809 0a0b 0b0d 1848 4948 4a4b 4c5f 1010  .......HIHJKL_..
-00001050: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00001060: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00001070: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00001080: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
-00001090: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
-000010a0: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
-000010b0: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
-000010c0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-000010d0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-000010e0: 7369 6f6e 0909 ab0e 171c 2125 2a2f 3439  sion......!%*/49
-000010f0: 3e43 d40f 1011 120b 140b 1657 7669 7369  >C.........Wvisi
-00001100: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00001110: 696e 675a 6964 656e 7469 6669 6572 0911  ingZidentifier..
-00001120: 01c7 0954 6e61 6d65 d40f 1011 1218 1918  ...Tname........
-00001130: 1b08 1023 0858 7562 6971 7569 7479 d40f  ...#.Xubiquity..
-00001140: 1011 120b 1e18 2009 10b5 085c 6461 7465  ...... ....\date
-00001150: 4d6f 6469 6669 6564 d40f 1011 1218 1e18  Modified........
-00001160: 2408 085b 6461 7465 4372 6561 7465 64d4  $..[dateCreated.
-00001170: 0f10 1112 0b27 1829 0910 6108 5473 697a  .....'.)..a.Tsiz
-00001180: 65d4 0f10 1112 0b2c 0b2e 0910 7309 546b  e......,....s.Tk
-00001190: 696e 64d4 0f10 1112 1831 0b33 0810 6409  ind......1.3..d.
-000011a0: 556c 6162 656c d40f 1011 1218 360b 3808  Ulabel......6.8.
-000011b0: 104b 0957 7665 7273 696f 6ed4 0f10 1112  .K.Wversion.....
-000011c0: 183b 0b3d 0811 012c 0958 636f 6d6d 656e  .;.=...,.Xcommen
-000011d0: 7473 d40f 1011 1218 4018 4208 10c8 085e  ts......@.B....^
-000011e0: 6461 7465 4c61 7374 4f70 656e 6564 d40f  dateLastOpened..
-000011f0: 1011 1218 1e18 4608 0859 6461 7465 4164  ......F..YdateAd
-00001200: 6465 6408 2300 0000 0000 0000 0023 4028  ded.#........#@(
-00001210: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
-00001220: 6965 6423 4030 0000 0000 0000 1001 0008  ied#@0..........
-00001230: 001d 0030 0042 004a 005e 0070 0079 008b  ...0.B.J.^.p.y..
-00001240: 0096 009f 00b4 00b5 00b6 00c2 00cb 00d3  ................
-00001250: 00d9 00e3 00ee 00ef 00f2 00f3 00f8 0101  ................
-00001260: 0102 0104 0105 010e 0117 0118 011a 011b  ................
-00001270: 0128 0131 0132 0133 013f 0148 0149 014b  .(.1.2.3.?.H.I.K
-00001280: 014c 0151 015a 015b 015d 015e 0163 016c  .L.Q.Z.[.].^.c.l
-00001290: 016d 016f 0170 0176 017f 0180 0182 0183  .m.o.p.v........
-000012a0: 018b 0194 0195 0198 0199 01a2 01ab 01ac  ................
-000012b0: 01ae 01af 01be 01c7 01c8 01c9 01d3 01d4  ................
-000012c0: 01dd 01e6 01f3 01fc 0000 0000 0000 0201  ................
+00001040: 0809 0a0b 0c0d 1848 4948 4a4b 0c5f 1012  .......HIHJK._..
+00001050: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001060: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001070: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001080: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001090: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000010a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000010b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000010c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+000010d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+000010e0: 6174 6573 1001 09ab 0e17 1c21 252a 2f34  ates.......!%*/4
+000010f0: 393e 43d4 0f10 1112 0c14 0c16 5776 6973  9>C.........Wvis
+00001100: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00001110: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+00001120: 1101 c709 546e 616d 65d4 0f10 1112 1819  ....Tname.......
+00001130: 181b 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
+00001140: 0f10 1112 0c1e 1820 0910 b508 5c64 6174  ....... ....\dat
+00001150: 654d 6f64 6966 6965 64d4 0f10 1112 181e  eModified.......
+00001160: 1824 0808 5b64 6174 6543 7265 6174 6564  .$..[dateCreated
+00001170: d40f 1011 120c 2718 2909 1061 0854 7369  ......'.)..a.Tsi
+00001180: 7a65 d40f 1011 120c 2c0c 2e09 1073 0954  ze......,....s.T
+00001190: 6b69 6e64 d40f 1011 1218 310c 3308 1064  kind......1.3..d
+000011a0: 0955 6c61 6265 6cd4 0f10 1112 1836 0c38  .Ulabel......6.8
+000011b0: 0810 4b09 5776 6572 7369 6f6e d40f 1011  ..K.Wversion....
+000011c0: 1218 3b0c 3d08 1101 2c09 5863 6f6d 6d65  ..;.=...,.Xcomme
+000011d0: 6e74 73d4 0f10 1112 1840 1842 0810 c808  nts......@.B....
+000011e0: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+000011f0: 0f10 1112 181e 1846 0808 5964 6174 6541  .......F..YdateA
+00001200: 6464 6564 0823 0000 0000 0000 0000 2340  dded.#........#@
+00001210: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
+00001220: 6669 6564 2340 3000 0000 0000 0009 0008  fied#@0.........
+00001230: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
+00001240: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d4  ................
+00001250: 00da 00e4 00ef 00f0 00f3 00f4 00f9 0102  ................
+00001260: 0103 0105 0106 010f 0118 0119 011b 011c  ................
+00001270: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
+00001280: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
+00001290: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
+000012a0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
+000012b0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
+000012c0: 01de 01e7 01f4 01fd 0000 0000 0000 0201  ................
 000012d0: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
 000012e0: 0000 0000 0000 01fe 0000 0008 0000 000e  ................
 000012f0: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00001300: 006f 0072 0074 0065 0072 0073 6c73 7643  .o.r.t.e.r.slsvC
 00001310: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
 00001320: d801 0203 0405 0607 0809 0a0b 1846 4748  .............FGH
 00001330: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
@@ -713,66 +713,66 @@
 00002c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 00002c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 00002ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 00002cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 00002cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 00002cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 00002ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002cf0: 0064 5473 697a 6555 6c61 6265 6c54 6b69  .dTsizeUlabelTki
-00002d00: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-00002d10: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
-00002d20: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00002d30: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
-00002d40: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
-00002d50: 190a 251a 0909 10b5 08d4 1617 1819 1a25  ..%............%
-00002d60: 1a2a 0808 1002 d416 1718 190a 2d1a 2f09  .*..........-./.
-00002d70: 1061 0810 03d4 1617 1819 1a32 0a34 0810  .a.........2.4..
-00002d80: 6409 1005 d416 1718 190a 370a 3909 1073  d.........7.9..s
-00002d90: 0910 04d4 1617 1819 1a3c 0a3e 0810 4b09  .........<.>..K.
-00002da0: 1006 d416 1718 190a 410a 4309 1101 c709  ........A.C.....
-00002db0: 1000 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
-00002dc0: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
-00002dd0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-00002de0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
-00002df0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
-00002e00: f901 0101 0701 1101 1701 1801 1b01 1c01  ................
-00002e10: 1e01 2701 2801 2a01 2b01 2d01 3601 3701  ..'.(.*.+.-.6.7.
-00002e20: 3901 3a01 4301 4401 4501 4701 5001 5101  9.:.C.D.E.G.P.Q.
-00002e30: 5301 5401 5601 5f01 6001 6201 6301 6501  S.T.V._.`.b.c.e.
-00002e40: 6e01 6f01 7101 7201 7401 7d01 7e01 8001  n.o.q.r.t.}.~...
-00002e50: 8101 8301 8c01 8d01 9001 9101 9301 9401  ................
-00002e60: 9d01 aa01 b300 0000 0000 0002 0100 0000  ................
-00002e70: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
-00002e80: 0000 0001 b400 0000 0c00 7500 6e00 7300  ..........u.n.s.
-00002e90: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00002ea0: 646d 6f44 4462 6c6f 6200 0000 08e7 da8e  dmoDDblob.......
-00002eb0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
-00002ec0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00002ed0: 646d 6f64 4462 6c6f 6200 0000 08e7 da8e  dmodDblob.......
-00002ee0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
-00002ef0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-00002f00: 6470 6831 5363 6f6d 7000 0000 0000 02b0  dph1Scomp.......
-00002f10: 0000 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
-00002f20: 6500 7200 7600 6900 7300 6500 6476 5372  e.r.v.i.s.e.dvSr
-00002f30: 6e6c 6f6e 6700 0000 0100 0000 0500 7500  nlong.........u.
-00002f40: 7400 6900 6c00 7362 7773 7062 6c6f 6200  t.i.l.sbwspblob.
-00002f50: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-00002f60: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00002f70: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00002f80: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00002f90: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00002fa0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-00002fb0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-00002fc0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00002fd0: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
-00002fe0: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
-00002ff0: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
-00003000: 0000 0101 0000 0000 0000 0010 0000 0005  ................
+00002cf0: 0074 6543 7265 6174 6564 5473 697a 6555  .teCreatedTsizeU
+00002d00: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+00002d10: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+00002d20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00002d30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00002d40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
+00002d50: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
+00002d60: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
+00002d70: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
+00002d80: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
+00002d90: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
+00002da0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
+00002db0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
+00002dc0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+00002dd0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
+00002de0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+00002df0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
+00002e00: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+00002e10: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
+00002e20: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
+00002e30: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
+00002e40: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
+00002e50: 0189 018a 018c 0195 0196 0199 019a 019c  ................
+00002e60: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
+00002e70: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+00002e80: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
+00002e90: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002ea0: 0064 6d6f 4444 626c 6f62 0000 0008 fdf7  .dmoDDblob......
+00002eb0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+00002ec0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002ed0: 0064 6d6f 6444 626c 6f62 0000 0008 fdf7  .dmodDblob......
+00002ee0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+00002ef0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+00002f00: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
+00002f10: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+00002f20: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
+00002f30: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
+00002f40: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
+00002f50: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00002f60: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+00002f70: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+00002f80: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+00002f90: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00002fa0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00002fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00002fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+00002fd0: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
+00002fe0: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
+00002ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+00003000: 0000 0001 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0004 22e0 0000 0005 0075  mp......"......u
+00003020: 6d70 0000 0000 0004 520a 0000 0005 0075  mp......R......u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 084d 44b7  smoDDblob....MD.
-00003570: 8e43 0dc5 4100 0000 0500 7500 7400 6900  .C..A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 084b  l.smodDblob....K
-00003590: 8540 afbf 0cc5 4100 0000 0500 7500 7400  .@....A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 086f 9b46  smoDDblob....o.F
+00003570: 7beb 0fc5 4100 0000 0500 7500 7400 6900  {...A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 086f  l.smodDblob....o
+00003590: 9b46 7beb 0fc5 4100 0000 0500 7500 7400  .F{...A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 04d0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035b0: 0000 0520 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -876,15 +876,15 @@
 000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
 000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
 000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
 000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
 00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
 00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003720: 7000 0000 0000 0315 b900 0000 1000 7600  p.............v.
+00003720: 7000 0000 0000 0333 0b00 0000 1000 7600  p......3......v.
 00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
 00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
 00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
 00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
 00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
 00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -972,15 +972,15 @@
 00003cb0: 5eee cc0c c541 0000 0010 0076 0069 0064  ^....A.....v.i.d
 00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
 00003ce0: 6f62 0000 0008 85b8 5eee cc0c c541 0000  ob......^....A..
 00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
 00003d10: 0073 7068 3153 636f 6d70 0000 0000 0003  .sph1Scomp......
-00003d20: d000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
+00003d20: f000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
 00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1035,17 +1035,17 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0000  ._lg1Scomp......
-00004110: c6dd 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
+00004110: c933 0000 000b 005f 005f 0070 0079 0063  .3....._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 8cb8 a0f8 740e c541  blob........t..A
+00004130: 626c 6f62 0000 0008 68ff 13ac ef0f c541  blob....h......A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
 00004160: 6f62 0000 0008 a913 1348 cc0c c541 0000  ob.......H...A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0000 e000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
@@ -1188,77 +1188,77 @@
 00004a30: 7200 6100 6700 6570 6831 5363 6f6d 7000  r.a.g.eph1Scomp.
 00004a40: 0000 0000 0020 0000 0000 0c00 6200 6c00  ..... ......b.l.
 00004a50: 6f00 6200 5f00 7300 7400 6f00 7200 6100  o.b._.s.t.o.r.a.
 00004a60: 6700 6576 5372 6e6c 6f6e 6700 0000 0100  g.evSrnlong.....
 00004a70: 0000 1200 6200 6f00 7500 6e00 6400 6900  ....b.o.u.n.d.i.
 00004a80: 6e00 6700 5f00 6200 6f00 7800 5f00 7400  n.g._.b.o.x._.t.
 00004a90: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
-00004aa0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+00004aa0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 00004ab0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00004ac0: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
 00004ad0: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
 00004ae0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00004af0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00004b00: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00004b10: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00004b20: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
-00004b30: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
-00004b40: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
-00004b50: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00004b60: 0000 0000 0000 0000 0000 009a 0000 0012  ................
-00004b70: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
-00004b80: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
-00004b90: 006c 0073 6473 636c 626f 6f6c 0000 0000  .l.sdsclbool....
-00004ba0: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
-00004bb0: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
-00004bc0: 6f00 6c00 736c 6731 5363 6f6d 7000 0000  o.l.slg1Scomp...
-00004bd0: 0000 019d 6000 0000 1200 6200 6f00 7500  ....`.....b.o.u.
-00004be0: 6e00 6400 6900 6e00 6700 5f00 6200 6f00  n.d.i.n.g._.b.o.
-00004bf0: 7800 5f00 7400 6f00 6f00 6c00 736c 7376  x._.t.o.o.l.slsv
-00004c00: 4362 6c6f 6200 0002 7962 706c 6973 7430  Cblob...ybplist0
-00004c10: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
-00004c20: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
-00004c30: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-00004c40: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-00004c50: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-00004c60: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-00004c70: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-00004c80: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-00004c90: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
-00004ca0: 3237 3c41 d40d 0e0f 100a 120a 1457 7669  27<A.........Wvi
-00004cb0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-00004cc0: 6e64 696e 675a 6964 656e 7469 6669 6572  ndingZidentifier
-00004cd0: 0911 01c7 0954 6e61 6d65 d40d 0e0f 1016  .....Tname......
-00004ce0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
-00004cf0: d40d 0e0f 100a 1c16 1e09 10b5 085c 6461  .............\da
-00004d00: 7465 4d6f 6469 6669 6564 d40d 0e0f 1016  teModified......
-00004d10: 1c16 2208 085b 6461 7465 4372 6561 7465  .."..[dateCreate
-00004d20: 64d4 0d0e 0f10 0a25 1627 0910 6108 5473  d......%.'..a.Ts
-00004d30: 697a 65d4 0d0e 0f10 0a2a 0a2c 0910 7309  ize......*.,..s.
-00004d40: 546b 696e 64d4 0d0e 0f10 162f 0a31 0810  Tkind....../.1..
-00004d50: 6409 556c 6162 656c d40d 0e0f 1016 340a  d.Ulabel......4.
-00004d60: 3608 104b 0957 7665 7273 696f 6ed4 0d0e  6..K.Wversion...
-00004d70: 0f10 1639 0a3b 0811 012c 0958 636f 6d6d  ...9.;...,.Xcomm
-00004d80: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
-00004d90: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00004da0: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
-00004db0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00004dc0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00004dd0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-00004de0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
-00004df0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
-00004e00: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
-00004e10: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
-00004e20: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
-00004e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00004e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00004e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00004e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00004e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00004e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00004b20: 095f 1019 7b7b 3335 342c 2031 3234 7d2c  ._..{{354, 124},
+00004b30: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
+00004b40: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
+00004b50: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+00004b60: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
+00004b70: 1200 6200 6f00 7500 6e00 6400 6900 6e00  ..b.o.u.n.d.i.n.
+00004b80: 6700 5f00 6200 6f00 7800 5f00 7400 6f00  g._.b.o.x._.t.o.
+00004b90: 6f00 6c00 7364 7363 6c62 6f6f 6c00 0000  o.l.sdsclbool...
+00004ba0: 0012 0062 006f 0075 006e 0064 0069 006e  ...b.o.u.n.d.i.n
+00004bb0: 0067 005f 0062 006f 0078 005f 0074 006f  .g._.b.o.x._.t.o
+00004bc0: 006f 006c 0073 6c67 3153 636f 6d70 0000  .o.l.slg1Scomp..
+00004bd0: 0000 0001 9d60 0000 0012 0062 006f 0075  .....`.....b.o.u
+00004be0: 006e 0064 0069 006e 0067 005f 0062 006f  .n.d.i.n.g._.b.o
+00004bf0: 0078 005f 0074 006f 006f 006c 0073 6c73  .x._.t.o.o.l.sls
+00004c00: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
+00004c10: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
+00004c20: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
+00004c30: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00004c40: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00004c50: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00004c60: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00004c70: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
+00004c80: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
+00004c90: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
+00004ca0: 2d32 373c 41d4 0d0e 0f10 0a12 0a14 5776  -27<A.........Wv
+00004cb0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00004cc0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
+00004cd0: 7209 1101 c709 546e 616d 65d4 0d0e 0f10  r.....Tname.....
+00004ce0: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
+00004cf0: 79d4 0d0e 0f10 0a1c 161e 0910 b508 5c64  y.............\d
+00004d00: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
+00004d10: 161c 1622 0808 5b64 6174 6543 7265 6174  ..."..[dateCreat
+00004d20: 6564 d40d 0e0f 100a 2516 2709 1061 0854  ed......%.'..a.T
+00004d30: 7369 7a65 d40d 0e0f 100a 2a0a 2c09 1073  size......*.,..s
+00004d40: 0954 6b69 6e64 d40d 0e0f 1016 2f0a 3108  .Tkind....../.1.
+00004d50: 1064 0955 6c61 6265 6cd4 0d0e 0f10 1634  .d.Ulabel......4
+00004d60: 0a36 0810 4b09 5776 6572 7369 6f6e d40d  .6..K.Wversion..
+00004d70: 0e0f 1016 390a 3b08 1101 2c09 5863 6f6d  ....9.;...,.Xcom
+00004d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
+00004d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00004da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
+00004db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00004dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
+00004dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+00004de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
+00004df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
+00004e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
+00004e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
+00004e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
+00004e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
+00004e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
+00004e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00004e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00004e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00004e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
 00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1351,170 +1351,170 @@
 00005460: 6200 0000 087e 81a5 d736 fec4 4100 0000  b....~...6..A...
 00005470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
 00005480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
 00005490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
 000054a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
 000054b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
 000054c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000054d0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
+000054d0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
 000054e0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 000054f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00005500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00005510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00005520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00005530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00005540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00005550: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-00005560: 7b7b 3333 352c 2031 3938 7d2c 207b 3932  {{335, 198}, {92
-00005570: 372c 2035 3638 7d7d 0908 1725 313d 4960  7, 568}}...%1=I`
-00005580: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-00005590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000055a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
-000055b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
-000055c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
-000055d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
-000055e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-000055f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-00005600: 0000 037a 7d00 0000 0f00 6400 6100 7400  ...z}.....d.a.t.
-00005610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
-00005620: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
-00005630: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
-00005640: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
-00005650: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00005660: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-00005670: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00005680: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00005690: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-000056a0: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
-000056b0: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
-000056c0: 0109 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
-000056d0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-000056e0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-000056f0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-00005700: 01c7 0909 d410 0e0f 0d16 1716 1908 1023  ...............#
-00005710: 0858 7562 6971 7569 7479 d40d 0e0f 101b  .Xubiquity......
-00005720: 1c16 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00005730: 10b5 0809 d40d 0e0f 1020 1c16 165b 6461  ......... ...[da
-00005740: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
-00005750: 2425 160a 5473 697a 6510 6108 09d4 0d0e  $%..Tsize.a.....
-00005760: 0f10 292a 0a0a 546b 696e 6410 7309 09d4  ..)*..Tkind.s...
-00005770: 0d0e 0f10 2e2f 0a16 556c 6162 656c 1064  ...../..Ulabel.d
-00005780: 0908 d40d 0e0f 1033 340a 1657 7665 7273  .......34..Wvers
-00005790: 696f 6e10 4b09 08d4 0d0e 0f10 3839 0a16  ion.K.......89..
-000057a0: 5863 6f6d 6d65 6e74 7311 012c 0908 d40d  Xcomments..,....
-000057b0: 0e0f 103d 3e16 165e 6461 7465 4c61 7374  ...=>..^dateLast
-000057c0: 4f70 656e 6564 10c8 0808 d410 0e0f 0d16  Opened..........
-000057d0: 1c16 4408 0859 6461 7465 4164 6465 6408  ..D..YdateAdded.
-000057e0: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
-000057f0: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
-00005800: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
-00005810: 0079 008c 008e 008f 009b 00a4 00af 00b5  .y..............
-00005820: 00bf 00c7 00cc 00cf 00d0 00d1 00da 00db  ................
-00005830: 00dd 00de 00e7 00f0 00fd 00ff 0100 0101  ................
-00005840: 010a 0116 0117 0118 0121 0126 0128 0129  .........!.&.(.)
-00005850: 012a 0133 0138 013a 013b 013c 0145 014b  .*.3.8.:.;.<.E.K
-00005860: 014d 014e 014f 0158 0160 0162 0163 0164  .M.N.O.X.`.b.c.d
-00005870: 016d 0176 0179 017a 017b 0184 0193 0195  .m.v.y.z.{......
-00005880: 0196 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
-00005890: 01c3 01cc 0000 0000 0000 0201 0000 0000  ................
-000058a0: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-000058b0: 0000 01cd 0000 000f 0064 0061 0074 0061  .........d.a.t.a
-000058c0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-000058d0: 006f 0072 0073 6c73 7670 626c 6f62 0000  .o.r.slsvpblob..
-000058e0: 0266 6270 6c69 7374 3030 d801 0203 0405  .fbplist00......
-000058f0: 0607 0809 0a0b 1a45 4647 0a5f 1012 7669  .......EFG._..vi
-00005900: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00005910: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00005920: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00005930: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
-00005940: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
-00005950: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
-00005960: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
-00005970: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
-00005980: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
-00005990: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
-000059a0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
-000059b0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
-000059c0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
-000059d0: 6d65 d416 1718 191a 1b0a 1d57 7669 7369  me.........Wvisi
-000059e0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-000059f0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
-00005a00: d416 1718 191a 201a 2208 10c8 0810 08d4  ...... .".......
-00005a10: 1617 1819 0a25 1a09 0910 b508 d416 1718  .....%..........
-00005a20: 191a 251a 2a08 0810 02d4 1617 1819 0a2d  ..%.*..........-
-00005a30: 1a2f 0910 6108 1003 d416 1718 191a 320a  ./..a.........2.
-00005a40: 3408 1064 0910 05d4 1617 1819 0a37 0a39  4..d.........7.9
-00005a50: 0910 7309 1004 d416 1718 191a 3c0a 3e08  ..s.........<.>.
-00005a60: 104b 0910 06d4 1617 1819 0a41 0a43 0911  .K.........A.C..
-00005a70: 01c7 0910 0008 2340 2800 0000 0000 005c  ......#@(......\
-00005a80: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
-00005a90: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
-00005aa0: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
-00005ab0: 00ab 00ba 00c7 00d3 00d8 00de 00e3 00eb  ................
-00005ac0: 00f0 00f9 0101 0107 0111 0117 0118 011b  ................
-00005ad0: 011c 011e 0127 0128 012a 012b 012d 0136  .....'.(.*.+.-.6
-00005ae0: 0137 0139 013a 0143 0144 0145 0147 0150  .7.9.:.C.D.E.G.P
-00005af0: 0151 0153 0154 0156 015f 0160 0162 0163  .Q.S.T.V._.`.b.c
-00005b00: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
-00005b10: 0180 0181 0183 018c 018d 0190 0191 0193  ................
-00005b20: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
-00005b30: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-00005b40: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
-00005b50: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
-00005b60: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00005b70: 6f62 0000 0008 1421 9b0e 8b0e c541 0000  ob.....!.....A..
-00005b80: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
-00005b90: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
-00005ba0: 6d6f 6444 626c 6f62 0000 0008 1421 9b0e  modDblob.....!..
-00005bb0: 8b0e c541 0000 000f 0064 0061 0074 0061  ...A.....d.a.t.a
-00005bc0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-00005bd0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
-00005be0: 0000 0004 7000 0000 000f 0064 0061 0074  ....p......d.a.t
-00005bf0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
-00005c00: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
-00005c10: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
-00005c20: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
-00005c30: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
-00005c40: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
-00005c50: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
-00005c60: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00005c70: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
-00005c80: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00005c90: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00005ca0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00005cb0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00005cc0: 7208 0809 0809 5f10 187b 7b33 3335 2c20  r....._..{{335, 
-00005cd0: 3139 387d 2c20 7b39 3237 2c20 3536 387d  198}, {927, 568}
-00005ce0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00005cf0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
-00005d00: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00005d10: 9a00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
-00005d20: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-00005d30: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
-00005d40: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
-00005d50: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
-00005d60: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d70: 6d70 0000 0000 0008 ae3a 0958 636f 6d6d  mp.......:.Xcomm
-00005d80: 656e 7473 d40d 0e0f 1016 3e16 4008 10c8  ents......>.@...
-00005d90: 085e 6461 7465 4c61 7374 4f70 656e 6564  .^dateLastOpened
-00005da0: d40d 0e0f 1016 1c16 4408 0859 6461 7465  ........D..Ydate
-00005db0: 4164 6465 6408 2340 2800 0000 0000 0054  Added.#@(......T
-00005dc0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
-00005dd0: 0019 002e 0040 0048 005c 0065 0070 0079  .....@.H.\.e.p.y
-00005de0: 008c 008e 008f 009b 00a4 00ac 00b2 00bc  ................
-00005df0: 00c7 00c8 00cb 00cc 00d1 00da 00db 00dd  ................
-00005e00: 00de 00e7 00f0 00f1 00f3 00f4 0101 010a  ................
-00005e10: 010b 010c 0118 0121 0122 0124 0125 012a  .......!.".$.%.*
-00005e20: 0133 0134 0136 0137 013c 0145 0146 0148  .3.4.6.7.<.E.F.H
-00005e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00005e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00005e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00005e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00005e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00005e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00005550: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00005560: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00005570: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+00005580: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
+000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
+000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
+000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
+000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
+00005600: 0000 0003 9607 0000 000f 0064 0061 0074  ...........d.a.t
+00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
+00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
+00005630: 0000 0281 6270 6c69 7374 3030 d801 0203  ....bplist00....
+00005640: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
+00005650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00005660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00005670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00005680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00005690: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+000056a0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+000056b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000056c0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
+000056d0: 0d0e 0f10 1112 0a0a 5a69 6465 6e74 6966  ........Zidentif
+000056e0: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
+000056f0: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
+00005700: 1101 c709 09d4 100e 0f0d 1617 1619 0810  ................
+00005710: 2308 5875 6269 7175 6974 79d4 0d0e 0f10  #.Xubiquity.....
+00005720: 1b1c 160a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00005730: 6410 b508 09d4 0d0e 0f10 201c 1616 5b64  d......... ...[d
+00005740: 6174 6543 7265 6174 6564 0808 d40d 0e0f  ateCreated......
+00005750: 1024 2516 0a54 7369 7a65 1061 0809 d40d  .$%..Tsize.a....
+00005760: 0e0f 1029 2a0a 0a54 6b69 6e64 1073 0909  ...)*..Tkind.s..
+00005770: d40d 0e0f 102e 2f0a 1655 6c61 6265 6c10  ....../..Ulabel.
+00005780: 6409 08d4 0d0e 0f10 3334 0a16 5776 6572  d.......34..Wver
+00005790: 7369 6f6e 104b 0908 d40d 0e0f 1038 390a  sion.K.......89.
+000057a0: 1658 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
+000057b0: 0d0e 0f10 3d3e 1616 5e64 6174 654c 6173  ....=>..^dateLas
+000057c0: 744f 7065 6e65 6410 c808 08d4 100e 0f0d  tOpened.........
+000057d0: 161c 1644 0808 5964 6174 6541 6464 6564  ...D..YdateAdded
+000057e0: 0823 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+000057f0: 6f64 6966 6965 6423 4030 0000 0000 0000  odified#@0......
+00005800: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+00005810: 7000 7900 8c00 8e00 8f00 9b00 a400 af00  p.y.............
+00005820: b500 bf00 c700 cc00 cf00 d000 d100 da00  ................
+00005830: db00 dd00 de00 e700 f000 fd00 ff01 0001  ................
+00005840: 0101 0a01 1601 1701 1801 2101 2601 2801  ..........!.&.(.
+00005850: 2901 2a01 3301 3801 3a01 3b01 3c01 4501  ).*.3.8.:.;.<.E.
+00005860: 4b01 4d01 4e01 4f01 5801 6001 6201 6301  K.M.N.O.X.`.b.c.
+00005870: 6401 6d01 7601 7901 7a01 7b01 8401 9301  d.m.v.y.z.{.....
+00005880: 9501 9601 9701 a001 a101 a201 ac01 ad01  ................
+00005890: b601 c301 cc00 0000 0000 0002 0100 0000  ................
+000058a0: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
+000058b0: 0000 0001 cd00 0000 0f00 6400 6100 7400  ..........d.a.t.
+000058c0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+000058d0: 7300 6f00 7200 736c 7376 7062 6c6f 6200  s.o.r.slsvpblob.
+000058e0: 0002 6662 706c 6973 7430 30d8 0102 0304  ..fbplist00.....
+000058f0: 0506 0708 090a 0b1a 4546 470a 5f10 1276  ........EFG._..v
+00005900: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00005910: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00005920: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00005930: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00005940: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00005950: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+00005960: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+00005970: 0109 d90c 0d0e 0f10 1112 1314 151e 2327  ..............#'
+00005980: 2b30 353a 3f58 636f 6d6d 656e 7473 5e64  +05:?Xcomments^d
+00005990: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+000059a0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+000059b0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+000059c0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+000059d0: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
+000059e0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+000059f0: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00005a00: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
+00005a10: d416 1718 190a 251a 0909 10b5 08d4 1617  ......%.........
+00005a20: 1819 1a25 1a2a 0808 1002 d416 1718 190a  ...%.*..........
+00005a30: 2d1a 2f09 1061 0810 03d4 1617 1819 1a32  -./..a.........2
+00005a40: 0a34 0810 6409 1005 d416 1718 190a 370a  .4..d.........7.
+00005a50: 3909 1073 0910 04d4 1617 1819 1a3c 0a3e  9..s.........<.>
+00005a60: 0810 4b09 1006 d416 1718 190a 410a 4309  ..K.........A.C.
+00005a70: 1101 c709 1000 0823 4028 0000 0000 0000  .......#@(......
+00005a80: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
+00005a90: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
+00005aa0: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
+00005ab0: a200 ab00 ba00 c700 d300 d800 de00 e300  ................
+00005ac0: eb00 f000 f901 0101 0701 1101 1701 1801  ................
+00005ad0: 1b01 1c01 1e01 2701 2801 2a01 2b01 2d01  ......'.(.*.+.-.
+00005ae0: 3601 3701 3901 3a01 4301 4401 4501 4701  6.7.9.:.C.D.E.G.
+00005af0: 5001 5101 5301 5401 5601 5f01 6001 6201  P.Q.S.T.V._.`.b.
+00005b00: 6301 6501 6e01 6f01 7101 7201 7401 7d01  c.e.n.o.q.r.t.}.
+00005b10: 7e01 8001 8101 8301 8c01 8d01 9001 9101  ~...............
+00005b20: 9301 9401 9d01 aa01 b300 0000 0000 0002  ................
+00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
+00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
+00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
+00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
+00005b70: 6c6f 6200 0000 0826 8880 05f4 11c5 4100  lob....&......A.
+00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
+00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
+00005ba0: 736d 6f64 4462 6c6f 6200 0000 08b3 69d3  smodDblob.....i.
+00005bb0: 74cd 0fc5 4100 0000 0f00 6400 6100 7400  t...A.....d.a.t.
+00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
+00005be0: 0000 0000 0480 0000 0000 0f00 6400 6100  ............d.a.
+00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
+00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
+00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
+00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
+00005c30: 7200 6100 6300 7400 6f00 7200 7362 7773  r.a.c.t.o.r.sbws
+00005c40: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
+00005c50: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
+00005c60: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00005c70: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
+00005c80: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
+00005c90: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
+00005ca0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
+00005cb0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
+00005cc0: 6172 0808 0908 095f 1018 7b7b 3333 352c  ar....._..{{335,
+00005cd0: 2031 3938 7d2c 207b 3932 372c 2035 3638   198}, {927, 568
+00005ce0: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00005cf0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
+00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
+00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
+00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
+00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
+00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
+00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
+00005d70: 6f6d 7000 0000 0000 08ae 3a09 5863 6f6d  omp.......:.Xcom
+00005d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
+00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
+00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
+00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
+00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
+00005df0: bc00 c700 c800 cb00 cc00 d100 da00 db00  ................
+00005e00: dd00 de00 e700 f000 f100 f300 f401 0101  ................
+00005e10: 0a01 0b01 0c01 1801 2101 2201 2401 2501  ........!.".$.%.
+00005e20: 2a01 3301 3401 3601 3701 3c01 4501 4601  *.3.4.6.7.<.E.F.
+00005e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
+00005e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
+00005e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00005e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00005e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00005e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
 00005e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1607,15 +1607,15 @@
 00006460: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
 00006470: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
 00006480: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
 00006490: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 000064a0: 0000 0000 0000 0000 0000 009a 0000 0009  ................
 000064b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
 000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0001  .glg1Scomp......
-000064d0: 8eb7 0000 0009 006c 0061 0062 0065 006c  .......l.a.b.e.l
+000064d0: 9f8d 0000 0009 006c 0061 0062 0065 006c  .......l.a.b.e.l
 000064e0: 006c 0069 006e 0067 6c73 7643 626c 6f62  .l.i.n.glsvCblob
 000064f0: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
 00006500: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00006510: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00006520: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00006530: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00006540: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -1690,87 +1690,87 @@
 00006990: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
 000069a0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
 000069b0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
 000069c0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
 000069d0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 000069e0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000069f0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 08ed  n.gmoDDblob.....
-00006a10: 41b1 f1cc 0cc5 4100 0000 0900 6c00 6100  A.....A.....l.a.
+00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 0854  n.gmoDDblob....T
+00006a10: 1422 3e3d 0fc5 4100 0000 0900 6c00 6100  .">=..A.....l.a.
 00006a20: 6200 6500 6c00 6c00 6900 6e00 676d 6f64  b.e.l.l.i.n.gmod
-00006a30: 4462 6c6f 6200 0000 08ed 41b1 f1cc 0cc5  Dblob.....A.....
+00006a30: 4462 6c6f 6200 0000 0854 1422 3e3d 0fc5  Dblob....T.">=..
 00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
 00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
-00006a60: 0000 0000 01d0 0000 0000 0900 6c00 6100  ............l.a.
+00006a60: 0000 0000 01e0 0000 0000 0900 6c00 6100  ............l.a.
 00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
 00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
 00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
-00006aa0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+00006aa0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
 00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
 00006ae0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
 00006af0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
 00006b00: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00006b20: 0908 095f 1018 7b7b 3333 352c 2031 3938  ..._..{{335, 198
-00006b30: 7d2c 207b 3932 372c 2035 3638 7d7d 0908  }, {927, 568}}..
-00006b40: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
-00006b50: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-00006b60: 0000 0000 0000 0000 0000 0000 009a 0000  ................
-00006b70: 0006 006d 0069 0078 0069 006e 0073 6c67  ...m.i.x.i.n.slg
-00006b80: 3153 636f 6d70 0000 0000 0007 e4c3 0000  1Scomp..........
-00006b90: 0006 006d 0069 0078 0069 006e 0073 6c73  ...m.i.x.i.n.sls
-00006ba0: 7643 626c 6f62 0000 0281 6270 6c69 7374  vCblob....bplist
-00006bb0: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00006bc0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00006bd0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00006be0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00006bf0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00006c00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00006c10: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00006c20: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00006c30: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-00006c40: 2d32 373c 41d4 0d0e 0f10 1112 0a0a 5a69  -27<A.........Zi
-00006c50: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
-00006c60: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00006c70: 6554 6e61 6d65 1101 c709 09d4 100e 0f0d  eTname..........
-00006c80: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00006c90: 79d4 0d0e 0f10 1b1c 160a 5c64 6174 654d  y.........\dateM
-00006ca0: 6f64 6966 6965 6410 b508 09d4 0d0e 0f10  odified.........
-00006cb0: 201c 1616 5b64 6174 6543 7265 6174 6564   ...[dateCreated
-00006cc0: 0808 d40d 0e0f 1024 2516 0a54 7369 7a65  .......$%..Tsize
-00006cd0: 1061 0809 d40d 0e0f 1029 2a0a 0a54 6b69  .a.......)*..Tki
-00006ce0: 6e64 1073 0909 d40d 0e0f 102e 2f0a 1655  nd.s......../..U
-00006cf0: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3334  label.d.......34
-00006d00: 0a16 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
-00006d10: 0e0f 1038 390a 1658 636f 6d6d 656e 7473  ...89..Xcomments
-00006d20: 1101 2c09 08d4 0d0e 0f10 3d3e 1616 5e64  ..,.......=>..^d
-00006d30: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
-00006d40: 08d4 100e 0f0d 161c 1644 0808 5964 6174  .........D..Ydat
-00006d50: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-00006d60: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
-00006d70: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
-00006d80: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
-00006d90: 9b00 a400 af00 b500 bf00 c700 cc00 cf00  ................
-00006da0: d000 d100 da00 db00 dd00 de00 e700 f000  ................
-00006db0: fd00 ff01 0001 0101 0a01 1601 1701 1801  ................
-00006dc0: 2101 2601 2801 2901 2a01 3301 3801 3a01  !.&.(.).*.3.8.:.
-00006dd0: 3b01 3c01 4501 4b01 4d01 4e01 4f01 5801  ;.<.E.K.M.N.O.X.
-00006de0: 6001 6201 6301 6401 6d01 7601 7901 7a01  `.b.c.d.m.v.y.z.
-00006df0: 7b01 8401 9301 9501 9601 9701 a001 a101  {...............
-00006e00: a201 ac01 ad01 b601 c301 cc00 0000 0000  ................
-00006e10: 0002 0100 0000 0000 0000 4a00 0000 0000  ..........J.....
-00006e20: 0000 0000 0000 0000 0001 cd45 0146 0148  ...........E.F.H
-00006e30: 0149 014f 0158 0159 015b 015c 0164 016d  .I.O.X.Y.[.\.d.m
-00006e40: 016e 0171 0172 017b 0184 0185 0187 0188  .n.q.r.{........
-00006e50: 0197 01a0 01a1 01a2 01ac 01ad 01b6 01bb  ................
-00006e60: 01c4 0000 0000 0000 0201 0000 0000 0000  ................
-00006e70: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00006e80: 01c5 0000 0000 0000 0000 0000 0000 0000  ................
+00006b20: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
+00006b30: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
+00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00006b60: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
+00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006b80: 6731 5363 6f6d 7000 0000 0000 0826 1f00  g1Scomp......&..
+00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
+00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
+00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00006c00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00006c10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+00006c20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+00006c30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+00006c40: 282d 3237 3c41 d40d 0e0f 1011 120a 0a5a  (-27<A.........Z
+00006c50: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+00006c60: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00006c70: 6c65 546e 616d 6511 01c7 0909 d410 0e0f  leTname.........
+00006c80: 0d16 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
+00006c90: 7479 d40d 0e0f 101b 1c16 0a5c 6461 7465  ty.........\date
+00006ca0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00006cb0: 1020 1c16 165b 6461 7465 4372 6561 7465  . ...[dateCreate
+00006cc0: 6408 08d4 0d0e 0f10 2425 160a 5473 697a  d.......$%..Tsiz
+00006cd0: 6510 6108 09d4 0d0e 0f10 292a 0a0a 546b  e.a.......)*..Tk
+00006ce0: 696e 6410 7309 09d4 0d0e 0f10 2e2f 0a16  ind.s......../..
+00006cf0: 556c 6162 656c 1064 0908 d40d 0e0f 1033  Ulabel.d.......3
+00006d00: 340a 1657 7665 7273 696f 6e10 4b09 08d4  4..Wversion.K...
+00006d10: 0d0e 0f10 3839 0a16 5863 6f6d 6d65 6e74  ....89..Xcomment
+00006d20: 7311 012c 0908 d40d 0e0f 103d 3e16 165e  s..,.......=>..^
+00006d30: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00006d40: 0808 d410 0e0f 0d16 1c16 4408 0859 6461  ..........D..Yda
+00006d50: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+00006d60: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
+00006d70: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
+00006d80: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
+00006d90: 009b 00a4 00af 00b5 00bf 00c7 00cc 00cf  ................
+00006da0: 00d0 00d1 00da 00db 00dd 00de 00e7 00f0  ................
+00006db0: 00fd 00ff 0100 0101 010a 0116 0117 0118  ................
+00006dc0: 0121 0126 0128 0129 012a 0133 0138 013a  .!.&.(.).*.3.8.:
+00006dd0: 013b 013c 0145 014b 014d 014e 014f 0158  .;.<.E.K.M.N.O.X
+00006de0: 0160 0162 0163 0164 016d 0176 0179 017a  .`.b.c.d.m.v.y.z
+00006df0: 017b 0184 0193 0195 0196 0197 01a0 01a1  .{..............
+00006e00: 01a2 01ac 01ad 01b6 01c3 01cc 0000 0000  ................
+00006e10: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+00006e20: 0000 0000 0000 0000 0000 01cd 4501 4601  ............E.F.
+00006e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
+00006e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
+00006e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
+00006e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
+00006e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
+00006e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 4c95 e52c 740e c541  blob....L..,t..A
+00007020: 626c 6f62 0000 0008 2594 dda2 e311 c541  blob....%......A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 5404 fa15  modDblob....T...
-00007050: cc0c c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 f794 ee44  modDblob.......D
+00007050: dd11 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0008 9000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0008 e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1902,204 +1902,204 @@
 000076d0: 626c 6f62 0000 0008 32f5 d3ed cc0c c541  blob....2......A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
 000076f0: 3153 636f 6d70 0000 0000 0001 6000 0000  1Scomp......`...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
-00007740: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00007740: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
 00007770: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
 00007780: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00007790: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 000077a0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 000077b0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-000077c0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
-000077d0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
-000077e0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
-000077f0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
-00007800: 0000 0000 0000 0000 0000 9a00 0000 0d00  ................
-00007810: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
-00007820: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
-00007830: 7000 0000 0000 00bd dd00 0000 0d00 6f00  p.............o.
-00007840: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
-00007850: 6f00 6f00 6c00 736c 7376 4362 6c6f 6200  o.o.l.slsvCblob.
-00007860: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
-00007870: 0506 0708 090a 0b0c 0d18 4849 484a 0c4c  ..........HIHJ.L
-00007880: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00007890: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-000078a0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-000078b0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-000078c0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
-000078d0: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
-000078e0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
-000078f0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00007900: 6552 656c 6174 6976 6544 6174 6573 5869  eRelativeDatesXi
-00007910: 636f 6e53 697a 6510 0109 ab0e 171c 2125  conSize.......!%
-00007920: 2a2f 3439 3e43 d40f 1011 1213 140c 0c5a  */49>C.........Z
-00007930: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-00007940: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00007950: 6c65 546e 616d 6511 01c7 0909 d412 1011  leTname.........
-00007960: 0f18 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
-00007970: 7479 d412 1011 0f0c 1e18 2009 10b5 085c  ty........ ....\
-00007980: 6461 7465 4d6f 6469 6669 6564 d412 1011  dateModified....
-00007990: 0f18 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
-000079a0: 7465 64d4 1210 110f 0c27 1829 0910 6108  ted......'.)..a.
-000079b0: 5473 697a 65d4 1210 110f 0c2c 0c2e 0910  Tsize......,....
-000079c0: 7309 546b 696e 64d4 1210 110f 1831 0c33  s.Tkind......1.3
-000079d0: 0810 6409 556c 6162 656c d412 1011 0f18  ..d.Ulabel......
-000079e0: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
-000079f0: 1210 110f 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
-00007a00: 6d6d 656e 7473 d412 1011 0f18 4018 4208  mments......@.B.
-00007a10: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
-00007a20: 6564 d412 1011 0f18 1e18 4608 0859 6461  ed........F..Yda
-00007a30: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
-00007a40: 0023 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
-00007a50: 2340 3000 0000 0000 0000 0800 1d00 3200  #@0...........2.
-00007a60: 4400 4c00 6000 7200 7b00 8d00 9800 ab00  D.L.`.r.{.......
-00007a70: b400 b600 b700 c300 cc00 d700 dd00 e700  ................
-00007a80: ef00 f400 f700 f800 f901 0201 0301 0501  ................
-00007a90: 0601 0f01 1801 1901 1b01 1c01 2901 3201  ............).2.
-00007aa0: 3301 3401 4001 4901 4a01 4c01 4d01 5201  3.4.@.I.J.L.M.R.
-00007ab0: 5b01 5c01 5e01 5f01 6401 6d01 6e01 7001  [.\.^._.d.m.n.p.
-00007ac0: 7101 7701 8001 8101 8301 8401 8c01 9501  q.w.............
-00007ad0: 9601 9901 9a01 a301 ac01 ad01 af01 b001  ................
-00007ae0: bf01 c801 c901 ca01 d401 d501 de01 e701  ................
-00007af0: ec01 ed00 0000 0000 0002 0100 0000 0000  ................
-00007b00: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00007b10: 0001 f600 0000 0d00 6f00 7500 7400 6c00  ........o.u.t.l.
-00007b20: 6900 6500 7200 5f00 7400 6f00 6f00 6c00  i.e.r._.t.o.o.l.
-00007b30: 736c 7376 7062 6c6f 6200 0002 9562 706c  slsvpblob....bpl
-00007b40: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
-00007b50: 0b0c 0d1f 4748 4749 0c4b 5f10 1276 6965  ....GHGI.K_..vie
-00007b60: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
-00007b70: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
-00007b80: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
-00007b90: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
-00007ba0: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
-00007bb0: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
-00007bc0: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
-00007bd0: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00007be0: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00007bf0: 6510 0109 d90e 0f10 1112 1314 1516 1720  e.............. 
-00007c00: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
-00007c10: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
-00007c20: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
-00007c30: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
-00007c40: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
-00007c50: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5569  Tname.........Ui
-00007c60: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
-00007c70: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
-00007c80: 2c09 08d4 1819 1a1b 2122 1f1f 1008 10c8  ,.......!"......
-00007c90: 0808 d418 191a 1b0b 261f 0c10 b508 09d4  ........&.......
-00007ca0: 1819 1a1b 2a26 1f1f 1002 0808 d418 191a  ....*&..........
-00007cb0: 1b2e 2f1f 0c10 0310 6108 09d4 1819 1a1b  ../.....a.......
-00007cc0: 3334 0c1f 1005 1064 0908 d418 191a 1b38  34.....d.......8
-00007cd0: 390c 0c10 0410 7309 09d4 1819 1a1b 3d3e  9.....s.......=>
-00007ce0: 0c1f 1006 104b 0908 d41b 191a 180c 430c  .....K........C.
-00007cf0: 4509 1101 c709 1000 0823 0000 0000 0000  E........#......
-00007d00: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
-00007d10: 0923 4030 0000 0000 0000 0008 001d 0032  .#@0...........2
-00007d20: 0044 004c 0060 0072 007b 008d 0098 00ab  .D.L.`.r.{......
-00007d30: 00b4 00b6 00b7 00ca 00d3 00e2 00ef 00fb  ................
-00007d40: 0100 0106 010b 0113 0118 0121 0127 012d  ...........!.'.-
-00007d50: 0137 013f 0141 0144 0145 0146 014f 0151  .7.?.A.D.E.F.O.Q
-00007d60: 0153 0154 0155 015e 0160 0161 0162 016b  .S.T.U.^.`.a.b.k
-00007d70: 016d 016e 016f 0178 017a 017c 017d 017e  .m.n.o.x.z.|.}.~
-00007d80: 0187 0189 018b 018c 018d 0196 0198 019a  ................
-00007d90: 019b 019c 01a5 01a7 01a9 01aa 01ab 01b4  ................
-00007da0: 01b5 01b8 01b9 01bb 01bc 01c5 01ce 01d3  ................
-00007db0: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
-00007dc0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
-00007dd0: 01dd 0000 000d 006f 0075 0074 006c 0069  .......o.u.t.l.i
-00007de0: 0065 0072 005f 0074 006f 006f 006c 0073  .e.r._.t.o.o.l.s
-00007df0: 6d6f 4444 626c 6f62 0000 0008 cf5e 2d04  moDDblob.....^-.
-00007e00: 750e c541 0000 000d 006f 0075 0074 006c  u..A.....o.u.t.l
-00007e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00007e20: 0073 6d6f 6444 626c 6f62 0000 0008 bea6  .smodDblob......
-00007e30: cfed cc0c c541 0000 000d 006f 0075 0074  .....A.....o.u.t
-00007e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00007e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
-00007e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
-00007e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00007e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
-00007e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
-00007ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00007eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00007ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00007ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00007ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00007ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00007f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00007f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00007f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00007f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
-00007f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
-00007f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00007f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00007f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
-00007f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00007f90: 6f6d 7000 0000 0000 08bf a300 0000 0000  omp.............
+000077c0: 5f10 197b 7b33 3534 2c20 3132 347d 2c20  _..{{354, 124}, 
+000077d0: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
+000077e0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+000077f0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00007800: 0000 0000 0000 0000 0000 009b 0000 000d  ................
+00007810: 006f 0075 0074 006c 0069 0065 0072 005f  .o.u.t.l.i.e.r._
+00007820: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
+00007830: 6d70 0000 0000 0000 bdd1 0000 000d 006f  mp.............o
+00007840: 0075 0074 006c 0069 0065 0072 005f 0074  .u.t.l.i.e.r._.t
+00007850: 006f 006f 006c 0073 6c73 7643 626c 6f62  .o.o.l.slsvCblob
+00007860: 0000 02b0 6270 6c69 7374 3030 da01 0203  ....bplist00....
+00007870: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
+00007880: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
+00007890: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
+000078a0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+000078b0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+000078c0: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
+000078d0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
+000078e0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
+000078f0: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
+00007900: 7365 5265 6c61 7469 7665 4461 7465 7358  seRelativeDatesX
+00007910: 6963 6f6e 5369 7a65 1001 09ab 0e17 1c21  iconSize.......!
+00007920: 252a 2f34 393e 43d4 0f10 1112 1314 0c0c  %*/49>C.........
+00007930: 5a69 6465 6e74 6966 6965 7255 7769 6474  ZidentifierUwidt
+00007940: 6859 6173 6365 6e64 696e 6757 7669 7369  hYascendingWvisi
+00007950: 626c 6554 6e61 6d65 1101 c709 09d4 1210  bleTname........
+00007960: 110f 1819 181b 0810 2308 5875 6269 7175  ........#.Xubiqu
+00007970: 6974 79d4 1210 110f 0c1e 1820 0910 b508  ity........ ....
+00007980: 5c64 6174 654d 6f64 6966 6965 64d4 1210  \dateModified...
+00007990: 110f 181e 1824 0808 5b64 6174 6543 7265  .....$..[dateCre
+000079a0: 6174 6564 d412 1011 0f0c 2718 2909 1061  ated......'.)..a
+000079b0: 0854 7369 7a65 d412 1011 0f0c 2c0c 2e09  .Tsize......,...
+000079c0: 1073 0954 6b69 6e64 d412 1011 0f18 310c  .s.Tkind......1.
+000079d0: 3308 1064 0955 6c61 6265 6cd4 1210 110f  3..d.Ulabel.....
+000079e0: 1836 0c38 0810 4b09 5776 6572 7369 6f6e  .6.8..K.Wversion
+000079f0: d412 1011 0f18 3b0c 3d08 1101 2c09 5863  ......;.=...,.Xc
+00007a00: 6f6d 6d65 6e74 73d4 1210 110f 1840 1842  omments......@.B
+00007a10: 0810 c808 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
+00007a20: 6e65 64d4 1210 110f 181e 1846 0808 5964  ned........F..Yd
+00007a30: 6174 6541 6464 6564 0823 0000 0000 0000  ateAdded.#......
+00007a40: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00007a50: 0923 4030 0000 0000 0000 0008 001d 0032  .#@0...........2
+00007a60: 0044 004c 0060 0072 007b 008d 0098 00ab  .D.L.`.r.{......
+00007a70: 00b4 00b6 00b7 00c3 00cc 00d7 00dd 00e7  ................
+00007a80: 00ef 00f4 00f7 00f8 00f9 0102 0103 0105  ................
+00007a90: 0106 010f 0118 0119 011b 011c 0129 0132  .............).2
+00007aa0: 0133 0134 0140 0149 014a 014c 014d 0152  .3.4.@.I.J.L.M.R
+00007ab0: 015b 015c 015e 015f 0164 016d 016e 0170  .[.\.^._.d.m.n.p
+00007ac0: 0171 0177 0180 0181 0183 0184 018c 0195  .q.w............
+00007ad0: 0196 0199 019a 01a3 01ac 01ad 01af 01b0  ................
+00007ae0: 01bf 01c8 01c9 01ca 01d4 01d5 01de 01e7  ................
+00007af0: 01ec 01ed 0000 0000 0000 0201 0000 0000  ................
+00007b00: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+00007b10: 0000 01f6 0000 000d 006f 0075 0074 006c  .........o.u.t.l
+00007b20: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00007b30: 0073 6c73 7670 626c 6f62 0000 0295 6270  .slsvpblob....bp
+00007b40: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
+00007b50: 0a0b 0c0d 1f47 4847 490c 4b5f 1012 7669  .....GHGI.K_..vi
+00007b60: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00007b70: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00007b80: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00007b90: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+00007ba0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+00007bb0: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+00007bc0: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+00007bd0: 436f 6c75 6d6e 5f10 1075 7365 5265 6c61  Column_..useRela
+00007be0: 7469 7665 4461 7465 7358 6963 6f6e 5369  tiveDatesXiconSi
+00007bf0: 7a65 1001 09d9 0e0f 1011 1213 1415 1617  ze..............
+00007c00: 2025 292d 3237 3c41 5863 6f6d 6d65 6e74   %)-27<AXcomment
+00007c10: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
+00007c20: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
+00007c30: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
+00007c40: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
+00007c50: 6e54 6e61 6d65 d418 191a 1b1c 1d0c 1f55  nTname.........U
+00007c60: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
+00007c70: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
+00007c80: 012c 0908 d418 191a 1b21 221f 1f10 0810  .,.......!".....
+00007c90: c808 08d4 1819 1a1b 0b26 1f0c 10b5 0809  .........&......
+00007ca0: d418 191a 1b2a 261f 1f10 0208 08d4 1819  .....*&.........
+00007cb0: 1a1b 2e2f 1f0c 1003 1061 0809 d418 191a  .../.....a......
+00007cc0: 1b33 340c 1f10 0510 6409 08d4 1819 1a1b  .34.....d.......
+00007cd0: 3839 0c0c 1004 1073 0909 d418 191a 1b3d  89.....s.......=
+00007ce0: 3e0c 1f10 0610 4b09 08d4 1b19 1a18 0c43  >.....K........C
+00007cf0: 0c45 0911 01c7 0910 0008 2300 0000 0000  .E........#.....
+00007d00: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00007d10: 6509 2340 3000 0000 0000 0000 0800 1d00  e.#@0...........
+00007d20: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
+00007d30: ab00 b400 b600 b700 ca00 d300 e200 ef00  ................
+00007d40: fb01 0001 0601 0b01 1301 1801 2101 2701  ............!.'.
+00007d50: 2d01 3701 3f01 4101 4401 4501 4601 4f01  -.7.?.A.D.E.F.O.
+00007d60: 5101 5301 5401 5501 5e01 6001 6101 6201  Q.S.T.U.^.`.a.b.
+00007d70: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
+00007d80: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
+00007d90: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
+00007da0: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
+00007db0: d301 d400 0000 0000 0002 0100 0000 0000  ................
+00007dc0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
+00007dd0: 0001 dd00 0000 0d00 6f00 7500 7400 6c00  ........o.u.t.l.
+00007de0: 6900 6500 7200 5f00 7400 6f00 6f00 6c00  i.e.r._.t.o.o.l.
+00007df0: 736d 6f44 4462 6c6f 6200 0000 0845 bf9c  smoDDblob....E..
+00007e00: d4d3 0fc5 4100 0000 0d00 6f00 7500 7400  ....A.....o.u.t.
+00007e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00007e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08be  l.smodDblob.....
+00007e30: a6cf edcc 0cc5 4100 0000 0d00 6f00 7500  ......A.....o.u.
+00007e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
+00007e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
+00007e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00007e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00007e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
+00007e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
+00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
+00007eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00007ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00007ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00007ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00007ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00007f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00007f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00007f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00007f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00007f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+00007f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00007f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+00007f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
+00007f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
+00007f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
 00008010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00008020: 6c73 7670 626c 6f62 0000 029d 6270 6c69  lsvpblob....bpli
 00008030: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00008040: 0b0d 1f48 4948 4a4b 265f 1010 7573 6552  ...HIHJK&_..useR
-00008050: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
-00008060: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
-00008070: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
-00008080: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
-00008090: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
-000080a0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
-000080b0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
-000080c0: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
-000080d0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-000080e0: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
-000080f0: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
-00008100: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-00008110: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-00008120: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00008130: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00008140: 616d 65d4 1819 1a1b 1c1d 0b1f 5569 6e64  ame.........Uind
-00008150: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
-00008160: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
-00008170: 08d4 1819 1a1b 2122 1f1f 1008 10c8 0808  ......!"........
-00008180: d418 191a 1b26 271f 0b10 0110 b508 09d4  .....&'.........
-00008190: 1819 1a1b 2b27 1f1f 1002 0808 d418 191a  ....+'..........
-000081a0: 1b2f 301f 0b10 0310 6108 09d4 1819 1a1b  ./0.....a.......
-000081b0: 3435 0b1f 1005 1064 0908 d418 191a 1b39  45.....d.......9
-000081c0: 3a0b 0b10 0410 7309 09d4 1819 1a1b 3e3f  :.....s.......>?
-000081d0: 0b1f 1006 104b 0908 d418 191a 1b43 440b  .....K.......CD.
-000081e0: 0b10 0011 01c7 0909 0823 0000 0000 0000  .........#......
-000081f0: 0000 2340 2800 0000 0000 005c 6461 7465  ..#@(......\date
-00008200: 4d6f 6469 6669 6564 2340 3000 0000 0000  Modified#@0.....
-00008210: 0000 0800 1d00 3000 4200 4a00 5e00 7000  ......0.B.J.^.p.
-00008220: 7900 8b00 9600 9f00 b400 b500 b600 c900  y...............
-00008230: d200 e100 ee00 fa00 ff01 0501 0a01 1201  ................
-00008240: 1701 2001 2601 2c01 3601 3e01 4001 4301  .. .&.,.6.>.@.C.
-00008250: 4401 4501 4e01 5001 5201 5301 5401 5d01  D.E.N.P.R.S.T.].
-00008260: 5f01 6101 6201 6301 6c01 6e01 6f01 7001  _.a.b.c.l.n.o.p.
-00008270: 7901 7b01 7d01 7e01 7f01 8801 8a01 8c01  y.{.}.~.........
-00008280: 8d01 8e01 9701 9901 9b01 9c01 9d01 a601  ................
-00008290: a801 aa01 ab01 ac01 b501 b701 ba01 bb01  ................
-000082a0: bc01 bd01 c601 cf01 dc00 0000 0000 0002  ................
+00008040: 0c0d 1f47 4847 494a 0c5f 1012 7669 6577  ...GHGIJ._..view
+00008050: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00008060: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00008070: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00008080: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00008090: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000080a0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000080b0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000080c0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+000080d0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000080e0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+000080f0: 292d 3237 3c41 5863 6f6d 6d65 6e74 735e  )-27<AXcomments^
+00008100: 6461 7465 4c61 7374 4f70 656e 6564 5c64  dateLastOpened\d
+00008110: 6174 654d 6f64 6966 6965 645b 6461 7465  ateModified[date
+00008120: 4372 6561 7465 6454 7369 7a65 556c 6162  CreatedTsizeUlab
+00008130: 656c 546b 696e 6457 7665 7273 696f 6e54  elTkindWversionT
+00008140: 6e61 6d65 d418 191a 1b1c 1d0c 1f55 696e  name.........Uin
+00008150: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
+00008160: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
+00008170: 0908 d418 191a 1b21 221f 1f10 0810 c808  .......!".......
+00008180: 08d4 1819 1a1b 0b26 1f0c 10b5 0809 d418  .......&........
+00008190: 191a 1b2a 261f 1f10 0208 08d4 1819 1a1b  ...*&...........
+000081a0: 2e2f 1f0c 1003 1061 0809 d418 191a 1b33  ./.....a.......3
+000081b0: 340c 1f10 0510 6409 08d4 1819 1a1b 3839  4.....d.......89
+000081c0: 0c0c 1004 1073 0909 d418 191a 1b3d 3e0c  .....s.......=>.
+000081d0: 1f10 0610 4b09 08d4 1819 1a1b 4243 0c0c  ....K.......BC..
+000081e0: 1000 1101 c709 0908 2300 0000 0000 0000  ........#.......
+000081f0: 0023 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+00008200: 6f64 6966 6965 6423 4030 0000 0000 0000  odified#@0......
+00008210: 0900 0800 1d00 3200 4400 4c00 6000 7200  ......2.D.L.`.r.
+00008220: 7b00 8d00 9800 a100 b400 b600 b700 ca00  {...............
+00008230: d300 e200 ef00 fb01 0001 0601 0b01 1301  ................
+00008240: 1801 2101 2701 2d01 3701 3f01 4101 4401  ..!.'.-.7.?.A.D.
+00008250: 4501 4601 4f01 5101 5301 5401 5501 5e01  E.F.O.Q.S.T.U.^.
+00008260: 6001 6101 6201 6b01 6d01 6e01 6f01 7801  `.a.b.k.m.n.o.x.
+00008270: 7a01 7c01 7d01 7e01 8701 8901 8b01 8c01  z.|.}.~.........
+00008280: 8d01 9601 9801 9a01 9b01 9c01 a501 a701  ................
+00008290: a901 aa01 ab01 b401 b601 b901 ba01 bb01  ................
+000082a0: bc01 c501 ce01 db01 e400 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 0858 a85b 5485 0ec5  Dblob....X.[T...
+000082e0: 4462 6c6f 6200 0000 08e6 e1c8 639f 12c5  Dblob.......c...
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 08dc f782 48cc 0cc5 4100 0000 0800 7000  ....H...A.....p.
+00008310: 08e6 e1c8 639f 12c5 4100 0000 0800 7000  ....c...A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
 00008330: 5363 6f6d 7000 0000 0000 0ae0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
@@ -2264,42 +2264,42 @@
 00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
 00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 020c 7a5f 0074 006f 006f 006c 0073  ....z_.t.o.o.l.s
-00008df0: 6d6f 4444 626c 6f62 0000 0008 cf5e 2d04  moDDblob.....^-.
-00008e00: 750e c541 0000 000d 006f 0075 0074 006c  u..A.....o.u.t.l
-00008e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00008e20: 0073 6d6f 6444 626c 6f62 0000 0008 bea6  .smodDblob......
-00008e30: cfed cc0c c541 0000 000d 006f 0075 0074  .....A.....o.u.t
-00008e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00008e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
-00008e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
-00008e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00008e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
-00008e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
-00008ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00008eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00008ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00008ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00008ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00008ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00008f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00008f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00008f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00008f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
-00008f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
-00008f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00008f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00008f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
-00008f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00008f90: 6f6d 7000 0000 0000 08bf a300 0000 0000  omp.............
+00008de0: 0000 020c 7a00 5f00 7400 6f00 6f00 6c00  ....z._.t.o.o.l.
+00008df0: 736d 6f44 4462 6c6f 6200 0000 0845 bf9c  smoDDblob....E..
+00008e00: d4d3 0fc5 4100 0000 0d00 6f00 7500 7400  ....A.....o.u.t.
+00008e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08be  l.smodDblob.....
+00008e30: a6cf edcc 0cc5 4100 0000 0d00 6f00 7500  ......A.....o.u.
+00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
+00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
+00008e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00008e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00008e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
+00008e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
+00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
+00008eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00008ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00008ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00008ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00008ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00008f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00008f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00008f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00008f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00008f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+00008f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00008f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+00008f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
+00008f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
+00008f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2370,15 +2370,15 @@
 00009410: 197b 7b32 3332 2c20 3139 317d 2c20 7b31  .{{232, 191}, {1
 00009420: 3330 322c 2037 3134 7d7d 0908 1725 313d  302, 714}}...%1=
 00009430: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009440: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009450: 0000 0000 0000 0000 009b 0000 000f 0070  ...............p
 00009460: 006f 0073 0065 005f 0070 0072 006f 0063  .o.s.e._.p.r.o.c
 00009470: 0065 0073 0073 006f 0072 0073 6c67 3153  .e.s.s.o.r.slg1S
-00009480: 636f 6d70 0000 0000 0000 84af 0000 000f  comp............
+00009480: 636f 6d70 0000 0000 0000 9702 0000 000f  comp............
 00009490: 0070 006f 0073 0065 005f 0070 0072 006f  .p.o.s.e._.p.r.o
 000094a0: 0063 0065 0073 0073 006f 0072 0073 6c73  .c.e.s.s.o.r.sls
 000094b0: 7643 626c 6f62 0000 0297 6270 6c69 7374  vCblob....bplist
 000094c0: 3030 d801 0203 0405 0607 0809 0a0b 1949  00.............I
 000094d0: 4a0a 4c58 6963 6f6e 5369 7a65 5f10 0f73  J.LXiconSize_..s
 000094e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
 000094f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
@@ -2465,15 +2465,15 @@
 00009a00: 6f44 4462 6c6f 6200 0000 08e3 bf98 f1cc  oDDblob.........
 00009a10: 0cc5 4100 0000 0f00 7000 6f00 7300 6500  ..A.....p.o.s.e.
 00009a20: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 00009a30: 6f00 7200 736d 6f64 4462 6c6f 6200 0000  o.r.smodDblob...
 00009a40: 08e3 bf98 f1cc 0cc5 4100 0000 0f00 7000  ........A.....p.
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
-00009a70: 6f6d 7000 0000 0000 00e0 0000 0000 0f00  omp.............
+00009a70: 6f6d 7000 0000 0000 0100 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
 00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
 00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
 00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 042b 2400 0000 0900  omp......+$.....
+00009bb0: 6f6d 7000 0000 0000 0432 8900 0000 0900  omp......2......
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2527,50 +2527,50 @@
 00009de0: 0101 010a 010b 010c 0118 0121 0122 0124  ...........!.".$
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-00009e50: 0000 0000 01c5 3153 636f 6d70 0000 0000  ......1Scomp....
-00009e60: 0001 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
-00009e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00009e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
-00009e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
-00009ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
-00009eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
-00009ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00009ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
-00009ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00009ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00009f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00009f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00009f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-00009f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
-00009f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
-00009f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-00009f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-00009f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
-00009f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00009f90: 6f6d 7000 0000 0000 08bf a300 0000 0000  omp.............
+00009e50: 0000 0000 01c5 6831 5363 6f6d 7000 0000  ......h1Scomp...
+00009e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
+00009e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
+00009e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
+00009e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
+00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
+00009eb0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
+00009ec0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
+00009ed0: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
+00009ee0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00009ef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00009f00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00009f10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00009f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+00009f30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+00009f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+00009f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+00009f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+00009f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
+00009f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
+00009f90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
 0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 d6ea  .smoDDblob......
 0000a030: 0380 cc0c c541 0000 0009 0072 006f 0069  .....A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 0000a050: 626c 6f62 0000 0008 d6ea 0380 cc0c c541  blob...........A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-0000a080: 0000 0005 1000 0000 0009 0072 006f 0069  ...........r.o.i
+0000a080: 0000 0005 2000 0000 0009 0072 006f 0069  .... ......r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 001b 0074 0068  long.........t.h
 0000a0b0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
 0000a0c0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
 0000a0d0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
 0000a0e0: 0073 6277 7370 626c 6f62 0000 00ca 6270  .sbwspblob....bp
 0000a0f0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
@@ -2586,15 +2586,15 @@
 0000a190: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
 0000a1a0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 0000a1b0: 0000 0000 0000 009b 0000 001b 0074 0068  .............t.h
 0000a1c0: 0069 0072 0064 005f 0070 0061 0072 0074  .i.r.d._.p.a.r.t
 0000a1d0: 0079 005f 006c 0061 0062 0065 006c 005f  .y._.l.a.b.e.l._
 0000a1e0: 0061 0070 0070 0065 006e 0064 0065 0072  .a.p.p.e.n.d.e.r
 0000a1f0: 0073 6c67 3153 636f 6d70 0000 0000 0002  .slg1Scomp......
-0000a200: 24e1 0000 001b 0074 0068 0069 0072 0064  $......t.h.i.r.d
+0000a200: 2603 0000 001b 0074 0068 0069 0072 0064  &......t.h.i.r.d
 0000a210: 005f 0070 0061 0072 0074 0079 005f 006c  ._.p.a.r.t.y._.l
 0000a220: 0061 0062 0065 006c 005f 0061 0070 0070  .a.b.e.l._.a.p.p
 0000a230: 0065 006e 0064 0065 0072 0073 6c73 7643  .e.n.d.e.r.slsvC
 0000a240: 626c 6f62 0000 0279 6270 6c69 7374 3030  blob...ybplist00
 0000a250: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
 0000a260: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
 0000a270: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
@@ -2676,16 +2676,16 @@
 0000a730: 8201 8301 8c01 8e01 9101 9201 9301 9401  ................
 0000a740: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
 0000a750: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
 0000a760: 0000 0001 ac00 0000 1b00 7400 6800 6900  ..........t.h.i.
 0000a770: 7200 6400 5f00 7000 6100 7200 7400 7900  r.d._.p.a.r.t.y.
 0000a780: 5f00 6c00 6100 6200 6500 6c00 5f00 6100  _.l.a.b.e.l._.a.
 0000a790: 7000 7000 6500 6e00 6400 6500 7200 736d  p.p.e.n.d.e.r.sm
-0000a7a0: 6f44 4462 6c6f 6200 0000 0899 d8b8 be4e  oDDblob........N
-0000a7b0: 0dc5 4100 0000 1b00 7400 6800 6900 7200  ..A.....t.h.i.r.
+0000a7a0: 6f44 4462 6c6f 6200 0000 083f 8021 40a0  oDDblob....?.!@.
+0000a7b0: 12c5 4100 0000 1b00 7400 6800 6900 7200  ..A.....t.h.i.r.
 0000a7c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a7d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a7e0: 7000 6500 6e00 6400 6500 7200 736d 6f64  p.e.n.d.e.r.smod
 0000a7f0: 4462 6c6f 6200 0000 08cb c8d0 edcc 0cc5  Dblob...........
 0000a800: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
 0000a810: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
 0000a820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
@@ -2700,22 +2700,22 @@
 0000a8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 0000a8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 0000a8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
 0000a8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
 0000a8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
 0000a900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
 0000a910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000a920: 0908 095f 1019 7b7b 3333 332c 2031 3238  ..._..{{333, 128
+0000a920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000a930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000a940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000a950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000a960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000a970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000a980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000a990: 0000 0000 0009 65ba 0000 0002 0075 0069  ......e......u.i
+0000a990: 0000 0000 0009 72ef 0000 0002 0075 0069  ......r......u.i
 0000a9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000a9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000a9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000a9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000a9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000a9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000aa00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -2792,162 +2792,162 @@
 0000ae70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000ae80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000ae90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
 0000aea0: 6f44 4462 6c6f 6200 0000 0841 e3d5 bf76  oDDblob....A...v
 0000aeb0: 0ec5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
 0000aec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000aed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
-0000aee0: 0000 0000 0c70 006c 6261 725b 5368 6f77  .....p.lbar[Show
-0000aef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-0000af00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-0000af10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-0000af20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-0000af30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
-0000af40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
-0000af50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-0000af60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-0000af70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
-0000af80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000af90: 6f6d 7000 0000 0000 08bf a300 0000 0000  omp.............
+0000aee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
+0000aef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+0000af00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+0000af10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+0000af20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+0000af30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+0000af40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+0000af50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+0000af60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+0000af70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
+0000af80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
+0000af90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
 0000b010: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
 0000b020: 0069 0073 0065 0064 6277 7370 626c 6f62  .i.s.e.dbwspblob
-0000b030: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b030: 0000 00ca 6270 6c69 7374 3030 d701 0203  ....bplist00....
 0000b040: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 0000b050: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 0000b060: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 0000b070: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 0000b080: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 0000b090: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 0000b0a0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b0b0: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
-0000b0c0: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
-0000b0d0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-0000b0e0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-0000b0f0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-0000b100: 0c00 7500 6e00 7300 7500 7000 6500 7200  ..u.n.s.u.p.e.r.
-0000b110: 7600 6900 7300 6500 6464 7363 6c62 6f6f  v.i.s.e.ddsclboo
-0000b120: 6c00 0000 000c 0075 006e 0073 0075 0070  l......u.n.s.u.p
-0000b130: 0065 0072 0076 0069 0073 0065 0064 6c67  .e.r.v.i.s.e.dlg
-0000b140: 3153 636f 6d70 0000 0000 0002 4b53 0000  1Scomp......KS..
-0000b150: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-0000b160: 0076 0069 0073 0065 0064 6c73 7643 626c  .v.i.s.e.dlsvCbl
-0000b170: 6f62 0000 0281 6270 6c69 7374 3030 d801  ob....bplist00..
-0000b180: 0203 0405 0607 0809 0a0b 1846 4748 0a5f  ...........FGH._
-0000b190: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-0000b1a0: 7369 6f6e 5f10 0f73 686f 7749 636f 6e50  sion_..showIconP
-0000b1b0: 7265 7669 6577 5763 6f6c 756d 6e73 5f10  reviewWcolumns_.
-0000b1c0: 1163 616c 6375 6c61 7465 416c 6c53 697a  .calculateAllSiz
-0000b1d0: 6573 5874 6578 7453 697a 655a 736f 7274  esXtextSizeZsort
-0000b1e0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-0000b1f0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-0000b200: 6573 1001 09ab 0c15 1a1f 2328 2d32 373c  es........#(-27<
-0000b210: 41d4 0d0e 0f10 1112 0a0a 5a69 6465 6e74  A.........Zident
-0000b220: 6966 6965 7255 7769 6474 6859 6173 6365  ifierUwidthYasce
-0000b230: 6e64 696e 6757 7669 7369 626c 6554 6e61  ndingWvisibleTna
-0000b240: 6d65 1101 c709 09d4 0d0e 0f10 1617 1818  me..............
-0000b250: 5875 6269 7175 6974 7910 2308 08d4 0d0e  Xubiquity.#.....
-0000b260: 0f10 1b1c 180a 5c64 6174 654d 6f64 6966  ......\dateModif
-0000b270: 6965 6410 b508 09d4 0d0e 0f10 201c 1818  ied......... ...
-0000b280: 5b64 6174 6543 7265 6174 6564 0808 d40d  [dateCreated....
-0000b290: 0e0f 1024 2518 0a54 7369 7a65 1061 0809  ...$%..Tsize.a..
-0000b2a0: d40d 0e0f 1029 2a0a 0a54 6b69 6e64 1073  .....)*..Tkind.s
-0000b2b0: 0909 d40d 0e0f 102e 2f0a 1855 6c61 6265  ......../..Ulabe
-0000b2c0: 6c10 6409 08d4 0d0e 0f10 3334 0a18 5776  l.d.......34..Wv
-0000b2d0: 6572 7369 6f6e 104b 0908 d40d 0e0f 1038  ersion.K.......8
-0000b2e0: 390a 1858 636f 6d6d 656e 7473 1101 2c09  9..Xcomments..,.
-0000b2f0: 08d4 0d0e 0f10 3d3e 1818 5e64 6174 654c  ......=>..^dateL
-0000b300: 6173 744f 7065 6e65 6410 c808 08d4 0d0e  astOpened.......
-0000b310: 0f10 421c 1818 5964 6174 6541 6464 6564  ..B...YdateAdded
-0000b320: 0808 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
-0000b330: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
-0000b340: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-0000b350: 6500 7000 7900 8c00 8e00 8f00 9b00 a400  e.p.y...........
-0000b360: af00 b500 bf00 c700 cc00 cf00 d000 d100  ................
-0000b370: da00 e300 e500 e600 e700 f000 fd00 ff01  ................
-0000b380: 0001 0101 0a01 1601 1701 1801 2101 2601  ............!.&.
-0000b390: 2801 2901 2a01 3301 3801 3a01 3b01 3c01  (.).*.3.8.:.;.<.
-0000b3a0: 4501 4b01 4d01 4e01 4f01 5801 6001 6201  E.K.M.N.O.X.`.b.
-0000b3b0: 6301 6401 6d01 7601 7901 7a01 7b01 8401  c.d.m.v.y.z.{...
-0000b3c0: 9301 9501 9601 9701 a001 aa01 ab01 ac01  ................
-0000b3d0: ad01 b601 c301 cc00 0000 0000 0002 0100  ................
-0000b3e0: 0000 0000 0000 4a00 0000 0000 0000 0000  ......J.........
-0000b3f0: 0000 0000 0001 cd00 0000 0c00 7500 6e00  ............u.n.
-0000b400: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
-0000b410: 6500 646c 7376 7062 6c6f 6200 0002 6662  e.dlsvpblob...fb
-0000b420: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-0000b430: 090a 0b1a 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
-0000b440: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
-0000b450: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
-0000b460: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
-0000b470: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
-0000b480: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
-0000b490: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
-0000b4a0: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
-0000b4b0: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
-0000b4c0: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
-0000b4d0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-0000b4e0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-0000b4f0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-0000b500: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-0000b510: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
-0000b520: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-0000b530: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
-0000b540: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
-0000b550: 190a 251a 0909 10b5 08d4 1617 1819 1a25  ..%............%
-0000b560: 1a2a 0808 1002 d416 1718 190a 2d1a 2f09  .*..........-./.
-0000b570: 1061 0810 03d4 1617 1819 1a32 0a34 0810  .a.........2.4..
-0000b580: 6409 1005 d416 1718 190a 370a 3909 1073  d.........7.9..s
-0000b590: 0910 04d4 1617 1819 1a3c 0a3e 0810 4b09  .........<.>..K.
-0000b5a0: 1006 d416 1718 190a 410a 4309 1101 c709  ........A.C.....
-0000b5b0: 1000 0823 4028 0000 0000 0000 5c64 6174  ...#@(......\dat
-0000b5c0: 654d 6f64 6966 6965 6423 4030 0000 0000  eModified#@0....
-0000b5d0: 0000 0900 0800 1900 2e00 4000 4800 5c00  ..........@.H.\.
-0000b5e0: 6500 7000 7900 8c00 8e00 8f00 a200 ab00  e.p.y...........
-0000b5f0: ba00 c700 d300 d800 de00 e300 eb00 f000  ................
-0000b600: f901 0101 0701 1101 1701 1801 1b01 1c01  ................
-0000b610: 1e01 2701 2801 2a01 2b01 2d01 3601 3701  ..'.(.*.+.-.6.7.
-0000b620: 3901 3a01 4301 4401 4501 4701 5001 5101  9.:.C.D.E.G.P.Q.
-0000b630: 5301 5401 5601 5f01 6001 6201 6301 6501  S.T.V._.`.b.c.e.
-0000b640: 6e01 6f01 7101 7201 7401 7d01 7e01 8001  n.o.q.r.t.}.~...
-0000b650: 8101 8301 8c01 8d01 9001 9101 9301 9401  ................
-0000b660: 9d01 aa01 b300 0000 0000 0002 0100 0000  ................
-0000b670: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
-0000b680: 0000 0001 b400 0000 0c00 7500 6e00 7300  ..........u.n.s.
-0000b690: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-0000b6a0: 646d 6f44 4462 6c6f 6200 0000 08e7 da8e  dmoDDblob.......
-0000b6b0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
-0000b6c0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-0000b6d0: 646d 6f64 4462 6c6f 6200 0000 08e7 da8e  dmodDblob.......
-0000b6e0: f9a1 0cc5 4100 0000 0c00 7500 6e00 7300  ....A.....u.n.s.
-0000b6f0: 7500 7000 6500 7200 7600 6900 7300 6500  u.p.e.r.v.i.s.e.
-0000b700: 6470 6831 5363 6f6d 7000 0000 0000 02b0  dph1Scomp.......
-0000b710: 0000 0000 0c00 7500 6e00 7300 7500 7000  ......u.n.s.u.p.
-0000b720: 6500 7200 7600 6900 7300 6500 6476 5372  e.r.v.i.s.e.dvSr
-0000b730: 6e6c 6f6e 6700 0000 0100 0000 0500 7500  nlong.........u.
-0000b740: 7400 6900 6c00 7362 7773 7062 6c6f 6200  t.i.l.sbwspblob.
-0000b750: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-0000b760: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-0000b770: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-0000b780: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-0000b790: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-0000b7a0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-0000b7b0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-0000b7c0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-0000b7d0: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
-0000b7e0: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
-0000b7f0: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
-0000b800: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-0000b810: 0000 0000 0000 0000 0000 009a 5f00 6c00  ............_.l.
+0000b0b0: 0809 5f10 197b 7b33 3534 2c20 3132 347d  .._..{{354, 124}
+0000b0c0: 2c20 7b31 3037 362c 2036 3231 7d7d 0908  , {1076, 621}}..
+0000b0d0: 1725 313d 4960 6d79 7a7b 7c7d 7e9a 0000  .%1=I`myz{|}~...
+0000b0e0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+0000b0f0: 0000 0000 0000 0000 0000 0000 009b 0000  ................
+0000b100: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
+0000b110: 0076 0069 0073 0065 0064 6473 636c 626f  .v.i.s.e.ddsclbo
+0000b120: 6f6c 0000 0000 0c00 7500 6e00 7300 7500  ol......u.n.s.u.
+0000b130: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
+0000b140: 6731 5363 6f6d 7000 0000 0000 03e8 6c00  g1Scomp.......l.
+0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
+0000b160: 7200 7600 6900 7300 6500 646c 7376 4362  r.v.i.s.e.dlsvCb
+0000b170: 6c6f 6200 0002 8162 706c 6973 7430 30d8  lob....bplist00.
+0000b180: 0102 0304 0506 0708 090a 0b18 4647 0a49  ............FG.I
+0000b190: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+0000b1a0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+0000b1b0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+0000b1c0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+0000b1d0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+0000b1e0: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+0000b1f0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+0000b200: 696f 6e23 4030 0000 0000 0000 09ab 0c15  ion#@0..........
+0000b210: 1a1f 2328 2d32 373c 41d4 0d0e 0f10 1112  ..#(-27<A.......
+0000b220: 0a0a 5a69 6465 6e74 6966 6965 7255 7769  ..ZidentifierUwi
+0000b230: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
+0000b240: 7369 626c 6554 6e61 6d65 1101 c709 09d4  sibleTname......
+0000b250: 0d0e 0f10 1617 1818 5875 6269 7175 6974  ........Xubiquit
+0000b260: 7910 2308 08d4 100e 0f0d 0a1c 0a1e 0910  y.#.............
+0000b270: b509 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
+0000b280: 0d0e 0f10 201c 1818 5b64 6174 6543 7265  .... ...[dateCre
+0000b290: 6174 6564 0808 d40d 0e0f 1024 2518 0a54  ated.......$%..T
+0000b2a0: 7369 7a65 1061 0809 d40d 0e0f 1029 2a0a  size.a.......)*.
+0000b2b0: 0a54 6b69 6e64 1073 0909 d40d 0e0f 102e  .Tkind.s........
+0000b2c0: 2f0a 1855 6c61 6265 6c10 6409 08d4 0d0e  /..Ulabel.d.....
+0000b2d0: 0f10 3334 0a18 5776 6572 7369 6f6e 104b  ..34..Wversion.K
+0000b2e0: 0908 d40d 0e0f 1038 390a 1858 636f 6d6d  .......89..Xcomm
+0000b2f0: 656e 7473 1101 2c09 08d4 0d0e 0f10 3d3e  ents..,.......=>
+0000b300: 1818 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+0000b310: 6410 c808 08d4 0d0e 0f10 421c 1818 5964  d.........B...Yd
+0000b320: 6174 6541 6464 6564 0808 0823 4028 0000  ateAdded...#@(..
+0000b330: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+0000b340: 6409 1001 0008 0019 0022 0034 003c 0050  d........".4.<.P
+0000b350: 0059 0064 0077 008c 0095 0096 00a2 00ab  .Y.d.w..........
+0000b360: 00b6 00bc 00c6 00ce 00d3 00d6 00d7 00d8  ................
+0000b370: 00e1 00ea 00ec 00ed 00ee 00f7 00f8 00fa  ................
+0000b380: 00fb 0108 0111 011d 011e 011f 0128 012d  .............(.-
+0000b390: 012f 0130 0131 013a 013f 0141 0142 0143  ./.0.1.:.?.A.B.C
+0000b3a0: 014c 0152 0154 0155 0156 015f 0167 0169  .L.R.T.U.V._.g.i
+0000b3b0: 016a 016b 0174 017d 0180 0181 0182 018b  .j.k.t.}........
+0000b3c0: 019a 019c 019d 019e 01a7 01b1 01b2 01b3  ................
+0000b3d0: 01b4 01bd 01ca 01cb 0000 0000 0000 0201  ................
+0000b3e0: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+0000b3f0: 0000 0000 0000 01cd 0000 000c 0075 006e  .............u.n
+0000b400: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
+0000b410: 0065 0064 6c73 7670 626c 6f62 0000 0266  .e.dlsvpblob...f
+0000b420: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+0000b430: 0809 0a0b 1a46 470a 2458 6963 6f6e 5369  .....FG.$XiconSi
+0000b440: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+0000b450: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+0000b460: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+0000b470: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+0000b480: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+0000b490: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+0000b4a0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+0000b4b0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
+0000b4c0: 151e 2328 2c31 363b 4058 636f 6d6d 656e  ..#(,16;@Xcommen
+0000b4d0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+0000b4e0: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
+0000b4f0: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
+0000b500: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
+0000b510: 6f6e 546e 616d 65d4 1617 1819 1a1b 0a1d  onTname.........
+0000b520: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+0000b530: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+0000b540: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
+0000b550: c808 1008 d419 1718 1624 250a 0a10 0110  .........$%.....
+0000b560: b509 09d4 1617 1819 1a25 1a2b 0808 1002  .........%.+....
+0000b570: d416 1718 190a 2e1a 3009 1061 0810 03d4  ........0..a....
+0000b580: 1617 1819 1a33 0a35 0810 6409 1005 d416  .....3.5..d.....
+0000b590: 1718 190a 380a 3a09 1073 0910 04d4 1617  ....8.:..s......
+0000b5a0: 1819 1a3d 0a3f 0810 4b09 1006 d416 1718  ...=.?..K.......
+0000b5b0: 190a 420a 4409 1101 c709 1000 0823 4028  ..B.D........#@(
+0000b5c0: 0000 0000 0000 5c64 6174 654d 6f64 6966  ......\dateModif
+0000b5d0: 6965 6409 0008 0019 0022 0034 003c 0050  ied......".4.<.P
+0000b5e0: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+0000b5f0: 00c1 00ce 00da 00df 00e5 00ea 00f2 00f7  ................
+0000b600: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+0000b610: 0125 012e 012f 0131 0132 0134 013d 013f  .%.../.1.2.4.=.?
+0000b620: 0141 0142 0143 014c 014d 014e 0150 0159  .A.B.C.L.M.N.P.Y
+0000b630: 015a 015c 015d 015f 0168 0169 016b 016c  .Z.\.]._.h.i.k.l
+0000b640: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
+0000b650: 0189 018a 018c 0195 0196 0199 019a 019c  ................
+0000b660: 019d 01a6 01b3 0000 0000 0000 0201 0000  ................
+0000b670: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+0000b680: 0000 0000 01b4 0000 000c 0075 006e 0073  ...........u.n.s
+0000b690: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b6a0: 0064 6d6f 4444 626c 6f62 0000 0008 fdf7  .dmoDDblob......
+0000b6b0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+0000b6c0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b6d0: 0064 6d6f 6444 626c 6f62 0000 0008 fdf7  .dmodDblob......
+0000b6e0: dec3 530f c541 0000 000c 0075 006e 0073  ..S..A.....u.n.s
+0000b6f0: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b700: 0064 7068 3153 636f 6d70 0000 0000 0004  .dph1Scomp......
+0000b710: d000 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+0000b720: 0065 0072 0076 0069 0073 0065 0064 7653  .e.r.v.i.s.e.dvS
+0000b730: 726e 6c6f 6e67 0000 0001 0000 0005 0075  rnlong.........u
+0000b740: 0074 0069 006c 0073 6277 7370 626c 6f62  .t.i.l.sbwspblob
+0000b750: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+0000b760: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
+0000b770: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
+0000b780: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
+0000b790: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+0000b7a0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+0000b7b0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+0000b7c0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
+0000b7d0: 0809 5f10 187b 7b33 3335 2c20 3139 387d  .._..{{335, 198}
+0000b7e0: 2c20 7b39 3237 2c20 3536 387d 7d09 0817  , {927, 568}}...
+0000b7f0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
+0000b800: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
+0000b810: 0000 0000 0000 0000 0000 0000 9a00 6c00  ..............l.
 0000b820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 0000b830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
 0000b840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
 0000b850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
 0000b860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
 0000b870: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
 0000b880: 6500 7200 7376 5372 6e6c 6f6e 6700 0000  e.r.svSrnlong...
@@ -2956,22 +2956,22 @@
 0000b8b0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 0000b8c0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 0000b8d0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
 0000b8e0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
 0000b8f0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
 0000b900: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
 0000b910: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000b920: 0908 095f 1019 7b7b 3333 332c 2031 3238  ..._..{{333, 128
+0000b920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000b930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000b940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000b950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000b960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000b970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000b980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000b990: 0000 0000 0009 65ba 0000 0002 0075 0069  ......e......u.i
+0000b990: 0000 0000 0009 72ef 0000 0002 0075 0069  ......r......u.i
 0000b9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000b9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000b9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000b9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000b9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000b9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000ba00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -3048,26 +3048,26 @@
 0000be70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000be80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000be90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
 0000bea0: 6f44 4462 6c6f 6200 0000 0841 e3d5 bf76  oDDblob....A...v
 0000beb0: 0ec5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
 0000bec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000bed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
-0000bee0: 0000 0000 0c70 006c 6261 725b 5368 6f77  .....p.lbar[Show
-0000bef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-0000bf00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-0000bf10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-0000bf20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
-0000bf30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
-0000bf40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
-0000bf50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
-0000bf60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
-0000bf70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
-0000bf80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-0000bf90: 6f6d 7000 0000 0000 08bf a300 0000 0000  omp.............
+0000bee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
+0000bef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+0000bf00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+0000bf10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+0000bf20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
+0000bf30: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
+0000bf40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
+0000bf50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
+0000bf60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+0000bf70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
+0000bf80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
+0000bf90: 5363 6f6d 7000 0000 0000 08bf 7d00 0000  Scomp.......}...
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
                 self.scaled_df[c[0]] = self.scaled_df[c[0]] - df['correction_x']
                 self.scaled_df[c[1]] = self.scaled_df[c[1]] - df['correction_y']
             self.scaled_df = self.scaled_df.fillna((self.img_size[0]/2))
             if self.visualize:
                 self.visualize()
             self.featurize()
 
-
     def visualize(self):
         max_x, max_y = np.nanmax(self.scaled_df[self.bp_headers['x']].values), np.nanmax(self.scaled_df[self.bp_headers['y']].values)
         img = np.zeros(shape=[int(max_x), int(max_y), 3], dtype=np.uint8)
         for frm in range(len(self.scaled_df)):
             frm_data = self.scaled_df.iloc[frm].astype(int)
             frm_img = deepcopy(img)
             for bp_name, bp in self.bp_dict.items():
@@ -128,8 +127,8 @@
                                                                          self.scaled_df[col_names[3]].values)
 
         for c, t in (list(itertools.product(results.columns, self.rolling_window_sizes.keys()))):
             results[f'{c}_rolling_{t}_window_mean'] = results[c].rolling(int(self.rolling_window_sizes[t]), min_periods=1).mean()
             results[f'{c}_rolling_{t}_window_stdev'] = results[c].rolling(int(self.rolling_window_sizes[t]), min_periods=1).std()
         self.results = results.fillna(-1)
 
-aligner = EgocentricalAlignmentFeaturizer(data_path= '/Users/simon/Desktop/envs/simba_dev/simba/features_scripts/misc/test_data_mouse_OF', visualize=False)
+#aligner = EgocentricalAlignmentFeaturizer(data_path= '/Users/simon/Desktop/envs/simba_dev/simba/features_scripts/misc/test_data_mouse_OF', visualize=False)
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.61.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.61.4/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,15 +188,14 @@
             elif additional_clfs and self.err_settings[Methods.ADDITIONAL_THIRD_PARTY_CLFS.value] == Methods.ERROR.value:
                 raise ThirdPartyAnnotationsAdditionalClfError(video_name=self.video_name, clf_names=additional_clfs)
 
             features_df = read_df(file_path=file_path, file_type=self.file_type)
             out_df = deepcopy(features_df)
             for clf in self.clf_names:
                 clf_annot = annot_df[(annot_df[BEHAVIOR] == clf)].reset_index(drop=True)
-
                 if len(clf_annot) == 0:
                     if self.err_settings[Methods.ZERO_THIRD_PARTY_VIDEO_BEHAVIOR_ANNOTATIONS.value] == Methods.WARNING.value:
                         ThirdPartyAnnotationsMissingAnnotationsWarning(video_name=self.video_name, clf_names=self.clf_names, log_status=self.settings['log'])
                         out_df[clf] = 0
                         continue
                     elif self.err_settings[Methods.ZERO_THIRD_PARTY_VIDEO_BEHAVIOR_ANNOTATIONS.value] == Methods.ERROR.value:
                         raise ThirdPartyAnnotationsMissingAnnotationsError(video_name=self.video_name, clf_names=self.clf_names)
@@ -214,43 +213,48 @@
                                                                               log_status=self.settings['log'])
                     elif self.err_settings[Methods.THIRD_PARTY_FRAME_COUNT_CONFLICT.value] == Methods.ERROR.value:
                         raise ThirdPartyAnnotationsOutsidePoseEstimationDataError(video_name=self.video_name,
                                                                                   clf_name=clf,
                                                                                   frm_cnt=out_df.index[-1],
                                                                                   first_error_frm=idx_diff[0],
                                                                                   ambiguous_cnt=len(idx_diff))
-
                 annot_idx = [x for x in annot_idx if x not in idx_diff]
                 out_df[clf] = 0
                 out_df.loc[annot_idx, clf] = 1
             save_path = os.path.join(self.targets_folder, self.video_name + '.' + self.file_type)
             write_df(out_df, self.file_type, save_path)
             print(f'Saved {self.app} annotations for video {self.video_name}...')
         self.timer.stop_timer()
         stdout_success(msg=f'{self.app} annotations appended to dataset and saved in project_folder/csv/targets_inserted directory', elapsed_time=self.timer.elapsed_time_str)
 
-settings = {'log': True,  'file_format': 'csv', 'errors': {'INVALID annotations file data format': 'WARNING',
-                                                           'ADDITIONAL third-party behavior detected': 'NONE',
-                                                           'Annotations EVENT COUNT conflict': 'WARNING',
-                                                           'Annotations OVERLAP inaccuracy': 'WARNING',
-                                                           'ZERO third-party video behavior annotations found': 'WARNING',
-                                                           'Annotations and pose FRAME COUNT conflict': 'WARNING',
-                                                           'Annotations data file NOT FOUND': 'WARNING'}}
-
-
+# settings = {'log': True,  'file_format': 'csv', 'errors': {'INVALID annotations file data format': 'WARNING',
+#                        'ADDITIONAL third-party behavior detected': 'WARNING',
+#                        'Annotations EVENT COUNT conflict': 'WARNING',
+#                        'Annotations OVERLAP inaccuracy': 'WARNING',
+#                        'ZERO third-party video behavior annotations found': 'WARNING',
+#                        'Annotations and pose FRAME COUNT conflict': 'WARNING',
+#                        'Annotations data file NOT FOUND': 'WARNING'}}
 #
+# settings['file_format'] = 'csv'
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                data_dir='/Users/simon/Downloads/FIXED',
+#                                data_dir='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/ethovision_annotations',
+#                                settings=settings,
+#                                app='ETHOVISION')
+# test.run()
+
+#
+# test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini',
+#                                data_dir='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/boris_annotations',
 #                                settings=settings,
 #                                app='BORIS')
 # test.run()
 
 
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                data_dir='/Users/simon/Desktop/envs/simba_dev/tests/test_data/deepethogram_example',
+#                                data_dir='/Users/simon/Desktop/envs/simba_dev/old_tests/test_data/deepethogram_example',
 #                                settings=settings,
 #                                app='DEEPETHOGRAM')
 # test.run()
 
 
 # test = ThirdPartyLabelAppender(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                data_dir=r'/Users/simon/Desktop/envs/simba_dev/tests/test_data/import_tests/ethovision_data',
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.61.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.61.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.61.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.61.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.61.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.61.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_bout_based_calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 from datetime import datetime
 from typing import Dict, Union, List
 import cv2
 
 from simba.utils.read_write import get_fn_ext, read_df, get_video_meta_data
 from simba.utils.data import detect_bouts, create_color_palettes, find_bins
-from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.checks import check_if_filepath_list_is_empty, check_that_column_exist
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.errors import InvalidVideoFileError
 
 class SeverityBoutCalculator(ConfigReader, FeatureExtractionMixin):
@@ -74,31 +74,33 @@
         movements = self.__calculate_movements(data_paths=self.machine_results_paths)
         video_bins_info = find_bins(data=movements, bracket_type=self.settings['bracket_type'], bracket_cnt=self.settings['brackets'], normalization_method=self.settings['normalization'])
         self.results = pd.DataFrame(columns=['VIDEO', 'EVENT', 'START TIME', 'END TIME', 'START FRAME', 'END FRAME', 'BOUT TIME', 'MOVEMENT', 'SEVERITY'])
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
             df = read_df(file_path=file_path, file_type=self.file_type)
+            check_that_column_exist(df=df, column_name=self.settings['clf'], file_name=file_path)
             bout_df = detect_bouts(data_df=df, target_lst=[self.settings['clf']], fps=fps)
             bout_df.columns = ['EVENT', 'START TIME', 'END TIME', 'START FRAME', 'END FRAME', 'BOUT TIME']
             severity_lst, movement_lst = [], []
-            for i in bout_df[['START FRAME', 'END FRAME']].values:
-                bout_move_val = np.mean(movements[video_name][i[0]:i[1]])
-                if bout_move_val >= video_bins_info[video_name][-1][1]:
-                    severity_lst.append(self.settings['brackets'])
-                    movement_lst.append(bout_move_val)
-                else:
-                    for j_cnt, j in enumerate(video_bins_info[video_name]):
-                        if j[0] <= bout_move_val <= j[1]:
-                            severity_lst.append(j_cnt+1)
-                            movement_lst.append(round(bout_move_val, 4))
-            bout_df['MOVEMENT'] = movement_lst
-            bout_df['SEVERITY'] = severity_lst
-            bout_df.insert(0, 'VIDEO', video_name)
-            self.results = pd.concat([self.results, bout_df], axis=0).reset_index(drop=True)
+            if len(bout_df) > 0:
+                for i in bout_df[['START FRAME', 'END FRAME']].values:
+                    bout_move_val = np.mean(movements[video_name][i[0]:i[1]])
+                    if bout_move_val >= video_bins_info[video_name][-1][1]:
+                        severity_lst.append(self.settings['brackets'])
+                        movement_lst.append(bout_move_val)
+                    else:
+                        for j_cnt, j in enumerate(video_bins_info[video_name]):
+                            if j[0] <= bout_move_val <= j[1]:
+                                severity_lst.append(j_cnt+1)
+                                movement_lst.append(round(bout_move_val, 4))
+                bout_df['MOVEMENT'] = movement_lst
+                bout_df['SEVERITY'] = severity_lst
+                bout_df.insert(0, 'VIDEO', video_name)
+                self.results = pd.concat([self.results, bout_df], axis=0).reset_index(drop=True)
         self.save()
         if self.settings['save_bin_definitions']:
             self.save_bin_definitions(data=video_bins_info)
         if self.settings['visualize']:
             self.visualize()
 
     def save(self):
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/severity_frame_based_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import pandas as pd
 from datetime import datetime
 import cv2
 from typing import Dict, Union
 
 from simba.utils.read_write import get_fn_ext, read_df
-from simba.utils.checks import check_if_filepath_list_is_empty
+from simba.utils.checks import check_if_filepath_list_is_empty, check_that_column_exist
 from simba.utils.data import find_bins, detect_bouts, get_video_meta_data, create_color_palettes
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.errors import NoDataError, InvalidVideoFileError
 
@@ -75,14 +75,15 @@
         self.video_bins_info = find_bins(data=self.movements, bracket_type=self.settings['bracket_type'], bracket_cnt=self.settings['brackets'], normalization_method=self.settings['normalization'])
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
             print(f'Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
             self.results[video_name] = {}
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
             df = read_df(file_path=file_path, file_type=self.file_type).astype(int)
+            check_that_column_exist(df=df, column_name=self.settings['clf'], file_name=file_path)
             move_df = pd.DataFrame(self.movements[video_name], columns=['MOVEMENT'])
             video_bins = np.array((0))
             video_bins = np.hstack((video_bins, self.video_bins_info[video_name][: , -1]))
             hist = np.histogram([self.movements[video_name]], bins=video_bins)
             move_df['BIN'] = np.fmin(np.digitize(self.movements[video_name], hist[1]), self.settings['brackets'])
             df = pd.concat([df, move_df], axis=1)
             if self.settings['visualize']: self.visualization_data[video_name] = df
```

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.61.4/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.61.4/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.61.4/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.61.4/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.61.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.61.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.61.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.61.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.61.4/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.61.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.61.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.61.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.61.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.61.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.61.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.61.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.61.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.61.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.61.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.3
+Version: 1.61.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,16 @@
 simba/plotting/ROI_feature_visualizer.py
 simba/plotting/ROI_feature_visualizer_mp.py
 simba/plotting/ROI_plotter.py
 simba/plotting/ROI_plotter_mp.py
 simba/plotting/__init__.py
 simba/plotting/clf_validator.py
 simba/plotting/data_plotter.py
+simba/plotting/directing_animals_visualizer.py
+simba/plotting/directing_animals_visualizer_mp.py
 simba/plotting/distance_plotter.py
 simba/plotting/distance_plotter_mp.py
 simba/plotting/ez_lineplot.py
 simba/plotting/frame_mergerer_ffmpeg.py
 simba/plotting/gantt_creator.py
 simba/plotting/gantt_creator_mp.py
 simba/plotting/heat_mapper_clf.py
@@ -430,14 +432,15 @@
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
 tests/__init__.py
 tests/test_data_processors.py
 tests/test_featurizers.py
 tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
+tests/test_visualize_directing_animals.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
 tests/data/test_projects/zebrafish/feature_file/__init__.py
 tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
```

### Comparing `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.61.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/LICENSE.md` & `Simba-UW-tf-dev-1.61.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.61.4/tests/test_data_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 from simba.data_processors.agg_clf_calculator import AggregateClfCalculator
 from simba.data_processors.fsttc_calculator import FSTTCCalculator
 from simba.data_processors.kleinberg_calculator import KleinbergCalculator
 from simba.data_processors.movement_calculator import MovementCalculator
 from simba.data_processors.timebins_clf_calculator import TimeBinsClfCalculator
 from simba.data_processors.timebins_movement_calculator import TimeBinsMovementCalculator
 
-
-
-
-@pytest.mark.parametrize("config_path, data_measures, classifiers", [('/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', ['Bout count'], ['Attack']),
-                                                                     ('/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', ['Total event duration (s)'], ['Attack'])])
-def test_create_clf_log_use_case(config_path, data_measures, classifiers):
+@pytest.mark.parametrize("config_path, data_measures, video_meta_data, classifiers", [('/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', ['Bout count'], [], ['Attack']),
+                                                                                      ('/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', ['Total event duration (s)'], [], ['Attack'])])
+def test_create_clf_log_use_case(config_path, data_measures, video_meta_data, classifiers):
 
     clf_log_creator = AggregateClfCalculator(config_path=config_path,
-                                             data_measures=data_measures, classifiers=classifiers)
+                                             data_measures=data_measures,
+                                             video_meta_data=[],
+                                             classifiers=classifiers)
     clf_log_creator.run()
     clf_log_creator.save()
     assert len(clf_log_creator.results_df) == len(data_measures)
     assert os.path.isfile(clf_log_creator.save_path)
     os.remove(clf_log_creator.save_path)
 
 @pytest.mark.parametrize("config_path, time_window, behavior_lst, create_graph", [('/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', 2000, ['Attack', 'Sniffing'], False)])
```

### Comparing `Simba-UW-tf-dev-1.61.3/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.61.4/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.61.4/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.61.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.61.4/tests/test_thirdparty_appenders.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from simba.third_party_label_appenders.BORIS_appender import BorisAppender
 from simba.third_party_label_appenders.solomon_importer import SolomonImporter
 from simba.third_party_label_appenders.ethovision_import import ImportEthovision
 from simba.third_party_label_appenders.observer_importer import NoldusObserverImporter
 from simba.third_party_label_appenders.BENTO_appender import BentoAppender
 from simba.third_party_label_appenders.deepethogram_importer import DeepEthogramImporter
 
-
 @pytest.mark.parametrize("config_path, boris_path", [('/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/project_folder/project_config.ini',
                                                       '/Users/simon/Desktop/envs/simba_dev/test/data/test_projects/two_c57/boris_annotations')])
 def test_boris_import_use_case(config_path, boris_path):
     boris_appender = BorisAppender(config_path=config_path,
                                    data_dir=boris_path)
     boris_appender.create_boris_master_file()
     boris_appender.run()
```

### Comparing `Simba-UW-tf-dev-1.61.3/README.md` & `Simba-UW-tf-dev-1.61.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.3/setup.py` & `Simba-UW-tf-dev-1.61.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.61.3",
+    version="1.61.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```


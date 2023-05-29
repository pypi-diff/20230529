# Comparing `tmp/octavvs-0.1.8.tar.gz` & `tmp/octavvs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/octavvs-0.1.8.tar", last modified: Tue Sep 14 07:31:34 2021, max compression
+gzip compressed data, was "dist/octavvs-0.1.9.tar", last modified: Fri Oct  8 09:53:08 2021, max compression
```

## Comparing `octavvs-0.1.8.tar` & `octavvs-0.1.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.113128 octavvs-0.1.8/
--rw-r--r--   0 carl      (1000) users      (100)     5592 2021-09-14 07:31:34.113128 octavvs-0.1.8/PKG-INFO
--rw-r--r--   0 carl      (1000) users      (100)     4307 2021-09-06 13:18:48.000000 octavvs-0.1.8/README.md
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.097122 octavvs-0.1.8/octavvs/
--rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/__init__.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.101123 octavvs-0.1.8/octavvs/algorithms/
--rw-r--r--   0 carl      (1000) users      (100)        0 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/algorithms/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)     6649 2020-06-03 08:42:35.000000 octavvs-0.1.8/octavvs/algorithms/atm_correction.py
--rw-r--r--   0 carl      (1000) users      (100)     9232 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/algorithms/baseline.py
--rw-r--r--   0 carl      (1000) users      (100)      263 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/algorithms/correction.py
--rwxr-xr-x   0 carl      (1000) users      (100)    12158 2021-09-13 12:12:07.000000 octavvs-0.1.8/octavvs/algorithms/decomposition.py
--rwxr-xr-x   0 carl      (1000) users      (100)     9306 2021-07-14 11:12:19.000000 octavvs-0.1.8/octavvs/algorithms/decomposition_working.py
--rwxr-xr-x   0 carl      (1000) users      (100)    11390 2021-07-24 13:08:37.000000 octavvs-0.1.8/octavvs/algorithms/decomposition_working_2.py
--rw-r--r--   0 carl      (1000) users      (100)    28061 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/algorithms/mie_correction.py
--rw-r--r--   0 carl      (1000) users      (100)     2035 2021-09-06 13:17:48.000000 octavvs-0.1.8/octavvs/algorithms/normalization.py
--rw-r--r--   0 carl      (1000) users      (100)     3809 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/algorithms/ptir.py
--rw-r--r--   0 carl      (1000) users      (100)     4705 2021-09-06 13:17:48.000000 octavvs-0.1.8/octavvs/algorithms/util.py
--rw-r--r--   0 carl      (1000) users      (100)    55653 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/clustering.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.101123 octavvs-0.1.8/octavvs/decomp/
--rw-r--r--   0 carl      (1000) users      (100)        0 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/decomp/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)    43034 2021-09-13 21:14:10.000000 octavvs-0.1.8/octavvs/decomp/decomposition.ui
--rw-r--r--   0 carl      (1000) users      (100)     7024 2021-09-13 12:12:07.000000 octavvs-0.1.8/octavvs/decomp/decompworker.py
--rwxr-xr-x   0 carl      (1000) users      (100)    26011 2021-09-13 12:12:07.000000 octavvs-0.1.8/octavvs/decomp/plotwidget.py
--rw-r--r--   0 carl      (1000) users      (100)     3170 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/decomp/settings_table.ui
--rw-r--r--   0 carl      (1000) users      (100)    38750 2021-09-13 21:13:25.000000 octavvs-0.1.8/octavvs/decomposition.py
--rw-r--r--   0 carl      (1000) users      (100)    91070 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/icons_src_rc.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.101123 octavvs-0.1.8/octavvs/io/
--rw-r--r--   0 carl      (1000) users      (100)      217 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/io/__init__.py
--rwxr-xr-x   0 carl      (1000) users      (100)    20677 2021-09-13 12:12:07.000000 octavvs-0.1.8/octavvs/io/decompositiondata.py
--rw-r--r--   0 carl      (1000) users      (100)      475 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/io/image.py
--rw-r--r--   0 carl      (1000) users      (100)     3430 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/io/opusreader.py
--rw-r--r--   0 carl      (1000) users      (100)      757 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/io/parameters.py
--rw-r--r--   0 carl      (1000) users      (100)     3896 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/io/ptirreader.py
--rw-r--r--   0 carl      (1000) users      (100)     4030 2021-07-02 12:18:30.000000 octavvs-0.1.8/octavvs/io/spectraldata.py
--rw-r--r--   0 carl      (1000) users      (100)     1270 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/launcher.py
--rw-r--r--   0 carl      (1000) users      (100)      917 2021-09-06 13:18:48.000000 octavvs-0.1.8/octavvs/make_icons.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.101123 octavvs-0.1.8/octavvs/mcr/
--rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/mcr/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)     3697 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/mcr/about.ui
--rw-r--r--   0 carl      (1000) users      (100)    55065 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/mcr/clustering_ui.ui
--rw-r--r--   0 carl      (1000) users      (100)     4404 2020-02-19 14:24:37.000000 octavvs-0.1.8/octavvs/mcr/ftir_function.py
--rw-r--r--   0 carl      (1000) users      (100)    37549 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/mcr/mcr_final_loc.ui
--rw-r--r--   0 carl      (1000) users      (100)     2766 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/mcr/mcr_roi_sub.ui
--rw-r--r--   0 carl      (1000) users      (100)     4690 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/mcr/mpl.py
--rw-r--r--   0 carl      (1000) users      (100)     4807 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/mcr/table_ui.ui
--rw-r--r--   0 carl      (1000) users      (100)    59369 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/mcr_als.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.105125 octavvs-0.1.8/octavvs/prep/
--rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/prep/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)     3612 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/prep/create_reference.ui
--rw-r--r--   0 carl      (1000) users      (100)     8941 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/prep/dataplotwidget.py
--rw-r--r--   0 carl      (1000) users      (100)    48114 2019-12-05 23:25:28.000000 octavvs-0.1.8/octavvs/prep/octavvs_prep.icns
--rw-r--r--   0 carl      (1000) users      (100)    10980 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/prep/octavvs_prep.ico
--rw-r--r--   0 carl      (1000) users      (100)     7358 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/prep/octavvs_prep_48.ico
--rw-r--r--   0 carl      (1000) users      (100)    44477 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/prep/preprocessing_ui.ui
--rw-r--r--   0 carl      (1000) users      (100)    15150 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/prep/prepworker.py
--rw-r--r--   0 carl      (1000) users      (100)    16273 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/prep/scadvanced.ui
--rw-r--r--   0 carl      (1000) users      (100)    42285 2021-07-02 12:18:42.000000 octavvs-0.1.8/octavvs/preprocessing.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.105125 octavvs-0.1.8/octavvs/pymcr_new/
--rw-r--r--   0 carl      (1000) users      (100)      159 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/pymcr_new/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)     2103 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/pymcr_new/constraints.py
--rw-r--r--   0 carl      (1000) users      (100)      226 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/pymcr_new/metrics.py
--rw-r--r--   0 carl      (1000) users      (100)     2736 2019-11-27 08:55:42.000000 octavvs-0.1.8/octavvs/pymcr_new/regressors.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.109127 octavvs-0.1.8/octavvs/reference_spectra/
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:38:37.000000 octavvs-0.1.8/octavvs/reference_spectra/CAS_bg_10perc_crub7.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:04:16.000000 octavvs-0.1.8/octavvs/reference_spectra/CAS_wh_5perc.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:43:10.000000 octavvs-0.1.8/octavvs/reference_spectra/CMC_bg_10perc_crub7.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:04:55.000000 octavvs-0.1.8/octavvs/reference_spectra/CMC_wh_5perc.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:46:50.000000 octavvs-0.1.8/octavvs/reference_spectra/LIG_bg_10perc_crub7.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:05:31.000000 octavvs-0.1.8/octavvs/reference_spectra/LIG_wh_5perc.mat
--rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:49:43.000000 octavvs-0.1.8/octavvs/reference_spectra/PEC_bg_10perc_crub7.mat
--rw-r--r--   0 carl      (1000) users      (100)  2640440 2021-04-24 20:44:28.000000 octavvs-0.1.8/octavvs/reference_spectra/Q_table.mat
--rw-r--r--   0 carl      (1000) users      (100)        0 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/reference_spectra/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)    25096 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/reference_spectra/casein.mat
--rw-r--r--   0 carl      (1000) users      (100)    25096 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/reference_spectra/lignin.mat
--rw-r--r--   0 carl      (1000) users      (100)   101224 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/reference_spectra/matrigel.mat
--rw-r--r--   0 carl      (1000) users      (100)    24712 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/reference_spectra/water.mat
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.113128 octavvs-0.1.8/octavvs/ui/
--rw-r--r--   0 carl      (1000) users      (100)      206 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/__init__.py
--rw-r--r--   0 carl      (1000) users      (100)      131 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/constants.py
--rw-r--r--   0 carl      (1000) users      (100)      724 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/copyfigure.py
--rw-r--r--   0 carl      (1000) users      (100)      554 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/elidedlabel.py
--rw-r--r--   0 carl      (1000) users      (100)      962 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/exceptiondialog.py
--rw-r--r--   0 carl      (1000) users      (100)     9282 2021-09-06 13:17:48.000000 octavvs-0.1.8/octavvs/ui/fileloader.py
--rw-r--r--   0 carl      (1000) users      (100)     6254 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/fileloader.ui
--rw-r--r--   0 carl      (1000) users      (100)     7476 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/imagevisualizer.py
--rw-r--r--   0 carl      (1000) users      (100)    11347 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/imagevisualizer.ui
--rw-r--r--   0 carl      (1000) users      (100)     2257 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/linedouble.py
--rw-r--r--   0 carl      (1000) users      (100)      437 2020-03-27 16:04:10.000000 octavvs-0.1.8/octavvs/ui/norepeatstyle.py
--rw-r--r--   0 carl      (1000) users      (100)     7058 2021-09-14 07:31:25.000000 octavvs-0.1.8/octavvs/ui/octavvsapplication.py
--rw-r--r--   0 carl      (1000) users      (100)    15285 2021-09-06 13:17:48.000000 octavvs-0.1.8/octavvs/ui/projectionwidget.py
--rw-r--r--   0 carl      (1000) users      (100)     1693 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/uitools.py
--rw-r--r--   0 carl      (1000) users      (100)     2500 2021-06-30 23:41:02.000000 octavvs-0.1.8/octavvs/ui/whitelightwidget.py
-drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-09-14 07:31:34.097122 octavvs-0.1.8/octavvs.egg-info/
--rw-r--r--   0 carl      (1000) users      (100)     5592 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) users      (100)     2655 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) users      (100)        1 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) users      (100)      186 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/entry_points.txt
--rw-r--r--   0 carl      (1000) users      (100)      102 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) users      (100)        8 2021-09-14 07:31:33.000000 octavvs-0.1.8/octavvs.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) users      (100)       38 2021-09-14 07:31:34.113128 octavvs-0.1.8/setup.cfg
--rw-r--r--   0 carl      (1000) users      (100)     1454 2021-09-14 07:31:25.000000 octavvs-0.1.8/setup.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.404407 octavvs-0.1.9/
+-rw-r--r--   0 carl      (1000) users      (100)     5592 2021-10-08 09:53:08.404407 octavvs-0.1.9/PKG-INFO
+-rw-r--r--   0 carl      (1000) users      (100)     4307 2021-09-06 13:18:48.000000 octavvs-0.1.9/README.md
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.384407 octavvs-0.1.9/octavvs/
+-rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/__init__.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.388407 octavvs-0.1.9/octavvs/algorithms/
+-rw-r--r--   0 carl      (1000) users      (100)        0 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/algorithms/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)     6648 2021-10-05 22:50:20.000000 octavvs-0.1.9/octavvs/algorithms/atm_correction.py
+-rw-r--r--   0 carl      (1000) users      (100)     9232 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/algorithms/baseline.py
+-rw-r--r--   0 carl      (1000) users      (100)      263 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/algorithms/correction.py
+-rwxr-xr-x   0 carl      (1000) users      (100)    14201 2021-10-08 09:49:28.000000 octavvs-0.1.9/octavvs/algorithms/decomposition.py
+-rwxr-xr-x   0 carl      (1000) users      (100)     9306 2021-07-14 11:12:19.000000 octavvs-0.1.9/octavvs/algorithms/decomposition_working.py
+-rwxr-xr-x   0 carl      (1000) users      (100)    11390 2021-07-24 13:08:37.000000 octavvs-0.1.9/octavvs/algorithms/decomposition_working_2.py
+-rw-r--r--   0 carl      (1000) users      (100)    28061 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/algorithms/mie_correction.py
+-rw-r--r--   0 carl      (1000) users      (100)     2035 2021-09-06 13:17:48.000000 octavvs-0.1.9/octavvs/algorithms/normalization.py
+-rw-r--r--   0 carl      (1000) users      (100)     3809 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/algorithms/ptir.py
+-rw-r--r--   0 carl      (1000) users      (100)     4705 2021-09-06 13:17:48.000000 octavvs-0.1.9/octavvs/algorithms/util.py
+-rw-r--r--   0 carl      (1000) users      (100)    55653 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/clustering.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.388407 octavvs-0.1.9/octavvs/decomp/
+-rw-r--r--   0 carl      (1000) users      (100)        0 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/decomp/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)    46734 2021-10-08 09:50:11.000000 octavvs-0.1.9/octavvs/decomp/decomposition.ui
+-rw-r--r--   0 carl      (1000) users      (100)     7303 2021-10-08 09:49:50.000000 octavvs-0.1.9/octavvs/decomp/decompworker.py
+-rwxr-xr-x   0 carl      (1000) users      (100)    26011 2021-09-13 12:12:07.000000 octavvs-0.1.9/octavvs/decomp/plotwidget.py
+-rw-r--r--   0 carl      (1000) users      (100)     3170 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/decomp/settings_table.ui
+-rw-r--r--   0 carl      (1000) users      (100)    39002 2021-10-08 09:49:29.000000 octavvs-0.1.9/octavvs/decomposition.py
+-rw-r--r--   0 carl      (1000) users      (100)    91070 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/icons_src_rc.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.388407 octavvs-0.1.9/octavvs/io/
+-rw-r--r--   0 carl      (1000) users      (100)      217 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/io/__init__.py
+-rwxr-xr-x   0 carl      (1000) users      (100)    20677 2021-09-13 12:12:07.000000 octavvs-0.1.9/octavvs/io/decompositiondata.py
+-rw-r--r--   0 carl      (1000) users      (100)      475 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/io/image.py
+-rw-r--r--   0 carl      (1000) users      (100)     3430 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/io/opusreader.py
+-rw-r--r--   0 carl      (1000) users      (100)      757 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/io/parameters.py
+-rw-r--r--   0 carl      (1000) users      (100)     3896 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/io/ptirreader.py
+-rw-r--r--   0 carl      (1000) users      (100)     4030 2021-07-02 12:18:30.000000 octavvs-0.1.9/octavvs/io/spectraldata.py
+-rw-r--r--   0 carl      (1000) users      (100)     1270 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/launcher.py
+-rw-r--r--   0 carl      (1000) users      (100)      917 2021-09-06 13:18:48.000000 octavvs-0.1.9/octavvs/make_icons.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.392407 octavvs-0.1.9/octavvs/mcr/
+-rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/mcr/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)     3697 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/mcr/about.ui
+-rw-r--r--   0 carl      (1000) users      (100)    55065 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/mcr/clustering_ui.ui
+-rw-r--r--   0 carl      (1000) users      (100)     4404 2020-02-19 14:24:37.000000 octavvs-0.1.9/octavvs/mcr/ftir_function.py
+-rw-r--r--   0 carl      (1000) users      (100)    37549 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/mcr/mcr_final_loc.ui
+-rw-r--r--   0 carl      (1000) users      (100)     2766 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/mcr/mcr_roi_sub.ui
+-rw-r--r--   0 carl      (1000) users      (100)     4690 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/mcr/mpl.py
+-rw-r--r--   0 carl      (1000) users      (100)     4807 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/mcr/table_ui.ui
+-rw-r--r--   0 carl      (1000) users      (100)    59369 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/mcr_als.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.392407 octavvs-0.1.9/octavvs/prep/
+-rw-r--r--   0 carl      (1000) users      (100)        0 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/prep/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)     3612 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/prep/create_reference.ui
+-rw-r--r--   0 carl      (1000) users      (100)     8941 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/prep/dataplotwidget.py
+-rw-r--r--   0 carl      (1000) users      (100)    48114 2019-12-05 23:25:28.000000 octavvs-0.1.9/octavvs/prep/octavvs_prep.icns
+-rw-r--r--   0 carl      (1000) users      (100)    10980 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/prep/octavvs_prep.ico
+-rw-r--r--   0 carl      (1000) users      (100)     7358 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/prep/octavvs_prep_48.ico
+-rw-r--r--   0 carl      (1000) users      (100)    44477 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/prep/preprocessing_ui.ui
+-rw-r--r--   0 carl      (1000) users      (100)    15150 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/prep/prepworker.py
+-rw-r--r--   0 carl      (1000) users      (100)    16273 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/prep/scadvanced.ui
+-rw-r--r--   0 carl      (1000) users      (100)    42285 2021-07-02 12:18:42.000000 octavvs-0.1.9/octavvs/preprocessing.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.392407 octavvs-0.1.9/octavvs/pymcr_new/
+-rw-r--r--   0 carl      (1000) users      (100)      159 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/pymcr_new/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)     2103 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/pymcr_new/constraints.py
+-rw-r--r--   0 carl      (1000) users      (100)      226 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/pymcr_new/metrics.py
+-rw-r--r--   0 carl      (1000) users      (100)     2736 2019-11-27 08:55:42.000000 octavvs-0.1.9/octavvs/pymcr_new/regressors.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.400407 octavvs-0.1.9/octavvs/reference_spectra/
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:38:37.000000 octavvs-0.1.9/octavvs/reference_spectra/CAS_bg_10perc_crub7.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:04:16.000000 octavvs-0.1.9/octavvs/reference_spectra/CAS_wh_5perc.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:43:10.000000 octavvs-0.1.9/octavvs/reference_spectra/CMC_bg_10perc_crub7.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:04:55.000000 octavvs-0.1.9/octavvs/reference_spectra/CMC_wh_5perc.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:46:50.000000 octavvs-0.1.9/octavvs/reference_spectra/LIG_bg_10perc_crub7.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 23:05:31.000000 octavvs-0.1.9/octavvs/reference_spectra/LIG_wh_5perc.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24664 2021-03-02 13:49:43.000000 octavvs-0.1.9/octavvs/reference_spectra/PEC_bg_10perc_crub7.mat
+-rw-r--r--   0 carl      (1000) users      (100)  2640440 2021-04-24 20:44:28.000000 octavvs-0.1.9/octavvs/reference_spectra/Q_table.mat
+-rw-r--r--   0 carl      (1000) users      (100)        0 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/reference_spectra/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)    25096 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/reference_spectra/casein.mat
+-rw-r--r--   0 carl      (1000) users      (100)    25096 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/reference_spectra/lignin.mat
+-rw-r--r--   0 carl      (1000) users      (100)   101224 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/reference_spectra/matrigel.mat
+-rw-r--r--   0 carl      (1000) users      (100)    24712 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/reference_spectra/water.mat
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.404407 octavvs-0.1.9/octavvs/ui/
+-rw-r--r--   0 carl      (1000) users      (100)      206 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/__init__.py
+-rw-r--r--   0 carl      (1000) users      (100)      131 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/constants.py
+-rw-r--r--   0 carl      (1000) users      (100)      724 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/copyfigure.py
+-rw-r--r--   0 carl      (1000) users      (100)      554 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/elidedlabel.py
+-rw-r--r--   0 carl      (1000) users      (100)      962 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/exceptiondialog.py
+-rw-r--r--   0 carl      (1000) users      (100)     9282 2021-09-06 13:17:48.000000 octavvs-0.1.9/octavvs/ui/fileloader.py
+-rw-r--r--   0 carl      (1000) users      (100)     6254 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/fileloader.ui
+-rw-r--r--   0 carl      (1000) users      (100)     7476 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/imagevisualizer.py
+-rw-r--r--   0 carl      (1000) users      (100)    11347 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/imagevisualizer.ui
+-rw-r--r--   0 carl      (1000) users      (100)     2257 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/linedouble.py
+-rw-r--r--   0 carl      (1000) users      (100)      437 2020-03-27 16:04:10.000000 octavvs-0.1.9/octavvs/ui/norepeatstyle.py
+-rw-r--r--   0 carl      (1000) users      (100)     7058 2021-10-08 09:52:55.000000 octavvs-0.1.9/octavvs/ui/octavvsapplication.py
+-rw-r--r--   0 carl      (1000) users      (100)    15285 2021-09-06 13:17:48.000000 octavvs-0.1.9/octavvs/ui/projectionwidget.py
+-rw-r--r--   0 carl      (1000) users      (100)     1693 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/uitools.py
+-rw-r--r--   0 carl      (1000) users      (100)     2500 2021-06-30 23:41:02.000000 octavvs-0.1.9/octavvs/ui/whitelightwidget.py
+drwxr-xr-x   0 carl      (1000) users      (100)        0 2021-10-08 09:53:08.384407 octavvs-0.1.9/octavvs.egg-info/
+-rw-r--r--   0 carl      (1000) users      (100)     5592 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) users      (100)     2655 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) users      (100)        1 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) users      (100)      186 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/entry_points.txt
+-rw-r--r--   0 carl      (1000) users      (100)      102 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) users      (100)        8 2021-10-08 09:53:07.000000 octavvs-0.1.9/octavvs.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) users      (100)       38 2021-10-08 09:53:08.404407 octavvs-0.1.9/setup.cfg
+-rw-r--r--   0 carl      (1000) users      (100)     1454 2021-10-08 09:52:55.000000 octavvs-0.1.9/setup.py
```

### Comparing `octavvs-0.1.8/PKG-INFO` & `octavvs-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octavvs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Chemometrics Toolkit for Analysis and Visualization of Vibrational Spectroscopy data
 Home-page: https://github.com/ctroein/octavvs
 Author: Syahril Siregar, Carl Troein, Michiel Op De Beeck et al.
 Author-email: carl@thep.lu.se
 License: UNKNOWN
 Description: # OCTAVVS: Open Chemometrics Toolbox for Analysis and Visualization of Vibrational Spectroscopy data
```

### Comparing `octavvs-0.1.8/README.md` & `octavvs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/atm_correction.py` & `octavvs-0.1.9/octavvs/algorithms/atm_correction.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         ranges = np.array([0, len(wn)])
     else:
         ranges = find_wn_ranges(wn, ranges)
 
     for i in range(corr_ranges):
         p, q = ranges[i]
         if q - p < 2: continue
-        atm[p:q] -= baseline.straight(wn[p:q], atm[p:q]);
+        atm[p:q] -= baseline.straight(wn[p:q], atm[p:q])
 
     savgolwin = 1 + 2 * int(smooth_win * (len(wn) - 1) / np.abs(wn[0] - wn[-1]))
 
     if progressCallback:
         progressA = 0
         progressB = 1 + corr_ranges * (extra_iters + (1 if savgolwin > 1 else 0))
         progressCallback(progressA, progressB)
```

### Comparing `octavvs-0.1.8/octavvs/algorithms/baseline.py` & `octavvs-0.1.9/octavvs/algorithms/baseline.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/decomposition.py` & `octavvs-0.1.9/octavvs/algorithms/decomposition_working_2.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 Created on Tue May 18 14:45:53 2021
 
 @author: carl
 """
 
 import numpy as np
 import scipy
+import sklearn
+import sklearn.metrics
 import time
-from threadpoolctl import threadpool_limits
 
 def simplisma(d, nr, f):
     """
     The SIMPLISMA algorithm for finding a set of 'pure' spectra to serve
     as starting point for MCR-ALS etc.
     Reference Matlab Code:
         J. Jaumot, R. Gargallo, A. de Juan, R. Tauler,
@@ -66,250 +67,234 @@
             w[j] = np.linalg.det(dm[0:i+1, 0:i+1])
         imp[i] = (p * w).argmax()
 
     ss = d[:,imp]
     spout = ss / np.sqrt(np.sum(ss**2, axis=0))
     return spout.T, imp
 
+# import pymcr
+
+
+# def pymcr_als(sp, initial_components, maxiters, reltol,
+#             callback_iter):
+
+#     mcr = pymcr.mcr.McrAR(max_iter=maxiters,
+#                           tol_err_change=reltol,
+#                           tol_increase=1., tol_n_increase=10,
+#                           tol_n_above_min=30)
+#     mcr.fit(sp, ST=initial_components, post_iter_fcn=callback_iter)
+
+#     return mcr.n_iter, mcr.C_opt_.T, mcr.ST_opt_, np.asarray(mcr.err)
 
-def numpy_scipy_threading_fix_(func):
-    """
-    This decorator for mcr_als prevents threading in BLAS if scipy's NNLS
-    is used, because for some reason NNLS won't be parallelized if called
-    shortly after lstsq or @. This makes a *massive* difference to the
-    time needed for Anderson acceleration, where the BLAS calls themselves
-    take negligible time. For mixed NNLS/lstsq solving (of MCR-ALS on
-    derivatives) it's less obvious whether NNSL or lstsq should be allowed
-    to be parallelized.
-    Note: This issue is seen on
-    """
-    def check(*args, **kwargs):
-        if np.any(kwargs['nonnegative']):
-            with threadpool_limits(1, 'blas'):
-                return func(*args, **kwargs)
-        else:
-            return func(*args, **kwargs)
-    return check
 
-@numpy_scipy_threading_fix_
-def mcr_als(sp, initial_A, *, maxiters, nonnegative=(True, True),
+def mcr_als(sp, initial_components, maxiters, nonnegative=(True, True),
             tol_abs_error=0, tol_rel_improv=None, tol_ups_after_best=None,
-            maxtime=None, callback=None, acceleration=None, normalize=None,
-            contrast_weight=None, return_time=False, **kwargs):
+            maxtime=None, callback=None, acceleration=None,
+            return_time=False, **kwargs):
     """
     Perform MCR-ALS nonnegative matrix decomposition on the matrix sp
 
     Parameters
     ----------
     sp : array(nsamples, nfeatures)
         Spectra to be decomposed.
-    initial_A : array(ncomponents, nfeatures)
-        Initial spectra or concentrations.
+    initial_components : array(ncomponents, nfeatures)
+        Initial concentrations.
     maxiters : int
         Maximum number of iterations.
-    nonnegative : pair of bool, default (True, True)
+    nonnegative : pair of bool
         True if (initial, other) components must be non-negative
     tol_abs_error : float, optional
         Error target (mean square error).
     tol_rel_improv : float, optional
         Stop when relative improvement is less than this over 10 iterations.
     tol_ups_after_best : int, optional
         Stop after error going net up this many times since best error.
     maxtime : float, optional
         Stop after this many seconds of process time have elapsed
     callback : func(it : int, err : float, A : array, B : array)
         Callback for every iteration.
-    acceleration : str, optional
-        None or 'Anderson'.
-        Anderson acceleration operates on whole iterations (A or B updates),
+    acceleration : str
+        None, 'Anderson', 'AdaptiveOverstep'.
+        Use one of two stabilized acceleration schemes.
+        Anderson acceleration operates on whole iterations (A+B updates),
         mixing earlier directions to step towards the fixed point. This
-        implementation restarts from basic updates when those would be
-        better.
-    normalize : str, optional
-        Which matrix to l2 normalize: None, 'A' or 'B'
-    contrast_weight : (str, float), optional
-        Increase contrast in one matrix by mixing the other, named matrix
-        ('A' or 'B') with the mean of its vectors. If A is spectra,
-        try contrast_weight=('B', 0.05) to increase spectral contrast.
-        See Windig and Keenan, Applied Spectroscopy 65: 349 (2011).
-    return_time : bool, default False
+        implementation temporarily falls back to basic updates if those
+        would be much better.
+        The AdaptiveOverstep algorithm attempts to gradually modify the
+        step length, picking the best of a shorter or longer step.
+    m : int, >1
+        For Anderson acceleration: the number of earlier steps to consider.
+    return_time : bool
         Measure and return process_time at each iteration.
 
-    Anderson acceleration parameters in kwargs
-    -------
-    m : int, >1, default 2
-        The maximum number of earlier steps to consider.
-    alternate : bool, default True
-        Alternate between accelerating A and B, switching when restarting.
-    beta : float, default 1.
-        Scaling factor for accelerated step length.
-    betascale : float, default 1.
-        Reduction factor for beta after each restart.
-    bmode : bool, default False
-        Start with accelerating B instead of A.
-
     Returns
     -------
     A : array(ncomponents, nfeatures)
         Spectra (at lowest error)
     B : array(ncomponents, nsamples)
         Concentrations at lowest error
     error : list(float)
         Mean square error at every iteration
     process_time : list(float)
         Time relative start at each iteration, only if return_time is True.
     """
-    if normalize not in [None, 'A', 'B']:
-        raise ValueError('Normalization must be None, A or B')
-    unknown_args = kwargs.keys() - {
-        'm', 'alternate', 'beta', 'betascale', 'bmode'}
-    if unknown_args:
-        raise TypeError('Unknown arguments: {}'.format(unknown_args))
-
-    nrow, ncol = sp.shape
-    nr = initial_A.shape[0]
-    if normalize == 'A':
-        norm = np.linalg.norm(initial_A, axis=1)
-        A = np.divide(initial_A.T, norm, where=norm!=0,
-                      out=np.zeros(initial_A.shape[::-1]))
-    else:
-        A = initial_A.T.copy()
+    nrow, ncol = np.shape(sp)
+    nr = initial_components.shape[0]
+    A = initial_components.T.copy()
     B = np.empty((nr, nrow))
     errors = []
     errorbest = None # Avoid spurious warning
-    # prevA, prevB = (None, None)
-    newA = newB = None
-    error = preverror = None
-
-    cw = 0
-    if contrast_weight is not None:
-        if contrast_weight[0] == 'A':
-            cw = contrast_weight[1]
-        elif contrast_weight[0] == 'B':
-            cw = -contrast_weight[1]
-        else:
-            raise ValueError("contrast_weight must be ('A'|'B', [0-1])")
+    prevA, prevB = (None, None)
 
+    unknown_args = kwargs.keys() - {'m', 'aosettings'}
+    if unknown_args:
+        raise TypeError('Unknown arguments: {}'.format(unknown_args))
 
-    if acceleration == 'Anderson':
-        ason_Bmode = kwargs.get('bmode', False)
-        ason_alternate = kwargs.get('alternate', True)
+    if acceleration == 'AndersonOld':
+        ason_m = kwargs.get('m', 2)
+        ason_g = None
+        ason_G = []
+        ason_X = []
+    elif acceleration == 'Anderson':
         ason_m = kwargs.get('m', 2)
-        ason_beta = kwargs.get('beta', 1.)
-        ason_betascale = kwargs.get('betascale', 1.)
         ason_g = None
         ason_G = []
         ason_X = []
     elif acceleration:
         raise ValueError("acceleration must be None or 'Anderson'")
 
     starttime = time.process_time()
     if return_time:
         times = []
     tol_rel_iters = 10
 
+    aerror = berror = saveA = 0 # Avoid warnings
     for it in range(maxiters):
-        ba = 0
-        retry = False
-        while ba < 2:
-            if not retry:
-                preverror = error
-            if ba == 0:
-                if newA is None:
-                    newA = A
-                prevA = newA
-                if cw > 0:
-                    newA = (1 - cw) * newA + cw * newA.mean(1)[:,None]
-                if nonnegative[1]:
-                    error = 0
-                    if not retry:
-                        B = np.empty_like(B)
-                    for i in range(nrow):
-                        B[:, i], res = scipy.optimize.nnls(newA, sp[i, :])
-                        error = error + res * res
-                else:
-                    B, res, _, _ = np.linalg.lstsq(newA, sp.T, rcond=-1)
-                    error = res.sum()
-                if normalize == 'B':
-                    norm = np.linalg.norm(B, axis=1)
-                    B = np.divide(B.T, norm, where=norm!=0, out=B.T).T
-                newA = None
+        # print('strides', it, A.strides, B.strides)
+        # Update B
+        while(True):
+            prevB = B
+            if nonnegative[1]:
+                error = 0
+                B = np.empty_like(B)
+                for i in range(nrow):
+                    B[:, i], res = scipy.optimize.nnls(A, sp[i, :])
+                    error = error + res * res
             else:
-                if newB is None:
-                    newB = B
-                prevB = newB
-                if cw < 0:
-                    newB = (1 + cw) * newB - cw * newB.mean(1)[:,None]
-                if nonnegative[0]:
-                    error = 0
-                    if not retry:
-                        A = np.empty_like(A)
-                    for i in range(ncol):
-                        A[i, :], res = scipy.optimize.nnls(newB.T, sp[:, i])
-                        error = error + res * res
-                else:
-                    A, res, _, _ = np.linalg.lstsq(newB.T, sp, rcond=-1)
-                    A = A.T
-                    error = res.sum()
-                if normalize == 'A':
-                    norm = np.linalg.norm(A, axis=0)
-                    np.divide(A, norm, where=norm!=0, out=A)
-                newB = None
-
-            if acceleration is None:
-                pass
-            elif ba == ason_Bmode:
-                if retry:
-                    retry = False
-                    if ason_alternate:
-                        ason_Bmode = not ason_Bmode
-                    ason_beta = ason_beta * ason_betascale
-                elif len(ason_X) > 1 and error > preverror:
+                B, res, _, _ = np.linalg.lstsq(A, sp.T, rcond=-1)
+                error = res.sum()
+
+            if acceleration == 'Anderson' and len(ason_X) > 1 \
+                and error > aerror:
+                print('restart', it, error-aerror, error-berror)
+                print('gamma', gamma, np.linalg.norm(ason_g))
+                ason_X = []
+                ason_G = []
+                A = saveA
+            else:
+                if acceleration == 'Anderson' and len(ason_X) < 1:
+                    print('Bstep', it, error-aerror, error-berror)
+                break
+        berror = error
+
+        prevA = A
+        if nonnegative[0]:
+            error = 0
+            A = np.empty_like(A)
+            for i in range(ncol):
+                A[i, :], res = scipy.optimize.nnls(B.T, sp[:, i])
+                error = error + res * res
+        else:
+            A, res, _, _ = np.linalg.lstsq(B.T, sp, rcond=-1)
+            A = A.T
+            error = res.sum()
+
+        if acceleration == 'Anderson':
+            aerror = error
+            prevg = ason_g
+            ason_g = (A - prevA).flatten()
+            if len(ason_X) < 1:
+                ason_X.append(ason_g)
+            else:
+                ason_G.append(ason_g - prevg)
+                while(len(ason_G) > ason_m):
+                    ason_G.pop(0)
+                    ason_X.pop(0)
+                Garr = np.asarray(ason_G)
+                try:
+                    gamma = np.linalg.lstsq(Garr.T, ason_g, rcond=-1)[0]
+                    # print('gamma', gamma, np.linalg.norm(ason_g))
+                except np.linalg.LinAlgError:
+                    print('lstsq failed to converge; restart at iter %d' % it)
+                    print('nans', np.isnan(Garr).sum(), np.isnan(ason_g).sum())
                     ason_X = []
                     ason_G = []
-                    retry = True
-                    ba = ba - 1
                 else:
-                    pass
-            elif ason_Bmode == 1 and it == 0:
-                pass
+                    dx = ason_g - gamma @ (np.asarray(ason_X) + Garr)
+                    ason_X.append(dx)
+                    saveA = A
+                    # A = prevA + dx.reshape(A.shape)
+                    if nonnegative[0]:
+                        A = np.maximum(0, A)
+
+        error = error / sp.size
+
+        # Anderson
+        # A0 -> B0   errb0
+        # B0 -> A1   erra1:E  A1-A0: X0,g0
+        # A1 -> B1   errb1
+        # B1 -> A2   erra2:E  A2-A1: g1  g1-g0: G0   g1=v0G: v0
+        #            g1-v0(X+G): X1   A1+X1: A'2
+        # A'2 -> B2  errb2  if errb2>erra2:  XG=[]  A2 -> B2   (seed??)
+        # B2 -> A3   erra3:E  A3-A2: g2  g2-g1: G1   g2=v1G: v1
+        #            g2-v1(X+G): X2   A2+X2: A'3
+        # A'3 -> B3  errb3  if errb3>erra3:  XG=[]  A3 -> B3   (seed??)
+
+        if acceleration == 'AndersonOld' and it > 2:
+            prevg = ason_g
+            ason_g = np.empty(A.size + B.size)
+            ason_g[:A.size] = (A - prevA).flatten()
+            ason_g[A.size:] = (B - prevB).flatten()
+            if len(ason_X) < 1:
+                ason_X.append(ason_g)
             else:
-                prevg = ason_g
-                ason_g = ((A - prevA) if ba else (B - prevB)).flatten()
-                if len(ason_X) < 1:
-                    ason_X.append(ason_g)
+                ason_G.append(ason_g - prevg)
+                while(len(ason_G) > ason_m):
+                    ason_G.pop(0)
+                    ason_X.pop(0)
+                Garr = np.asarray(ason_G)
+                try:
+                    gamma = np.linalg.lstsq(Garr.T, ason_g, rcond=-1)[0]
+                except np.linalg.LinAlgError:
+                    print('lstsq failed to converge; restart at iter %d' % it)
+                    print('nans', np.isnan(Garr).sum(), np.isnan(ason_g).sum())
+                    ason_X = []
+                    ason_G = []
                 else:
-                    ason_G.append(ason_g - prevg)
-                    while(len(ason_G) > ason_m):
-                        ason_G.pop(0)
-                        ason_X.pop(0)
-                    Garr = np.asarray(ason_G)
-                    try:
-                        gamma = scipy.linalg.lstsq(Garr.T, ason_g)[0]
-                    except scipy.linalg.LinAlgError:
-                        print('lstsq failed to converge; '
-                              'restart at iter %d' % it)
-                        # print('nans', np.isnan(Garr).sum(),
-                        #       np.isnan(ason_g).sum())
+                    # print('gamma', gamma, np.linalg.norm(ason_g))
+                    xstep = ason_g - gamma @ (np.asarray(ason_X) + Garr)
+                    ason_X.append(xstep)
+                    nA = prevA + xstep[:A.size].reshape(A.shape)
+                    if nonnegative[0]:
+                        nA = np.maximum(0, nA)
+                    nB = prevB + xstep[A.size:].reshape(B.shape)
+                    if nonnegative[1]:
+                        nB = np.maximum(0, nB)
+                    nerror = np.linalg.norm(sp - nB.T @ nA.T)**2 / sp.size
+                    # Reject changes that are much worse than the basic step
+                    de = error - errors[-1]
+                    nde = nerror - errors[-1]
+                    if nde > .5 * de or (de > 0 and nde > 2 * de):
                         ason_X = []
                         ason_G = []
+                        print('aold restart',it)
                     else:
-                        gamma = ason_beta * gamma
-                        dx = ason_g - gamma @ (np.asarray(ason_X) + Garr)
-                        ason_X.append(dx)
-                        if ba:
-                            newA = prevA + dx.reshape(A.shape)
-                            if nonnegative[0]:
-                                np.maximum(0, newA, out=newA)
-                        else:
-                            newB = prevB + dx.reshape(B.shape)
-                            if nonnegative[1]:
-                                np.maximum(0, newB, out=newB)
-            ba = ba + 1
-        # error = error / sp.size
+                        A, B, error = (nA, nB, nerror)
+
 
         curtime = time.process_time() - starttime
         if return_time:
             times.append(curtime)
         errors.append(error)
         if not it or error < errorbest:
             errorbest = error
```

### Comparing `octavvs-0.1.8/octavvs/algorithms/decomposition_working.py` & `octavvs-0.1.9/octavvs/algorithms/decomposition_working.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/mie_correction.py` & `octavvs-0.1.9/octavvs/algorithms/mie_correction.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/normalization.py` & `octavvs-0.1.9/octavvs/algorithms/normalization.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/ptir.py` & `octavvs-0.1.9/octavvs/algorithms/ptir.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/algorithms/util.py` & `octavvs-0.1.9/octavvs/algorithms/util.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/clustering.py` & `octavvs-0.1.9/octavvs/clustering.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/decomp/decomposition.ui` & `octavvs-0.1.9/octavvs/prep/preprocessing_ui.ui`

 * *Files 7% similar despite different names*

#### Comparing `octavvs-0.1.8/octavvs/decomp/decomposition.ui` & `octavvs-0.1.9/octavvs/prep/preprocessing_ui.ui`

```diff
@@ -2,31 +2,31 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1166</width>
-        <height>785</height>
+        <width>1423</width>
+        <height>955</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>OCTAVVS Decomposition</string>
+      <string>OCTAVVS Preprocessing</string>
     </property>
     <property name="styleSheet">
       <string notr="true">QSplitter::handle:horizontal {
 border: 1px solid #ccc;
 border-right-color: #bbb;
 border-bottom-color: #bbb;
 margin: 5px;
 }</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <layout class="QHBoxLayout" name="horizontalLayout_17" stretch="3,5">
+      <layout class="QHBoxLayout" name="horizontalLayout_17" stretch="1,1,1">
         <property name="leftMargin">
           <number>6</number>
         </property>
         <property name="topMargin">
           <number>6</number>
         </property>
         <property name="rightMargin">
@@ -52,1158 +52,1130 @@
             </item>
             <item>
               <widget class="ImageVisualizerWidget" name="imageVisualizer" native="true"/>
             </item>
           </layout>
         </item>
         <item>
-          <layout class="QVBoxLayout" name="verticalLayout_2" stretch="0,0,0">
+          <layout class="QVBoxLayout" name="verticalLayout_4" stretch="0,1,0,0,1,0,0,0,1,0,1">
+            <property name="sizeConstraint">
+              <enum>QLayout::SetMinimumSize</enum>
+            </property>
+            <item>
+              <widget class="QWidget" name="widgetMC" native="true">
+                <layout class="QVBoxLayout" name="verticalLayout_6" stretch="0">
+                  <property name="leftMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="topMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="rightMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="bottomMargin">
+                    <number>0</number>
+                  </property>
+                  <item>
+                    <layout class="QHBoxLayout" name="horizontalLayout_16" stretch="4,2,1,2,1">
+                      <property name="topMargin">
+                        <number>0</number>
+                      </property>
+                      <item>
+                        <widget class="QCheckBox" name="checkBoxMC">
+                          <property name="font">
+                            <font>
+                              <weight>75</weight>
+                              <bold>true</bold>
+                            </font>
+                          </property>
+                          <property name="toolTip">
+                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Clustered Resonant Mie Scattering Correction; see the article by Troein, Siregar, Op De Beeck et al for details and consult the thesis of Paul Bassan for a description of the basic algorithm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                          </property>
+                          <property name="layoutDirection">
+                            <enum>Qt::LeftToRight</enum>
+                          </property>
+                          <property name="text">
+                            <string>mIRage correction</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="label_6">
+                          <property name="text">
+                            <string>Endpoints</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                          </property>
+                          <property name="buddy">
+                            <cstring>spinBoxMCEndpoints</cstring>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QSpinBox" name="spinBoxMCEndpoints">
+                          <property name="minimum">
+                            <number>2</number>
+                          </property>
+                          <property name="maximum">
+                            <number>40</number>
+                          </property>
+                          <property name="value">
+                            <number>6</number>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="label_7">
+                          <property name="text">
+                            <string>Slopefactor</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                          </property>
+                          <property name="buddy">
+                            <cstring>lineEditMCSlopefactor</cstring>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="LineDouble" name="lineEditMCSlopefactor">
+                          <property name="text">
+                            <string>.5</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                </layout>
+              </widget>
+            </item>
             <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_8">
+              <widget class="MCPlotWidget" name="plot_MC" native="true"/>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_15" stretch="0,1">
                 <item>
-                  <widget class="QLabel" name="label_20">
+                  <widget class="QCheckBox" name="checkBoxAC">
+                    <property name="font">
+                      <font>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
                     <property name="toolTip">
-                      <string>Where to save decomposition metadata (.dmd) files. 'Other directory' requires that input files have unique names.</string>
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Atmospheric correction, designed to remove spectral contributions from H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O and CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; by subtracting an atmospheric reference spectrum (times an appropriate factor) in each of two H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions and, optionally, one CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; region.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
+                    <property name="layoutDirection">
+                      <enum>Qt::LeftToRight</enum>
                     </property>
                     <property name="text">
-                      <string>Save data in</string>
+                      <string>Atmospheric correction</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QComboBox" name="comboBoxDirectory">
-                    <item>
-                      <property name="text">
-                        <string>Input directory</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>Other directory</string>
-                      </property>
-                    </item>
+                  <widget class="QLabel" name="labelACInfo">
+                    <property name="toolTip">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Estimated mean magnitude of the corrections, relative to the level in the corrected regions.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
+                    <property name="text">
+                      <string/>
+                    </property>
+                    <property name="textFormat">
+                      <enum>Qt::AutoText</enum>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
                   </widget>
                 </item>
+              </layout>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_4" stretch="1,1,1,0,3">
                 <item>
-                  <widget class="QLineEdit" name="lineEditDirectory">
-                    <property name="enabled">
-                      <bool>false</bool>
+                  <widget class="QCheckBox" name="checkBoxSpline">
+                    <property name="toolTip">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Replace data in the CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; region (2245-2445 cm&lt;span style=&quot; vertical-align:super;&quot;&gt;-1&lt;/span&gt;) with a smooth curve. Otherwise apply the same type of correction as in the H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
+                    <property name="text">
+                      <string>Spline at CO₂</string>
+                    </property>
+                    <property name="checked">
+                      <bool>true</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QPushButton" name="pushButtonDirectory">
+                  <widget class="QCheckBox" name="checkBoxLocalPeak">
+                    <property name="toolTip">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Attempt to refine the correction in a small sliding window to account for fluctuations in H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O peak intensities.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
                     <property name="text">
-                      <string>Select dir</string>
+                      <string>Local peak corr.</string>
+                    </property>
+                    <property name="checked">
+                      <bool>true</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QPushButton" name="pushButtonLoadParameters">
+                  <widget class="QCheckBox" name="checkBoxSmoothCorrected">
+                    <property name="toolTip">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Apply a weak denoising filter to the H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions of the spectrum.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
                     <property name="text">
-                      <string>Load parameters</string>
+                      <string>Smoothing</string>
+                    </property>
+                    <property name="checked">
+                      <bool>true</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QPushButton" name="pushButtonSaveParameters">
+                  <widget class="QPushButton" name="pushButtonACLoadReference">
                     <property name="text">
-                      <string>Save parameters</string>
+                      <string>Load ref.</string>
                     </property>
                   </widget>
                 </item>
+                <item>
+                  <widget class="QLineEdit" name="lineEditACReference"/>
+                </item>
               </layout>
             </item>
             <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_10" stretch="0,0,0">
+              <widget class="ACPlotWidget" name="plot_AC" native="true"/>
+            </item>
+            <item>
+              <widget class="QWidget" name="widgetSC" native="true">
+                <layout class="QHBoxLayout" name="layoutSC_1" stretch="4,1,0">
+                  <property name="leftMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="topMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="rightMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="bottomMargin">
+                    <number>0</number>
+                  </property>
+                  <item>
+                    <widget class="QCheckBox" name="checkBoxSC">
+                      <property name="font">
+                        <font>
+                          <weight>75</weight>
+                          <bold>true</bold>
+                        </font>
+                      </property>
+                      <property name="toolTip">
+                        <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Clustered Resonant Mie Scattering Correction; see the article by Troein, Siregar, Op De Beeck et al for details and consult the thesis of Paul Bassan for a description of the basic algorithm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                      </property>
+                      <property name="layoutDirection">
+                        <enum>Qt::LeftToRight</enum>
+                      </property>
+                      <property name="text">
+                        <string>Scattering correction (CRMieSC)</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <widget class="QPushButton" name="pushButtonSCRefresh">
+                      <property name="enabled">
+                        <bool>false</bool>
+                      </property>
+                      <property name="text">
+                        <string>Update</string>
+                      </property>
+                    </widget>
+                  </item>
+                  <item>
+                    <widget class="QToolButton" name="pushButtonSCStop">
+                      <property name="enabled">
+                        <bool>false</bool>
+                      </property>
+                      <property name="text">
+                        <string>Stop</string>
+                      </property>
+                    </widget>
+                  </item>
+                </layout>
+              </widget>
+            </item>
+            <item>
+              <widget class="QProgressBar" name="progressBarSC">
+                <property name="value">
+                  <number>0</number>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <widget class="QWidget" name="widgetSCOptions" native="true">
+                <layout class="QVBoxLayout" name="verticalLayout_5">
+                  <property name="leftMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="topMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="rightMargin">
+                    <number>0</number>
+                  </property>
+                  <property name="bottomMargin">
+                    <number>0</number>
+                  </property>
+                  <item>
+                    <layout class="QHBoxLayout" name="layoutSC_2" stretch="0,1,4">
+                      <item>
+                        <widget class="QLabel" name="label_36">
+                          <property name="text">
+                            <string>Reference</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                          </property>
+                          <property name="buddy">
+                            <cstring>comboBoxReference</cstring>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QComboBox" name="comboBoxReference">
+                          <property name="sizePolicy">
+                            <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
+                              <horstretch>0</horstretch>
+                              <verstretch>0</verstretch>
+                            </sizepolicy>
+                          </property>
+                          <property name="toolTip">
+                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Reference spectrum used to initialize the RMieSC algorithm; choose a non-scattered spectrum from a sample as similar as possible to that studied.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                          </property>
+                          <item>
+                            <property name="text">
+                              <string>Mean</string>
+                            </property>
+                          </item>
+                          <item>
+                            <property name="text">
+                              <string>Percentile</string>
+                            </property>
+                          </item>
+                          <item>
+                            <property name="text">
+                              <string>Casein</string>
+                            </property>
+                          </item>
+                          <item>
+                            <property name="text">
+                              <string>Lignin</string>
+                            </property>
+                          </item>
+                          <item>
+                            <property name="text">
+                              <string>Matrigel</string>
+                            </property>
+                          </item>
+                          <item>
+                            <property name="text">
+                              <string>Other</string>
+                            </property>
+                          </item>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QStackedWidget" name="stackedSC">
+                          <property name="currentIndex">
+                            <number>0</number>
+                          </property>
+                          <widget class="QWidget" name="page">
+                            <layout class="QHBoxLayout" name="horizontalLayout_24" stretch="2,1,3">
+                              <property name="leftMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="topMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="rightMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="bottomMargin">
+                                <number>0</number>
+                              </property>
+                              <item>
+                                <widget class="QLabel" name="label_4">
+                                  <property name="text">
+                                    <string>Percentile</string>
+                                  </property>
+                                  <property name="alignment">
+                                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                  </property>
+                                  <property name="buddy">
+                                    <cstring>lineEditSCRefPercentile</cstring>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="LineDouble" name="lineEditSCRefPercentile"/>
+                              </item>
+                              <item>
+                                <widget class="QPushButton" name="pushButtonCreateReference">
+                                  <property name="text">
+                                    <string>Create from dataset</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                          <widget class="QWidget" name="page_5">
+                            <layout class="QHBoxLayout" name="horizontalLayout_25" stretch="0,0">
+                              <property name="leftMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="topMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="rightMargin">
+                                <number>0</number>
+                              </property>
+                              <property name="bottomMargin">
+                                <number>0</number>
+                              </property>
+                              <item>
+                                <widget class="QPushButton" name="pushButtonLoadOther">
+                                  <property name="toolTip">
+                                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Load your own reference spectrum. This should be a MATLAB matrix called 'AB' with two columns: wavenumber and intensity.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                                  </property>
+                                  <property name="text">
+                                    <string>Load other</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="lineEditReferenceName">
+                                  <property name="readOnly">
+                                    <bool>true</bool>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                  <item>
+                    <layout class="QHBoxLayout" name="layoutSC_3" stretch="0,1,0,1,0,1">
+                      <item>
+                        <widget class="QLabel" name="label_38">
+                          <property name="text">
+                            <string>Max iterations</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                          </property>
+                          <property name="buddy">
+                            <cstring>spinBoxNIteration</cstring>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QSpinBox" name="spinBoxNIteration">
+                          <property name="toolTip">
+                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Iterations of the RMieSC algorithm; a value of 10-20 may be required for good convergence.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                          </property>
+                          <property name="minimum">
+                            <number>1</number>
+                          </property>
+                          <property name="maximum">
+                            <number>999</number>
+                          </property>
+                          <property name="singleStep">
+                            <number>1</number>
+                          </property>
+                          <property name="value">
+                            <number>30</number>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QCheckBox" name="checkBoxClusters">
+                          <property name="text">
+                            <string>Clusters</string>
+                          </property>
+                          <property name="checked">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QSpinBox" name="spinBoxNclusScat">
+                          <property name="toolTip">
+                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;The number of clusters to divide the spectra into when computing new reference spectra. This must be set high enough that the spectra in each cluster are practically identical, in which case it will confer robustness to the correction. A value of 0 disables clustering; the spectra are then corrected individually which takes a very long time and gives less robust results.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                          </property>
+                          <property name="minimum">
+                            <number>1</number>
+                          </property>
+                          <property name="maximum">
+                            <number>100</number>
+                          </property>
+                          <property name="singleStep">
+                            <number>1</number>
+                          </property>
+                          <property name="value">
+                            <number>30</number>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QCheckBox" name="checkBoxStabilize">
+                          <property name="toolTip">
+                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;With this option, the scattering correction is stabilized by two means: first fittiing a common reference spectrum to the whole image before fitting with clustering, and in later iterations updating reference spectra with mixing between previous and new.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                          </property>
+                          <property name="text">
+                            <string>Stabilize</string>
+                          </property>
+                          <property name="checked">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QPushButton" name="pushButtonSCAdvanced">
+                          <property name="text">
+                            <string>Advanced</string>
+                          </property>
+                        </widget>
+                      </item>
+                    </layout>
+                  </item>
+                </layout>
+              </widget>
+            </item>
+            <item>
+              <widget class="SCPlotWidget" name="plot_SC" native="true"/>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_9" stretch="0,2,1,1,1">
                 <item>
-                  <widget class="QPushButton" name="pushButtonRdcLoad">
-                    <property name="toolTip">
-                      <string>Load selection from an arbitrary file</string>
+                  <widget class="QCheckBox" name="checkBoxSGF">
+                    <property name="font">
+                      <font>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
+                    </property>
+                    <property name="layoutDirection">
+                      <enum>Qt::LeftToRight</enum>
                     </property>
                     <property name="text">
-                      <string>Load</string>
+                      <string>Denoising (Savitzky-Golay) filter</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QPushButton" name="pushButtonRdcSave">
+                  <widget class="QLabel" name="label_16">
                     <property name="text">
-                      <string>Save</string>
+                      <string>Window size</string>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
+                    <property name="buddy">
+                      <cstring>spinBoxWindowLength</cstring>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QCheckBox" name="checkBoxRdcAutosave">
-                    <property name="toolTip">
-                      <string>Automatically save all changes.</string>
+                  <widget class="QSpinBox" name="spinBoxWindowLength">
+                    <property name="keyboardTracking">
+                      <bool>false</bool>
+                    </property>
+                    <property name="minimum">
+                      <number>1</number>
+                    </property>
+                    <property name="singleStep">
+                      <number>2</number>
+                    </property>
+                    <property name="value">
+                      <number>9</number>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_17">
+                    <property name="text">
+                      <string>Poly. order</string>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
+                    <property name="buddy">
+                      <cstring>spinBoxPolyOrder</cstring>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QSpinBox" name="spinBoxPolyOrder">
+                    <property name="keyboardTracking">
+                      <bool>false</bool>
+                    </property>
+                    <property name="minimum">
+                      <number>1</number>
+                    </property>
+                    <property name="singleStep">
+                      <number>1</number>
+                    </property>
+                    <property name="value">
+                      <number>3</number>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <widget class="SGFPlotWidget" name="plot_SGF" native="true"/>
+            </item>
+          </layout>
+        </item>
+        <item>
+          <layout class="QVBoxLayout" name="verticalLayout_2" stretch="0,2,0,0,2,0,2,0,0,0">
+            <property name="sizeConstraint">
+              <enum>QLayout::SetMinimumSize</enum>
+            </property>
+            <item>
+              <layout class="QGridLayout" name="gridLayout_6" columnstretch="0,1,4,1">
+                <item row="1" column="2">
+                  <widget class="QSlider" name="horizontalSliderMax">
+                    <property name="value">
+                      <number>99</number>
+                    </property>
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="1" rowspan="2">
+                  <widget class="LineDouble" name="lineEditMinwn">
+                    <property name="text">
+                      <string>800</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="2">
+                  <widget class="QSlider" name="horizontalSliderMin">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="3" rowspan="2">
+                  <widget class="LineDouble" name="lineEditMaxwn">
+                    <property name="text">
+                      <string>4000</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="0" rowspan="2">
+                  <widget class="QCheckBox" name="checkBoxSR">
+                    <property name="font">
+                      <font>
+                        <weight>75</weight>
+                        <bold>true</bold>
+                      </font>
                     </property>
                     <property name="layoutDirection">
                       <enum>Qt::LeftToRight</enum>
                     </property>
                     <property name="text">
-                      <string>Auto-save all changes</string>
+                      <string>Spectral region</string>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <widget class="SRPlotWidget" name="plot_SR" native="true">
+                <property name="mouseTracking">
+                  <bool>true</bool>
+                </property>
+              </widget>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_21" stretch="0,2">
+                <item>
+                  <widget class="QCheckBox" name="checkBoxBC">
+                    <property name="text">
+                      <string>Baseline correction</string>
                     </property>
                   </widget>
                 </item>
+                <item>
+                  <widget class="QComboBox" name="comboBoxBaseline">
+                    <property name="layoutDirection">
+                      <enum>Qt::LeftToRight</enum>
+                    </property>
+                    <property name="currentIndex">
+                      <number>2</number>
+                    </property>
+                    <item>
+                      <property name="text">
+                        <string>Rubberband</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Concave rubberband</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>AsLS</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>arPLS</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Assym. trunc. quad.</string>
+                      </property>
+                    </item>
+                  </widget>
+                </item>
               </layout>
             </item>
             <item>
-              <widget class="QTabWidget" name="tabWidget">
+              <widget class="QStackedWidget" name="bcParams">
                 <property name="currentIndex">
                   <number>2</number>
                 </property>
-                <widget class="QWidget" name="tab">
-                  <attribute name="title">
-                    <string>Region of interest</string>
-                  </attribute>
-                  <layout class="QVBoxLayout" name="verticalLayout_4" stretch="0,0,1">
+                <widget class="QWidget" name="page_0">
+                  <layout class="QHBoxLayout" name="horizontalLayout_19">
                     <property name="leftMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="topMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="rightMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_9">
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRoiClear">
-                            <property name="text">
-                              <string>Clear all</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRoiAdd">
-                            <property name="text">
-                              <string>&amp;Add area</string>
-                            </property>
-                            <property name="shortcut">
-                              <string>A</string>
-                            </property>
-                            <property name="checkable">
-                              <bool>true</bool>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRoiRemove">
-                            <property name="text">
-                              <string>&amp;Remove area</string>
-                            </property>
-                            <property name="shortcut">
-                              <string>R</string>
-                            </property>
-                            <property name="checkable">
-                              <bool>true</bool>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRoiErase">
-                            <property name="text">
-                              <string>&amp;Erase last point</string>
-                            </property>
-                            <property name="shortcut">
-                              <string>E</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRoiInvert">
-                            <property name="text">
-                              <string>In&amp;vert</string>
-                            </property>
-                            <property name="shortcut">
-                              <string>V</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QLabel" name="label">
+                        <property name="text">
+                          <string/>
+                        </property>
+                      </widget>
                     </item>
+                  </layout>
+                </widget>
+                <widget class="QWidget" name="page_1">
+                  <layout class="QHBoxLayout" name="horizontalLayout" stretch="1,1,2">
+                    <property name="leftMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="topMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="rightMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="bottomMargin">
+                      <number>0</number>
+                    </property>
                     <item>
-                      <widget class="QLabel" name="labelRoiSelected">
+                      <widget class="QLabel" name="labelItersBC">
                         <property name="text">
-                          <string>Selected: XXXX / XXXX</string>
+                          <string>Iterations</string>
+                        </property>
+                        <property name="buddy">
+                          <cstring>spinBoxItersBC</cstring>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QSpinBox" name="spinBoxItersBC">
+                        <property name="keyboardTracking">
+                          <bool>false</bool>
+                        </property>
+                        <property name="minimum">
+                          <number>1</number>
+                        </property>
+                        <property name="maximum">
+                          <number>100</number>
                         </property>
-                        <property name="alignment">
-                          <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                        <property name="value">
+                          <number>10</number>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="RoiPlotWidget" name="plot_roi" native="true"/>
+                      <widget class="QLabel" name="label_3">
+                        <property name="text">
+                          <string/>
+                        </property>
+                      </widget>
                     </item>
                   </layout>
                 </widget>
-                <widget class="QWidget" name="tab_2">
-                  <attribute name="title">
-                    <string>Decomposition</string>
-                  </attribute>
-                  <layout class="QVBoxLayout" name="verticalLayout_3" stretch="0,0,0,0,0,1,0">
+                <widget class="QWidget" name="page_2">
+                  <layout class="QHBoxLayout" name="horizontalLayout_26">
                     <property name="leftMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="topMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="rightMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout" stretch="0,2,1,0,1,0,1,0">
-                        <item>
-                          <widget class="QLabel" name="label_7">
-                            <property name="text">
-                              <string>Algorithm</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxAlgorithm">
-                            <item>
-                              <property name="text">
-                                <string>MCR-ALS Accelerated</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>MCR-ALS</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_8">
-                            <property name="text">
-                              <string>Derivative</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxDerivative">
-                            <item>
-                              <property name="text">
-                                <string>None</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>1st derivative</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>2nd derivative</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_11">
-                            <property name="text">
-                              <string>SG polyorder</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxDerivativePoly">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="minimumSize">
-                              <size>
-                                <width>45</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>1</number>
-                            </property>
-                            <property name="maximum">
-                              <number>5</number>
-                            </property>
-                            <property name="singleStep">
-                              <number>2</number>
-                            </property>
-                            <property name="value">
-                              <number>3</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_9">
-                            <property name="text">
-                              <string>SG window</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxDerivativeWindow">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="minimumSize">
-                              <size>
-                                <width>45</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>5</number>
-                            </property>
-                            <property name="singleStep">
-                              <number>2</number>
-                            </property>
-                            <property name="value">
-                              <number>11</number>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
-                    </item>
-                    <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_3">
-                        <item>
-                          <widget class="QLabel" name="label_3">
-                            <property name="text">
-                              <string>Components</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxComponents">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="minimumSize">
-                              <size>
-                                <width>45</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>1</number>
-                            </property>
-                            <property name="maximum">
-                              <number>40</number>
-                            </property>
-                            <property name="value">
-                              <number>5</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_4">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>Starting point</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxStartingPoint">
-                            <item>
-                              <property name="text">
-                                <string>Spectra</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Contributions</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_6">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="toolTip">
-                              <string>The SIMPLISMA algorithm attempts to chooses maximally orthogonal components. The SIMPLISMA noise parameter is set to 0.1 here.
-
-K-means clustering performs a clustering on the unscaled data and chooses representative cluster centers as starting points.</string>
-                            </property>
-                            <property name="text">
-                              <string>Initial values</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxInitialValues">
-                            <item>
-                              <property name="text">
-                                <string>Simplisma</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>K means clusters</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Load from file</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_25">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="toolTip">
-                              <string>How to treat the region of interest. If required, at least one spectrum must be selected in every image.</string>
-                            </property>
-                            <property name="text">
-                              <string>Use ROI</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxUseRoi">
-                            <property name="currentIndex">
-                              <number>1</number>
-                            </property>
-                            <item>
-                              <property name="text">
-                                <string>Ignored</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>If defined</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Required</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QLabel" name="labelLambda">
+                        <property name="text">
+                          <string>&amp;lambda;</string>
+                        </property>
+                        <property name="textFormat">
+                          <enum>Qt::RichText</enum>
+                        </property>
+                        <property name="buddy">
+                          <cstring>horizontalSliderLambda</cstring>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_2">
-                        <item>
-                          <widget class="QCheckBox" name="checkBoxContrast">
-                            <property name="toolTip">
-                              <string>Improve contrast by angle-constrained ALS; see Windig and Keenan, Applied Spectroscopy 65: 349 (2011).</string>
-                            </property>
-                            <property name="text">
-                              <string>Enhance contrast of</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxContrast">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <item>
-                              <property name="text">
-                                <string>spectra</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>contributions</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_17">
-                            <property name="text">
-                              <string>by</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSlider" name="horizontalSliderContrast">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="maximum">
-                              <number>50</number>
-                            </property>
-                            <property name="pageStep">
-                              <number>5</number>
-                            </property>
-                            <property name="orientation">
-                              <enum>Qt::Horizontal</enum>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="LineDouble" name="lineEditContrast">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>0</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_10">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>Max iterations</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxIterations">
-                            <property name="minimumSize">
-                              <size>
-                                <width>50</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>1</number>
-                            </property>
-                            <property name="maximum">
-                              <number>9999</number>
-                            </property>
-                            <property name="value">
-                              <number>500</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_13">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="toolTip">
-                              <string>Stop at this relative decrease in error</string>
-                            </property>
-                            <property name="text">
-                              <string>Stopping improv.</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="LineDouble" name="lineEditTolerance">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>0.01</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_14">
-                            <property name="text">
-                              <string>%</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QSlider" name="horizontalSliderLambda">
+                        <property name="enabled">
+                          <bool>true</bool>
+                        </property>
+                        <property name="maximum">
+                          <number>80</number>
+                        </property>
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_4" stretch="2,0,1,5,1,1,0">
-                        <item>
-                          <widget class="QPushButton" name="pushButtonStart">
-                            <property name="text">
-                              <string>Run decomposition</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonStop">
-                            <property name="text">
-                              <string>Stop</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_15">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>Iteration</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QProgressBar" name="progressBarIteration">
-                            <property name="value">
-                              <number>0</number>
-                            </property>
-                            <property name="format">
-                              <string>idle</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_16">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="toolTip">
-                              <string>Mean square error relative to naively estimating data as the mean of all spectra.</string>
-                            </property>
-                            <property name="text">
-                              <string>Rel. err.</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLineEdit" name="lineEditRelError">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="minimumSize">
-                              <size>
-                                <width>40</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="readOnly">
-                              <bool>true</bool>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_12">
-                            <property name="text">
-                              <string>%</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="LineDouble" name="lineEditLambda">
+                        <property name="text">
+                          <string>1000</string>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_11" stretch="0,6,0">
-                        <item>
-                          <widget class="QLabel" name="label_2">
-                            <property name="text">
-                              <string>Plot mode</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxPlotMode">
-                            <property name="currentIndex">
-                              <number>-1</number>
-                            </property>
-                            <property name="maxVisibleItems">
-                              <number>16</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonSettingsInfo">
-                            <property name="text">
-                              <string>Show settings used</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QLabel" name="labelP">
+                        <property name="text">
+                          <string>p</string>
+                        </property>
+                        <property name="buddy">
+                          <cstring>horizontalSliderP</cstring>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <widget class="DecompositionPlotWidget" name="plot_decomp" native="true">
-                        <property name="minimumSize">
-                          <size>
-                            <width>50</width>
-                            <height>50</height>
-                          </size>
+                      <widget class="QSlider" name="horizontalSliderP">
+                        <property name="enabled">
+                          <bool>true</bool>
+                        </property>
+                        <property name="maximum">
+                          <number>50</number>
+                        </property>
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_13">
-                        <item>
-                          <widget class="QProgressBar" name="progressBarRun">
-                            <property name="value">
-                              <number>0</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonRun">
-                            <property name="toolTip">
-                              <string>Run decomposition with the current setting on all data files</string>
-                            </property>
-                            <property name="text">
-                              <string>Run batch</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QToolButton" name="pushButtonRunStop">
-                            <property name="enabled">
-                              <bool>false</bool>
-                            </property>
-                            <property name="text">
-                              <string>Stop</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="LineDouble" name="lineEditP">
+                        <property name="text">
+                          <string>0.01</string>
+                        </property>
+                      </widget>
                     </item>
                   </layout>
                 </widget>
-                <widget class="QWidget" name="tab_3">
-                  <attribute name="title">
-                    <string>Clustering</string>
-                  </attribute>
-                  <layout class="QVBoxLayout" name="verticalLayout_5" stretch="0,0,0,0,0,1">
+                <widget class="QWidget" name="page_3">
+                  <layout class="QHBoxLayout" name="horizontalLayout_22" stretch="0,1,1,2">
                     <property name="leftMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="topMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="rightMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>6</number>
+                      <number>0</number>
                     </property>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_21" stretch="0,1,0,0">
-                        <item>
-                          <widget class="QLabel" name="label_34">
-                            <property name="text">
-                              <string>Input data</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxClusterInput">
-                            <property name="currentIndex">
-                              <number>2</number>
-                            </property>
-                            <item>
-                              <property name="text">
-                                <string>Raw data (ROI)</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Raw data (all)</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Decomposition concentrations</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_5">
-                            <property name="text">
-                              <string>Feature scaling</string>
-                            </property>
-                            <property name="alignment">
-                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxClusterNormalization">
-                            <item>
-                              <property name="text">
-                                <string>As-is</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Unit mean (divisive)</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Zero mean (subtractive)</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Zero mean, unit variance</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QLabel" name="labelLambdaArpls">
+                        <property name="text">
+                          <string>&amp;lambda;</string>
+                        </property>
+                        <property name="textFormat">
+                          <enum>Qt::RichText</enum>
+                        </property>
+                        <property name="buddy">
+                          <cstring>horizontalSliderLambdaArpls</cstring>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_20" stretch="0,1,0,0,0,0,1">
-                        <item>
-                          <widget class="QLabel" name="label_26">
-                            <property name="text">
-                              <string>Method</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxClusterMethod">
-                            <item>
-                              <property name="text">
-                                <string>K-means</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>K-Means (minibatch)</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>Strongest component</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_28">
-                            <property name="text">
-                              <string>Clusters</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxClusterClusters">
-                            <property name="minimumSize">
-                              <size>
-                                <width>50</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>2</number>
-                            </property>
-                            <property name="value">
-                              <number>5</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QLabel" name="label_29">
-                            <property name="text">
-                              <string>Best of</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QSpinBox" name="spinBoxClusterRestarts">
-                            <property name="minimumSize">
-                              <size>
-                                <width>45</width>
-                                <height>0</height>
-                              </size>
-                            </property>
-                            <property name="minimum">
-                              <number>1</number>
-                            </property>
-                            <property name="maximum">
-                              <number>10000</number>
-                            </property>
-                            <property name="value">
-                              <number>10</number>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QPushButton" name="pushButtonCluster">
-                            <property name="text">
-                              <string>Cluster</string>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QSlider" name="horizontalSliderLambdaArpls">
+                        <property name="enabled">
+                          <bool>true</bool>
+                        </property>
+                        <property name="maximum">
+                          <number>80</number>
+                        </property>
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_18"/>
+                      <widget class="LineDouble" name="lineEditLambdaArpls">
+                        <property name="text">
+                          <string>1000</string>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_14">
-                        <item>
-                          <layout class="QVBoxLayout" name="verticalLayout_6">
-                            <item>
-                              <widget class="QLabel" name="label_18">
-                                <property name="text">
-                                  <string>Input data</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QListWidget" name="listWidgetClusterInputs">
-                                <property name="enabled">
-                                  <bool>false</bool>
-                                </property>
-                                <property name="selectionMode">
-                                  <enum>QAbstractItemView::MultiSelection</enum>
-                                </property>
-                              </widget>
-                            </item>
-                          </layout>
-                        </item>
-                        <item>
-                          <layout class="QVBoxLayout" name="verticalLayout_7">
-                            <item>
-                              <layout class="QHBoxLayout" name="horizontalLayout_19">
-                                <item>
-                                  <widget class="QLabel" name="label_27">
-                                    <property name="text">
-                                      <string>Annotations</string>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item>
-                                  <widget class="QToolButton" name="toolButtonAnnotationPlus">
-                                    <property name="font">
-                                      <font>
-                                        <weight>75</weight>
-                                        <bold>true</bold>
-                                      </font>
-                                    </property>
-                                    <property name="text">
-                                      <string>+</string>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item>
-                                  <widget class="QToolButton" name="toolButtonAnnotationMinus">
-                                    <property name="text">
-                                      <string/>
-                                    </property>
-                                    <property name="icon">
-                                      <iconset theme="list-add.png">
-                                        <normaloff>../../../../.designer/backup</normaloff>
-                                        ../../../../.designer/backup
-                                      </iconset>
-                                    </property>
-                                  </widget>
-                                </item>
-                              </layout>
-                            </item>
-                            <item>
-                              <widget class="QListWidget" name="listWidgetClusterAnnotations"/>
-                            </item>
-                          </layout>
-                        </item>
-                        <item>
-                          <layout class="QVBoxLayout" name="verticalLayout_8">
-                            <item>
-                              <widget class="QLabel" name="label_31">
-                                <property name="text">
-                                  <string>Assigned clusters</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QListWidget" name="listWidgetClusterUsed">
-                                <property name="enabled">
-                                  <bool>false</bool>
-                                </property>
-                                <property name="dragDropMode">
-                                  <enum>QAbstractItemView::DragDrop</enum>
-                                </property>
-                                <property name="defaultDropAction">
-                                  <enum>Qt::MoveAction</enum>
-                                </property>
-                                <property name="selectionMode">
-                                  <enum>QAbstractItemView::NoSelection</enum>
-                                </property>
-                              </widget>
-                            </item>
-                          </layout>
-                        </item>
-                        <item>
-                          <layout class="QVBoxLayout" name="verticalLayout_9">
-                            <item>
-                              <widget class="QLabel" name="label_32">
-                                <property name="text">
-                                  <string>Unassigned clusters</string>
-                                </property>
-                              </widget>
-                            </item>
-                            <item>
-                              <widget class="QListWidget" name="listWidgetClusterUnused">
-                                <property name="dragDropMode">
-                                  <enum>QAbstractItemView::DragDrop</enum>
-                                </property>
-                                <property name="defaultDropAction">
-                                  <enum>Qt::MoveAction</enum>
-                                </property>
-                                <property name="selectionMode">
-                                  <enum>QAbstractItemView::NoSelection</enum>
-                                </property>
-                              </widget>
-                            </item>
-                          </layout>
-                        </item>
-                      </layout>
-                    </item>
-                    <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_16" stretch="0,1,1,1">
-                        <item>
-                          <widget class="QLabel" name="label">
-                            <property name="text">
-                              <string>Colors</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="comboBoxClusterCmap">
-                            <item>
-                              <property name="text">
-                                <string>tab10</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>tab20</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>rainbow</string>
-                              </property>
-                            </item>
-                            <item>
-                              <property name="text">
-                                <string>terrain</string>
-                              </property>
-                            </item>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QCheckBox" name="checkBoxClusterShowAnnotations">
-                            <property name="text">
-                              <string>Show annotations</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QToolButton" name="toolButtonClusterExport">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
-                            <property name="text">
-                              <string>Export annotated spectra</string>
-                            </property>
-                            <property name="popupMode">
-                              <enum>QToolButton::InstantPopup</enum>
-                            </property>
-                            <property name="arrowType">
-                              <enum>Qt::NoArrow</enum>
-                            </property>
-                          </widget>
-                        </item>
-                      </layout>
+                      <widget class="QLabel" name="label_2">
+                        <property name="text">
+                          <string/>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+                <widget class="QWidget" name="page_4">
+                  <layout class="QHBoxLayout" name="horizontalLayout_2" stretch="1,1,1,1">
+                    <property name="leftMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="topMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="rightMargin">
+                      <number>0</number>
+                    </property>
+                    <property name="bottomMargin">
+                      <number>0</number>
+                    </property>
+                    <item>
+                      <widget class="QLabel" name="labelBCThresh">
+                        <property name="text">
+                          <string>Poly-order</string>
+                        </property>
+                        <property name="buddy">
+                          <cstring>spinBoxBCPoly</cstring>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QSpinBox" name="spinBoxBCPoly">
+                        <property name="minimum">
+                          <number>1</number>
+                        </property>
+                        <property name="maximum">
+                          <number>10</number>
+                        </property>
+                        <property name="value">
+                          <number>3</number>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QLabel" name="labelBCPoly">
+                        <property name="text">
+                          <string>Threshold</string>
+                        </property>
+                        <property name="buddy">
+                          <cstring>lineEditBCThresh</cstring>
+                        </property>
+                      </widget>
                     </item>
                     <item>
-                      <widget class="ClusterPlotWidget" name="plot_cluster" native="true"/>
+                      <widget class="LineDouble" name="lineEditBCThresh">
+                        <property name="text">
+                          <string>0.01</string>
+                        </property>
+                      </widget>
                     </item>
                   </layout>
                 </widget>
               </widget>
             </item>
+            <item>
+              <widget class="BCPlotWidget" name="plot_BC" native="true"/>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_20" stretch="0,3,1,0">
+                <item>
+                  <widget class="QCheckBox" name="checkBoxNorm">
+                    <property name="toolTip">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Rescale each spectrum so that some quantity becomes 1.&lt;/p&gt;&lt;p&gt;Mean: Mean intensity = 1&lt;br/&gt;Total area: Area under curve = 1&lt;br/&gt;Wavenumber: Intensity at specified wavenumber = 1&lt;br/&gt;Maximum: The maximum intensity of the spectrum = 1&lt;br/&gt;Vector: Euclidean norm = 1&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
+                    <property name="text">
+                      <string>Normalization</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QComboBox" name="comboBoxNormMethod">
+                    <item>
+                      <property name="text">
+                        <string>Mean</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Total area</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Wavenumber</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Maximum</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Vector</string>
+                      </property>
+                    </item>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="LineDouble" name="lineEditNormWavenum">
+                    <property name="text">
+                      <string>1655</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_18">
+                    <property name="text">
+                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;cm&lt;span style=&quot; vertical-align:super;&quot;&gt;-1&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <widget class="NormPlotWidget" name="plot_norm" native="true"/>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_13">
+                <item>
+                  <widget class="QPushButton" name="pushButtonSaveParameters">
+                    <property name="text">
+                      <string>Save parameters</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QPushButton" name="pushButtonLoadParameters">
+                    <property name="text">
+                      <string>Load parameters</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QPushButton" name="pushButtonRun">
+                    <property name="text">
+                      <string>Run batch</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QToolButton" name="pushButtonRunStop">
+                    <property name="enabled">
+                      <bool>false</bool>
+                    </property>
+                    <property name="text">
+                      <string>Stop</string>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="horizontalLayout_28" stretch="1,2,1,2">
+                <item>
+                  <widget class="QLabel" name="label_13">
+                    <property name="text">
+                      <string>Save suffix</string>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLineEdit" name="lineEditSaveExt">
+                    <property name="toolTip">
+                      <string>Extension added before .mat in output files.</string>
+                    </property>
+                    <property name="text">
+                      <string/>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QLabel" name="label_8">
+                    <property name="text">
+                      <string>Save format</string>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QComboBox" name="comboBoxSaveFormat">
+                    <item>
+                      <property name="text">
+                        <string>AB.mat</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Quasar.mat</string>
+                      </property>
+                    </item>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <widget class="QProgressBar" name="progressBarRun">
+                <property name="value">
+                  <number>0</number>
+                </property>
+              </widget>
+            </item>
           </layout>
         </item>
       </layout>
     </widget>
   </widget>
   <customwidgets>
     <customwidget>
@@ -1218,40 +1190,91 @@
     <customwidget>
       <class>FileLoaderWidget</class>
       <extends>QWidget</extends>
       <header location="global">octavvs/ui/fileloader.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>DecompositionPlotWidget</class>
+      <class>ImageVisualizerWidget</class>
+      <extends>QWidget</extends>
+      <header location="global">octavvs/ui/imagevisualizer.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>NormPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/decomp/plotwidget.h</header>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
       <container>1</container>
+      <slots>
+        <signal>clicked()</signal>
+        <slot>popOut()</slot>
+      </slots>
     </customwidget>
     <customwidget>
-      <class>ImageVisualizerWidget</class>
+      <class>BCPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/ui/imagevisualizer.h</header>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>SCPlotWidget</class>
+      <extends>QWidget</extends>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>ACPlotWidget</class>
+      <extends>QWidget</extends>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <container>1</container>
+    </customwidget>
+    <customwidget>
+      <class>SGFPlotWidget</class>
+      <extends>QWidget</extends>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>RoiPlotWidget</class>
+      <class>SRPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/decomp/plotwidget.h</header>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>ClusterPlotWidget</class>
+      <class>MCPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/decomp/plotwidget.h</header>
+      <header location="global">octavvs/prep/dataplotwidget.h</header>
       <container>1</container>
     </customwidget>
   </customwidgets>
   <tabstops>
-    <tabstop>comboBoxClusterMethod</tabstop>
+    <tabstop>checkBoxAC</tabstop>
+    <tabstop>checkBoxSpline</tabstop>
+    <tabstop>checkBoxLocalPeak</tabstop>
+    <tabstop>checkBoxSmoothCorrected</tabstop>
+    <tabstop>checkBoxSC</tabstop>
+    <tabstop>pushButtonSCRefresh</tabstop>
+    <tabstop>pushButtonSCStop</tabstop>
+    <tabstop>comboBoxReference</tabstop>
+    <tabstop>spinBoxNIteration</tabstop>
+    <tabstop>checkBoxClusters</tabstop>
+    <tabstop>spinBoxNclusScat</tabstop>
+    <tabstop>checkBoxStabilize</tabstop>
+    <tabstop>pushButtonSCAdvanced</tabstop>
+    <tabstop>spinBoxWindowLength</tabstop>
+    <tabstop>spinBoxPolyOrder</tabstop>
+    <tabstop>lineEditMinwn</tabstop>
+    <tabstop>horizontalSliderMin</tabstop>
+    <tabstop>horizontalSliderMax</tabstop>
+    <tabstop>lineEditMaxwn</tabstop>
+    <tabstop>comboBoxBaseline</tabstop>
+    <tabstop>comboBoxNormMethod</tabstop>
+    <tabstop>lineEditNormWavenum</tabstop>
+    <tabstop>pushButtonSaveParameters</tabstop>
+    <tabstop>pushButtonLoadParameters</tabstop>
     <tabstop>pushButtonRun</tabstop>
     <tabstop>pushButtonRunStop</tabstop>
   </tabstops>
   <resources/>
   <connections/>
   <designerdata>
     <property name="gridDeltaX">
```

### Comparing `octavvs-0.1.8/octavvs/decomp/decompworker.py` & `octavvs-0.1.9/octavvs/decomp/decompworker.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,21 +84,26 @@
             nonneg[int(c_first)] = False
 
         base_error = np.linalg.norm(y - y.mean(0))**2
         if c_first:
             y = y.T
 
         if params.dcInitialValues == 'simplisma':
-            simplisma_noise = 0.1
+            # simplisma_noise = 0.1
             initst = decomposition.simplisma(
-                y.T, params.dcComponents, simplisma_noise)[0]
+                y.T, params.dcComponents, params.dcInitialValuesNoise)[0]
         elif params.dcInitialValues == 'kmeans':
             km = sklearn.cluster.MiniBatchKMeans(
                 n_clusters=params.dcComponents).fit(y)
             initst = km.cluster_centers_
+        elif params.dcInitialValues == 'clustersubtract':
+            initst = decomposition.clustersubtract(
+                y, components=params.dcComponents,
+                skewness=params.dcInitialValuesSkew,
+                power=params.dcInitialValuesPower)
         else:
             raise ValueError('Unknown params.dcInitialValues')
 
         if c_first and params.dcDerivative:
             # If concentrations-first is combined with derivatives,
             # the initial concentrations need to be made positive.
             initst = np.abs(initst)
```

### Comparing `octavvs-0.1.8/octavvs/decomp/plotwidget.py` & `octavvs-0.1.9/octavvs/decomp/plotwidget.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/decomp/settings_table.ui` & `octavvs-0.1.9/octavvs/decomp/settings_table.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/decomposition.py` & `octavvs-0.1.9/octavvs/decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         self.pushButtonRunStop.clicked.connect(self.stopDC)
         self.pushButtonSettingsInfo.clicked.connect(self.dcSettingsShow)
         self.dialogSettingsTable = DialogSettingsTable()
         self.dialogSettingsTable.buttonBox.clicked.connect(
             self.dcSettingsClicked)
         self.comboBoxInitialValues.currentIndexChanged.connect(
             self.dcInitialValuesChanged)
+        self.lineEditInitSkew.setFormat('%g')
+        self.lineEditInitSkew.setRange(1, 1000)
+        self.lineEditInitNoise.setFormat('%g')
+        self.lineEditInitNoise.setRange(.001, 1)
         self.comboBoxDerivative.currentIndexChanged.connect(
             self.dcDerivativeChanged)
         self.checkBoxContrast.toggled.connect(self.dcContrastChanged)
         self.lineEditContrast.setFormat("%g")
         self.lineEditContrast.setRange(0, .1)
         self.lineEditContrast.editingFinished.connect(self.dcContrastEdit)
         self.horizontalSliderContrast.valueChanged.connect(
@@ -485,34 +489,25 @@
             self.plot_decomp.set_concentrations(concentrations)
             self.plot_decomp.set_spectra(spectra)
         else:
             # self.data.add_decomposition_data(0, spectra, None)
             self.plot_decomp.set_initial_spectra(spectra)
         self.plot_decomp.set_errors(errors)
 
-    # def clusterDC(self):
-    #     data = self.plot_decomp.get_concentrations().T
-    #     data = data / data.mean(axis=0)
-    #     kmeans = sklearn.cluster.MiniBatchKMeans(
-    #         self.spinBoxClusters.value())
-    #     labels = kmeans.fit_predict(data)
-    #     self.plot_decomp.add_clustering('K-means', labels)
-    #     self.comboBoxPlotMode.setCurrentText('K-means')
-    #     self.plot_decomp.draw_idle()
-
     # def dcLoad(self, auto=False):
     #     self.genericLoad(auto, what='decomposition',
     #                      description='decomposition data')
 
     # def dcSave(self, auto=False):
     #     self.genericSave(auto, what='decomposition',
     #                      description='decomposition data')
 
     def dcInitialValuesChanged(self):
-        pass
+        self.stackedWidgetInit.setCurrentIndex(
+            self.comboBoxInitialValues.currentIndex())
 
     def dcDerivativeChanged(self):
         en = self.comboBoxDerivative.currentIndex() > 0
         self.spinBoxDerivativePoly.setEnabled(en)
         self.spinBoxDerivativeWindow.setEnabled(en)
 
     def dcContrastChanged(self):
@@ -819,15 +814,15 @@
                 self.showDetailedErrorMessage(
                         "Error saving settings to "+filename+": "+repr(e),
                         traceback.format_exc())
 
 
     # Parameter handling
     useRoiNames = ['ignore', 'ifdef', 'require']
-    dcInitialValuesNames = ['simplisma', 'kmeans']
+    dcInitialValuesNames = ['simplisma', 'kmeans', 'clustersubtract']
     dcAlgorithmNames = ['mcr-als-anderson', 'mcr-als']
     caInputNames = ['raw-roi', 'raw', 'decomposition']
     caMethodNames = ['kmeans', 'mbkmeans', 'strongest']
     caNormalizationNames = ['none', 'mean1', 'mean0', 'mean0var1']
     # caMethodNames = ['kmeans', 'meanshift', 'spectral']
 
     # Loading and saving parameters
@@ -846,14 +841,17 @@
         p.dcDerivative = self.comboBoxDerivative.currentIndex()
         p.dcDerivativeWindow = self.spinBoxDerivativeWindow.value()
         p.dcDerivativePoly = self.spinBoxDerivativePoly.value()
         p.dcComponents = self.spinBoxComponents.value()
         p.dcStartingPoint = self.comboBoxStartingPoint.currentIndex()
         p.dcInitialValues = self.dcInitialValuesNames[
             self.comboBoxInitialValues.currentIndex()]
+        p.dcInitialValuesSkew = self.lineEditInitSkew.value()
+        p.dcInitialValuesPower = self.spinBoxInitPower.value()
+        p.dcInitialValuesNoise = self.lineEditInitNoise.value()
         p.dcRoi = self.useRoiNames[self.comboBoxUseRoi.currentIndex()]
         p.dcContrast = self.checkBoxContrast.isChecked()
         p.dcContrastConcentrations = self.comboBoxContrast.currentIndex()
         p.dcContrastWeight = self.lineEditContrast.value()
         p.dcIterations = self.spinBoxIterations.value()
         p.dcTolerance = self.lineEditTolerance.value()
 
@@ -901,14 +899,17 @@
         self.comboBoxDerivative.setCurrentIndex(p.dcDerivative)
         self.spinBoxDerivativeWindow.setValue(p.dcDerivativeWindow)
         self.spinBoxDerivativePoly.setValue(p.dcDerivativePoly)
         self.spinBoxComponents.setValue(p.dcComponents)
         self.comboBoxStartingPoint.setCurrentIndex(p.dcStartingPoint)
         self.comboBoxInitialValues.setCurrentIndex(
             self.dcInitialValuesNames.index(p.dcInitialValues))
+        self.lineEditInitSkew.setValue(p.dcInitialValuesSkew)
+        self.spinBoxInitPower.setValue(p.dcInitialValuesPower)
+        self.lineEditInitNoise.setValue(p.dcInitialValuesNoise)
         self.comboBoxUseRoi.setCurrentIndex(self.useRoiNames.index(p.dcRoi))
         self.checkBoxContrast.setChecked(p.dcContrast)
         self.comboBoxContrast.setCurrentIndex(p.dcContrastConcentrations)
         self.lineEditContrast.setValue(p.dcContrastWeight)
         self.spinBoxIterations.setValue(p.dcIterations)
         self.lineEditTolerance.setValue(p.dcTolerance)
```

### Comparing `octavvs-0.1.8/octavvs/icons_src_rc.py` & `octavvs-0.1.9/octavvs/icons_src_rc.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/io/decompositiondata.py` & `octavvs-0.1.9/octavvs/io/decompositiondata.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/io/opusreader.py` & `octavvs-0.1.9/octavvs/io/opusreader.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/io/parameters.py` & `octavvs-0.1.9/octavvs/io/parameters.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/io/ptirreader.py` & `octavvs-0.1.9/octavvs/io/ptirreader.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/io/spectraldata.py` & `octavvs-0.1.9/octavvs/io/spectraldata.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/launcher.py` & `octavvs-0.1.9/octavvs/launcher.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/make_icons.py` & `octavvs-0.1.9/octavvs/make_icons.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/about.ui` & `octavvs-0.1.9/octavvs/mcr/about.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/clustering_ui.ui` & `octavvs-0.1.9/octavvs/mcr/clustering_ui.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/ftir_function.py` & `octavvs-0.1.9/octavvs/mcr/ftir_function.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/mcr_final_loc.ui` & `octavvs-0.1.9/octavvs/mcr/mcr_final_loc.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/mcr_roi_sub.ui` & `octavvs-0.1.9/octavvs/mcr/mcr_roi_sub.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/mpl.py` & `octavvs-0.1.9/octavvs/mcr/mpl.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr/table_ui.ui` & `octavvs-0.1.9/octavvs/mcr/table_ui.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/mcr_als.py` & `octavvs-0.1.9/octavvs/mcr_als.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/create_reference.ui` & `octavvs-0.1.9/octavvs/prep/create_reference.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/dataplotwidget.py` & `octavvs-0.1.9/octavvs/prep/dataplotwidget.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/octavvs_prep.icns` & `octavvs-0.1.9/octavvs/prep/octavvs_prep.icns`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/octavvs_prep.ico` & `octavvs-0.1.9/octavvs/prep/octavvs_prep.ico`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/octavvs_prep_48.ico` & `octavvs-0.1.9/octavvs/prep/octavvs_prep_48.ico`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/preprocessing_ui.ui` & `octavvs-0.1.9/octavvs/decomp/decomposition.ui`

 * *Files 16% similar despite different names*

#### Comparing `octavvs-0.1.8/octavvs/prep/preprocessing_ui.ui` & `octavvs-0.1.9/octavvs/decomp/decomposition.ui`

```diff
@@ -2,31 +2,31 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1423</width>
-        <height>955</height>
+        <width>1220</width>
+        <height>785</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>OCTAVVS Preprocessing</string>
+      <string>OCTAVVS Decomposition</string>
     </property>
     <property name="styleSheet">
       <string notr="true">QSplitter::handle:horizontal {
 border: 1px solid #ccc;
 border-right-color: #bbb;
 border-bottom-color: #bbb;
 margin: 5px;
 }</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <layout class="QHBoxLayout" name="horizontalLayout_17" stretch="1,1,1">
+      <layout class="QHBoxLayout" name="horizontalLayout_17" stretch="3,5">
         <property name="leftMargin">
           <number>6</number>
         </property>
         <property name="topMargin">
           <number>6</number>
         </property>
         <property name="rightMargin">
@@ -52,1128 +52,1253 @@
             </item>
             <item>
               <widget class="ImageVisualizerWidget" name="imageVisualizer" native="true"/>
             </item>
           </layout>
         </item>
         <item>
-          <layout class="QVBoxLayout" name="verticalLayout_4" stretch="0,1,0,0,1,0,0,0,1,0,1">
-            <property name="sizeConstraint">
-              <enum>QLayout::SetMinimumSize</enum>
-            </property>
+          <layout class="QVBoxLayout" name="verticalLayout_2" stretch="0,0,0">
             <item>
-              <widget class="QWidget" name="widgetMC" native="true">
-                <layout class="QVBoxLayout" name="verticalLayout_6" stretch="0">
-                  <property name="leftMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="topMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="rightMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="bottomMargin">
-                    <number>0</number>
-                  </property>
-                  <item>
-                    <layout class="QHBoxLayout" name="horizontalLayout_16" stretch="4,2,1,2,1">
-                      <property name="topMargin">
-                        <number>0</number>
-                      </property>
-                      <item>
-                        <widget class="QCheckBox" name="checkBoxMC">
-                          <property name="font">
-                            <font>
-                              <weight>75</weight>
-                              <bold>true</bold>
-                            </font>
-                          </property>
-                          <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Clustered Resonant Mie Scattering Correction; see the article by Troein, Siregar, Op De Beeck et al for details and consult the thesis of Paul Bassan for a description of the basic algorithm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                          <property name="layoutDirection">
-                            <enum>Qt::LeftToRight</enum>
-                          </property>
-                          <property name="text">
-                            <string>mIRage correction</string>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QLabel" name="label_6">
-                          <property name="text">
-                            <string>Endpoints</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                          </property>
-                          <property name="buddy">
-                            <cstring>spinBoxMCEndpoints</cstring>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QSpinBox" name="spinBoxMCEndpoints">
-                          <property name="minimum">
-                            <number>2</number>
-                          </property>
-                          <property name="maximum">
-                            <number>40</number>
-                          </property>
-                          <property name="value">
-                            <number>6</number>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QLabel" name="label_7">
-                          <property name="text">
-                            <string>Slopefactor</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                          </property>
-                          <property name="buddy">
-                            <cstring>lineEditMCSlopefactor</cstring>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="LineDouble" name="lineEditMCSlopefactor">
-                          <property name="text">
-                            <string>.5</string>
-                          </property>
-                        </widget>
-                      </item>
-                    </layout>
-                  </item>
-                </layout>
-              </widget>
-            </item>
-            <item>
-              <widget class="MCPlotWidget" name="plot_MC" native="true"/>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_15" stretch="0,1">
+              <layout class="QHBoxLayout" name="horizontalLayout_8">
                 <item>
-                  <widget class="QCheckBox" name="checkBoxAC">
-                    <property name="font">
-                      <font>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
-                    </property>
+                  <widget class="QLabel" name="label_20">
                     <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Atmospheric correction, designed to remove spectral contributions from H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O and CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; by subtracting an atmospheric reference spectrum (times an appropriate factor) in each of two H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions and, optionally, one CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; region.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
-                    <property name="layoutDirection">
-                      <enum>Qt::LeftToRight</enum>
+                      <string>Where to save decomposition metadata (.dmd) files. 'Other directory' requires that input files have unique names.</string>
                     </property>
                     <property name="text">
-                      <string>Atmospheric correction</string>
+                      <string>Save data in</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QLabel" name="labelACInfo">
-                    <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Estimated mean magnitude of the corrections, relative to the level in the corrected regions.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
-                    <property name="text">
-                      <string/>
-                    </property>
-                    <property name="textFormat">
-                      <enum>Qt::AutoText</enum>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
+                  <widget class="QComboBox" name="comboBoxDirectory">
+                    <item>
+                      <property name="text">
+                        <string>Input directory</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Other directory</string>
+                      </property>
+                    </item>
                   </widget>
                 </item>
-              </layout>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_4" stretch="1,1,1,0,3">
                 <item>
-                  <widget class="QCheckBox" name="checkBoxSpline">
-                    <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Replace data in the CO&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt; region (2245-2445 cm&lt;span style=&quot; vertical-align:super;&quot;&gt;-1&lt;/span&gt;) with a smooth curve. Otherwise apply the same type of correction as in the H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
-                    <property name="text">
-                      <string>Spline at CO₂</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
+                  <widget class="QLineEdit" name="lineEditDirectory">
+                    <property name="enabled">
+                      <bool>false</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QCheckBox" name="checkBoxLocalPeak">
-                    <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Attempt to refine the correction in a small sliding window to account for fluctuations in H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O peak intensities.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
+                  <widget class="QPushButton" name="pushButtonDirectory">
                     <property name="text">
-                      <string>Local peak corr.</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
+                      <string>Select dir</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QCheckBox" name="checkBoxSmoothCorrected">
-                    <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Apply a weak denoising filter to the H&lt;span style=&quot; vertical-align:sub;&quot;&gt;2&lt;/span&gt;O regions of the spectrum.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
+                  <widget class="QPushButton" name="pushButtonLoadParameters">
                     <property name="text">
-                      <string>Smoothing</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
+                      <string>Load parameters</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QPushButton" name="pushButtonACLoadReference">
+                  <widget class="QPushButton" name="pushButtonSaveParameters">
                     <property name="text">
-                      <string>Load ref.</string>
+                      <string>Save parameters</string>
                     </property>
                   </widget>
                 </item>
-                <item>
-                  <widget class="QLineEdit" name="lineEditACReference"/>
-                </item>
               </layout>
             </item>
             <item>
-              <widget class="ACPlotWidget" name="plot_AC" native="true"/>
-            </item>
-            <item>
-              <widget class="QWidget" name="widgetSC" native="true">
-                <layout class="QHBoxLayout" name="layoutSC_1" stretch="4,1,0">
-                  <property name="leftMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="topMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="rightMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="bottomMargin">
-                    <number>0</number>
-                  </property>
-                  <item>
-                    <widget class="QCheckBox" name="checkBoxSC">
-                      <property name="font">
-                        <font>
-                          <weight>75</weight>
-                          <bold>true</bold>
-                        </font>
-                      </property>
-                      <property name="toolTip">
-                        <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Clustered Resonant Mie Scattering Correction; see the article by Troein, Siregar, Op De Beeck et al for details and consult the thesis of Paul Bassan for a description of the basic algorithm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                      </property>
-                      <property name="layoutDirection">
-                        <enum>Qt::LeftToRight</enum>
-                      </property>
-                      <property name="text">
-                        <string>Scattering correction (CRMieSC)</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item>
-                    <widget class="QPushButton" name="pushButtonSCRefresh">
-                      <property name="enabled">
-                        <bool>false</bool>
-                      </property>
-                      <property name="text">
-                        <string>Update</string>
-                      </property>
-                    </widget>
-                  </item>
-                  <item>
-                    <widget class="QToolButton" name="pushButtonSCStop">
-                      <property name="enabled">
-                        <bool>false</bool>
-                      </property>
-                      <property name="text">
-                        <string>Stop</string>
-                      </property>
-                    </widget>
-                  </item>
-                </layout>
-              </widget>
-            </item>
-            <item>
-              <widget class="QProgressBar" name="progressBarSC">
-                <property name="value">
-                  <number>0</number>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <widget class="QWidget" name="widgetSCOptions" native="true">
-                <layout class="QVBoxLayout" name="verticalLayout_5">
-                  <property name="leftMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="topMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="rightMargin">
-                    <number>0</number>
-                  </property>
-                  <property name="bottomMargin">
-                    <number>0</number>
-                  </property>
-                  <item>
-                    <layout class="QHBoxLayout" name="layoutSC_2" stretch="0,1,4">
-                      <item>
-                        <widget class="QLabel" name="label_36">
-                          <property name="text">
-                            <string>Reference</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                          </property>
-                          <property name="buddy">
-                            <cstring>comboBoxReference</cstring>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QComboBox" name="comboBoxReference">
-                          <property name="sizePolicy">
-                            <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
-                              <horstretch>0</horstretch>
-                              <verstretch>0</verstretch>
-                            </sizepolicy>
-                          </property>
-                          <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Reference spectrum used to initialize the RMieSC algorithm; choose a non-scattered spectrum from a sample as similar as possible to that studied.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                          <item>
-                            <property name="text">
-                              <string>Mean</string>
-                            </property>
-                          </item>
-                          <item>
-                            <property name="text">
-                              <string>Percentile</string>
-                            </property>
-                          </item>
-                          <item>
-                            <property name="text">
-                              <string>Casein</string>
-                            </property>
-                          </item>
-                          <item>
-                            <property name="text">
-                              <string>Lignin</string>
-                            </property>
-                          </item>
-                          <item>
-                            <property name="text">
-                              <string>Matrigel</string>
-                            </property>
-                          </item>
-                          <item>
-                            <property name="text">
-                              <string>Other</string>
-                            </property>
-                          </item>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QStackedWidget" name="stackedSC">
-                          <property name="currentIndex">
-                            <number>0</number>
-                          </property>
-                          <widget class="QWidget" name="page">
-                            <layout class="QHBoxLayout" name="horizontalLayout_24" stretch="2,1,3">
-                              <property name="leftMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="topMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="rightMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="bottomMargin">
-                                <number>0</number>
-                              </property>
-                              <item>
-                                <widget class="QLabel" name="label_4">
-                                  <property name="text">
-                                    <string>Percentile</string>
-                                  </property>
-                                  <property name="alignment">
-                                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                                  </property>
-                                  <property name="buddy">
-                                    <cstring>lineEditSCRefPercentile</cstring>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="LineDouble" name="lineEditSCRefPercentile"/>
-                              </item>
-                              <item>
-                                <widget class="QPushButton" name="pushButtonCreateReference">
-                                  <property name="text">
-                                    <string>Create from dataset</string>
-                                  </property>
-                                </widget>
-                              </item>
-                            </layout>
-                          </widget>
-                          <widget class="QWidget" name="page_5">
-                            <layout class="QHBoxLayout" name="horizontalLayout_25" stretch="0,0">
-                              <property name="leftMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="topMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="rightMargin">
-                                <number>0</number>
-                              </property>
-                              <property name="bottomMargin">
-                                <number>0</number>
-                              </property>
-                              <item>
-                                <widget class="QPushButton" name="pushButtonLoadOther">
-                                  <property name="toolTip">
-                                    <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Load your own reference spectrum. This should be a MATLAB matrix called 'AB' with two columns: wavenumber and intensity.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                                  </property>
-                                  <property name="text">
-                                    <string>Load other</string>
-                                  </property>
-                                </widget>
-                              </item>
-                              <item>
-                                <widget class="QLineEdit" name="lineEditReferenceName">
-                                  <property name="readOnly">
-                                    <bool>true</bool>
-                                  </property>
-                                </widget>
-                              </item>
-                            </layout>
-                          </widget>
-                        </widget>
-                      </item>
-                    </layout>
-                  </item>
-                  <item>
-                    <layout class="QHBoxLayout" name="layoutSC_3" stretch="0,1,0,1,0,1">
-                      <item>
-                        <widget class="QLabel" name="label_38">
-                          <property name="text">
-                            <string>Max iterations</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                          </property>
-                          <property name="buddy">
-                            <cstring>spinBoxNIteration</cstring>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QSpinBox" name="spinBoxNIteration">
-                          <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Iterations of the RMieSC algorithm; a value of 10-20 may be required for good convergence.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                          <property name="minimum">
-                            <number>1</number>
-                          </property>
-                          <property name="maximum">
-                            <number>999</number>
-                          </property>
-                          <property name="singleStep">
-                            <number>1</number>
-                          </property>
-                          <property name="value">
-                            <number>30</number>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QCheckBox" name="checkBoxClusters">
-                          <property name="text">
-                            <string>Clusters</string>
-                          </property>
-                          <property name="checked">
-                            <bool>true</bool>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QSpinBox" name="spinBoxNclusScat">
-                          <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;The number of clusters to divide the spectra into when computing new reference spectra. This must be set high enough that the spectra in each cluster are practically identical, in which case it will confer robustness to the correction. A value of 0 disables clustering; the spectra are then corrected individually which takes a very long time and gives less robust results.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                          <property name="minimum">
-                            <number>1</number>
-                          </property>
-                          <property name="maximum">
-                            <number>100</number>
-                          </property>
-                          <property name="singleStep">
-                            <number>1</number>
-                          </property>
-                          <property name="value">
-                            <number>30</number>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QCheckBox" name="checkBoxStabilize">
-                          <property name="toolTip">
-                            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;With this option, the scattering correction is stabilized by two means: first fittiing a common reference spectrum to the whole image before fitting with clustering, and in later iterations updating reference spectra with mixing between previous and new.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                          </property>
-                          <property name="text">
-                            <string>Stabilize</string>
-                          </property>
-                          <property name="checked">
-                            <bool>true</bool>
-                          </property>
-                        </widget>
-                      </item>
-                      <item>
-                        <widget class="QPushButton" name="pushButtonSCAdvanced">
-                          <property name="text">
-                            <string>Advanced</string>
-                          </property>
-                        </widget>
-                      </item>
-                    </layout>
-                  </item>
-                </layout>
-              </widget>
-            </item>
-            <item>
-              <widget class="SCPlotWidget" name="plot_SC" native="true"/>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_9" stretch="0,2,1,1,1">
+              <layout class="QHBoxLayout" name="horizontalLayout_10" stretch="0,0,0">
                 <item>
-                  <widget class="QCheckBox" name="checkBoxSGF">
-                    <property name="font">
-                      <font>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
-                    </property>
-                    <property name="layoutDirection">
-                      <enum>Qt::LeftToRight</enum>
+                  <widget class="QPushButton" name="pushButtonRdcLoad">
+                    <property name="toolTip">
+                      <string>Load selection from an arbitrary file</string>
                     </property>
                     <property name="text">
-                      <string>Denoising (Savitzky-Golay) filter</string>
+                      <string>Load</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QLabel" name="label_16">
+                  <widget class="QPushButton" name="pushButtonRdcSave">
                     <property name="text">
-                      <string>Window size</string>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
-                    <property name="buddy">
-                      <cstring>spinBoxWindowLength</cstring>
+                      <string>Save</string>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <widget class="QSpinBox" name="spinBoxWindowLength">
-                    <property name="keyboardTracking">
-                      <bool>false</bool>
-                    </property>
-                    <property name="minimum">
-                      <number>1</number>
-                    </property>
-                    <property name="singleStep">
-                      <number>2</number>
-                    </property>
-                    <property name="value">
-                      <number>9</number>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QLabel" name="label_17">
-                    <property name="text">
-                      <string>Poly. order</string>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
-                    <property name="buddy">
-                      <cstring>spinBoxPolyOrder</cstring>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QSpinBox" name="spinBoxPolyOrder">
-                    <property name="keyboardTracking">
-                      <bool>false</bool>
-                    </property>
-                    <property name="minimum">
-                      <number>1</number>
-                    </property>
-                    <property name="singleStep">
-                      <number>1</number>
-                    </property>
-                    <property name="value">
-                      <number>3</number>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <widget class="SGFPlotWidget" name="plot_SGF" native="true"/>
-            </item>
-          </layout>
-        </item>
-        <item>
-          <layout class="QVBoxLayout" name="verticalLayout_2" stretch="0,2,0,0,2,0,2,0,0,0">
-            <property name="sizeConstraint">
-              <enum>QLayout::SetMinimumSize</enum>
-            </property>
-            <item>
-              <layout class="QGridLayout" name="gridLayout_6" columnstretch="0,1,4,1">
-                <item row="1" column="2">
-                  <widget class="QSlider" name="horizontalSliderMax">
-                    <property name="value">
-                      <number>99</number>
-                    </property>
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="1" rowspan="2">
-                  <widget class="LineDouble" name="lineEditMinwn">
-                    <property name="text">
-                      <string>800</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="2">
-                  <widget class="QSlider" name="horizontalSliderMin">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="3" rowspan="2">
-                  <widget class="LineDouble" name="lineEditMaxwn">
-                    <property name="text">
-                      <string>4000</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="0" rowspan="2">
-                  <widget class="QCheckBox" name="checkBoxSR">
-                    <property name="font">
-                      <font>
-                        <weight>75</weight>
-                        <bold>true</bold>
-                      </font>
+                  <widget class="QCheckBox" name="checkBoxRdcAutosave">
+                    <property name="toolTip">
+                      <string>Automatically save all changes.</string>
                     </property>
                     <property name="layoutDirection">
                       <enum>Qt::LeftToRight</enum>
                     </property>
                     <property name="text">
-                      <string>Spectral region</string>
+                      <string>Auto-save all changes</string>
                     </property>
                   </widget>
                 </item>
               </layout>
             </item>
             <item>
-              <widget class="SRPlotWidget" name="plot_SR" native="true">
-                <property name="mouseTracking">
-                  <bool>true</bool>
-                </property>
-              </widget>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_21" stretch="0,2">
-                <item>
-                  <widget class="QCheckBox" name="checkBoxBC">
-                    <property name="text">
-                      <string>Baseline correction</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QComboBox" name="comboBoxBaseline">
-                    <property name="layoutDirection">
-                      <enum>Qt::LeftToRight</enum>
-                    </property>
-                    <property name="currentIndex">
-                      <number>2</number>
-                    </property>
-                    <item>
-                      <property name="text">
-                        <string>Rubberband</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>Concave rubberband</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>AsLS</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>arPLS</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>Assym. trunc. quad.</string>
-                      </property>
-                    </item>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <widget class="QStackedWidget" name="bcParams">
+              <widget class="QTabWidget" name="tabWidget">
                 <property name="currentIndex">
-                  <number>2</number>
+                  <number>1</number>
                 </property>
-                <widget class="QWidget" name="page_0">
-                  <layout class="QHBoxLayout" name="horizontalLayout_19">
+                <widget class="QWidget" name="tab">
+                  <attribute name="title">
+                    <string>Region of interest</string>
+                  </attribute>
+                  <layout class="QVBoxLayout" name="verticalLayout_4" stretch="0,0,1">
                     <property name="leftMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="topMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="rightMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <item>
-                      <widget class="QLabel" name="label">
-                        <property name="text">
-                          <string/>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_9">
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRoiClear">
+                            <property name="text">
+                              <string>Clear all</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRoiAdd">
+                            <property name="text">
+                              <string>&amp;Add area</string>
+                            </property>
+                            <property name="shortcut">
+                              <string>A</string>
+                            </property>
+                            <property name="checkable">
+                              <bool>true</bool>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRoiRemove">
+                            <property name="text">
+                              <string>&amp;Remove area</string>
+                            </property>
+                            <property name="shortcut">
+                              <string>R</string>
+                            </property>
+                            <property name="checkable">
+                              <bool>true</bool>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRoiErase">
+                            <property name="text">
+                              <string>&amp;Erase last point</string>
+                            </property>
+                            <property name="shortcut">
+                              <string>E</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRoiInvert">
+                            <property name="text">
+                              <string>In&amp;vert</string>
+                            </property>
+                            <property name="shortcut">
+                              <string>V</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
-                  </layout>
-                </widget>
-                <widget class="QWidget" name="page_1">
-                  <layout class="QHBoxLayout" name="horizontalLayout" stretch="1,1,2">
-                    <property name="leftMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="topMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="rightMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="bottomMargin">
-                      <number>0</number>
-                    </property>
                     <item>
-                      <widget class="QLabel" name="labelItersBC">
+                      <widget class="QLabel" name="labelRoiSelected">
                         <property name="text">
-                          <string>Iterations</string>
+                          <string>Selected: XXXX / XXXX</string>
                         </property>
-                        <property name="buddy">
-                          <cstring>spinBoxItersBC</cstring>
+                        <property name="alignment">
+                          <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="QSpinBox" name="spinBoxItersBC">
-                        <property name="keyboardTracking">
-                          <bool>false</bool>
-                        </property>
-                        <property name="minimum">
-                          <number>1</number>
-                        </property>
-                        <property name="maximum">
-                          <number>100</number>
-                        </property>
-                        <property name="value">
-                          <number>10</number>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="label_3">
-                        <property name="text">
-                          <string/>
-                        </property>
-                      </widget>
+                      <widget class="RoiPlotWidget" name="plot_roi" native="true"/>
                     </item>
                   </layout>
                 </widget>
-                <widget class="QWidget" name="page_2">
-                  <layout class="QHBoxLayout" name="horizontalLayout_26">
+                <widget class="QWidget" name="tab_2">
+                  <attribute name="title">
+                    <string>Decomposition</string>
+                  </attribute>
+                  <layout class="QVBoxLayout" name="verticalLayout_3" stretch="0,0,0,0,0,1,0">
                     <property name="leftMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="topMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="rightMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <item>
-                      <widget class="QLabel" name="labelLambda">
-                        <property name="text">
-                          <string>&amp;lambda;</string>
-                        </property>
-                        <property name="textFormat">
-                          <enum>Qt::RichText</enum>
-                        </property>
-                        <property name="buddy">
-                          <cstring>horizontalSliderLambda</cstring>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QSlider" name="horizontalSliderLambda">
-                        <property name="enabled">
-                          <bool>true</bool>
-                        </property>
-                        <property name="maximum">
-                          <number>80</number>
-                        </property>
-                        <property name="orientation">
-                          <enum>Qt::Horizontal</enum>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="LineDouble" name="lineEditLambda">
-                        <property name="text">
-                          <string>1000</string>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="labelP">
-                        <property name="text">
-                          <string>p</string>
-                        </property>
-                        <property name="buddy">
-                          <cstring>horizontalSliderP</cstring>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout" stretch="0,2,1,0,1,0,1,0">
+                        <item>
+                          <widget class="QLabel" name="label_7">
+                            <property name="text">
+                              <string>Algorithm</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxAlgorithm">
+                            <item>
+                              <property name="text">
+                                <string>MCR-ALS Accelerated</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>MCR-ALS</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_8">
+                            <property name="text">
+                              <string>Derivative</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxDerivative">
+                            <item>
+                              <property name="text">
+                                <string>None</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>1st derivative</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>2nd derivative</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_11">
+                            <property name="text">
+                              <string>SG polyorder</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxDerivativePoly">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>45</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>1</number>
+                            </property>
+                            <property name="maximum">
+                              <number>5</number>
+                            </property>
+                            <property name="singleStep">
+                              <number>2</number>
+                            </property>
+                            <property name="value">
+                              <number>3</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_9">
+                            <property name="text">
+                              <string>SG window</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxDerivativeWindow">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>45</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>5</number>
+                            </property>
+                            <property name="singleStep">
+                              <number>2</number>
+                            </property>
+                            <property name="value">
+                              <number>11</number>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <widget class="QSlider" name="horizontalSliderP">
-                        <property name="enabled">
-                          <bool>true</bool>
-                        </property>
-                        <property name="maximum">
-                          <number>50</number>
-                        </property>
-                        <property name="orientation">
-                          <enum>Qt::Horizontal</enum>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_3" stretch="0,0,1,1,1,1,2">
+                        <item>
+                          <widget class="QLabel" name="label_3">
+                            <property name="text">
+                              <string>Components</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxComponents">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>45</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>1</number>
+                            </property>
+                            <property name="maximum">
+                              <number>40</number>
+                            </property>
+                            <property name="value">
+                              <number>5</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_4">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="text">
+                              <string>Starting point</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxStartingPoint">
+                            <item>
+                              <property name="text">
+                                <string>Spectra</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Contributions</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_6">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="toolTip">
+                              <string>The SIMPLISMA algorithm attempts to chooses maximally orthogonal components. The SIMPLISMA noise parameter is set to 0.1 here.
+
+K-means clustering performs a clustering on the unscaled data and chooses representative cluster centers as starting points.</string>
+                            </property>
+                            <property name="text">
+                              <string>Initial values</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxInitialValues">
+                            <item>
+                              <property name="text">
+                                <string>Simplisma</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>K means clusters</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Clustersubtract</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QStackedWidget" name="stackedWidgetInit">
+                            <property name="currentIndex">
+                              <number>0</number>
+                            </property>
+                            <widget class="QWidget" name="page_2">
+                              <layout class="QHBoxLayout" name="horizontalLayout_6" stretch="1,0">
+                                <property name="leftMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="topMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="rightMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="bottomMargin">
+                                  <number>0</number>
+                                </property>
+                                <item>
+                                  <widget class="QLabel" name="label_22">
+                                    <property name="text">
+                                      <string>Noise</string>
+                                    </property>
+                                    <property name="alignment">
+                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="LineDouble" name="lineEditInitNoise">
+                                    <property name="text">
+                                      <string>0.1</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </widget>
+                            <widget class="QWidget" name="page_3"/>
+                            <widget class="QWidget" name="page">
+                              <layout class="QHBoxLayout" name="horizontalLayout_5" stretch="1,0,1,0">
+                                <property name="leftMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="topMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="rightMargin">
+                                  <number>0</number>
+                                </property>
+                                <property name="bottomMargin">
+                                  <number>0</number>
+                                </property>
+                                <item>
+                                  <widget class="QLabel" name="label_19">
+                                    <property name="text">
+                                      <string>Skew</string>
+                                    </property>
+                                    <property name="alignment">
+                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="LineDouble" name="lineEditInitSkew">
+                                    <property name="text">
+                                      <string>100</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QLabel" name="label_21">
+                                    <property name="text">
+                                      <string>P</string>
+                                    </property>
+                                    <property name="alignment">
+                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QSpinBox" name="spinBoxInitPower">
+                                    <property name="minimum">
+                                      <number>0</number>
+                                    </property>
+                                    <property name="maximum">
+                                      <number>3</number>
+                                    </property>
+                                    <property name="value">
+                                      <number>2</number>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </widget>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <widget class="LineDouble" name="lineEditP">
-                        <property name="text">
-                          <string>0.01</string>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_2" stretch="0,1,0,1,1,1,1">
+                        <item>
+                          <widget class="QCheckBox" name="checkBoxContrast">
+                            <property name="toolTip">
+                              <string>Improve contrast by angle-constrained ALS; see Windig and Keenan, Applied Spectroscopy 65: 349 (2011).</string>
+                            </property>
+                            <property name="text">
+                              <string>Enhance contrast of</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxContrast">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <item>
+                              <property name="text">
+                                <string>spectra</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>contributions</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_17">
+                            <property name="text">
+                              <string>by</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSlider" name="horizontalSliderContrast">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="maximum">
+                              <number>50</number>
+                            </property>
+                            <property name="pageStep">
+                              <number>5</number>
+                            </property>
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="LineDouble" name="lineEditContrast">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="text">
+                              <string>0</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_25">
+                            <property name="toolTip">
+                              <string>How to treat the region of interest. If required, at least one spectrum must be selected in every image.</string>
+                            </property>
+                            <property name="text">
+                              <string>Use ROI</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxUseRoi">
+                            <property name="currentIndex">
+                              <number>1</number>
+                            </property>
+                            <item>
+                              <property name="text">
+                                <string>Ignored</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>If defined</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Required</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
-                  </layout>
-                </widget>
-                <widget class="QWidget" name="page_3">
-                  <layout class="QHBoxLayout" name="horizontalLayout_22" stretch="0,1,1,2">
-                    <property name="leftMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="topMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="rightMargin">
-                      <number>0</number>
-                    </property>
-                    <property name="bottomMargin">
-                      <number>0</number>
-                    </property>
                     <item>
-                      <widget class="QLabel" name="labelLambdaArpls">
-                        <property name="text">
-                          <string>&amp;lambda;</string>
-                        </property>
-                        <property name="textFormat">
-                          <enum>Qt::RichText</enum>
-                        </property>
-                        <property name="buddy">
-                          <cstring>horizontalSliderLambdaArpls</cstring>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_4" stretch="0,0,0,1,0,1,5,1,1,0">
+                        <item>
+                          <widget class="QLabel" name="label_10">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="text">
+                              <string>Max iterations</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxIterations">
+                            <property name="minimumSize">
+                              <size>
+                                <width>50</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>1</number>
+                            </property>
+                            <property name="maximum">
+                              <number>9999</number>
+                            </property>
+                            <property name="value">
+                              <number>500</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_13">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="toolTip">
+                              <string>Stop at this relative decrease in error</string>
+                            </property>
+                            <property name="text">
+                              <string>Stopping improv.</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="LineDouble" name="lineEditTolerance">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>40</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="text">
+                              <string>0.01</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_14">
+                            <property name="text">
+                              <string>%</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_15">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="text">
+                              <string>Iteration</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QProgressBar" name="progressBarIteration">
+                            <property name="value">
+                              <number>0</number>
+                            </property>
+                            <property name="format">
+                              <string>idle</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_16">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="toolTip">
+                              <string>Mean square error relative to naively estimating data as the mean of all spectra.</string>
+                            </property>
+                            <property name="text">
+                              <string>Rel. err.</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLineEdit" name="lineEditRelError">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>40</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="readOnly">
+                              <bool>true</bool>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_12">
+                            <property name="text">
+                              <string>%</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <widget class="QSlider" name="horizontalSliderLambdaArpls">
-                        <property name="enabled">
-                          <bool>true</bool>
-                        </property>
-                        <property name="maximum">
-                          <number>80</number>
-                        </property>
-                        <property name="orientation">
-                          <enum>Qt::Horizontal</enum>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_11" stretch="0,0,0,6,0">
+                        <item>
+                          <widget class="QPushButton" name="pushButtonStart">
+                            <property name="text">
+                              <string>Run decomposition</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonStop">
+                            <property name="text">
+                              <string>Stop</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_2">
+                            <property name="text">
+                              <string>Plot mode</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxPlotMode">
+                            <property name="currentIndex">
+                              <number>-1</number>
+                            </property>
+                            <property name="maxVisibleItems">
+                              <number>16</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonSettingsInfo">
+                            <property name="text">
+                              <string>Show settings used</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <widget class="LineDouble" name="lineEditLambdaArpls">
-                        <property name="text">
-                          <string>1000</string>
+                      <widget class="DecompositionPlotWidget" name="plot_decomp" native="true">
+                        <property name="minimumSize">
+                          <size>
+                            <width>50</width>
+                            <height>50</height>
+                          </size>
                         </property>
                       </widget>
                     </item>
                     <item>
-                      <widget class="QLabel" name="label_2">
-                        <property name="text">
-                          <string/>
-                        </property>
-                      </widget>
+                      <layout class="QHBoxLayout" name="horizontalLayout_13">
+                        <item>
+                          <widget class="QProgressBar" name="progressBarRun">
+                            <property name="value">
+                              <number>0</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonRun">
+                            <property name="toolTip">
+                              <string>Run decomposition with the current setting on all data files</string>
+                            </property>
+                            <property name="text">
+                              <string>Run batch</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QToolButton" name="pushButtonRunStop">
+                            <property name="enabled">
+                              <bool>false</bool>
+                            </property>
+                            <property name="text">
+                              <string>Stop</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                   </layout>
                 </widget>
-                <widget class="QWidget" name="page_4">
-                  <layout class="QHBoxLayout" name="horizontalLayout_2" stretch="1,1,1,1">
+                <widget class="QWidget" name="tab_3">
+                  <attribute name="title">
+                    <string>Clustering</string>
+                  </attribute>
+                  <layout class="QVBoxLayout" name="verticalLayout_5" stretch="0,0,0,0,0,1">
                     <property name="leftMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="topMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="rightMargin">
-                      <number>0</number>
+                      <number>6</number>
                     </property>
                     <property name="bottomMargin">
-                      <number>0</number>
-                    </property>
-                    <item>
-                      <widget class="QLabel" name="labelBCThresh">
-                        <property name="text">
-                          <string>Poly-order</string>
-                        </property>
-                        <property name="buddy">
-                          <cstring>spinBoxBCPoly</cstring>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QSpinBox" name="spinBoxBCPoly">
-                        <property name="minimum">
-                          <number>1</number>
-                        </property>
-                        <property name="maximum">
-                          <number>10</number>
-                        </property>
-                        <property name="value">
-                          <number>3</number>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="labelBCPoly">
-                        <property name="text">
-                          <string>Threshold</string>
-                        </property>
-                        <property name="buddy">
-                          <cstring>lineEditBCThresh</cstring>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="LineDouble" name="lineEditBCThresh">
-                        <property name="text">
-                          <string>0.01</string>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </widget>
-              </widget>
-            </item>
-            <item>
-              <widget class="BCPlotWidget" name="plot_BC" native="true"/>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_20" stretch="0,3,1,0">
-                <item>
-                  <widget class="QCheckBox" name="checkBoxNorm">
-                    <property name="toolTip">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Rescale each spectrum so that some quantity becomes 1.&lt;/p&gt;&lt;p&gt;Mean: Mean intensity = 1&lt;br/&gt;Total area: Area under curve = 1&lt;br/&gt;Wavenumber: Intensity at specified wavenumber = 1&lt;br/&gt;Maximum: The maximum intensity of the spectrum = 1&lt;br/&gt;Vector: Euclidean norm = 1&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
-                    <property name="text">
-                      <string>Normalization</string>
+                      <number>6</number>
                     </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QComboBox" name="comboBoxNormMethod">
-                    <item>
-                      <property name="text">
-                        <string>Mean</string>
-                      </property>
-                    </item>
                     <item>
-                      <property name="text">
-                        <string>Total area</string>
-                      </property>
-                    </item>
-                    <item>
-                      <property name="text">
-                        <string>Wavenumber</string>
-                      </property>
+                      <layout class="QHBoxLayout" name="horizontalLayout_21" stretch="0,1,0,0">
+                        <item>
+                          <widget class="QLabel" name="label_34">
+                            <property name="text">
+                              <string>Input data</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxClusterInput">
+                            <property name="currentIndex">
+                              <number>2</number>
+                            </property>
+                            <item>
+                              <property name="text">
+                                <string>Raw data (ROI)</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Raw data (all)</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Decomposition concentrations</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_5">
+                            <property name="text">
+                              <string>Feature scaling</string>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxClusterNormalization">
+                            <item>
+                              <property name="text">
+                                <string>As-is</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Unit mean (divisive)</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Zero mean (subtractive)</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Zero mean, unit variance</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <property name="text">
-                        <string>Maximum</string>
-                      </property>
+                      <layout class="QHBoxLayout" name="horizontalLayout_20" stretch="0,1,0,0,0,0,1">
+                        <item>
+                          <widget class="QLabel" name="label_26">
+                            <property name="text">
+                              <string>Method</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxClusterMethod">
+                            <item>
+                              <property name="text">
+                                <string>K-means</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>K-Means (minibatch)</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>Strongest component</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_28">
+                            <property name="text">
+                              <string>Clusters</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxClusterClusters">
+                            <property name="minimumSize">
+                              <size>
+                                <width>50</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>2</number>
+                            </property>
+                            <property name="value">
+                              <number>5</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="label_29">
+                            <property name="text">
+                              <string>Best of</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="spinBoxClusterRestarts">
+                            <property name="minimumSize">
+                              <size>
+                                <width>45</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                            <property name="minimum">
+                              <number>1</number>
+                            </property>
+                            <property name="maximum">
+                              <number>10000</number>
+                            </property>
+                            <property name="value">
+                              <number>10</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QPushButton" name="pushButtonCluster">
+                            <property name="text">
+                              <string>Cluster</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <property name="text">
-                        <string>Vector</string>
-                      </property>
+                      <layout class="QHBoxLayout" name="horizontalLayout_18"/>
                     </item>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="LineDouble" name="lineEditNormWavenum">
-                    <property name="text">
-                      <string>1655</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QLabel" name="label_18">
-                    <property name="text">
-                      <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;cm&lt;span style=&quot; vertical-align:super;&quot;&gt;-1&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <widget class="NormPlotWidget" name="plot_norm" native="true"/>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_13">
-                <item>
-                  <widget class="QPushButton" name="pushButtonSaveParameters">
-                    <property name="text">
-                      <string>Save parameters</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="pushButtonLoadParameters">
-                    <property name="text">
-                      <string>Load parameters</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QPushButton" name="pushButtonRun">
-                    <property name="text">
-                      <string>Run batch</string>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QToolButton" name="pushButtonRunStop">
-                    <property name="enabled">
-                      <bool>false</bool>
-                    </property>
-                    <property name="text">
-                      <string>Stop</string>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <layout class="QHBoxLayout" name="horizontalLayout_28" stretch="1,2,1,2">
-                <item>
-                  <widget class="QLabel" name="label_13">
-                    <property name="text">
-                      <string>Save suffix</string>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QLineEdit" name="lineEditSaveExt">
-                    <property name="toolTip">
-                      <string>Extension added before .mat in output files.</string>
-                    </property>
-                    <property name="text">
-                      <string/>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QLabel" name="label_8">
-                    <property name="text">
-                      <string>Save format</string>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
-                  </widget>
-                </item>
-                <item>
-                  <widget class="QComboBox" name="comboBoxSaveFormat">
                     <item>
-                      <property name="text">
-                        <string>AB.mat</string>
-                      </property>
+                      <layout class="QHBoxLayout" name="horizontalLayout_14">
+                        <item>
+                          <layout class="QVBoxLayout" name="verticalLayout_6">
+                            <item>
+                              <widget class="QLabel" name="label_18">
+                                <property name="text">
+                                  <string>Input data</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QListWidget" name="listWidgetClusterInputs">
+                                <property name="enabled">
+                                  <bool>false</bool>
+                                </property>
+                                <property name="selectionMode">
+                                  <enum>QAbstractItemView::MultiSelection</enum>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QVBoxLayout" name="verticalLayout_7">
+                            <item>
+                              <layout class="QHBoxLayout" name="horizontalLayout_19">
+                                <item>
+                                  <widget class="QLabel" name="label_27">
+                                    <property name="text">
+                                      <string>Annotations</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QToolButton" name="toolButtonAnnotationPlus">
+                                    <property name="font">
+                                      <font>
+                                        <weight>75</weight>
+                                        <bold>true</bold>
+                                      </font>
+                                    </property>
+                                    <property name="text">
+                                      <string>+</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QToolButton" name="toolButtonAnnotationMinus">
+                                    <property name="text">
+                                      <string/>
+                                    </property>
+                                    <property name="icon">
+                                      <iconset theme="list-add.png">
+                                        <normaloff>../../../../.designer/backup</normaloff>
+                                        ../../../../.designer/backup
+                                      </iconset>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </item>
+                            <item>
+                              <widget class="QListWidget" name="listWidgetClusterAnnotations"/>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QVBoxLayout" name="verticalLayout_8">
+                            <item>
+                              <widget class="QLabel" name="label_31">
+                                <property name="text">
+                                  <string>Assigned clusters</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QListWidget" name="listWidgetClusterUsed">
+                                <property name="enabled">
+                                  <bool>false</bool>
+                                </property>
+                                <property name="dragDropMode">
+                                  <enum>QAbstractItemView::DragDrop</enum>
+                                </property>
+                                <property name="defaultDropAction">
+                                  <enum>Qt::MoveAction</enum>
+                                </property>
+                                <property name="selectionMode">
+                                  <enum>QAbstractItemView::NoSelection</enum>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                        <item>
+                          <layout class="QVBoxLayout" name="verticalLayout_9">
+                            <item>
+                              <widget class="QLabel" name="label_32">
+                                <property name="text">
+                                  <string>Unassigned clusters</string>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QListWidget" name="listWidgetClusterUnused">
+                                <property name="dragDropMode">
+                                  <enum>QAbstractItemView::DragDrop</enum>
+                                </property>
+                                <property name="defaultDropAction">
+                                  <enum>Qt::MoveAction</enum>
+                                </property>
+                                <property name="selectionMode">
+                                  <enum>QAbstractItemView::NoSelection</enum>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_16" stretch="0,1,1,1">
+                        <item>
+                          <widget class="QLabel" name="label">
+                            <property name="text">
+                              <string>Colors</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QComboBox" name="comboBoxClusterCmap">
+                            <item>
+                              <property name="text">
+                                <string>tab10</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>tab20</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>rainbow</string>
+                              </property>
+                            </item>
+                            <item>
+                              <property name="text">
+                                <string>terrain</string>
+                              </property>
+                            </item>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QCheckBox" name="checkBoxClusterShowAnnotations">
+                            <property name="text">
+                              <string>Show annotations</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QToolButton" name="toolButtonClusterExport">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="text">
+                              <string>Export annotated spectra</string>
+                            </property>
+                            <property name="popupMode">
+                              <enum>QToolButton::InstantPopup</enum>
+                            </property>
+                            <property name="arrowType">
+                              <enum>Qt::NoArrow</enum>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
                     </item>
                     <item>
-                      <property name="text">
-                        <string>Quasar.mat</string>
-                      </property>
+                      <widget class="ClusterPlotWidget" name="plot_cluster" native="true"/>
                     </item>
-                  </widget>
-                </item>
-              </layout>
-            </item>
-            <item>
-              <widget class="QProgressBar" name="progressBarRun">
-                <property name="value">
-                  <number>0</number>
-                </property>
+                  </layout>
+                </widget>
               </widget>
             </item>
           </layout>
         </item>
       </layout>
     </widget>
   </widget>
@@ -1190,91 +1315,40 @@
     <customwidget>
       <class>FileLoaderWidget</class>
       <extends>QWidget</extends>
       <header location="global">octavvs/ui/fileloader.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>ImageVisualizerWidget</class>
-      <extends>QWidget</extends>
-      <header location="global">octavvs/ui/imagevisualizer.h</header>
-      <container>1</container>
-    </customwidget>
-    <customwidget>
-      <class>NormPlotWidget</class>
-      <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
-      <container>1</container>
-      <slots>
-        <signal>clicked()</signal>
-        <slot>popOut()</slot>
-      </slots>
-    </customwidget>
-    <customwidget>
-      <class>BCPlotWidget</class>
-      <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
-      <container>1</container>
-    </customwidget>
-    <customwidget>
-      <class>SCPlotWidget</class>
-      <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
-      <container>1</container>
-    </customwidget>
-    <customwidget>
-      <class>ACPlotWidget</class>
+      <class>DecompositionPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <header location="global">octavvs/decomp/plotwidget.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>SGFPlotWidget</class>
+      <class>ImageVisualizerWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <header location="global">octavvs/ui/imagevisualizer.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>SRPlotWidget</class>
+      <class>RoiPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <header location="global">octavvs/decomp/plotwidget.h</header>
       <container>1</container>
     </customwidget>
     <customwidget>
-      <class>MCPlotWidget</class>
+      <class>ClusterPlotWidget</class>
       <extends>QWidget</extends>
-      <header location="global">octavvs/prep/dataplotwidget.h</header>
+      <header location="global">octavvs/decomp/plotwidget.h</header>
       <container>1</container>
     </customwidget>
   </customwidgets>
   <tabstops>
-    <tabstop>checkBoxAC</tabstop>
-    <tabstop>checkBoxSpline</tabstop>
-    <tabstop>checkBoxLocalPeak</tabstop>
-    <tabstop>checkBoxSmoothCorrected</tabstop>
-    <tabstop>checkBoxSC</tabstop>
-    <tabstop>pushButtonSCRefresh</tabstop>
-    <tabstop>pushButtonSCStop</tabstop>
-    <tabstop>comboBoxReference</tabstop>
-    <tabstop>spinBoxNIteration</tabstop>
-    <tabstop>checkBoxClusters</tabstop>
-    <tabstop>spinBoxNclusScat</tabstop>
-    <tabstop>checkBoxStabilize</tabstop>
-    <tabstop>pushButtonSCAdvanced</tabstop>
-    <tabstop>spinBoxWindowLength</tabstop>
-    <tabstop>spinBoxPolyOrder</tabstop>
-    <tabstop>lineEditMinwn</tabstop>
-    <tabstop>horizontalSliderMin</tabstop>
-    <tabstop>horizontalSliderMax</tabstop>
-    <tabstop>lineEditMaxwn</tabstop>
-    <tabstop>comboBoxBaseline</tabstop>
-    <tabstop>comboBoxNormMethod</tabstop>
-    <tabstop>lineEditNormWavenum</tabstop>
-    <tabstop>pushButtonSaveParameters</tabstop>
-    <tabstop>pushButtonLoadParameters</tabstop>
+    <tabstop>comboBoxClusterMethod</tabstop>
     <tabstop>pushButtonRun</tabstop>
     <tabstop>pushButtonRunStop</tabstop>
   </tabstops>
   <resources/>
   <connections/>
   <designerdata>
     <property name="gridDeltaX">
```

### Comparing `octavvs-0.1.8/octavvs/prep/prepworker.py` & `octavvs-0.1.9/octavvs/prep/prepworker.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/prep/scadvanced.ui` & `octavvs-0.1.9/octavvs/prep/scadvanced.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/preprocessing.py` & `octavvs-0.1.9/octavvs/preprocessing.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/pymcr_new/constraints.py` & `octavvs-0.1.9/octavvs/pymcr_new/constraints.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/pymcr_new/regressors.py` & `octavvs-0.1.9/octavvs/pymcr_new/regressors.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/CAS_bg_10perc_crub7.mat` & `octavvs-0.1.9/octavvs/reference_spectra/CAS_bg_10perc_crub7.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/CAS_wh_5perc.mat` & `octavvs-0.1.9/octavvs/reference_spectra/CAS_wh_5perc.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/CMC_bg_10perc_crub7.mat` & `octavvs-0.1.9/octavvs/reference_spectra/CMC_bg_10perc_crub7.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/CMC_wh_5perc.mat` & `octavvs-0.1.9/octavvs/reference_spectra/CMC_wh_5perc.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/LIG_bg_10perc_crub7.mat` & `octavvs-0.1.9/octavvs/reference_spectra/LIG_bg_10perc_crub7.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/LIG_wh_5perc.mat` & `octavvs-0.1.9/octavvs/reference_spectra/LIG_wh_5perc.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/PEC_bg_10perc_crub7.mat` & `octavvs-0.1.9/octavvs/reference_spectra/PEC_bg_10perc_crub7.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/Q_table.mat` & `octavvs-0.1.9/octavvs/reference_spectra/Q_table.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/casein.mat` & `octavvs-0.1.9/octavvs/reference_spectra/casein.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/lignin.mat` & `octavvs-0.1.9/octavvs/reference_spectra/lignin.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/matrigel.mat` & `octavvs-0.1.9/octavvs/reference_spectra/matrigel.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/reference_spectra/water.mat` & `octavvs-0.1.9/octavvs/reference_spectra/water.mat`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/copyfigure.py` & `octavvs-0.1.9/octavvs/ui/copyfigure.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/elidedlabel.py` & `octavvs-0.1.9/octavvs/ui/elidedlabel.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/exceptiondialog.py` & `octavvs-0.1.9/octavvs/ui/exceptiondialog.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/fileloader.py` & `octavvs-0.1.9/octavvs/ui/fileloader.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/fileloader.ui` & `octavvs-0.1.9/octavvs/ui/fileloader.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/imagevisualizer.py` & `octavvs-0.1.9/octavvs/ui/imagevisualizer.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/imagevisualizer.ui` & `octavvs-0.1.9/octavvs/ui/imagevisualizer.ui`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/linedouble.py` & `octavvs-0.1.9/octavvs/ui/linedouble.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/octavvsapplication.py` & `octavvs-0.1.9/octavvs/ui/octavvsapplication.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 
 class OctavvsMainWindow(QMainWindow):
 
     fileOptions = QFileDialog.Options() | QFileDialog.DontUseNativeDialog
 
-    octavvs_version = 'v0.1.8'
+    octavvs_version = 'v0.1.9'
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.settings = QSettings('MICCS', 'OCTAVVS ' + self.program_name())
         qApp.installEventFilter(self)
         self.setupUi(self)
```

### Comparing `octavvs-0.1.8/octavvs/ui/projectionwidget.py` & `octavvs-0.1.9/octavvs/ui/projectionwidget.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/uitools.py` & `octavvs-0.1.9/octavvs/ui/uitools.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs/ui/whitelightwidget.py` & `octavvs-0.1.9/octavvs/ui/whitelightwidget.py`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/octavvs.egg-info/PKG-INFO` & `octavvs-0.1.9/octavvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octavvs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Open Chemometrics Toolkit for Analysis and Visualization of Vibrational Spectroscopy data
 Home-page: https://github.com/ctroein/octavvs
 Author: Syahril Siregar, Carl Troein, Michiel Op De Beeck et al.
 Author-email: carl@thep.lu.se
 License: UNKNOWN
 Description: # OCTAVVS: Open Chemometrics Toolbox for Analysis and Visualization of Vibrational Spectroscopy data
```

### Comparing `octavvs-0.1.8/octavvs.egg-info/SOURCES.txt` & `octavvs-0.1.9/octavvs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octavvs-0.1.8/setup.py` & `octavvs-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                'clustering': 'Clustering'}
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="octavvs",
-    version="0.1.8",
+    version="0.1.9",
     author="Syahril Siregar, Carl Troein, Michiel Op De Beeck et al.",
     author_email="carl@thep.lu.se",
     description="Open Chemometrics Toolkit for Analysis and Visualization of Vibrational Spectroscopy data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ctroein/octavvs",
     packages=setuptools.find_packages(),
```


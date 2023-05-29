# Comparing `tmp/nzpyida-0.3.5.tar.gz` & `tmp/nzpyida-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.3.5.tar", last modified: Mon May 29 14:02:59 2023, max compression
+gzip compressed data, was "nzpyida-0.3.6.tar", last modified: Mon May 29 14:25:47 2023, max compression
```

## Comparing `nzpyida-0.3.5.tar` & `nzpyida-0.3.6.tar`

### file list

```diff
@@ -1,157 +1,158 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.696948 nzpyida-0.3.5/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.5/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.5/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.5/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:02:59.697030 nzpyida-0.3.5/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.3.5/README.md
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.664654 nzpyida-0.3.5/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.5/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.668240 nzpyida-0.3.5/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.5/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.5/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2638 2023-05-25 14:48:09.000000 nzpyida-0.3.5/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.672110 nzpyida-0.3.5/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.5/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.675061 nzpyida-0.3.5/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.677029 nzpyida-0.3.5/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.677338 nzpyida-0.3.5/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.678429 nzpyida-0.3.5/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     1815 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.3.5/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.679077 nzpyida-0.3.5/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.682616 nzpyida-0.3.5/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     6581 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/glm.py
--rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.686917 nzpyida-0.3.5/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     3561 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-05-17 10:45:26.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_glm.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     2393 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.687664 nzpyida-0.3.5/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     7634 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.3.5/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.689546 nzpyida-0.3.5/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.5/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.691345 nzpyida-0.3.5/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.3.5/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.696706 nzpyida-0.3.5/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.5/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.5/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.5/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.5/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.673059 nzpyida-0.3.5/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4726 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-29 14:02:59.697302 nzpyida-0.3.5/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3318 2023-05-25 07:54:36.000000 nzpyida-0.3.5/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.762159 nzpyida-0.3.6/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.6/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.6/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.6/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:25:47.762226 nzpyida-0.3.6/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.3.6/README.md
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.738536 nzpyida-0.3.6/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.6/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.741168 nzpyida-0.3.6/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.6/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geoFrame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geoSeries.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.6/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2638 2023-05-25 14:48:09.000000 nzpyida-0.3.6/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.6/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.743181 nzpyida-0.3.6/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.6/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.745180 nzpyida-0.3.6/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.746293 nzpyida-0.3.6/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.746473 nzpyida-0.3.6/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.747185 nzpyida-0.3.6/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     1833 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.3.6/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.747691 nzpyida-0.3.6/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.750089 nzpyida-0.3.6/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8440 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.754220 nzpyida-0.3.6/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     3591 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-05-17 10:45:26.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2067 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_cross_validation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3041 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.754975 nzpyida-0.3.6/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10906 2023-05-29 14:08:02.000000 nzpyida-0.3.6/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.3.6/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.756726 nzpyida-0.3.6/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.6/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.758039 nzpyida-0.3.6/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.3.6/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.762024 nzpyida-0.3.6/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.6/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.6/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.3.6/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.6/nzpyida/tests/test_geoFrame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.6/nzpyida/tests/test_geoSeries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.6/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:25:47.743975 nzpyida-0.3.6/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4775 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-29 14:25:47.000000 nzpyida-0.3.6/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-29 14:25:47.762509 nzpyida-0.3.6/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3318 2023-05-29 14:25:35.000000 nzpyida-0.3.6/setup.py
```

### Comparing `nzpyida-0.3.5/LICENSE.txt` & `nzpyida-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/PKG-INFO` & `nzpyida-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.5
+Version: 0.3.6
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.3.5/README.md` & `nzpyida-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/.DS_Store` & `nzpyida-0.3.6/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/Makefile` & `nzpyida-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/make.bat` & `nzpyida-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/base.rst` & `nzpyida-0.3.6/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/conf.py` & `nzpyida-0.3.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/frame.rst` & `nzpyida-0.3.6/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/geoFrame.rst` & `nzpyida-0.3.6/docs/source/geoFrame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/geoSeries.rst` & `nzpyida-0.3.6/docs/source/geoSeries.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/geospatial.rst` & `nzpyida-0.3.6/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/ibm.png` & `nzpyida-0.3.6/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/index.rst` & `nzpyida-0.3.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/install.rst` & `nzpyida-0.3.6/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/kc.ico` & `nzpyida-0.3.6/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/legal.rst` & `nzpyida-0.3.6/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/predictive.rst` & `nzpyida-0.3.6/docs/source/predictive.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/start.rst` & `nzpyida-0.3.6/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/docs/source/utils.rst` & `nzpyida-0.3.6/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/__init__.py` & `nzpyida-0.3.6/nzpyida/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/__init__.py` & `nzpyida-0.3.6/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/apply.py` & `nzpyida-0.3.6/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.3.6/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/groupedapply.py` & `nzpyida-0.3.6/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/install.py` & `nzpyida-0.3.6/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/result_builder.py` & `nzpyida-0.3.6/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/shaper.py` & `nzpyida-0.3.6/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/tapply.py` & `nzpyida-0.3.6/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/tapply_class.py` & `nzpyida-0.3.6/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.3.6/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/aggregation.py` & `nzpyida-0.3.6/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/__init__.py` & `nzpyida-0.3.6/nzpyida/analytics/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 from .predictive.glm import BernoulliRegressor, BinomialRegressor, \
     NegativeBinomialRegressor, GaussianRegressor, GammaRegressor, \
     PoissonRegressor, WaldRegressor
 from .exploration.distribution import bitable, moments, histogram, outliers
 from .exploration.distribution import quantile, unitable
 from .transform.discretization import EFDisc, EMDisc, EWDisc
 from .transform.discretization import ef_disc, em_disc, ew_disc
-from .transform.preparation import std_norm, impute_data, random_sample
+from .transform.preparation import std_norm, impute_data, random_sample, train_test_split
 from .model_manager import ModelManager
 from .auto_delete_context import AutoDeleteContext
 from .exploration.relation_identification import corr, cov, covariance_matrix, \
 spearman_corr, mutual_info, chisq, t_me_test, t_ls_test, t_pmd_test, t_umd_test, \
 mww_test, wilcoxon_test, canonical_corr, anova_crd_test, anova_rbd_test, \
 manova_one_way_test, manova_two_way_test
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.3.6/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.3.6/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.3.6/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/model_manager.py` & `nzpyida-0.3.6/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/regression.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,87 +5,90 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 """
-This module contains a class that is the base for all classification algorithms.
+This module contains a class that is the base for all regression algorithms.
 """
-from typing import Tuple
+from typing import Dict
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
-from nzpyida.analytics.utils import get_auto_delete_context
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 
 
-class Classification(PredictiveModeling):
+class Regression(PredictiveModeling):
     """
-    Base class for classification algorithms.
+    Base class for regression algorithms.
     """
 
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
-        Creates the classifier class.
+        Creates the regressor class.
 
         Parameters
         ----------
 
         idada : IdaDataBase
             database connector
 
         model_name : str
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
-        self.target_column_in_output = 'CLASS'
+        self.score_proc = 'MSE'
         self.id_column_in_output = 'ID'
-        self.score_proc = 'CERROR'
-        self.score_inv = True
 
     def predict(self, in_df: IdaDataFrame, out_table: str=None,
         id_column: str=None) -> IdaDataFrame:
         """
         Makes predictions based on this model. The model must exist.
 
         Parameters
         ----------
         in_df : IdaDataFrame
-            the input data frame for predictions
+            the input data frame to predict
 
         out_table : str, optional
             the output table where the predictions will be stored
 
         id_column : str, optional
             the input table column identifying a unique instance id
             Default: id column used to build the model
+
+        Returns
+        -------
+        IdaDataFrame
+            the data frame containing row identifiers and predicted target values
         """
 
         params = {
             'id': id_column
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
-    def score(self, in_df: IdaDataFrame, target_column: str, id_column: str=None) -> float:
+    def score(self, in_df: IdaDataFrame, target_column: str,
+        id_column: str=None) -> float:
         """
         Scores the model. The model must exist.
 
         Parameters
         ----------
         in_df : IdaDataFrame
             the input data frame for scoring
 
         target_column : str
             the input table column representing the class
 
-        id_column : str, optional
+        id_column : str
             the input table column identifying a unique instance id - if skipped, 
             the input data frame indexer must be set and will be used as an instance id
 
         Returns
         -------
         float
             the model score
@@ -93,103 +96,76 @@
 
         params = {
             'id': id_column
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
 
-    def conf_matrix(self, in_df: IdaDataFrame, target_column: str, id_column: str=None,
-        out_matrix_table: str=None) -> Tuple[IdaDataFrame, float, float]:
+    def score_all(self, in_df: IdaDataFrame, target_column: str,
+        id_column: str=None) -> Dict[str, float]:
         """
-        Makes a predition for a test data set given by the user and returns a confusion matrix,
-        together with other stats (ACC and WACC).
+        Scores the model using MSE, MAE, RSE and RAE. The model must exist.
 
         Parameters
         ----------
         in_df : IdaDataFrame
             the input data frame for scoring
 
         target_column : str
             the input table column representing the class
 
         id_column : str, optional
             the input table column identifying a unique instance id - if skipped, 
             the input data frame indexer must be set and will be used as an instance id
 
-        out_matrix_table : str, optional
-            the output table where the confidence matrix will be stored
-
         Returns
         -------
-        IdaDataFrame
-            the confidence matrix data frame
-
-        float
-            classification accuracy (ACC)
-
-        float
-            weighted classification accuracy (WACC)
+        dict
+            the model scores in a dictionary with MSE, MAE, RSE and RAE as keys
         """
-
-        params = {
-            'id': id_column,
-            'target': target_column
-        }
-        return self._conf_matrix(in_df, out_matrix_table, params)
-        
-    def _conf_matrix(self, in_df: IdaDataFrame, out_matrix_table: str=None,
-                     params: dict={}) -> Tuple[IdaDataFrame, float, float]:
-
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
-        if not params.get('id'):
+        if not id_column:
             if in_df.indexer:
-                params['id'] = in_df.indexer
+                id_column = in_df.indexer
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         out_table = make_temp_table_name()
 
         pred_view_needs_delete, true_view_needs_delete = False, False
         try:
-            pred_df = self._predict(in_df=in_df, out_table=out_table, params=params)
+            pred_df = self.predict(in_df=in_df, out_table=out_table, id_column=id_column)
+
             pred_view, pred_view_needs_delete = materialize_df(pred_df)
             true_view, true_view_needs_delete = materialize_df(in_df)
 
-            auto_delete_context = None
-            if not out_matrix_table:
-                auto_delete_context = get_auto_delete_context('out_matrix_table')
-                out_matrix_table = make_temp_table_name()
-
-            params_s = map_to_props({
-                'resulttable': pred_view,
-                'intable': true_view,
-                'resultid': 'ID',
-                'id': params['id'],
-                'resulttarget': 'CLASS',
-                'target': params['target'],
-                'matrixTable': out_matrix_table
-            })
-            self.idadb.ida_query(f'call NZA..CONFUSION_MATRIX(\'{params_s}\')')
-
-            if auto_delete_context:
-                auto_delete_context.add_table_to_delete(out_matrix_table)
-
-            out_df = IdaDataFrame(self.idadb, out_matrix_table)
-
             params = map_to_props({
-                'matrixTable': out_matrix_table
+                'pred_table': pred_view,
+                'true_table': true_view,
+                'pred_id': id_column if self.id_column_in_output is None
+                    else self.id_column_in_output,
+                'true_id': id_column,
+                'pred_column': target_column if self.target_column_in_output is None
+                    else self.target_column_in_output,
+                'true_column': target_column
             })
 
-            res_acc = self.idadb.ida_query(f'call NZA..CMATRIX_ACC(\'{params}\')')
-            res_wacc = self.idadb.ida_query(f'call NZA..CMATRIX_WACC(\'{params}\')')
-
-            return out_df, res_acc[0], res_wacc[0]
-
+            res1 = pred_df.ida_query(f'call NZA..MSE(\'{params}\')')
+            res2 = pred_df.ida_query(f'call NZA..MAE(\'{params}\')')
+            res3 = pred_df.ida_query(f'call NZA..RSE(\'{params}\')')
+            res4 = pred_df.ida_query(f'call NZA..RAE(\'{params}\')')
+            res_dict = {
+                "MSE": res1[0],
+                "MAE": res2[0],
+                "RSE": res3[0],
+                "RAE": res4[0]
+            }
+            return res_dict
         finally:
             self.idadb.drop_table(out_table)
             if pred_view_needs_delete:
                 self.idadb.drop_view(pred_view)
             if true_view_needs_delete:
                 self.idadb.drop_view(true_view)
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/glm.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/classification.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,90 +5,90 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 """
-This module contains a class that is the base for all regression algorithms.
+This module contains a class that is the base for all classification algorithms.
 """
-from typing import Dict
+from typing import Tuple
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
-from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name
+from nzpyida.analytics.utils import map_to_props, materialize_df, make_temp_table_name, \
+call_proc_df_in_out
+from nzpyida.analytics.utils import get_auto_delete_context
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
+from nzpyida.analytics.model_manager import ModelManager
 
 
-class Regression(PredictiveModeling):
+class Classification(PredictiveModeling):
     """
-    Base class for regression algorithms.
+    Base class for classification algorithms.
     """
 
     def __init__(self, idadb: IdaDataBase, model_name: str):
         """
-        Creates the regressor class.
+        Creates the classifier class.
 
         Parameters
         ----------
 
         idada : IdaDataBase
             database connector
 
         model_name : str
             model name - if it exists in the database, it will be used, otherwise
             it must be trained using fit() function before prediction or scoring is called.
         """
 
         super().__init__(idadb, model_name)
-        self.score_proc = 'MSE'
+        self.target_column_in_output = 'CLASS'
         self.id_column_in_output = 'ID'
+        self.score_proc = 'CERROR'
+        self.score_inv = True
+        self.type = None
 
     def predict(self, in_df: IdaDataFrame, out_table: str=None,
         id_column: str=None) -> IdaDataFrame:
         """
         Makes predictions based on this model. The model must exist.
 
         Parameters
         ----------
         in_df : IdaDataFrame
-            the input data frame to predict
+            the input data frame for predictions
 
         out_table : str, optional
             the output table where the predictions will be stored
 
         id_column : str, optional
             the input table column identifying a unique instance id
             Default: id column used to build the model
-
-        Returns
-        -------
-        IdaDataFrame
-            the data frame containing row identifiers and predicted target values
         """
 
         params = {
             'id': id_column
         }
 
         return self._predict(in_df=in_df, params=params, out_table=out_table)
 
-    def score(self, in_df: IdaDataFrame, target_column: str,
-        id_column: str=None) -> float:
+    def score(self, in_df: IdaDataFrame, target_column: str, id_column: str=None) -> float:
         """
         Scores the model. The model must exist.
 
         Parameters
         ----------
         in_df : IdaDataFrame
             the input data frame for scoring
 
         target_column : str
             the input table column representing the class
 
-        id_column : str
+        id_column : str, optional
             the input table column identifying a unique instance id - if skipped, 
             the input data frame indexer must be set and will be used as an instance id
 
         Returns
         -------
         float
             the model score
@@ -96,76 +96,153 @@
 
         params = {
             'id': id_column
         }
 
         return self._score(in_df=in_df, predict_params=params, target_column=target_column)
 
-    def score_all(self, in_df: IdaDataFrame, target_column: str,
-        id_column: str=None) -> Dict[str, float]:
+    def conf_matrix(self, in_df: IdaDataFrame, target_column: str, id_column: str=None,
+        out_matrix_table: str=None) -> Tuple[IdaDataFrame, float, float]:
         """
-        Scores the model using MSE, MAE, RSE and RAE. The model must exist.
+        Makes a predition for a test data set given by the user and returns a confusion matrix,
+        together with other stats (ACC and WACC).
 
         Parameters
         ----------
         in_df : IdaDataFrame
             the input data frame for scoring
 
         target_column : str
             the input table column representing the class
 
         id_column : str, optional
             the input table column identifying a unique instance id - if skipped, 
             the input data frame indexer must be set and will be used as an instance id
 
+        out_matrix_table : str, optional
+            the output table where the confidence matrix will be stored
+
         Returns
         -------
-        dict
-            the model scores in a dictionary with MSE, MAE, RSE and RAE as keys
+        IdaDataFrame
+            the confidence matrix data frame
+
+        float
+            classification accuracy (ACC)
+
+        float
+            weighted classification accuracy (WACC)
         """
+
+        params = {
+            'id': id_column,
+            'target': target_column
+        }
+        return self._conf_matrix(in_df, out_matrix_table, params)
+        
+    def _conf_matrix(self, in_df: IdaDataFrame, out_matrix_table: str=None,
+                     params: dict={}) -> Tuple[IdaDataFrame, float, float]:
+
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
-        if not id_column:
+        if not params.get('id'):
             if in_df.indexer:
-                id_column = in_df.indexer
+                params['id'] = in_df.indexer
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
 
         out_table = make_temp_table_name()
 
         pred_view_needs_delete, true_view_needs_delete = False, False
         try:
-            pred_df = self.predict(in_df=in_df, out_table=out_table, id_column=id_column)
-
+            pred_df = self._predict(in_df=in_df, out_table=out_table, params=params)
             pred_view, pred_view_needs_delete = materialize_df(pred_df)
             true_view, true_view_needs_delete = materialize_df(in_df)
 
+            auto_delete_context = None
+            if not out_matrix_table:
+                auto_delete_context = get_auto_delete_context('out_matrix_table')
+                out_matrix_table = make_temp_table_name()
+
+            params_s = map_to_props({
+                'resulttable': pred_view,
+                'intable': true_view,
+                'resultid': 'ID',
+                'id': params['id'],
+                'resulttarget': 'CLASS',
+                'target': params['target'],
+                'matrixTable': out_matrix_table
+            })
+            self.idadb.ida_query(f'call NZA..CONFUSION_MATRIX(\'{params_s}\')')
+
+            if auto_delete_context:
+                auto_delete_context.add_table_to_delete(out_matrix_table)
+
+            out_df = IdaDataFrame(self.idadb, out_matrix_table)
+
             params = map_to_props({
-                'pred_table': pred_view,
-                'true_table': true_view,
-                'pred_id': id_column if self.id_column_in_output is None
-                    else self.id_column_in_output,
-                'true_id': id_column,
-                'pred_column': target_column if self.target_column_in_output is None
-                    else self.target_column_in_output,
-                'true_column': target_column
+                'matrixTable': out_matrix_table
             })
 
-            res1 = pred_df.ida_query(f'call NZA..MSE(\'{params}\')')
-            res2 = pred_df.ida_query(f'call NZA..MAE(\'{params}\')')
-            res3 = pred_df.ida_query(f'call NZA..RSE(\'{params}\')')
-            res4 = pred_df.ida_query(f'call NZA..RAE(\'{params}\')')
-            res_dict = {
-                "MSE": res1[0],
-                "MAE": res2[0],
-                "RSE": res3[0],
-                "RAE": res4[0]
-            }
-            return res_dict
+            res_acc = self.idadb.ida_query(f'call NZA..CMATRIX_ACC(\'{params}\')')
+            res_wacc = self.idadb.ida_query(f'call NZA..CMATRIX_WACC(\'{params}\')')
+
+            return out_df, res_acc[0], res_wacc[0]
+
         finally:
             self.idadb.drop_table(out_table)
             if pred_view_needs_delete:
                 self.idadb.drop_view(pred_view)
             if true_view_needs_delete:
                 self.idadb.drop_view(true_view)
+    
+    def cross_validation(self, in_df: IdaDataFrame, id_column: str=None, 
+                         target_column: str=None, out_table: str=None, folds: int=10, 
+                         rand_seed: float=None) -> Tuple[IdaDataFrame, float]:
+        """
+        Performs a cross validation on <in_df> data for given model. Numer of batches 
+        and size of train/test split isdetermined by parameter <folds>
+
+        Parameters
+        ----------
+        in_df : IdaDataFrame
+            the input data frame for scoring
+
+        id_column : str, optional
+            the input table column identifying a unique instance id - if skipped, 
+            the input data frame indexer must be set and will be used as an instance id
+
+        target_column : str
+            the input table column representing the class
+
+        out_table : str, optional
+            the output table where the predicted values will be stored
+
+        Returns
+        -------
+        IdaDataFrame
+            the data frame with predicted values for all <in_df>
+
+        float
+            classification accuracy (ACC) for all batches 
+        """
+        params = {
+            'modelType': self.fit_proc,
+            'model': self.model_name,
+            'intable': in_df,
+            'id': id_column,
+            'target': target_column,
+            'outtable': out_table,
+            'folds': folds,
+        }
+        if isinstance(rand_seed, int):
+            params['seed'] = rand_seed
+        
+        ModelManager(self.idadb).drop_model(self.model_name)
+        
+        ret_df, ret_acc = call_proc_df_in_out(proc="CROSS_VALIDATION", in_df=in_df, params=params,
+                                   out_table=out_table)
+        
+        return ret_df, ret_acc[0]
+
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.3.6/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/conftest.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,7 +113,8 @@
 TAB_NAME_TEST = "TAB_NAME1"
 TAB_NAME_TRAIN = "TAB_NAME2"
 
 MOD_NAME = "TEST_MOD1"
 
 OUT_TABLE_PRED = "OUT_TABLE_PRED"
 OUT_TABLE_CM = "OUT_TABLE_CM"
+OUT_TABLE_CV = "OUT_TABLE_CV"
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_glm.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_preparation.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,45 @@
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 import pytest
 import numpy as np
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.auto_delete_context import AutoDeleteContext
-from nzpyida.analytics.tests.conftest import df_train, TAB_NAME_TRAIN
-from nzpyida.analytics.transform.preparation import std_norm, impute_data, random_sample
+from nzpyida.analytics.tests.conftest import df_train, TAB_NAME_TRAIN, \
+    TAB_NAME_TEST
+from nzpyida.analytics.transform.preparation import std_norm, impute_data, \
+    random_sample, train_test_split
 
-TEST_TAB_NAME = "TEST_TAB_NAME"
+TAB_NAME = "TAB_NAME0"
 
 @pytest.fixture(scope='function')
 def clean_up(idadb: IdaDataBase):
-    if idadb.exists_table(TEST_TAB_NAME):
-        idadb.drop_table(TEST_TAB_NAME)
+    if idadb.exists_table(TAB_NAME_TRAIN):
+        idadb.drop_table(TAB_NAME_TRAIN)
+    if idadb.exists_table(TAB_NAME_TEST):
+        idadb.drop_table(TAB_NAME_TEST)
     yield
-    if idadb.exists_table(TEST_TAB_NAME):
-        idadb.drop_table(TEST_TAB_NAME)
+    if idadb.exists_table(TAB_NAME_TRAIN):
+        idadb.drop_table(TAB_NAME_TRAIN)
+    if idadb.exists_table(TAB_NAME_TEST):
+        idadb.drop_table(TAB_NAME_TEST)
 
 @pytest.fixture(scope='module')
 def idf(idadb: IdaDataBase):
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
+    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME, clear_existing=True, indexer='ID')
     yield idf
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
+    if idadb.exists_table(TAB_NAME):
+        idadb.drop_table(TAB_NAME)
 
 def test_std_norm(idadb: IdaDataBase, clean_up, idf):
 
-    out_df = std_norm(idf, in_column=["A:S"], by_column=['B'], out_table=TEST_TAB_NAME)
+    out_df = std_norm(idf, in_column=["A:S"], by_column=['B'], out_table=TAB_NAME_TEST)
     assert out_df
-    assert idadb.exists_table_or_view(TEST_TAB_NAME)
+    assert idadb.exists_table_or_view(TAB_NAME_TEST)
 
     assert all(out_df.columns == ['B', 'ID', 'STD_A'])
 
     assert len(out_df) == len(idf)
 
 
 def test_random_sample(idadb: IdaDataBase, idf, clean_up):
@@ -60,7 +66,19 @@
 
 def test_impute_data(idadb: IdaDataBase, clean_up):
     df_train['new'] = np.nan
     idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
 
     assert idf
     assert idadb.exists_table_or_view(TAB_NAME_TRAIN)
+
+
+def test_train_test_split(idadb: IdaDataBase, idf, clean_up):
+    train_df, test_df = train_test_split(idf, TAB_NAME_TRAIN, TAB_NAME_TEST, fraction=0.8,
+                                         id_column="ID")
+    assert test_df
+    assert test_df
+    assert round(len(train_df)/len(idf), 1) == 0.8
+    assert round(len(test_df)/len(idf), 1) == 0.2
+
+    assert not any(el in train_df['ID'].as_dataframe().values for el in test_df["ID"].as_dataframe().values)
+
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.3.6/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.3.6/nzpyida/analytics/transform/discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.3.6/nzpyida/analytics/transform/preparation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 # Copyright (c) 2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 """
 This module contains function that can be used to prepare an input data
 frame for machine learning.
 """
-from typing import List
+from typing import List, Tuple
 from nzpyida.frame import IdaDataFrame
-from nzpyida.analytics.utils import call_proc_df_in_out
+from nzpyida.analytics.utils import materialize_df, make_temp_table_name, \
+    get_auto_delete_context, call_proc_df_in_out, map_to_props
 
 
-def std_norm(in_df: IdaDataFrame, in_column: List[str], id_column: str=None,
-    by_column: str=None, out_table: str=None) -> IdaDataFrame:
+def std_norm(in_df: IdaDataFrame, in_column: List[str], id_column: str = None,
+             by_column: str = None, out_table: str = None) -> IdaDataFrame:
     """
     Standardization and normalization transformations use the original continuous
     attribute a to generate a new continuous attribute a ' that has a different range
     or distribution than the original attribute. Common transformations modify the
     range to fit the [-1,1 ] interval (normalization) or modify the distribution to
     have a mean of 0 and a standard deviation of 1 (standardization).
 
@@ -59,27 +60,27 @@
         the data frame with requested transformations
     """
     if not id_column:
         if in_df.indexer:
             id_column = in_df.indexer
         else:
             raise TypeError('Missing id column - either use id_column attribute or set '
-                'indexer column in the input data frame')
+                            'indexer column in the input data frame')
 
     params = {
         'id': id_column,
         'incolumn': in_column,
         'by': by_column
     }
-    return call_proc_df_in_out(proc='STD_NORM', in_df=in_df, params=params, 
-        out_table=out_table, copy_indexer=True)[0]
+    return call_proc_df_in_out(proc='STD_NORM', in_df=in_df, params=params,
+                               out_table=out_table, copy_indexer=True)[0]
 
 
-def impute_data(in_df: IdaDataFrame, in_column: str=None, method: str=None,
-    numeric_value: float=-1, nominal_value: str='missing', out_table: str=None) -> IdaDataFrame:
+def impute_data(in_df: IdaDataFrame, in_column: str = None, method: str = None,
+                numeric_value: float = -1, nominal_value: str = 'missing', out_table: str = None) -> IdaDataFrame:
     """
     Many analytic algorithms require that the data set has no missing attribute values.
     However, real-world data sets frequently suffer from missing attribute values.
     Missing value imputation provides usable attribute values in place of the missing values,
     allowing the algorithms to run.
 
     This function replaces missing values in the input data frame and returns the result
@@ -116,32 +117,32 @@
 
     params = {
         'incolumn': in_column,
         'method': method,
         'numericvalue': numeric_value,
         'nominalvalue': nominal_value
     }
-    return call_proc_df_in_out(proc='IMPUTE_DATA', in_df=in_df, params=params, 
-        out_table=out_table, copy_indexer=True)[0]
+    return call_proc_df_in_out(proc='IMPUTE_DATA', in_df=in_df, params=params,
+                               out_table=out_table, copy_indexer=True)[0]
 
 
-def random_sample(in_df: IdaDataFrame, size: int=None, fraction: float=None, by_column: str=None,
-    out_signature: str=None, rand_seed: int=None, out_table: str=None) -> IdaDataFrame:
+def random_sample(in_df: IdaDataFrame, size: int = None, fraction: float = None, by_column: str = None,
+                  out_signature: str = None, rand_seed: int = None, out_table: str = None) -> IdaDataFrame:
     """
     Random sampling procedures are a vital component of many analytical systems. They can
     be used to select a test sample and a training sample for a model building process
     (machine learning). They can also be used to get a smaller sample of the training
     set, which you may do because of learning algorithm complexity considerations.
     In both cases, you would sample without replacement.
 
     Another application of sampling is the learning methods based on bootstrapping.
     This requires many independent samples from the same data, which are preferentially
     applied if the available data sets are small or for other reasons where the sample
     independence is vital. Samples with replacement are usually drawn in this case.
-    
+
     In application, sampling is used for promotion campaigns, for example when you want
     only a representative set of customers to be subjects of an action.
     In all cases, whether for use with scientific methods or business practices, uniform
     sampling is important.
 
     This function creates a random sample of a data frame a fixed size or a fixed
     probability and returns the result in a new data frame.
@@ -186,8 +187,101 @@
         'size': size,
         'fraction': fraction,
         'by': by_column,
         'outsignature': out_signature,
         'randseed': rand_seed
     }
     return call_proc_df_in_out(proc='RANDOM_SAMPLE', in_df=in_df, params=params,
-        out_table=out_table, copy_indexer=True)[0]
+                               out_table=out_table, copy_indexer=True)[0]
+
+
+def train_test_split(in_df: IdaDataFrame, out_table_train: str=None, out_table_test: str=None,
+                     id_column: str = None, fraction: float = 0.5, rand_seed: float = None,
+                     out_table_type: str = 'table') -> Tuple[IdaDataFrame, IdaDataFrame]:
+    """
+    Parameters
+    ----------
+    in_df : IdaDataFrame
+        the input data frame
+
+    out_table_train : str, optional
+        the name of output dataframe that will contain the given fraction of the input records
+
+    out_table_test : str, optional
+        the name of output dataframe that will contain the rest (1-<fraction>) of the input records
+
+    id_column: str, optional
+        the input dataframe column identifying a unique instance id
+
+    fraction : float, optional
+        the fraction of the data to that goes to the training dataframe
+
+    rand_seed : int, optional
+        the seed of the random function
+
+    out_table_type : str, optional
+        the type of the output tables. It can be 'table' or 'temporary'
+
+    Returns
+    -------
+    IdaDataFrame
+        the data frame with train data
+    
+    IdaDataFrame
+        the data frame with test data
+    """
+    
+    if not isinstance(in_df, IdaDataFrame):
+        raise TypeError("Argument in_df should be an IdaDataFrame")
+    
+    if not id_column:
+        if not in_df.indexer:
+            raise ValueError("If dataframe has no indexer 'id_column' has to be provided")
+        else:
+            id_column = in_df.indexer
+    temp_view_name, need_delete = materialize_df(in_df)
+    
+    auto_delete_context = None
+    if not out_table_train:
+        auto_delete_context = get_auto_delete_context('out_table_train')
+        out_table_train = make_temp_table_name()
+
+    if not out_table_test:
+        auto_delete_context = get_auto_delete_context('out_table_test')
+        out_table_test = make_temp_table_name()
+
+    params = {
+        'intable': temp_view_name,
+        'traintable': out_table_train,
+        'testtable': out_table_test,
+        'id': id_column,
+        'fraction': fraction,
+        'outtabletype': out_table_type,
+    }
+
+    if isinstance(rand_seed, float):
+        params['seed'] = rand_seed
+
+    params_s = map_to_props(params)
+
+    try:
+        in_df.ida_query(f'call NZA..SPLIT_DATA(\'{params_s}\')')
+    finally:
+        if need_delete:
+            in_df._idadb.drop_view(temp_view_name)
+
+    if not in_df._idadb.exists_table_or_view(out_table_train) or \
+       not in_df._idadb.exists_table_or_view(out_table_test):
+        # stored procedure call was successful by did not produce a table
+        return None, None
+
+    if auto_delete_context:
+        auto_delete_context.add_table_to_delete(out_table_train)
+        auto_delete_context.add_table_to_delete(out_table_test)
+
+    out_df_train = IdaDataFrame(in_df._idadb, out_table_train)
+    out_df_test = IdaDataFrame(in_df._idadb, out_table_test)
+    
+    if in_df.indexer:
+        out_df_train.indexer = in_df.indexer
+        out_df_test.indexer = in_df.indexer
+    return out_df_train, out_df_test
```

### Comparing `nzpyida-0.3.5/nzpyida/analytics/utils.py` & `nzpyida-0.3.6/nzpyida/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/base.py` & `nzpyida-0.3.6/nzpyida/base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/exceptions.py` & `nzpyida-0.3.6/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/__init__.py` & `nzpyida-0.3.6/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.3.6/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/entropy.py` & `nzpyida-0.3.6/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.3.6/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/gini.py` & `nzpyida-0.3.6/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.3.6/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/private.py` & `nzpyida-0.3.6/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.3.6/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/feature_selection/tstats.py` & `nzpyida-0.3.6/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/filtering.py` & `nzpyida-0.3.6/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/frame.py` & `nzpyida-0.3.6/nzpyida/frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/indexing.py` & `nzpyida-0.3.6/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/internals.py` & `nzpyida-0.3.6/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/__init__.py` & `nzpyida-0.3.6/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/iris.py` & `nzpyida-0.3.6/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/iris.txt` & `nzpyida-0.3.6/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/swiss.py` & `nzpyida-0.3.6/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/swiss.txt` & `nzpyida-0.3.6/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/titanic.py` & `nzpyida-0.3.6/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sampledata/titanic.txt` & `nzpyida-0.3.6/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/series.py` & `nzpyida-0.3.6/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/sql.py` & `nzpyida-0.3.6/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/statistics.py` & `nzpyida-0.3.6/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/conftest.py` & `nzpyida-0.3.6/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_aggregation.py` & `nzpyida-0.3.6/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_association_rules.py` & `nzpyida-0.3.6/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_base.py` & `nzpyida-0.3.6/nzpyida/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.3.6/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_base_private.py` & `nzpyida-0.3.6/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.3.6/nzpyida/tests/test_base_table_manipulation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.3.6/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_filtering.py` & `nzpyida-0.3.6/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_frame.py` & `nzpyida-0.3.6/nzpyida/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.3.6/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_frame_private.py` & `nzpyida-0.3.6/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_geoFrame.py` & `nzpyida-0.3.6/nzpyida/tests/test_geoFrame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_geoSeries.py` & `nzpyida-0.3.6/nzpyida/tests/test_geoSeries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_indexing.py` & `nzpyida-0.3.6/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_internals.py` & `nzpyida-0.3.6/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_kmeans.py` & `nzpyida-0.3.6/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.3.6/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_series.py` & `nzpyida-0.3.6/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_sorting.py` & `nzpyida-0.3.6/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_statistics.py` & `nzpyida-0.3.6/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/tests/test_utils.py` & `nzpyida-0.3.6/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida/utils.py` & `nzpyida-0.3.6/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.5/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.3.6/nzpyida.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.5
+Version: 0.3.6
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.3.5/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.3.6/nzpyida.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 nzpyida/analytics/predictive/regression_trees.py
 nzpyida/analytics/predictive/timeseries.py
 nzpyida/analytics/predictive/two_step_clustering.py
 nzpyida/analytics/tests/conftest.py
 nzpyida/analytics/tests/test_association_rules.py
 nzpyida/analytics/tests/test_auto_delete_context.py
 nzpyida/analytics/tests/test_bisecting_kmeans.py
+nzpyida/analytics/tests/test_cross_validation.py
 nzpyida/analytics/tests/test_decision_trees.py
 nzpyida/analytics/tests/test_discretization.py
 nzpyida/analytics/tests/test_glm.py
 nzpyida/analytics/tests/test_kmeans.py
 nzpyida/analytics/tests/test_knn.py
 nzpyida/analytics/tests/test_linear_regression.py
 nzpyida/analytics/tests/test_model_manager.py
```

### Comparing `nzpyida-0.3.5/setup.py` & `nzpyida-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
       ]
 
 setup(name='nzpyida',
-      version='0.3.5',
+      version='0.3.6',
       install_requires=['pandas','numpy','future','six','pypyodbc','pyodbc', 'lazy', 'nzpy'],
 
       extras_require={
         'jdbc':['JayDeBeApi==1.*', 'Jpype1==0.6.3'],
         'test':['pytest', 'flaky==3.4.0'],
         'doc':['sphinx', 'ipython', 'numpydoc', 'sphinx_rtd_theme']
       },
```


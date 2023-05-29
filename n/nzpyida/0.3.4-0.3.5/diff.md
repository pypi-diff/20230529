# Comparing `tmp/nzpyida-0.3.4.tar.gz` & `tmp/nzpyida-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.3.4.tar", last modified: Tue May 16 10:00:38 2023, max compression
+gzip compressed data, was "nzpyida-0.3.5.tar", last modified: Mon May 29 14:02:59 2023, max compression
```

## Comparing `nzpyida-0.3.4.tar` & `nzpyida-0.3.5.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.307392 nzpyida-0.3.4/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.4/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.4/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.4/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     4782 2023-05-16 10:00:38.307485 nzpyida-0.3.4/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3265 2023-05-10 12:49:36.000000 nzpyida-0.3.4/README.md
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.280148 nzpyida-0.3.4/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.4/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.284391 nzpyida-0.3.4/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.4/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.4/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2453 2023-05-16 09:58:38.000000 nzpyida-0.3.4/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.286975 nzpyida-0.3.4/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.4/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.289718 nzpyida-0.3.4/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.290947 nzpyida-0.3.4/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.291111 nzpyida-0.3.4/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.291965 nzpyida-0.3.4/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     1642 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2529 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.292476 nzpyida-0.3.4/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.294825 nzpyida-0.3.4/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     9919 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     6581 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    10454 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8700 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12287 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.298099 nzpyida-0.3.4/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     1896 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3552 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     2393 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.298725 nzpyida-0.3.4/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     7634 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93174 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.300788 nzpyida-0.3.4/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      957 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     7631 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/correlation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5517 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/discretize.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.4/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.302548 nzpyida-0.3.4/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.307229 nzpyida-0.3.4/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.4/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.4/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23587 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.4/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.4/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.288162 nzpyida-0.3.4/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     4782 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4735 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-16 10:00:38.307787 nzpyida-0.3.4/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3069 2023-05-16 09:46:30.000000 nzpyida-0.3.4/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.696948 nzpyida-0.3.5/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.5/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.5/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.5/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:02:59.697030 nzpyida-0.3.5/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.3.5/README.md
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.664654 nzpyida-0.3.5/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.5/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.668240 nzpyida-0.3.5/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.5/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geoFrame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geoSeries.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.5/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2638 2023-05-25 14:48:09.000000 nzpyida-0.3.5/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.5/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.672110 nzpyida-0.3.5/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.5/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.675061 nzpyida-0.3.5/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.677029 nzpyida-0.3.5/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.677338 nzpyida-0.3.5/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.678429 nzpyida-0.3.5/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     1815 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.3.5/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.679077 nzpyida-0.3.5/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.682616 nzpyida-0.3.5/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11482 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6581 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9450 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10920 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8852 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12701 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.686917 nzpyida-0.3.5/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     3561 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-05-17 10:45:26.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4035 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2393 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.687664 nzpyida-0.3.5/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7634 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93282 2023-05-26 14:10:56.000000 nzpyida-0.3.5/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.689546 nzpyida-0.3.5/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.5/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.691345 nzpyida-0.3.5/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-25 14:47:30.000000 nzpyida-0.3.5/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.696706 nzpyida-0.3.5/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.5/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.5/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-05-25 14:48:09.000000 nzpyida-0.3.5/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.5/nzpyida/tests/test_geoFrame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.5/nzpyida/tests/test_geoSeries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.5/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-29 14:02:59.673059 nzpyida-0.3.5/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4726 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-29 14:02:59.000000 nzpyida-0.3.5/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-29 14:02:59.697302 nzpyida-0.3.5/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3318 2023-05-25 07:54:36.000000 nzpyida-0.3.5/setup.py
```

### Comparing `nzpyida-0.3.4/LICENSE.txt` & `nzpyida-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/PKG-INFO` & `nzpyida-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.4
+Version: 0.3.5
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
+Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
+Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/IBM/nzpyida
+Project-URL: Tracker, https://github.com/IBM/nzpyida/issues
 Keywords: data analytics database development ibm netezza pandas scikitlearn scalability machine-learning knowledge discovery
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -126,7 +130,14 @@
     petal_length      0.871754    -0.428440      1.000000     0.962865
     petal_width       0.817941    -0.366126      0.962865     1.000000
 
 # Contributors
 
 The nzpyida is based on ibmdbpy project developed for IBM Db2 Warehouse.
 See https://github.com/ibmdbanalytics/ibmdbpy for details.
+
+# How to contribute
+You want to contribute? That's great! There are many things you can do.
+
+If you are a member of the ibmdbanalytics group, you can create branchs and merge them to master. Otherwise, you can fork the project and do a pull request. You are very welcome to contribute to the code and to the documentation.
+
+There are many ways to contribute. If you find bugs and have improvement ideas or need some new specific features, please open a ticket! We do care about it.
```

### Comparing `nzpyida-0.3.4/README.md` & `nzpyida-0.3.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -90,7 +90,14 @@
     petal_length      0.871754    -0.428440      1.000000     0.962865
     petal_width       0.817941    -0.366126      0.962865     1.000000
 
 # Contributors
 
 The nzpyida is based on ibmdbpy project developed for IBM Db2 Warehouse.
 See https://github.com/ibmdbanalytics/ibmdbpy for details.
+
+# How to contribute
+You want to contribute? That's great! There are many things you can do.
+
+If you are a member of the ibmdbanalytics group, you can create branchs and merge them to master. Otherwise, you can fork the project and do a pull request. You are very welcome to contribute to the code and to the documentation.
+
+There are many ways to contribute. If you find bugs and have improvement ideas or need some new specific features, please open a ticket! We do care about it.
```

### Comparing `nzpyida-0.3.4/docs/.DS_Store` & `nzpyida-0.3.5/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/Makefile` & `nzpyida-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/make.bat` & `nzpyida-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/base.rst` & `nzpyida-0.3.5/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/conf.py` & `nzpyida-0.3.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/frame.rst` & `nzpyida-0.3.5/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/geoFrame.rst` & `nzpyida-0.3.5/docs/source/geoFrame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/geoSeries.rst` & `nzpyida-0.3.5/docs/source/geoSeries.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/geospatial.rst` & `nzpyida-0.3.5/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/ibm.png` & `nzpyida-0.3.5/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/index.rst` & `nzpyida-0.3.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/install.rst` & `nzpyida-0.3.5/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/kc.ico` & `nzpyida-0.3.5/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/legal.rst` & `nzpyida-0.3.5/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/predictive.rst` & `nzpyida-0.3.5/docs/source/predictive.rst`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,22 @@
 -----------------------------------------------------
 
 .. automodule:: nzpyida.analytics.predictive.timeseries
    :members:
    :undoc-members:
    :show-inheritance:
 
+Generalized Linear Models
+-----------------------------------------------------
+
+.. automodule:: nzpyida.analytics.predictive.glm
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Classification base module
 --------------------------------------------------
 
 .. automodule:: nzpyida.analytics.predictive.classification
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `nzpyida-0.3.4/docs/source/start.rst` & `nzpyida-0.3.5/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/docs/source/utils.rst` & `nzpyida-0.3.5/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/__init__.py` & `nzpyida-0.3.5/nzpyida/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/__init__.py` & `nzpyida-0.3.5/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/apply.py` & `nzpyida-0.3.5/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.3.5/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/groupedapply.py` & `nzpyida-0.3.5/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/install.py` & `nzpyida-0.3.5/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/result_builder.py` & `nzpyida-0.3.5/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/shaper.py` & `nzpyida-0.3.5/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/tapply.py` & `nzpyida-0.3.5/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/tapply_class.py` & `nzpyida-0.3.5/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.3.5/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/aggregation.py` & `nzpyida-0.3.5/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/__init__.py` & `nzpyida-0.3.5/nzpyida/analytics/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from .predictive.linear_regression import LinearRegression
 from .predictive.naive_bayes import NaiveBayesClassifier
 from .predictive.association_rules import ARule
 from .predictive.bisecting_kmeans import BisectingKMeans
 from .predictive.regression_trees import DecisionTreeRegressor
 from .predictive.two_step_clustering import TwoStepClustering
 from .predictive.timeseries import TimeSeries
+from .predictive.glm import BernoulliRegressor, BinomialRegressor, \
+    NegativeBinomialRegressor, GaussianRegressor, GammaRegressor, \
+    PoissonRegressor, WaldRegressor
 from .exploration.distribution import bitable, moments, histogram, outliers
 from .exploration.distribution import quantile, unitable
 from .transform.discretization import EFDisc, EMDisc, EWDisc
 from .transform.discretization import ef_disc, em_disc, ew_disc
 from .transform.preparation import std_norm, impute_data, random_sample
 from .model_manager import ModelManager
 from .auto_delete_context import AutoDeleteContext
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.3.5/nzpyida/analytics/auto_delete_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,40 +38,37 @@
 
         Returns
         -------
         AutoDeleteContext
             the current thread AutoDeleteContext or None
         """
 
-        if getattr(AutoDeleteContext.active_group, 'auto_delete_context', False):
-            return AutoDeleteContext.active_group.auto_delete_context
+        if getattr(AutoDeleteContext.active_group, 'auto_delete_context_st', False) and \
+            AutoDeleteContext.active_group.auto_delete_context_st:
+            return AutoDeleteContext.active_group.auto_delete_context_st[-1]
         return None
 
     def add_table_to_delete(self, table_name: str):
         """
         Register a table to be deleted when this context exits.
 
         Parameters
         ----------
         table_name : str
             the table name
         """
         self.temp_out_tables.add(table_name)
 
     def __enter__(self):
-        if getattr(AutoDeleteContext.active_group, 'auto_delete_context', False):
-            AutoDeleteContext.active_group.active_groups += 1
-            return AutoDeleteContext.active_group.auto_delete_context
-        AutoDeleteContext.active_group.auto_delete_context = self
-        AutoDeleteContext.active_group.active_groups = 1
+        if not getattr(AutoDeleteContext.active_group, 'auto_delete_context_st', False):
+            AutoDeleteContext.active_group.auto_delete_context_st = []
+        AutoDeleteContext.active_group.auto_delete_context_st.append(self)
         return self
 
     def __exit__(self, ex_type, value, traceback):
-        AutoDeleteContext.active_group.active_groups -= 1
-        if AutoDeleteContext.active_group.active_groups == 0:
-            curr = AutoDeleteContext.current()
-            for table_name in curr.temp_out_tables:
-                if curr.idadb.exists_table(table_name):
-                    curr.idadb.drop_table(table_name)
-            curr.temp_out_tables = set()
-            delattr(AutoDeleteContext.active_group, 'auto_delete_context')
+        for table_name in self.temp_out_tables:
+            if self.idadb.exists_table(table_name):
+                self.idadb.drop_table(table_name)
+        self.temp_out_tables = set()
+        AutoDeleteContext.active_group.auto_delete_context_st.pop()
+
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.3.5/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.3.5/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/model_manager.py` & `nzpyida-0.3.5/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,34 @@
 
 The divisive clustering algorithm may return different results for the same data set 
 and the same random generator seed when you use different input data distribution or 
 a different number of dataslices. This is due to the behavior of the random number 
 generator, which generates random sequences depending on the number of dataslices 
 and data distribution. The algorithm returns the same model when you use the same machine, 
 the same input data distribution, and the same random seed.
+
+The cluster formation process of the divisive clustering algorithm begins with a single cluster 
+containing all training instances, then the first invocation of k-means divides it into two 
+subclusters by creating two descendant nodes of the clustering tree. Subsequent invocations 
+divide these clusters into more subclusters, and so on, until a stop criterion is satisfied. 
+Stop criterion can be specified by the maximum clustering tree depth or by the minimum required 
+umber of instances for further partitioning. The resulting hierarchical clustering tree can be 
+used to classify instances by propagating them down from the root node, and choosing at each 
+level the best matching sub-cluster with respect to the instance’s distance from sub-cluster centers.
+
+The internal k-means process of the divisive clustering algorithm operates using the ordinary 
+k-means algorithm (with the modified initial centroid generation), discussed in the K-Means 
+Clustering section, using a fixed value of k=2 and working with the subset of data from the 
+parent cluster. The initial centroid generation consists two steps: random generation n>>k 
+candidates and then selection of outermost pair of candidates. The cluster center representation 
+and distance measures remain the same. The numbering scheme for clusters in a clustering tree is 
+the same as decision trees: the root node is number 1, and the descendants of node number 'i' have 
+numbers '2i' and '2i+1' 
+
+Additionally, leaves, which are clusters with no subclusters, are designated by negative numbers.
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, make_temp_table_name
 from nzpyida.analytics.utils import get_auto_delete_context
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,22 @@
             Indicating statistics=all is equal to statistics=values:100.
 
         transform : str, optional
             flag indicating if the input table columns have to be transformed.
             Allowed values are: L (for leave as is), N (for normalization)
             or S (for standardization).
             If it is not specified, no transformation will be performed.
+        
+        Returns
+        -------
+        IdaDataFrame
+            output table with following columns: id, cluster_id, distance. The id column matches 
+            the <id_column>  of the input table. Each input table record is associated with a cluster, 
+            where the distance from the record to the cluster center is the smallest. The cluster ID 
+            and the distance to the cluster center are given in the columns cluster_id and distance
 
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
 
         if not id_column:
             if in_df.indexer:
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/timeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 """
-A time series model is built by analyzing series of timed numeric values, and is 
-applied immediately for predicting future values. The model itself is stored but 
-not really needed any more (except for understanding the predicted values).
 
-If specified, a table <outtable> is additionally created with the following columns: 
-<by>, <time>, forecast, standarderror. The table contains the forecast values for 
-future time points of the time series identified by <by>. For each prediction, 
-the standarderror value indicates a confidence interval around the forecast value.
+Many types of business-relevant or scientific data have values that change over time. 
+Some typical examples are:
+- Daily sales figures for a store
+- Energy consumption readings from household electric meters 
+- Price per gallon at a local gas station
+It is often useful to analyze the behavior of such changes, both to describe the development 
+over time, specifically for a particular trend and seasonality, as well as to predict unknown 
+values of the series, usually for the future. A typical area of application is supply chain
+management, where future needs may be predicted based on past trends.
 
-If specified, a table <seasadjtable> is additionally created with the following columns: 
-<by>, <time>, adjusted. The values in column <target> of the input table are seasonally 
-adjusted and then copied into this table, with the values of columns <by> and <time>
+A time series is a sequence of numerical data values, measured at successive, but not necessarily 
+equidistant—points in time. Examples are daily stock prices, monthly unemployment counts, 
+or annual changes in global temperature. The two main goals of time series analysis are to 
+understand the underlying patterns which are represented by the observed data and to make forecasts.
 """
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.predictive.predictive_modeling import PredictiveModeling
 from nzpyida.analytics.utils import call_proc_df_in_out
 from nzpyida.analytics.model_manager import ModelManager
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.3.5/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,32 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 """
-The divisive clustering algorithm is a computationally efficient, top-down approach 
-to creating hierarchical clustering models. Conceptually, it can be thought of as 
-a wrapper around the k -means algorithm (with a specialized method for initial centroid setting), 
-running the algorithm several times to divide clusters into subclusters. 
-The internal k-means algorithm assumes a fixed k =2 value.
+TwoStep clustering is a data mining algorithm for large data sets. It is faster than 
+traditional methods because it typically scans a data set only once before it saves 
+the data to a clustering feature (CF) tree. TwoStep clustering can make clustering 
+decisions without repeated data scans, whereas other clustering methods scan all 
+data points, which requires multiple iterations. Non- uniform points are not gathered, 
+so each iteration requires a reinspection of each data point, regardless of the 
+significance of the data point. Because TwoStep clustering treats dense areas 
+as a single unit and ignores pattern outliers, it provides high-quality clustering 
+results without exceeding memory constraints.
 
-The divisive clustering algorithm may return different results for the same data set 
-and the same random generator seed when you use different input data distribution or 
-a different number of dataslices. This is due to the behavior of the random number 
-generator, which generates random sequences depending on the number of dataslices 
-and data distribution. The algorithm returns the same model when you use the same machine, 
-the same input data distribution, and the same random seed.
+The TwoStep algorithm has the following advantages:
+- It automatically determines the optimal number of clusters. You do not have to 
+manually create a different clustering model for each number of clusters.
+- It detects input columns that are not useful for the clustering process. 
+These columns are automatically set to supplementary. Statistics are gathered 
+for these columns but they do not influence the clustering algorithm.
+- The configuration of the CF tree can be granular, so that you can balance between 
+memory usage and model quality, according to the environment and needs.
 """
 
 from typing import List
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.utils import map_to_props, make_temp_table_name
 from nzpyida.analytics.utils import get_auto_delete_context
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,17 @@
         with AutoDeleteContext(idadb) as adc:
             pass
         assert not adc.current()
 
     def test_nested_contexts(self, idadb):
         with AutoDeleteContext(idadb) as adc1:
             with AutoDeleteContext(idadb) as adc2:
-                assert adc1 == adc2
+                assert adc1 != adc2
+                assert adc2 == AutoDeleteContext.current()
+            assert adc1 == AutoDeleteContext.current()
 
 
 class TestAddTableToDelete:
     def test_table_not_deleted(self, idadb, create_test_table):
         with AutoDeleteContext(idadb) as adc:
             df = IdaDataFrame(idadb, 'TEST_TABLE')
             adc.add_table_to_delete('TEST_TABLE')
```

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.3.5/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.3.5/nzpyida/analytics/transform/discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.3.5/nzpyida/analytics/transform/preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/analytics/utils.py` & `nzpyida-0.3.5/nzpyida/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/base.py` & `nzpyida-0.3.5/nzpyida/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,16 @@
         if isinstance(dsn,str):
             if dsn.startswith('jdbc:'):
               self._con_type = "jdbc"
               if dsn.startswith('jdbc:netezza:'):
                   self._database_system = 'netezza'
                   # for Netezza the internal connection is always in autocommit mode
                   # to allow explicit commits
-                  dsn += ';autocommit=false'
+                  if not autocommit:
+                    dsn += ';autocommit=false'
                   url_1stparam_del = ';'
               elif dsn.startswith('jdbc:db2:'):
                   self._database_system = 'db2'
               else:
                   raise IdaDataBaseError(("The JDBC connection string is invalid for Db2 and Netezza. " +
                                           "It has to start either with 'jdbc:db2:' or 'jdbc:netezza:'."))
 
@@ -303,14 +304,15 @@
                 self._con = nzpy.connect(user=user, password=password,host=host, port=port,
                                         database=database, securityLevel=securityLevel,logLevel=logLevel)
             except Exception as e:
                 raise IdaDataBaseError(str(e))
             self._connection_string ={'user':user,'password':password,'host':host,
                 'port':port, 'database':database, 'securityLevel':securityLevel,'logLevel':logLevel}
             self._database_system = 'netezza'
+            self._con.autocommit = autocommit
 
         if self._con_type == 'odbc' :
 
             self._connection_string = "DSN=%s; UID=%s; PWD=%s;LONGDATACOMPAT=1;"%(dsn,uid,pwd)
             """
             Workaround for CLOB retrieval: 
             Set the CLI/ODBC LongDataCompat keyword to 1. 
@@ -319,15 +321,15 @@
             SQL_CLOB to SQL_LONGVARCHAR
             SQL_BLOB to SQL_LONGVARBINARY
             SQL_DBCLOB to SQL_WLONGVARCHAR
             """
 
             import pyodbc
             try:
-                self._con = pyodbc.connect(self._connection_string)
+                self._con = pyodbc.connect(self._connection_string, autocommit=autocommit)
                 self._con.setdecoding(pyodbc.SQL_CHAR, encoding='utf-8')
                 self._con.setdecoding(pyodbc.SQL_WCHAR, encoding='utf-8')
                 self._con.setencoding(encoding='utf-8')
             except Exception as e:
                 raise IdaDataBaseError(str(e))
             try:
                 self.ida_query("select count(*) from _V_OBJECT")
```

### Comparing `nzpyida-0.3.4/nzpyida/exceptions.py` & `nzpyida-0.3.5/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/__init__.py` & `nzpyida-0.3.5/nzpyida/feature_selection/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,23 +12,20 @@
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
 
-from .correlation import  pearson, spearman
-
 from .entropy import entropy, entropy_stats
 
 from .info_gain import info_gain
 
 from .gain_ratio import gain_ratio
 
 from .symmetric_uncertainty import su
 
 from .gini import gini, gini_pairwise
-from .discretize import discretize
 
 from .chisquared import chisquared
 from .tstats import ttest
```

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.3.5/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/correlation.py` & `nzpyida-0.3.5/nzpyida/feature_selection/gini.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,221 +1,178 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
-# All rights reserved.
-#
-# Distributed under the terms of the BSD Simplified License.
-#
-# The full license is in the LICENSE file, distributed with this software.
-#-----------------------------------------------------------------------------
+"""
+Created on Tue Dec  1 12:29:30 2015
 
+@author: efouche
+"""
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
-from collections import OrderedDict
 
-import nzpyida
-from nzpyida.internals import idadf_state
-from nzpyida.utils import timed, chunklist
+
+from collections import OrderedDict
 
 import pandas as pd
+import numpy as np
+import six
 
+from nzpyida.internals import idadf_state
+from nzpyida.utils import timed
 from nzpyida.feature_selection.private import _check_input
 
-
 @idadf_state
 @timed
-def pearson(idadf, target=None, features=None, ignore_indexer=True):
+def gini_pairwise(idadf, target=None, features=None, ignore_indexer=True):
     """
-    Compute the pearson correlation coefficients between a set of features and a 
-    set of target in an IdaDataFrame. Provide more granualirity than 
-    IdaDataFrame.corr
+    Compute the conditional gini coefficients between a set of features and a 
+    set of target in an IdaDataFrame. 
     
     Parameters
     ----------
     idadf : IdaDataFrame
     
     target : str or list of str, optional
         A column or list of columns against to be used as target. Per default, 
         consider all columns
     
     features : str or list of str, optional
         A column or list of columns to be used as features. Per default, 
         consider all columns. 
-        
+    
     ignore_indexer : bool, default: True
         Per default, ignore the column declared as indexer in idadf
         
     Returns
     -------
     Pandas.DataFrame or Pandas.Series if only one target
     
     Notes
     -----
-    Input columns as target and features should be numerical. 
+    Input columns as target and features should be categorical, otherwise 
+    this measure does not make much sense. 
     
     Examples
     --------
     >>> idadf = IdaDataFrame(idadb, "IRIS")
-    >>> pearson(idadf)
+    >>> gini_pairwise(idadf)
     """
-    # check if the corr function is installed on the Netezza system
-    if idadf._idadb._is_netezza_system():
-        corr_query = "SELECT count(*) from _V_OBJECT  where OBJNAME like 'CORR#%' AND OBJDB = CURRENT_DB"
-        if idadf._idadb.ida_scalar_query(corr_query) == 0:
-            raise NotImplementedError("The CORR function is not installed on the Netezza database.")
-
-
-    numerical_columns = idadf._get_numerical_columns()
-    if features is None:
-        features = numerical_columns
-        
+    # Check input
     target, features = _check_input(idadf, target, features, ignore_indexer)
-    
-    value_dict = OrderedDict()
-    
-    for feature in features:
-        if feature not in numerical_columns:
-            raise TypeError("Correlation-based measure not available for non-numerical column %s"%feature)
-                    
-    if target == features:
-        return idadf.corr(features = features, ignore_indexer=ignore_indexer)
-    else:
-        for t in target:
-            if feature not in numerical_columns:
-                raise TypeError("Correlation-based measure not available for non-numerical column %s"%t)
         
-        for t in target:
-            value_dict[t] = OrderedDict()
-            
-            features_notarget = [x for x in features if x != t]
+    gini_dict = OrderedDict()
+    length = len(idadf)
 
-            if idadf._idadb._is_netezza_system():
-                corr_funct = "CORR"
-            else:
-                corr_funct = "CORRELATION"
-
-            if len(features_notarget) < 64:
-                agg_list = ["%s(\"%s\",\"%s\")"%(corr_funct, x, t) for x in features_notarget]
-                agg_string = ', '.join(agg_list)
-                name = idadf.internal_state.current_state
-                data = idadf.ida_query("SELECT %s FROM %s"%(agg_string, name), first_row_only = True)
-            else:
-                chunkgen = chunklist(features_notarget, 100)
-                data = ()
-                for chunk in chunkgen: 
-                    agg_list = ["%s(\"%s\",\"%s\")"%(corr_funct, x, t) for x in chunk]
-                    agg_string = ', '.join(agg_list)
+    if idadf._idadb._is_netezza_system():
+        power_function = "POW"
+        div_term = "* POW(c,-1)) * POW(%s,-1)"%length
+    else:
+        power_function = "POWER"
+        div_term = "/c)/%s"%length
+
+    for t in target:
+        gini_dict[t] = OrderedDict() 
+        features_notarget = [x for x in features if (x != t)]
+        
+        for feature in features_notarget:
+            if t not in gini_dict:
+                gini_dict[t] = OrderedDict()
             
-                    name = idadf.internal_state.current_state
-                    data += idadf.ida_query("SELECT %s FROM %s"%(agg_string, name), first_row_only = True)
-    
-            for i, feature in enumerate(features_notarget):
-                value_dict[t][feature] = data[i]
-        
-        ### Fill the matrix
-        result = pd.DataFrame(value_dict).fillna(1)
+            query = ("SELECT SUM((%s(c,2) - gini)%s FROM "+
+            "(SELECT SUM(%s(count,2)) as gini, SUM(count) as c FROM "+
+            "(SELECT CAST(COUNT(*) AS FLOAT) AS count, \"%s\" FROM %s GROUP BY \"%s\",\"%s\") AS T1 "+
+            "GROUP BY \"%s\") AS T2 ")
+            query0 = query%(power_function, div_term, power_function, feature, idadf.name, t, feature, feature)
+            gini_dict[t][feature] = idadf.ida_scalar_query(query0)
+            
+    result = pd.DataFrame(gini_dict).fillna(np.nan)
         
-        if len(result.columns) == 1:
-            if len(result) == 1:
-                result = result.iloc[0,0]
-            else:
-                result = result[result.columns[0]].copy()
-                result.sort_values(inplace=True, ascending=False)
+    if len(result.columns) > 1:
+        order = [x for x in result.columns if x in features] + [x for x in features if x not in result.columns]
+        result = result.reindex(order)
+       
+    result = result.dropna(axis=1, how="all")
+    
+    if len(result.columns) == 1:
+        if len(result) == 1:
+            result = result.iloc[0,0]
         else:
-            order = [x for x in result.columns if x in features] + [x for x in features if x not in result.columns]
-            result = result.reindex(order)
+            result = result[result.columns[0]].copy()
+            result.sort_values(ascending = True)
+    else:
+        result = result.fillna(0)
+    
+    return result
+               
+    
         
-        return result 
-  
+    
+    
+    
 @idadf_state
-@timed          
-def spearman(idadf, target=None, features = None, ignore_indexer=True):
+@timed
+def gini(idadf, features=None, ignore_indexer=True):
     """
-    Compute the spearman rho correlation coefficients between a set of features 
-    and a set of target in an IdaDataFrame.
+    Compute the gini coefficients for a set of features in an IdaDataFrame. 
     
     Parameters
     ----------
     idadf : IdaDataFrame
     
-    target : str or list of str, optional
-        A column or list of columns against to be used as target. Per default, 
-        consider all columns
-    
     features : str or list of str, optional
         A column or list of columns to be used as features. Per default, 
         consider all columns. 
-        
+    
     ignore_indexer : bool, default: True
         Per default, ignore the column declared as indexer in idadf
         
     Returns
     -------
-    Pandas.DataFrame or Pandas.Series if only one target
+    Pandas.Series
     
     Notes
     -----
-    Input columns as target and features should be numerical. 
-    This function is a wrapper for pearson. 
-    The scalability of this approach is not very good. Should not be used on 
-    high dimensional data. 
+    Input column should be categorical, otherwise this measure does not make 
+    much sense. 
     
     Examples
     --------
     >>> idadf = IdaDataFrame(idadb, "IRIS")
-    >>> spearman(idadf)
+    >>> gini(idadf)
     """
-    numerical_columns = idadf._get_numerical_columns()
     if features is None:
-        features = numerical_columns
-        
-    target, features = _check_input(idadf, target, features, ignore_indexer)
-    
-    for feature in features:
-        if feature not in numerical_columns:
-            raise TypeError("Correlation-based measure not available for non-numerical column %s"%feature)
-    
+        features = list(idadf.columns)
+    else:
+        if isinstance(features, six.string_types):
+            features = [features]
+
     if ignore_indexer is True:
         if idadf.indexer:
-            if idadf.indexer in numerical_columns:
+            if idadf.indexer in features:
                 features.remove(idadf.indexer)
-    
-    if features is None:
-        features = list(idadf.columns)
-    
-    numerical_features = [x for x in features if x in numerical_columns]
-    numerical_targets = [x for x in target if x in numerical_columns]
-    
-    numerical_features = list(set(numerical_features) | set(numerical_targets))
-    
-    
-    agg_list = ["CAST(RANK() OVER (ORDER BY \"%s\") AS INTEGER) AS \"%s_RANK\""%(x, x) for x in numerical_features]
-    agg_string = ', '.join(agg_list)
-    subselect_stmt = "SELECT %s FROM %s"%(agg_string, idadf.name)
-
-    select_list = ["\"%s_RANK\" AS \"%s\""%(x, x) for x in numerical_features]
-    select_string = ', '.join(select_list)
-    select_stmt = "SELECT " + select_string + " FROM ( " + subselect_stmt + ") AS T"
-
-    viewname = idadf._idadb._create_view_from_expression(select_stmt)
-    
-    try:
-        idadf_rank = nzpyida.IdaDataFrame(idadf._idadb, viewname)
-        return pearson(idadf_rank, target = target, features=numerical_features, ignore_indexer=ignore_indexer)
-    except:
-        raise
-    finally:
-        idadf._idadb.drop_view(viewname)
-    
-    
-    
-    
- 
+      
         
+    value_dict = OrderedDict()
         
+    length = len(idadf)**2
 
-        
+    if idadf._idadb._is_netezza_system():
+      power_function = "POW"
+      div_term = "* POW(%s, -1)"%length
+    else:
+      power_function = "POWER"
+      div_term ="/%s"%length
+
+    for feature in features:
+        
+        subquery = "SELECT COUNT(*) AS count FROM %s GROUP BY \"%s\""%(idadf.name, feature)
+        query = "SELECT (%s - SUM(%s(count,2)))%s FROM (%s) AS T "%(length, power_function, div_term, subquery)
+        value_dict[feature] = idadf.ida_scalar_query(query)
+            
+        if len(features) > 1:
+            result = pd.Series(value_dict) 
+        else:
+            result = value_dict[feature]
+    
+    return result
```

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/discretize.py` & `nzpyida-0.3.5/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,158 +1,157 @@
 # -*- coding: utf-8 -*-
 """
-Created on Mon Nov 23 09:02:30 2015
+Created on Mon Nov 23 09:53:19 2015
 
 @author: efouche
 """
+from __future__ import division
 from __future__ import unicode_literals
 from __future__ import print_function
-from __future__ import division
 from __future__ import absolute_import
+from builtins import dict
 from future import standard_library
 standard_library.install_aliases()
 
-from nzpyida.internals import idadf_state
+from collections import OrderedDict
+
 import nzpyida
+
+from nzpyida.feature_selection import entropy
+from nzpyida.feature_selection.private import _check_input
+
+from nzpyida.internals import idadf_state
 from nzpyida.utils import timed
 
-import six
+import pandas as pd
+import numpy as np
 
+@idadf_state
 @timed
-@idadf_state(force = True)   
-def discretize(idadf, columns = None, disc= "em", target = None, bins = None, outtable = None, clear_existing=False):
+def su(idadf, target = None, features = None, ignore_indexer=True):
     """
-    Discretize a set of numerical columns from an IdaDataFrame and returns an 
-    IdaDataFrame open on the discretized version of the dataset. 
+    Compute the symmetric uncertainty coefficients between a set of features
+    and a set of target in an IdaDataFrame. 
     
     Parameters
     ----------
     idadf : IdaDataFrame
     
-    columns : str or list of str, optional
-        A column or list of columns to be discretized
-    
-    disc : "ef", "em", "ew", "ewn" default: "em"
-        Discretization method to be used
-        
-        - ef: Discretization bins of equal frequency 
-        
-        - em: Discretization bins of minimal entropy 
-        
-        - ew: Discretization bins of equal width
-        
-        - ewn: Discretization bins of equal width with human-friendly limits 
-    
-    target : str
-        Target column again which the discretization will be done. Relevant
-        only for "em" discretization. 
-        
-    bins: int, optional
-        Number of bins. Not relevant for "em" discretization. 
-        
-    outtable: str, optional
-        The name of the output table where the assigned clusters are stored.
-        If this parameter is not specified, it is generated automatically.
-        If the parameter corresponds to an existing table in the database,
-        it is replaced.
-    
-    clear_existing: bool, default: False
-        If set to True, a table will be replaced when a table with the same 
-        name already exists  in the database.
+    target : str or list of str, optional
+        A column or list of columns against to be used as target. Per default, 
+        consider all columns
+    
+    features : str or list of str, optional
+        A column or list of columns to be used as features. Per default, 
+        consider all columns. 
+    
+    ignore_indexer : bool, default: True
+        Per default, ignore the column declared as indexer in idadf
+        
+    Returns
+    -------
+    Pandas.DataFrame or Pandas.Series if only one target
+    
+    Notes
+    -----
+    Input columns as target and features should be categorical, otherwise 
+    this measure does not make much sense. 
+    
+    Examples
+    --------
+    >>> idadf = IdaDataFrame(idadb, "IRIS")
+    >>> su(idadf)
     """
-    if columns is None:
-        columns = idadf._get_numerical_columns()
-        if target is not None:
-            columns = [x for x in columns if columns != target]    
-    else:
-        if isinstance(columns, six.string_types):
-                columns = [columns]
+    # Check input
+    target, features = _check_input(idadf, target, features, ignore_indexer)
                 
-    stored_proc = _check(idadf, columns, disc, target, bins, outtable)
+    entropy_dict = dict()
+    length = len(idadf)
+    corrector = np.log(length)*length
+    values = OrderedDict()
+        
+    for t in target:
+        if t not in values:
+            values[t] = OrderedDict() 
+        features_notarget = [x for x in features if (x != t)]
+        
+        for feature in features_notarget:
+            if feature not in values:
+                values[feature] = OrderedDict()
+            if t not in values[feature]:
+                if t not in entropy_dict:
+                    entropy_dict[t] = entropy(idadf, t, mode = "raw")
+                if feature not in entropy_dict:
+                    entropy_dict[feature] = entropy(idadf, feature, mode = "raw")
+                join_entropy = entropy(idadf, [t] + [feature], mode = "raw")     
+                disjoin_entropy = entropy_dict[t] + entropy_dict[feature]
+                value = (2.0*(disjoin_entropy - join_entropy + corrector)/(disjoin_entropy + corrector*2))
+                values[t][feature] = value
+                if feature in target:
+                    values[feature][t] = value
+    
+    result = pd.DataFrame(values).fillna(np.nan)
+    result = result.dropna(axis=1, how="all")
+        
+    if len(result.columns) > 1:
+        order = [x for x in result.columns if x in features] + [x for x in features if x not in result.columns]
+        result = result.reindex(order)
+    
+    if len(result.columns) == 1:
+        if len(result) == 1:
+            result = result.iloc[0,0]
+        else:
+            result = result[result.columns[0]].copy()
+            result.sort_values(ascending = True)
+    else:
+        result = result.fillna(1)
+   
+    return result
 
-    bound_outtable = idadf._idadb._get_valid_tablename('DISC_BOUNDS_%s_'%idadf.tablename)
-    intable = idadf.name   # either the table or a view on the top 
-    incolumn = "\";\"".join(columns)
+@idadf_state
+@timed
+def outer_su(idadf1, key1, idadf2, key2, target = None, features1 = None, features2 = None):
+    """
+    Compute the symmetric uncertainty coefficients between a set of features
+    and a set of target from two different IdaDataFrames on a particular key. 
     
+    This is experimental 
+    """
+    target1, features1 = _check_input(idadf1, target, features1)
+    target2, features2 = _check_input(idadf2, None, features2)
     
-    # Calculate bounds
-    idadf._idadb._call_stored_procedure(stored_proc,
-                                        outtable=bound_outtable,
-                                        intable=intable,
-                                        incolumn=incolumn,
-                                        target=target,
-                                        bins=bins)
-        
-    # Create discretized dataset
-        
-    if outtable is None:
-        disc_outtable = idadf._idadb._get_valid_tablename('DISC_%s_'%idadf.tablename)
+    if key1 not in idadf1.columns:
+        raise ValueError("%s is not a column in idadf1")
+    if key2 not in idadf2.columns:
+        raise ValueError("%s is not a column in idadf2")
+       
+    condition = "a.\"%s\" = b.\"%s\""%(key1,key2)
+    
+    if key2 in features2:
+        features2.remove(key2)
+    
+    afeaturesas = ", ".join(["a.\"%s\" as \"a.%s\" "%(feature, feature) for feature in features1])
+    bfeaturesas = ", ".join(["b.\"%s\" as \"b.%s\" "%(feature, feature) for feature in features2])
+    
+    selectlist = [afeaturesas, bfeaturesas]
+    
+    if target1 is not None:
+        atargetas = ", ".join(["a.\"%s\" as \"a.%s\" "%(tar, tar) for tar in [target1]])
+        selectlist.append(atargetas)
+        atarget = "a." + target1
     else:
-        if clear_existing is True:
-            try:
-                idadf._idadb.drop_table(outtable)
-            except:
-                pass
-        disc_outtable = outtable
+        atarget = None
+        
+    abfeatures = ["a." + feature for feature in features1] + ["b." + feature for feature in features2]
+    selectstr = ", ".join(selectlist)
+    
+    expression = "SELECT %s FROM %s as a FULL OUTER JOIN %s as b ON %s"%(selectstr, idadf1.name, idadf2.name, condition)
+    
+    viewname = idadf1._idadb._create_view_from_expression(expression)
     
     try:
-        idadf._idadb._call_stored_procedure("APPLY_DISC",
-                                            outtable=disc_outtable,
-                                            intable=intable,
-                                            btable=bound_outtable,
-                                            replace="T")
+        idadf_join = nzpyida.IdaDataFrame(idadf1._idadb, viewname)
+        return su(idadf_join, target = atarget, features = abfeatures)
     except:
         raise
     finally:
-        idadf._idadb.drop_table(bound_outtable)
-    
-    return nzpyida.IdaDataFrame(idadf._idadb, disc_outtable)
-    
-    
-def _check(idadf, columns, disc, target, bins, outtable):
-    """
-    Helper function to handle basic checks for 
-    ibmdbpy.feature_selection.discretize
-    """
-    if outtable is not None:
-        nzpyida.utils.check_tablename(outtable)
-    if bins is not None:
-        if not isinstance(bins, int):
-            raise TypeError("bins argument is not of integer type")
-            
-    if columns is not None:
-        
-        if target is not None:
-            if target in columns:
-                raise ValueError("Target in columns.")
-        unknown = []
-        for column in columns:
-            if column not in idadf.columns:
-                unknown.append(column)
-        if unknown:
-            raise ValueError("Undefined columns: %s"%", ".join(unknown))
-        
-    if disc == "em":
-        if bins is not None:
-            raise ValueError("Number of bins is automatically detected for Entropy Minimization discretization.")
-        if target is None:
-            raise ValueError("Need to define a target for Entropy Minimization discretization.")
-        if target in columns:
-            raise ValueError("Target column %s cannot be discretize too"%target)
-        if target not in idadf.columns:
-            raise ValueError("Undefined target column %s"%target)
-        stored_proc = "EMDISC"
-    else:
-        if target is not None:
-            raise ValueError("Target attribute defined only for Entropy Minimization discretization.")
-        if bins is None:
-            bins = 10      
-        if disc == "ef":
-            stored_proc = "EFDISC"
-        elif disc == "ew":
-            stored_proc = "EWDISC"
-        elif disc == "ewn":
-            stored_proc = "EWDISC_NICE"
-        else:
-            raise ValueError("Unknown discretization method.")
-            
-    return stored_proc
+        idadf1._idadb.drop_view(viewname)
```

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/entropy.py` & `nzpyida-0.3.5/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.3.5/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.3.5/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/private.py` & `nzpyida-0.3.5/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/feature_selection/tstats.py` & `nzpyida-0.3.5/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/filtering.py` & `nzpyida-0.3.5/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/frame.py` & `nzpyida-0.3.5/nzpyida/frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/indexing.py` & `nzpyida-0.3.5/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/internals.py` & `nzpyida-0.3.5/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/__init__.py` & `nzpyida-0.3.5/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/iris.py` & `nzpyida-0.3.5/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/iris.txt` & `nzpyida-0.3.5/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/swiss.py` & `nzpyida-0.3.5/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/swiss.txt` & `nzpyida-0.3.5/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/titanic.py` & `nzpyida-0.3.5/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sampledata/titanic.txt` & `nzpyida-0.3.5/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/series.py` & `nzpyida-0.3.5/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/sql.py` & `nzpyida-0.3.5/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/statistics.py` & `nzpyida-0.3.5/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/conftest.py` & `nzpyida-0.3.5/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_aggregation.py` & `nzpyida-0.3.5/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_association_rules.py` & `nzpyida-0.3.5/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_base.py` & `nzpyida-0.3.5/nzpyida/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.3.5/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_base_private.py` & `nzpyida-0.3.5/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.3.5/nzpyida/tests/test_base_table_manipulation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.3.5/nzpyida/tests/test_feature_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 from builtins import zip
 from future import standard_library
 standard_library.install_aliases()
 
 import pandas
 import pytest
 
-from nzpyida.feature_selection import pearson
-from nzpyida.feature_selection import spearman
 from nzpyida.feature_selection import ttest
 from nzpyida.feature_selection import chisquared
 from nzpyida.feature_selection import gini, gini_pairwise
 from nzpyida.feature_selection import entropy
 from nzpyida.feature_selection import info_gain, gain_ratio, su
 
 # Test symmetry
```

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_filtering.py` & `nzpyida-0.3.5/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_frame.py` & `nzpyida-0.3.5/nzpyida/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.3.5/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_frame_private.py` & `nzpyida-0.3.5/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_geoFrame.py` & `nzpyida-0.3.5/nzpyida/tests/test_geoFrame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_geoSeries.py` & `nzpyida-0.3.5/nzpyida/tests/test_geoSeries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_indexing.py` & `nzpyida-0.3.5/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_internals.py` & `nzpyida-0.3.5/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_kmeans.py` & `nzpyida-0.3.5/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.3.5/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_series.py` & `nzpyida-0.3.5/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_sorting.py` & `nzpyida-0.3.5/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_statistics.py` & `nzpyida-0.3.5/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/tests/test_utils.py` & `nzpyida-0.3.5/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida/utils.py` & `nzpyida-0.3.5/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.4/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.3.5/nzpyida.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.4
+Version: 0.3.5
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
+Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
+Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/IBM/nzpyida
+Project-URL: Tracker, https://github.com/IBM/nzpyida/issues
 Keywords: data analytics database development ibm netezza pandas scikitlearn scalability machine-learning knowledge discovery
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -126,7 +130,14 @@
     petal_length      0.871754    -0.428440      1.000000     0.962865
     petal_width       0.817941    -0.366126      0.962865     1.000000
 
 # Contributors
 
 The nzpyida is based on ibmdbpy project developed for IBM Db2 Warehouse.
 See https://github.com/ibmdbanalytics/ibmdbpy for details.
+
+# How to contribute
+You want to contribute? That's great! There are many things you can do.
+
+If you are a member of the ibmdbanalytics group, you can create branchs and merge them to master. Otherwise, you can fork the project and do a pull request. You are very welcome to contribute to the code and to the documentation.
+
+There are many ways to contribute. If you find bugs and have improvement ideas or need some new specific features, please open a ticket! We do care about it.
```

### Comparing `nzpyida-0.3.4/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.3.5/nzpyida.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 nzpyida/analytics/exploration/distribution.py
 nzpyida/analytics/exploration/relation_identification.py
 nzpyida/analytics/predictive/__init__.py
 nzpyida/analytics/predictive/association_rules.py
 nzpyida/analytics/predictive/bisecting_kmeans.py
 nzpyida/analytics/predictive/classification.py
 nzpyida/analytics/predictive/decision_trees.py
+nzpyida/analytics/predictive/glm.py
 nzpyida/analytics/predictive/kmeans.py
 nzpyida/analytics/predictive/knn.py
 nzpyida/analytics/predictive/linear_regression.py
 nzpyida/analytics/predictive/naive_bayes.py
 nzpyida/analytics/predictive/predictive_modeling.py
 nzpyida/analytics/predictive/regression.py
 nzpyida/analytics/predictive/regression_trees.py
@@ -81,14 +82,15 @@
 nzpyida/analytics/predictive/two_step_clustering.py
 nzpyida/analytics/tests/conftest.py
 nzpyida/analytics/tests/test_association_rules.py
 nzpyida/analytics/tests/test_auto_delete_context.py
 nzpyida/analytics/tests/test_bisecting_kmeans.py
 nzpyida/analytics/tests/test_decision_trees.py
 nzpyida/analytics/tests/test_discretization.py
+nzpyida/analytics/tests/test_glm.py
 nzpyida/analytics/tests/test_kmeans.py
 nzpyida/analytics/tests/test_knn.py
 nzpyida/analytics/tests/test_linear_regression.py
 nzpyida/analytics/tests/test_model_manager.py
 nzpyida/analytics/tests/test_naive_bayes.py
 nzpyida/analytics/tests/test_preparation.py
 nzpyida/analytics/tests/test_regression_trees.py
@@ -96,16 +98,14 @@
 nzpyida/analytics/tests/test_timeseries.py
 nzpyida/analytics/tests/test_two_step_clustering.py
 nzpyida/analytics/transform/__init__.py
 nzpyida/analytics/transform/discretization.py
 nzpyida/analytics/transform/preparation.py
 nzpyida/feature_selection/__init__.py
 nzpyida/feature_selection/chisquared.py
-nzpyida/feature_selection/correlation.py
-nzpyida/feature_selection/discretize.py
 nzpyida/feature_selection/entropy.py
 nzpyida/feature_selection/gain_ratio.py
 nzpyida/feature_selection/gini.py
 nzpyida/feature_selection/info_gain.py
 nzpyida/feature_selection/private.py
 nzpyida/feature_selection/symmetric_uncertainty.py
 nzpyida/feature_selection/tstats.py
```

### Comparing `nzpyida-0.3.4/setup.py` & `nzpyida-0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
       ]
 
 setup(name='nzpyida',
-      version='0.3.4',
+      version='0.3.5',
       install_requires=['pandas','numpy','future','six','pypyodbc','pyodbc', 'lazy', 'nzpy'],
 
       extras_require={
         'jdbc':['JayDeBeApi==1.*', 'Jpype1==0.6.3'],
         'test':['pytest', 'flaky==3.4.0'],
         'doc':['sphinx', 'ipython', 'numpydoc', 'sphinx_rtd_theme']
       },
@@ -80,9 +80,14 @@
       author='IBM Corp.',
       author_email='mlabenski@ibm.com,pawel.mroz1@ibm.com',
       license='BSD',
       classifiers=classifiers,
       keywords='data analytics database development ibm netezza pandas scikitlearn scalability machine-learning knowledge discovery',
       packages=find_packages(exclude=['docs', 'tests*']),
       package_data={
-        'nzpyida.sampledata': ['*.txt']}
+        'nzpyida.sampledata': ['*.txt']},
+      url="https://github.com/ibm/nzpyida",
+      project_urls={
+        "Documentation": "https://nzpyida.readthedocs.io/en/latest/",
+        "Source": "https://github.com/IBM/nzpyida",
+        "Tracker": "https://github.com/IBM/nzpyida/issues"},
      )
```


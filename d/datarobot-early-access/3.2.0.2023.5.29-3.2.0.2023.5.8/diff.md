# Comparing `tmp/datarobot_early_access-3.2.0.2023.5.29.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.29.tar", last modified: Mon May 29 16:46:53 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.5.8.tar", last modified: Mon May  8 16:47:08 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.5.29.tar` & `datarobot_early_access-3.2.0.2023.5.8.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   173064 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5678 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2257 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      927 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18879 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2463 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    25285 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8680 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4012 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23047 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59133 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    58123 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4832 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93319 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256106 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215251 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6340 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24120 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8680 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17330 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5684 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1108 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3103 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-29 16:46:53.000000 datarobot_early_access-3.2.0.2023.5.29/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-29 16:46:10.000000 datarobot_early_access-3.2.0.2023.5.29/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   169379 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8705 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5638 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2271 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17252 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2063 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24305 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   100246 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4044 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8437 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23045 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    83098 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40817 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    56459 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4829 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12639 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    93316 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16683 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21038 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   256106 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9565 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209815 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6051 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19984 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1560 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17373 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-05-08 16:46:19.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5675 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1079 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-05-08 16:47:07.000000 datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3148 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-05-08 16:47:08.000000 datarobot_early_access-3.2.0.2023.5.8/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-05-08 16:46:20.000000 datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.5.8/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 - Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
 
 - Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings.
    :meth:`Deployment.get_bias_and_fairness_settings<datarobot.models.Deployment.get_bias_and_fairness_settings>`
    :meth:`Deployment.update_bias_and_fairness_settings<datarobot.models.Deployment.update_bias_and_fairness_settings>`
 
 - Added a new class :class:`UseCase <datarobot.UseCase>` for interacting with the DataRobot Use Cases API.
+- Added a new class :class:`Notebook <datarobot.Notebook>` for retrieving DataRobot Notebooks available to the user.
 - Added a new class :class:`Application <datarobot.Application>` for retrieving DataRobot Applications available to the user.
 - Added a new class :class:`SharingRole <datarobot.models.sharing.SharingRole>` to hold user or organization access rights.
 - Added a new class :class:`BatchMonitoringJob <datarobot.models.BatchMonitoringJob>` for interacting with batch monitoring jobs.
 - Added a new class :class:`BatchMonitoringJobDefinition <datarobot.models.BatchMonitoringJobDefinition>` for interacting with batch monitoring jobs definitions.
 - Added a new methods for handling monitoring job definitions: list, get, create, update, delete, run_on_schedule and run_once
   :meth:`BatchMonitoringJobDefinition.list <datarobot.models.BatchMonitoringJobDefinition.list>`
   :meth:`BatchMonitoringJobDefinition.get <datarobot.models.BatchMonitoringJobDefinition.get>`
@@ -29,78 +30,44 @@
   :meth:`BatchMonitoringJobDefinition.delete <datarobot.models.BatchMonitoringJobDefinition.delete>`
   :meth:`BatchMonitoringJobDefinition.run_on_schedule <datarobot.models.BatchMonitoringJobDefinition.run_on_schedule>`
   :meth:`BatchMonitoringJobDefinition.run_once <datarobot.models.BatchMonitoringJobDefinition.run_once>`
 - Added a new method to retrieve a monitoring job
   :meth:`BatchMonitoringJob.get <datarobot.models.BatchMonitoringJob.get>`
 - Added the ability to filter return objects by a Use Case ID passed to the following methods:
   :meth:`Dataset.list <datarobot.models.Dataset.list>`
+  :meth:`Notebook.list <datarobot.Notebook.list>`
   :meth:`Project.list <datarobot.models.Project.list>`
-- Added the ability to automatically add a newly created dataset or project to a Use Case by passing a UseCase, list of UseCase objects, UseCase ID or list of UseCase IDs using the keyword argument `use_cases` to the following methods:
-  :meth:`Dataset.create_from_file <datarobot.models.Dataset.create_from_file>`
-  :meth:`Dataset.create_from_in_memory_data <datarobot.models.Dataset.create_from_in_memory_data>`
-  :meth:`Dataset.create_from_url <datarobot.models.Dataset.create_from_url>`
-  :meth:`Dataset.create_from_data_source <datarobot.models.Dataset.create_from_data_source>`
-  :meth:`Dataset.create_from_query_generator <datarobot.models.Dataset.create_from_query_generator>`
-  :meth:`Dataset.create_project <datarobot.models.Dataset.create_project>`
-  :meth:`Project.create <datarobot.models.Project.create>`
-  :meth:`Project.create_from_data_source <datarobot.models.Project.create_from_data_source>`
-  :meth:`Project.create_from_dataset <datarobot.models.Project.create_from_dataset>`
-  :meth:`Project.create_segmented_project_from_clustering_model <datarobot.models.Project.create_segmented_project_from_clustering_model>`
-  :meth:`Project.start <datarobot.models.Project.start>`
-- Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set in several ways.
-
-  - If the user configures the client via `Client(...)`, then invoke `Client(..., default_use_case = <id>)`.
-  - If the user configures the client via dr.config.yaml, then add the property `default_use_case: <id>`.
-  - If the user configures the client via env vars, then set the env var ``DATAROBOT_DEFAULT_USE_CASE``.
-  - The default use case can also be set programmatically as a context manager via `with UseCase.get(<id>):`.
 
-- Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
-- Added a new class :class:`FairnessScoresOverTime <datarobot.models.deployment.bias_and_fairness.FairnessScoresOverTime>` to retrieve fairness over time information.
-- Added a new method :meth:`Deployment.get_fairness_scores_over_time <datarobot.models.Deployment.get_fairness_scores_over_time>` to retrieve fairness scores over time of a deployment.
-- Added a new `use_gpu` parameter to the method :meth:`Project.analyze_and_model<datarobot.models.Project.analyze_and_model>` to set whether the project should allow usage of GPU
-- Added a new `use_gpu` parameter to the class :class:`Project <datarobot.models.Project>` with information whether project allows usage of GPU
-- Added a new class :class:`TrainingData <datarobot.models.custom_model_version.TrainingData>` for retrieving TrainingData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
-- Added a new class :class:`HoldoutData <datarobot.models.custom_model_version.HoldoutData>` for retrieving HoldoutData assigned to :class:`CustomModelVersion <datarobot.CustomModelVersion>`.
+- Added the ability to set a default :class:`UseCase <datarobot.UseCase>` for requests. It can be set by:
+
+  - invoking `Client(..., use_case = <id>)`, or
+  - setting `use_case: <id>` in drconfig.yaml, or
+  - setting the env var DATAROBOT_DEFAULT_USE_CASE, or
+  - calling `with UseCase.get(<id>):`.
 
+- Added method meth:`Deployment.get_predictions_over_time <datarobot.models.Deployment.get_predictions_over_time>` to retrieve deployment predictions over time data.
 
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
 
 - Extended :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>` by two parameters
   to filter for a target value range in regression projects.
 
 - Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>` and made sure it is returned in both :py:meth:`datarobot.PredictionExplanations.get_all_as_dataframe`  and :py:meth:`datarobot.PredictionExplanations.get_rows` method.
 
-- Added two new parameters to :meth:`Project.upload_dataset_from_catalog <datarobot.models.Project.upload_dataset_from_catalog>`:
-    - `credential_id`
-    - `credential_data`
-
-- Implemented training and holdout data assignment for Custom Model Version creation APIs:
-    - :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>`
-    - :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_from_previous>`
-
-    The parameters added to both APIs are:
-        - `training_dataset_id`
-        - `partition_column`
-        - `holdout_dataset_id`
-        - `keep_training_holdout_data`
-        - `max_wait`
-
 Bugfixes
 ********
-- Fixed incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
-- Fixed a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
-- Fixed an issue where failed authentication when invoking `datarobot.client.Client()` raises a misleading error about client-server compatibility.
+- Fix incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
+- Fix a crash when using non-"latin-1" characters in Panda's DataFrame used as prediction data in :meth:`BatchPredictionJob.score <datarobot.models.BatchPredictionJob.score>`.
 
 API Changes
 ***********
-- Added parameter ``unsupervised_type`` to the class :class:`DatetimePartitioning <datarobot.DatetimePartitioning>`.
 
 Deprecation Summary
 *******************
 - ``Model.get_feature_fit_metadata`` has been removed.
   Use :meth:`Model.get_feature_effect_metadata <datarobot.models.Model.get_feature_effect_metadata>` instead.
 - ``DatetimeModel.get_feature_fit_metadata`` has been removed.
   Use :meth:`DatetimeModel.get_feature_effect_metadata <datarobot.models.DatetimeModel.get_feature_effect_metadata>` instead.
@@ -115,20 +82,20 @@
 - ``Model.get_or_request_feature_fit`` has been removed.
   Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
 - ``DatetimeModel.get_or_request_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
 
 Configuration Changes
 *********************
+- Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
 Documentation Changes
 *********************
 - Fixed in-line documentation of `DataRobotClientConfig`.
-- Fixed documentation around client configuration from environment variables or config file.
 
 Experimental changes
 *********************
 - Added experimental support for data matching:
 
   - :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`
   - :class:`DataMatchingQuery <datarobot._experimental.models.data_matching.DataMatchingQuery>`
@@ -141,24 +108,14 @@
 
 - Added experimental support for model lineage: :class:`ModelLineage <datarobot._experimental.models.model_lineage.ModelLineage>`
 
 - Changed behavior for methods that search for the closest data points in :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. If the index is missing, instead of throwing the error, methods try to create the index and then query it. This is enabled by default, but if this is not the intended behavior it can be changed by passing `False` to the new `build_index` parameter added to the methods:
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
-- Added a new class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` for retrieving DataRobot Notebooks available to the user.
-
-
-3.1.1
-=====
-
-Configuration Changes
-*********************
-- Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
-- Update `typing-extensions <https://pypi.org/project/typing-extensions/>`_ to be inclusive of versions from 4.3.0 to < 5.0.0.
 
 3.1.0
 =====
 
 New Features
 ************
 
@@ -204,15 +161,15 @@
 *******************
 - Deprecated method :meth:`Project.create_from_hdfs<datarobot.models.Project.create_from_hdfs>`.
 - Deprecated method :meth:`DatetimePartitioning.generate <datarobot.DatetimePartitioning.generate>`.
 - Deprecated parameter ``in_use`` from :meth:`ImageAugmentationList.create<datarobot.models.visualai.ImageAugmentationList.create>` as DataRobot will take care of it automatically.
 - Deprecated property ``Deployment.capabilities`` from :class:`Deployment <datarobot.models.Deployment>`.
 - ``ImageAugmentationSample.compute`` was removed in v3.1. You
   can get the same information with the method ``ImageAugmentationList.compute_samples``.
-- ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead.
+- ``sample_id`` parameter removed from ``ImageAugmentationSample.list``. Please use ``auglist_id`` instead. 
 
 Configuration Changes
 *********************
 
 Experimental changes
 *********************
 
@@ -223,23 +180,23 @@
 - Update the documentation to suggest setting `use_start_end_format` of :py:meth:`Backtest.to_specification <datarobot.helpers.partitioning_methods.Backtest.to_specification>` to `True` will mirror the same behavior as the Web UI.
 
 3.0.3
 =====
 
 Bugfixes
 ********
-- Fixed an issue affecting backwards compatibility in :class:`datarobot.models.DatetimeModel`, where an unexpected keyword from the DataRobot API would break class deserialization.
+- Fixed an issue affecting backwards compatibility in :class:`datarobot.models.DatetimeModel`, where an unexpected keyword from the DataRobot API would break class deserialization. 
 
 3.0.2
 =====
 
 Bugfixes
 ********
 - Restored :meth:`Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>`, :meth:`Model.open_model_browser <datarobot.models.Model.open_model_browser>`,
-  :meth:`Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>`, and :meth:`Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`.
+  :meth:`Project.get_leaderboard_ui_permalink <datarobot.models.Project.get_leaderboard_ui_permalink>`, and :meth:`Project.open_leaderboard_browser <datarobot.models.Project.open_leaderboard_browser>`. 
   These methods were accidentally removed instead of deprecated.
 - Fix for ipykernel < 6.0.0 which does not persist contextvars across cells
 
 Deprecation Summary
 *******************
 - Deprecated method :meth:`Model.get_leaderboard_ui_permalink <datarobot.models.Model.get_leaderboard_ui_permalink>`. Please use :meth:`Model.get_uri <datarobot.models.Model.get_uri>` instead.
 - Deprecated method :meth:`Model.open_model_browser <datarobot.models.Model.open_model_browser>`. Please use :meth:`Model.open_in_browser <datarobot.models.Model.open_in_browser>` instead.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.5.29
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/README.md` & `datarobot_early_access-3.2.0.2023.5.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,46 +4,27 @@
 [DataRobot](!http://datarobot.com) platform API.
 
 This README is primarily intended for those developing the client. There is
 also documentation intended for users of the client contained in the `docs`
 directory of this repository. You can view the public documentation at
 [https://datarobot-public-api-client.readthedocs-hosted.com](https://datarobot-public-api-client.readthedocs-hosted.com).
 
-## Topics
-
-* Development:
-  * [Getting Started](#getting-started)
-  * [Guidelines](#guidelines)
-  * [Setup datarobot sdk locally](#installation)
-  * [Running tests](#running-tests)
-  * [Linting](#linting)
-* Setup topics:
-  * [Common DataRobot Client setup](#datarobot-client-setup)
-    * [Setup with cfg file](#setup-with-cfg-file)
-    * [Setup explicitly in code](#setup-explicitly-in-code)
-    * [Setup with environment variables](#setup-with-environment-variables)
-* Building the documentation
-
 ## Getting Started
 
 You need to have
 
     - Git
     - Docker
     - Python >= 3.7
     - DataRobot account
     - pip
 
 We recommend using a virtualenv to keep dependencies from conflicting with
 projects you may have on your machine.
 
-## Guidelines
-
-Our full list of suggestions and guidelines for code being added to this repository can be found [here](GUIDELINES.md).
-
 ## Installation
 
 ```console
 git clone git@github.com:datarobot/public_api_client.git
 cd public_api_client
 # mkvirtualenv ...
 make req  # upgrades pip, setuptools, installs dev requirements
@@ -90,14 +71,27 @@
 To build a PDF of the docs for release:
 
 ```console
 cd sdk_docs
 make clean xelatexpdf
 ```
 
+## Topics
+
+* Setup topics:
+  * [Common DataRobot Client setup](#datarobot-client-setup)
+    * [Setup with cfg file](#setup-with-cfg-file)
+    * [Setup explicitly in code](#setup-explicitly-in-code)
+    * [Setup with environment variables](#setup-with-environment-variables)
+* Building the documentation
+* Development:
+  * [Setup datarobot sdk locally](#installation)
+  * [Running tests](#running-tests)
+  * [Linting](#linting)
+
 ### DataRobot Client Setup
 
 There are three different ways to set up the client to authenticate with the
 server: through a config file, through environment variables, or explicitly in
 the code.
 
 You must specify an endpoint and an API token.  You can manage your API tokens in the DataRobot
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/common_setup.py` & `datarobot_early_access-3.2.0.2023.5.8/common_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,16 +181,15 @@
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
         "requests>=2.28.1",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
         "urllib3>=1.23,<2.0.0",
-        "typing-extensions>=4.3.0,<5",
-        "mypy-extensions>=0.4.0,<2",
+        "typing-extensions==4.3.0",
     ],
     extras_require={
         "dev": dev_require,
         "examples": example_require,
         "release": release_require,
         "lint": lint_require,
         "images": images_require,
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     Job,
     Model,
     ModelBlueprintChart,
     ModelingFeature,
     ModelingFeaturelist,
     ModelJob,
     ModelRecommendation,
+    Notebook,
     PayoffMatrix,
     PredictionDataset,
     PredictionExplanations,
     PredictionExplanationsInitialization,
     Predictions,
     PredictionServer,
     PredictJob,
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/notebooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 import trafaret as t
 
-from datarobot._experimental.models.enums import NotebookPermissions, NotebookStatus
+from datarobot.enums import NotebookPermissions
 from datarobot.models.api_object import APIObject
-from datarobot.models.use_cases.utils import resolve_use_cases, UseCaseLike
+from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils.pagination import unpaginate
 
 notebook_user_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("username"): t.String,
         t.Key("first_name"): t.String,
@@ -45,19 +45,15 @@
         t.Key("hide_cell_outputs"): t.Bool,
         t.Key("show_scrollers"): t.Bool,
     }
 )
 
 
 notebook_session_trafaret = t.Dict(
-    {
-        t.Key("status"): t.String,
-        t.Key("notebook_id"): t.String,
-        t.Key("started_at", optional=True): t.String,
-    }
+    {t.Key("status"): t.String, t.Key("notebook_id"): t.String, t.Key("started_at"): t.String}
 )
 
 
 class NotebookUser(APIObject):
     """
     A user associated with a Notebook.
 
@@ -86,25 +82,25 @@
 class NotebookSession(APIObject):
     """
     Information about the current status of a Notebook.
 
     Attributes
     ----------
 
-    status : NotebookStatus
+    status : str
         The current status of the Notebook kernel.
     notebook_id : str
         The ID of the Notebook.
-    started_at : Optional[str]
-        The date and time when the notebook was started. Optional.
+    started_at : str
+
     """
 
     _converter = notebook_session_trafaret
 
-    def __init__(self, status: NotebookStatus, notebook_id: str, started_at: Optional[str] = None):
+    def __init__(self, status: str, notebook_id: str, started_at: str):
         self.status = status
         self.notebook_id = notebook_id
         self.started_at = started_at
 
 
 class NotebookActivity(APIObject):
     """
@@ -124,15 +120,15 @@
     def __init__(self, at: str, by: Dict[str, str]):
         self.at = at
         self.by = NotebookUser.from_server_data(by)
 
 
 class NotebookSettings(APIObject):
     """
-    Settings for a DataRobot Notebook.
+    A user associated with a Notebook.
 
     Attributes
     ----------
 
     show_line_numbers : bool
         Whether line numbers in cells should be displayed.
     hide_cell_titles : bool
@@ -197,34 +193,34 @@
         {
             t.Key("id"): t.String,
             t.Key("name"): t.String,
             t.Key("description", optional=True): t.Or(t.String, t.Null),
             t.Key("permissions"): t.List(t.String),
             t.Key("tags"): t.List(t.String),
             t.Key("created"): notebook_activity_trafaret,
-            t.Key("updated", optional=True): notebook_activity_trafaret,
+            t.Key("updated"): notebook_activity_trafaret,
             t.Key("last_viewed"): notebook_activity_trafaret,
             t.Key("settings"): notebook_settings_trafaret,
-            t.Key("org_id", optional=True): t.String,
+            t.Key("org_id"): t.String,
             t.Key("session", optional=True): t.Or(notebook_session_trafaret, t.Null),
             t.Key("use_case_id", optional=True): t.Or(t.String, t.Null),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         id: str,
         name: str,
         permissions: List[str],
         tags: List[str],
         created: Dict[str, Any],
+        updated: Dict[str, Any],
         last_viewed: Dict[str, Any],
         settings: Dict[str, bool],
-        updated: Optional[Dict[str, Any]] = None,
-        org_id: Optional[str] = None,
+        org_id: str,
         description: Optional[str] = None,
         session: Optional[Dict[str, str]] = None,
         use_case_id: Optional[str] = None,
     ):
         self.id = id
         self.name = name
         self.description = description
@@ -264,15 +260,15 @@
         cls,
         created_before: Optional[str] = None,
         created_after: Optional[str] = None,
         order_by: Optional[str] = None,
         tags: Optional[List[str]] = None,
         owners: Optional[List[str]] = None,
         query: Optional[str] = None,
-        use_cases: Optional[UseCaseLike] = None,
+        use_case_id: Optional[str] = None,
     ) -> List[Notebook]:
         """
         List all Notebooks available to the user.
 
         Parameters
         ----------
         created_before : Optional[str]
@@ -288,26 +284,28 @@
         tags : Optional[List[str]]
             A list of tags that returned Notebooks should be associated with. Optional.
         owners : Optional[List[str]]
             A list of user IDs used to filter returned Notebooks.
             The respective users share ownership of the Notebooks. Optional.
         query : Optional[str]
             A specific regex query to use when filtering Notebooks. Optional.
-        use_cases : Optional[UseCase or List[UseCase] or str or List[str]]
-            Filters returned Notebooks by a specific Use Case or Cases. Accepts either the entity or the ID. Optional.
+        use_case_id : Optional[str]
+            Constrain returned Notebooks to a specific Use Case. Optional.
         Returns
         -------
         notebooks : List[Notebook]
             A list of Notebooks available to the user.
         """
         params = {
             "created_before": created_before,
             "created_after": created_after,
             "order_by": order_by,
             "tags": tags,
             "owners": owners,
             "query": query,
         }
-        params = resolve_use_cases(use_cases=use_cases, params=params, use_case_key="use_case_id")
+        params = resolve_use_case(
+            use_case_id=use_case_id, params=params, use_case_key="use_case_id"
+        )
         url = f"{cls._client.domain}/{cls._path}"
         r_data = unpaginate(url, params, cls._client)
         return [Notebook.from_server_data(data) for data in r_data]
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/project_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,16 @@
         One of BiasMitigationTechnique.
         The technique by which we'll mitigate bias, which will inform which bias mitigation task
         we insert into blueprints and how
     include_bias_mitigation_feature_as_predictor_variable : bool or None, optional
         Whether we should also use the mitigation feature as in input to the modeler just like
         any other categorical used for training, i.e. do we want the model to "train on" this
         feature in addition to using it for bias mitigation
+    force_cpu: bool, optional
+        If GPUs enabled, override and force running everything on CPUs
     min_clusters: int, optional
         The minimum number of clusters allowed when training clustering models.
     max_clusters: int, optional
         The maximum number of clusters allowed when training clustering models
     segmentation_id_column: string, optional
         The segmentation column name or automated segmentation column name specified for the
         project through the UI
@@ -515,14 +517,15 @@
                 t.Null(), t.Dict({}), FeatureEngineeringOptions._converter
             ),
             t.Key("feature_engineering_prediction_point", optional=True): t.Null()
             | Feature._converter,
             t.Key("featurelist_id", optional=True): t.Null() | String(),
             t.Key("feature_settings", optional=True): t.Null()
             | t.List(_feature_settings_converter),
+            t.Key("force_cpu", optional=True): t.Null() | t.Bool(),
             t.Key("forecast_window_end", optional=True): t.Null() | Int(),
             t.Key("forecast_window_start", optional=True): t.Null() | Int(),
             t.Key("gap_duration", optional=True): t.Null() | String(),
             t.Key("holdout_duration", optional=True): t.Or(t.Null(), String(), Duration._converter),
             t.Key("holdout_end_date", optional=True): t.Null() | parse_time,
             t.Key("holdout_level", optional=True): t.Null() | t.Or(String(), Int()),
             t.Key("holdout_pct", optional=True): t.Null() | Int(),
@@ -604,14 +607,15 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
+        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -690,14 +694,15 @@
             feature_derivation_window_end=feature_derivation_window_end,
             feature_derivation_window_start=feature_derivation_window_start,
             feature_engineering_graphs=feature_engineering_graphs,
             feature_engineering_options=feature_engineering_options,
             feature_engineering_prediction_point=feature_engineering_prediction_point,
             featurelist_id=featurelist_id,
             feature_settings=feature_settings,
+            force_cpu=force_cpu,
             forecast_window_end=forecast_window_end,
             forecast_window_start=forecast_window_start,
             gap_duration=gap_duration,
             holdout_duration=holdout_duration,
             holdout_end_date=holdout_end_date,
             holdout_level=holdout_level,
             holdout_pct=holdout_pct,
@@ -771,14 +776,15 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
+        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -894,14 +900,15 @@
                     if "a_priori" not in feature_setting.keys()
                     else {"known_in_advance": feature_setting.pop("a_priori"), **feature_setting}
                 )
                 for feature_setting in feature_settings
             ]
         else:
             self.feature_settings = feature_settings
+        self.force_cpu = force_cpu
         self.forecast_window_end = forecast_window_end
         self.forecast_window_start = forecast_window_start
         self.gap_duration = gap_duration
         if holdout_duration and isinstance(holdout_duration, dict):
             self.holdout_duration = Duration(**holdout_duration)
         else:
             self.holdout_duration = holdout_duration
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/_experimental/models/retraining.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 import trafaret as t
 
 from datarobot._compat import String
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
 from datarobot.utils.pagination import unpaginate
 
 
-class RetrainingPolicy(APIObject):
+class RetrainingPolicy(APIObject, DeploymentQueryBuilderMixin):
     """Retraining Policy.
 
     Attributes
     ----------
     policy_id : str
         ID of the retraining policy
     name : str
@@ -144,15 +145,15 @@
             )
         """
 
         path = "{}{}/".format(cls._path.format(deployment_id), retraining_policy_id)
         cls._client.delete(path)
 
 
-class RetrainingPolicyRun(APIObject):
+class RetrainingPolicyRun(APIObject, DeploymentQueryBuilderMixin):
     """Retraining policy run.
 
     Attributes
     ----------
     policy_run_id : str
         ID of the retraining policy run
     status : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from typing import Optional, Tuple, TYPE_CHECKING, Union
 import warnings
 
 from urllib3 import Retry
 import yaml
 
 from ._version import __expected_server_version__, __version__
-from .context import Context, DefaultUseCase
 from .errors import ClientError
 from .rest import DataRobotClientConfig, RESTClientObject
 
 if TYPE_CHECKING:
     from requests import Response
 
 logger = logging.getLogger(__package__)
@@ -44,29 +43,24 @@
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
-    default_use_case: Optional[str] = None,
-) -> Tuple[RESTClientObject, Optional[str]]:
-    """Return a new `RESTClientObject` and default_use_case id with optional configuration.
-    The client will be configured in one of the following ways, in order of priority.
-
-      1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
-      2. From a YAML file at the path specified in the ``config_path`` kwarg;
-      3. From a YAML file at the path specified in the env var ``DATAROBOT_CONFIG_FILE``;
-      4. From env vars, iff ``DATAROBOT_ENDPOINT`` and ``DATAROBOT_API_TOKEN`` are specified;
-      5. From a YAML file at the path `$HOME/.config/datarobot/drconfig.yaml`.
+    use_case: Optional[str] = None,
+) -> RESTClientObject:
+    """Return a new `RESTClientObject` with optional configuration.
+    Missing configuration will be read from environment variables or a config
+    file.
 
     .. note::
-        This function is intended for use with the ``Client`` function and the
-        ``client_configuration`` context manager only. Use of the global context will
-        be deprecated in v4.0.
+        This function is intended for use with the ``client_configuration``
+        context manager only. Use of the global context will eventually
+        be deprecated.
 
     Parameters
     ----------
     token : str, optional
         API token
     endpoint : str, optional
         Base url of API
@@ -85,28 +79,28 @@
         Could be set to path with certificates of trusted certification authorities
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools
-    default_use_case: str, optional
+    use_case: str, optional
         The entity ID of the default Use Case to use with any requests made by this Client instance.
     """
     env_config = _get_config_file_from_env()
     if token and endpoint:
         drconfig = DataRobotClientConfig(
             endpoint=endpoint,
             token=token,
             connect_timeout=connect_timeout,
             user_agent_suffix=user_agent_suffix,
             ssl_verify=ssl_verify,
             max_retries=max_retries,
             token_type=token_type,
-            default_use_case=default_use_case,
+            use_case=use_case,
         )
     elif config_path:
         if not _file_exists(config_path):
             raise ValueError(f"Invalid config path - no file at {config_path}")
         drconfig = _config_from_file(config_path)
     elif env_config:
         if not _file_exists(env_config):
@@ -125,43 +119,32 @@
     if not drconfig.max_retries:
         drconfig.max_retries = Retry(backoff_factor=0.1, respect_retry_after_header=True)
 
     client = RESTClientObject.from_config(drconfig)
     if not _is_compatible_client(client):
         raise ValueError("The client is not compatible with the server version")
 
-    return client, drconfig.default_use_case
+    return client
 
 
 def Client(
     token: Optional[str] = None,
     endpoint: Optional[str] = None,
     config_path: Optional[str] = None,
     connect_timeout: Optional[int] = None,
     user_agent_suffix: Optional[str] = None,
     ssl_verify: bool = True,
     max_retries: Optional[Union[int, Retry]] = None,
     token_type: str = "Token",
-    default_use_case: Optional[str] = None,
+    use_case: Optional[str] = None,
 ) -> RESTClientObject:
     """
-    Configures the global API client for the Python SDK. The client will be configured in one of
-    the following ways, in order of priority.
-
-      1. From call args iff ``token`` and ``endpoint`` kwargs are specified;
-      2. From a YAML file at the path specified in the ``config_path`` kwarg;
-      3. From a YAML file at the path specified in the env var ``DATAROBOT_CONFIG_FILE``;
-      4. From env vars, iff ``DATAROBOT_ENDPOINT`` and ``DATAROBOT_API_TOKEN`` are specified;
-      5. From a YAML file at the path `$HOME/.config/datarobot/drconfig.yaml`.
-
-    .. note::
-        All client configuration must be done via a single method; there is no fall back to
-        lower priority methods.
-
-    This can also have the side effect of setting a default Use Case for client API requests.
+    Configures the global API client for the Python SDK with optional
+    configuration. Missing configuration will be read from env
+    or config file.
 
     Parameters
     ----------
     token : str, optional
         API token
     endpoint : str, optional
         Base url of API
@@ -180,34 +163,33 @@
         Could be set to path with certificates of trusted certification authorities.
     max_retries : int or datarobot.rest.Retry, optional
         Either an integer number of times to retry connection errors,
         or a `urllib3.util.retry.Retry` object to configure retries.
     token_type: str, "Token" by default
         Authentication token type: Token, Bearer.
         "Bearer" is for DataRobot OAuth2 token, "Token" for token generated in Developer Tools.
-    default_use_case: str, optional
-        The entity ID of the default Use Case to use with any requests made by the client.
+    use_case: str, optional
+        The entity ID of the default Use Case to use with any requests made by this Client instance.
     Returns
     -------
         The ``RESTClientObject`` instance created.
     """
-    new_client, default_use_case = _create_client(
+    new_client = _create_client(
         token,
         endpoint,
         config_path,
         connect_timeout,
         user_agent_suffix,
         ssl_verify,
         max_retries,
         token_type,
-        default_use_case,
+        use_case,
     )
 
     set_client(new_client)
-    Context.use_case = default_use_case
 
     return new_client
 
 
 def _is_compatible_client(client: RESTClientObject) -> bool:
     """
     Check that this client version is not ahead of the DataRobot version that
@@ -216,26 +198,18 @@
     Parameters
     ----------
     client : RESTClientObject
 
     Returns
     -------
     bool : True if client is compatible with server, False otherwise.
-
-    Raises
-    ------
-    ClientError
-        If the client is unable to authenticate with the DataRobot API.
-
     """
     try:
         server_response = client.get("version/")
     except ClientError as cerr:
-        # TODO Prefer to do further error handling via BaseException.add_note but that
-        # is only available in Python 3.11+
         if cerr.status_code == 401:
             w_msg_tmpl = (
                 'Unable to authenticate to the server - are you sure the provided token of "{}" '
                 'and endpoint of "{}" are correct? '.format(client.token, client.endpoint)
             )
         else:
             w_msg_tmpl = (
@@ -245,17 +219,16 @@
                 "incompatible with this version of the DataRobot client package. "
             )
         w_msg_tmpl += (
             "Note that if you access the DataRobot webapp at "
             "`https://app.datarobot.com`, then the correct endpoint to specify would "
             "be `https://app.datarobot.com/api/v2`."
         )
-        raise ClientError(
-            w_msg_tmpl.format(client.endpoint), status_code=cerr.status_code
-        ) from cerr
+        warnings.warn(w_msg_tmpl.format(client.endpoint))
+        return False
 
     if not _is_compatible_version(server_response):
         return False
 
     _ensure_protocol_match(client, server_response)
     return True
 
@@ -356,18 +329,14 @@
 
 
 def _get_client_version() -> str:
     return __version__
 
 
 def get_client() -> RESTClientObject:
-    """
-    Returns the global HTTP client for the Python SDK, instantiating it
-    if necessary.
-    """
     return _context_client.get(_global_client) or Client()
 
 
 class staticproperty(property):
     def __get__(self, instance, owner):
         return self.fget()
 
@@ -410,17 +379,23 @@
 
 
 _file_exists = os.path.isfile
 
 
 def _config_from_env() -> DataRobotClientConfig:
     """
-    Create and return a DataRobotClientConfig from environment variables. This method only allows
-    for configuration of endpoint, token, user_agent_suffix, max retries, and a default use case.
-    More advanced configuration must be done through a yaml file.
+    Create and return a DataRobotClientConfig from environment variables.
+
+    There are two ways this can be used:
+    1. Use the environment variable DATAROBOT_CONFIG_FILE to specify the path to a yaml config
+       file specifying the configuration to use
+    2. Use both the environment variables DATAROBOT_ENDPOINT and DATAROBOT_API_TOKEN to specify
+       the connection parameters. This method only allows for configuration of endpoint, token,
+       user_agent_suffix, and max retries. More advanced configuration must be done through a yaml
+       file
 
     Returns
     -------
     config : DataRobotClientConfig
 
     Raises
     ------
@@ -445,15 +420,15 @@
         )
         raise ValueError(e_msg)
     return DataRobotClientConfig(
         endpoint=endpoint,
         token=token,
         user_agent_suffix=user_agent_suffix,
         max_retries=max_retries,
-        default_use_case=use_case_id,
+        use_case=use_case_id,
     )
 
 
 def _config_from_file(config_path: str) -> DataRobotClientConfig:
     """
     Create and return a DataRobotClientConfig from a config path. The file must be
     a yaml formatted file
@@ -481,15 +456,15 @@
     per thread.
 
     DataRobot does not recommend nesting these contexts.
 
     Parameters
     ----------
         args : Parameters passed to ``datarobot.client.Client()``
-        kwargs : Keyword arguments passed to ``datarobot.client.Client()``
+        kwargs : Keyword arguments passed to ``datarobot.Client()``
 
     Examples
     --------
 
     .. code-block:: python
 
         from datarobot.client import client_configuration
@@ -508,18 +483,14 @@
 
         with client_configuration(config_path="/path/to/a/drconfig.yaml"):
             # Interact with DataRobot using a different configuration.
             Project.list()
     """
 
     contextvars_token: contextvars.Token[RESTClientObject] = None
-    previous_use_case: DefaultUseCase = None
     try:
-        client, default_use_case = _create_client(*args, **kwargs)
+        client = _create_client(*args, **kwargs)
         contextvars_token = _context_client.set(client)
-        previous_use_case = Context.get_use_case(raw=True)
-        Context.use_case = default_use_case
         yield
     finally:
         if contextvars_token is not None:
             _context_client.reset(contextvars_token)
-        Context.use_case = previous_use_case
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/context.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,33 +47,26 @@
 
     _use_case: DefaultUseCase = field(init=False, default=None)
 
     @property
     def use_case(self) -> DefaultUseCase:
         """Returns the default Use Case. If a string representing the Use Case ID
         was provided, lookup, cache, and return the actual entity."""
-        return self.get_use_case()
+        if isinstance(self._use_case, str):
+            try:
+                from .models.use_cases.use_case import (  # pylint: disable=import-outside-toplevel
+                    UseCase,
+                )
+
+                self._use_case = UseCase.get(use_case_id=self._use_case)
+            except (DataError, ClientError) as e:
+                raise ValueError("Current use case is invalid.", e)
+        return self._use_case or None
 
     @use_case.setter
     def use_case(self, value: DefaultUseCase = None) -> None:
         self._use_case = value
 
-    def get_use_case(self, raw: bool = False) -> DefaultUseCase:
-        """Returns the default Use Case. If a string representing the Use Case ID
-        was provided and raw=False, lookup, cache, and return the actual entity.
-        Otherwise, simply return the stored default Use Case in its current form"""
-        if not raw:
-            if isinstance(self._use_case, str):
-                try:
-                    from .models.use_cases.use_case import (  # pylint: disable=import-outside-toplevel
-                        UseCase,
-                    )
-
-                    self._use_case = UseCase.get(use_case_id=self._use_case)
-                except (DataError, ClientError) as e:
-                    raise ValueError("Current use case is invalid.", e)
-        return self._use_case or None
-
 
 _context: ContextVar[_ContextGlobals] = ContextVar("current_context", default=_ContextGlobals())
 
 Context = _context.get()
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,27 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from __future__ import annotations
-
-from enum import Enum, EnumMeta
-from typing import Optional
+from enum import Enum
 
 
 # A decorator to add an ALL attribute to (str, Enum) classes.
 def use_all(enum_instance):
     setattr(enum_instance, "ALL", list(map(lambda c: c, enum_instance)))
     return enum_instance
 
 
-class StrEnum(EnumMeta):
-    """
-    Enum that permits comparison of strings.
-    Ref: https://stackoverflow.com/questions/63335753/how-to-check-if-string-exists-in-enum-of-strings
-    """
-
-    def __contains__(cls: type, member: object) -> bool:
-        try:
-            cls(member)  # pylint: disable=no-value-for-parameter
-        except ValueError:
-            return False
-        return True
-
-
 def enum(*vals, **enums):
     """
     Enum without third party libs and compatible with py2 and py3 versions.
     """
     enums.update(dict(zip(vals, vals)))
     return type("Enum", (), enums)
 
@@ -332,19 +315,14 @@
     USER = ("USER",)
     EDITOR = ("EDITOR",)
     READ_ONLY = ("READ_ONLY",)
     CONSUMER = ("CONSUMER",)
     NO_ROLE = "NO_ROLE"
 
 
-class SHARING_RECIPIENT_TYPE(str, Enum):
-    USER = "user"
-    ORGANIZATION = "organization"
-
-
 MODEL_REPLACEMENT_REASON = enum(
     ACCURACY="ACCURACY",
     DATA_DRIFT="DATA_DRIFT",
     ERRORS="ERRORS",
     SCHEDULED_REFRESH="SCHEDULED_REFRESH",
     SCORING_SPEED="SCORING_SPEED",
     OTHER="OTHER",
@@ -897,41 +875,29 @@
 
 
 class ComplianceDocTemplateType(str, Enum):
     NORMAL = "normal"
     TIME_SERIES = "time_series"
 
 
-class UseCaseEntityType(str, Enum, metaclass=StrEnum):
+class UseCaseEntities(str, Enum):
     PROJECT = "project"
     DATASET = "dataset"
     NOTEBOOK = "notebook"
     APPLICATION = "application"
     RECIPE = "recipe"
 
 
-class UseCaseAPIPathEntityType(str, Enum):
-    PROJECT = "projects"
-    DATASET = "datasets"
-    APPLICATION = "applications"
-    RECIPE = "recipes"
-
-
-UseCaseReferenceEntityMap: dict[Optional[UseCaseEntityType], UseCaseAPIPathEntityType] = {
-    UseCaseEntityType.PROJECT: UseCaseAPIPathEntityType.PROJECT,
-    UseCaseEntityType.DATASET: UseCaseAPIPathEntityType.DATASET,
-    UseCaseEntityType.APPLICATION: UseCaseAPIPathEntityType.APPLICATION,
-    UseCaseEntityType.RECIPE: UseCaseAPIPathEntityType.RECIPE,
-}
+class NotebookPermissions(str, Enum):
+    CAN_READ = "CAN_READ"
+    CAN_UPDATE = "CAN_UPDATE"
+    CAN_DELETE = "CAN_DELETE"
+    CAN_SHARE = "CAN_SHARE"
+    CAN_COPY = "CAN_COPY"
+    CAN_EXECUTE = "CAN_EXECUTE"
 
 
 class ApplicationPermissions(str, Enum):
     CAN_DELETE = "CAN_DELETE"
     CAN_SHARE = "CAN_SHARE"
     CAN_UPDATE = "CAN_UPDATE"
     CAN_VIEW = "CAN_VIEW"
-
-
-class CredentialTypes(str, Enum):
-    BASIC = "basic"
-    OAUTH = "oauth"
-    S3 = "s3"
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,34 +135,14 @@
 
 class DuplicateFeaturesError(Exception):
     """
     Raised when trying to create featurelist with duplicating features
     """
 
 
-class TrainingDataAssignmentError(Exception):
-    """
-    Raised when the training data assignment for a custom model version fails
-    """
-
-    def __init__(
-        self, custom_model_id: str, custom_model_version_id: str, error_message: str
-    ) -> None:
-        self.custom_model_id = custom_model_id
-        self.custom_model_version_id = custom_model_version_id
-        self.error_message = error_message
-        self.message = (
-            f"Training data assignment failed for: "
-            f"model ID: {custom_model_id}; "
-            f"version ID: {custom_model_version_id}; "
-            f"Error message: {error_message}"
-        )
-        super().__init__(self.message)
-
-
 class DataRobotDeprecationWarning(DeprecationWarning):
     """
     Raised when using deprecated functions or using functions in a deprecated way
 
     See Also
     --------
     PlatformDeprecationWarning
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/partitioning_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     CV_METHOD,
     DEFAULT_MAX_WAIT,
     DIFFERENCING_METHOD,
     PERIODICITY_MAX_TIME_STEP,
     SERIES_AGGREGATION_TYPE,
     TIME_UNITS,
     TREAT_AS_EXPONENTIAL,
-    UnsupervisedTypeEnum,
 )
 from datarobot.errors import InvalidUsageError, UpdateAttributesError
 from datarobot.mixins.update_attributes_mixin import UpdateAttributesMixin
 from datarobot.utils import (
     deprecated,
     deprecation_warning,
     from_api,
@@ -1093,18 +1092,14 @@
     model_splits: int, optional
         (New in version v2.21) Sets the cap on the number of jobs per model used when
         building models to control number of jobs in the queue. Higher number of model splits
         will allow for less downsampling leading to the use of more post-processed data.
     allow_partial_history_time_series_predictions: bool, optional
         (New in version v2.24) Whether to allow time series models to make predictions using
         partial historical data.
-    unsupervised_type: str, optional
-        (New in version v3.2) The unsupervised project type, only valid if ``unsupervised_mode`` is
-        True. Use values from ``datarobot.enums.UnsupervisedTypeEnum`` enum.
-        If not specified then the project defaults to 'anomaly' when ``unsupervised_mode`` is True.
     """
 
     _converter = t.Dict(
         {
             t.Key("datetime_partition_column"): String(),
             t.Key("autopilot_data_selection_method", optional=True): String(),
             t.Key("validation_duration", optional=True): String(),
@@ -1151,17 +1146,14 @@
                 SERIES_AGGREGATION_TYPE.AVERAGE, SERIES_AGGREGATION_TYPE.TOTAL
             ),
             t.Key("cross_series_group_by_columns", optional=True): t.List(String()),
             t.Key("calendar_id", optional=True): String(),
             t.Key("unsupervised_mode", optional=True): t.Bool(),
             t.Key("model_splits", optional=True): Int(),
             t.Key("allow_partial_history_time_series_predictions", optional=True): t.Bool,
-            t.Key("unsupervised_type", optional=True): t.Enum(
-                UnsupervisedTypeEnum.ANOMALY, UnsupervisedTypeEnum.CLUSTERING
-            ),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         datetime_partition_column: str,
         autopilot_data_selection_method: Optional[str] = None,
@@ -1189,15 +1181,14 @@
         aggregation_type: Optional[str] = None,
         cross_series_group_by_columns: Optional[List[str]] = None,
         calendar_id: Optional[str] = None,
         holdout_end_date=None,
         unsupervised_mode: bool = False,
         model_splits: Optional[int] = None,
         allow_partial_history_time_series_predictions: bool = False,
-        unsupervised_type: Optional[str] = None,
     ) -> None:
         self.datetime_partition_column = datetime_partition_column
         self.autopilot_data_selection_method = autopilot_data_selection_method
         self.validation_duration = validation_duration
         self.holdout_start_date = holdout_start_date
         self.holdout_duration = holdout_duration
         self.holdout_end_date = holdout_end_date
@@ -1223,15 +1214,14 @@
         self.cross_series_group_by_columns = cross_series_group_by_columns
         self.calendar_id = calendar_id
         self.unsupervised_mode = unsupervised_mode
         self.model_splits = model_splits
         self.allow_partial_history_time_series_predictions = (
             allow_partial_history_time_series_predictions
         )
-        self.unsupervised_type = unsupervised_type
 
     def collect_payload(self) -> Dict[str, Any]:
         if self.holdout_start_date and not isinstance(self.holdout_start_date, datetime):
             raise ValueError("expected holdout_start_date to be a datetime.datetime")
         if self.holdout_end_date and not isinstance(self.holdout_end_date, datetime):
             raise ValueError("expected holdout_end_date to be a datetime.datetime")
         if self.holdout_duration and self.holdout_end_date:
@@ -1276,16 +1266,14 @@
             "model_splits": self.model_splits,
             "allow_partial_history_time_series_predictions": (
                 self.allow_partial_history_time_series_predictions
             ),
         }
         if self.unsupervised_mode:
             payload["unsupervised_mode"] = self.unsupervised_mode
-            if self.unsupervised_type:
-                payload["unsupervised_type"] = self.unsupervised_type
         if not self.disable_holdout:
             payload["holdout_start_date"] = self.holdout_start_date
             if self.holdout_duration:
                 payload["holdout_duration"] = self.holdout_duration
             elif self.holdout_end_date:
                 payload["holdout_end_date"] = self.holdout_end_date
 
@@ -1530,18 +1518,14 @@
         building models to control number of jobs in the queue. Higher number of model splits
         will allow for less downsampling leading to the use of more post-processed data.
     allow_partial_history_time_series_predictions: bool, optional
         (New in version v2.24) Whether to allow time series models to make predictions using
         partial historical data.
     unsupervised_mode: bool, optional
         (New in version v3.1) Whether the date/time partitioning is for an unsupervised project
-    unsupervised_type: str, optional
-        (New in version v3.2) The unsupervised project type, only valid if ``unsupervised_mode`` is
-        True. Use values from ``datarobot.enums.UnsupervisedTypeEnum`` enum.
-        If not specified then the project defaults to 'anomaly' when ``unsupervised_mode`` is True.
     """
 
     _client = staticproperty(get_client)
     _converter = t.Dict(
         {
             t.Key("project_id"): String(),
             t.Key("datetime_partitioning_id", optional=True): t.Or(String(), t.Null),
@@ -1608,17 +1592,14 @@
             ),
             t.Key("cross_series_group_by_columns", optional=True): t.List(String()),
             t.Key("calendar_id", optional=True): String(),
             t.Key("calendar_name", optional=True): String(),
             t.Key("model_splits", optional=True): Int(),
             t.Key("allow_partial_history_time_series_predictions", optional=True): t.Bool,
             t.Key("unsupervised_mode", optional=True): t.Bool,
-            t.Key("unsupervised_type", optional=True): t.Enum(
-                UnsupervisedTypeEnum.ANOMALY, UnsupervisedTypeEnum.CLUSTERING
-            ),
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         project_id=None,
         datetime_partitioning_id=None,
@@ -1665,15 +1646,14 @@
         aggregation_type=None,
         cross_series_group_by_columns=None,
         calendar_id=None,
         calendar_name=None,
         model_splits=None,
         allow_partial_history_time_series_predictions=False,
         unsupervised_mode=False,
-        unsupervised_type=None,
     ):
         self.project_id = project_id
         self.datetime_partitioning_id = datetime_partitioning_id
         self.datetime_partition_column = datetime_partition_column
         self.date_format = date_format
         self.autopilot_data_selection_method = autopilot_data_selection_method
         self.validation_duration = validation_duration
@@ -1718,15 +1698,14 @@
         self.calendar_id = calendar_id
         self.calendar_name = calendar_name
         self.model_splits = model_splits
         self.allow_partial_history_time_series_predictions = (
             allow_partial_history_time_series_predictions
         )
         self.unsupervised_mode = unsupervised_mode
-        self.unsupervised_type = unsupervised_type
 
     @classmethod
     def from_server_data(cls, data):  # pylint: disable=missing-function-docstring
         converted_data = cls._converter.check(from_api(data))
         converted_data["backtests"] = [
             Backtest(**backtest_data) for backtest_data in converted_data["backtests"]
         ]
@@ -2034,15 +2013,14 @@
             "calendar_id": self.calendar_id,
             "model_splits": self.model_splits,
             "disable_holdout": self.disable_holdout,
             "allow_partial_history_time_series_predictions": (
                 self.allow_partial_history_time_series_predictions
             ),
             "unsupervised_mode": self.unsupervised_mode,
-            "unsupervised_type": self.unsupervised_type,
         }
         if use_holdout_start_end_format:
             init_data["holdout_end_date"] = self.holdout_end_date
         else:
             init_data["holdout_duration"] = self.holdout_duration
 
         return DatetimePartitioningSpecification(**init_data)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     FrozenModel,
     Model,
     ModelParameters,
     PrimeModel,
     RatingTableModel,
 )
 from .modeljob import ModelJob
+from .notebooks import Notebook
 from .pairwise_statistics import (
     PairwiseConditionalProbabilities,
     PairwiseCorrelations,
     PairwiseJointProbabilities,
 )
 from .payoff_matrix import PayoffMatrix
 from .predict_job import PredictJob
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/application.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from typing import List, Optional
 
 import trafaret as t
 from typing_extensions import TypedDict
 
 from datarobot.enums import ApplicationPermissions
 from datarobot.models.api_object import APIObject
-from datarobot.models.use_cases.utils import resolve_use_cases, UseCaseLike
 from datarobot.utils.pagination import unpaginate
 
 
 class ApplicationDeployment(TypedDict):
     deployment_id: str
     reference_name: str
 
@@ -123,15 +122,15 @@
                 }
             ),
             t.Key("application_template_type", optional=True): t.String,
             t.Key("deactivation_status_id", optional=True): t.String,
             t.Key("created_first_name", optional=True): t.String,
             t.Key("creator_last_name", optional=True): t.String,
             t.Key("creator_userhash", optional=True): t.String,
-            t.Key("deployments", optional=True): t.List(
+            t.Key("deployments"): t.List(
                 t.Dict(
                     {
                         t.Key("deployment_id"): t.String,
                         t.Key("reference_name"): t.String,
                     }
                 )
             ),
@@ -193,36 +192,31 @@
         self.deployments = deployments
 
     @classmethod
     def list(
         cls,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
-        use_cases: Optional[UseCaseLike] = None,
     ) -> List[Application]:
         """
         Retrieve a list of user applications.
 
         Parameters
         ----------
         offset : Optional[int]
             Optional. Retrieve applications in a list after this number.
         limit : Optional[int]
             Optional. Retrieve only this number of applications.
-        use_cases: Optional[Union[UseCase, List[UseCase], str, List[str]]]
-            Optional. Filter available Applications by a specific Use Case or Use Cases.
-            Accepts either the entity or the ID.
 
         Returns
         -------
         applications : List[Application]
             The requested list of user applications.
         """
         query = {"offset": offset, "limit": limit}
-        query = resolve_use_cases(use_cases=use_cases, params=query)
         applications = unpaginate(initial_url=cls._path, initial_params=query, client=cls._client)
         return [cls.from_server_data(application) for application in applications]
 
     @classmethod
     def get(cls, application_id: str) -> Application:
         """
         Retrieve a single application.
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_monitoring_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
         username: Optional[str]
         full_name: Optional[str]
 
     class MonitoringAggregation(TypedDict):
         retention_policy: str
         retention_value: int
 
-    class PredictionColumnMap(TypedDict):
+    class PredictionColumMap(TypedDict):
         class_name: str
         column_name: str
 
     class MonitoringColumns(TypedDict):
-        predictions_columns: Optional[Union[str, PredictionColumnMap]]
+        predictions_columns: Optional[Union[str, PredictionColumMap]]
         association_id_column: Optional[str]
         actuals_value_column: Optional[str]
         acted_upon_column: Optional[str]
         actuals_timestamp_column: Optional[str]
 
     class MonitoringOutputSettings(TypedDict):
         unique_row_identifier_columns: List[str]
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_model_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,31 +5,26 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-from __future__ import annotations
-
 import contextlib
 import copy
 import json
 import os
-import time
-from typing import Any, cast, Dict, Iterable, List, Mapping, Optional, Tuple, Union
 
-from requests import Response
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
-from datarobot.errors import InvalidUsageError, TrainingDataAssignmentError
-from datarobot.models.api_object import APIObject, ServerDataType
+from datarobot.errors import InvalidUsageError
+from datarobot.models.api_object import APIObject
 from datarobot.models.job import filter_feature_impact_result
 from datarobot.models.validators import custom_model_feature_impact_trafaret
 from datarobot.utils import camelize
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution, wait_for_custom_resolution
 
 
@@ -41,151 +36,56 @@
     Attributes
     ----------
     field_name: str
         The required field names.  Required field names are defined by the
         environment's required_metadata_keys. This value will be added as an
         environment vairable when running custom models.
     value: str
-        The value for the required field.
+        the value for the required field.
     """
 
     _converter = t.Dict({t.Key("field_name"): String(), t.Key("value"): String()})
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "{}(field_name={!r}, value={!r})".format(
             self.__class__.__name__,
             self.field_name,
             self.value,
         )
 
-    def _set_values(self, field_name: str, value: str) -> None:
+    def _set_values(self, field_name, value):
         self.field_name = field_name
         self.value = value
 
-    def to_dict(self) -> Dict[str, str]:
-        return cast(
-            Dict[str, str],
-            self._converter.check({"field_name": self.field_name, "value": self.value}),
-        )
-
-
-class TrainingData(APIObject):
-    """Training data assigned to a DataRobot custom model version.
-
-    .. versionadded:: v3.2
-
-    Attributes
-    ----------
-    dataset_id: str
-        The ID of the dataset.
-    dataset_version_id: str
-        The ID of the dataset version.
-    dataset_name: str
-        The name of the dataset.
-    assignment_in_progress: bool
-        The status of the assignment in progress.
-    assignment_error: dict
-        The assignment error message.
-    """
-
-    _converter = t.Dict(
-        {
-            t.Key("dataset_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("dataset_version_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("dataset_name", optional=True): t.Or(String(), t.Null()),
-            t.Key("assignment_in_progress", optional=True): t.Bool(),
-            t.Key("assignment_error", optional=True): t.Dict(
-                {
-                    t.Key("message"): t.Or(String(), t.Null()),
-                }
-            )
-            | t.Null,
-        }
-    ).ignore_extra("*")
-
-    schema = _converter
-
-    def __init__(
-        self,
-        dataset_id: Optional[str] = None,
-        dataset_version_id: Optional[str] = None,
-        dataset_name: Optional[str] = None,
-        assignment_in_progress: Optional[str] = None,
-        assignment_error: Optional[Dict[str, str]] = None,
-    ) -> None:
-        self.dataset_id = dataset_id
-        self.dataset_version_id = dataset_version_id
-        self.dataset_name = dataset_name
-        self.assignment_in_progress = assignment_in_progress
-        self.assignment_error = assignment_error
-
-
-class HoldoutData(APIObject):
-    """Holdout data assigned to a DataRobot custom model version.
-
-    .. versionadded:: v3.2
-
-    Attributes
-    ----------
-    dataset_id: str
-        The ID of the dataset.
-    dataset_version_id: str
-        The ID of the dataset version.
-    dataset_name: str
-        The name of the dataset.
-    partition_column: str
-        The name of the partitions column.
-    """
-
-    _converter = t.Dict(
-        {
-            t.Key("dataset_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("dataset_version_id", optional=True): t.Or(String(), t.Null()),
-            t.Key("dataset_name", optional=True): t.Or(String(), t.Null()),
-            t.Key("partition_column", optional=True): t.Or(String(), t.Null()),
-        }
-    ).ignore_extra("*")
-
-    schema = _converter
-
-    def __init__(
-        self,
-        dataset_id: Optional[str] = None,
-        dataset_version_id: Optional[str] = None,
-        dataset_name: Optional[str] = None,
-        partition_column: Optional[str] = None,
-    ) -> None:
-        self.dataset_id = dataset_id
-        self.dataset_version_id = dataset_version_id
-        self.dataset_name = dataset_name
-        self.partition_column = partition_column
+    def to_dict(self):
+        return self._converter.check({"field_name": self.field_name, "value": self.value})
 
 
 class CustomModelFileItem(APIObject):
     """A file item attached to a DataRobot custom model version.
 
     .. versionadded:: v2.21
 
     Attributes
     ----------
     id: str
-        The ID of the file item.
+        id of the file item
     file_name: str
-        The name of the file item.
+        name of the file item
     file_path: str
-        The path of the file item.
+        path of the file item
     file_source: str
-        The source of the file item.
+        source of the file item
     created_at: str, optional
-        ISO-8601 formatted timestamp of when the version was created.
+        ISO-8601 formatted timestamp of when the version was created
     """
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
             t.Key("file_name"): String(),
             t.Key("file_path"): String(),
@@ -194,20 +94,20 @@
         }
     ).ignore_extra("*")
 
     schema = _converter
 
     def __init__(
         self,
-        id: str,
-        file_name: str,
-        file_path: str,
-        file_source: str,
-        created_at: Optional[str] = None,
-    ) -> None:
+        id,
+        file_name,
+        file_path,
+        file_source,
+        created_at=None,
+    ):
         self.id = id
         self.file_name = file_name
         self.file_path = file_path
         self.file_source = file_source
         self.created_at = created_at
 
 
@@ -215,23 +115,23 @@
     """Metadata about a DataRobot custom model version's dependency build
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     custom_model_id: str
-        The ID of the custom model.
+        id of the custom model
     custom_model_version_id: str
-        The ID of the custom model version.
+        id of the custom model version
     build_status: str
-        The status of the custom model version's dependency build.
+        the status of the custom model version's dependency build
     started_at: str
-        ISO-8601 formatted timestamp of when the build was started.
+        ISO-8601 formatted timestamp of when the build was started
     completed_at: str, optional
-        ISO-8601 formatted timestamp of when the build has completed.
+        ISO-8601 formatted timestamp of when the build has completed
     """
 
     _path = "customModels/{}/versions/{}/dependencyBuild/"
     _log_path = "customModels/{}/versions/{}/dependencyBuildLog/"
 
     _converter = t.Dict(
         {
@@ -241,100 +141,91 @@
             t.Key("build_start") >> "started_at": String(),
             t.Key("build_end", optional=True) >> "completed_at": String(allow_blank=True),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "{}(model={!r}, version={!r}, status={!r})".format(
             self.__class__.__name__,
             self.custom_model_id,
             self.custom_model_version_id,
             self.build_status,
         )
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        custom_model_id: str,
-        custom_model_version_id: str,
-        build_status: str,
-        started_at: str,
-        completed_at: Optional[str] = None,
-    ) -> None:
+        custom_model_id,
+        custom_model_version_id,
+        build_status,
+        started_at,
+        completed_at=None,
+    ):
         self.custom_model_id = custom_model_id
         self.custom_model_version_id = custom_model_version_id
         self.build_status = build_status
         self.started_at = started_at
         self.completed_at = completed_at
 
     @classmethod
-    def _update_server_data(
-        cls, server_data: Dict[str, Any], custom_model_id: str, custom_model_version_id: str
-    ) -> Dict[str, Any]:
+    def _update_server_data(cls, server_data, custom_model_id, custom_model_version_id):
         updated_data = copy.copy(server_data)
         updated_data.update(
             {"customModelId": custom_model_id, "customModelVersionId": custom_model_version_id}
         )
         return updated_data
 
     @classmethod
-    def get_build_info(
-        cls, custom_model_id: str, custom_model_version_id: str
-    ) -> CustomModelVersionDependencyBuild:
+    def get_build_info(cls, custom_model_id, custom_model_version_id):
         """Retrieve information about a custom model version's dependency build
 
         .. versionadded:: v2.22
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model.
+            the id of the custom model
         custom_model_version_id: str
-            The ID of the custom model version.
+            the id of the custom model version
 
         Returns
         -------
         CustomModelVersionDependencyBuild
-            The dependency build information.
+            the dependency build information
         """
         url = cls._path.format(custom_model_id, custom_model_version_id)
         response = cls._client.get(url)
         server_data = response.json()
         updated_data = cls._update_server_data(
             server_data, custom_model_id, custom_model_version_id
         )
         return cls.from_server_data(updated_data)
 
     @classmethod
-    def start_build(
-        cls,
-        custom_model_id: str,
-        custom_model_version_id: str,
-        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
-    ) -> Optional[CustomModelVersionDependencyBuild]:
+    def start_build(cls, custom_model_id, custom_model_version_id, max_wait=DEFAULT_MAX_WAIT):
         """Start the dependency build for a custom model version  dependency build
 
         .. versionadded:: v2.22
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model
+            the id of the custom model
         custom_model_version_id: str
-            the ID of the custom model version
+            the id of the custom model version
         max_wait: int, optional
-            Max time to wait for a build completion.
+            max time to wait for a build completion.
             If set to None - method will return without waiting.
         """
 
-        def build_complete(response: Response) -> Optional[CustomModelVersionDependencyBuild]:
+        def build_complete(response):
             data = response.json()
             if data["buildStatus"] in ["success", "failed"]:
                 updated_data = cls._update_server_data(
                     data, custom_model_id, custom_model_version_id
                 )
                 return cls.from_server_data(updated_data)
             return None
@@ -345,205 +236,191 @@
         if max_wait is None:
             server_data = response.json()
             updated_data = cls._update_server_data(
                 server_data, custom_model_id, custom_model_version_id
             )
             return cls.from_server_data(updated_data)
         else:
-            return cast(
-                Optional[CustomModelVersionDependencyBuild],
-                wait_for_custom_resolution(cls._client, url, build_complete, max_wait),
-            )
+            return wait_for_custom_resolution(cls._client, url, build_complete, max_wait)
 
-    def get_log(self) -> str:
+    def get_log(self):
         """Get log of a custom model version dependency build.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status
         """
         url = self._log_path.format(self.custom_model_id, self.custom_model_version_id)
-        return cast(str, self._client.get(url).text)
+        return self._client.get(url).text
 
-    def cancel(self) -> None:
+    def cancel(self):
         """Cancel custom model version dependency build that is in progress.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status
         """
         url = self._path.format(self.custom_model_id, self.custom_model_version_id)
         self._client.delete(url)
 
-    def refresh(self) -> None:
+    def refresh(self):
         """Update custom model version dependency build with the latest data from server.
 
         .. versionadded:: v2.22
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status
         """
         url = self._path.format(self.custom_model_id, self.custom_model_version_id)
 
         response = self._client.get(url)
 
         data = response.json()
         updated_data = self._update_server_data(
             data, self.custom_model_id, self.custom_model_version_id
         )
-        self._set_values(**self._safe_data(updated_data, do_recursive=True))  # type: ignore[no-untyped-call]
+        self._set_values(**self._safe_data(updated_data, do_recursive=True))
 
 
 class CustomDependencyConstraint(APIObject):
     """Metadata about a constraint on a dependency of a custom model version
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     constraint_type: str
-        How the dependency should be constrained by version (<, <=, ==, >=, >).
+        How the dependency should be constrained by version (<, <=, ==, >=, >)
     version: str
-        The version to use in the dependency's constraint.
+        The version to use in the dependency's constraint
     """
 
     _converter = t.Dict(
         {t.Key("constraint_type"): String(), t.Key("version"): String()}
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "{}(constraint_type={!r}, version={!r})".format(
             self.__class__.__name__,
             self.constraint_type,
             self.version,
         )
 
-    def _set_values(self, constraint_type: str, version: str) -> None:
+    def _set_values(self, constraint_type, version):
         self.constraint_type = constraint_type
         self.version = version
 
 
 class CustomDependency(APIObject):
     """Metadata about an individual dependency of a custom model version
 
     .. versionadded:: v2.22
 
     Attributes
     ----------
     package_name: str
-        The dependency's package name.
+        The dependency's package name
     constraints: List[CustomDependencyConstraint]
-        Version constraints to apply on the dependency.
+        Version constraints to apply on the dependency
     line: str
-        The original line from the requirements file.
+        The original line from the requirements file
     line_number: int
-        The line number the requirement was on in the requirements file.
+        The line number the requirement was on in the requirements file
     """
 
     _converter = t.Dict(
         {
             t.Key("package_name"): String(),
             t.Key("constraints"): t.List(CustomDependencyConstraint.schema),
             t.Key("line"): String(),
             t.Key("line_number"): Int(gt=0),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "{}(package_name={!r}, constraints={!r})".format(
             self.__class__.__name__,
             self.package_name,
             self.constraints,
         )
 
-    def _set_values(  # pylint: disable=missing-function-docstring
-        self,
-        package_name: str,
-        constraints: List[CustomDependencyConstraint],
-        line: str,
-        line_number: int,
-    ) -> None:
+    def _set_values(self, package_name, constraints, line, line_number):
         self.package_name = package_name
-        # TODO: maybe CustomDependencyConstraint should be implemented as TypedDict
-        self.constraints = [CustomDependencyConstraint(**c) for c in constraints]  # type: ignore[arg-type]
+        self.constraints = [CustomDependencyConstraint(**c) for c in constraints]
         self.line = line
         self.line_number = line_number
 
 
 class CustomModelVersion(APIObject):
     """A version of a DataRobot custom model.
 
     .. versionadded:: v2.21
 
     Attributes
     ----------
     id: str
-        The ID of the custom model version.
+        id of the custom model version
     custom_model_id: str
-        The ID of the custom model.
+        id of the custom model
     version_minor: int
-        A minor version number of the custom model version.
+        a minor version number of custom model version
     version_major: int
-        A major version number of the custom model version.
+        a major version number of custom model version
     is_frozen: bool
-        A flag if the custom model version is frozen.
+        a flag if the custom model version is frozen
     items: List[CustomModelFileItem]
-        A list of file items attached to the custom model version.
+        a list of file items attached to the custom model version
     base_environment_id: str
-        The ID of the environment to use with the model.
+        id of the environment to use with the model
     base_environment_version_id: str
-        The ID of the environment version to use with the model.
+        id of the environment version to use with the model
     label: str, optional
-        A short human readable string to label the version.
+        short human readable string to label the version
     description: str, optional
-        The custom model version description.
+        custom model version description
     created_at: str, optional
-        ISO-8601 formatted timestamp of when the version was created.
+        ISO-8601 formatted timestamp of when the version was created
     dependencies: List[CustomDependency]
-        The parsed dependencies of the custom model version if the
-        version has a valid requirements.txt file.
+        the parsed dependencies of the custom model version if the
+        version has a valid requirements.txt file
     network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
         Determines whether the given custom model is isolated, or can access the public network.
-        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
+        Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
     maximum_memory: int, optional
         The maximum memory that might be allocated by the custom-model.
-        If exceeded, the custom-model will be killed by k8s.
+        If exceeded, the custom-model will be killed by k8s
     replicas: int, optional
-        A fixed number of replicas that will be deployed in the cluster.
+        A fixed number of replicas that will be deployed in the cluster
     required_metadata_values: List[RequiredMetadataValue]
         Additional parameters required by the execution environment. The required keys are
         defined by the fieldNames in the base environment's requiredMetadataKeys.
-    training_data: TrainingData, optional
-        The information about the training data assigned to the model version.
-    holdout_data: HoldoutData, optional
-        The information about the holdout data assigned to the model version.
     """
 
     _path = "customModels/{}/versions/"
 
     _converter = t.Dict(
         {
             t.Key("id"): String(),
@@ -562,392 +439,224 @@
             ),
             t.Key("created", optional=True) >> "created_at": String(),
             t.Key("dependencies", optional=True): t.List(CustomDependency.schema),
             t.Key("network_egress_policy", optional=True): t.Enum(*NETWORK_EGRESS_POLICY.ALL),
             t.Key("maximum_memory", optional=True): Int(),
             t.Key("replicas", optional=True): Int(),
             t.Key("required_metadata_values", optional=True): t.List(RequiredMetadataValue.schema),
-            t.Key("training_data", optional=True): t.Or(TrainingData.schema, t.Null()),
-            t.Key("holdout_data", optional=True): t.Or(HoldoutData.schema, t.Null()),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return f"{self.__class__.__name__}({self.label or self.id!r})"
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        id: str,
-        custom_model_id: str,
-        version_minor: int,
-        version_major: int,
-        is_frozen: bool,
-        items: List[CustomModelFileItem],
-        base_environment_id: Optional[str] = None,
-        base_environment_version_id: Optional[str] = None,
-        label: Optional[str] = None,
-        description: Optional[str] = None,
-        created_at: Optional[str] = None,
-        dependencies: Optional[List[CustomDependency]] = None,
-        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
-        maximum_memory: Optional[int] = None,
-        replicas: Optional[int] = None,
-        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
-        training_data: Optional[Mapping[str, Any]] = None,
-        holdout_data: Optional[Mapping[str, Any]] = None,
-    ) -> None:
+        id,
+        custom_model_id,
+        version_minor,
+        version_major,
+        is_frozen,
+        items,
+        base_environment_id=None,
+        base_environment_version_id=None,
+        label=None,
+        description=None,
+        created_at=None,
+        dependencies=None,
+        network_egress_policy=None,
+        maximum_memory=None,
+        replicas=None,
+        required_metadata_values=None,
+    ):
         self.id = id
         self.custom_model_id = custom_model_id
         self.version_minor = version_minor
         self.version_major = version_major
         self.is_frozen = is_frozen
-        self.items = [CustomModelFileItem(**item) for item in items]  # type: ignore[arg-type]
+        self.items = [CustomModelFileItem(**item) for item in items]
         self.base_environment_id = base_environment_id
         self.base_environment_version_id = base_environment_version_id
         self.label = label
         self.description = description
         self.created_at = created_at
-        self.dependencies = [CustomDependency(**dep) for dep in dependencies or []]  # type: ignore[arg-type]
+        self.dependencies = [CustomDependency(**dep) for dep in dependencies or []]
         self.network_egress_policy = network_egress_policy
         self.maximum_memory = maximum_memory
         self.replicas = replicas
         self.required_metadata_values = (
-            [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]  # type: ignore[arg-type]
+            [RequiredMetadataValue.from_server_data(val) for val in required_metadata_values]
             if required_metadata_values
             else None
         )
-        self.training_data = TrainingData(**training_data) if training_data else None
-        self.holdout_data = HoldoutData(**holdout_data) if holdout_data else None
 
     @classmethod
-    def from_server_data(
-        cls, data: ServerDataType, keep_attrs: Optional[Iterable[str]] = None
-    ) -> CustomModelVersion:
+    def from_server_data(cls, data, keep_attrs=None):
         initial = super().from_server_data(data, keep_attrs)
         # from_server_data will make the keys in requiredMetadata lowercase,
         # which is not OK. we need to preserve case
-        initial.required_metadata = data.get("requiredMetadata")  # type: ignore[union-attr]
+        initial.required_metadata = data.get("requiredMetadata")
         return initial
 
     @classmethod
     def create_clean(
         cls,
-        custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
-        folder_path: Optional[str] = None,
-        files: Optional[List[Tuple[str, str]]] = None,
-        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
-        maximum_memory: Optional[int] = None,
-        replicas: Optional[int] = None,
-        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
-        training_dataset_id: Optional[str] = None,
-        partition_column: Optional[str] = None,
-        holdout_dataset_id: Optional[str] = None,
-        keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
-    ) -> CustomModelVersion:
+        custom_model_id,
+        base_environment_id,
+        is_major_update=True,
+        folder_path=None,
+        files=None,
+        network_egress_policy=None,
+        maximum_memory=None,
+        replicas=None,
+        required_metadata_values=None,
+    ):
         """Create a custom model version without files from previous versions.
 
-           Create a version with training or holdout data:
-           If training/holdout data related parameters are provided,
-           the training data is assigned asynchronously.
-           In this case:
-           * if max_wait is not None, the function returns once the job is finished.
-           * if max_wait is None, the function returns immediately. Progress can be polled by the user (see examples).
-
-           If training data assignment fails, new version is still created,
-           but it is not allowed to create a model package for the model version and to deploy it.
-           To check for training data assignment error, check version.training_data.assignment_error["message"].
-
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model.
+            the id of the custom model
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
+            the id of the base environment to use with the custom model version
         is_major_update: bool
-            The flag defining if a custom model version will be a minor or a major version.
+            the flag defining if a custom model version
+            will be a minor or a major version.
             Default to `True`
         folder_path: str, optional
-            The path to a folder containing files to be uploaded.
-            Each file in the folder is uploaded under path relative to a folder path.
+            the path to a folder containing files to be uploaded.
+            Each file in the folder is uploaded under path relative
+            to a folder path
         files: list, optional
-            The list of tuples, where values in each tuple are the local filesystem path and
+            the list of tuples, where values in each tuple are the local filesystem path and
             the path the file should be placed in the model.
-            If the list is of strings, then basenames will be used for tuples.
+            if list is of strings, then basenames will be used for tuples
             Example:
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
-            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'.
+            Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
-            If exceeded, the custom-model will be killed by k8s.
+            If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
-            A fixed number of replicas that will be deployed in the cluster.
+            A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
-        training_dataset_id: str, optional
-            The ID of the training dataset to assign to the custom model.
-        partition_column: str, optional
-            Name of a partition column in a training dataset assigned to the custom model.
-            Can only be assigned for structured models.
-        holdout_dataset_id: str, optional
-            The ID of the holdout dataset to assign to the custom model.
-            Can only be assigned for unstructured models.
-        keep_training_holdout_data: bool, optional
-            If the version should inherit training and holdout data from the previous version.
-            Defaults to True.
-            This field is only applicable if the model has training data for versions enabled,
-            otherwise the field value will be ignored.
-        max_wait: int, optional
-            Max time to wait for training data assignment.
-            If set to None - method will return without waiting.
-            Defaults to 10 minutes.
 
         Returns
         -------
         CustomModelVersion
-            Created custom model version.
+            created custom model version
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
-        datarobot.errors.InvalidUsageError
-            If wrong parameters are provided.
-        datarobot.errors.TrainingDataAssignmentError
-            If training data assignment fails.
-
-        Examples
-        --------
-        Create a version with blocking (default max_wait=600) training data assignment:
-
-        .. code-block:: python
-
-            import datarobot as dr
-            from datarobot.errors import TrainingDataAssignmentError
-
-            dr.Client(token=my_token, endpoint=endpoint)
-
-            try:
-                version = dr.CustomModelVersion.create_from_previous(
-                    custom_model_id="6444482e5583f6ee2e572265",
-                    base_environment_id="642209acc563893014a41e24",
-                    training_dataset_id="6421f2149a4f9b1bec6ad6dd",
-                )
-            except TrainingDataAssignmentError as e:
-                print(e)
-
-        Create a version with non-blocking training data assignment:
-
-        .. code-block:: python
-
-            import datarobot as dr
-
-            dr.Client(token=my_token, endpoint=endpoint)
-
-            version = dr.CustomModelVersion.create_from_previous(
-                custom_model_id="6444482e5583f6ee2e572265",
-                base_environment_id="642209acc563893014a41e24",
-                training_dataset_id="6421f2149a4f9b1bec6ad6dd",
-                max_wait=None,
-            )
-
-            while version.training_data.assignment_in_progress:
-                time.sleep(10)
-                version.refresh()
-            if version.training_data.assignment_error:
-                print(version.training_data.assignment_error["message"])
+            if the server responded with 5xx status
         """
-        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
-            files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
+        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):
+            files = [(filename, os.path.basename(filename)) for filename in files]
         return cls._create(
             "post",
             custom_model_id,
             is_major_update,
             base_environment_id,
             folder_path,
             files,
-            extra_upload_data=None,
             network_egress_policy=network_egress_policy,
             maximum_memory=maximum_memory,
             replicas=replicas,
             required_metadata_values=required_metadata_values,
-            training_dataset_id=training_dataset_id,
-            partition_column=partition_column,
-            holdout_dataset_id=holdout_dataset_id,
-            keep_training_holdout_data=keep_training_holdout_data,
-            max_wait=max_wait,
         )
 
     @classmethod
     def create_from_previous(
         cls,
-        custom_model_id: str,
-        base_environment_id: str,
-        is_major_update: bool = True,
-        folder_path: Optional[str] = None,
-        files: Optional[List[Tuple[str, str]]] = None,
-        files_to_delete: Optional[List[str]] = None,
-        network_egress_policy: Optional[NETWORK_EGRESS_POLICY] = None,
-        maximum_memory: Optional[int] = None,
-        replicas: Optional[int] = None,
-        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
-        training_dataset_id: Optional[str] = None,
-        partition_column: Optional[str] = None,
-        holdout_dataset_id: Optional[str] = None,
-        keep_training_holdout_data: Optional[bool] = None,
-        max_wait: int = DEFAULT_MAX_WAIT,
-    ) -> CustomModelVersion:
+        custom_model_id,
+        base_environment_id,
+        is_major_update=True,
+        folder_path=None,
+        files=None,
+        files_to_delete=None,
+        network_egress_policy=None,
+        maximum_memory=None,
+        replicas=None,
+        required_metadata_values=None,
+    ):
         """Create a custom model version containing files from a previous version.
 
-           Create a version with training/holdout data:
-           If training/holdout data related parameters are provided,
-           the training data is assigned asynchronously.
-           In this case:
-           * if max_wait is not None, function returns once job is finished.
-           * if max_wait is None, function returns immediately, progress can be polled by the user, see examples.
-
-           If training data assignment fails, new version is still created,
-           but it is not allowed to create a model package for the model version and to deploy it.
-           To check for training data assignment error, check version.training_data.assignment_error["message"].
-
-
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model.
+            the id of the custom model
         base_environment_id: str
-            The ID of the base environment to use with the custom model version.
+            the id of the base environment to use with the custom model version
         is_major_update: bool, optional
-            The flag defining if a custom model version will be a minor or a major version.
-            Defaults to `True`.
+            the flag defining if a custom model version
+            will be a minor or a major version.
+            Default to `True`
         folder_path: str, optional
-            The path to a folder containing files to be uploaded.
-            Each file in the folder is uploaded under path relative to a folder path.
+            the path to a folder containing files to be uploaded.
+            Each file in the folder is uploaded under path relative
+            to a folder path
         files: list, optional
-            The list of tuples, where values in each tuple are the local filesystem path and
+            the list of tuples, where values in each tuple are the local filesystem path and
             the path the file should be placed in the model.
-            If list is of strings, then basenames will be used for tuples
+            if list is of strings, then basenames will be used for tuples
             Example:
             [("/home/user/Documents/myModel/file1.txt", "file1.txt"),
             ("/home/user/Documents/myModel/folder/file2.txt", "folder/file2.txt")]
             or
             ["/home/user/Documents/myModel/file1.txt",
             "/home/user/Documents/myModel/folder/file2.txt"]
         files_to_delete: list, optional
-            The list of a file items ids to be deleted.
+            the list of a file items ids to be deleted
             Example: ["5ea95f7a4024030aba48e4f9", "5ea6b5da402403181895cc51"]
         network_egress_policy: datarobot.NETWORK_EGRESS_POLICY, optional
             Determines whether the given custom model is isolated, or can access the public network.
             Can be either 'datarobot.NONE' or 'datarobot.PUBLIC'
         maximum_memory: int, optional
             The maximum memory that might be allocated by the custom-model.
             If exceeded, the custom-model will be killed by k8s
         replicas: int, optional
             A fixed number of replicas that will be deployed in the cluster
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
-        training_dataset_id: str, optional
-            The ID of the training dataset to assign to the custom model.
-        partition_column: str, optional
-            Name of a partition column in a training dataset assigned to the custom model.
-            Can only be assigned for structured models.
-        holdout_dataset_id: str, optional
-            The ID of the holdout dataset to assign to the custom model.
-            Can only be assigned for unstructured models.
-        keep_training_holdout_data: bool, optional
-            If the version should inherit training and holdout data from the previous version.
-            Defaults to True.
-            This field is only applicable if the model has training data for versions enabled,
-            otherwise the field value will be ignored.
-        max_wait: int, optional
-            Max time to wait for training data assignment.
-            If set to None - method will return without waiting.
-            Defaults to 10 minutes.
 
         Returns
         -------
         CustomModelVersion
             created custom model version
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
-        datarobot.errors.InvalidUsageError
-            If wrong parameters are provided.
-        datarobot.errors.TrainingDataAssignmentError
-            If training data assignment fails.
-
-        Examples
-        --------
-        Create a version with blocking (default max_wait=600) training data assignment:
-
-        .. code-block:: python
-
-            import datarobot as dr
-            from datarobot.errors import TrainingDataAssignmentError
-
-            dr.Client(token=my_token, endpoint=endpoint)
-
-            try:
-                version = dr.CustomModelVersion.create_from_previous(
-                    custom_model_id="6444482e5583f6ee2e572265",
-                    base_environment_id="642209acc563893014a41e24",
-                    training_dataset_id="6421f2149a4f9b1bec6ad6dd",
-                )
-            except TrainingDataAssignmentError as e:
-                print(e)
-
-        Create a version with non-blocking training data assignment:
-
-        .. code-block:: python
-
-            import datarobot as dr
-
-            dr.Client(token=my_token, endpoint=endpoint)
-
-            version = dr.CustomModelVersion.create_from_previous(
-                custom_model_id="6444482e5583f6ee2e572265",
-                base_environment_id="642209acc563893014a41e24",
-                training_dataset_id="6421f2149a4f9b1bec6ad6dd",
-                max_wait=None,
-            )
-
-            while version.training_data.assignment_in_progress:
-                time.sleep(10)
-                version.refresh()
-            if version.training_data.assignment_error:
-                print(version.training_data.assignment_error["message"])
-
+            if the server responded with 5xx status
         """
-        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):  # type: ignore[unreachable]
-            files = [(filename, os.path.basename(filename)) for filename in files]  # type: ignore[unreachable]
+        if files and not isinstance(files[0], tuple) and isinstance(files[0], str):
+            files = [(filename, os.path.basename(filename)) for filename in files]
         if files_to_delete:
             upload_data = [("filesToDelete", file_id) for file_id in files_to_delete]
         else:
             upload_data = None
         return cls._create(
             "patch",
             custom_model_id,
@@ -956,90 +665,35 @@
             folder_path,
             files,
             upload_data,
             network_egress_policy,
             maximum_memory,
             replicas,
             required_metadata_values=required_metadata_values,
-            training_dataset_id=training_dataset_id,
-            partition_column=partition_column,
-            holdout_dataset_id=holdout_dataset_id,
-            keep_training_holdout_data=keep_training_holdout_data,
-            max_wait=max_wait,
         )
 
     @classmethod
-    def _create(
+    def _create(  # pylint: disable=missing-function-docstring
         cls,
-        method: str,
-        custom_model_id: str,
-        is_major_update: bool,
-        base_environment_id: str,
-        folder_path: Optional[str],
-        files: Optional[List[Tuple[str, str]]],
-        extra_upload_data: Optional[List[Tuple[str, Any]]],
-        network_egress_policy: Optional[NETWORK_EGRESS_POLICY],
-        maximum_memory: Optional[int],
-        replicas: Optional[int],
-        required_metadata_values: Optional[List[RequiredMetadataValue]],
-        training_dataset_id: Optional[str],
-        partition_column: Optional[str],
-        holdout_dataset_id: Optional[str],
-        keep_training_holdout_data: Optional[bool],
-        max_wait: Optional[int],
-    ) -> CustomModelVersion:
-        # TODO: pass model object
-        """Create a custom model version"""
-
-        def _wait_for_training_data_assignment(version: CustomModelVersion) -> None:
-            # This check is needed to make sure user explicitly passes new training data.
-            # Checking only for `version.training_data.assignment_in_progress` is not enough as it is not known
-            # whether this training data is new or copied from the previous version.
-            # TODO: replace `not holdout_dataset_id` with `not model.is_unstructured_model_kind`
-            #  once `model` entity is introduced in the API
-            if training_dataset_id and max_wait and not holdout_dataset_id:
-                start_time = time.time()
-                while time.time() < start_time + max_wait:
-                    version.refresh()
-                    if (
-                        not version.training_data
-                        or not version.training_data.assignment_in_progress
-                    ):
-                        break
-                    time.sleep(5)
-
-                if version.training_data and version.training_data.assignment_error:
-                    raise TrainingDataAssignmentError(
-                        version.custom_model_id,
-                        version.id,
-                        version.training_data.assignment_error["message"],
-                    )
-
+        method,
+        custom_model_id,
+        is_major_update,
+        base_environment_id,
+        folder_path=None,
+        files=None,
+        extra_upload_data=None,
+        network_egress_policy=None,
+        maximum_memory=None,
+        replicas=None,
+        required_metadata_values=None,
+    ):
         url = cls._path.format(custom_model_id)
 
         with contextlib.ExitStack() as stack:
-            # TODO: add training data params checks depending on structured/unstructured model kind.
-            if not training_dataset_id and (holdout_dataset_id or partition_column):
-                raise InvalidUsageError(
-                    "It is not allowed to provide holdout data or partition column without training data."
-                )
-
-            if holdout_dataset_id and partition_column:
-                raise InvalidUsageError(
-                    "It is not allowed to provide holdout_dataset_id and partition_column at the same time. "
-                    "For regular(structured) models you can provide training_dataset_id and partition_column. "
-                    "For unstructured models you can provide training_dataset_id and holdout_dataset_id."
-                )
-
-            if keep_training_holdout_data and (training_dataset_id or holdout_dataset_id):
-                raise InvalidUsageError(
-                    "It is not allowed to keep existing training/holdout data and to provide a new ones."
-                )
-
-            upload_data: List[Tuple[str, Any]] = [
+            upload_data = [
                 ("isMajorUpdate", str(is_major_update)),
                 ("baseEnvironmentId", base_environment_id),
             ]
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
                     for path in file_paths:
@@ -1077,191 +731,162 @@
                                 {camelize(k): v for k, v in val.to_dict().items()}
                                 for val in required_metadata_values
                             ]
                         ),
                     )
                 )
 
-            if training_dataset_id:
-                keep_training_holdout_data = False
-
-                td_payload = {
-                    "datasetId": training_dataset_id,
-                }
-                upload_data.append(("trainingData", json.dumps(td_payload)))
-
-                # If holdout data is not provided don't include it in the payload with None values.
-                # There should be more checks added in the API.
-                hd_payload = {}
-                if holdout_dataset_id:
-                    hd_payload["datasetId"] = holdout_dataset_id
-                if partition_column:
-                    hd_payload["partitionColumn"] = partition_column
-
-                if len(hd_payload):
-                    upload_data.append(("holdoutData", json.dumps(hd_payload)))
-            if keep_training_holdout_data is not None:
-                upload_data.append(("keepTrainingHoldoutData", str(keep_training_holdout_data)))
-
             encoder = MultipartEncoder(fields=upload_data)
             headers = {"Content-Type": encoder.content_type}
             response = cls._client.request(method, url, data=encoder, headers=headers)
-            new_version = cls.from_server_data(response.json())
-
-            _wait_for_training_data_assignment(new_version)
-
-        return new_version
+            return cls.from_server_data(response.json())
 
     @classmethod
-    def list(cls, custom_model_id: str) -> List[CustomModelVersion]:
+    def list(cls, custom_model_id):
         """List custom model versions.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model.
+            the id of the custom model
 
         Returns
         -------
         List[CustomModelVersion]
-            A list of custom model versions.
+            a list of custom model versions
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status
         """
         url = cls._path.format(custom_model_id)
         data = unpaginate(url, None, cls._client)
         return [cls.from_server_data(item) for item in data]
 
     @classmethod
-    def get(cls, custom_model_id: str, custom_model_version_id: str) -> CustomModelVersion:
+    def get(cls, custom_model_id, custom_model_version_id):
         """Get custom model version by id.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         custom_model_id: str
-            The ID of the custom model.
+            the id of the custom model
         custom_model_version_id: str
-            The id of the custom model version to retrieve.
+            the id of the custom model version to retrieve
 
         Returns
         -------
         CustomModelVersion
-            Retrieved custom model version.
+            retrieved custom model version
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
         url = cls._path.format(custom_model_id)
         path = f"{url}{custom_model_version_id}/"
         return cls.from_location(path)
 
-    def download(self, file_path: str) -> None:
+    def download(self, file_path):
         """Download custom model version.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         file_path: str
-            Path to create a file with custom model version content.
+            path to create a file with custom model version content
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/download/"
 
         response = self._client.get(path)
         with open(file_path, "wb") as f:
             f.write(response.content)
 
-    def update(
-        self,
-        description: Optional[str] = None,
-        required_metadata_values: Optional[List[RequiredMetadataValue]] = None,
-    ) -> None:
+    def update(self, description=None, required_metadata_values=None):
         """Update custom model version properties.
 
         .. versionadded:: v2.21
 
         Parameters
         ----------
         description: str
-            New custom model version description.
+            new custom model version description
         required_metadata_values: List[RequiredMetadataValue]
             Additional parameters required by the execution environment. The required keys are
             defined by the fieldNames in the base environment's requiredMetadataKeys.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
-        payload: Dict[str, Any] = {}
+        payload = {}
         if description:
             payload.update({"description": description})
 
         if required_metadata_values is not None:
             payload.update(
                 {"requiredMetadataValues": [val.to_dict() for val in required_metadata_values]}
             )
 
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/"
 
         response = self._client.patch(path, data=payload)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
+        self._set_values(**self._safe_data(data, do_recursive=True))
         # _safe_data will make the keys in requiredMetadata lowercase,
         # which is not OK. we need to preserve case
         self.required_metadata = data.get(  # pylint: disable=attribute-defined-outside-init
             "requiredMetadata"
         )
 
-    def refresh(self) -> None:
+    def refresh(self):
         """Update custom model version with the latest data from server.
 
         .. versionadded:: v2.21
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/"
 
         response = self._client.get(path)
 
         data = response.json()
-        self._set_values(**self._safe_data(data, do_recursive=True))  # type: ignore[no-untyped-call]
+        self._set_values(**self._safe_data(data, do_recursive=True))
 
-    def get_feature_impact(self, with_metadata: bool = False) -> List[Dict[str, Any]]:
+    def get_feature_impact(self, with_metadata=False):
         """Get custom model feature impact.
 
         .. versionadded:: v2.23
 
         Parameters
         ----------
         with_metadata : bool
@@ -1272,34 +897,33 @@
         feature_impacts : list of dict
            The feature impact data. Each item is a dict with the keys 'featureName',
            'impactNormalized', and 'impactUnnormalized', and 'redundantWith'.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
         url = self._path.format(self.custom_model_id)
         path = f"{url}{self.id}/featureImpact/"
         data = self._client.get(path).json()
         data = custom_model_feature_impact_trafaret.check(data)
-        ret = filter_feature_impact_result(data, with_metadata=with_metadata)  # type: ignore[no-untyped-call]
-        return ret  # type: ignore[no-any-return]
+        return filter_feature_impact_result(data, with_metadata=with_metadata)
 
-    def calculate_feature_impact(self, max_wait: int = DEFAULT_MAX_WAIT) -> None:
+    def calculate_feature_impact(self, max_wait=DEFAULT_MAX_WAIT):
         """Calculate custom model feature impact.
 
         .. versionadded:: v2.23
 
         Parameters
         ----------
         max_wait: int, optional
-            Max time to wait for feature impact calculation.
+            max time to wait for feature impact calculation.
             If set to None - method will return without waiting.
             Defaults to 10 min
 
         Raises
         ------
         datarobot.errors.ClientError
             if the server responded with 4xx status
@@ -1318,21 +942,21 @@
     """A conversion of a DataRobot custom model version.
 
     .. versionadded:: v2.27
 
     Attributes
     ----------
     id: str
-        The ID of the custom model version conversion.
+        ID of the custom model version conversion.
     custom_model_version_id: str
-        The ID of the custom model version.
+        ID of the custom model version.
     created: str
         ISO-8601 timestamp of when the custom model conversion created.
     main_program_item_id: str or None
-        The ID of the main program item.
+        ID of the main program item.
     log_message: str or None
         The conversion output log message.
     generated_metadata: dict or None
         The dict contains two items: 'outputDataset' & 'outputColumns'.
     conversion_succeeded: bool
         Whether the conversion succeeded or not.
     conversion_in_progress: bool
@@ -1362,121 +986,117 @@
             t.Key("conversion_in_progress", optional=True): t.Bool() | t.Null(),
             t.Key("should_stop", optional=True): t.Bool(),
         }
     ).ignore_extra("*")
 
     schema = _converter
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs):
         self._set_values(**kwargs)
         self.custom_model_id = None
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return f"{self.__class__.__name__}({self.id!r})"
 
     def _set_values(  # pylint: disable=missing-function-docstring
         self,
-        id: str,
-        custom_model_version_id: str,
-        created: str,
-        main_program_item_id: Optional[str] = None,
-        log_message: Optional[str] = None,
-        generated_metadata: Optional[Dict[str, Union[List[str], List[List[str]]]]] = None,
-        conversion_succeeded: Optional[bool] = None,
-        conversion_in_progress: Optional[bool] = None,
-        should_stop: Optional[bool] = None,
-    ) -> None:
+        id,
+        custom_model_version_id,
+        created,
+        main_program_item_id=None,
+        log_message=None,
+        generated_metadata=None,
+        conversion_succeeded=None,
+        conversion_in_progress=None,
+        should_stop=None,
+    ):
         self.id = id
         self.custom_model_version_id = custom_model_version_id
         self.created = created
         self.main_program_item_id = main_program_item_id
         self.log_message = log_message
         self.generated_metadata = generated_metadata
         self.conversion_succeeded = conversion_succeeded
         self.conversion_in_progress = conversion_in_progress
         self.should_stop = should_stop
 
     @classmethod
     def run_conversion(
         cls,
-        custom_model_id: str,
-        custom_model_version_id: str,
-        main_program_item_id: str,
-        max_wait: Optional[int] = None,
-    ) -> str:
+        custom_model_id,
+        custom_model_version_id,
+        main_program_item_id,
+        max_wait=None,
+    ):
         """Initiate a new custom model version conversion.
 
         Parameters
         ----------
         custom_model_id : str
             The associated custom model ID.
         custom_model_version_id : str
             The associated custom model version ID.
         main_program_item_id : str
             The selected main program item ID. This should be one of the SAS items in the
             associated custom model version.
         max_wait: int or None
-            Max wait time in seconds. If None, then don't wait.
+            Max wait time in seconds. If None, than don't wait.
 
         Returns
         -------
         conversion_id : str
             The ID of the newly created conversion entity.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx statuscustom model conversion
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         payload = {"mainProgramItemId": main_program_item_id}
         response = cls._client.post(base_conversion_url, json=payload)
         if max_wait is not None:
             wait_for_async_resolution(cls._client, response.headers["Location"], max_wait)
-        return cast(str, response.json()["conversionId"])
+        return response.json()["conversionId"]
 
     @classmethod
-    def stop_conversion(
-        cls, custom_model_id: str, custom_model_version_id: str, conversion_id: str
-    ) -> Response:
+    def stop_conversion(cls, custom_model_id, custom_model_version_id, conversion_id):
         """
         Stop a conversion that is in progress.
 
         Parameters
         ----------
         custom_model_id : str
-            The ID of the associated custom model.
+            ID of the associated custom model.
         custom_model_version_id : str
-            The ID of the associated custom model version.
+            ID of the associated custom model version.
         conversion_id :
-            THe ID of a conversion that is in-progress.
+            ID of a conversion that is in-progress.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
 
         conversion = cls.get(custom_model_id, custom_model_version_id, conversion_id)
         if not conversion.conversion_in_progress:
             raise InvalidUsageError("You may only stop a conversion that is in progress.")
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         conversion_entity_url = "{}{}/".format(base_conversion_url, conversion_id)
-        return cast(Response, cls._client.delete(conversion_entity_url))
+        return cls._client.delete(conversion_entity_url)
 
     @classmethod
-    def get(
-        cls, custom_model_id: str, custom_model_version_id: str, conversion_id: str
-    ) -> CustomModelVersionConversion:
+    def get(cls, custom_model_id, custom_model_version_id, conversion_id):
         """Get custom model version conversion by id.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1490,27 +1110,25 @@
         -------
         CustomModelVersionConversion
             Retrieved custom model version conversion.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         conversion_entity_url = "{}{}/".format(base_conversion_url, conversion_id)
         return cls.from_location(conversion_entity_url)
 
     @classmethod
-    def get_latest(
-        cls, custom_model_id: str, custom_model_version_id: str
-    ) -> Optional[CustomModelVersionConversion]:
+    def get_latest(cls, custom_model_id, custom_model_version_id):
         """Get latest custom model version conversion for a given custom model version.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1522,27 +1140,25 @@
         -------
         CustomModelVersionConversion or None
             Retrieved latest conversion for a given custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         data = unpaginate(base_conversion_url, {"isLatest": True}, cls._client)
         return cls.from_server_data(next(data))
 
     @classmethod
-    def list(
-        cls, custom_model_id: str, custom_model_version_id: str
-    ) -> List[CustomModelVersionConversion]:
+    def list(cls, custom_model_id, custom_model_version_id):
         """Get custom model version conversions list per custom model version.
 
         .. versionadded:: v2.27
 
         Parameters
         ----------
         custom_model_id: str
@@ -1554,15 +1170,15 @@
         -------
         List[CustomModelVersionConversion]
             Retrieved conversions for a given custom model version.
 
         Raises
         ------
         datarobot.errors.ClientError
-            If the server responded with 4xx status.
+            if the server responded with 4xx status.
         datarobot.errors.ServerError
-            If the server responded with 5xx status.
+            if the server responded with 5xx status.
         """
 
         base_conversion_url = cls._path.format(custom_model_id, custom_model_version_id)
         data = unpaginate(base_conversion_url, None, cls._client)
         return [cls.from_server_data(item) for item in data]
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         - `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.ANOMALY`
         - `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.TRANSFORM`
     latest_version: datarobot.CustomTaskVersion or None
         latest version of the custom task if the task has a latest version. If the
         latest version is None, the custom task is not ready for use in user blueprints.
         You must create its first CustomTaskVersion before you can use the CustomTask
     created_by: str
-        The username of the user who created the custom task.
+        username of a user who user who created the custom task
     updated_at: str
-        An ISO-8601 formatted timestamp of when the custom task was updated.
+        ISO-8601 formatted timestamp of when the custom task was updated
     created_at: str
         ISO-8601 formatted timestamp of when the custom task was created
     calibrate_predictions: bool
         whether anomaly predictions should be calibrated to be between 0 and 1 by DR.
         only applies to custom estimators with target type
         `datarobot.enums.CUSTOM_TASK_TARGET_TYPE.ANOMALY`
     """
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -26,22 +26,22 @@
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject
 from datarobot.models.credential import CredentialDataSchema
 from datarobot.models.feature import DatasetFeature
 from datarobot.models.featurelist import DatasetFeaturelist
 from datarobot.models.project import Project
 from datarobot.models.sharing import SharingAccess
-from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_cases, UseCaseLike
 from datarobot.utils import assert_single_parameter, dataframe_to_buffer
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.source import parse_source_type
 from datarobot.utils.sourcedata import list_of_records_to_buffer
 from datarobot.utils.waiters import wait_for_async_resolution
 
 from ..enums import DEFAULT_MAX_WAIT, DEFAULT_TIMEOUT
+from .use_cases.utils import resolve_use_case
 
 ProjectLocation = namedtuple("ProjectLocation", ["url", "id"])
 
 FeatureTypeCount = namedtuple("FeatureTypeCount", ["count", "feature_type"])
 
 
 TDataset = TypeVar("TDataset", bound="Dataset")
@@ -200,15 +200,14 @@
             return cls.create_from_file(file_path=cast(str, source))
         elif source_type == LocalSourceType.DATA_FRAME:
             return cls.create_from_in_memory_data(data_frame=source)
         elif source_type == LocalSourceType.FILELIKE:
             return cls.create_from_file(filelike=cast(IOBase, source))
 
     @classmethod
-    @add_to_use_case(allow_multiple=True)
     def create_from_file(
         cls: Type[TDataset],
         file_path: Optional[str] = None,
         filelike: Optional[IOBase] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -232,17 +231,14 @@
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             A fully armed and operational Dataset
         """
         assert_single_parameter(("filelike", "file_path"), file_path, filelike)
@@ -273,15 +269,14 @@
         )
         dataset = cls.from_location(new_dataset_location)
         if categories:
             dataset.modify(categories=categories)
         return dataset
 
     @classmethod
-    @add_to_use_case(allow_multiple=True)
     def create_from_in_memory_data(
         cls: Type[TDataset],
         data_frame: Optional[pd.DataFrame] = None,
         records: Optional[List[Dict[str, Any]]] = None,
         categories: Optional[List[str]] = None,
         read_timeout: int = DEFAULT_TIMEOUT.UPLOAD,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -307,17 +302,14 @@
         read_timeout: int, optional
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful
         fname: string, optional
             The file name, "data.csv" by default
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data.
 
         Raises
@@ -338,15 +330,14 @@
             filelike=buff,
             categories=categories,
             read_timeout=read_timeout,
             max_wait=max_wait,
         )
 
     @classmethod
-    @add_to_use_case(allow_multiple=True)
     def create_from_url(
         cls: Type[TDataset],
         url: str,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
         categories: Optional[List[str]] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
@@ -373,17 +364,14 @@
             available. Specifying this parameter to false and `doSnapshot` to true will result in
             an error.
         categories: list[string], optional
             An array of strings describing the intended use of the dataset. The
             current supported options are "TRAINING" and "PREDICTION".
         max_wait: int, optional
             Time in seconds after which dataset creation is considered unsuccessful.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -398,15 +386,14 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
-    @add_to_use_case(allow_multiple=True)
     def create_from_data_source(
         cls: Type[TDataset],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         do_snapshot: Optional[bool] = None,
         persist_data_after_ingestion: Optional[bool] = None,
@@ -455,17 +442,15 @@
             If unset, uses the server default: False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int, optional
             Time in seconds after which project creation is considered unsuccessful.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
+
 
         Returns
         -------
         response: Dataset
             The Dataset created from the uploaded data
         """
         base_data = {
@@ -489,15 +474,14 @@
 
         new_dataset_location = wait_for_async_resolution(
             cls._client, response.headers["Location"], max_wait
         )
         return cls.from_location(new_dataset_location)
 
     @classmethod
-    @add_to_use_case(allow_multiple=True)
     def create_from_query_generator(
         cls: Type[TDataset],
         generator_id: str,
         dataset_id: Optional[str] = None,
         dataset_version_id: Optional[str] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TDataset:
@@ -516,17 +500,14 @@
         dataset_id: str, optional
             The id of the dataset to apply the query to.
         dataset_version_id: str, optional
             The id of the dataset version to apply the query to. If not specified the
             latest version associated with dataset_id (if specified) is used.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case IDs or a single Use Case ID to add this new dataset to. Must be a kwarg.
 
         Returns
         -------
         response: Dataset
             The Dataset created from the query generator
         """
         url = "dataEngineWorkspaceStates/fromDataEngineQueryGenerator/"
@@ -601,15 +582,15 @@
 
     @classmethod
     def list(
         cls: Type[TDataset],
         category: Optional[str] = None,
         filter_failed: Optional[bool] = None,
         order_by: Optional[str] = None,
-        use_cases: Optional[UseCaseLike] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> List[TDataset]:
         """
         List all datasets a user can view.
 
 
         Parameters
         ----------
@@ -624,42 +605,40 @@
             If True invalid datasets will be excluded.
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
-
-        use_cases: Union[UseCase, List[UseCase], str, List[str]], optional
-            Filter available datasets by a specific Use Case or Cases. Accepts either the entity or the ID.
-
+        use_case_ids: string or List[string], optional
+            Filter available datasets by a specific Use Case ID or IDs.
         Returns
         -------
         list[Dataset]
             a list of datasets the user can view
 
         """
         return list(
             cls.iterate(
                 category=category,
                 order_by=order_by,
                 filter_failed=filter_failed,
-                use_cases=use_cases,
+                use_case_ids=use_case_ids,
             )
         )
 
     @classmethod
     def iterate(
         cls: Type[TDataset],
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         category: Optional[str] = None,
         order_by: Optional[str] = None,
         filter_failed: Optional[bool] = None,
-        use_cases: Optional[UseCaseLike] = None,
+        use_case_ids: Optional[Union[str, List[str]]] = None,
     ) -> Generator[TDataset, None, None]:
         """
         Get an iterator for the requested datasets a user can view.
         This lazily retrieves results. It does not get the next page from the server until the
         current page is exhausted.
 
         Parameters
@@ -683,31 +662,33 @@
 
         order_by: string, optional
             If unset, uses the server default: "-created".
             Sorting order which will be applied to catalog list, valid options are:
             - "created" -- ascending order by creation datetime;
             - "-created" -- descending order by creation datetime.
 
-        use_cases: Union[UseCase, List[UseCase], str, List[str]], optional
-            Filter available datasets by a specific Use Case or Cases. Accepts either the entity or the ID.
-
+        use_case_ids: string or List[string], optional
+            Filter available datasets by a specific Use Case ID or IDs.
         Yields
         ------
         Dataset
             An iterator of the datasets the user can view
 
         """
         all_params = {
             "offset": offset,
             "limit": limit,
             "category": category,
             "order_by": order_by,
             "filter_failed": filter_failed,
+            "experiment_container_ids": use_case_ids,
         }
-        all_params = resolve_use_cases(use_cases=use_cases, params=all_params)
+        all_params = resolve_use_case(
+            use_case_id=use_case_ids, use_case_key="experiment_container_ids", params=all_params
+        )
         params = _remove_empty_params(all_params)
         _update_filter_failed(params)
 
         for dataset_json in unpaginate(cls._path, params, cls._client):
             yield cls.from_server_data(dataset_json)
 
     def update(self) -> None:
@@ -993,15 +974,14 @@
         Returns
         -------
         locations: list[ProjectLocation]
         """
         url = f"{self._path}{self.id}/projects/"
         return [ProjectLocation(**kwargs) for kwargs in unpaginate(url, None, self._client)]
 
-    @add_to_use_case(allow_multiple=True)
     def create_project(
         self,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -1025,17 +1005,14 @@
             The ID of the set of credentials to use instead of user and password.
         use_kerberos: bool, optional
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
-        use_cases: list[UseCase] | UseCase | list[string] | string, optional
-            A list of UseCase objects, UseCase object,
-            list of Use Case ids or a single Use Case id to add this new Dataset to. Must be a kwarg.
 
         Returns
         -------
         Project
         """
         return Project.create_from_dataset(
             self.id,
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import dateutil
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import ACCURACY_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -41,15 +41,15 @@
 
     class Bucket(TypedDict):
         period: Period
         value: int
         sample_size: int
 
 
-class Accuracy(APIObject, MonitoringDataQueryBuilderMixin):
+class Accuracy(APIObject, DeploymentQueryBuilderMixin):
     """Deployment accuracy information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metrics
     period : dict
@@ -184,15 +184,15 @@
         -------
         percent_changes: Dict
         """
 
         return {name: value.get("percent_change") for name, value in self.metrics.items()}
 
 
-class AccuracyOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class AccuracyOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment accuracy over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/bias_and_fairness.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import dateutil
 import trafaret as t
 from trafaret import Bool, Float
 
 from datarobot._compat import String
 from datarobot.enums import BUCKET_SIZE
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -33,15 +33,15 @@
 
     class Bucket(TypedDict):
         period: Period
         value: int
         sample_size: int
 
 
-class FairnessScoresOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class FairnessScoresOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment fairness over time information.
 
     Attributes
     ----------
     buckets : List
         fairness over time bucket for each model and bucket queried
     protected_feature : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/data_drift.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from typing import List, Optional, TYPE_CHECKING
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import BUCKET_SIZE, DATA_DRIFT_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         start: datetime
@@ -49,15 +49,15 @@
         row_count: Optional[int]
         mean_predicted_value: Optional[int]
         percentiles: List[Percentile]
         mean_probabilities: List[MeanProbability]
         class_distribution: List[ClassDistribution]
 
 
-class TargetDrift(APIObject, MonitoringDataQueryBuilderMixin):
+class TargetDrift(APIObject, DeploymentQueryBuilderMixin):
     """Deployment target drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve target drift metric
     period : dict
@@ -173,15 +173,15 @@
         if metric:
             params["metric"] = metric
         data = cls._client.get(path, params=params).json()
         data = from_api(data, keep_null_keys=True)
         return cls.from_data(data)
 
 
-class FeatureDrift(APIObject, MonitoringDataQueryBuilderMixin):
+class FeatureDrift(APIObject, DeploymentQueryBuilderMixin):
     """Deployment feature drift information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve feature drift metric
     period : dict
@@ -320,15 +320,15 @@
             response_json = from_api(response_json, keep_null_keys=True)
             for item in response_json["data"]:
                 data.append(_from_data_item(item))
 
         return data
 
 
-class PredictionsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class PredictionsOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment predictions over time information.
 
     Attributes
     ----------
     baselines : List
         target baseline for each model queried
     buckets : List
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     ACCURACY_METRIC,
     BUCKET_SIZE,
     DEFAULT_MAX_WAIT,
     FileLocationType,
     LocalSourceType,
 )
 from datarobot.errors import InvalidUsageError
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.mixins.browser_mixin import BrowserMixin
 from datarobot.models.api_object import APIObject, ServerDataDictType
 from datarobot.models.batch_prediction_job import BatchPredictionJob
 from datarobot.models.custom_model_version import CustomModelVersion
 from datarobot.models.deployment.accuracy import Accuracy, AccuracyOverTime
 from datarobot.models.deployment.bias_and_fairness import FairnessScoresOverTime
 from datarobot.models.deployment.data_drift import FeatureDrift, PredictionsOverTime, TargetDrift
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.models.deployment.service_stats import ServiceStats, ServiceStatsOverTime
 from datarobot.models.deployment.sharing import (
     DeploymentGrantSharedRoleWithId,
     DeploymentGrantSharedRoleWithUsername,
     DeploymentSharedRole,
 )
 from datarobot.utils import deprecated, from_api, get_id_from_location
@@ -138,15 +138,15 @@
     # Allow users to pass a single value even if a list of values is expected.
     if isinstance(trafaret, t.List) and not isinstance(value, list):
         value = [value]
 
     return trafaret.check(value)
 
 
-class Deployment(APIObject, MonitoringDataQueryBuilderMixin, BrowserMixin):
+class Deployment(APIObject, DeploymentQueryBuilderMixin, BrowserMixin):
     """A deployment created from a DataRobot model.
 
     Attributes
     ----------
     id : str
         the id of the deployment
     label : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/helpers/deployment_monitoring.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pytz
 
 if TYPE_CHECKING:
     from datetime import datetime
 
 
-class MonitoringDataQueryBuilderMixin:  # pylint: disable=missing-class-docstring
+class DeploymentQueryBuilderMixin:  # pylint: disable=missing-class-docstring
     @staticmethod
     def _build_query_params(  # pylint: disable=missing-function-docstring
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         def timezone_aware(dt: datetime) -> datetime:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/service_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from typing import cast, List, Optional, TYPE_CHECKING, Union
 
 import dateutil
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import SERVICE_STAT_METRIC
+from datarobot.helpers.deployment_monitoring import DeploymentQueryBuilderMixin
 from datarobot.models.api_object import APIObject
-from datarobot.models.deployment.mixins import MonitoringDataQueryBuilderMixin
 from datarobot.utils import from_api
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class Period(TypedDict, total=False):
         """Type dict for period"""
@@ -51,15 +51,15 @@
         serverErrorRate: float
         numConsumers: int
         cacheHitRatio: float
         medianLoad: float
         peakLoad: float
 
 
-class ServiceStats(APIObject, MonitoringDataQueryBuilderMixin):
+class ServiceStats(APIObject, DeploymentQueryBuilderMixin):
     """Deployment service stats information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve service stats metrics
     period : dict
@@ -175,15 +175,15 @@
         metrics = data.pop("metrics")
 
         data = from_api(data, keep_null_keys=True)
         data["metrics"] = metrics
         return cls.from_data(data)
 
 
-class ServiceStatsOverTime(APIObject, MonitoringDataQueryBuilderMixin):
+class ServiceStatsOverTime(APIObject, DeploymentQueryBuilderMixin):
     """Deployment service stats over time information.
 
     Attributes
     ----------
     model_id : str
         the model used to retrieve accuracy metric
     metric : str
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/lift_chart.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             t.Key("num_columns"): Int(),
             t.Key("forecast_point", optional=True): parse_time,
             t.Key("predictions_start_date", optional=True): parse_time,
             t.Key("predictions_end_date", optional=True): parse_time,
             t.Key("relax_known_in_advance_features_check", optional=True): t.Bool(),
             # do not forget to update `test_data_quality_warnings`
             # in datarobot-python-api-tests repo
-            t.Key("data_quality_warnings", optional=True): t.Dict(
+            t.Key("data_quality_warnings"): t.Dict(
                 {
                     t.Key("has_kia_missing_values_in_forecast_window"): t.Bool(),
                     t.Key("insufficient_rows_for_evaluating_models"): t.Bool(),
                     t.Key("single_class_actual_value_column"): t.Bool(),
                 }
             ).allow_extra("*"),
             t.Key("forecast_point_range", optional=True): t.List(parse_time),
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -20,15 +20,14 @@
 
 from pandas import DataFrame
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import (
     AUTOPILOT_MODE,
-    CredentialTypes,
     CV_METHOD,
     DEFAULT_MAX_WAIT,
     DEFAULT_TIMEOUT,
     LEADERBOARD_SORT_KEY,
     MONOTONICITY_FEATURELIST_DEFAULT,
     NonPersistableProjectOptions,
     PROJECT_STAGE,
@@ -85,15 +84,15 @@
 from datarobot.models.relationships_configuration import RelationshipsConfiguration
 from datarobot.models.restore_discarded_features import (
     DiscardedFeaturesInfo,
     FeatureRestorationStatus,
 )
 from datarobot.models.segmentation import SegmentationTask
 from datarobot.models.sharing import SharingAccess
-from datarobot.models.use_cases.utils import add_to_use_case, resolve_use_cases, UseCaseLike
+from datarobot.models.use_cases.utils import resolve_use_case
 from datarobot.utils import (
     assert_single_or_zero_parameter,
     camelize,
     datetime_to_string,
     deprecated,
     from_api,
     get_duplicate_features,
@@ -120,39 +119,14 @@
     from datarobot.models.dataset import Dataset
 
     class SegmentationDict(TypedDict):
         segmentation_task_id: Optional[str]
         parent_project_id: Optional[str]
         segment: Optional[str]
 
-    class BaseCredentialsDataDict(TypedDict):
-        credentialType: CredentialTypes
-
-    class BasicCredentialsDataDict(BaseCredentialsDataDict):
-        user: str
-        password: str
-
-    class S3CredentialsDataDict(BaseCredentialsDataDict):
-        awsAccessKeyId: str
-        awsSecretAccessKey: str
-        awsSessionToken: str
-
-    class OAuthCredentialsDataDict(BaseCredentialsDataDict):
-        oauthRefreshToken: str
-        oauthClientId: str
-        oauthClientSecret: str
-        oauthAccessToken: str
-
-    class BasicCredentialsDict(TypedDict):
-        user: str
-        password: str
-
-    class CredentialIdCredentialsDict(TypedDict):
-        credentialId: str
-
 
 class Project(APIObject, BrowserMixin):
     """A project built from a particular training dataset
 
     Attributes
     ----------
     id : str
@@ -213,16 +187,14 @@
         (New in version v3.0) The partitioning class for this project. This attribute should only be used
         with newly-created projects and before calling `Project.analyze_and_model()`. After the project has been
         aimed, see `Project.partition` for actual partitioning options.
     catalog_id : str
         (New in version v3.0) ID of the dataset used during creation of the project.
     catalog_version_id : str
         (New in version v3.0) The object ID of the ``catalog_version`` which the project's dataset belongs to.
-    use_gpu: bool
-        (New in version v3.2) Whether project allows usage of GPUs
     """
 
     _path = "projects/"
     _clone_path = "projectClones/"
     _scaleout_modeling_mode_converter = String()
     _advanced_options_converter = t.Dict(
         {
@@ -317,15 +289,14 @@
             t.Key("created", optional=True): parse_time,
             t.Key("advanced_options", optional=True): _advanced_options_converter,
             t.Key("max_train_pct", optional=True): t.Float(),
             t.Key("max_train_rows", optional=True): Int(),
             t.Key("file_name", optional=True): String(allow_blank=True),
             t.Key("credentials", optional=True): _feg_credentials_converter,
             t.Key("feature_engineering_prediction_point", optional=True): String(),
-            t.Key("use_gpu", optional=True): t.Bool(),
             t.Key("unsupervised_mode", default=False): t.Bool(),
             t.Key("use_feature_discovery", optional=True, default=False): t.Bool(),
             t.Key("relationships_configuration_id", optional=True): String(),
             t.Key("query_generator_id", optional=True): String(),
             t.Key("segmentation", optional=True): _segmentation_converter,
             t.Key("partitioning_method", optional=True): t.Or(
                 _partitioning_method_converter, DatetimePartitioning._converter
@@ -359,15 +330,14 @@
         relationships_configuration_id: Optional[str] = None,
         project_description: Optional[str] = None,
         query_generator_id: Optional[str] = None,
         segmentation: Optional[SegmentationDict] = None,
         partitioning_method=None,
         catalog_id: Optional[str] = None,
         catalog_version_id: Optional[str] = None,
-        use_gpu: Optional[bool] = None,
     ) -> None:
 
         self.id = id
         self.project_name = project_name
         self.project_description = project_description
         self.mode = mode
         self.target = target
@@ -391,15 +361,14 @@
         self.use_feature_discovery = use_feature_discovery
         self.relationships_configuration_id = relationships_configuration_id
         self.query_generator_id = query_generator_id
         self.segmentation = segmentation
         self.partitioning_method = partitioning_method
         self.catalog_id = catalog_id
         self.catalog_version_id = catalog_version_id
-        self.use_gpu = use_gpu
         self.__options = None
 
     @property
     def use_time_series(self) -> bool:
         return bool(self.partition and self.partition.get("use_time_series"))
 
     @property
@@ -607,23 +576,22 @@
             keep_attrs=[
                 "advanced_options.default_monotonic_increasing_featurelist_id",
                 "advanced_options.default_monotonic_decreasing_featurelist_id",
             ],
         )
 
     @classmethod
-    @add_to_use_case(allow_multiple=False)
     def create(
         cls,
         sourcedata,
         project_name="Untitled Project",
         max_wait=DEFAULT_MAX_WAIT,
         read_timeout=DEFAULT_TIMEOUT.UPLOAD,
         dataset_filename=None,
-    ) -> TProject:
+    ):
         """
         Creates a project with provided data.
 
         Project creation is asynchronous process, which means that after
         initial request we will keep polling status of async process
         that is responsible for project creation until it's finished.
         For SDK users this only means that this method might raise
@@ -643,16 +611,14 @@
             unsuccessful
         read_timeout: int
             The maximum number of seconds to wait for the server to respond indicating that the
             initial upload is complete
         dataset_filename : string or None, optional
             (New in version v2.14) File name to use for dataset.
             Ignored for url and file path sources.
-        use_case: UseCase | string, optional
-            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             Instance with initialized data.
 
         Raises
@@ -759,15 +725,14 @@
         if project_name is not None:
             payload["project_name"] = project_name
 
         response = cls._client.post(hdfs_project_create_endpoint, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case(allow_multiple=False)
     def create_from_data_source(
         cls: Type[TProject],
         data_source_id: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         credential_id: Optional[str] = None,
         use_kerberos: Optional[bool] = None,
@@ -798,16 +763,14 @@
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         project_name : str, optional
             optional, a name to give to the project.
         max_wait : int
             optional, the maximum number of seconds to wait before giving up.
-        use_case: UseCase | string, optional
-            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Raises
         ------
         InvalidUsageError
             Raised if either ``username`` or ``password`` is passed without the other.
 
         Returns
@@ -833,15 +796,14 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case(allow_multiple=False)
     def create_from_dataset(
         cls: Type[TProject],
         dataset_id: str,
         dataset_version_id: Optional[str] = None,
         project_name: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
@@ -875,16 +837,14 @@
             Server default is False.
             If true, use kerberos authentication for database authentication.
         credential_data: dict, optional
             The credentials to authenticate with the database, to use instead of user/password or
             credential ID.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
-        use_case: UseCase | string, optional
-            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         Project
         """
         payload = {
             "dataset_id": dataset_id,
@@ -901,15 +861,14 @@
         if "credential_data" in new_payload:
             new_payload["credential_data"] = CredentialDataSchema(new_payload["credential_data"])
 
         response = cls._client.post(cls._path, data=new_payload)
         return cls.from_async(response.headers["Location"], max_wait=max_wait)
 
     @classmethod
-    @add_to_use_case(allow_multiple=False)
     def create_segmented_project_from_clustering_model(
         cls: Type[TProject],
         clustering_project_id: str,
         clustering_model_id: str,
         target: str,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> TProject:
@@ -924,16 +883,14 @@
             The identifier of the clustering model you want to use as the
             segmentation method.
         target : str
             The name of the target column that will be used from the
             clustering project.
         max_wait: int
             optional, the maximum number of seconds to wait before giving up.
-        use_case: UseCase | string, optional
-            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             The created project
         """
         prepare_model_package_path = (
@@ -1049,15 +1006,14 @@
             )
             proj_id = get_id_from_location(finished_location)
             return cls.get(proj_id)
         except AppPlatformError as e:
             raise ProjectAsyncFailureError(repr(e), e.status_code, async_location)
 
     @classmethod
-    @add_to_use_case(allow_multiple=False)
     def start(
         cls: Type[TProject],
         sourcedata: Union[str, DataFrame],
         target: Optional[str] = None,
         project_name: str = "Untitled Project",
         worker_count: Optional[int] = None,
         metric: Optional[str] = None,
@@ -1178,16 +1134,14 @@
             - 'postProcessingRejectionOptionBasedClassification'
             The technique by which we'll mitigate bias, which will inform which bias mitigation task
             we insert into blueprints
         include_bias_mitigation_feature_as_predictor_variable : bool, optional
             Whether we should also use the mitigation feature as in input to the modeler just like
             any other categorical used for training, i.e. do we want the model to "train on" this
             feature in addition to using it for bias mitigation
-        use_case: UseCase | string, optional
-            A single UseCase object or ID to add this new Project to. Must be a kwarg.
 
         Returns
         -------
         project : Project
             The newly created and initialized project.
 
         Raises
@@ -1268,31 +1222,27 @@
             unsupervised_type=unsupervised_type,
             autopilot_cluster_list=autopilot_cluster_list,
         )
         return project
 
     @classmethod
     def list(
-        cls, search_params: Optional[Dict[str, str]] = None, use_cases: Optional[UseCaseLike] = None
+        cls, search_params: Optional[Dict[str, str]] = None, use_case_id: Optional[str] = None
     ) -> List[Project]:
         """
         Returns the projects associated with this account.
 
         Parameters
         ----------
         search_params : dict, optional.
             If not `None`, the returned projects are filtered by lookup.
             Currently you can query projects by:
 
             * ``project_name``
 
-        use_cases : Union[UseCase, List[UseCase], str, List[str]], optional.
-            If not `None`, the returned projects are filtered to those associated
-            with a specific Use Case or Use Cases. Accepts either the entity or the ID.
-
         Returns
         -------
         projects : list of Project instances
             Contains a list of projects associated with this user
             account.
 
         Raises
@@ -1324,18 +1274,17 @@
             else:
                 raise TypeError(
                     "Provided search_params argument {} is invalid type {}".format(
                         search_params, type(search_params)
                     )
                 )
         # This is a special case we needed to cover. A user could pass in "experiment_container_id" themselves to
-        # `search_params`, so we need to check for that and default to `use_cases` if that was passed in.
-        # Then we proceed to check if resolve_use_case(`use_case_id`) arg was set, and use a global use case if
-        # it's available.
-        get_params = resolve_use_cases(use_cases=use_cases, params=get_params)
+        # `search_params`, so we need to check for that and default to `use_case_id` if that was passed in.
+        # Then we proceed to check if `use_case_id` was set, and use a global use case if it's available.
+        get_params = resolve_use_case(use_case_id=use_case_id, params=get_params)
         r_data = cls._client.get(cls._path, params=get_params).json()
         return [cls.from_server_data(item) for item in r_data]
 
     def _update(self, **data) -> Project:
         """
         Change the project properties.
 
@@ -1449,15 +1398,14 @@
         feature_engineering_prediction_point=None,
         unsupervised_mode=False,
         relationships_configuration_id=None,
         class_mapping_aggregation_settings=None,
         segmentation_task_id=None,
         unsupervised_type=None,
         autopilot_cluster_list=None,
-        use_gpu=None,
     ):
         """
         Set target variable of an existing project and begin the autopilot process or send data to DataRobot
         for feature analysis only if manual mode is specified.
 
         Any options saved using ``set_options`` will be used if nothing is passed to ``advanced_options``.
         However, saved options will be ignored if ``advanced_options`` are passed.
@@ -1535,16 +1483,14 @@
         unsupervised_type : UnsupervisedTypeEnum, optional
             (New in version v2.27) Specifies whether an unsupervised project is anomaly detection
             or clustering.
         autopilot_cluster_list : list(int), optional
             (New in version v2.27) Specifies the list of clusters to build for each model during
             Autopilot. Specifying multiple values in a list will build models with each number
             of clusters for the Leaderboard.
-        use_gpu : bool, optional
-            (New in version v3.2) Specifies whether project should use GPUs
 
         Returns
         -------
         project : Project
             The instance with updated attributes.
 
         Raises
@@ -1630,16 +1576,14 @@
                 aim_payload["segmentation_task_id"] = segmentation_task_id.id
             elif isinstance(segmentation_task_id, str):
                 aim_payload["segmentation_task_id"] = segmentation_task_id
             else:
                 raise ValueError(
                     "segmentation_task_id must be either a string id or a SegmentationTask object"
                 )
-        if use_gpu is not None:
-            aim_payload["use_gpu"] = use_gpu
 
         url = f"{self._path}{self.id}/aim/"
         response = self._client.patch(url, data=aim_payload)
         async_location = response.headers["Location"]
 
         # Waits for project to be ready for modeling, but ignores the return value
         self.from_async(async_location, max_wait=max_wait)
@@ -2125,15 +2069,15 @@
         predictions_start_date=None,
         predictions_end_date=None,
         dataset_filename=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ) -> PredictionDataset:
+    ):
         """Upload a new dataset to make predictions against
 
         Parameters
         ----------
         sourcedata : str, file or pandas.DataFrame
             Data to be used for predictions. If string, can be either a path to a local file,
             a publicly accessible URL (starting with ``http://``, ``https://``, ``file://``), or
@@ -2266,15 +2210,15 @@
         forecast_point=None,
         relax_known_in_advance_features_check=None,
         credentials=None,
         predictions_start_date=None,
         predictions_end_date=None,
         actual_value_column=None,
         secondary_datasets_config_id=None,
-    ) -> PredictionDataset:
+    ):
         """
         Upload a new dataset from a data source to make predictions against
 
         Parameters
         ----------
         data_source_id : str
             The identifier of the data source.
@@ -2347,104 +2291,46 @@
         async_loc = initial_project_post_response.headers["Location"]
         dataset_loc = wait_for_async_resolution(self._client, async_loc, max_wait=max_wait)
         dataset_data = self._client.get(dataset_loc, join_endpoint=False).json()
         return PredictionDataset.from_server_data(dataset_data)
 
     def upload_dataset_from_catalog(
         self,
-        dataset_id: str,
-        credential_id: Optional[str] = None,
-        credential_data: Optional[
-            Union[BasicCredentialsDataDict, S3CredentialsDataDict, OAuthCredentialsDataDict]
-        ] = None,
-        dataset_version_id: Optional[str] = None,
-        max_wait: Optional[int] = DEFAULT_MAX_WAIT,
-        forecast_point: Optional[datetime] = None,
-        relax_known_in_advance_features_check: Optional[bool] = None,
-        credentials: Optional[
-            List[Union[BasicCredentialsDict, CredentialIdCredentialsDict]]
-        ] = None,
-        predictions_start_date: Optional[datetime] = None,
-        predictions_end_date: Optional[datetime] = None,
-        actual_value_column: Optional[str] = None,
-        secondary_datasets_config_id: Optional[str] = None,
-    ) -> PredictionDataset:
+        dataset_id,
+        dataset_version_id=None,
+        max_wait=DEFAULT_MAX_WAIT,
+        forecast_point=None,
+        relax_known_in_advance_features_check=None,
+        credentials=None,
+        predictions_start_date=None,
+        predictions_end_date=None,
+        actual_value_column=None,
+        secondary_datasets_config_id=None,
+    ):
         """Upload a new dataset from a catalog dataset to make predictions against
 
         Parameters
         ----------
         dataset_id : str
             The identifier of the dataset.
-        credential_id : str, optional
-            The credential ID of the AI Catalog dataset to upload.
-        credential_data : BasicCredentialsDataDict | S3CredentialsDataDict | OAuthCredentialsDataDict, optional
-            Credential data of the catalog dataset to upload. `credential_data` can be in
-            one of the following forms:
-
-            Basic Credentials
-                credentialType : str
-                    The credential type. For basic credentials, this value must be CredentialTypes.BASIC.
-                user : str
-                    The username for database authentication.
-                password : str
-                    The password for database authentication.
-                    The password is encrypted at rest and never saved or stored.
-
-            S3 Credentials
-                credentialType : str
-                    The credential type. For S3 credentials, this value must be CredentialTypes.S3.
-                awsAccessKeyId : str
-                    The S3 AWS access key ID.
-                awsSecretAccessKey : str
-                    The S3 AWS secret access key.
-                awsSessionToken : str
-                    The S3 AWS session token.
-
-            OAuth Credentials
-                credentialType : str
-                    The credential type. For OAuth credentials, this value must be CredentialTypes.OAUTH.
-                oauthRefreshToken : str
-                    The oauth refresh token.
-                oauthClientId : str
-                    The oauth client ID.
-                oauthClientSecret : str
-                    The oauth client secret.
-                oauthAccessToken : str
-                    The oauth access token.
         dataset_version_id : str, optional
             The version id of the dataset to use.
         max_wait : int, optional
             Optional, the maximum number of seconds to wait before giving up.
         forecast_point : datetime.datetime or None, optional
             For time series projects only. This is the default point relative
             to which predictions will be generated, based on the forecast window of the project. See
             the time series :ref:`prediction documentation <time_series_predict>` for more
             information.
         relax_known_in_advance_features_check : bool, optional
             For time series projects only. If True, missing values in the
             known in advance features are allowed in the forecast window at the prediction time.
             If omitted or False, missing values are not allowed.
-        credentials: list[BasicCredentialsDict | CredentialIdCredentialsDict], optional
+        credentials: list, optional
             A list of credentials for the datasets used in Feature discovery project.
-
-            Items in `credentials` can have the following forms:
-
-            Basic Credentials
-                user : str
-                    The username for database authentication.
-                password : str
-                    The password (in cleartext) for database authentication. The password
-                    will be encrypted on the server side in scope of HTTP request
-                    and never saved or stored.
-
-            Credential ID
-                credentialId : str
-                    The ID of the set of credentials to use instead of user and password.
-                    Note that with this change, username and password will become optional.
-
         predictions_start_date : datetime.datetime or None, optional
             For time series projects only. The start date for bulk
             predictions. Note that this parameter is for generating historical predictions using the
             training data. This parameter should be provided in conjunction with
             ``predictions_end_date``. Can't be provided with the ``forecast_point`` parameter.
         predictions_end_date : datetime.datetime or None, optional
             For time series projects only. The end date for bulk predictions,
@@ -2454,24 +2340,21 @@
         actual_value_column : string, optional
             Actual value column name, valid for the prediction
             files if the project is unsupervised and the dataset is considered as bulk predictions
             dataset. Cannot be provided with the ``forecast_point`` parameter.
         secondary_datasets_config_id: string or None, optional
             The Id of the alternative secondary dataset config
             to use during prediction for Feature discovery project.
+
         Returns
         -------
         dataset : PredictionDataset
             the newly uploaded dataset
         """
         form_data = {"datasetId": dataset_id}
-        if credential_id:
-            form_data["credentialId"] = credential_id
-        if credential_data:
-            form_data["credentialData"] = credential_data
         if dataset_version_id:
             form_data["datasetVersionId"] = dataset_version_id
         if forecast_point:
             if not isinstance(forecast_point, datetime):
                 raise ValueError("forecast_point must be an instance of datetime.datetime")
             form_data["forecastPoint"] = datetime_to_string(forecast_point)
         if predictions_start_date:
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/project_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,14 +441,16 @@
         One of BiasMitigationTechnique.
         The technique by which we'll mitigate bias, which will inform which bias mitigation task
         we insert into blueprints and how
     include_bias_mitigation_feature_as_predictor_variable : bool or None, optional
         Whether we should also use the mitigation feature as in input to the modeler just like
         any other categorical used for training, i.e. do we want the model to "train on" this
         feature in addition to using it for bias mitigation
+    force_cpu: bool, optional
+        If GPUs enabled, override and force running everything on CPUs
     min_clusters: int, optional
         The minimum number of clusters allowed when training clustering models.
     max_clusters: int, optional
         The maximum number of clusters allowed when training clustering models
     segmentation_id_column: string, optional
         The segmentation column name or automated segmentation column name specified for the
         project through the UI
@@ -475,16 +477,14 @@
     class_mapping_aggregation_settings: ClassMappingAggregationSettings, optional
         For multiclass additional settings can be specified to control aggregation of target
         values in final classes.
     class_mapping_aggregation_settings_enabled: bool, optional
         Is the class mapping aggregation settings section enabled or not in UI
     datetime_partitioning_id: str, optional
         Id of the datetime partitioning to use
-    use_gpu: bool, optional
-        Whether to allow GPU usage for the project
     """
 
     _backtest_specification_converter = t.Dict(
         {
             t.Key("gap_duration", optional=True): String(),
             t.Key("index", optional=True): Int(),
             t.Key("primary_training_end_date", optional=True): parse_time,
@@ -555,14 +555,15 @@
                 t.Null(), t.Dict({}), FeatureEngineeringOptions._converter
             ),
             t.Key("feature_engineering_prediction_point", optional=True): t.Null()
             | Feature._converter,
             t.Key("featurelist_id", optional=True): t.Null() | String(),
             t.Key("feature_settings", optional=True): t.Null()
             | t.List(_feature_settings_converter),
+            t.Key("force_cpu", optional=True): t.Null() | t.Bool(),
             t.Key("forecast_window_end", optional=True): t.Null() | Int(),
             t.Key("forecast_window_start", optional=True): t.Null() | Int(),
             t.Key("gap_duration", optional=True): t.Null() | String(),
             t.Key("holdout_duration", optional=True): t.Or(t.Null(), String(), Duration._converter),
             t.Key("holdout_end_date", optional=True): t.Null() | parse_time,
             t.Key("holdout_level", optional=True): t.Null() | t.Or(String(), Int()),
             t.Key("holdout_pct", optional=True): t.Null() | Int(),
@@ -602,15 +603,14 @@
             t.Key("segmentation_task_id", optional=True): t.Null() | String(),
             t.Key("segments_count", optional=True): t.Null() | Int(),
             t.Key("target", optional=True): t.Null() | String(),
             t.Key("target_type", optional=True): t.Null() | t.Enum(*TARGET_TYPE.ALL),
             t.Key("training_level", optional=True): t.Null() | t.Or(String(), Int()),
             t.Key("treat_as_exponential", optional=True): t.Null()
             | t.Enum(*TREAT_AS_EXPONENTIAL.ALL),
-            t.Key("use_gpu", optional=True): t.Null() | t.Bool(),
             t.Key("unsupervised_mode", optional=True): t.Null() | t.Bool(),
             t.Key("use_cross_series_features", optional=True): t.Null() | t.Bool(),
             t.Key("use_project_settings", optional=True): t.Null() | t.Bool(),
             t.Key("user_partition_col", optional=True): t.Null() | Feature._converter,
             t.Key("use_time_series", optional=True): t.Null() | t.Bool(),
             t.Key("validation_duration", optional=True): t.Null() | String(),
             t.Key("validation_level", optional=True): t.Null() | t.Or(String(), Int()),
@@ -649,14 +649,15 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
+        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -692,15 +693,14 @@
         segmentation_model_package_name: Optional[str] = None,
         segmentation_task_id: Optional[str] = None,
         segments_count: Optional[int] = None,
         target: Optional[str] = None,
         target_type: Optional[TARGET_TYPE] = None,
         training_level: Optional[Union[str, int]] = None,
         treat_as_exponential: Optional[TREAT_AS_EXPONENTIAL] = None,
-        use_gpu: Optional[bool] = None,
         unsupervised_mode: Optional[bool] = None,
         use_cross_series_features: Optional[bool] = None,
         use_project_settings: Optional[bool] = None,
         user_partition_col: Optional[Feature] = None,
         use_time_series: Optional[bool] = None,
         validation_duration: Optional[str] = None,
         validation_level: Optional[Union[str, int]] = None,
@@ -736,14 +736,15 @@
             feature_derivation_window_end=feature_derivation_window_end,
             feature_derivation_window_start=feature_derivation_window_start,
             feature_engineering_graphs=feature_engineering_graphs,
             feature_engineering_options=feature_engineering_options,
             feature_engineering_prediction_point=feature_engineering_prediction_point,
             featurelist_id=featurelist_id,
             feature_settings=feature_settings,
+            force_cpu=force_cpu,
             forecast_window_end=forecast_window_end,
             forecast_window_start=forecast_window_start,
             gap_duration=gap_duration,
             holdout_duration=holdout_duration,
             holdout_end_date=holdout_end_date,
             holdout_level=holdout_level,
             holdout_pct=holdout_pct,
@@ -772,15 +773,14 @@
             segmentation_model_package_name=segmentation_model_package_name,
             segmentation_task_id=segmentation_task_id,
             segments_count=segments_count,
             target=target,
             target_type=target_type,
             training_level=training_level,
             treat_as_exponential=treat_as_exponential,
-            use_gpu=use_gpu,
             unsupervised_mode=unsupervised_mode,
             use_cross_series_features=use_cross_series_features,
             use_project_settings=use_project_settings,
             user_partition_col=user_partition_col,
             use_time_series=use_time_series,
             validation_duration=validation_duration,
             validation_level=validation_level,
@@ -818,14 +818,15 @@
         feature_derivation_window_end: Optional[int] = None,
         feature_derivation_window_start: Optional[int] = None,
         feature_engineering_graphs: Optional[List[RelationshipGraph]] = None,
         feature_engineering_options: Optional[FeatureEngineeringOptions] = None,
         feature_engineering_prediction_point: Optional[Feature] = None,
         featurelist_id: Optional[str] = None,
         feature_settings: Optional[List[FeatureSettings]] = None,
+        force_cpu: Optional[bool] = None,
         forecast_window_end: Optional[int] = None,
         forecast_window_start: Optional[int] = None,
         gap_duration: Optional[str] = None,
         holdout_duration: Optional[Duration] = None,
         holdout_end_date: Optional[str] = None,
         holdout_level: Optional[Union[str, int]] = None,
         holdout_pct: Optional[int] = None,
@@ -856,15 +857,14 @@
         segmentation_model_package_name: Optional[str] = None,
         segmentation_task_id: Optional[str] = None,
         segments_count: Optional[int] = None,
         target: Optional[str] = None,
         target_type: Optional[TARGET_TYPE] = None,
         training_level: Optional[Union[str, int]] = None,
         treat_as_exponential: Optional[TREAT_AS_EXPONENTIAL] = None,
-        use_gpu: Optional[bool] = None,
         unsupervised_mode: Optional[bool] = None,
         use_cross_series_features: Optional[bool] = None,
         use_project_settings: Optional[bool] = None,
         user_partition_col: Optional[Feature] = None,
         use_time_series: Optional[bool] = None,
         validation_duration: Optional[str] = None,
         validation_level: Optional[Union[str, int]] = None,
@@ -942,14 +942,15 @@
                     if "a_priori" not in feature_setting.keys()
                     else {"known_in_advance": feature_setting.pop("a_priori"), **feature_setting}
                 )
                 for feature_setting in feature_settings
             ]
         else:
             self.feature_settings = feature_settings
+        self.force_cpu = force_cpu
         self.forecast_window_end = forecast_window_end
         self.forecast_window_start = forecast_window_start
         self.gap_duration = gap_duration
         if holdout_duration and isinstance(holdout_duration, dict):
             self.holdout_duration = Duration(**holdout_duration)
         else:
             self.holdout_duration = holdout_duration
@@ -984,15 +985,14 @@
         self.segmentation_model_package_name = segmentation_model_package_name
         self.segmentation_task_id = segmentation_task_id
         self.segments_count = segments_count
         self.target = target
         self.target_type = target_type
         self.training_level = training_level
         self.treat_as_exponential = treat_as_exponential
-        self.use_gpu = use_gpu
         self.unsupervised_mode = unsupervised_mode
         self.use_cross_series_features = use_cross_series_features
         self.use_project_settings = use_project_settings
         if user_partition_col and isinstance(user_partition_col, dict):
             self.user_partition_col = Feature(**user_partition_col)
         else:
             self.user_partition_col = user_partition_col
@@ -1091,15 +1091,14 @@
             "model_splits": self.model_splits,
             "number_of_backtests": self.number_of_backtests,
             "prepare_model_for_deployment": self.prepare_model_for_deployment,
             "run_leakage_removed_feature_list": self.run_leakage_removed_feature_list,
             "smart_downsampled": self.smart_downsampled,
             "target": self.target,
             "treat_as_exponential": self.treat_as_exponential,
-            "use_gpu": self.use_gpu,
             "unsupervised_mode": self.unsupervised_mode,
             "use_supervised_feature_reduction": self.use_supervised_feature_reduction,
             "use_time_series": self.use_time_series,
             "validation_duration": self.validation_duration,
             "windows_basis_unit": self.windows_basis_unit,
         }
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/residuals.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/sharing.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
 
 import trafaret as t
 
 from datarobot._compat import String
-from datarobot.enums import SHARING_RECIPIENT_TYPE, SHARING_ROLE
-from datarobot.errors import InvalidUsageError
+from datarobot.enums import SHARING_ROLE
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
     class SharingAccessPayload(TypedDict, total=False):
         username: str
@@ -118,29 +117,28 @@
             payload["can_use_data"] = self.can_use_data
         return payload
 
 
 class SharingRole(APIObject):
     """
     Represents metadata about a user who has been granted access to an entity.
-    At least one of `id` or `username` must be set.
 
     Attributes
     ----------
     id : str or None
         The ID of the user.
     role : str
         Represents a particular level of access. Should be one of
         ``datarobot.enums.SHARING_ROLE``.
     can_share : bool
         Indicates whether this user is permitted to share with other users. When False, the
         user has access to the entity, but can only revoke their own access. They cannot not modify
         any user's access role. When True, the user can share with any other user at an access
         role up to their own.
-    share_recipient_type : SHARING_RECIPIENT_TYPE
+    share_recipient_type : str
         The type of user for the object of the method. Can be ``user`` or ``organization``.
     user_full_name : str or None
         The full name of the user.
     username : str or None
         The username (usually the email) of the user.
     """
 
@@ -154,21 +152,19 @@
             t.Key("can_share"): t.Bool,
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         role: SHARING_ROLE,
-        share_recipient_type: SHARING_RECIPIENT_TYPE,
+        share_recipient_type: str,
         can_share: bool,
         id: Optional[str] = None,
         user_full_name: Optional[str] = None,
         username: Optional[str] = None,
     ):
-        if not id and not username:
-            raise InvalidUsageError("Please include either a username or an ID of a user.")
         self.id = id
         self.user_full_name = user_full_name
         self.role = SHARING_ROLE[role]
         self.share_recipient_type = share_recipient_type
         self.username = username
         self.can_share = can_share
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/types.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/use_cases/use_case.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,50 +5,43 @@
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-#  pylint: disable=C0415
 from __future__ import annotations
 
-from dataclasses import dataclass
 from types import TracebackType
-from typing import Dict, List, Optional, Tuple, Type, TypeVar, Union
+from typing import cast, Dict, List, Optional, Tuple, Type, Union
 
 import trafaret as t
 
-from datarobot.context import Context, DefaultUseCase
-from datarobot.enums import (
-    SHARING_RECIPIENT_TYPE,
-    SHARING_ROLE,
-    UseCaseAPIPathEntityType,
-    UseCaseEntityType,
-    UseCaseReferenceEntityMap,
-)
+from datarobot.context import Context
+from datarobot.enums import SHARING_ROLE, UseCaseEntities
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
+from datarobot.models.application import Application
+from datarobot.models.dataset import Dataset
+from datarobot.models.notebooks import Notebook
+from datarobot.models.project import Project
 from datarobot.models.sharing import SharingRole
 from datarobot.utils.pagination import unpaginate
 
-T = TypeVar("T")
-
 use_case_user_trafaret = t.Dict(
     {
         t.Key("id"): t.String,
         t.Key("full_name", optional=True): t.Or(t.String, t.Null),
         t.Key("email", optional=True): t.Or(t.String, t.Null),
         t.Key("userhash", optional=True): t.Or(t.String, t.Null),
         t.Key("username", optional=True): t.Or(t.String, t.Null),
     }
 ).ignore_extra("*")
 
 
-@dataclass
 class UseCaseUser(APIObject):
     """Experiment container user.
 
     Attributes
     ----------
     id : str
         The id of the user.
@@ -60,28 +53,36 @@
         User's gravatar hash. Optional.
     username : str
         The username of the user. Optional.
     """
 
     _converter = use_case_user_trafaret
 
-    id: str
-    full_name: Optional[str] = None
-    email: Optional[str] = None
-    userhash: Optional[str] = None
-    username: Optional[str] = None
+    def __init__(
+        self,
+        id: str,
+        full_name: Optional[str] = None,
+        email: Optional[str] = None,
+        userhash: Optional[str] = None,
+        username: Optional[str] = None,
+    ):
+        self.id = id
+        self.full_name = full_name
+        self.email = email
+        self.userhash = userhash
+        self.username = username
 
 
 class UseCaseReferenceEntity(APIObject):
     """
     An entity associated with a Use Case.
 
     Attributes
     ----------
-    entity_type : UseCaseEntityType
+    entity_type : UseCaseEntities
         The type of the entity.
     use_case_id : str
         The Use Case this entity is associated with.
     id : str
         The ID of the entity.
     created_at : str
         The date and time this entity was linked with the Use Case.
@@ -102,15 +103,15 @@
             t.Key("is_deleted"): t.Bool,
         }
     ).ignore_extra("*")
 
     def __init__(
         self,
         id: str,
-        entity_type: UseCaseEntityType,
+        entity_type: UseCaseEntities,
         entity_id: str,
         use_case_id: str,
         created_at: str,
         created: Dict[str, str],
         is_deleted: bool,
     ):
         self.id = id
@@ -217,26 +218,14 @@
         self.notebooks_count: int = notebooks_count
         self.applications_count: int = applications_count
         self.members: List[UseCaseUser] = [UseCaseUser(**member) for member in members]
         self.owners: Optional[List[UseCaseUser]] = (
             [UseCaseUser(**owner) for owner in owners] if owners else None
         )
 
-    def __repr__(self) -> str:
-        return (
-            f"UseCase(id={self.id}, "
-            f"name={self.name}, "
-            f"description={self.description}, "
-            f"models={self.models_count}, "
-            f"projects={self.projects_count}, "
-            f"datasets={self.datasets_count}, "
-            f"notebooks={self.notebooks_count}, "
-            f"applications={self.applications_count})"
-        )
-
     @classmethod
     def get(cls, use_case_id: str) -> UseCase:
         """
         Gets information about a use case.
 
         Parameters
         ----------
@@ -339,33 +328,20 @@
         use_case_id : str
             The ID of the Use Case to be deleted.
         """
         path = f"{cls._path}{use_case_id}/"
         cls._client.delete(path)
         return None
 
-    @classmethod
-    def _resolve_api_entity(
-        cls, entity_type: Optional[UseCaseEntityType] = None
-    ) -> UseCaseAPIPathEntityType | None:
-        """
-        For a given reference entity type, return the corresponding API endpoint type.
-        """
-        if entity_type == UseCaseEntityType.NOTEBOOK:
-            raise InvalidUsageError(
-                "Notebooks are currently unavailable for adding or removing from Use Cases via the API."
-            )
-        return UseCaseReferenceEntityMap.get(entity_type)
-
     def __enter__(self) -> UseCase:
         # Not declared in __init__ because this attribute has a very
         # specific use in context management and nowhere else
-        # pylint: disable-next=attribute-defined-outside-init
-        self.__previous: DefaultUseCase = Context.get_use_case(raw=True)
-
+        self.__previous: UseCase = cast(  # pylint: disable=attribute-defined-outside-init
+            UseCase, Context.use_case
+        )
         Context.use_case = self
         return self
 
     def __exit__(
         self,
         __exc_type: Type[BaseException] | None,
         __exc_value: BaseException | None,
@@ -392,84 +368,69 @@
         """
         payload = {"name": name, "description": description}
         path = f"{self._path}{self.id}/"
         r_data = self._client.patch(path, data=payload).json()
         return self.from_server_data(r_data)
 
     def _get_reference_entity_info(
-        self, entity: Union[UseCaseReferenceEntity, T]
-    ) -> Tuple[UseCaseAPIPathEntityType, Optional[str]]:
+        self, entity: Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+    ) -> Tuple[UseCaseEntities, Optional[str]]:
         """
         Get the entity type and entity id for a reference entity instance
         Parameters
         ----------
-        entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
+        entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             The entity instance to add to a Use Case.
         Returns
         -------
-        entity_info : Tuple[UseCaseEntityType, str]
+        entity_info : Tuple[UseCaseEntities, str]
             The entity type and entity id
         """
-        from ..application import Application
-        from ..dataset import Dataset
-        from ..prediction_dataset import PredictionDataset
-        from ..project import Project
-
         if isinstance(entity, Project):
-            return UseCaseAPIPathEntityType.PROJECT, entity.id
+            return UseCaseEntities.PROJECT, entity.id
         elif isinstance(entity, Dataset):
-            return UseCaseAPIPathEntityType.DATASET, entity.id
+            return UseCaseEntities.DATASET, entity.id
+        elif isinstance(entity, Notebook):
+            return UseCaseEntities.NOTEBOOK, entity.id
         elif isinstance(entity, Application):
-            return UseCaseAPIPathEntityType.APPLICATION, entity.id
+            return UseCaseEntities.APPLICATION, entity.id
         elif isinstance(entity, UseCaseReferenceEntity):
-            entity_type = UseCaseReferenceEntityMap.get(entity.entity_type)
-            if entity_type:
-                return entity_type, entity.entity_id
-        error_message = (
-            f"Entity must be Project, Dataset, Application, "
-            f"or UseCaseReferenceEntity. Invalid type: {type(entity).__name__}."
+            return entity.entity_type, entity.entity_id
+        raise TypeError(
+            "entity must be Project, Dataset, Notebook, Application, or UseCaseReferenceEntity"
         )
-        if isinstance(entity, UseCaseReferenceEntity):
-            # If we're failing here, it's because the UseCaseReferenceEntity is a notebook or other unsupported type
-            error_message = error_message + f" Unsupported Entity Type: {entity.entity_type}."
-        if isinstance(entity, PredictionDataset):
-            # Adding a specific error for PredictionDataset since the name would indicate it could
-            # be treated as a Dataset, when in fact it's a separate entity and not a subclass.
-            error_message = (
-                error_message + " PredictionDataset is not a subclass of Dataset and "
-                "cannot be added to a UseCase at this time."
-            )
-        raise TypeError(error_message)
 
     def add(
         self,
-        entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
-        entity_type: Optional[UseCaseEntityType] = None,
+        entity: Optional[
+            Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+        ] = None,
+        entity_type: Optional[UseCaseEntities] = None,
         entity_id: Optional[str] = None,
     ) -> UseCaseReferenceEntity:
         """
-        Add an entity (project, dataset, etc.) to a Use Case. Can only accept either an entity or
+        Add an entity (project, notebook, dataset, etc.) to a Use Case. Can only accept either an entity or
         an entity type and entity ID, but not both.
 
         Parameters
         ----------
-        entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
+        entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             An existing entity linked to a different Use Case to be linked to this Use Case.
             Can not be used if entity_type and entity_id are passed.
-        entity_type : UseCaseEntityType
+        entity_type : UseCaseEntities
             The entity type of the entity to link to this Use Case. Can not be used if entity is passed.
         entity_id : str
             The ID of the entity to link to this Use Case. Can not be used if entity is passed.
 
         Returns
         -------
         use_case_reference_entity : UseCaseReferenceEntity
             The newly created reference link between this Use Case and the entity.
         """
-        e_type = self._resolve_api_entity(entity_type)
+        e_type = entity_type
         e_id = entity_id
         if entity and (e_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not e_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
@@ -477,32 +438,34 @@
             e_type, e_id = self._get_reference_entity_info(entity)
         path = f"{self._path}{self.id}/{e_type}/{e_id}/"
         r_data = self._client.post(path)
         return UseCaseReferenceEntity.from_server_data(r_data.json())
 
     def remove(
         self,
-        entity: Optional[Union[UseCaseReferenceEntity, T]] = None,
-        entity_type: Optional[UseCaseEntityType] = None,
+        entity: Optional[
+            Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
+        ] = None,
+        entity_type: Optional[UseCaseEntities] = None,
         entity_id: Optional[str] = None,
     ) -> None:
         """
         Remove an entity from a Use Case. Only supports passing an entity instance, or an entity type and ID.
 
         Parameters
         ----------
-        entity : Union[UseCaseReferenceEntity, Project, Dataset, Application]
+        entity : Union[UseCaseReferenceEntity, Project, Dataset, Notebook, Application]
             An existing entity instance to be removed from a Use Case.
             Can not be used if entity_type and entity_id are passed.
-        entity_type : UseCaseEntityType
+        entity_type : UseCaseEntities
             The entity type of the entity to link to this Use Case. Can not be used if entity is passed.
         entity_id : str
             The ID of the entity to link to this Use Case.  Can not be used if entity is passed.
         """
-        e_type = self._resolve_api_entity(entity_type)
+        e_type = entity_type
         e_id = entity_id
         if entity and (entity_type or entity_id):
             raise InvalidUsageError(
                 "Can only accept either an entity, or an entity type and entity id."
             )
         if not entity and (not entity_type or not entity_id):
             raise InvalidUsageError("Missing entity, or an entity type and entity id.")
@@ -519,78 +482,32 @@
         """
         Share this Use Case or remove access from one (or multiple) user(s).
 
         Parameters
         ----------
         roles : List[SharingRole]
             The users to share or remove access from this Use Case and their access levels.
-            Currently, the only supported roles for Use Cases are OWNER, EDITOR, and CONSUMER,
-            and the only supported SHARING_RECIPIENT_TYPE is USER.
+            Currently, the only supported roles for Use Cases are OWNER, EDITOR, and CONSUMER.
             To remove access, set a user's role to ``datarobot.enums.SHARING_ROLE.NO_ROLE``.
 
-        Examples
-        --------
-        The SharingRole :class:`datarobot.models.sharing.SharingRole` class is needed in order to
-        share a Use Case with one or more users.
-
-        For example, suppose you had a list of user IDs you wanted to share this Use Case with. You could use
-        a loop to generate a list of SharingRole objects for them, and bulk share this Use Case.
-
-        .. code-block:: python
-
-            >>> from datarobot.models.use_cases.use_case import UseCase
-            >>> from datarobot.models.sharing import SharingRole
-            >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
-            >>>
-            >>> user_ids = ["60912e09fd1f04e832a575c1", "639ce542862e9b1b1bfa8f1b", "63e185e7cd3a5f8e190c6393"]
-            >>> sharing_roles = []
-            >>> for user_id in user_ids:
-            ...     new_sharing_role = SharingRole(
-            ...         role=SHARING_ROLE.CONSUMER,
-            ...         share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
-            ...         id=user_id,
-            ...         can_share=True,
-            ...     )
-            ...     sharing_roles.append(new_sharing_role)
-            >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
-            >>> use_case.share(roles=sharing_roles)
-
-        Similarly, a `SharingRole` instance can be used to remove a user's access if the `role`
-        is set to `SHARING_ROLE.NO_ROLE`, like in this example:
-
-        .. code-block:: python
-
-            >>> from datarobot.models.use_cases.use_case import UseCase
-            >>> from datarobot.models.sharing import SharingRole
-            >>> from datarobot.enums import SHARING_ROLE, SHARING_RECIPIENT_TYPE
-            >>>
-            >>> user_to_remove = "foo.bar@datarobot.com"
-            ... remove_sharing_role = SharingRole(
-            ...     role=SHARING_ROLE.NO_ROLE,
-            ...     share_recipient_type=SHARING_RECIPIENT_TYPE.USER,
-            ...     username=user_to_remove,
-            ...     can_share=False,
-            ... )
-            >>> use_case = UseCase.get(use_case_id="5f33f1fd9071ae13568237b2")
-            >>> use_case.share(roles=[remove_sharing_role])
         """
         if any(
             role.role
             not in [
                 SHARING_ROLE.NO_ROLE,
                 SHARING_ROLE.OWNER,
                 SHARING_ROLE.EDITOR,
                 SHARING_ROLE.CONSUMER,
             ]
             for role in roles
         ):
             raise InvalidUsageError(
                 "Only NO_ROLE, OWNER, EDITOR, and CONSUMER roles are supported by Use Cases"
             )
-        if any(role.share_recipient_type != SHARING_RECIPIENT_TYPE.USER for role in roles):
+        if any(role.share_recipient_type != "user" for role in roles):
             raise InvalidUsageError(
                 "Use Cases currently only support sharing with users, not organizations."
             )
         formatted_roles = []
         for role in roles:
             formatted_role = {"role": role.role, "shareRecipientType": role.share_recipient_type}
             if role.id:
@@ -622,45 +539,39 @@
             Return the access control information for a user with this user ID. Optional.
         """
         params = {"offset": offset, "limit": limit, "id": id}
         path = f"{self._path}{self.id}/sharedRoles/"
         r_data = unpaginate(path, params, self._client)
         return [SharingRole.from_server_data(data) for data in r_data]
 
-    def list_projects(self) -> List[T]:
+    def list_notebooks(self) -> List[Notebook]:
         """
-        List all projects associated with this Use Case.
+        List all notebooks associated with this Use Case.
 
         Returns
         -------
-        projects : List[Project]
-            All projects associated with this Use Case.
+        notebooks : List[Notebook]
+            All notebooks associated with this Use Case.
         """
-        from ..project import Project
+        return Notebook.list(use_case_id=self.id)
 
-        return Project.list(search_params={"experiment_container_ids": self.id})  # type: ignore[return-value]
-
-    def list_datasets(self) -> List[T]:
+    def list_projects(self) -> List[Project]:
         """
-        List all datasets associated with this Use Case.
+        List all projects associated with this Use Case.
 
         Returns
         -------
-        datasets : List[Dataset]
-            All datasets associated with this Use Case.
+        projects : List[Project]
+            All projects associated with this Use Case.
         """
-        from ..dataset import Dataset
-
-        return Dataset.list(use_cases=self.id)  # type: ignore[return-value]
+        return Project.list(search_params={"experiment_container_id": self.id})
 
-    def list_applications(self) -> List[T]:
+    def list_datasets(self) -> List[Dataset]:
         """
-        List all applications associated with this Use Case.
+        List all datasets associated with this Use Case.
 
         Returns
         -------
-        applications : List[Application]
-            All applications associated with this Use Case.
+        datasets : List[Dataset]
+            All datasets associated with this Use Case.
         """
-        from ..application import Application
-
-        return Application.list(use_cases=self.id)  # type: ignore[return-value]
+        return Dataset.list(use_case_ids=self.id)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import trafaret as t
 from urllib3 import Retry
 
 from datarobot.mixins.browser_mixin import BrowserMixin
 
 from ._compat import Int, String
 from ._version import __version__
+from .context import Context
 from .enums import DEFAULT_TIMEOUT
 from .errors import ClientError, JobAlreadyRequested, PlatformDeprecationWarning, ServerError
 from .utils import to_api
 
 if TYPE_CHECKING:
     from io import BufferedReader, IOBase
 
@@ -328,18 +329,15 @@
         # pylint rule disabled because we wanted a clearer docstring
         # for this function than what is provided by APIObject, and
         # this is the only way I know to do this other than writing
         # manual docs in the .rst files
         return super(RESTClientObject, self).open_in_browser()
 
 
-def _http_message(response: Response) -> str:
-    """
-    Helper function to retrieve the message from a Response object.
-    """
+def _http_message(response: Response) -> str:  # pylint: disable=missing-function-docstring
     if response.status_code == 401:
         message = (
             "The server is saying you are not properly "
             "authenticated. Please make sure your API "
             "token is valid."
         )
     elif response.headers["content-type"] == "application/json":
@@ -410,36 +408,39 @@
             t.Key("endpoint"): String(),
             t.Key("token"): String(),
             t.Key("connect_timeout", optional=True): Int(),
             t.Key("ssl_verify", optional=True): t.Or(t.Bool(), String()),
             t.Key("user_agent_suffix", optional=True): String(),
             t.Key("max_retries", optional=True): Int(),
             t.Key("token_type", optional=True): String(),
-            t.Key("default_use_case", optional=True): String(),
+            t.Key("use_case", optional=True): String(),
         }
     ).allow_extra("*")
     _fields = {k.to_name or k.name for k in _converter.keys}
 
     def __init__(
         self,
         endpoint: str,
         token: str,
         connect_timeout: Optional[int] = None,
         ssl_verify: bool = True,
         user_agent_suffix: Optional[str] = None,
         max_retries: Optional[Union[int, Retry]] = None,
         token_type: Optional[str] = None,
-        default_use_case: Optional[str] = None,
+        use_case: Optional[str] = None,
     ) -> None:
         self.endpoint = endpoint
         self.token = token
         self.connect_timeout = connect_timeout
         self.ssl_verify = ssl_verify
         self.user_agent_suffix = user_agent_suffix
         self.max_retries = max_retries
         self.token_type = token_type
-        self.default_use_case = default_use_case
+        self.use_case = use_case
+
+        if self.use_case is not None:
+            Context.use_case = self.use_case
 
     @classmethod
     def from_data(cls, data: Dict[str, Any]) -> DataRobotClientConfig:
         checked = {k: v for k, v in cls._converter.check(data).items() if k in cls._fields}
         return cls(**checked)
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.5.8/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.5.29
+Version: 3.2.0.2023.5.8
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 datarobot/_experimental/models/__init__.py
 datarobot/_experimental/models/data_matching.py
 datarobot/_experimental/models/enums.py
 datarobot/_experimental/models/idiomatic_project.py
 datarobot/_experimental/models/model.py
 datarobot/_experimental/models/model_lineage.py
 datarobot/_experimental/models/model_package.py
-datarobot/_experimental/models/notebooks.py
 datarobot/_experimental/models/project_options.py
 datarobot/_experimental/models/retraining.py
 datarobot/_experimental/models/documentai/__init__.py
 datarobot/_experimental/models/documentai/document.py
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
+datarobot/helpers/deployment_monitoring.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
 datarobot/helpers/image_utils.py
 datarobot/helpers/partitioning_methods.py
 datarobot/mixins/__init__.py
 datarobot/mixins/browser_mixin.py
 datarobot/mixins/update_attributes_mixin.py
@@ -75,14 +75,15 @@
 datarobot/models/featurelist.py
 datarobot/models/imported_model.py
 datarobot/models/job.py
 datarobot/models/lift_chart.py
 datarobot/models/missing_report.py
 datarobot/models/model.py
 datarobot/models/modeljob.py
+datarobot/models/notebooks.py
 datarobot/models/pairwise_statistics.py
 datarobot/models/pareto_front.py
 datarobot/models/payoff_matrix.py
 datarobot/models/predict_job.py
 datarobot/models/prediction_dataset.py
 datarobot/models/prediction_explanations.py
 datarobot/models/prediction_server.py
@@ -109,15 +110,14 @@
 datarobot/models/validators.py
 datarobot/models/word_cloud.py
 datarobot/models/deployment/__init__.py
 datarobot/models/deployment/accuracy.py
 datarobot/models/deployment/bias_and_fairness.py
 datarobot/models/deployment/data_drift.py
 datarobot/models/deployment/deployment.py
-datarobot/models/deployment/mixins.py
 datarobot/models/deployment/service_stats.py
 datarobot/models/deployment/sharing.py
 datarobot/models/external_dataset_scores_insights/__init__.py
 datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
 datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
 datarobot/models/external_dataset_scores_insights/external_lift_chart.py
 datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.5.8/datarobot_early_access.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 pandas>=0.15
 numpy
 pyyaml>=3.11
 requests>=2.28.1
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
 urllib3<2.0.0,>=1.23
-typing-extensions<5,>=4.3.0
-mypy-extensions<2,>=0.4.0
+typing-extensions==4.3.0
 
 [dev]
 mock==3.0.5
 pytest==7.1.2
 pytest-cov
 responses==0.21
 pytest-asyncio
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/pyproject.toml` & `datarobot_early_access-3.2.0.2023.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     ### START Models directory
     ### These rules are purposely one file at a time in this directory so any new files added _must_ have annotations
     ### And also we can delete an entry for a file and fix the corresponding errors as we piece-meal annotate the whole repo.
     "datarobot.models.api_object",
     "datarobot.models.batch_prediction_job",
     "datarobot.models.custom_model",
     "datarobot.models.custom_model_test",
+    "datarobot.models.custom_model_version",
     "datarobot.models.custom_task_version",
     "datarobot.models.data_engine_query_generator",
     "datarobot.models.datetime_trend_plots",
     "datarobot.models.execution_environment",
     "datarobot.models.execution_environment_version",
     "datarobot.models.feature",
     "datarobot.models.feature_effect",
```

### Comparing `datarobot_early_access-3.2.0.2023.5.29/setup.py` & `datarobot_early_access-3.2.0.2023.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.5.29/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.5.8/setup_weekly.py`

 * *Files identical despite different names*


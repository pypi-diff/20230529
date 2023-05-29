# Comparing `tmp/tfy-mlflow-client-0.0.8.tar.gz` & `tmp/tfy-mlflow-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfy-mlflow-client-0.0.8.tar", last modified: Fri May  6 08:57:48 2022, max compression
+gzip compressed data, was "tfy-mlflow-client-0.0.9.tar", last modified: Fri Jun  3 08:48:19 2022, max compression
```

## Comparing `tfy-mlflow-client-0.0.8.tar` & `tfy-mlflow-client-0.0.9.tar`

### file list

```diff
@@ -1,291 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11382 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7172 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/README_SKINNY.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.048264 tfy-mlflow-client-0.0.8/mlflow/
--rw-r--r--   0 runner    (1001) docker     (121)     6146 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/_spark_autologging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.048264 tfy-mlflow-client-0.0.8/mlflow/azure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5814 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/azure/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.048264 tfy-mlflow-client-0.0.8/mlflow/azureml/
--rw-r--r--   0 runner    (1001) docker     (121)    31543 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/azureml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/azureml/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    13056 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/catboost.py
--rw-r--r--   0 runner    (1001) docker     (121)    18027 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.048264 tfy-mlflow-client-0.0.8/mlflow/deployments/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9678 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9884 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/deployments/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/entities/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/_mlflow_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/auth_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/columns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/entity_subject_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/experiment_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/file_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/lifecycle_stage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/_model_registry_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_stages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/registered_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/registered_model_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/param.py
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6462 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run_log.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/run_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/source_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/user_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/entities/view_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5004 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/fastai/
--rw-r--r--   0 runner    (1001) docker     (121)    23154 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/fastai/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/gluon/
--rw-r--r--   0 runner    (1001) docker     (121)    16722 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/gluon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/gluon/_autolog.py
--rw-r--r--   0 runner    (1001) docker     (121)    12298 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/h2o.py
--rw-r--r--   0 runner    (1001) docker     (121)    35643 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/keras.py
--rw-r--r--   0 runner    (1001) docker     (121)    26537 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/ml-package-versions.yml
--rw-r--r--   0 runner    (1001) docker     (121)    12564 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/mleap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6783 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/models/container/
--rw-r--r--   0 runner    (1001) docker     (121)     8258 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/container/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/models/container/scoring_server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/container/scoring_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/container/scoring_server/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.052264 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (121)    32166 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    24474 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/default_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/evaluator_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/evaluation/lift_curve.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/flavor_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/flavor_backend_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     9179 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16539 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/paddle/
--rw-r--r--   0 runner    (1001) docker     (121)    21752 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/paddle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4590 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/paddle/_paddle_autolog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/projects/
--rw-r--r--   0 runner    (1001) docker     (121)    15342 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/_project_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/projects/backend/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/backend/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/backend/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)    14128 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    19468 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/databricks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     6338 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/submitted_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    12210 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/projects/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12228 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/prophet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/protos/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18645 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/databricks_artifacts_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    29871 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/databricks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    11954 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/mlflow_artifacts_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    10762 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/mlfoundry_remote_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)   102524 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/model_registry_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/protos/scalapb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/scalapb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7327 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/scalapb/scalapb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)   171007 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/protos/service_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/pyfunc/
--rw-r--r--   0 runner    (1001) docker     (121)    59514 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/mlserver.py
--rw-r--r--   0 runner    (1001) docker     (121)    12698 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/pyfunc/scoring_server/
--rw-r--r--   0 runner    (1001) docker     (121)    14392 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/scoring_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/scoring_server/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/spark_model_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyfunc/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)  7106583 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pypi_package_index.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/pyspark/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyspark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.056264 tfy-mlflow-client-0.0.8/mlflow/pyspark/ml/
--rw-r--r--   0 runner    (1001) docker     (121)    45343 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyspark/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)    41206 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12894 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pytorch/_pytorch_autolog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/pytorch/pickle_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/rfunc/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/rfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/rfunc/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (121)    80931 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21012 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/sagemaker/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    25115 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)    78467 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33288 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/sklearn/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12519 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/spacy.py
--rw-r--r--   0 runner    (1001) docker     (121)    36255 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/spark.py
--rw-r--r--   0 runner    (1001) docker     (121)    22085 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/store/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/store/artifact/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10212 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5274 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/artifact_repository_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    29706 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/databricks_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    10186 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5034 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/ftp_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/gcs_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/http_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/local_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5830 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/models_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/runs_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     9143 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/s3_artifact_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/sftp_artifact_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/store/artifact/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/artifact/utils/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/store/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/db/base_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/db/db_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.060264 tfy-mlflow-client-0.0.8/mlflow/store/entities/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/entities/paged_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9705 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/abstract_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/dbmodels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/dbmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/dbmodels/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    16170 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/rest_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    38568 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/model_registry/sqlalchemy_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/store/tracking/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12951 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/tracking/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    39123 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/tracking/file_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    15792 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/store/tracking/rest_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (121)    45450 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tensorflow/_autolog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/tracking/
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14477 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/fluent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     6042 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21069 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/artifact_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)   115635 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.064264 tfy-mlflow-client-0.0.8/mlflow/tracking/context/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/abstract_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_cluster_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_command_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_job_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_notebook_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/default_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/git_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/context/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    63156 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/fluent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.068264 tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.068264 tfy-mlflow-client-0.0.8/mlflow/types/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15346 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/types/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.068264 tfy-mlflow-client-0.0.8/mlflow/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     5712 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/_capture_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/_spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/arguments_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/
--rw-r--r--   0 runner    (1001) docker     (121)    24857 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15652 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10937 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/events.py
--rw-r--r--   0 runner    (1001) docker     (121)    13396 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-r--r--   0 runner    (1001) docker     (121)    41279 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/safety.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/class_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (121)     6688 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/databricks_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6222 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/docstring_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (121)    12118 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    15225 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    24167 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/gorilla.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/mlflow/utils/import_hooks/
--rw-r--r--   0 runner    (1001) docker     (121)    13048 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/import_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/mlflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (121)    14573 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/proto_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14555 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/requirements_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14186 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/rest_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    33840 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12625 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/uri.py
--rw-r--r--   0 runner    (1001) docker     (121)    16047 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/mlflow/xgboost/
--rw-r--r--   0 runner    (1001) docker     (121)    31151 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/mlflow/xgboost/_autolog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/pylint_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/pylint_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/pylint_plugins/pytest_raises_without_match/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/pylint_plugins/pytest_raises_without_match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6275 2022-05-06 08:57:45.000000 tfy-mlflow-client-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 08:57:48.072264 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-06 08:57:47.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7996 2022-05-06 08:57:48.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-06 08:57:47.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-06 08:57:47.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-06 08:57:47.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-06 08:57:47.000000 tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11382 2022-06-03 08:48:13.000000 tfy-mlflow-client-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-06-03 08:48:13.000000 tfy-mlflow-client-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7172 2022-06-03 08:48:13.000000 tfy-mlflow-client-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-06-03 08:48:13.000000 tfy-mlflow-client-0.0.9/README_SKINNY.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.172096 tfy-mlflow-client-0.0.9/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (121)     6242 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9570 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/_spark_autologging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.172096 tfy-mlflow-client-0.0.9/mlflow/azure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5814 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/azure/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.176096 tfy-mlflow-client-0.0.9/mlflow/azureml/
+-rw-r--r--   0 runner    (1001) docker     (121)    31543 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/azureml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/azureml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13056 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18027 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/db.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.176096 tfy-mlflow-client-0.0.9/mlflow/deployments/
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9678 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9884 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/deployments/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/entities/
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/_mlflow_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/auth_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/columns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/entity_subject_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3761 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/experiment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/file_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/lifecycle_stage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_stages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/registered_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/registered_model_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3089 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6697 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3019 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      890 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/run_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/entities/view_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3217 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5004 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/fastai/
+-rw-r--r--   0 runner    (1001) docker     (121)    23154 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/fastai/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/gluon/
+-rw-r--r--   0 runner    (1001) docker     (121)    16722 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/gluon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/gluon/_autolog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12298 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/h2o.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35643 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/keras.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26537 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10947 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/ml-package-versions.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    12564 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/mleap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6783 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.180096 tfy-mlflow-client-0.0.9/mlflow/models/container/
+-rw-r--r--   0 runner    (1001) docker     (121)     8258 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/container/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.184096 tfy-mlflow-client-0.0.9/mlflow/models/container/scoring_server/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/container/scoring_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/container/scoring_server/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5029 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.184096 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32166 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24474 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/default_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/evaluator_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/evaluation/lift_curve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/flavor_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/flavor_backend_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9179 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/signature.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16539 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.184096 tfy-mlflow-client-0.0.9/mlflow/paddle/
+-rw-r--r--   0 runner    (1001) docker     (121)    21752 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/paddle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4590 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/paddle/_paddle_autolog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.184096 tfy-mlflow-client-0.0.9/mlflow/projects/
+-rw-r--r--   0 runner    (1001) docker     (121)    15342 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/_project_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.184096 tfy-mlflow-client-0.0.9/mlflow/projects/backend/
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/backend/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/backend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14128 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19468 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/docker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6338 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/submitted_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12210 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/projects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12228 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/prophet.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.188096 tfy-mlflow-client-0.0.9/mlflow/protos/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8710 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/databricks_artifacts_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10804 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/databricks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5235 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/mlfoundry_remote_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51879 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/model_registry_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.188096 tfy-mlflow-client-0.0.9/mlflow/protos/scalapb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/scalapb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3307 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78892 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/protos/service_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/pyfunc/
+-rw-r--r--   0 runner    (1001) docker     (121)    59514 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7072 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/mlserver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12698 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/pyfunc/scoring_server/
+-rw-r--r--   0 runner    (1001) docker     (121)    14392 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/scoring_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/spark_model_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyfunc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)  7106583 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pypi_package_index.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyspark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/pyspark/ml/
+-rw-r--r--   0 runner    (1001) docker     (121)    45343 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyspark/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)    41206 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12894 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pytorch/_pytorch_autolog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/pytorch/pickle_module.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/rfunc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/rfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/rfunc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (121)    80931 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21012 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/sagemaker/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25115 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (121)    78467 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33288 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/sklearn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12519 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36255 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/spark.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22085 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/store/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.196097 tfy-mlflow-client-0.0.9/mlflow/store/artifact/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10212 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5274 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/artifact_repository_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29706 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10186 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5034 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/http_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/local_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5830 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/models_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6016 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/runs_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9143 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/s3_artifact_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/sftp_artifact_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/artifact/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/artifact/utils/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/db/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/db/base_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/db/db_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7499 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/entities/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/entities/paged_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9705 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/abstract_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/dbmodels/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/dbmodels/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16170 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/rest_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38568 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/model_registry/sqlalchemy_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/store/tracking/
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13115 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/tracking/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39123 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/tracking/file_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16554 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/store/tracking/rest_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.200096 tfy-mlflow-client-0.0.9/mlflow/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (121)    45450 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tensorflow/_autolog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.204097 tfy-mlflow-client-0.0.9/mlflow/tracking/
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.204097 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14477 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3692 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6042 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.204097 tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21457 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6781 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/artifact_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)   116086 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.208097 tfy-mlflow-client-0.0.9/mlflow/tracking/context/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/abstract_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_cluster_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_command_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_job_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_notebook_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/default_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/git_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/context/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)    63156 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.208097 tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.208097 tfy-mlflow-client-0.0.9/mlflow/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15346 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/types/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.212097 tfy-mlflow-client-0.0.9/mlflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     5712 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/_capture_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/_spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/arguments_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)    24857 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15652 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10937 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13396 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41279 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/safety.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/class_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6688 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/conda.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/databricks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6222 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/docstring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12118 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15225 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24167 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/gorilla.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/mlflow/utils/import_hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)    13048 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/import_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/mlflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14573 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/proto_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14555 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/requirements_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14186 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/rest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33840 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12625 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/uri.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16407 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/mlflow/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (121)    31151 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/mlflow/xgboost/_autolog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/pylint_plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/pylint_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/pylint_plugins/pytest_raises_without_match/
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/pylint_plugins/pytest_raises_without_match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6281 2022-06-03 08:48:14.000000 tfy-mlflow-client-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 08:48:19.216097 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8024 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-03 08:48:19.000000 tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/top_level.txt
```

### Comparing `tfy-mlflow-client-0.0.8/LICENSE.txt` & `tfy-mlflow-client-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/README.rst` & `tfy-mlflow-client-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/README_SKINNY.rst` & `tfy-mlflow-client-0.0.9/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,55 +25,59 @@
 The fluent tracking API is not currently threadsafe. Any concurrent callers to the tracking API must
 implement mutual exclusion manually.
 
 For a lower level API, see the :py:mod:`mlflow.tracking` module.
 """
 import sys
 
-from mlflow.version import VERSION as __version__  # pylint: disable=unused-import
-from mlflow.utils.logging_utils import _configure_mlflow_loggers
-import mlflow.tracking._model_registry.fluent
-import mlflow.tracking.fluent
-
 # Filter annoying Cython warnings that serve no good purpose, and so before
 # importing other modules.
 # See: https://github.com/numpy/numpy/pull/432/commits/170ed4e33d6196d7
 import warnings
 
+# isort: off
+# this needs to be imported before importing any other mlflow modules
+from mlflow.version import VERSION as __version__  # pylint: disable=unused-import
+
+# isort: on
+import mlflow.tracking._model_registry.fluent
+import mlflow.tracking.fluent
+from mlflow.utils.logging_utils import _configure_mlflow_loggers
+
 warnings.filterwarnings("ignore", message="numpy.dtype size changed")
 warnings.filterwarnings("ignore", message="numpy.ufunc size changed")
 
+import mlflow.models
 import mlflow.projects as projects
 import mlflow.tracking as tracking
-import mlflow.models
 
 # model flavors
 _model_flavors_supported = []
 try:
     # pylint: disable=unused-import
     import mlflow.catboost as catboost
     import mlflow.fastai as fastai
     import mlflow.gluon as gluon
     import mlflow.h2o as h2o
     import mlflow.keras as keras
     import mlflow.lightgbm as lightgbm
     import mlflow.mleap as mleap
     import mlflow.onnx as onnx
+    import mlflow.paddle as paddle
+    import mlflow.prophet as prophet
     import mlflow.pyfunc as pyfunc
+    import mlflow.pyspark as pyspark
     import mlflow.pytorch as pytorch
+    import mlflow.shap as shap
     import mlflow.sklearn as sklearn
     import mlflow.spacy as spacy
     import mlflow.spark as spark
     import mlflow.statsmodels as statsmodels
     import mlflow.tensorflow as tensorflow
     import mlflow.xgboost as xgboost
-    import mlflow.shap as shap
-    import mlflow.pyspark as pyspark
-    import mlflow.paddle as paddle
-    import mlflow.prophet as prophet
 
     _model_flavors_supported = [
         "catboost",
         "fastai",
         "gluon",
         "h2o",
         "keras",
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/_spark_autologging.py` & `tfy-mlflow-client-0.0.9/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/azure/client.py` & `tfy-mlflow-client-0.0.9/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/azureml/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/azureml/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/azureml/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/azureml/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/catboost.py` & `tfy-mlflow-client-0.0.9/mlflow/catboost.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/data.py` & `tfy-mlflow-client-0.0.9/mlflow/data.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/db.py` & `tfy-mlflow-client-0.0.9/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/base.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/interface.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/plugin_manager.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/deployments/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from mlflow.entities.param import Param
 from mlflow.entities.run import Run
 from mlflow.entities.run_data import RunData
 from mlflow.entities.run_info import RunInfo
 from mlflow.entities.run_log import RunLog
 from mlflow.entities.run_status import RunStatus
 from mlflow.entities.run_tag import RunTag
+from mlflow.entities.sentinel import SENTINEL
 from mlflow.entities.source_type import SourceType
 from mlflow.entities.view_type import ViewType
 
 __all__ = [
     "Experiment",
     "FileInfo",
     "Metric",
@@ -37,8 +38,9 @@
     "LifecycleStage",
     "SubjectType",
     "EntityType",
     "Role",
     "EntitySubjectRole",
     "Columns",
     "RunLog",
+    "SENTINEL",
 ]
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/_mlflow_object.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/auth_enums.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/auth_enums.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/columns.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/columns.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/entity_subject_role.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/entity_subject_role.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/experiment.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,27 @@
         artifact_location,
         lifecycle_stage,
         tags=None,
         creator_user_id=None,
         owner_subject_id=None,
         num_runs=None,
         num_user_collaborators=None,
+        description=None,
     ):
         super().__init__()
         self._experiment_id = experiment_id
         self._name = name
         self._artifact_location = artifact_location
         self._lifecycle_stage = lifecycle_stage
         self._tags = {tag.key: tag.value for tag in (tags or [])}
         self._creator_user_id = creator_user_id
         self._owner_subject_id = owner_subject_id
         self._num_runs = num_runs
         self._num_user_collaborators = num_user_collaborators
+        self._description = description
 
     @property
     def experiment_id(self):
         """String ID of the experiment."""
         return self._experiment_id
 
     @property
@@ -78,25 +80,30 @@
     def tags(self):
         """Tags that have been set on the experiment."""
         return self._tags
 
     def _add_tag(self, tag):
         self._tags[tag.key] = tag.value
 
+    @property
+    def description(self):
+        return self._description
+
     @classmethod
     def from_proto(cls, proto):
         experiment = cls(
             proto.experiment_id,
             proto.name,
             proto.artifact_location,
             proto.lifecycle_stage,
             creator_user_id=proto.creator_user_id,
             owner_subject_id=proto.owner_subject_id,
             num_runs=proto.num_runs,
             num_user_collaborators=proto.num_user_collaborators,
+            description=proto.description,
         )
         for proto_tag in proto.tags:
             experiment._add_tag(ExperimentTag.from_proto(proto_tag))
         return experiment
 
     def to_proto(self):
         experiment = ProtoExperiment()
@@ -107,8 +114,9 @@
         experiment.tags.extend(
             [ProtoExperimentTag(key=key, value=val) for key, val in self._tags.items()]
         )
         experiment.creator_user_id = self.creator_user_id
         experiment.owner_subject_id = self.owner_subject_id
         experiment.num_runs = self.num_runs
         experiment.num_user_collaborators = self.num_user_collaborators
+        experiment.description = self.description or ""
         return experiment
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/experiment_tag.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/file_info.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/lifecycle_stage.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/metric.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_stages.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_status.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/model_version_tag.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/registered_model.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/model_registry/registered_model_tag.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/param.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run_data.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run_info.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         start_time,
         end_time,
         lifecycle_stage,
         artifact_uri=None,
         run_id=None,
         name="",
         fqn="",
+        description=None,
     ):
         if run_uuid is None:
             raise Exception("run_uuid cannot be None")
         if experiment_id is None:
             raise Exception("experiment_id cannot be None")
         if user_id is None:
             raise Exception("user_id cannot be None")
@@ -73,14 +74,15 @@
         self._status = status
         self._start_time = start_time
         self._end_time = end_time
         self._lifecycle_stage = lifecycle_stage
         self._artifact_uri = artifact_uri
         self._name = name
         self._fqn = fqn
+        self._description = description
 
     def __eq__(self, other):
         if type(other) is type(self):
             # TODO deep equality here?
             return self.__dict__ == other.__dict__
         return False
 
@@ -146,14 +148,18 @@
     def name(self):
         return self._name
 
     @searchable_attribute
     def fqn(self):
         return self._fqn
 
+    @property
+    def description(self):
+        return self._description
+
     def to_proto(self):
         proto = ProtoRunInfo()
         proto.run_uuid = self.run_uuid
         proto.run_id = self.run_id
         proto.experiment_id = self.experiment_id
         proto.user_id = self.user_id
         proto.status = RunStatus.from_string(self.status)
@@ -161,14 +167,15 @@
         if self.end_time:
             proto.end_time = self.end_time
         if self.artifact_uri:
             proto.artifact_uri = self.artifact_uri
         proto.lifecycle_stage = self.lifecycle_stage
         proto.name = self.name or ""
         proto.fqn = self.fqn
+        proto.description = self.description or ""
         return proto
 
     @classmethod
     def from_proto(cls, proto):
         end_time = proto.end_time
         # The proto2 default scalar value of zero indicates that the run's end time is absent.
         # An absent end time is represented with a NoneType in the `RunInfo` class
@@ -182,14 +189,15 @@
             status=RunStatus.to_string(proto.status),
             start_time=proto.start_time,
             end_time=end_time,
             lifecycle_stage=proto.lifecycle_stage,
             artifact_uri=proto.artifact_uri,
             name=proto.name,
             fqn=proto.fqn,
+            description=proto.description,
         )
 
     @classmethod
     def get_searchable_attributes(cls):
         return sorted(
             [p for p in cls.__dict__ if isinstance(getattr(cls, p), searchable_attribute)]
         )
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run_log.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run_log.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run_status.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/run_tag.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/source_type.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/entities/view_type.py` & `tfy-mlflow-client-0.0.9/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/exceptions.py` & `tfy-mlflow-client-0.0.9/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/experiments.py` & `tfy-mlflow-client-0.0.9/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/fastai/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/fastai/callback.py` & `tfy-mlflow-client-0.0.9/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/gluon/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/gluon/_autolog.py` & `tfy-mlflow-client-0.0.9/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/h2o.py` & `tfy-mlflow-client-0.0.9/mlflow/h2o.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/keras.py` & `tfy-mlflow-client-0.0.9/mlflow/keras.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/lightgbm.py` & `tfy-mlflow-client-0.0.9/mlflow/lightgbm.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/ml-package-versions.yml` & `tfy-mlflow-client-0.0.9/mlflow/ml-package-versions.yml`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/mleap.py` & `tfy-mlflow-client-0.0.9/mlflow/mleap.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/container/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/docker_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/evaluation/artifacts.py` & `tfy-mlflow-client-0.0.9/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/evaluation/base.py` & `tfy-mlflow-client-0.0.9/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/evaluation/default_evaluator.py` & `tfy-mlflow-client-0.0.9/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/evaluation/evaluator_registry.py` & `tfy-mlflow-client-0.0.9/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/evaluation/lift_curve.py` & `tfy-mlflow-client-0.0.9/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/flavor_backend.py` & `tfy-mlflow-client-0.0.9/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/flavor_backend_registry.py` & `tfy-mlflow-client-0.0.9/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/model.py` & `tfy-mlflow-client-0.0.9/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/signature.py` & `tfy-mlflow-client-0.0.9/mlflow/models/signature.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/models/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/onnx.py` & `tfy-mlflow-client-0.0.9/mlflow/onnx.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/paddle/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/paddle/_paddle_autolog.py` & `tfy-mlflow-client-0.0.9/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/_project_spec.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/backend/abstract_backend.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/backend/loader.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/backend/local.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/databricks.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/docker.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/kubernetes.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/submitted_run.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/projects/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/prophet.py` & `tfy-mlflow-client-0.0.9/mlflow/prophet.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/backend.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/mlserver.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/model.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/scoring_server/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/spark_model_cache.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyfunc/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/pyfunc/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pypi_package_index.json` & `tfy-mlflow-client-0.0.9/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyspark/ml/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pyspark/ml/log_model_allowlist.txt` & `tfy-mlflow-client-0.0.9/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pytorch/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pytorch/_pytorch_autolog.py` & `tfy-mlflow-client-0.0.9/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/pytorch/pickle_module.py` & `tfy-mlflow-client-0.0.9/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/rfunc/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/rfunc/backend.py` & `tfy-mlflow-client-0.0.9/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/runs.py` & `tfy-mlflow-client-0.0.9/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/sagemaker/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/sagemaker/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/shap.py` & `tfy-mlflow-client-0.0.9/mlflow/shap.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/sklearn/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/sklearn/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/spacy.py` & `tfy-mlflow-client-0.0.9/mlflow/spacy.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/spark.py` & `tfy-mlflow-client-0.0.9/mlflow/spark.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/statsmodels.py` & `tfy-mlflow-client-0.0.9/mlflow/statsmodels.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/artifact_repository_registry.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/azure_blob_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/cli.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/databricks_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/databricks_models_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/dbfs_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/ftp_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/gcs_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/hdfs_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/http_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/http_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/local_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/mlflow_artifacts_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/models_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/runs_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/s3_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/sftp_artifact_repo.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/artifact/utils/models.py` & `tfy-mlflow-client-0.0.9/mlflow/store/artifact/utils/models.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/db/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/model_registry/abstract_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/model_registry/dbmodels/models.py` & `tfy-mlflow-client-0.0.9/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/model_registry/rest_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/model_registry/sqlalchemy_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/tracking/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/tracking/abstract_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/tracking/abstract_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         :return: A :py:class:`PagedList <mlflow.store.entities.PagedList>` of
                  :py:class:`Experiment <mlflow.entities.Experiment>` objects. The pagination token
                  for the next page can be obtained via the ``token`` attribute of the object.
         """
         pass
 
     @abstractmethod
-    def create_experiment(self, name, artifact_location, tags):
+    def create_experiment(self, name, artifact_location, tags, description):
         """
         Create a new experiment.
         If an experiment with the given name already exists, throws exception.
 
         :param name: Desired name for an experiment
         :param artifact_location: Base location for artifacts in runs. May be None.
         :param tags: Experiment tags to set upon experiment creation
@@ -127,24 +127,24 @@
 
         :return: A single :py:class:`mlflow.entities.Run` object, if the run exists. Otherwise,
                  raises an exception.
         """
         pass
 
     @abstractmethod
-    def update_run_info(self, run_id, run_status, end_time):
+    def update_run_info(self, run_id, run_status, end_time, description):
         """
         Update the metadata of the specified run.
 
         :return: :py:class:`mlflow.entities.RunInfo` describing the updated run.
         """
         pass
 
     @abstractmethod
-    def create_run(self, experiment_id, user_id, start_time, tags, name):
+    def create_run(self, experiment_id, user_id, start_time, tags, name, description):
         """
         Create a run under the specified experiment ID, setting the run's status to "RUNNING"
         and the start time to the current time.
 
         :param experiment_id: String id of the experiment for this run
         :param user_id: ID of the user launching this run
 
@@ -346,7 +346,10 @@
     def list_run_logs(
         self, run_uuid: str, key: typing.Optional[str], log_type: typing.Optional[str]
     ) -> typing.List[RunLog]:
         raise NotImplementedError()
 
     def get_run_by_fqn(self, fqn: str) -> Run:
         raise NotImplementedError()
+
+    def update_experiment(self, experiment_id: str, description: typing.Optional[str]):
+        raise NotImplementedError()
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/tracking/file_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/store/tracking/rest_store.py` & `tfy-mlflow-client-0.0.9/mlflow/store/tracking/rest_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-from mlflow.entities import Experiment, Metric, Run, RunInfo, RunLog, ViewType
+from mlflow.entities import SENTINEL, Experiment, Metric, Run, RunInfo, RunLog, ViewType
 from mlflow.exceptions import MlflowException
 from mlflow.protos import databricks_pb2
 from mlflow.protos.service_pb2 import (
     CreateExperiment,
     CreateRun,
     DeleteExperiment,
     DeleteRun,
@@ -37,14 +37,15 @@
 from mlflow.utils.proto_json_utils import message_to_json
 from mlflow.utils.rest_utils import (
     _REST_API_PATH_PREFIX,
     call_endpoint,
     extract_api_info_for_service,
 )
 
+SENTINEL = object()
 _METHOD_TO_INFO = extract_api_info_for_service(MlflowService, _REST_API_PATH_PREFIX)
 
 
 class RestStore(AbstractStore):
     """
     Client for a remote tracking server accessed via REST API calls
 
@@ -89,26 +90,31 @@
         # If the response doesn't contain `next_page_token`, `response_proto.next_page_token`
         # returns an empty string (default value for a string proto field).
         token = (
             response_proto.next_page_token if response_proto.HasField("next_page_token") else None
         )
         return PagedList(experiments, token)
 
-    def create_experiment(self, name, artifact_location=None, tags=None):
+    def create_experiment(self, name, artifact_location=None, tags=None, description=None):
         """
         Create a new experiment.
         If an experiment with the given name already exists, throws exception.
 
         :param name: Desired name for an experiment
 
         :return: experiment_id (string) for the newly created experiment if successful, else None
         """
         tag_protos = [tag.to_proto() for tag in tags] if tags else []
         req_body = message_to_json(
-            CreateExperiment(name=name, artifact_location=artifact_location, tags=tag_protos)
+            CreateExperiment(
+                name=name,
+                artifact_location=artifact_location,
+                tags=tag_protos,
+                description=description,
+            )
         )
         response_proto = self._call_endpoint(CreateExperiment, req_body)
         return response_proto.experiment_id
 
     def get_experiment(self, experiment_id):
         """
         Fetch the experiment from the backend store.
@@ -132,35 +138,46 @@
 
     def rename_experiment(self, experiment_id, new_name):
         req_body = message_to_json(
             UpdateExperiment(experiment_id=str(experiment_id), new_name=new_name)
         )
         self._call_endpoint(UpdateExperiment, req_body)
 
+    def update_experiment(self, experiment_id, description):
+        req_body = message_to_json(
+            UpdateExperiment(experiment_id=str(experiment_id), description=description)
+        )
+        self._call_endpoint(UpdateExperiment, req_body)
+
     def get_run(self, run_id):
         """
         Fetch the run from backend store
 
         :param run_id: Unique identifier for the run
 
         :return: A single Run object if it exists, otherwise raises an Exception
         """
         req_body = message_to_json(GetRun(run_uuid=run_id, run_id=run_id))
         response_proto = self._call_endpoint(GetRun, req_body)
         return Run.from_proto(response_proto.run)
 
-    def update_run_info(self, run_id, run_status, end_time):
+    def update_run_info(self, run_id, run_status=None, end_time=None, description=SENTINEL):
         """Updates the metadata of the specified run."""
-        req_body = message_to_json(
-            UpdateRun(run_uuid=run_id, run_id=run_id, status=run_status, end_time=end_time)
-        )
+        updated_run_info = {}
+        if run_status is not None:
+            updated_run_info["status"] = run_status
+        if end_time is not None:
+            updated_run_info["end_time"] = end_time
+        if description is not SENTINEL:
+            updated_run_info["description"] = description or ""
+        req_body = message_to_json(UpdateRun(run_uuid=run_id, run_id=run_id, **updated_run_info))
         response_proto = self._call_endpoint(UpdateRun, req_body)
         return RunInfo.from_proto(response_proto.run_info)
 
-    def create_run(self, experiment_id, user_id, start_time, tags, name):
+    def create_run(self, experiment_id, user_id, start_time, tags, name, description):
         """
         Create a run under the specified experiment ID, setting the run's status to "RUNNING"
         and the start time to the current time.
 
         :param experiment_id: ID of the experiment for this run
         :param user_id: ID of the user launching this run
         :param start_time: timestamp of the initialization of the run
@@ -172,14 +189,15 @@
         req_body = message_to_json(
             CreateRun(
                 experiment_id=str(experiment_id),
                 user_id=user_id,
                 start_time=start_time,
                 tags=tag_protos,
                 name=name,
+                description=description or "",
             )
         )
         response_proto = self._call_endpoint(CreateRun, req_body)
         run = Run.from_proto(response_proto.run)
         return run
 
     def log_metric(self, run_id, metric):
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tensorflow/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tensorflow/_autolog.py` & `tfy-mlflow-client-0.0.9/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/client.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/fluent.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/registry.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_model_registry/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/client.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         :param run_id: Unique identifier for run
         :param key: Metric name within the run
 
         :return: A list of :py:class:`mlflow.entities.Metric` entities if logged, else empty list
         """
         return self.store.get_metric_history(run_id=run_id, metric_key=key)
 
-    def create_run(self, experiment_id, start_time=None, tags=None, name=""):
+    def create_run(self, experiment_id, start_time=None, tags=None, name="", description=None):
         """
         Create a :py:class:`mlflow.entities.Run` object that can be associated with
         metrics, parameters, artifacts, etc.
         Unlike :py:func:`mlflow.projects.run`, creates objects but does not run code.
         Unlike :py:func:`mlflow.start_run`, does not change the "active run" used by
         :py:func:`mlflow.log_param`.
 
@@ -113,14 +113,15 @@
 
         return self.store.create_run(
             experiment_id=experiment_id,
             user_id=user_id,
             start_time=start_time or int(time.time() * 1000),
             tags=[RunTag(key, value) for (key, value) in tags.items()],
             name=name,
+            description=description,
         )
 
     def list_run_infos(
         self,
         experiment_id,
         run_view_type=ViewType.ACTIVE_ONLY,
         max_results=SEARCH_MAX_RESULTS_DEFAULT,
@@ -173,15 +174,15 @@
     def get_experiment_by_name(self, name, owner_subject_id: typing.Optional[str] = None):
         """
         :param name: The experiment name.
         :return: :py:class:`mlflow.entities.Experiment`
         """
         return self.store.get_experiment_by_name(name, owner_subject_id=owner_subject_id)
 
-    def create_experiment(self, name, artifact_location=None, tags=None):
+    def create_experiment(self, name, artifact_location=None, tags=None, description=None):
         """Create an experiment.
 
         :param name: The experiment name. Must be unique.
         :param artifact_location: The location to store run artifacts.
                                   If not provided, the server picks an appropriate default.
         :param tags: A dictionary of key-value pairs that are converted into
                                   :py:class:`mlflow.entities.ExperimentTag` objects.
@@ -190,14 +191,15 @@
         _validate_experiment_name(name)
         _validate_experiment_artifact_location(artifact_location)
 
         return self.store.create_experiment(
             name=name,
             artifact_location=artifact_location,
             tags=[ExperimentTag(key, value) for (key, value) in tags.items()] if tags else [],
+            description=description,
         )
 
     def delete_experiment(self, experiment_id):
         """
         Delete an experiment from the backend store.
 
         :param experiment_id: The experiment ID returned from ``create_experiment``.
@@ -216,14 +218,17 @@
         """
         Update an experiment's name. The new name must be unique.
 
         :param experiment_id: The experiment ID returned from ``create_experiment``.
         """
         self.store.rename_experiment(experiment_id, new_name)
 
+    def update_experiment(self, experiment_id, description):
+        self.store.update_experiment(experiment_id, description)
+
     def log_metric(self, run_id, key, value, timestamp=None, step=None):
         """
         Log a metric against the run ID.
 
         :param run_id: The run id to which the metric should be logged.
         :param key: Metric name (string). This string may only contain alphanumerics,
                     underscores (_), dashes (-), periods (.), spaces ( ), and slashes (/).
@@ -406,17 +411,22 @@
 
         :param status: A string value of :py:class:`mlflow.entities.RunStatus`.
                        Defaults to "FINISHED".
         :param end_time: If not provided, defaults to the current time."""
         end_time = end_time if end_time else int(time.time() * 1000)
         status = status if status else RunStatus.to_string(RunStatus.FINISHED)
         self.store.update_run_info(
-            run_id, run_status=RunStatus.from_string(status), end_time=end_time
+            run_id,
+            run_status=RunStatus.from_string(status),
+            end_time=end_time,
         )
 
+    def update_run(self, run_id: str, description: str):
+        self.store.update_run_info(run_id, description=description)
+
     def delete_run(self, run_id):
         """
         Deletes a run with the given ID.
         """
         self.store.delete_run(run_id)
 
     def restore_run(self, run_id):
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/registry.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/_tracking_service/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/artifact_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/client.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,14 +229,15 @@
 
     def create_run(
         self,
         experiment_id: str,
         start_time: Optional[int] = None,
         tags: Optional[Dict[str, Any]] = None,
         name: str = "",
+        description: Optional[str] = None,
     ) -> Run:
         """
         Create a :py:class:`mlflow.entities.Run` object that can be associated with
         metrics, parameters, artifacts, etc.
         Unlike :py:func:`mlflow.projects.run`, creates objects but does not run code.
         Unlike :py:func:`mlflow.start_run`, does not change the "active run" used by
         :py:func:`mlflow.log_param`.
@@ -270,15 +271,17 @@
 
             Run tags: {'engineering': 'ML Platform'}
             Experiment id: 0
             Run id: 65fb9e2198764354bab398105f2e70c1
             lifecycle_stage: active
             status: RUNNING
         """
-        return self._tracking_client.create_run(experiment_id, start_time, tags, name=name)
+        return self._tracking_client.create_run(
+            experiment_id, start_time, tags, name=name, description=description
+        )
 
     def list_run_infos(
         self,
         experiment_id: str,
         run_view_type: int = ViewType.ACTIVE_ONLY,
         max_results: int = SEARCH_MAX_RESULTS_DEFAULT,
         order_by: Optional[List[str]] = None,
@@ -477,14 +480,15 @@
         return self._tracking_client.get_experiment_by_name(name, owner_subject_id=owner_subject_id)
 
     def create_experiment(
         self,
         name: str,
         artifact_location: Optional[str] = None,
         tags: Optional[Dict[str, Any]] = None,
+        description: Optional[str] = None,
     ) -> str:
         """Create an experiment.
 
         :param name: The experiment name. Must be unique.
         :param artifact_location: The location to store run artifacts.
                                   If not provided, the server picks an appropriate default.
         :param tags: A dictionary of key-value pairs that are converted into
@@ -515,15 +519,17 @@
 
             Name: Social NLP Experiments
             Experiment_id: 1
             Artifact Location: file:///.../mlruns/1
             Tags: {'nlp.framework': 'Spark NLP'}
             Lifecycle_stage: active
         """
-        return self._tracking_client.create_experiment(name, artifact_location, tags)
+        return self._tracking_client.create_experiment(
+            name, artifact_location, tags, description=description
+        )
 
     def delete_experiment(self, experiment_id: str) -> None:
         """
         Delete an experiment from the backend store.
 
         :param experiment_id: The experiment ID returned from ``create_experiment``.
 
@@ -635,14 +641,17 @@
             --
             Name: Social Media NLP Experiments
             Experiment_id: 1
             Lifecycle_stage: active
         """
         self._tracking_client.rename_experiment(experiment_id, new_name)
 
+    def update_experiment(self, experiment_id: str, description) -> None:
+        self._tracking_client.update_experiment(experiment_id, description)
+
     def log_metric(
         self,
         run_id: str,
         key: str,
         value: float,
         timestamp: Optional[int] = None,
         step: Optional[int] = None,
@@ -1468,14 +1477,17 @@
             status: RUNNING
             --
             run_id: 575fb62af83f469e84806aee24945973
             status: KILLED
         """
         self._tracking_client.set_terminated(run_id, status, end_time)
 
+    def update_run(self, run_id: str, description: str):
+        self._tracking_client.update_run(run_id, description)
+
     def delete_run(self, run_id: str) -> None:
         """Deletes a run with the given ID.
 
         :param run_id: The unique run id to delete.
 
         .. code-block:: python
             :caption: Example
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/abstract_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_cluster_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_command_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_job_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/databricks_notebook_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/default_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/git_context.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/context/registry.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/fluent.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/registry.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/abstract_request_header_provider.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/databricks_request_header_provider.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/tracking/request_header/registry.py` & `tfy-mlflow-client-0.0.9/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/types/schema.py` & `tfy-mlflow-client-0.0.9/mlflow/types/schema.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/types/utils.py` & `tfy-mlflow-client-0.0.9/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/_capture_modules.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/annotations.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/client.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/events.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/logging_and_warnings.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/safety.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/autologging_utils/versioning.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/cli_args.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/conda.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/databricks_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/docstring_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/environment.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/environment.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/file_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/gorilla.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/import_hooks/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/logging_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/mlflow_tags.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/model_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/process.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/proto_json_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/requirements_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/requirements_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/rest_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/s3_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/search_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/string_utils.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/uri.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/utils/validation.py` & `tfy-mlflow-client-0.0.9/mlflow/utils/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 MAX_MODEL_REGISTRY_TAG_KEY_LENGTH = 250
 MAX_MODEL_REGISTRY_TAG_VALUE_LENGTH = 5000
 MAX_EXPERIMENTS_LISTED_PER_PAGE = 50000
 MAX_USER_EMAIL_LENGTH = 64
 MAX_TEAM_NAME_LENGTH = 64
 MAX_RUN_LOG_KEY_NAME_LENGTH = 128
 MAX_RUN_LOG_LOG_TYPE_LENGTH = 128
+MAX_EXPERIMENT_DESCRIPTION_LENGTH = 512
+MAX_RUN_DESCRIPTION_LENGTH = 512
 
 _UNSUPPORTED_DB_TYPE_MSG = "Supported database engines are {%s}" % ", ".join(DATABASE_ENGINES)
 
 PARAM_VALIDATION_MSG = """
 
 The cause of this error is typically due to repeated calls
 to an individual run_id event logging.
@@ -423,7 +425,15 @@
 
 
 def _validate_team_name(team_name):
     """ "Validates the string if it is a valid team_id"""
     _validate_length_limit("Team Name", MAX_TEAM_NAME_LENGTH, team_name)
     if team_name is None or team_name == "":
         raise MlflowException(f"Invalid Team Name: {team_name}", INVALID_PARAMETER_VALUE)
+
+
+def _validate_experiment_description(description):
+    _validate_length_limit("Experiment Description", MAX_EXPERIMENT_DESCRIPTION_LENGTH, description)
+
+
+def _validate_run_description(description):
+    _validate_length_limit("Run Description", MAX_RUN_DESCRIPTION_LENGTH, description)
```

### Comparing `tfy-mlflow-client-0.0.8/mlflow/xgboost/__init__.py` & `tfy-mlflow-client-0.0.9/mlflow/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/mlflow/xgboost/_autolog.py` & `tfy-mlflow-client-0.0.9/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/pylint_plugins/pytest_raises_without_match/__init__.py` & `tfy-mlflow-client-0.0.9/pylint_plugins/pytest_raises_without_match/__init__.py`

 * *Files identical despite different names*

### Comparing `tfy-mlflow-client-0.0.8/setup.py` & `tfy-mlflow-client-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 SKINNY_REQUIREMENTS = [
     "click>=7.0",
     "cloudpickle",
     "databricks-cli>=0.8.7",
     "entrypoints",
     "gitpython>=2.1.0",
     "pyyaml>=5.1",
-    "protobuf>=3.7.0",
+    "protobuf >=3.12, <5.0",
     "pytz",
     "requests>=2.17.3",
     "packaging",
     # Automated dependency detection in MLflow Models relies on
     # `importlib_metadata.packages_distributions` to resolve a module name to its package name
     # (e.g. 'sklearn' -> 'scikit-learn'). importlib_metadata 3.7.0 or newer supports this function:
     # https://github.com/python/importlib_metadata/blob/main/CHANGES.rst#v370
```

### Comparing `tfy-mlflow-client-0.0.8/tfy_mlflow_client.egg-info/SOURCES.txt` & `tfy-mlflow-client-0.0.9/tfy_mlflow_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 mlflow/entities/param.py
 mlflow/entities/run.py
 mlflow/entities/run_data.py
 mlflow/entities/run_info.py
 mlflow/entities/run_log.py
 mlflow/entities/run_status.py
 mlflow/entities/run_tag.py
+mlflow/entities/sentinel.py
 mlflow/entities/source_type.py
 mlflow/entities/user_info.py
 mlflow/entities/view_type.py
 mlflow/entities/model_registry/__init__.py
 mlflow/entities/model_registry/_model_registry_entity.py
 mlflow/entities/model_registry/model_version.py
 mlflow/entities/model_registry/model_version_stages.py
```


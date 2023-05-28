# Comparing `tmp/kserve-0.9.0.tar.gz` & `tmp/kserve-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kserve-0.9.0.tar", last modified: Sat Jul 23 00:57:13 2022, max compression
+gzip compressed data, was "kserve-0.9.0rc0.tar", last modified: Mon Jun 13 03:09:51 2022, max compression
```

## Comparing `kserve-0.9.0.tar` & `kserve-0.9.0rc0.tar`

### file list

```diff
@@ -1,198 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.630647 kserve-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-23 00:57:00.000000 kserve-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-07-23 00:57:13.630647 kserve-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5779 2022-07-23 00:57:00.000000 kserve-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.590646 kserve-0.9.0/kserve/
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.590646 kserve-0.9.0/kserve/api/
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/api/creds_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22101 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/api/kserve_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/api/watch.py
--rw-r--r--   0 runner    (1001) docker     (121)    26693 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12927 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.590646 kserve-0.9.0/kserve/constants/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.594647 kserve-0.9.0/kserve/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/explain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/health.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/model_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/handlers/predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     9634 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/model_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.610647 kserve-0.9.0/kserve/models/
--rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/knative_addressable.py
--rw-r--r--   0 runner    (1001) docker     (121)     8460 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/knative_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/knative_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    10908 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/knative_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     3968 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/knative_volatile_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/net_url_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     8692 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_built_in_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_cluster_serving_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7655 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_cluster_serving_runtime_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    10281 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     7971 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_graph_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     4369 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_graph_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7424 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_graph_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     9236 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     5870 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_inference_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_serving_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_serving_runtime_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     8680 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_serving_runtime_pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    18786 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_serving_runtime_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_storage_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     6123 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_supported_model_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     7911 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_trained_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7448 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_trained_model_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1alpha1_trained_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    35034 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_aix_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    35598 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_alibi_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    35034 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_art_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_batcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    12945 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_component_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    11890 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_component_status_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    52263 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_custom_explainer.py
--rw-r--r--   0 runner    (1001) docker     (121)    52263 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_custom_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)    52551 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_custom_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_deploy_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5342 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_explainer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    34659 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_explainer_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    63095 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5224 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_explainers_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7216 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_failure_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     8001 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_inference_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     7517 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_inference_service_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5795 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_inference_service_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    10058 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_inference_service_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_inference_services_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9840 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_ingress_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    33911 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_light_gbm_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_logger_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_model_copies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_model_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_model_revision_states.py
--rw-r--r--   0 runner    (1001) docker     (121)    35391 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_model_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    34235 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_onnx_runtime_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    34343 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_paddle_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    33479 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_pmml_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    50851 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    10007 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_predictor_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    34991 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_predictor_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_predictor_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    68149 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_predictor_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     9790 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_predictors_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    33803 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_sk_learn_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     6538 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_storage_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    34019 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_tf_serving_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    34127 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_torch_serve_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_transformer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    61462 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_transformer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_transformers_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    33695 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_triton_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    33803 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/models/v1beta1_xg_boost_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)    12804 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/rest.py
--rw-r--r--   0 runner    (1001) docker     (121)    23966 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.614647 kserve-0.9.0/kserve/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/utils/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3759 2022-07-23 00:57:00.000000 kserve-0.9.0/kserve/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.590646 kserve-0.9.0/kserve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6880 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-23 00:57:13.000000 kserve-0.9.0/kserve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-07-23 00:57:00.000000 kserve-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-07-23 00:57:13.630647 kserve-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-07-23 00:57:00.000000 kserve-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-23 00:57:13.630647 kserve-0.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_creds_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3811 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_inference_service_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_knative_addressable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_knative_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_knative_url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_knative_volatile_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_net_url_userinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_s3_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)    22107 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     8562 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_built_in_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4254 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_cluster_serving_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7726 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_cluster_serving_runtime_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_graph_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_graph_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_graph_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_step.py
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_inference_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_serving_runtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7617 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_serving_runtime_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_serving_runtime_pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_serving_runtime_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_storage_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_supported_model_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_trained_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_trained_model_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1alpha1_trained_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_aix_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_alibi_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_art_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_batcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_component_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_component_status_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_custom_explainer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_custom_predictor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_custom_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_deploy_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_explainer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_explainer_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     7426 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_explainer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_explainers_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_failure_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    17464 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_inference_service.py
--rw-r--r--   0 runner    (1001) docker     (121)    38493 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_inference_service_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    27538 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_inference_service_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_inference_service_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_inference_services_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_ingress_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_light_gbm_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_logger_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_model_copies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_model_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_model_revision_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_model_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_onnx_runtime_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_paddle_server_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_pmml_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_predictor_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_predictor_extension_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_predictor_protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)    12845 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_predictor_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_predictors_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_sk_learn_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_storage_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_tf_serving_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_torch_serve_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_transformer_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_transformer_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_transformers_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3092 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_triton_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-07-23 00:57:00.000000 kserve-0.9.0/test/test_v1beta1_xg_boost_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.884838 kserve-0.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-06-13 03:09:51.884838 kserve-0.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5329 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.872838 kserve-0.9.0rc0/kserve/
+-rw-r--r--   0 runner    (1001) docker     (121)     5963 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.872838 kserve-0.9.0rc0/kserve/api/
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/api/creds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17217 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/api/kserve_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/api/watch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26693 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12927 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.872838 kserve-0.9.0rc0/kserve/constants/
+-rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.872838 kserve-0.9.0rc0/kserve/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/explain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/health.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/handlers/predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9622 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6748 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/model_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.880838 kserve-0.9.0rc0/kserve/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     5295 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/knative_addressable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8460 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/knative_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5094 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/knative_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10908 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/knative_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3968 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/knative_volatile_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5287 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/net_url_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8692 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_built_in_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8249 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_cluster_serving_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7655 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_cluster_serving_runtime_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10281 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_container.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6233 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7494 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8680 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18786 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_storage_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6123 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_supported_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7911 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7448 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35034 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_aix_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35598 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_alibi_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35034 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_art_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12533 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_component_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11890 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_component_status_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52263 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_custom_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52263 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_custom_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52551 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_custom_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_deploy_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5342 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_explainer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34659 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_explainer_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62683 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5224 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_explainers_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7216 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_failure_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8001 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_inference_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7517 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5795 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10058 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6253 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_inference_services_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9112 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_ingress_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33911 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_light_gbm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4918 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_logger_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_model_copies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_model_revision_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35391 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_model_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34235 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_onnx_runtime_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34343 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_paddle_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33479 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_pmml_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50851 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10007 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_predictor_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34991 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_predictor_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_predictor_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67737 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_predictor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9790 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_predictors_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33803 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_sk_learn_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6538 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_storage_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34019 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_tf_serving_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34127 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_torch_serve_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_transformer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61050 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_transformer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_transformers_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33695 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_triton_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33803 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/models/v1beta1_xg_boost_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12804 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23966 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.880838 kserve-0.9.0rc0/kserve/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/utils/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/kserve/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.872838 kserve-0.9.0rc0/kserve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6250 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-13 03:09:51.000000 kserve-0.9.0rc0/kserve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-13 03:09:51.884838 kserve-0.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 03:09:51.884838 kserve-0.9.0rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    12183 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_creds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3811 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_inference_service_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_knative_addressable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_knative_condition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_knative_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_knative_volatile_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_net_url_userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5474 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_s3_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21337 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8562 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_built_in_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4254 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_cluster_serving_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7726 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_cluster_serving_runtime_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_container.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7617 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_storage_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_supported_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_trained_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_trained_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1alpha1_trained_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_aix_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3315 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_alibi_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_art_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_component_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_component_status_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_custom_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_custom_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3904 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_custom_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_deploy_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_explainer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_explainer_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7426 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_explainer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_explainers_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_failure_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17464 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_inference_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38493 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_inference_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27538 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_inference_service_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_inference_service_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7328 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_inference_services_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_ingress_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_light_gbm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_logger_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_model_copies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_model_revision_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_onnx_runtime_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_paddle_server_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_pmml_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_predictor_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_predictor_extension_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_predictor_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12845 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_predictor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_predictors_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_sk_learn_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_storage_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_tf_serving_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_torch_serve_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_transformer_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_transformer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_transformers_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3092 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_triton_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-06-13 03:09:41.000000 kserve-0.9.0rc0/test/test_v1beta1_xg_boost_spec.py
```

### Comparing `kserve-0.9.0/PKG-INFO` & `kserve-0.9.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kserve
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: KServe Python SDK
 Home-page: https://github.com/kserve/kserve/tree/master/python/kserve
 Author: The KServe Authors
 Author-email: ellisbigelow@google.com, hejinchi@cn.ibm.com, dsun20@bloomberg.net
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `kserve-0.9.0/README.md` & `kserve-0.9.0rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -67,21 +67,14 @@
 ## Documentation For Models
 
  - [KnativeAddressable](docs/KnativeAddressable.md)
  - [KnativeCondition](docs/KnativeCondition.md)
  - [KnativeURL](docs/KnativeURL.md)
  - [KnativeVolatileTime](docs/KnativeVolatileTime.md)
  - [NetUrlUserinfo](docs/NetUrlUserinfo.md)
- - [V1alpha1InferenceGraph](docs/V1alpha1InferenceGraph.md)
- - [V1alpha1InferenceGraphList](docs/V1alpha1InferenceGraphList.md)
- - [V1alpha1InferenceGraphSpec](docs/V1alpha1InferenceGraphSpec.md)
- - [V1alpha1InferenceGraphStatus](docs/V1alpha1InferenceGraphStatus.md)
- - [V1alpha1InferenceRouter](docs/V1alpha1InferenceRouter.md)
- - [V1alpha1InferenceStep](docs/V1alpha1InferenceStep.md)
- - [V1alpha1InferenceTarget](docs/V1alpha1InferenceTarget.md)
  - [V1beta1AIXExplainerSpec](docs/V1beta1AIXExplainerSpec.md)
  - [V1beta1AlibiExplainerSpec](docs/V1beta1AlibiExplainerSpec.md)
  - [V1beta1Batcher](docs/V1beta1Batcher.md)
  - [V1beta1ComponentExtensionSpec](docs/V1beta1ComponentExtensionSpec.md)
  - [V1beta1ComponentStatusSpec](docs/V1beta1ComponentStatusSpec.md)
  - [V1beta1CustomExplainer](docs/V1beta1CustomExplainer.md)
  - [V1beta1CustomPredictor](docs/V1beta1CustomPredictor.md)
```

### Comparing `kserve-0.9.0/kserve/__init__.py` & `kserve-0.9.0rc0/kserve/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,21 +35,14 @@
 from kserve.exceptions import ApiException
 
 # import v1alpha1 models into kserve packages
 from kserve.models.v1alpha1_built_in_adapter import V1alpha1BuiltInAdapter
 from kserve.models.v1alpha1_cluster_serving_runtime import V1alpha1ClusterServingRuntime
 from kserve.models.v1alpha1_cluster_serving_runtime_list import V1alpha1ClusterServingRuntimeList
 from kserve.models.v1alpha1_container import V1alpha1Container
-from kserve.models.v1alpha1_inference_graph import V1alpha1InferenceGraph
-from kserve.models.v1alpha1_inference_graph_list import V1alpha1InferenceGraphList
-from kserve.models.v1alpha1_inference_graph_spec import V1alpha1InferenceGraphSpec
-from kserve.models.v1alpha1_inference_graph_status import V1alpha1InferenceGraphStatus
-from kserve.models.v1alpha1_inference_router import V1alpha1InferenceRouter
-from kserve.models.v1alpha1_inference_step import V1alpha1InferenceStep
-from kserve.models.v1alpha1_inference_target import V1alpha1InferenceTarget
 from kserve.models.v1alpha1_model_spec import V1alpha1ModelSpec
 from kserve.models.v1alpha1_serving_runtime import V1alpha1ServingRuntime
 from kserve.models.v1alpha1_serving_runtime_list import V1alpha1ServingRuntimeList
 from kserve.models.v1alpha1_serving_runtime_pod_spec import V1alpha1ServingRuntimePodSpec
 from kserve.models.v1alpha1_serving_runtime_spec import V1alpha1ServingRuntimeSpec
 from kserve.models.v1alpha1_storage_helper import V1alpha1StorageHelper
 from kserve.models.v1alpha1_supported_model_format import V1alpha1SupportedModelFormat
```

### Comparing `kserve-0.9.0/kserve/api/__init__.py` & `kserve-0.9.0rc0/kserve/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/api/creds_utils.py` & `kserve-0.9.0rc0/kserve/api/creds_utils.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/api/watch.py` & `kserve-0.9.0rc0/kserve/api/watch.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/api_client.py` & `kserve-0.9.0rc0/kserve/api_client.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/configuration.py` & `kserve-0.9.0rc0/kserve/configuration.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/constants/__init__.py` & `kserve-0.9.0rc0/kserve/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/constants/constants.py` & `kserve-0.9.0rc0/kserve/constants/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 
 # KServe K8S constants
 KSERVE_GROUP = 'serving.kserve.io'
 KSERVE_KIND = 'InferenceService'
 KSERVE_PLURAL = 'inferenceservices'
 KSERVE_KIND_TRAINEDMODEL = 'TrainedModel'
 KSERVE_PLURAL_TRAINEDMODEL = 'trainedmodels'
-KSERVE_KIND_INFERENCEGRAPH = 'InferenceGraph'
-KSERVE_PLURAL_INFERENCEGRAPH = 'inferencegraphs'
 KSERVE_V1BETA1_VERSION = 'v1beta1'
 KSERVE_V1ALPHA1_VERSION = "v1alpha1"
 
 KSERVE_V1BETA1 = KSERVE_GROUP + '/' + KSERVE_V1BETA1_VERSION
 KSERVE_V1ALPHA1 = KSERVE_GROUP + '/' + KSERVE_V1ALPHA1_VERSION
 
 KSERVE_LOGLEVEL = os.environ.get('KSERVE_LOGLEVEL', 'INFO').upper()
```

### Comparing `kserve-0.9.0/kserve/exceptions.py` & `kserve-0.9.0rc0/kserve/exceptions.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/__init__.py` & `kserve-0.9.0rc0/kserve/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/base.py` & `kserve-0.9.0rc0/kserve/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/explain.py` & `kserve-0.9.0rc0/kserve/handlers/explain.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/health.py` & `kserve-0.9.0rc0/kserve/handlers/health.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/model_management.py` & `kserve-0.9.0rc0/kserve/handlers/model_management.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/handlers/predict.py` & `kserve-0.9.0rc0/kserve/handlers/predict.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/model.py` & `kserve-0.9.0rc0/kserve/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,21 +103,21 @@
             if ":" not in self.predictor_host:
                 self.predictor_host = self.predictor_host + ":80"
             _channel = grpc.aio.insecure_channel(self.predictor_host)
             self._grpc_client_stub = service_pb2_grpc.GRPCInferenceServiceStub(_channel)
         return self._grpc_client_stub
 
     def validate(self, request):
-        if self.protocol == PredictorProtocol.REST_V2.value:
+        if self.protocol == PredictorProtocol.REST_V2:
             if "inputs" in request and not isinstance(request["inputs"], list):
                 raise tornado.web.HTTPError(
                     status_code=HTTPStatus.BAD_REQUEST,
                     reason="Expected \"inputs\" to be a list"
                 )
-        elif isinstance(request, Dict) or self.protocol == PredictorProtocol.REST_V1.value:
+        elif isinstance(request, Dict) or self.protocol == PredictorProtocol.REST_V1:
             if "instances" in request and not isinstance(request["instances"], list):
                 raise tornado.web.HTTPError(
                     status_code=HTTPStatus.BAD_REQUEST,
                     reason="Expected \"instances\" to be a list"
                 )
         return request
```

### Comparing `kserve-0.9.0/kserve/model_repository.py` & `kserve-0.9.0rc0/kserve/model_repository.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/model_server.py` & `kserve-0.9.0rc0/kserve/model_server.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/__init__.py` & `kserve-0.9.0rc0/kserve/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,14 @@
 
 from __future__ import absolute_import
 
 # import models into model package
 from kserve.models.v1alpha1_built_in_adapter import V1alpha1BuiltInAdapter
 from kserve.models.v1alpha1_cluster_serving_runtime import V1alpha1ClusterServingRuntime
 from kserve.models.v1alpha1_cluster_serving_runtime_list import V1alpha1ClusterServingRuntimeList
-from kserve.models.v1alpha1_inference_graph import V1alpha1InferenceGraph
-from kserve.models.v1alpha1_inference_graph_list import V1alpha1InferenceGraphList
-from kserve.models.v1alpha1_inference_graph_spec import V1alpha1InferenceGraphSpec
-from kserve.models.v1alpha1_inference_graph_status import V1alpha1InferenceGraphStatus
-from kserve.models.v1alpha1_inference_router import V1alpha1InferenceRouter
-from kserve.models.v1alpha1_inference_step import V1alpha1InferenceStep
-from kserve.models.v1alpha1_inference_target import V1alpha1InferenceTarget
 from kserve.models.v1alpha1_model_spec import V1alpha1ModelSpec
 from kserve.models.v1alpha1_serving_runtime import V1alpha1ServingRuntime
 from kserve.models.v1alpha1_serving_runtime_list import V1alpha1ServingRuntimeList
 from kserve.models.v1alpha1_serving_runtime_pod_spec import V1alpha1ServingRuntimePodSpec
 from kserve.models.v1alpha1_serving_runtime_spec import V1alpha1ServingRuntimeSpec
 from kserve.models.v1alpha1_storage_helper import V1alpha1StorageHelper
 from kserve.models.v1alpha1_supported_model_format import V1alpha1SupportedModelFormat
```

### Comparing `kserve-0.9.0/kserve/models/knative_addressable.py` & `kserve-0.9.0rc0/kserve/models/knative_addressable.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/knative_condition.py` & `kserve-0.9.0rc0/kserve/models/knative_condition.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/knative_status.py` & `kserve-0.9.0rc0/kserve/models/knative_status.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/knative_url.py` & `kserve-0.9.0rc0/kserve/models/knative_url.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/knative_volatile_time.py` & `kserve-0.9.0rc0/kserve/models/knative_volatile_time.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/net_url_userinfo.py` & `kserve-0.9.0rc0/kserve/models/net_url_userinfo.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1_time.py` & `kserve-0.9.0rc0/kserve/models/v1_time.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_built_in_adapter.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_built_in_adapter.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_cluster_serving_runtime.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_cluster_serving_runtime.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_cluster_serving_runtime_list.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_cluster_serving_runtime_list.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_container.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_container.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_graph.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_inference_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceGraph(object):
+class V1beta1InferenceService(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -46,28 +46,28 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
-        'spec': 'V1alpha1InferenceGraphSpec',
-        'status': 'V1alpha1InferenceGraphStatus'
+        'spec': 'V1beta1InferenceServiceSpec',
+        'status': 'V1beta1InferenceServiceStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
         'status': 'status'
     }
 
     def __init__(self, api_version=None, kind=None, metadata=None, spec=None, status=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceGraph - a model defined in OpenAPI"""  # noqa: E501
+        """V1beta1InferenceService - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._api_version = None
         self._kind = None
         self._metadata = None
@@ -84,117 +84,117 @@
         if spec is not None:
             self.spec = spec
         if status is not None:
             self.status = status
 
     @property
     def api_version(self):
-        """Gets the api_version of this V1alpha1InferenceGraph.  # noqa: E501
+        """Gets the api_version of this V1beta1InferenceService.  # noqa: E501
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :return: The api_version of this V1alpha1InferenceGraph.  # noqa: E501
+        :return: The api_version of this V1beta1InferenceService.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this V1alpha1InferenceGraph.
+        """Sets the api_version of this V1beta1InferenceService.
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :param api_version: The api_version of this V1alpha1InferenceGraph.  # noqa: E501
+        :param api_version: The api_version of this V1beta1InferenceService.  # noqa: E501
         :type: str
         """
 
         self._api_version = api_version
 
     @property
     def kind(self):
-        """Gets the kind of this V1alpha1InferenceGraph.  # noqa: E501
+        """Gets the kind of this V1beta1InferenceService.  # noqa: E501
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :return: The kind of this V1alpha1InferenceGraph.  # noqa: E501
+        :return: The kind of this V1beta1InferenceService.  # noqa: E501
         :rtype: str
         """
         return self._kind
 
     @kind.setter
     def kind(self, kind):
-        """Sets the kind of this V1alpha1InferenceGraph.
+        """Sets the kind of this V1beta1InferenceService.
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :param kind: The kind of this V1alpha1InferenceGraph.  # noqa: E501
+        :param kind: The kind of this V1beta1InferenceService.  # noqa: E501
         :type: str
         """
 
         self._kind = kind
 
     @property
     def metadata(self):
-        """Gets the metadata of this V1alpha1InferenceGraph.  # noqa: E501
+        """Gets the metadata of this V1beta1InferenceService.  # noqa: E501
 
 
-        :return: The metadata of this V1alpha1InferenceGraph.  # noqa: E501
+        :return: The metadata of this V1beta1InferenceService.  # noqa: E501
         :rtype: V1ObjectMeta
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
-        """Sets the metadata of this V1alpha1InferenceGraph.
+        """Sets the metadata of this V1beta1InferenceService.
 
 
-        :param metadata: The metadata of this V1alpha1InferenceGraph.  # noqa: E501
+        :param metadata: The metadata of this V1beta1InferenceService.  # noqa: E501
         :type: V1ObjectMeta
         """
 
         self._metadata = metadata
 
     @property
     def spec(self):
-        """Gets the spec of this V1alpha1InferenceGraph.  # noqa: E501
+        """Gets the spec of this V1beta1InferenceService.  # noqa: E501
 
 
-        :return: The spec of this V1alpha1InferenceGraph.  # noqa: E501
-        :rtype: V1alpha1InferenceGraphSpec
+        :return: The spec of this V1beta1InferenceService.  # noqa: E501
+        :rtype: V1beta1InferenceServiceSpec
         """
         return self._spec
 
     @spec.setter
     def spec(self, spec):
-        """Sets the spec of this V1alpha1InferenceGraph.
+        """Sets the spec of this V1beta1InferenceService.
 
 
-        :param spec: The spec of this V1alpha1InferenceGraph.  # noqa: E501
-        :type: V1alpha1InferenceGraphSpec
+        :param spec: The spec of this V1beta1InferenceService.  # noqa: E501
+        :type: V1beta1InferenceServiceSpec
         """
 
         self._spec = spec
 
     @property
     def status(self):
-        """Gets the status of this V1alpha1InferenceGraph.  # noqa: E501
+        """Gets the status of this V1beta1InferenceService.  # noqa: E501
 
 
-        :return: The status of this V1alpha1InferenceGraph.  # noqa: E501
-        :rtype: V1alpha1InferenceGraphStatus
+        :return: The status of this V1beta1InferenceService.  # noqa: E501
+        :rtype: V1beta1InferenceServiceStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this V1alpha1InferenceGraph.
+        """Sets the status of this V1beta1InferenceService.
 
 
-        :param status: The status of this V1alpha1InferenceGraph.  # noqa: E501
-        :type: V1alpha1InferenceGraphStatus
+        :param status: The status of this V1beta1InferenceService.  # noqa: E501
+        :type: V1beta1InferenceServiceStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -225,18 +225,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceGraph):
+        if not isinstance(other, V1beta1InferenceService):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceGraph):
+        if not isinstance(other, V1beta1InferenceService):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_graph_list.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceGraphList(object):
+class V1alpha1ServingRuntimeList(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -44,28 +44,28 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
-        'items': 'list[V1alpha1InferenceGraph]',
+        'items': 'list[V1alpha1ServingRuntime]',
         'kind': 'str',
         'metadata': 'V1ListMeta'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'items': 'items',
         'kind': 'kind',
         'metadata': 'metadata'
     }
 
     def __init__(self, api_version=None, items=None, kind=None, metadata=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceGraphList - a model defined in OpenAPI"""  # noqa: E501
+        """V1alpha1ServingRuntimeList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._api_version = None
         self._items = None
         self._kind = None
@@ -78,97 +78,97 @@
         if kind is not None:
             self.kind = kind
         if metadata is not None:
             self.metadata = metadata
 
     @property
     def api_version(self):
-        """Gets the api_version of this V1alpha1InferenceGraphList.  # noqa: E501
+        """Gets the api_version of this V1alpha1ServingRuntimeList.  # noqa: E501
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :return: The api_version of this V1alpha1InferenceGraphList.  # noqa: E501
+        :return: The api_version of this V1alpha1ServingRuntimeList.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this V1alpha1InferenceGraphList.
+        """Sets the api_version of this V1alpha1ServingRuntimeList.
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :param api_version: The api_version of this V1alpha1InferenceGraphList.  # noqa: E501
+        :param api_version: The api_version of this V1alpha1ServingRuntimeList.  # noqa: E501
         :type: str
         """
 
         self._api_version = api_version
 
     @property
     def items(self):
-        """Gets the items of this V1alpha1InferenceGraphList.  # noqa: E501
+        """Gets the items of this V1alpha1ServingRuntimeList.  # noqa: E501
 
 
-        :return: The items of this V1alpha1InferenceGraphList.  # noqa: E501
-        :rtype: list[V1alpha1InferenceGraph]
+        :return: The items of this V1alpha1ServingRuntimeList.  # noqa: E501
+        :rtype: list[V1alpha1ServingRuntime]
         """
         return self._items
 
     @items.setter
     def items(self, items):
-        """Sets the items of this V1alpha1InferenceGraphList.
+        """Sets the items of this V1alpha1ServingRuntimeList.
 
 
-        :param items: The items of this V1alpha1InferenceGraphList.  # noqa: E501
-        :type: list[V1alpha1InferenceGraph]
+        :param items: The items of this V1alpha1ServingRuntimeList.  # noqa: E501
+        :type: list[V1alpha1ServingRuntime]
         """
         if self.local_vars_configuration.client_side_validation and items is None:  # noqa: E501
             raise ValueError("Invalid value for `items`, must not be `None`")  # noqa: E501
 
         self._items = items
 
     @property
     def kind(self):
-        """Gets the kind of this V1alpha1InferenceGraphList.  # noqa: E501
+        """Gets the kind of this V1alpha1ServingRuntimeList.  # noqa: E501
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :return: The kind of this V1alpha1InferenceGraphList.  # noqa: E501
+        :return: The kind of this V1alpha1ServingRuntimeList.  # noqa: E501
         :rtype: str
         """
         return self._kind
 
     @kind.setter
     def kind(self, kind):
-        """Sets the kind of this V1alpha1InferenceGraphList.
+        """Sets the kind of this V1alpha1ServingRuntimeList.
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :param kind: The kind of this V1alpha1InferenceGraphList.  # noqa: E501
+        :param kind: The kind of this V1alpha1ServingRuntimeList.  # noqa: E501
         :type: str
         """
 
         self._kind = kind
 
     @property
     def metadata(self):
-        """Gets the metadata of this V1alpha1InferenceGraphList.  # noqa: E501
+        """Gets the metadata of this V1alpha1ServingRuntimeList.  # noqa: E501
 
 
-        :return: The metadata of this V1alpha1InferenceGraphList.  # noqa: E501
+        :return: The metadata of this V1alpha1ServingRuntimeList.  # noqa: E501
         :rtype: V1ListMeta
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
-        """Sets the metadata of this V1alpha1InferenceGraphList.
+        """Sets the metadata of this V1alpha1ServingRuntimeList.
 
 
-        :param metadata: The metadata of this V1alpha1InferenceGraphList.  # noqa: E501
+        :param metadata: The metadata of this V1alpha1ServingRuntimeList.  # noqa: E501
         :type: V1ListMeta
         """
 
         self._metadata = metadata
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -200,18 +200,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceGraphList):
+        if not isinstance(other, V1alpha1ServingRuntimeList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceGraphList):
+        if not isinstance(other, V1alpha1ServingRuntimeList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_graph_spec.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_storage_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,71 +28,68 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceGraphSpec(object):
+class V1alpha1StorageHelper(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'nodes': 'dict(str, V1alpha1InferenceRouter)'
+        'disabled': 'bool'
     }
 
     attribute_map = {
-        'nodes': 'nodes'
+        'disabled': 'disabled'
     }
 
-    def __init__(self, nodes=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceGraphSpec - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, disabled=None, local_vars_configuration=None):  # noqa: E501
+        """V1alpha1StorageHelper - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._nodes = None
+        self._disabled = None
         self.discriminator = None
 
-        self.nodes = nodes
+        if disabled is not None:
+            self.disabled = disabled
 
     @property
-    def nodes(self):
-        """Gets the nodes of this V1alpha1InferenceGraphSpec.  # noqa: E501
+    def disabled(self):
+        """Gets the disabled of this V1alpha1StorageHelper.  # noqa: E501
 
-        Map of InferenceGraph router nodes Each node defines the router which can be different routing types  # noqa: E501
 
-        :return: The nodes of this V1alpha1InferenceGraphSpec.  # noqa: E501
-        :rtype: dict(str, V1alpha1InferenceRouter)
+        :return: The disabled of this V1alpha1StorageHelper.  # noqa: E501
+        :rtype: bool
         """
-        return self._nodes
+        return self._disabled
 
-    @nodes.setter
-    def nodes(self, nodes):
-        """Sets the nodes of this V1alpha1InferenceGraphSpec.
+    @disabled.setter
+    def disabled(self, disabled):
+        """Sets the disabled of this V1alpha1StorageHelper.
 
-        Map of InferenceGraph router nodes Each node defines the router which can be different routing types  # noqa: E501
 
-        :param nodes: The nodes of this V1alpha1InferenceGraphSpec.  # noqa: E501
-        :type: dict(str, V1alpha1InferenceRouter)
+        :param disabled: The disabled of this V1alpha1StorageHelper.  # noqa: E501
+        :type: bool
         """
-        if self.local_vars_configuration.client_side_validation and nodes is None:  # noqa: E501
-            raise ValueError("Invalid value for `nodes`, must not be `None`")  # noqa: E501
 
-        self._nodes = nodes
+        self._disabled = disabled
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -120,18 +117,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceGraphSpec):
+        if not isinstance(other, V1alpha1StorageHelper):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceGraphSpec):
+        if not isinstance(other, V1alpha1StorageHelper):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_router.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,99 +28,98 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceRouter(object):
+class V1alpha1TrainedModelSpec(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'router_type': 'str',
-        'steps': 'list[V1alpha1InferenceStep]'
+        'inference_service': 'str',
+        'model': 'V1alpha1ModelSpec'
     }
 
     attribute_map = {
-        'router_type': 'routerType',
-        'steps': 'steps'
+        'inference_service': 'inferenceService',
+        'model': 'model'
     }
 
-    def __init__(self, router_type='', steps=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceRouter - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, inference_service='', model=None, local_vars_configuration=None):  # noqa: E501
+        """V1alpha1TrainedModelSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._router_type = None
-        self._steps = None
+        self._inference_service = None
+        self._model = None
         self.discriminator = None
 
-        self.router_type = router_type
-        if steps is not None:
-            self.steps = steps
+        self.inference_service = inference_service
+        self.model = model
 
     @property
-    def router_type(self):
-        """Gets the router_type of this V1alpha1InferenceRouter.  # noqa: E501
+    def inference_service(self):
+        """Gets the inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
 
-        RouterType  - `Sequence:` chain multiple inference steps with input/output from previous step  - `Splitter:` randomly routes to the target service according to the weight  - `Ensemble:` routes the request to multiple models and then merge the responses  - `Switch:` routes the request to one of the steps based on condition  # noqa: E501
+        parent inference service to deploy to  # noqa: E501
 
-        :return: The router_type of this V1alpha1InferenceRouter.  # noqa: E501
+        :return: The inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
         :rtype: str
         """
-        return self._router_type
+        return self._inference_service
 
-    @router_type.setter
-    def router_type(self, router_type):
-        """Sets the router_type of this V1alpha1InferenceRouter.
+    @inference_service.setter
+    def inference_service(self, inference_service):
+        """Sets the inference_service of this V1alpha1TrainedModelSpec.
 
-        RouterType  - `Sequence:` chain multiple inference steps with input/output from previous step  - `Splitter:` randomly routes to the target service according to the weight  - `Ensemble:` routes the request to multiple models and then merge the responses  - `Switch:` routes the request to one of the steps based on condition  # noqa: E501
+        parent inference service to deploy to  # noqa: E501
 
-        :param router_type: The router_type of this V1alpha1InferenceRouter.  # noqa: E501
+        :param inference_service: The inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and router_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `router_type`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and inference_service is None:  # noqa: E501
+            raise ValueError("Invalid value for `inference_service`, must not be `None`")  # noqa: E501
 
-        self._router_type = router_type
+        self._inference_service = inference_service
 
     @property
-    def steps(self):
-        """Gets the steps of this V1alpha1InferenceRouter.  # noqa: E501
+    def model(self):
+        """Gets the model of this V1alpha1TrainedModelSpec.  # noqa: E501
 
-        Steps defines destinations for the current router node  # noqa: E501
 
-        :return: The steps of this V1alpha1InferenceRouter.  # noqa: E501
-        :rtype: list[V1alpha1InferenceStep]
+        :return: The model of this V1alpha1TrainedModelSpec.  # noqa: E501
+        :rtype: V1alpha1ModelSpec
         """
-        return self._steps
+        return self._model
 
-    @steps.setter
-    def steps(self, steps):
-        """Sets the steps of this V1alpha1InferenceRouter.
+    @model.setter
+    def model(self, model):
+        """Sets the model of this V1alpha1TrainedModelSpec.
 
-        Steps defines destinations for the current router node  # noqa: E501
 
-        :param steps: The steps of this V1alpha1InferenceRouter.  # noqa: E501
-        :type: list[V1alpha1InferenceStep]
+        :param model: The model of this V1alpha1TrainedModelSpec.  # noqa: E501
+        :type: V1alpha1ModelSpec
         """
+        if self.local_vars_configuration.client_side_validation and model is None:  # noqa: E501
+            raise ValueError("Invalid value for `model`, must not be `None`")  # noqa: E501
 
-        self._steps = steps
+        self._model = model
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -148,18 +147,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceRouter):
+        if not isinstance(other, V1alpha1TrainedModelSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceRouter):
+        if not isinstance(other, V1alpha1TrainedModelSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_step.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_status.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,238 +28,232 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceStep(object):
+class V1beta1InferenceServiceStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'condition': 'str',
-        'data': 'str',
-        'name': 'str',
-        'node_name': 'str',
-        'service_name': 'str',
-        'service_url': 'str',
-        'weight': 'int'
+        'address': 'KnativeAddressable',
+        'annotations': 'dict(str, str)',
+        'components': 'dict(str, V1beta1ComponentStatusSpec)',
+        'conditions': 'list[KnativeCondition]',
+        'model_status': 'V1beta1ModelStatus',
+        'observed_generation': 'int',
+        'url': 'KnativeURL'
     }
 
     attribute_map = {
-        'condition': 'condition',
-        'data': 'data',
-        'name': 'name',
-        'node_name': 'nodeName',
-        'service_name': 'serviceName',
-        'service_url': 'serviceUrl',
-        'weight': 'weight'
+        'address': 'address',
+        'annotations': 'annotations',
+        'components': 'components',
+        'conditions': 'conditions',
+        'model_status': 'modelStatus',
+        'observed_generation': 'observedGeneration',
+        'url': 'url'
     }
 
-    def __init__(self, condition=None, data=None, name=None, node_name=None, service_name=None, service_url=None, weight=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceStep - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, address=None, annotations=None, components=None, conditions=None, model_status=None, observed_generation=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1InferenceServiceStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._condition = None
-        self._data = None
-        self._name = None
-        self._node_name = None
-        self._service_name = None
-        self._service_url = None
-        self._weight = None
+        self._address = None
+        self._annotations = None
+        self._components = None
+        self._conditions = None
+        self._model_status = None
+        self._observed_generation = None
+        self._url = None
         self.discriminator = None
 
-        if condition is not None:
-            self.condition = condition
-        if data is not None:
-            self.data = data
-        if name is not None:
-            self.name = name
-        if node_name is not None:
-            self.node_name = node_name
-        if service_name is not None:
-            self.service_name = service_name
-        if service_url is not None:
-            self.service_url = service_url
-        if weight is not None:
-            self.weight = weight
+        if address is not None:
+            self.address = address
+        if annotations is not None:
+            self.annotations = annotations
+        if components is not None:
+            self.components = components
+        if conditions is not None:
+            self.conditions = conditions
+        if model_status is not None:
+            self.model_status = model_status
+        if observed_generation is not None:
+            self.observed_generation = observed_generation
+        if url is not None:
+            self.url = url
 
     @property
-    def condition(self):
-        """Gets the condition of this V1alpha1InferenceStep.  # noqa: E501
+    def address(self):
+        """Gets the address of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        routing based on the condition  # noqa: E501
 
-        :return: The condition of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The address of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: KnativeAddressable
         """
-        return self._condition
+        return self._address
 
-    @condition.setter
-    def condition(self, condition):
-        """Sets the condition of this V1alpha1InferenceStep.
+    @address.setter
+    def address(self, address):
+        """Sets the address of this V1beta1InferenceServiceStatus.
 
-        routing based on the condition  # noqa: E501
 
-        :param condition: The condition of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param address: The address of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: KnativeAddressable
         """
 
-        self._condition = condition
+        self._address = address
 
     @property
-    def data(self):
-        """Gets the data of this V1alpha1InferenceStep.  # noqa: E501
+    def annotations(self):
+        """Gets the annotations of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        request data sent to the next route with input/output from the previous step $request $response.predictions  # noqa: E501
+        Annotations is additional Status fields for the Resource to save some additional State as well as convey more information to the user. This is roughly akin to Annotations on any k8s resource, just the reconciler conveying richer information outwards.  # noqa: E501
 
-        :return: The data of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The annotations of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: dict(str, str)
         """
-        return self._data
+        return self._annotations
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this V1alpha1InferenceStep.
+    @annotations.setter
+    def annotations(self, annotations):
+        """Sets the annotations of this V1beta1InferenceServiceStatus.
 
-        request data sent to the next route with input/output from the previous step $request $response.predictions  # noqa: E501
+        Annotations is additional Status fields for the Resource to save some additional State as well as convey more information to the user. This is roughly akin to Annotations on any k8s resource, just the reconciler conveying richer information outwards.  # noqa: E501
 
-        :param data: The data of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param annotations: The annotations of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: dict(str, str)
         """
 
-        self._data = data
+        self._annotations = annotations
 
     @property
-    def name(self):
-        """Gets the name of this V1alpha1InferenceStep.  # noqa: E501
+    def components(self):
+        """Gets the components of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        Unique name for the step within this node  # noqa: E501
+        Statuses for the components of the InferenceService  # noqa: E501
 
-        :return: The name of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The components of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: dict(str, V1beta1ComponentStatusSpec)
         """
-        return self._name
+        return self._components
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this V1alpha1InferenceStep.
+    @components.setter
+    def components(self, components):
+        """Sets the components of this V1beta1InferenceServiceStatus.
 
-        Unique name for the step within this node  # noqa: E501
+        Statuses for the components of the InferenceService  # noqa: E501
 
-        :param name: The name of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param components: The components of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: dict(str, V1beta1ComponentStatusSpec)
         """
 
-        self._name = name
+        self._components = components
 
     @property
-    def node_name(self):
-        """Gets the node_name of this V1alpha1InferenceStep.  # noqa: E501
+    def conditions(self):
+        """Gets the conditions of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        The node name for routing as next step  # noqa: E501
+        Conditions the latest available observations of a resource's current state.  # noqa: E501
 
-        :return: The node_name of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The conditions of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: list[KnativeCondition]
         """
-        return self._node_name
+        return self._conditions
 
-    @node_name.setter
-    def node_name(self, node_name):
-        """Sets the node_name of this V1alpha1InferenceStep.
+    @conditions.setter
+    def conditions(self, conditions):
+        """Sets the conditions of this V1beta1InferenceServiceStatus.
 
-        The node name for routing as next step  # noqa: E501
+        Conditions the latest available observations of a resource's current state.  # noqa: E501
 
-        :param node_name: The node_name of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param conditions: The conditions of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: list[KnativeCondition]
         """
 
-        self._node_name = node_name
+        self._conditions = conditions
 
     @property
-    def service_name(self):
-        """Gets the service_name of this V1alpha1InferenceStep.  # noqa: E501
+    def model_status(self):
+        """Gets the model_status of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        named reference for InferenceService  # noqa: E501
 
-        :return: The service_name of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The model_status of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: V1beta1ModelStatus
         """
-        return self._service_name
+        return self._model_status
 
-    @service_name.setter
-    def service_name(self, service_name):
-        """Sets the service_name of this V1alpha1InferenceStep.
+    @model_status.setter
+    def model_status(self, model_status):
+        """Sets the model_status of this V1beta1InferenceServiceStatus.
 
-        named reference for InferenceService  # noqa: E501
 
-        :param service_name: The service_name of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param model_status: The model_status of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: V1beta1ModelStatus
         """
 
-        self._service_name = service_name
+        self._model_status = model_status
 
     @property
-    def service_url(self):
-        """Gets the service_url of this V1alpha1InferenceStep.  # noqa: E501
+    def observed_generation(self):
+        """Gets the observed_generation of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        InferenceService URL, mutually exclusive with ServiceName  # noqa: E501
+        ObservedGeneration is the 'Generation' of the Service that was last processed by the controller.  # noqa: E501
 
-        :return: The service_url of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: str
+        :return: The observed_generation of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: int
         """
-        return self._service_url
+        return self._observed_generation
 
-    @service_url.setter
-    def service_url(self, service_url):
-        """Sets the service_url of this V1alpha1InferenceStep.
+    @observed_generation.setter
+    def observed_generation(self, observed_generation):
+        """Sets the observed_generation of this V1beta1InferenceServiceStatus.
 
-        InferenceService URL, mutually exclusive with ServiceName  # noqa: E501
+        ObservedGeneration is the 'Generation' of the Service that was last processed by the controller.  # noqa: E501
 
-        :param service_url: The service_url of this V1alpha1InferenceStep.  # noqa: E501
-        :type: str
+        :param observed_generation: The observed_generation of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: int
         """
 
-        self._service_url = service_url
+        self._observed_generation = observed_generation
 
     @property
-    def weight(self):
-        """Gets the weight of this V1alpha1InferenceStep.  # noqa: E501
+    def url(self):
+        """Gets the url of this V1beta1InferenceServiceStatus.  # noqa: E501
 
-        the weight for split of the traffic, only used for Split Router when weight is specified all the routing targets should be sum to 100  # noqa: E501
 
-        :return: The weight of this V1alpha1InferenceStep.  # noqa: E501
-        :rtype: int
+        :return: The url of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :rtype: KnativeURL
         """
-        return self._weight
+        return self._url
 
-    @weight.setter
-    def weight(self, weight):
-        """Sets the weight of this V1alpha1InferenceStep.
+    @url.setter
+    def url(self, url):
+        """Sets the url of this V1beta1InferenceServiceStatus.
 
-        the weight for split of the traffic, only used for Split Router when weight is specified all the routing targets should be sum to 100  # noqa: E501
 
-        :param weight: The weight of this V1alpha1InferenceStep.  # noqa: E501
-        :type: int
+        :param url: The url of this V1beta1InferenceServiceStatus.  # noqa: E501
+        :type: KnativeURL
         """
 
-        self._weight = weight
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -287,18 +281,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceStep):
+        if not isinstance(other, V1beta1InferenceServiceStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceStep):
+        if not isinstance(other, V1beta1InferenceServiceStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_inference_target.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_explainers_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,126 +28,120 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1InferenceTarget(object):
+class V1beta1ExplainersConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'node_name': 'str',
-        'service_name': 'str',
-        'service_url': 'str'
+        'aix': 'V1beta1ExplainerConfig',
+        'alibi': 'V1beta1ExplainerConfig',
+        'art': 'V1beta1ExplainerConfig'
     }
 
     attribute_map = {
-        'node_name': 'nodeName',
-        'service_name': 'serviceName',
-        'service_url': 'serviceUrl'
+        'aix': 'aix',
+        'alibi': 'alibi',
+        'art': 'art'
     }
 
-    def __init__(self, node_name=None, service_name=None, service_url=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1InferenceTarget - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, aix=None, alibi=None, art=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1ExplainersConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._node_name = None
-        self._service_name = None
-        self._service_url = None
+        self._aix = None
+        self._alibi = None
+        self._art = None
         self.discriminator = None
 
-        if node_name is not None:
-            self.node_name = node_name
-        if service_name is not None:
-            self.service_name = service_name
-        if service_url is not None:
-            self.service_url = service_url
+        if aix is not None:
+            self.aix = aix
+        if alibi is not None:
+            self.alibi = alibi
+        if art is not None:
+            self.art = art
 
     @property
-    def node_name(self):
-        """Gets the node_name of this V1alpha1InferenceTarget.  # noqa: E501
+    def aix(self):
+        """Gets the aix of this V1beta1ExplainersConfig.  # noqa: E501
 
-        The node name for routing as next step  # noqa: E501
 
-        :return: The node_name of this V1alpha1InferenceTarget.  # noqa: E501
-        :rtype: str
+        :return: The aix of this V1beta1ExplainersConfig.  # noqa: E501
+        :rtype: V1beta1ExplainerConfig
         """
-        return self._node_name
+        return self._aix
 
-    @node_name.setter
-    def node_name(self, node_name):
-        """Sets the node_name of this V1alpha1InferenceTarget.
+    @aix.setter
+    def aix(self, aix):
+        """Sets the aix of this V1beta1ExplainersConfig.
 
-        The node name for routing as next step  # noqa: E501
 
-        :param node_name: The node_name of this V1alpha1InferenceTarget.  # noqa: E501
-        :type: str
+        :param aix: The aix of this V1beta1ExplainersConfig.  # noqa: E501
+        :type: V1beta1ExplainerConfig
         """
 
-        self._node_name = node_name
+        self._aix = aix
 
     @property
-    def service_name(self):
-        """Gets the service_name of this V1alpha1InferenceTarget.  # noqa: E501
+    def alibi(self):
+        """Gets the alibi of this V1beta1ExplainersConfig.  # noqa: E501
 
-        named reference for InferenceService  # noqa: E501
 
-        :return: The service_name of this V1alpha1InferenceTarget.  # noqa: E501
-        :rtype: str
+        :return: The alibi of this V1beta1ExplainersConfig.  # noqa: E501
+        :rtype: V1beta1ExplainerConfig
         """
-        return self._service_name
+        return self._alibi
 
-    @service_name.setter
-    def service_name(self, service_name):
-        """Sets the service_name of this V1alpha1InferenceTarget.
+    @alibi.setter
+    def alibi(self, alibi):
+        """Sets the alibi of this V1beta1ExplainersConfig.
 
-        named reference for InferenceService  # noqa: E501
 
-        :param service_name: The service_name of this V1alpha1InferenceTarget.  # noqa: E501
-        :type: str
+        :param alibi: The alibi of this V1beta1ExplainersConfig.  # noqa: E501
+        :type: V1beta1ExplainerConfig
         """
 
-        self._service_name = service_name
+        self._alibi = alibi
 
     @property
-    def service_url(self):
-        """Gets the service_url of this V1alpha1InferenceTarget.  # noqa: E501
+    def art(self):
+        """Gets the art of this V1beta1ExplainersConfig.  # noqa: E501
 
-        InferenceService URL, mutually exclusive with ServiceName  # noqa: E501
 
-        :return: The service_url of this V1alpha1InferenceTarget.  # noqa: E501
-        :rtype: str
+        :return: The art of this V1beta1ExplainersConfig.  # noqa: E501
+        :rtype: V1beta1ExplainerConfig
         """
-        return self._service_url
+        return self._art
 
-    @service_url.setter
-    def service_url(self, service_url):
-        """Sets the service_url of this V1alpha1InferenceTarget.
+    @art.setter
+    def art(self, art):
+        """Sets the art of this V1beta1ExplainersConfig.
 
-        InferenceService URL, mutually exclusive with ServiceName  # noqa: E501
 
-        :param service_url: The service_url of this V1alpha1InferenceTarget.  # noqa: E501
-        :type: str
+        :param art: The art of this V1beta1ExplainersConfig.  # noqa: E501
+        :type: V1beta1ExplainerConfig
         """
 
-        self._service_url = service_url
+        self._art = art
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -175,18 +169,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1InferenceTarget):
+        if not isinstance(other, V1beta1ExplainersConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1InferenceTarget):
+        if not isinstance(other, V1beta1ExplainersConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_model_spec.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_model_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_serving_runtime.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_serving_runtime_pod_spec.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_pod_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_serving_runtime_spec.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_serving_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_storage_helper.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_predictor_protocols.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,68 +28,94 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1StorageHelper(object):
+class V1beta1PredictorProtocols(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'disabled': 'bool'
+        'v1': 'V1beta1PredictorConfig',
+        'v2': 'V1beta1PredictorConfig'
     }
 
     attribute_map = {
-        'disabled': 'disabled'
+        'v1': 'v1',
+        'v2': 'v2'
     }
 
-    def __init__(self, disabled=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1StorageHelper - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, v1=None, v2=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1PredictorProtocols - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._disabled = None
+        self._v1 = None
+        self._v2 = None
         self.discriminator = None
 
-        if disabled is not None:
-            self.disabled = disabled
+        if v1 is not None:
+            self.v1 = v1
+        if v2 is not None:
+            self.v2 = v2
 
     @property
-    def disabled(self):
-        """Gets the disabled of this V1alpha1StorageHelper.  # noqa: E501
+    def v1(self):
+        """Gets the v1 of this V1beta1PredictorProtocols.  # noqa: E501
 
 
-        :return: The disabled of this V1alpha1StorageHelper.  # noqa: E501
-        :rtype: bool
+        :return: The v1 of this V1beta1PredictorProtocols.  # noqa: E501
+        :rtype: V1beta1PredictorConfig
         """
-        return self._disabled
+        return self._v1
 
-    @disabled.setter
-    def disabled(self, disabled):
-        """Sets the disabled of this V1alpha1StorageHelper.
+    @v1.setter
+    def v1(self, v1):
+        """Sets the v1 of this V1beta1PredictorProtocols.
 
 
-        :param disabled: The disabled of this V1alpha1StorageHelper.  # noqa: E501
-        :type: bool
+        :param v1: The v1 of this V1beta1PredictorProtocols.  # noqa: E501
+        :type: V1beta1PredictorConfig
         """
 
-        self._disabled = disabled
+        self._v1 = v1
+
+    @property
+    def v2(self):
+        """Gets the v2 of this V1beta1PredictorProtocols.  # noqa: E501
+
+
+        :return: The v2 of this V1beta1PredictorProtocols.  # noqa: E501
+        :rtype: V1beta1PredictorConfig
+        """
+        return self._v2
+
+    @v2.setter
+    def v2(self, v2):
+        """Sets the v2 of this V1beta1PredictorProtocols.
+
+
+        :param v2: The v2 of this V1beta1PredictorProtocols.  # noqa: E501
+        :type: V1beta1PredictorConfig
+        """
+
+        self._v2 = v2
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -117,18 +143,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1StorageHelper):
+        if not isinstance(other, V1beta1PredictorProtocols):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1StorageHelper):
+        if not isinstance(other, V1beta1PredictorProtocols):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_supported_model_format.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_supported_model_format.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_trained_model.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_trained_model_list.py` & `kserve-0.9.0rc0/kserve/models/v1alpha1_trained_model_list.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1alpha1_trained_model_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_model_format.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,98 +28,98 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1alpha1TrainedModelSpec(object):
+class V1beta1ModelFormat(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'inference_service': 'str',
-        'model': 'V1alpha1ModelSpec'
+        'name': 'str',
+        'version': 'str'
     }
 
     attribute_map = {
-        'inference_service': 'inferenceService',
-        'model': 'model'
+        'name': 'name',
+        'version': 'version'
     }
 
-    def __init__(self, inference_service='', model=None, local_vars_configuration=None):  # noqa: E501
-        """V1alpha1TrainedModelSpec - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, name='', version=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1ModelFormat - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._inference_service = None
-        self._model = None
+        self._name = None
+        self._version = None
         self.discriminator = None
 
-        self.inference_service = inference_service
-        self.model = model
+        if name is not None:
+            self.name = name
+        if version is not None:
+            self.version = version
 
     @property
-    def inference_service(self):
-        """Gets the inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
+    def name(self):
+        """Gets the name of this V1beta1ModelFormat.  # noqa: E501
 
-        parent inference service to deploy to  # noqa: E501
+        Name of the model format.  # noqa: E501
 
-        :return: The inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
+        :return: The name of this V1beta1ModelFormat.  # noqa: E501
         :rtype: str
         """
-        return self._inference_service
+        return self._name
 
-    @inference_service.setter
-    def inference_service(self, inference_service):
-        """Sets the inference_service of this V1alpha1TrainedModelSpec.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this V1beta1ModelFormat.
 
-        parent inference service to deploy to  # noqa: E501
+        Name of the model format.  # noqa: E501
 
-        :param inference_service: The inference_service of this V1alpha1TrainedModelSpec.  # noqa: E501
+        :param name: The name of this V1beta1ModelFormat.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and inference_service is None:  # noqa: E501
-            raise ValueError("Invalid value for `inference_service`, must not be `None`")  # noqa: E501
 
-        self._inference_service = inference_service
+        self._name = name
 
     @property
-    def model(self):
-        """Gets the model of this V1alpha1TrainedModelSpec.  # noqa: E501
+    def version(self):
+        """Gets the version of this V1beta1ModelFormat.  # noqa: E501
 
+        Version of the model format. Used in validating that a predictor is supported by a runtime. Can be \"major\", \"major.minor\" or \"major.minor.patch\".  # noqa: E501
 
-        :return: The model of this V1alpha1TrainedModelSpec.  # noqa: E501
-        :rtype: V1alpha1ModelSpec
+        :return: The version of this V1beta1ModelFormat.  # noqa: E501
+        :rtype: str
         """
-        return self._model
+        return self._version
 
-    @model.setter
-    def model(self, model):
-        """Sets the model of this V1alpha1TrainedModelSpec.
+    @version.setter
+    def version(self, version):
+        """Sets the version of this V1beta1ModelFormat.
 
+        Version of the model format. Used in validating that a predictor is supported by a runtime. Can be \"major\", \"major.minor\" or \"major.minor.patch\".  # noqa: E501
 
-        :param model: The model of this V1alpha1TrainedModelSpec.  # noqa: E501
-        :type: V1alpha1ModelSpec
+        :param version: The version of this V1beta1ModelFormat.  # noqa: E501
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and model is None:  # noqa: E501
-            raise ValueError("Invalid value for `model`, must not be `None`")  # noqa: E501
 
-        self._model = model
+        self._version = version
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -147,18 +147,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1alpha1TrainedModelSpec):
+        if not isinstance(other, V1beta1ModelFormat):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1alpha1TrainedModelSpec):
+        if not isinstance(other, V1beta1ModelFormat):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_aix_explainer_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_aix_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_alibi_explainer_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_alibi_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_art_explainer_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_art_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_batcher.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_batcher.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_component_extension_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_component_extension_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -240,49 +240,49 @@
 
         self._min_replicas = min_replicas
 
     @property
     def scale_metric(self):
         """Gets the scale_metric of this V1beta1ComponentExtensionSpec.  # noqa: E501
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :return: The scale_metric of this V1beta1ComponentExtensionSpec.  # noqa: E501
         :rtype: str
         """
         return self._scale_metric
 
     @scale_metric.setter
     def scale_metric(self, scale_metric):
         """Sets the scale_metric of this V1beta1ComponentExtensionSpec.
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :param scale_metric: The scale_metric of this V1beta1ComponentExtensionSpec.  # noqa: E501
         :type: str
         """
 
         self._scale_metric = scale_metric
 
     @property
     def scale_target(self):
         """Gets the scale_target of this V1beta1ComponentExtensionSpec.  # noqa: E501
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :return: The scale_target of this V1beta1ComponentExtensionSpec.  # noqa: E501
         :rtype: int
         """
         return self._scale_target
 
     @scale_target.setter
     def scale_target(self, scale_target):
         """Sets the scale_target of this V1beta1ComponentExtensionSpec.
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :param scale_target: The scale_target of this V1beta1ComponentExtensionSpec.  # noqa: E501
         :type: int
         """
 
         self._scale_target = scale_target
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_component_status_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_component_status_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_custom_explainer.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_custom_explainer.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_custom_predictor.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_custom_predictor.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_custom_transformer.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_custom_transformer.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_deploy_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_deploy_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_explainer_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_explainer_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_explainer_extension_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_explainer_extension_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_explainer_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_explainer_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1041,49 +1041,49 @@
 
         self._runtime_class_name = runtime_class_name
 
     @property
     def scale_metric(self):
         """Gets the scale_metric of this V1beta1ExplainerSpec.  # noqa: E501
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :return: The scale_metric of this V1beta1ExplainerSpec.  # noqa: E501
         :rtype: str
         """
         return self._scale_metric
 
     @scale_metric.setter
     def scale_metric(self, scale_metric):
         """Sets the scale_metric of this V1beta1ExplainerSpec.
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :param scale_metric: The scale_metric of this V1beta1ExplainerSpec.  # noqa: E501
         :type: str
         """
 
         self._scale_metric = scale_metric
 
     @property
     def scale_target(self):
         """Gets the scale_target of this V1beta1ExplainerSpec.  # noqa: E501
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :return: The scale_target of this V1beta1ExplainerSpec.  # noqa: E501
         :rtype: int
         """
         return self._scale_target
 
     @scale_target.setter
     def scale_target(self, scale_target):
         """Sets the scale_target of this V1beta1ExplainerSpec.
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :param scale_target: The scale_target of this V1beta1ExplainerSpec.  # noqa: E501
         :type: int
         """
 
         self._scale_target = scale_target
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_explainers_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_spec.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,120 +28,121 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1beta1ExplainersConfig(object):
+class V1beta1InferenceServiceSpec(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'aix': 'V1beta1ExplainerConfig',
-        'alibi': 'V1beta1ExplainerConfig',
-        'art': 'V1beta1ExplainerConfig'
+        'explainer': 'V1beta1ExplainerSpec',
+        'predictor': 'V1beta1PredictorSpec',
+        'transformer': 'V1beta1TransformerSpec'
     }
 
     attribute_map = {
-        'aix': 'aix',
-        'alibi': 'alibi',
-        'art': 'art'
+        'explainer': 'explainer',
+        'predictor': 'predictor',
+        'transformer': 'transformer'
     }
 
-    def __init__(self, aix=None, alibi=None, art=None, local_vars_configuration=None):  # noqa: E501
-        """V1beta1ExplainersConfig - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, explainer=None, predictor=None, transformer=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1InferenceServiceSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._aix = None
-        self._alibi = None
-        self._art = None
+        self._explainer = None
+        self._predictor = None
+        self._transformer = None
         self.discriminator = None
 
-        if aix is not None:
-            self.aix = aix
-        if alibi is not None:
-            self.alibi = alibi
-        if art is not None:
-            self.art = art
+        if explainer is not None:
+            self.explainer = explainer
+        self.predictor = predictor
+        if transformer is not None:
+            self.transformer = transformer
 
     @property
-    def aix(self):
-        """Gets the aix of this V1beta1ExplainersConfig.  # noqa: E501
+    def explainer(self):
+        """Gets the explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
 
 
-        :return: The aix of this V1beta1ExplainersConfig.  # noqa: E501
-        :rtype: V1beta1ExplainerConfig
+        :return: The explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :rtype: V1beta1ExplainerSpec
         """
-        return self._aix
+        return self._explainer
 
-    @aix.setter
-    def aix(self, aix):
-        """Sets the aix of this V1beta1ExplainersConfig.
+    @explainer.setter
+    def explainer(self, explainer):
+        """Sets the explainer of this V1beta1InferenceServiceSpec.
 
 
-        :param aix: The aix of this V1beta1ExplainersConfig.  # noqa: E501
-        :type: V1beta1ExplainerConfig
+        :param explainer: The explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :type: V1beta1ExplainerSpec
         """
 
-        self._aix = aix
+        self._explainer = explainer
 
     @property
-    def alibi(self):
-        """Gets the alibi of this V1beta1ExplainersConfig.  # noqa: E501
+    def predictor(self):
+        """Gets the predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
 
 
-        :return: The alibi of this V1beta1ExplainersConfig.  # noqa: E501
-        :rtype: V1beta1ExplainerConfig
+        :return: The predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :rtype: V1beta1PredictorSpec
         """
-        return self._alibi
+        return self._predictor
 
-    @alibi.setter
-    def alibi(self, alibi):
-        """Sets the alibi of this V1beta1ExplainersConfig.
+    @predictor.setter
+    def predictor(self, predictor):
+        """Sets the predictor of this V1beta1InferenceServiceSpec.
 
 
-        :param alibi: The alibi of this V1beta1ExplainersConfig.  # noqa: E501
-        :type: V1beta1ExplainerConfig
+        :param predictor: The predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :type: V1beta1PredictorSpec
         """
+        if self.local_vars_configuration.client_side_validation and predictor is None:  # noqa: E501
+            raise ValueError("Invalid value for `predictor`, must not be `None`")  # noqa: E501
 
-        self._alibi = alibi
+        self._predictor = predictor
 
     @property
-    def art(self):
-        """Gets the art of this V1beta1ExplainersConfig.  # noqa: E501
+    def transformer(self):
+        """Gets the transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
 
 
-        :return: The art of this V1beta1ExplainersConfig.  # noqa: E501
-        :rtype: V1beta1ExplainerConfig
+        :return: The transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :rtype: V1beta1TransformerSpec
         """
-        return self._art
+        return self._transformer
 
-    @art.setter
-    def art(self, art):
-        """Sets the art of this V1beta1ExplainersConfig.
+    @transformer.setter
+    def transformer(self, transformer):
+        """Sets the transformer of this V1beta1InferenceServiceSpec.
 
 
-        :param art: The art of this V1beta1ExplainersConfig.  # noqa: E501
-        :type: V1beta1ExplainerConfig
+        :param transformer: The transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
+        :type: V1beta1TransformerSpec
         """
 
-        self._art = art
+        self._transformer = transformer
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -169,18 +170,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1beta1ExplainersConfig):
+        if not isinstance(other, V1beta1InferenceServiceSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1beta1ExplainersConfig):
+        if not isinstance(other, V1beta1InferenceServiceSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_failure_info.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_failure_info.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_inference_service.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_inference_service_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1beta1InferenceService(object):
+class V1beta1InferenceServiceList(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -44,161 +44,136 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
+        'items': 'list[V1beta1InferenceService]',
         'kind': 'str',
-        'metadata': 'V1ObjectMeta',
-        'spec': 'V1beta1InferenceServiceSpec',
-        'status': 'V1beta1InferenceServiceStatus'
+        'metadata': 'V1ListMeta'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
+        'items': 'items',
         'kind': 'kind',
-        'metadata': 'metadata',
-        'spec': 'spec',
-        'status': 'status'
+        'metadata': 'metadata'
     }
 
-    def __init__(self, api_version=None, kind=None, metadata=None, spec=None, status=None, local_vars_configuration=None):  # noqa: E501
-        """V1beta1InferenceService - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, api_version=None, items=None, kind=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1InferenceServiceList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._api_version = None
+        self._items = None
         self._kind = None
         self._metadata = None
-        self._spec = None
-        self._status = None
         self.discriminator = None
 
         if api_version is not None:
             self.api_version = api_version
+        self.items = items
         if kind is not None:
             self.kind = kind
         if metadata is not None:
             self.metadata = metadata
-        if spec is not None:
-            self.spec = spec
-        if status is not None:
-            self.status = status
 
     @property
     def api_version(self):
-        """Gets the api_version of this V1beta1InferenceService.  # noqa: E501
+        """Gets the api_version of this V1beta1InferenceServiceList.  # noqa: E501
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :return: The api_version of this V1beta1InferenceService.  # noqa: E501
+        :return: The api_version of this V1beta1InferenceServiceList.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this V1beta1InferenceService.
+        """Sets the api_version of this V1beta1InferenceServiceList.
 
         APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources  # noqa: E501
 
-        :param api_version: The api_version of this V1beta1InferenceService.  # noqa: E501
+        :param api_version: The api_version of this V1beta1InferenceServiceList.  # noqa: E501
         :type: str
         """
 
         self._api_version = api_version
 
     @property
+    def items(self):
+        """Gets the items of this V1beta1InferenceServiceList.  # noqa: E501
+
+
+        :return: The items of this V1beta1InferenceServiceList.  # noqa: E501
+        :rtype: list[V1beta1InferenceService]
+        """
+        return self._items
+
+    @items.setter
+    def items(self, items):
+        """Sets the items of this V1beta1InferenceServiceList.
+
+
+        :param items: The items of this V1beta1InferenceServiceList.  # noqa: E501
+        :type: list[V1beta1InferenceService]
+        """
+        if self.local_vars_configuration.client_side_validation and items is None:  # noqa: E501
+            raise ValueError("Invalid value for `items`, must not be `None`")  # noqa: E501
+
+        self._items = items
+
+    @property
     def kind(self):
-        """Gets the kind of this V1beta1InferenceService.  # noqa: E501
+        """Gets the kind of this V1beta1InferenceServiceList.  # noqa: E501
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :return: The kind of this V1beta1InferenceService.  # noqa: E501
+        :return: The kind of this V1beta1InferenceServiceList.  # noqa: E501
         :rtype: str
         """
         return self._kind
 
     @kind.setter
     def kind(self, kind):
-        """Sets the kind of this V1beta1InferenceService.
+        """Sets the kind of this V1beta1InferenceServiceList.
 
         Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds  # noqa: E501
 
-        :param kind: The kind of this V1beta1InferenceService.  # noqa: E501
+        :param kind: The kind of this V1beta1InferenceServiceList.  # noqa: E501
         :type: str
         """
 
         self._kind = kind
 
     @property
     def metadata(self):
-        """Gets the metadata of this V1beta1InferenceService.  # noqa: E501
+        """Gets the metadata of this V1beta1InferenceServiceList.  # noqa: E501
 
 
-        :return: The metadata of this V1beta1InferenceService.  # noqa: E501
-        :rtype: V1ObjectMeta
+        :return: The metadata of this V1beta1InferenceServiceList.  # noqa: E501
+        :rtype: V1ListMeta
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
-        """Sets the metadata of this V1beta1InferenceService.
+        """Sets the metadata of this V1beta1InferenceServiceList.
 
 
-        :param metadata: The metadata of this V1beta1InferenceService.  # noqa: E501
-        :type: V1ObjectMeta
+        :param metadata: The metadata of this V1beta1InferenceServiceList.  # noqa: E501
+        :type: V1ListMeta
         """
 
         self._metadata = metadata
 
-    @property
-    def spec(self):
-        """Gets the spec of this V1beta1InferenceService.  # noqa: E501
-
-
-        :return: The spec of this V1beta1InferenceService.  # noqa: E501
-        :rtype: V1beta1InferenceServiceSpec
-        """
-        return self._spec
-
-    @spec.setter
-    def spec(self, spec):
-        """Sets the spec of this V1beta1InferenceService.
-
-
-        :param spec: The spec of this V1beta1InferenceService.  # noqa: E501
-        :type: V1beta1InferenceServiceSpec
-        """
-
-        self._spec = spec
-
-    @property
-    def status(self):
-        """Gets the status of this V1beta1InferenceService.  # noqa: E501
-
-
-        :return: The status of this V1beta1InferenceService.  # noqa: E501
-        :rtype: V1beta1InferenceServiceStatus
-        """
-        return self._status
-
-    @status.setter
-    def status(self, status):
-        """Sets the status of this V1beta1InferenceService.
-
-
-        :param status: The status of this V1beta1InferenceService.  # noqa: E501
-        :type: V1beta1InferenceServiceStatus
-        """
-
-        self._status = status
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -225,18 +200,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1beta1InferenceService):
+        if not isinstance(other, V1beta1InferenceServiceList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1beta1InferenceService):
+        if not isinstance(other, V1beta1InferenceServiceList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_inference_service_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_inference_services_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,121 +28,123 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1beta1InferenceServiceSpec(object):
+class V1beta1InferenceServicesConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'explainer': 'V1beta1ExplainerSpec',
-        'predictor': 'V1beta1PredictorSpec',
-        'transformer': 'V1beta1TransformerSpec'
+        'explainers': 'V1beta1ExplainersConfig',
+        'predictors': 'V1beta1PredictorsConfig',
+        'transformers': 'V1beta1TransformersConfig'
     }
 
     attribute_map = {
-        'explainer': 'explainer',
-        'predictor': 'predictor',
-        'transformer': 'transformer'
+        'explainers': 'explainers',
+        'predictors': 'predictors',
+        'transformers': 'transformers'
     }
 
-    def __init__(self, explainer=None, predictor=None, transformer=None, local_vars_configuration=None):  # noqa: E501
-        """V1beta1InferenceServiceSpec - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, explainers=None, predictors=None, transformers=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1InferenceServicesConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._explainer = None
-        self._predictor = None
-        self._transformer = None
+        self._explainers = None
+        self._predictors = None
+        self._transformers = None
         self.discriminator = None
 
-        if explainer is not None:
-            self.explainer = explainer
-        self.predictor = predictor
-        if transformer is not None:
-            self.transformer = transformer
+        self.explainers = explainers
+        self.predictors = predictors
+        self.transformers = transformers
 
     @property
-    def explainer(self):
-        """Gets the explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
+    def explainers(self):
+        """Gets the explainers of this V1beta1InferenceServicesConfig.  # noqa: E501
 
 
-        :return: The explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :rtype: V1beta1ExplainerSpec
+        :return: The explainers of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :rtype: V1beta1ExplainersConfig
         """
-        return self._explainer
+        return self._explainers
 
-    @explainer.setter
-    def explainer(self, explainer):
-        """Sets the explainer of this V1beta1InferenceServiceSpec.
+    @explainers.setter
+    def explainers(self, explainers):
+        """Sets the explainers of this V1beta1InferenceServicesConfig.
 
 
-        :param explainer: The explainer of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :type: V1beta1ExplainerSpec
+        :param explainers: The explainers of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :type: V1beta1ExplainersConfig
         """
+        if self.local_vars_configuration.client_side_validation and explainers is None:  # noqa: E501
+            raise ValueError("Invalid value for `explainers`, must not be `None`")  # noqa: E501
 
-        self._explainer = explainer
+        self._explainers = explainers
 
     @property
-    def predictor(self):
-        """Gets the predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
+    def predictors(self):
+        """Gets the predictors of this V1beta1InferenceServicesConfig.  # noqa: E501
 
 
-        :return: The predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :rtype: V1beta1PredictorSpec
+        :return: The predictors of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :rtype: V1beta1PredictorsConfig
         """
-        return self._predictor
+        return self._predictors
 
-    @predictor.setter
-    def predictor(self, predictor):
-        """Sets the predictor of this V1beta1InferenceServiceSpec.
+    @predictors.setter
+    def predictors(self, predictors):
+        """Sets the predictors of this V1beta1InferenceServicesConfig.
 
 
-        :param predictor: The predictor of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :type: V1beta1PredictorSpec
+        :param predictors: The predictors of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :type: V1beta1PredictorsConfig
         """
-        if self.local_vars_configuration.client_side_validation and predictor is None:  # noqa: E501
-            raise ValueError("Invalid value for `predictor`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and predictors is None:  # noqa: E501
+            raise ValueError("Invalid value for `predictors`, must not be `None`")  # noqa: E501
 
-        self._predictor = predictor
+        self._predictors = predictors
 
     @property
-    def transformer(self):
-        """Gets the transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
+    def transformers(self):
+        """Gets the transformers of this V1beta1InferenceServicesConfig.  # noqa: E501
 
 
-        :return: The transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :rtype: V1beta1TransformerSpec
+        :return: The transformers of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :rtype: V1beta1TransformersConfig
         """
-        return self._transformer
+        return self._transformers
 
-    @transformer.setter
-    def transformer(self, transformer):
-        """Sets the transformer of this V1beta1InferenceServiceSpec.
+    @transformers.setter
+    def transformers(self, transformers):
+        """Sets the transformers of this V1beta1InferenceServicesConfig.
 
 
-        :param transformer: The transformer of this V1beta1InferenceServiceSpec.  # noqa: E501
-        :type: V1beta1TransformerSpec
+        :param transformers: The transformers of this V1beta1InferenceServicesConfig.  # noqa: E501
+        :type: V1beta1TransformersConfig
         """
+        if self.local_vars_configuration.client_side_validation and transformers is None:  # noqa: E501
+            raise ValueError("Invalid value for `transformers`, must not be `None`")  # noqa: E501
 
-        self._transformer = transformer
+        self._transformers = transformers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -170,18 +172,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1beta1InferenceServiceSpec):
+        if not isinstance(other, V1beta1InferenceServicesConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1beta1InferenceServiceSpec):
+        if not isinstance(other, V1beta1InferenceServicesConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_ingress_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_ingress_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,43 +49,40 @@
     openapi_types = {
         'domain_template': 'str',
         'ingress_class_name': 'str',
         'ingress_domain': 'str',
         'ingress_gateway': 'str',
         'ingress_service': 'str',
         'local_gateway': 'str',
-        'local_gateway_service': 'str',
-        'url_scheme': 'str'
+        'local_gateway_service': 'str'
     }
 
     attribute_map = {
         'domain_template': 'domainTemplate',
         'ingress_class_name': 'ingressClassName',
         'ingress_domain': 'ingressDomain',
         'ingress_gateway': 'ingressGateway',
         'ingress_service': 'ingressService',
         'local_gateway': 'localGateway',
-        'local_gateway_service': 'localGatewayService',
-        'url_scheme': 'urlScheme'
+        'local_gateway_service': 'localGatewayService'
     }
 
-    def __init__(self, domain_template=None, ingress_class_name=None, ingress_domain=None, ingress_gateway=None, ingress_service=None, local_gateway=None, local_gateway_service=None, url_scheme=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, domain_template=None, ingress_class_name=None, ingress_domain=None, ingress_gateway=None, ingress_service=None, local_gateway=None, local_gateway_service=None, local_vars_configuration=None):  # noqa: E501
         """V1beta1IngressConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._domain_template = None
         self._ingress_class_name = None
         self._ingress_domain = None
         self._ingress_gateway = None
         self._ingress_service = None
         self._local_gateway = None
         self._local_gateway_service = None
-        self._url_scheme = None
         self.discriminator = None
 
         if domain_template is not None:
             self.domain_template = domain_template
         if ingress_class_name is not None:
             self.ingress_class_name = ingress_class_name
         if ingress_domain is not None:
@@ -94,16 +91,14 @@
             self.ingress_gateway = ingress_gateway
         if ingress_service is not None:
             self.ingress_service = ingress_service
         if local_gateway is not None:
             self.local_gateway = local_gateway
         if local_gateway_service is not None:
             self.local_gateway_service = local_gateway_service
-        if url_scheme is not None:
-            self.url_scheme = url_scheme
 
     @property
     def domain_template(self):
         """Gets the domain_template of this V1beta1IngressConfig.  # noqa: E501
 
 
         :return: The domain_template of this V1beta1IngressConfig.  # noqa: E501
@@ -244,35 +239,14 @@
 
         :param local_gateway_service: The local_gateway_service of this V1beta1IngressConfig.  # noqa: E501
         :type: str
         """
 
         self._local_gateway_service = local_gateway_service
 
-    @property
-    def url_scheme(self):
-        """Gets the url_scheme of this V1beta1IngressConfig.  # noqa: E501
-
-
-        :return: The url_scheme of this V1beta1IngressConfig.  # noqa: E501
-        :rtype: str
-        """
-        return self._url_scheme
-
-    @url_scheme.setter
-    def url_scheme(self, url_scheme):
-        """Sets the url_scheme of this V1beta1IngressConfig.
-
-
-        :param url_scheme: The url_scheme of this V1beta1IngressConfig.  # noqa: E501
-        :type: str
-        """
-
-        self._url_scheme = url_scheme
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_light_gbm_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_light_gbm_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_logger_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_logger_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_model_copies.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_model_copies.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_model_format.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_transformers_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,98 +28,68 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1beta1ModelFormat(object):
+class V1beta1TransformersConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'name': 'str',
-        'version': 'str'
+        'feast': 'V1beta1TransformerConfig'
     }
 
     attribute_map = {
-        'name': 'name',
-        'version': 'version'
+        'feast': 'feast'
     }
 
-    def __init__(self, name='', version=None, local_vars_configuration=None):  # noqa: E501
-        """V1beta1ModelFormat - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, feast=None, local_vars_configuration=None):  # noqa: E501
+        """V1beta1TransformersConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._name = None
-        self._version = None
+        self._feast = None
         self.discriminator = None
 
-        if name is not None:
-            self.name = name
-        if version is not None:
-            self.version = version
+        if feast is not None:
+            self.feast = feast
 
     @property
-    def name(self):
-        """Gets the name of this V1beta1ModelFormat.  # noqa: E501
+    def feast(self):
+        """Gets the feast of this V1beta1TransformersConfig.  # noqa: E501
 
-        Name of the model format.  # noqa: E501
 
-        :return: The name of this V1beta1ModelFormat.  # noqa: E501
-        :rtype: str
+        :return: The feast of this V1beta1TransformersConfig.  # noqa: E501
+        :rtype: V1beta1TransformerConfig
         """
-        return self._name
+        return self._feast
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this V1beta1ModelFormat.
+    @feast.setter
+    def feast(self, feast):
+        """Sets the feast of this V1beta1TransformersConfig.
 
-        Name of the model format.  # noqa: E501
 
-        :param name: The name of this V1beta1ModelFormat.  # noqa: E501
-        :type: str
+        :param feast: The feast of this V1beta1TransformersConfig.  # noqa: E501
+        :type: V1beta1TransformerConfig
         """
 
-        self._name = name
-
-    @property
-    def version(self):
-        """Gets the version of this V1beta1ModelFormat.  # noqa: E501
-
-        Version of the model format. Used in validating that a predictor is supported by a runtime. Can be \"major\", \"major.minor\" or \"major.minor.patch\".  # noqa: E501
-
-        :return: The version of this V1beta1ModelFormat.  # noqa: E501
-        :rtype: str
-        """
-        return self._version
-
-    @version.setter
-    def version(self, version):
-        """Sets the version of this V1beta1ModelFormat.
-
-        Version of the model format. Used in validating that a predictor is supported by a runtime. Can be \"major\", \"major.minor\" or \"major.minor.patch\".  # noqa: E501
-
-        :param version: The version of this V1beta1ModelFormat.  # noqa: E501
-        :type: str
-        """
-
-        self._version = version
+        self._feast = feast
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -147,18 +117,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1beta1ModelFormat):
+        if not isinstance(other, V1beta1TransformersConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1beta1ModelFormat):
+        if not isinstance(other, V1beta1TransformersConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_model_revision_states.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_model_revision_states.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_model_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_model_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_model_status.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_model_status.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_onnx_runtime_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_onnx_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_paddle_server_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_paddle_server_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_pmml_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_pmml_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_pod_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_pod_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_predictor_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_predictor_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_predictor_extension_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_predictor_extension_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_predictor_protocols.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_transformer_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,94 +28,100 @@
 import re  # noqa: F401
 
 import six
 
 from kserve.configuration import Configuration
 
 
-class V1beta1PredictorProtocols(object):
+class V1beta1TransformerConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'v1': 'V1beta1PredictorConfig',
-        'v2': 'V1beta1PredictorConfig'
+        'default_image_version': 'str',
+        'image': 'str'
     }
 
     attribute_map = {
-        'v1': 'v1',
-        'v2': 'v2'
+        'default_image_version': 'defaultImageVersion',
+        'image': 'image'
     }
 
-    def __init__(self, v1=None, v2=None, local_vars_configuration=None):  # noqa: E501
-        """V1beta1PredictorProtocols - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, default_image_version='', image='', local_vars_configuration=None):  # noqa: E501
+        """V1beta1TransformerConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._v1 = None
-        self._v2 = None
+        self._default_image_version = None
+        self._image = None
         self.discriminator = None
 
-        if v1 is not None:
-            self.v1 = v1
-        if v2 is not None:
-            self.v2 = v2
+        self.default_image_version = default_image_version
+        self.image = image
 
     @property
-    def v1(self):
-        """Gets the v1 of this V1beta1PredictorProtocols.  # noqa: E501
+    def default_image_version(self):
+        """Gets the default_image_version of this V1beta1TransformerConfig.  # noqa: E501
 
+        default transformer docker image version  # noqa: E501
 
-        :return: The v1 of this V1beta1PredictorProtocols.  # noqa: E501
-        :rtype: V1beta1PredictorConfig
+        :return: The default_image_version of this V1beta1TransformerConfig.  # noqa: E501
+        :rtype: str
         """
-        return self._v1
+        return self._default_image_version
 
-    @v1.setter
-    def v1(self, v1):
-        """Sets the v1 of this V1beta1PredictorProtocols.
+    @default_image_version.setter
+    def default_image_version(self, default_image_version):
+        """Sets the default_image_version of this V1beta1TransformerConfig.
 
+        default transformer docker image version  # noqa: E501
 
-        :param v1: The v1 of this V1beta1PredictorProtocols.  # noqa: E501
-        :type: V1beta1PredictorConfig
+        :param default_image_version: The default_image_version of this V1beta1TransformerConfig.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and default_image_version is None:  # noqa: E501
+            raise ValueError("Invalid value for `default_image_version`, must not be `None`")  # noqa: E501
 
-        self._v1 = v1
+        self._default_image_version = default_image_version
 
     @property
-    def v2(self):
-        """Gets the v2 of this V1beta1PredictorProtocols.  # noqa: E501
+    def image(self):
+        """Gets the image of this V1beta1TransformerConfig.  # noqa: E501
 
+        transformer docker image name  # noqa: E501
 
-        :return: The v2 of this V1beta1PredictorProtocols.  # noqa: E501
-        :rtype: V1beta1PredictorConfig
+        :return: The image of this V1beta1TransformerConfig.  # noqa: E501
+        :rtype: str
         """
-        return self._v2
+        return self._image
 
-    @v2.setter
-    def v2(self, v2):
-        """Sets the v2 of this V1beta1PredictorProtocols.
+    @image.setter
+    def image(self, image):
+        """Sets the image of this V1beta1TransformerConfig.
 
+        transformer docker image name  # noqa: E501
 
-        :param v2: The v2 of this V1beta1PredictorProtocols.  # noqa: E501
-        :type: V1beta1PredictorConfig
+        :param image: The image of this V1beta1TransformerConfig.  # noqa: E501
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and image is None:  # noqa: E501
+            raise ValueError("Invalid value for `image`, must not be `None`")  # noqa: E501
 
-        self._v2 = v2
+        self._image = image
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -143,18 +149,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1beta1PredictorProtocols):
+        if not isinstance(other, V1beta1TransformerConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1beta1PredictorProtocols):
+        if not isinstance(other, V1beta1TransformerConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_predictor_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_predictor_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1139,49 +1139,49 @@
 
         self._runtime_class_name = runtime_class_name
 
     @property
     def scale_metric(self):
         """Gets the scale_metric of this V1beta1PredictorSpec.  # noqa: E501
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :return: The scale_metric of this V1beta1PredictorSpec.  # noqa: E501
         :rtype: str
         """
         return self._scale_metric
 
     @scale_metric.setter
     def scale_metric(self, scale_metric):
         """Sets the scale_metric of this V1beta1PredictorSpec.
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :param scale_metric: The scale_metric of this V1beta1PredictorSpec.  # noqa: E501
         :type: str
         """
 
         self._scale_metric = scale_metric
 
     @property
     def scale_target(self):
         """Gets the scale_target of this V1beta1PredictorSpec.  # noqa: E501
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :return: The scale_target of this V1beta1PredictorSpec.  # noqa: E501
         :rtype: int
         """
         return self._scale_target
 
     @scale_target.setter
     def scale_target(self, scale_target):
         """Sets the scale_target of this V1beta1PredictorSpec.
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :param scale_target: The scale_target of this V1beta1PredictorSpec.  # noqa: E501
         :type: int
         """
 
         self._scale_target = scale_target
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_predictors_config.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_predictors_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_sk_learn_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_sk_learn_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_storage_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_storage_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_tf_serving_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_tf_serving_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_torch_serve_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_torch_serve_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_transformer_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_transformer_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -963,49 +963,49 @@
 
         self._runtime_class_name = runtime_class_name
 
     @property
     def scale_metric(self):
         """Gets the scale_metric of this V1beta1TransformerSpec.  # noqa: E501
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :return: The scale_metric of this V1beta1TransformerSpec.  # noqa: E501
         :rtype: str
         """
         return self._scale_metric
 
     @scale_metric.setter
     def scale_metric(self, scale_metric):
         """Sets the scale_metric of this V1beta1TransformerSpec.
 
-        ScaleMetric defines the scaling metric type watched by autoscaler possible values are concurrency, rps, cpu, memory. concurrency, rps are supported via Knative Pod Autoscaler(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics).  # noqa: E501
+        ScaleMetric specifies scaling metric of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-metrics/).  # noqa: E501
 
         :param scale_metric: The scale_metric of this V1beta1TransformerSpec.  # noqa: E501
         :type: str
         """
 
         self._scale_metric = scale_metric
 
     @property
     def scale_target(self):
         """Gets the scale_target of this V1beta1TransformerSpec.  # noqa: E501
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :return: The scale_target of this V1beta1TransformerSpec.  # noqa: E501
         :rtype: int
         """
         return self._scale_target
 
     @scale_target.setter
     def scale_target(self, scale_target):
         """Sets the scale_target of this V1beta1TransformerSpec.
 
-        ScaleTarget specifies the integer target value of the metric type the Autoscaler watches for. concurrency and rps targets are supported by Knative Pod Autoscaler (https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
+        ScaleTarget specifies scaling value of the component concurrency(https://knative.dev/docs/serving/autoscaling/autoscaling-targets/).  # noqa: E501
 
         :param scale_target: The scale_target of this V1beta1TransformerSpec.  # noqa: E501
         :type: int
         """
 
         self._scale_target = scale_target
```

### Comparing `kserve-0.9.0/kserve/models/v1beta1_triton_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_triton_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/models/v1beta1_xg_boost_spec.py` & `kserve-0.9.0rc0/kserve/models/v1beta1_xg_boost_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/rest.py` & `kserve-0.9.0rc0/kserve/rest.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/storage.py` & `kserve-0.9.0rc0/kserve/storage.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/utils/__init__.py` & `kserve-0.9.0rc0/kserve/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/utils/numpy_encoder.py` & `kserve-0.9.0rc0/kserve/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/kserve/utils/utils.py` & `kserve-0.9.0rc0/kserve/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
-from typing import Dict, Union
-
 import psutil
+from typing import Dict, Union
 from cloudevents.http import CloudEvent, to_binary, to_structured
 
 
 def is_running_in_k8s():
     return os.path.isdir('/var/run/secrets/kubernetes.io/')
 
 
@@ -37,18 +36,14 @@
 
 def set_isvc_namespace(inferenceservice):
     isvc_namespace = inferenceservice.metadata.namespace
     namespace = isvc_namespace or get_default_target_namespace()
     return namespace
 
 
-def set_ig_namespace(inferencegraph):
-    return inferencegraph.metadata.namespace or get_default_target_namespace()
-
-
 def cpu_count():
     """Get the available CPU count for this system.
     Takes the minimum value from the following locations:
     - Total system cpus available on the host.
     - CPU Affinity (if set)
     - Cgroups limit (if set)
     """
```

### Comparing `kserve-0.9.0/kserve.egg-info/PKG-INFO` & `kserve-0.9.0rc0/kserve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kserve
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: KServe Python SDK
 Home-page: https://github.com/kserve/kserve/tree/master/python/kserve
 Author: The KServe Authors
 Author-email: ellisbigelow@google.com, hejinchi@cn.ibm.com, dsun20@bloomberg.net
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `kserve-0.9.0/kserve.egg-info/SOURCES.txt` & `kserve-0.9.0rc0/kserve.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -38,21 +38,14 @@
 kserve/models/knative_volatile_time.py
 kserve/models/net_url_userinfo.py
 kserve/models/v1_time.py
 kserve/models/v1alpha1_built_in_adapter.py
 kserve/models/v1alpha1_cluster_serving_runtime.py
 kserve/models/v1alpha1_cluster_serving_runtime_list.py
 kserve/models/v1alpha1_container.py
-kserve/models/v1alpha1_inference_graph.py
-kserve/models/v1alpha1_inference_graph_list.py
-kserve/models/v1alpha1_inference_graph_spec.py
-kserve/models/v1alpha1_inference_graph_status.py
-kserve/models/v1alpha1_inference_router.py
-kserve/models/v1alpha1_inference_step.py
-kserve/models/v1alpha1_inference_target.py
 kserve/models/v1alpha1_model_spec.py
 kserve/models/v1alpha1_serving_runtime.py
 kserve/models/v1alpha1_serving_runtime_list.py
 kserve/models/v1alpha1_serving_runtime_pod_spec.py
 kserve/models/v1alpha1_serving_runtime_spec.py
 kserve/models/v1alpha1_storage_helper.py
 kserve/models/v1alpha1_supported_model_format.py
@@ -119,21 +112,14 @@
 test/test_s3_storage.py
 test/test_server.py
 test/test_storage.py
 test/test_v1alpha1_built_in_adapter.py
 test/test_v1alpha1_cluster_serving_runtime.py
 test/test_v1alpha1_cluster_serving_runtime_list.py
 test/test_v1alpha1_container.py
-test/test_v1alpha1_inference_graph.py
-test/test_v1alpha1_inference_graph_list.py
-test/test_v1alpha1_inference_graph_spec.py
-test/test_v1alpha1_inference_graph_status.py
-test/test_v1alpha1_inference_router.py
-test/test_v1alpha1_inference_step.py
-test/test_v1alpha1_inference_target.py
 test/test_v1alpha1_model_spec.py
 test/test_v1alpha1_serving_runtime.py
 test/test_v1alpha1_serving_runtime_list.py
 test/test_v1alpha1_serving_runtime_pod_spec.py
 test/test_v1alpha1_serving_runtime_spec.py
 test/test_v1alpha1_storage_helper.py
 test/test_v1alpha1_supported_model_format.py
@@ -163,15 +149,14 @@
 test/test_v1beta1_ingress_config.py
 test/test_v1beta1_light_gbm_spec.py
 test/test_v1beta1_logger_spec.py
 test/test_v1beta1_model_copies.py
 test/test_v1beta1_model_format.py
 test/test_v1beta1_model_revision_states.py
 test/test_v1beta1_model_spec.py
-test/test_v1beta1_model_status.py
 test/test_v1beta1_onnx_runtime_spec.py
 test/test_v1beta1_paddle_server_spec.py
 test/test_v1beta1_pmml_spec.py
 test/test_v1beta1_pod_spec.py
 test/test_v1beta1_predictor_config.py
 test/test_v1beta1_predictor_extension_spec.py
 test/test_v1beta1_predictor_protocols.py
```

### Comparing `kserve-0.9.0/setup.py` & `kserve-0.9.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ]
 
 with open('requirements.txt') as f:
     REQUIRES = f.readlines()
 
 setuptools.setup(
     name='kserve',
-    version='0.9.0',
+    version='0.9.0rc0',
     author="The KServe Authors",
     author_email='ellisbigelow@google.com, hejinchi@cn.ibm.com, dsun20@bloomberg.net',
     license="Apache License Version 2.0",
     url="https://github.com/kserve/kserve/tree/master/python/kserve",
     description="KServe Python SDK",
     long_description="Python SDK for KServe Server and Client.",
     python_requires='>=3.7',
```

### Comparing `kserve-0.9.0/test/test_azure_storage.py` & `kserve-0.9.0rc0/test/test_azure_storage.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_creds_utils.py` & `kserve-0.9.0rc0/test/test_creds_utils.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_inference_service_client.py` & `kserve-0.9.0rc0/test/test_inference_service_client.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_knative_addressable.py` & `kserve-0.9.0rc0/test/test_knative_addressable.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_knative_condition.py` & `kserve-0.9.0rc0/test/test_knative_condition.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_knative_url.py` & `kserve-0.9.0rc0/test/test_knative_url.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_knative_volatile_time.py` & `kserve-0.9.0rc0/test/test_knative_volatile_time.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_net_url_userinfo.py` & `kserve-0.9.0rc0/test/test_net_url_userinfo.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_s3_storage.py` & `kserve-0.9.0rc0/test/test_s3_storage.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_server.py` & `kserve-0.9.0rc0/test/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 import avro.schema
 import io
 import pytest
 from cloudevents.http import CloudEvent, to_binary, to_structured
 from kserve import Model
 from kserve import ModelServer
 from kserve import ModelRepository
-from kserve.model import PredictorProtocol
 from tornado.httpclient import HTTPClientError
-from tornado.web import HTTPError
 from ray import serve
 
 
 test_avsc_schema = '''
         {
         "namespace": "example.avro",
          "type": "record",
@@ -157,34 +155,14 @@
             model.load()
             self.update(model)
             return model.ready
         else:
             return False
 
 
-class TestModel:
-
-    async def test_validate(self):
-        model = DummyModel("TestModel")
-        good_request = {"instances": []}
-        validated_request = model.validate(good_request)
-        assert validated_request == good_request
-        bad_request = {"instances": "invalid"}
-        with pytest.raises(HTTPError):
-            model.validate(bad_request)
-
-        model.protocol = PredictorProtocol.REST_V2.value
-        good_request = {"inputs": []}
-        validated_request = model.validate(good_request)
-        assert validated_request == good_request
-        bad_request = {"inputs": "invalid"}
-        with pytest.raises(HTTPError):
-            model.validate(bad_request)
-
-
 class TestTFHttpServer:
 
     @pytest.fixture(scope="class")
     def app(self):  # pylint: disable=no-self-use
         model = DummyModel("TestModel")
         model.load()
         server = ModelServer()
```

### Comparing `kserve-0.9.0/test/test_storage.py` & `kserve-0.9.0rc0/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_built_in_adapter.py` & `kserve-0.9.0rc0/test/test_v1alpha1_built_in_adapter.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_cluster_serving_runtime.py` & `kserve-0.9.0rc0/test/test_v1alpha1_cluster_serving_runtime.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_cluster_serving_runtime_list.py` & `kserve-0.9.0rc0/test/test_v1alpha1_cluster_serving_runtime_list.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_container.py` & `kserve-0.9.0rc0/test/test_v1alpha1_container.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_graph.py` & `kserve-0.9.0rc0/test/test_v1beta1_transformer_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,45 +26,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_graph import V1alpha1InferenceGraph  # noqa: E501
+from kserve.models.v1beta1_transformer_config import V1beta1TransformerConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceGraph(unittest.TestCase):
-    """V1alpha1InferenceGraph unit test stubs"""
+class TestV1beta1TransformerConfig(unittest.TestCase):
+    """V1beta1TransformerConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceGraph
+        """Test V1beta1TransformerConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_graph.V1alpha1InferenceGraph()  # noqa: E501
+        # model = kserve.models.v1beta1_transformer_config.V1beta1TransformerConfig()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceGraph(
-                api_version = '0', 
-                kind = '0', 
-                metadata = None, 
-                spec = None, 
-                status = None
+            return V1beta1TransformerConfig(
+                default_image_version = '0', 
+                image = '0'
             )
         else :
-            return V1alpha1InferenceGraph(
+            return V1beta1TransformerConfig(
+                default_image_version = '0',
+                image = '0',
         )
 
-    def testV1alpha1InferenceGraph(self):
-        """Test V1alpha1InferenceGraph"""
+    def testV1beta1TransformerConfig(self):
+        """Test V1beta1TransformerConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_graph_list.py` & `kserve-0.9.0rc0/test/test_v1alpha1_trained_model_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,59 +26,59 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_graph_list import V1alpha1InferenceGraphList  # noqa: E501
+from kserve.models.v1alpha1_trained_model_list import V1alpha1TrainedModelList  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceGraphList(unittest.TestCase):
-    """V1alpha1InferenceGraphList unit test stubs"""
+class TestV1alpha1TrainedModelList(unittest.TestCase):
+    """V1alpha1TrainedModelList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceGraphList
+        """Test V1alpha1TrainedModelList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_graph_list.V1alpha1InferenceGraphList()  # noqa: E501
+        # model = kserve.models.v1alpha1_trained_model_list.V1alpha1TrainedModelList()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceGraphList(
+            return V1alpha1TrainedModelList(
                 api_version = '0', 
                 items = [
-                    kserve.models.v1alpha1_inference_graph.V1alpha1InferenceGraph(
+                    kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
                         spec = None, 
                         status = None, )
                     ], 
                 kind = '0', 
                 metadata = None
             )
         else :
-            return V1alpha1InferenceGraphList(
+            return V1alpha1TrainedModelList(
                 items = [
-                    kserve.models.v1alpha1_inference_graph.V1alpha1InferenceGraph(
+                    kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
                         spec = None, 
                         status = None, )
                     ],
         )
 
-    def testV1alpha1InferenceGraphList(self):
-        """Test V1alpha1InferenceGraphList"""
+    def testV1alpha1TrainedModelList(self):
+        """Test V1alpha1TrainedModelList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_graph_spec.py` & `kserve-0.9.0rc0/test/test_v1alpha1_model_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,46 +26,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_graph_spec import V1alpha1InferenceGraphSpec  # noqa: E501
+from kserve.models.v1alpha1_model_spec import V1alpha1ModelSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceGraphSpec(unittest.TestCase):
-    """V1alpha1InferenceGraphSpec unit test stubs"""
+class TestV1alpha1ModelSpec(unittest.TestCase):
+    """V1alpha1ModelSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceGraphSpec
+        """Test V1alpha1ModelSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_graph_spec.V1alpha1InferenceGraphSpec()  # noqa: E501
+        # model = kserve.models.v1alpha1_model_spec.V1alpha1ModelSpec()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceGraphSpec(
-                nodes = {
-                    'key' : None
-                    }
+            return V1alpha1ModelSpec(
+                framework = '0', 
+                memory = '0', 
+                storage_uri = '0'
             )
         else :
-            return V1alpha1InferenceGraphSpec(
-                nodes = {
-                    'key' : None
-                    },
+            return V1alpha1ModelSpec(
+                framework = '0',
+                memory = '0', 
+                storage_uri = '0',
         )
 
-    def testV1alpha1InferenceGraphSpec(self):
-        """Test V1alpha1InferenceGraphSpec"""
+    def testV1alpha1ModelSpec(self):
+        """Test V1alpha1ModelSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_graph_status.py` & `kserve-0.9.0rc0/test/test_v1alpha1_trained_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,48 +26,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_graph_status import V1alpha1InferenceGraphStatus  # noqa: E501
+from kserve.models.v1alpha1_trained_model import V1alpha1TrainedModel  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceGraphStatus(unittest.TestCase):
-    """V1alpha1InferenceGraphStatus unit test stubs"""
+class TestV1alpha1TrainedModel(unittest.TestCase):
+    """V1alpha1TrainedModel unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceGraphStatus
+        """Test V1alpha1TrainedModel
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_graph_status.V1alpha1InferenceGraphStatus()  # noqa: E501
+        # model = kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceGraphStatus(
-                annotations = {
-                    'key' : '0'
-                    }, 
-                conditions = [
-                    None
-                    ], 
-                observed_generation = 56, 
-                url = None
+            return V1alpha1TrainedModel(
+                api_version = '0', 
+                kind = '0', 
+                metadata = None, 
+                spec = None, 
+                status = None
             )
         else :
-            return V1alpha1InferenceGraphStatus(
+            return V1alpha1TrainedModel(
         )
 
-    def testV1alpha1InferenceGraphStatus(self):
-        """Test V1alpha1InferenceGraphStatus"""
+    def testV1alpha1TrainedModel(self):
+        """Test V1alpha1TrainedModel"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_router.py` & `kserve-0.9.0rc0/test/test_v1alpha1_storage_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,52 +26,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_router import V1alpha1InferenceRouter  # noqa: E501
+from kserve.models.v1alpha1_storage_helper import V1alpha1StorageHelper  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceRouter(unittest.TestCase):
-    """V1alpha1InferenceRouter unit test stubs"""
+class TestV1alpha1StorageHelper(unittest.TestCase):
+    """V1alpha1StorageHelper unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceRouter
+        """Test V1alpha1StorageHelper
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_router.V1alpha1InferenceRouter()  # noqa: E501
+        # model = kserve.models.v1alpha1_storage_helper.V1alpha1StorageHelper()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceRouter(
-                router_type = '0', 
-                steps = [
-                    kserve.models.v1alpha1_inference_step.V1alpha1InferenceStep(
-                        condition = '0', 
-                        data = '0', 
-                        name = '0', 
-                        node_name = '0', 
-                        service_name = '0', 
-                        service_url = '0', 
-                        weight = 56, )
-                    ]
+            return V1alpha1StorageHelper(
+                disabled = True
             )
         else :
-            return V1alpha1InferenceRouter(
-                router_type = '0',
+            return V1alpha1StorageHelper(
         )
 
-    def testV1alpha1InferenceRouter(self):
-        """Test V1alpha1InferenceRouter"""
+    def testV1alpha1StorageHelper(self):
+        """Test V1alpha1StorageHelper"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_step.py` & `kserve-0.9.0rc0/test/test_v1beta1_batcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,47 +26,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_step import V1alpha1InferenceStep  # noqa: E501
+from kserve.models.v1beta1_batcher import V1beta1Batcher  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceStep(unittest.TestCase):
-    """V1alpha1InferenceStep unit test stubs"""
+class TestV1beta1Batcher(unittest.TestCase):
+    """V1beta1Batcher unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceStep
+        """Test V1beta1Batcher
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_step.V1alpha1InferenceStep()  # noqa: E501
+        # model = kserve.models.v1beta1_batcher.V1beta1Batcher()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceStep(
-                condition = '0', 
-                data = '0', 
-                name = '0', 
-                node_name = '0', 
-                service_name = '0', 
-                service_url = '0', 
-                weight = 56
+            return V1beta1Batcher(
+                max_batch_size = 56, 
+                max_latency = 56, 
+                timeout = 56
             )
         else :
-            return V1alpha1InferenceStep(
+            return V1beta1Batcher(
         )
 
-    def testV1alpha1InferenceStep(self):
-        """Test V1alpha1InferenceStep"""
+    def testV1beta1Batcher(self):
+        """Test V1beta1Batcher"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_inference_target.py` & `kserve-0.9.0rc0/test/test_v1beta1_explainer_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,43 +26,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_inference_target import V1alpha1InferenceTarget  # noqa: E501
+from kserve.models.v1beta1_explainer_config import V1beta1ExplainerConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1InferenceTarget(unittest.TestCase):
-    """V1alpha1InferenceTarget unit test stubs"""
+class TestV1beta1ExplainerConfig(unittest.TestCase):
+    """V1beta1ExplainerConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1InferenceTarget
+        """Test V1beta1ExplainerConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_inference_target.V1alpha1InferenceTarget()  # noqa: E501
+        # model = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig()  # noqa: E501
         if include_optional :
-            return V1alpha1InferenceTarget(
-                node_name = '0', 
-                service_name = '0', 
-                service_url = '0'
+            return V1beta1ExplainerConfig(
+                default_image_version = '0', 
+                image = '0'
             )
         else :
-            return V1alpha1InferenceTarget(
+            return V1beta1ExplainerConfig(
+                default_image_version = '0',
+                image = '0',
         )
 
-    def testV1alpha1InferenceTarget(self):
-        """Test V1alpha1InferenceTarget"""
+    def testV1beta1ExplainerConfig(self):
+        """Test V1beta1ExplainerConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_model_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_model_copies.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 The KServe Authors.
+# Copyright 2022 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,46 +26,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_model_spec import V1alpha1ModelSpec  # noqa: E501
+from kserve.models.v1beta1_model_copies import V1beta1ModelCopies  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1ModelSpec(unittest.TestCase):
-    """V1alpha1ModelSpec unit test stubs"""
+class TestV1beta1ModelCopies(unittest.TestCase):
+    """V1beta1ModelCopies unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1ModelSpec
+        """Test V1beta1ModelCopies
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_model_spec.V1alpha1ModelSpec()  # noqa: E501
+        # model = kserve.models.v1beta1_model_copies.V1beta1ModelCopies()  # noqa: E501
         if include_optional :
-            return V1alpha1ModelSpec(
-                framework = '0', 
-                memory = '0', 
-                storage_uri = '0'
+            return V1beta1ModelCopies(
+                failed_copies = 56, 
+                total_copies = 56
             )
         else :
-            return V1alpha1ModelSpec(
-                framework = '0',
-                memory = '0', 
-                storage_uri = '0',
+            return V1beta1ModelCopies(
+                failed_copies = 56,
         )
 
-    def testV1alpha1ModelSpec(self):
-        """Test V1alpha1ModelSpec"""
+    def testV1beta1ModelCopies(self):
+        """Test V1beta1ModelCopies"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_serving_runtime.py` & `kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_serving_runtime_list.py` & `kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_list.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_serving_runtime_pod_spec.py` & `kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_pod_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_serving_runtime_spec.py` & `kserve-0.9.0rc0/test/test_v1alpha1_serving_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_storage_helper.py` & `kserve-0.9.0rc0/test/test_v1beta1_deploy_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,41 +26,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_storage_helper import V1alpha1StorageHelper  # noqa: E501
+from kserve.models.v1beta1_deploy_config import V1beta1DeployConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1StorageHelper(unittest.TestCase):
-    """V1alpha1StorageHelper unit test stubs"""
+class TestV1beta1DeployConfig(unittest.TestCase):
+    """V1beta1DeployConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1StorageHelper
+        """Test V1beta1DeployConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_storage_helper.V1alpha1StorageHelper()  # noqa: E501
+        # model = kserve.models.v1beta1_deploy_config.V1beta1DeployConfig()  # noqa: E501
         if include_optional :
-            return V1alpha1StorageHelper(
-                disabled = True
+            return V1beta1DeployConfig(
+                default_deployment_mode = '0'
             )
         else :
-            return V1alpha1StorageHelper(
+            return V1beta1DeployConfig(
         )
 
-    def testV1alpha1StorageHelper(self):
-        """Test V1alpha1StorageHelper"""
+    def testV1beta1DeployConfig(self):
+        """Test V1beta1DeployConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1alpha1_supported_model_format.py` & `kserve-0.9.0rc0/test/test_v1alpha1_supported_model_format.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1alpha1_trained_model.py` & `kserve-0.9.0rc0/test/test_v1alpha1_trained_model_spec.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,45 +26,56 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1alpha1_trained_model import V1alpha1TrainedModel  # noqa: E501
+from kserve.models.v1alpha1_trained_model_spec import V1alpha1TrainedModelSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1alpha1TrainedModel(unittest.TestCase):
-    """V1alpha1TrainedModel unit test stubs"""
+class TestV1alpha1TrainedModelSpec(unittest.TestCase):
+    """V1alpha1TrainedModelSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1alpha1TrainedModel
+        """Test V1alpha1TrainedModelSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel()  # noqa: E501
+        # model = kserve.models.v1alpha1_trained_model_spec.V1alpha1TrainedModelSpec()  # noqa: E501
         if include_optional :
-            return V1alpha1TrainedModel(
-                api_version = '0', 
-                kind = '0', 
-                metadata = None, 
-                spec = None, 
-                status = None
+            return V1alpha1TrainedModelSpec(
+                inference_service = '0', 
+                model = kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel(
+                    api_version = '0',
+                    kind = '0',
+                    metadata = None,
+                    spec = None,
+                    status = None
+                )
             )
         else :
-            return V1alpha1TrainedModel(
+            return V1alpha1TrainedModelSpec(
+                inference_service = '0',
+                model = kserve.models.v1alpha1_trained_model.V1alpha1TrainedModel(
+                    api_version = '0',
+                    kind = '0',
+                    metadata = None,
+                    spec = None,
+                    status = None
+                )
         )
 
-    def testV1alpha1TrainedModel(self):
-        """Test V1alpha1TrainedModel"""
+    def testV1alpha1TrainedModelSpec(self):
+        """Test V1alpha1TrainedModelSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_aix_explainer_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_aix_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_alibi_explainer_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_alibi_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_art_explainer_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_art_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_batcher.py` & `kserve-0.9.0rc0/test/test_v1beta1_storage_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 The KServe Authors.
+# Copyright 2022 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,43 +26,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_batcher import V1beta1Batcher  # noqa: E501
+from kserve.models.v1beta1_storage_spec import V1beta1StorageSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1Batcher(unittest.TestCase):
-    """V1beta1Batcher unit test stubs"""
+class TestV1beta1StorageSpec(unittest.TestCase):
+    """V1beta1StorageSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1Batcher
+        """Test V1beta1StorageSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_batcher.V1beta1Batcher()  # noqa: E501
+        # model = kserve.models.v1beta1_storage_spec.V1beta1StorageSpec()  # noqa: E501
         if include_optional :
-            return V1beta1Batcher(
-                max_batch_size = 56, 
-                max_latency = 56, 
-                timeout = 56
+            return V1beta1StorageSpec(
+                key = '0', 
+                parameters = {
+                    'key' : '0'
+                    }, 
+                path = '0', 
+                schema_path = '0'
             )
         else :
-            return V1beta1Batcher(
+            return V1beta1StorageSpec(
         )
 
-    def testV1beta1Batcher(self):
-        """Test V1beta1Batcher"""
+    def testV1beta1StorageSpec(self):
+        """Test V1beta1StorageSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_component_extension_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_component_extension_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_component_status_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_component_status_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_custom_explainer.py` & `kserve-0.9.0rc0/test/test_v1beta1_custom_explainer.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_custom_predictor.py` & `kserve-0.9.0rc0/test/test_v1beta1_custom_predictor.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_custom_transformer.py` & `kserve-0.9.0rc0/test/test_v1beta1_custom_transformer.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_deploy_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_model_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,41 +26,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_deploy_config import V1beta1DeployConfig  # noqa: E501
+from kserve.models.v1beta1_model_format import V1beta1ModelFormat  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1DeployConfig(unittest.TestCase):
-    """V1beta1DeployConfig unit test stubs"""
+class TestV1beta1ModelFormat(unittest.TestCase):
+    """V1beta1ModelFormat unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1DeployConfig
+        """Test V1beta1ModelFormat
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_deploy_config.V1beta1DeployConfig()  # noqa: E501
+        # model = kserve.models.v1beta1_model_format.V1beta1ModelFormat()  # noqa: E501
         if include_optional :
-            return V1beta1DeployConfig(
-                default_deployment_mode = '0'
+            return V1beta1ModelFormat(
+                name = '0', 
+                version = '0'
             )
         else :
-            return V1beta1DeployConfig(
+            return V1beta1ModelFormat(
         )
 
-    def testV1beta1DeployConfig(self):
-        """Test V1beta1DeployConfig"""
+    def testV1beta1ModelFormat(self):
+        """Test V1beta1ModelFormat"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_explainer_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_explainers_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,44 +26,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_explainer_config import V1beta1ExplainerConfig  # noqa: E501
+from kserve.models.v1beta1_explainers_config import V1beta1ExplainersConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1ExplainerConfig(unittest.TestCase):
-    """V1beta1ExplainerConfig unit test stubs"""
+class TestV1beta1ExplainersConfig(unittest.TestCase):
+    """V1beta1ExplainersConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1ExplainerConfig
+        """Test V1beta1ExplainersConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig()  # noqa: E501
+        # model = kserve.models.v1beta1_explainers_config.V1beta1ExplainersConfig()  # noqa: E501
         if include_optional :
-            return V1beta1ExplainerConfig(
-                default_image_version = '0', 
-                image = '0'
+            return V1beta1ExplainersConfig(
+                aix = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig(
+                    default_image_version = '0', 
+                    image = '0', ), 
+                alibi = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig(
+                    default_image_version = '0', 
+                    image = '0', )
             )
         else :
-            return V1beta1ExplainerConfig(
-                default_image_version = '0',
-                image = '0',
+            return V1beta1ExplainersConfig(
         )
 
-    def testV1beta1ExplainerConfig(self):
-        """Test V1beta1ExplainerConfig"""
+    def testV1beta1ExplainersConfig(self):
+        """Test V1beta1ExplainersConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_explainer_extension_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_explainer_extension_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_explainer_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_explainer_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_explainers_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_transformers_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,46 +26,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_explainers_config import V1beta1ExplainersConfig  # noqa: E501
+from kserve.models.v1beta1_transformers_config import V1beta1TransformersConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1ExplainersConfig(unittest.TestCase):
-    """V1beta1ExplainersConfig unit test stubs"""
+class TestV1beta1TransformersConfig(unittest.TestCase):
+    """V1beta1TransformersConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1ExplainersConfig
+        """Test V1beta1TransformersConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_explainers_config.V1beta1ExplainersConfig()  # noqa: E501
+        # model = kserve.models.v1beta1_transformers_config.V1beta1TransformersConfig()  # noqa: E501
         if include_optional :
-            return V1beta1ExplainersConfig(
-                aix = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig(
-                    default_image_version = '0', 
-                    image = '0', ), 
-                alibi = kserve.models.v1beta1_explainer_config.V1beta1ExplainerConfig(
+            return V1beta1TransformersConfig(
+                feast = kserve.models.v1beta1_transformer_config.V1beta1TransformerConfig(
                     default_image_version = '0', 
                     image = '0', )
             )
         else :
-            return V1beta1ExplainersConfig(
+            return V1beta1TransformersConfig(
         )
 
-    def testV1beta1ExplainersConfig(self):
-        """Test V1beta1ExplainersConfig"""
+    def testV1beta1TransformersConfig(self):
+        """Test V1beta1TransformersConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_failure_info.py` & `kserve-0.9.0rc0/test/test_v1beta1_failure_info.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_inference_service.py` & `kserve-0.9.0rc0/test/test_v1beta1_inference_service.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_inference_service_list.py` & `kserve-0.9.0rc0/test/test_v1beta1_inference_service_list.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_inference_service_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_inference_service_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_inference_service_status.py` & `kserve-0.9.0rc0/test/test_v1beta1_inference_service_status.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_inference_services_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_inference_services_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_ingress_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_ingress_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_light_gbm_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_light_gbm_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_logger_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_logger_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_model_copies.py` & `kserve-0.9.0rc0/test/test_v1beta1_pmml_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,43 +26,80 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_model_copies import V1beta1ModelCopies  # noqa: E501
+from kserve.models.v1beta1_pmml_spec import V1beta1PMMLSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1ModelCopies(unittest.TestCase):
-    """V1beta1ModelCopies unit test stubs"""
+class TestV1beta1PMMLSpec(unittest.TestCase):
+    """V1beta1PMMLSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1ModelCopies
+        """Test V1beta1PMMLSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_model_copies.V1beta1ModelCopies()  # noqa: E501
+        # model = kserve.models.v1beta1_pmml_spec.V1beta1PMMLSpec()  # noqa: E501
         if include_optional :
-            return V1beta1ModelCopies(
-                failed_copies = 56, 
-                total_copies = 56
+            return V1beta1PMMLSpec(
+                args = [
+                    '0'
+                    ], 
+                command = [
+                    '0'
+                    ], 
+                env = [
+                    None
+                    ], 
+                env_from = [
+                    None
+                    ], 
+                image = '0', 
+                image_pull_policy = '0', 
+                lifecycle = None, 
+                liveness_probe = None, 
+                name = '0', 
+                ports = [
+                    None
+                    ], 
+                protocol_version = '0', 
+                readiness_probe = None, 
+                resources = None, 
+                runtime_version = '0', 
+                security_context = None, 
+                startup_probe = None, 
+                stdin = True, 
+                stdin_once = True, 
+                storage_uri = '0', 
+                termination_message_path = '0', 
+                termination_message_policy = '0', 
+                tty = True, 
+                volume_devices = [
+                    None
+                    ], 
+                volume_mounts = [
+                    None
+                    ], 
+                working_dir = '0'
             )
         else :
-            return V1beta1ModelCopies(
-                failed_copies = 56,
+            return V1beta1PMMLSpec(
+                storage_uri = '0',
         )
 
-    def testV1beta1ModelCopies(self):
-        """Test V1beta1ModelCopies"""
+    def testV1beta1PMMLSpec(self):
+        """Test V1beta1PMMLSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_model_format.py` & `kserve-0.9.0rc0/test/test_v1beta1_predictor_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,42 +26,48 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_model_format import V1beta1ModelFormat  # noqa: E501
+from kserve.models.v1beta1_predictor_config import V1beta1PredictorConfig  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1ModelFormat(unittest.TestCase):
-    """V1beta1ModelFormat unit test stubs"""
+class TestV1beta1PredictorConfig(unittest.TestCase):
+    """V1beta1PredictorConfig unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1ModelFormat
+        """Test V1beta1PredictorConfig
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_model_format.V1beta1ModelFormat()  # noqa: E501
+        # model = kserve.models.v1beta1_predictor_config.V1beta1PredictorConfig()  # noqa: E501
         if include_optional :
-            return V1beta1ModelFormat(
-                name = '0', 
-                version = '0'
+            return V1beta1PredictorConfig(
+                default_gpu_image_version = '0', 
+                default_image_version = '0', 
+                image = '0',
+                supported_frameworks=['0']
             )
         else :
-            return V1beta1ModelFormat(
+            return V1beta1PredictorConfig(
+                default_gpu_image_version = '0',
+                default_image_version = '0',
+                image = '0',
+                supported_frameworks=['0']
         )
 
-    def testV1beta1ModelFormat(self):
-        """Test V1beta1ModelFormat"""
+    def testV1beta1PredictorConfig(self):
+        """Test V1beta1PredictorConfig"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_model_revision_states.py` & `kserve-0.9.0rc0/test/test_v1beta1_model_revision_states.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_model_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_model_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_model_status.py` & `kserve-0.9.0rc0/test/test_v1beta1_sk_learn_spec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,54 +26,79 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_model_status import V1beta1ModelStatus  # noqa: E501
+from kserve.models.v1beta1_sk_learn_spec import V1beta1SKLearnSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1ModelStatus(unittest.TestCase):
-    """V1beta1ModelStatus unit test stubs"""
+class TestV1beta1SKLearnSpec(unittest.TestCase):
+    """V1beta1SKLearnSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1ModelStatus
+        """Test V1beta1SKLearnSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_model_status.V1beta1ModelStatus()  # noqa: E501
+        # model = kserve.models.v1beta1_sk_learn_spec.V1beta1SKLearnSpec()  # noqa: E501
         if include_optional :
-            return V1beta1ModelStatus(
-                copies = kserve.models.v1beta1_model_copies.V1beta1ModelCopies(
-                    failed_copies = 56, 
-                    total_copies = 56, ), 
-                last_failure_info = kserve.models.v1beta1_failure_info.V1beta1FailureInfo(
-                    location = '0', 
-                    message = '0', 
-                    model_revision_name = '0', 
-                    reason = '0', 
-                    time = None, ), 
-                states = kserve.models.v1beta1_model_revision_states.V1beta1ModelRevisionStates(
-                    active_model_state = '0', 
-                    target_model_state = '0', ), 
-                transition_status = '0'
+            return V1beta1SKLearnSpec(
+                args = [
+                    '0'
+                    ], 
+                command = [
+                    '0'
+                    ], 
+                env = [
+                    None
+                    ], 
+                env_from = [
+                    None
+                    ], 
+                image = '0', 
+                image_pull_policy = '0', 
+                lifecycle = None, 
+                liveness_probe = None, 
+                name = '0', 
+                ports = [
+                    None
+                    ], 
+                readiness_probe = None, 
+                resources = None, 
+                runtime_version = '0', 
+                security_context = None, 
+                startup_probe = None, 
+                stdin = True, 
+                stdin_once = True, 
+                storage_uri = '0', 
+                termination_message_path = '0', 
+                termination_message_policy = '0', 
+                tty = True, 
+                volume_devices = [
+                    None
+                    ], 
+                volume_mounts = [
+                    None
+                    ], 
+                working_dir = '0'
             )
         else :
-            return V1beta1ModelStatus(
-                transition_status = '0',
+            return V1beta1SKLearnSpec(
+                storage_uri = '0',
         )
 
-    def testV1beta1ModelStatus(self):
-        """Test V1beta1ModelStatus"""
+    def testV1beta1SKLearnSpec(self):
+        """Test V1beta1SKLearnSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_onnx_runtime_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_onnx_runtime_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_paddle_server_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_paddle_server_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_pmml_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_torch_serve_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,34 +26,34 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_pmml_spec import V1beta1PMMLSpec  # noqa: E501
+from kserve.models.v1beta1_torch_serve_spec import V1beta1TorchServeSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1PMMLSpec(unittest.TestCase):
-    """V1beta1PMMLSpec unit test stubs"""
+class TestV1beta1TorchServeSpec(unittest.TestCase):
+    """V1beta1TorchServeSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1PMMLSpec
+        """Test V1beta1TorchServeSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_pmml_spec.V1beta1PMMLSpec()  # noqa: E501
+        # model = kserve.models.v1beta1_torch_serve_spec.V1beta1TorchServeSpec()  # noqa: E501
         if include_optional :
-            return V1beta1PMMLSpec(
+            return V1beta1TorchServeSpec(
                 args = [
                     '0'
                     ], 
                 command = [
                     '0'
                     ], 
                 env = [
@@ -62,19 +62,18 @@
                 env_from = [
                     None
                     ], 
                 image = '0', 
                 image_pull_policy = '0', 
                 lifecycle = None, 
                 liveness_probe = None, 
-                name = '0', 
+                name = '0',
                 ports = [
                     None
                     ], 
-                protocol_version = '0', 
                 readiness_probe = None, 
                 resources = None, 
                 runtime_version = '0', 
                 security_context = None, 
                 startup_probe = None, 
                 stdin = True, 
                 stdin_once = True, 
@@ -87,19 +86,19 @@
                     ], 
                 volume_mounts = [
                     None
                     ], 
                 working_dir = '0'
             )
         else :
-            return V1beta1PMMLSpec(
+            return V1beta1TorchServeSpec(
                 storage_uri = '0',
         )
 
-    def testV1beta1PMMLSpec(self):
-        """Test V1beta1PMMLSpec"""
+    def testV1beta1TorchServeSpec(self):
+        """Test V1beta1TorchServeSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_pod_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_pod_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_predictor_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_predictor_protocols.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,48 +26,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_predictor_config import V1beta1PredictorConfig  # noqa: E501
+from kserve.models.v1beta1_predictor_protocols import (
+    V1beta1PredictorProtocols,
+)  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1PredictorConfig(unittest.TestCase):
-    """V1beta1PredictorConfig unit test stubs"""
+
+class TestV1beta1PredictorProtocols(unittest.TestCase):
+    """V1beta1PredictorProtocols unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1PredictorConfig
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = kserve.models.v1beta1_predictor_config.V1beta1PredictorConfig()  # noqa: E501
-        if include_optional :
-            return V1beta1PredictorConfig(
-                default_gpu_image_version = '0', 
-                default_image_version = '0', 
-                image = '0',
-                supported_frameworks=['0']
+        """Test V1beta1PredictorProtocols
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
+        # model = kserve.models.v1beta1_predictor_protocols.V1beta1PredictorProtocols()  # noqa: E501
+        if include_optional:
+            return V1beta1PredictorProtocols(
+                v1=kserve.models.v1beta1_predictor_config.V1beta1PredictorConfig(
+                    default_gpu_image_version="0",
+                    default_image_version="0",
+                    image="0",
+                    supported_frameworks=['0']
+                ),
+                v2=kserve.models.v1beta1_predictor_config.V1beta1PredictorConfig(
+                    default_gpu_image_version="0",
+                    default_image_version="0",
+                    image="0",
+                    supported_frameworks=['0']
+                ),
             )
-        else :
-            return V1beta1PredictorConfig(
-                default_gpu_image_version = '0',
-                default_image_version = '0',
-                image = '0',
-                supported_frameworks=['0']
-        )
+        else:
+            return V1beta1PredictorProtocols()
 
-    def testV1beta1PredictorConfig(self):
-        """Test V1beta1PredictorConfig"""
+    def testV1beta1PredictorProtocols(self):
+        """Test V1beta1PredictorProtocols"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_predictor_extension_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_predictor_extension_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_predictor_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_predictor_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_predictors_config.py` & `kserve-0.9.0rc0/test/test_v1beta1_predictors_config.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_sk_learn_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_triton_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,34 +26,34 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_sk_learn_spec import V1beta1SKLearnSpec  # noqa: E501
+from kserve.models.v1beta1_triton_spec import V1beta1TritonSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1SKLearnSpec(unittest.TestCase):
-    """V1beta1SKLearnSpec unit test stubs"""
+class TestV1beta1TritonSpec(unittest.TestCase):
+    """V1beta1TritonSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1SKLearnSpec
+        """Test V1beta1TritonSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_sk_learn_spec.V1beta1SKLearnSpec()  # noqa: E501
+        # model = kserve.models.v1beta1_triton_spec.V1beta1TritonSpec()  # noqa: E501
         if include_optional :
-            return V1beta1SKLearnSpec(
+            return V1beta1TritonSpec(
                 args = [
                     '0'
                     ], 
                 command = [
                     '0'
                     ], 
                 env = [
@@ -86,19 +86,19 @@
                     ], 
                 volume_mounts = [
                     None
                     ], 
                 working_dir = '0'
             )
         else :
-            return V1beta1SKLearnSpec(
+            return V1beta1TritonSpec(
                 storage_uri = '0',
         )
 
-    def testV1beta1SKLearnSpec(self):
-        """Test V1beta1SKLearnSpec"""
+    def testV1beta1TritonSpec(self):
+        """Test V1beta1TritonSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_storage_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_xg_boost_spec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The KServe Authors.
+# Copyright 2021 The KServe Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,46 +26,79 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kserve
-from kserve.models.v1beta1_storage_spec import V1beta1StorageSpec  # noqa: E501
+from kserve.models.v1beta1_xg_boost_spec import V1beta1XGBoostSpec  # noqa: E501
 from kserve.rest import ApiException
 
-class TestV1beta1StorageSpec(unittest.TestCase):
-    """V1beta1StorageSpec unit test stubs"""
+class TestV1beta1XGBoostSpec(unittest.TestCase):
+    """V1beta1XGBoostSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1beta1StorageSpec
+        """Test V1beta1XGBoostSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kserve.models.v1beta1_storage_spec.V1beta1StorageSpec()  # noqa: E501
+        # model = kserve.models.v1beta1_xg_boost_spec.V1beta1XGBoostSpec()  # noqa: E501
         if include_optional :
-            return V1beta1StorageSpec(
-                key = '0', 
-                parameters = {
-                    'key' : '0'
-                    }, 
-                path = '0', 
-                schema_path = '0'
+            return V1beta1XGBoostSpec(
+                args = [
+                    '0'
+                    ], 
+                command = [
+                    '0'
+                    ], 
+                env = [
+                    None
+                    ], 
+                env_from = [
+                    None
+                    ], 
+                image = '0', 
+                image_pull_policy = '0', 
+                lifecycle = None, 
+                liveness_probe = None, 
+                name = '0', 
+                ports = [
+                    None
+                    ], 
+                readiness_probe = None, 
+                resources = None, 
+                runtime_version = '0', 
+                security_context = None, 
+                startup_probe = None, 
+                stdin = True, 
+                stdin_once = True, 
+                storage_uri = '0', 
+                termination_message_path = '0', 
+                termination_message_policy = '0', 
+                tty = True, 
+                volume_devices = [
+                    None
+                    ], 
+                volume_mounts = [
+                    None
+                    ], 
+                working_dir = '0'
             )
         else :
-            return V1beta1StorageSpec(
+            return V1beta1XGBoostSpec(
+                storage_uri = '0',
         )
 
-    def testV1beta1StorageSpec(self):
-        """Test V1beta1StorageSpec"""
+    def testV1beta1XGBoostSpec(self):
+        """Test V1beta1XGBoostSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kserve-0.9.0/test/test_v1beta1_tf_serving_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_tf_serving_spec.py`

 * *Files identical despite different names*

### Comparing `kserve-0.9.0/test/test_v1beta1_transformer_spec.py` & `kserve-0.9.0rc0/test/test_v1beta1_transformer_spec.py`

 * *Files identical despite different names*


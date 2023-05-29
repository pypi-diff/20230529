# Comparing `tmp/coguard-cli-0.2.8.tar.gz` & `tmp/coguard-cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coguard-cli-0.2.8.tar", last modified: Fri May  5 13:06:22 2023, max compression
+gzip compressed data, was "coguard-cli-0.2.9.tar", last modified: Wed May 24 05:10:38 2023, max compression
```

## Comparing `coguard-cli-0.2.8.tar` & `coguard-cli-0.2.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.8/LICENSE
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/README.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/README_PYPI.md
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.8/pyproject.toml
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/setup.cfg
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.019754 coguard-cli-0.2.8/src/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    30759 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6842 2023-05-03 17:35:40.000000 coguard-cli-0.2.8/src/coguard_cli/__main__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10619 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/api_connection.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-04-24 14:18:39.000000 coguard-cli-0.2.8/src/coguard_cli/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.8/src/coguard_cli/auth/auth_config.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6313 2023-02-24 03:10:28.000000 coguard-cli-0.2.8/src/coguard_cli/auth/token.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/auth/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.019754 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/github/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.026421 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_abc.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2636 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_factory.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3470 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8639 2023-04-12 16:13:07.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.8/src/coguard_cli/docker_dao.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9403 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/folder_scan/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/print_colors.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    18437 2023-05-05 13:06:11.000000 coguard-cli-0.2.8/src/coguard_cli/tests/api_connection_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/auth/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/auth_config_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/common_auth_function_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/auth/token_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.033087 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    26999 2023-05-03 17:35:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/__init__.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.036421 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.039754 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6324 2023-04-12 16:13:07.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.039754 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/common_functions_test.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.043087 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/__init__.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/common_functions_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.8/src/coguard_cli/tests/image_check/docker_dao_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.8/src/coguard_cli/tests/util_test.py
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.8/src/coguard_cli/util.py
-drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-05 13:06:22.023087 coguard-cli-0.2.8/src/coguard_cli.egg-info/
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/PKG-INFO
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6416 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/entry_points.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/requires.txt
--rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-05-05 13:06:22.000000 coguard-cli-0.2.8/src/coguard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1071 2022-06-21 06:40:28.000000 coguard-cli-0.2.9/LICENSE
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8931 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/README.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8748 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/README_PYPI.md
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       84 2022-06-21 06:40:28.000000 coguard-cli-0.2.9/pyproject.toml
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      980 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/setup.cfg
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.241058 coguard-cli-0.2.9/src/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.244391 coguard-cli-0.2.9/src/coguard_cli/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    31377 2023-05-24 04:47:19.000000 coguard-cli-0.2.9/src/coguard_cli/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7036 2023-05-24 04:47:19.000000 coguard-cli-0.2.9/src/coguard_cli/__main__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10684 2023-05-24 04:47:19.000000 coguard-cli-0.2.9/src/coguard_cli/api_connection.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.244391 coguard-cli-0.2.9/src/coguard_cli/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8534 2023-04-24 14:18:39.000000 coguard-cli-0.2.9/src/coguard_cli/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1860 2022-07-03 06:44:40.000000 coguard-cli-0.2.9/src/coguard_cli/auth/auth_config.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7201 2023-05-24 04:47:19.000000 coguard-cli-0.2.9/src/coguard_cli/auth/token.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      269 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/auth/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1011 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      502 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2193 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.241058 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_scripts/
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_scripts/github/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      485 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_scripts/github/github_coguard_action.yml
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-22 20:18:10.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     1431 2023-03-30 03:21:13.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      799 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-24 03:43:49.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5713 2023-03-30 03:21:13.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2078 2023-03-30 03:21:13.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7364 2023-03-30 03:21:13.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2716 2023-03-31 15:08:41.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      232 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/data/versions.tf
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.247724 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4492 2023-03-31 15:08:41.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7608 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finder_abc.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2636 2023-05-05 13:06:11.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finder_factory.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    25095 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6096 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3470 2023-05-05 13:06:11.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4258 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4176 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3668 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6197 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3615 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6035 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3490 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5011 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7401 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7047 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5979 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8639 2023-04-12 16:13:07.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9482 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9241 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3849 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11379 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11573 2023-03-31 15:08:41.000000 coguard-cli-0.2.9/src/coguard_cli/docker_dao.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9403 2023-05-05 13:06:11.000000 coguard-cli-0.2.9/src/coguard_cli/folder_scan/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8557 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      239 2022-06-21 06:45:38.000000 coguard-cli-0.2.9/src/coguard_cli/print_colors.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    18557 2023-05-24 04:47:19.000000 coguard-cli-0.2.9/src/coguard_cli/tests/api_connection_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/auth/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/auth/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      675 2022-06-21 06:45:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/auth/auth_config_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4927 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/tests/auth/common_auth_function_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8441 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/tests/auth/token_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      595 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     2099 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    26999 2023-05-03 17:35:40.000000 coguard-cli-0.2.9/src/coguard_cli/tests/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/__init__.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      640 2023-02-02 14:16:57.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.251058 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-02-02 14:16:57.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8905 2023-02-02 14:16:57.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     4269 2023-02-02 14:16:57.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    11454 2023-03-30 03:21:13.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     3339 2023-01-25 15:30:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)      637 2023-01-25 15:30:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-25 15:30:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13736 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6934 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6597 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5465 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5865 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5736 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5634 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7029 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5883 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6248 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6932 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6899 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6324 2023-04-12 16:13:07.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     8168 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     7506 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5657 2023-02-14 11:54:29.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9100 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/src/coguard_cli/tests/folder_scan/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2023-01-23 19:31:49.000000 coguard-cli-0.2.9/src/coguard_cli/tests/folder_scan/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13956 2023-02-19 03:22:05.000000 coguard-cli-0.2.9/src/coguard_cli/tests/folder_scan/common_functions_test.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.254391 coguard-cli-0.2.9/src/coguard_cli/tests/image_check/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        0 2022-06-21 06:45:38.000000 coguard-cli-0.2.9/src/coguard_cli/tests/image_check/__init__.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    10470 2023-02-24 03:10:28.000000 coguard-cli-0.2.9/src/coguard_cli/tests/image_check/common_functions_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)    13136 2023-02-01 14:06:40.000000 coguard-cli-0.2.9/src/coguard_cli/tests/image_check/docker_dao_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6243 2023-02-23 02:56:51.000000 coguard-cli-0.2.9/src/coguard_cli/tests/util_test.py
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     5506 2023-03-05 05:26:44.000000 coguard-cli-0.2.9/src/coguard_cli/util.py
+drwxr-xr-x   0 aheinle   (1000) aheinle   (1000)        0 2023-05-24 05:10:38.244391 coguard-cli-0.2.9/src/coguard_cli.egg-info/
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     9303 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)     6416 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)        1 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       54 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       62 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/requires.txt
+-rw-r--r--   0 aheinle   (1000) aheinle   (1000)       12 2023-05-24 05:10:38.000000 coguard-cli-0.2.9/src/coguard_cli.egg-info/top_level.txt
```

### Comparing `coguard-cli-0.2.8/LICENSE` & `coguard-cli-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/PKG-INFO` & `coguard-cli-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.8/README.md` & `coguard-cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/README_PYPI.md` & `coguard-cli-0.2.9/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/setup.cfg` & `coguard-cli-0.2.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = coguard-cli
-version = 0.2.8
+version = 0.2.9
 author = Heinle Solutions Inc.
 author_email = albert@coguard.io
 description = A command line interface for scanning configuration files with CoGuard
 long_description = file: README_PYPI.md
 long_description_content_type = text/markdown
 url = https://github.com/coguardio/coguard-cli
 project_urls =
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/__init__.py` & `coguard-cli-0.2.9/src/coguard_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,25 @@
     documentation_candidate = entry["rule"]["documentation"]
     if isinstance(documentation_candidate, str):
         print(wrapper.fill(entry["rule"]["documentation"]))
     else:
         description = documentation_candidate["documentation"]
         remediation = documentation_candidate["remediation"]
         sources = ",\n".join(documentation_candidate["sources"])
+        if "scenarios" in documentation_candidate:
+            scenario_string = "\nReferences for the specific ruleset: " + ",\n".join(
+                documentation_candidate["scenarios"]
+            )
+        else:
+            scenario_string = ''
         documentation_string = f"""
         {description}
 
         Remediation: {remediation}
+        {scenario_string}
 
         Source:
         {sources}
         """.replace("        ", "")
         print(wrapper.fill(documentation_string))
 
 def output_result_json_from_coguard(
@@ -196,15 +203,16 @@
         auth_config: Optional[auth.auth_config.CoGuardCliConfig],
         deal_type,
         token: auth.token.Token,
         coguard_api_url: str,
         scan_identifier: str,
         output_format: str,
         fail_level: int,
-        organization: Optional[str]):
+        organization: Optional[str],
+        ruleset: str):
     """
     The common function to upload a zip file, as generated by the
     helper functions, and evaluate the returned result.
     """
     if zip_candidate is None:
         print(
             f"{COLOR_YELLOW}Unable to identify any known configuration files.{COLOR_TERMINATION}"
@@ -213,22 +221,24 @@
     zip_file, manifest_dict = zip_candidate
     result = api_connection.send_zip_file_for_scanning(
         zip_file,
         auth_config.get_username(),
         token,
         coguard_api_url,
         scan_identifier,
-        organization
+        organization,
+        ruleset
     )
     if result is None:
         print(
             f"{COLOR_RED} An error occurred while scanning. Please file a "
             f"bug report, and include the file located at {zip_file}, if possible. "
             f"{COLOR_TERMINATION}"
         )
+        sys.exit(1)
     logging.debug("The result from the api is: %s",
                   str(result))
     print(f"{COLOR_CYAN}SCANNING OF{COLOR_TERMINATION} {scan_identifier}"
           f" {COLOR_CYAN}COMPLETED{COLOR_TERMINATION}")
     if output_format == 'formatted':
         output_result_json_from_coguard(
             result or {},
@@ -362,15 +372,16 @@
         docker_image: Optional[str],
         auth_config: auth.CoGuardCliConfig,
         deal_type: auth.util.DealEnum,
         token: auth.token.Token,
         organization: str,
         coguard_api_url: Optional[str],
         output_format: str,
-        fail_level: int):
+        fail_level: int,
+        ruleset: str):
     """
     The helper function to run a Docker image scan. It takes in all necessary parameters.
     If the docker-image is None, then all Docker images found on the host system are being
     scanned.
     """
     docker_version = docker_dao.check_docker_version()
     if docker_version is None:
@@ -418,15 +429,16 @@
             auth_config,
             deal_type,
             token,
             coguard_api_url,
             image,
             output_format,
             fail_level,
-            organization
+            organization,
+            ruleset
         )
 
 # pylint: disable=bare-except
 def _find_and_merge_included_docker_images(
         collected_config_file_tuple: Tuple[str, Dict],
         auth_config: auth.CoGuardCliConfig,
         additional_failed_rules: List[str]):
@@ -473,15 +485,16 @@
         folder_name: Optional[str],
         deal_type: auth.util.DealEnum,
         auth_config: auth.CoGuardCliConfig,
         token: auth.token.Token,
         organization: str,
         coguard_api_url: Optional[str],
         output_format: str,
-        fail_level: int):
+        fail_level: int,
+        ruleset: str):
     """
     Helper function to run a scan on a folder. If the folder_name parameter is None,
     the current working directory is being used.
     """
     folder_name = folder_name or "."
     printed_folder_name = os.path.basename(os.path.dirname(folder_name + os.sep))
     print(f"{COLOR_CYAN}SCANNING FOLDER {COLOR_TERMINATION}{printed_folder_name}")
@@ -512,15 +525,16 @@
         auth_config,
         deal_type,
         token,
         coguard_api_url,
         printed_folder_name,
         output_format,
         fail_level,
-        organization
+        organization,
+        ruleset
     )
 
 def perform_folder_fix(
         folder_name: Optional[str],
         deal_type: auth.util.DealEnum,
         token: auth.token.Token,
         organization: str,
@@ -564,15 +578,16 @@
         credentials_file: Optional[str],
         deal_type: auth.util.DealEnum,
         auth_config: auth.CoGuardCliConfig,
         token: auth.token.Token,
         organization: str,
         coguard_api_url: Optional[str],
         output_format: str,
-        fail_level: int):
+        fail_level: int,
+        ruleset: str):
     """
     Helper function to run a scan on a folder. If the folder_name parameter is None,
     the current working directory is being used.
     """
     provider_name = cloud_provider_name or "aws"
     print(f"{COLOR_CYAN}SCANNING CLOUD_PROVIDER {COLOR_TERMINATION}{provider_name}")
     cloud_provider = None
@@ -610,15 +625,16 @@
         auth_config,
         deal_type,
         token,
         coguard_api_url,
         f"{provider_name}_extraction",
         output_format,
         fail_level,
-        organization
+        organization,
+        ruleset
     )
 
 def perform_ci_cd_action(
         ci_cd_provider,
         ci_cd_command,
         repository_folder):
     """
@@ -677,14 +693,15 @@
         return
     auth_config = auth.retrieve_configuration_object(
         arg_coguard_url = args.coguard_api_url,
         arg_auth_url = args.coguard_auth_url
     )
     deal_type = token.extract_deal_type_from_token()
     organization = token.extract_organization_from_token()
+    ruleset = args.ruleset
     logging.debug("Extracted deal type: %s", deal_type)
     logging.debug("Extracted organization: %s", organization)
     if args.subparsers_location == SubParserNames.DOCKER_IMAGE.value:
         if args.image_name:
             docker_image = args.image_name
         elif args.scan:
             # A small hack to keep scan an optional argument.
@@ -695,15 +712,16 @@
             docker_image,
             auth_config,
             deal_type,
             token,
             organization,
             args.coguard_api_url,
             args.output_format,
-            args.fail_level
+            args.fail_level,
+            ruleset
         )
     elif args.subparsers_location == SubParserNames.FOLDER_SCAN.value:
         folder_name = args.folder_name or \
             args.scan or \
             None # args.scan is a trick to
                  # think there is a positional argument
         if folder_name is not None:
@@ -721,30 +739,32 @@
                 folder_name,
                 deal_type,
                 auth_config,
                 token,
                 organization,
                 args.coguard_api_url,
                 args.output_format,
-                args.fail_level
+                args.fail_level,
+                ruleset
             )
     elif args.subparsers_location == SubParserNames.CLOUD_SCAN.value:
         cloud_provider_name = args.cloud_provider_name or args.scan or None
         # args.scan is a trick to
         # think there is a positional argument
         perform_cloud_provider_scan(
             cloud_provider_name,
             args.credentials_file,
             deal_type,
             auth_config,
             token,
             organization,
             args.coguard_api_url,
             args.output_format,
-            args.fail_level
+            args.fail_level,
+            ruleset
         )
     elif args.subparsers_location == SubParserNames.CI_CD_GEN.value:
         ci_cd_provider = args.ci_cd_provider_name
         ci_cd_command = args.ci_cd_command
         if ci_cd_command is None:
             print("No command specified")
             sys.exit(1)
@@ -759,31 +779,34 @@
             None,
             auth_config,
             deal_type,
             token,
             organization,
             args.coguard_api_url,
             args.output_format,
-            args.fail_level
+            args.fail_level,
+            ruleset
         )
         perform_folder_scan(
             None,
             deal_type,
             auth_config,
             token,
             organization,
             args.coguard_api_url,
             args.output_format,
-            args.fail_level
+            args.fail_level,
+            ruleset
         )
         for cloud_provider in ["aws", "azure", "gcp"]:
             perform_cloud_provider_scan(
                 cloud_provider,
                 args.credentials_file,
                 deal_type,
                 auth_config,
                 token,
                 organization,
                 args.coguard_api_url,
                 args.output_format,
-                args.fail_level
+                args.fail_level,
+                ruleset
             )
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/__main__.py` & `coguard-cli-0.2.9/src/coguard_cli/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,22 @@
         '--output-format',
         type=str,
         dest='output_format',
         default='formatted',
         help=("The format of the output. It is either `formatted` (default), "
               "i.e. human readable, or `json`.")
     )
+    parser.add_argument(
+        '--ruleset',
+        type=str,
+        dest='ruleset',
+        choices=["soc2", ""],
+        default='',
+        help=("The non-default rule-set to use.")
+    )
     subparsers = parser.add_subparsers(
         required=True,
         #Do not remove the next line. This is a workaround for https://bugs.python.org/issue29298
         dest='subparsers_location'
     )
     docker_image_parser = subparsers.add_parser(
         SubParserNames.DOCKER_IMAGE.value,
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/api_connection.py` & `coguard-cli-0.2.9/src/coguard_cli/api_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
 def send_zip_file_for_scanning(
         zip_file: str,
         user_name: str,
         auth_token: Token,
         coguard_api_url: str,
         scan_identifier: str,
-        organization: Optional[str]) -> Optional[Dict]:
+        organization: Optional[str],
+        ruleset: str) -> Optional[Dict]:
     """
     The helper function to send a zip file for scanning to the back-end.
     The return value will be an optional dictionary value as per the
     result jsons produced by the coguard engine.
 
     :param zip_file: The path to the zip file.
     :param user_name: The user name associated.
@@ -86,15 +87,15 @@
               scanning.
     """
     with open(zip_file, 'rb') as file_to_send:
         if organization:
             resp_upload = requests.post(
                 (f"{coguard_api_url}/cluster/"
                  f"upload-cluster-zip?organizationName={organization}&"
-                 "overwrite=true"),
+                 f"overwrite=true&compliance={ruleset}"),
                 headers={
                     "Authorization": f'Bearer {auth_token.get_token()}',
                     "Content-Type": "application/octet-stream"
                 },
                 data=file_to_send.read(),
                 timeout=300)
             if resp_upload.status_code != 204:
@@ -129,15 +130,15 @@
                     "Content-Type": "application/json"
                 },
                 timeout=300
             )
         else:
             resp = requests.post(
                 (f"{coguard_api_url}/coguard-cli/"
-                 f"upload-cluster-zip?userName={user_name}"),
+                 f"upload-cluster-zip?userName={user_name}&compliance={ruleset}"),
                 headers={
                     "Authorization": f'Bearer {auth_token.get_token()}',
                     "Content-Type": "application/octet-stream"
                 },
                 data=file_to_send.read(),
                 timeout=300)
     if resp.status_code != 200:
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/auth/__init__.py` & `coguard-cli-0.2.9/src/coguard_cli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/auth/auth_config.py` & `coguard-cli-0.2.9/src/coguard_cli/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/auth/token.py` & `coguard-cli-0.2.9/src/coguard_cli/auth/token.py`

 * *Files 20% similar despite different names*

```diff
@@ -130,15 +130,35 @@
         This is the helper function to extract the organization from the token.
         Returning None if there is no organization.
         """
         public_key = self.get_public_key()
         if not public_key:
             return None
         jwt_decoded = self.get_decoded_jwt_token(public_key)
-        return jwt_decoded.get("organization", None)
+        org_result = jwt_decoded.get("organization", None)
+        if isinstance(org_result, str):
+            return org_result
+        if isinstance(org_result, list) and len(org_result) > 0:
+            if len(org_result) == 1:
+                return org_result[0]
+            input_val = None
+            print("Multiple organizations detected:")
+            print("\n".join(org for org in org_result))
+            while input_val not in org_result:
+                input_val = input(
+                    f"Please type the organization you wish to use (default: {org_result[0]})"
+                )
+                if not input_val.strip():
+                    input_val = org_result[0]
+                if input_val not in org_result:
+                    print("You typed in an invalid organization. Please repeat.")
+            if input_val not in org_result:
+                return None
+            return input_val
+        return None
 
     def extract_deal_type_from_token(
             self
     ) -> util.DealEnum:
         """
         This function uses a token, and a configuruation object, and extracts the deal
         type of the account stored in the JWT token.
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_provider_abc.py` & `coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py` & `coguard-cli-0.2.9/src/coguard_cli/ci_cd/ci_cd_providers/ci_cd_provider_github.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_provider_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_provider_factory.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_aws.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_azure.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/Dockerfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile` & `coguard-cli-0.2.9/src/coguard_cli/discovery/cloud_discovery/terraformer_extract_image_helper/scripts/cmd_for_dfile`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_abc.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finder_abc.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finder_factory.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finder_factory.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/__init__.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_apache.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_aws_cfn.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_docker_compose.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_dockerfile.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_helm.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kafka.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kerberos.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_kubernetes.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_mongodb.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_mysql.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_netlify.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_nginx.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_open_telemetry_collector.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_postgres.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_redis.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_terraform.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py` & `coguard-cli-0.2.9/src/coguard_cli/discovery/config_file_finders/config_file_finder_tomcat.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/docker_dao.py` & `coguard-cli-0.2.9/src/coguard_cli/docker_dao.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/folder_scan/__init__.py` & `coguard-cli-0.2.9/src/coguard_cli/folder_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/image_check/__init__.py` & `coguard-cli-0.2.9/src/coguard_cli/image_check/__init__.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/api_connection_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/api_connection_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             self.assertIsNone(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "baz"),
                 "biz",
                 "zip",
-                None
+                None,
+                ''
             ))
 
     def test_send_zip_file_for_scanning_200_status(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(
@@ -51,15 +52,16 @@
             self.assertDictEqual(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "baz"),
                 "biz",
                 "zip",
-                None
+                None,
+                ''
             ), {"foo": "bar"})
 
     def test_send_zip_file_for_scanning_with_org_non_204_status(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(
@@ -76,15 +78,16 @@
             self.assertIsNone(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "baz"),
                 "biz",
                 "zip",
-                "org"
+                "org",
+                ''
             ))
 
     def test_send_zip_file_for_scanning_with_org_204_failed_run(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(
@@ -105,15 +108,16 @@
             self.assertIsNone(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "token"),
                 "biz",
                 "zip",
-                "org"
+                "org",
+                ''
             ))
 
     def test_send_zip_file_for_scanning_with_org_204_failed_latest_report(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(
@@ -138,15 +142,16 @@
             self.assertIsNone(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "token"),
                 "biz",
                 "zip",
-                "org"
+                "org",
+                ''
             ))
 
     def test_send_zip_file_for_scanning_with_org_204_not_failed_latest_report(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(
@@ -179,15 +184,16 @@
             self.assertDictEqual(api_connection.send_zip_file_for_scanning(
                 "foo",
                 "bar",
                 unittest.mock.Mock(
                     return_value = lambda: "token"),
                 "biz",
                 "zip",
-                "org"
+                "org",
+                ''
             ), {"foo": "bar"})
 
     def test_send_zip_file_for_fixing_non_200_status(self):
         """
         Testing the function and send a non 200 code.
         """
         mock_response = unittest.mock.Mock(status_code = 200)
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/auth/auth_config_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/auth/auth_config_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/auth/common_auth_function_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/auth/common_auth_function_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/auth/token_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/auth/token_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/ci_cd/ci_cd_providers/ci_cd_provider_github_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/common_functions_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_provider_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_aws_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_azure_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/cloud_discovery/cloud_providers/cloud_provider_gcp_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finder_abc_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finder_factory_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_apache_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_docker_compose_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_dockerfile_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_elasticsearch_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_helm_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kafka_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kerberos_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_kubernetes_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mongodb_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_mysql_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_nginx_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_opentelemetry_collector_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_postgres_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_redis_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_terraform_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/discovery/config_file_finders/config_file_finder_tomcat_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/folder_scan/common_functions_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/folder_scan/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/image_check/common_functions_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/image_check/common_functions_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/image_check/docker_dao_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/image_check/docker_dao_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/tests/util_test.py` & `coguard-cli-0.2.9/src/coguard_cli/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli/util.py` & `coguard-cli-0.2.9/src/coguard_cli/util.py`

 * *Files identical despite different names*

### Comparing `coguard-cli-0.2.8/src/coguard_cli.egg-info/PKG-INFO` & `coguard-cli-0.2.9/src/coguard_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coguard-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: A command line interface for scanning configuration files with CoGuard
 Home-page: https://github.com/coguardio/coguard-cli
 Author: Heinle Solutions Inc.
 Author-email: albert@coguard.io
 Project-URL: Bug Tracker, https://github.com/coguardio/coguard-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `coguard-cli-0.2.8/src/coguard_cli.egg-info/SOURCES.txt` & `coguard-cli-0.2.9/src/coguard_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*


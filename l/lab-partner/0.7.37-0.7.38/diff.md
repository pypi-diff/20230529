# Comparing `tmp/lab-partner-0.7.37.tar.gz` & `tmp/lab-partner-0.7.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.37.tar", last modified: Mon May 29 20:28:39 2023, max compression
+gzip compressed data, was "lab-partner-0.7.38.tar", last modified: Mon May 29 20:43:28 2023, max compression
```

## Comparing `lab-partner-0.7.37.tar` & `lab-partner-0.7.38.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.993642 lab-partner-0.7.37/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.961642 lab-partner-0.7.37/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.965642 lab-partner-0.7.37/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-05-29 20:28:03.000000 lab-partner-0.7.37/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 20:28:03.000000 lab-partner-0.7.37/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4298 2023-05-29 20:28:03.000000 lab-partner-0.7.37/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:28:03.000000 lab-partner-0.7.37/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 20:28:39.993642 lab-partner-0.7.37/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 20:28:03.000000 lab-partner-0.7.37/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 20:28:03.000000 lab-partner-0.7.37/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.961642 lab-partner-0.7.37/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.965642 lab-partner-0.7.37/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.965642 lab-partner-0.7.37/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.969642 lab-partner-0.7.37/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 20:28:03.000000 lab-partner-0.7.37/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.961642 lab-partner-0.7.37/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.969642 lab-partner-0.7.37/images/cli/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.973642 lab-partner-0.7.37/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 20:28:03.000000 lab-partner-0.7.37/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-29 20:28:03.000000 lab-partner-0.7.37/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 20:28:03.000000 lab-partner-0.7.37/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 20:28:03.000000 lab-partner-0.7.37/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:28:39.993642 lab-partner-0.7.37/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.961642 lab-partner-0.7.37/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.973642 lab-partner-0.7.37/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.981642 lab-partner-0.7.37/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2677 2023-05-29 20:28:03.000000 lab-partner-0.7.37/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.977642 lab-partner-0.7.37/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 20:28:39.000000 lab-partner-0.7.37/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.981642 lab-partner-0.7.37/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.961642 lab-partner-0.7.37/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.985642 lab-partner-0.7.37/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.985642 lab-partner-0.7.37/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 20:28:03.000000 lab-partner-0.7.37/tools/src/lab_partner_tools/web_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.985642 lab-partner-0.7.37/utils/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/run.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.965642 lab-partner-0.7.37/utils/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:28:39.993642 lab-partner-0.7.37/utils/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 20:28:03.000000 lab-partner-0.7.37/utils/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.072805 lab-partner-0.7.38/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.060805 lab-partner-0.7.38/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-05-29 20:43:03.000000 lab-partner-0.7.38/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 20:43:03.000000 lab-partner-0.7.38/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-05-29 20:43:03.000000 lab-partner-0.7.38/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:43:03.000000 lab-partner-0.7.38/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 20:43:28.072805 lab-partner-0.7.38/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 20:43:03.000000 lab-partner-0.7.38/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 20:43:03.000000 lab-partner-0.7.38/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.060805 lab-partner-0.7.38/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.060805 lab-partner-0.7.38/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.060805 lab-partner-0.7.38/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 20:43:03.000000 lab-partner-0.7.38/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.064805 lab-partner-0.7.38/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.064805 lab-partner-0.7.38/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 20:43:03.000000 lab-partner-0.7.38/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-29 20:43:03.000000 lab-partner-0.7.38/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 20:43:03.000000 lab-partner-0.7.38/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 20:43:03.000000 lab-partner-0.7.38/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:43:28.072805 lab-partner-0.7.38/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.064805 lab-partner-0.7.38/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.068805 lab-partner-0.7.38/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/docker/unix_user.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2677 2023-05-29 20:43:03.000000 lab-partner-0.7.38/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.064805 lab-partner-0.7.38/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 20:43:28.000000 lab-partner-0.7.38/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.068805 lab-partner-0.7.38/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.068805 lab-partner-0.7.38/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.068805 lab-partner-0.7.38/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 20:43:03.000000 lab-partner-0.7.38/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.068805 lab-partner-0.7.38/utils/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/README.md
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/run.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.056805 lab-partner-0.7.38/utils/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:28.072805 lab-partner-0.7.38/utils/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 20:43:03.000000 lab-partner-0.7.38/utils/src/lab_partner_utils/utils.py
```

### Comparing `lab-partner-0.7.37/.github/workflows/build-deploy.yml` & `lab-partner-0.7.38/.github/workflows/build-deploy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/.gitignore` & `lab-partner-0.7.38/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/Dockerfile` & `lab-partner-0.7.38/Dockerfile`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/LICENSE.md` & `lab-partner-0.7.38/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/PKG-INFO` & `lab-partner-0.7.38/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.37
+Version: 0.7.38
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.37/build.sh` & `lab-partner-0.7.38/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/docker-compose.yml` & `lab-partner-0.7.38/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.38/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.38/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.38/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.38/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.38/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/images/cli/bashrc` & `lab-partner-0.7.38/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.38/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/install_from_source.sh` & `lab-partner-0.7.38/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/pyproject.toml` & `lab-partner-0.7.38/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.38/src/lab_partner/docker/daemon_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Dict, Any, List, Optional
 import os
 import json
 
 import click
 
-from . import UnixUser
+from .unix_user import UnixUser
 from ..process_utils import (
     run_process,
     run_process_single_result,
     process_output_as_json
 )
 from ..platform_utils import is_linux
```

### Comparing `lab-partner-0.7.37/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.38/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.38/src/lab_partner/docker/run_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,11 @@
 import os
 from pathlib import Path
 from typing import Optional
-
-
-class UnixUser(object):
-    def __init__(self):
-        self._home = os.environ['HOME']
-        self._username = os.environ['USER']
-        self._uid = str(os.getuid())
-        self._gid = str(os.getgid())
-
-    @property
-    def home(self):
-        return self._home
-
-    @property
-    def username(self):
-        return self._username
-
-    @property
-    def uid(self):
-        return self._uid
-
-    @property
-    def gid(self):
-        return self._gid
-
-    def home_subdir(self, subdir: str) -> str:
-        R"""
-        Returns the path to a subdirectory under the user's home directory on the host system.
-        :param subdir: Subdirectory (e.g. ".ssh")
-        :return: Absolute path to home sub
-        """
-        return os.path.join(self._home, subdir)
+from .unix_user import UnixUser
 
 
 class InvalidDockerOptionConfiguration(Exception):
     pass
 
 
 class DockerRunOptions(object):
```

### Comparing `lab-partner-0.7.37/src/lab_partner/process_utils.py` & `lab-partner-0.7.38/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/src/lab_partner/start_cli.py` & `lab-partner-0.7.38/src/lab_partner/start_cli.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.38/src/lab_partner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.37
+Version: 0.7.38
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.37/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.38/src/lab_partner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/lab_partner.egg-info/entry_points.txt
 src/lab_partner.egg-info/requires.txt
 src/lab_partner.egg-info/top_level.txt
 src/lab_partner/docker/__init__.py
 src/lab_partner/docker/daemon_info.py
 src/lab_partner/docker/rootless_container.py
 src/lab_partner/docker/run_builder.py
+src/lab_partner/docker/unix_user.py
 tools/README.md
 tools/pyproject.toml
 tools/setup.cfg
 tools/src/lab_partner_tools/__init__.py
 tools/src/lab_partner_tools/dist.py
 tools/src/lab_partner_tools/services.py
 tools/src/lab_partner_tools/web_proxy.py
```

### Comparing `lab-partner-0.7.37/tools/pyproject.toml` & `lab-partner-0.7.38/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/tools/setup.cfg` & `lab-partner-0.7.38/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.38/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.38/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.38/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.38/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/LICENSE.md` & `lab-partner-0.7.38/utils/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/pyproject.toml` & `lab-partner-0.7.38/utils/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-0.7.38/utils/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/src/lab_partner_utils/command_builder.py` & `lab-partner-0.7.38/utils/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/src/lab_partner_utils/commands.py` & `lab-partner-0.7.38/utils/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-0.7.38/utils/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.37/utils/src/lab_partner_utils/utils.py` & `lab-partner-0.7.38/utils/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*


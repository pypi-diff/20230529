# Comparing `tmp/lab-partner-0.7.35.tar.gz` & `tmp/lab-partner-0.7.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.35.tar", last modified: Mon May 29 16:27:42 2023, max compression
+gzip compressed data, was "lab-partner-0.7.36.tar", last modified: Mon May 29 17:12:34 2023, max compression
```

## Comparing `lab-partner-0.7.35.tar` & `lab-partner-0.7.36.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.016042 lab-partner-0.7.35/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.972041 lab-partner-0.7.35/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.984042 lab-partner-0.7.35/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2333 2023-05-29 16:27:12.000000 lab-partner-0.7.35/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 16:27:12.000000 lab-partner-0.7.35/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4213 2023-05-29 16:27:12.000000 lab-partner-0.7.35/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 16:27:12.000000 lab-partner-0.7.35/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 16:27:42.016042 lab-partner-0.7.35/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 16:27:12.000000 lab-partner-0.7.35/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 16:27:12.000000 lab-partner-0.7.35/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.972041 lab-partner-0.7.35/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.984042 lab-partner-0.7.35/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.988041 lab-partner-0.7.35/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.988041 lab-partner-0.7.35/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 16:27:12.000000 lab-partner-0.7.35/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.976041 lab-partner-0.7.35/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.992041 lab-partner-0.7.35/images/cli/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.996042 lab-partner-0.7.35/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 16:27:12.000000 lab-partner-0.7.35/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      655 2023-05-29 16:27:12.000000 lab-partner-0.7.35/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 16:27:12.000000 lab-partner-0.7.35/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 16:27:12.000000 lab-partner-0.7.35/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 16:27:42.016042 lab-partner-0.7.35/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.976041 lab-partner-0.7.35/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.996042 lab-partner-0.7.35/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.004042 lab-partner-0.7.35/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2478 2023-05-29 16:27:12.000000 lab-partner-0.7.35/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.004042 lab-partner-0.7.35/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 16:27:41.000000 lab-partner-0.7.35/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.008042 lab-partner-0.7.35/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.980041 lab-partner-0.7.35/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.012042 lab-partner-0.7.35/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.012042 lab-partner-0.7.35/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 16:27:12.000000 lab-partner-0.7.35/tools/src/lab_partner_tools/web_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.012042 lab-partner-0.7.35/utils/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/run.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:41.980041 lab-partner-0.7.35/utils/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:42.016042 lab-partner-0.7.35/utils/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 16:27:12.000000 lab-partner-0.7.35/utils/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.245418 lab-partner-0.7.36/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.221418 lab-partner-0.7.36/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.229418 lab-partner-0.7.36/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-05-29 17:12:09.000000 lab-partner-0.7.36/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 17:12:09.000000 lab-partner-0.7.36/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-05-29 17:12:09.000000 lab-partner-0.7.36/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 17:12:09.000000 lab-partner-0.7.36/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 17:12:34.245418 lab-partner-0.7.36/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 17:12:09.000000 lab-partner-0.7.36/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 17:12:09.000000 lab-partner-0.7.36/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.225418 lab-partner-0.7.36/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.229418 lab-partner-0.7.36/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.229418 lab-partner-0.7.36/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.229418 lab-partner-0.7.36/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 17:12:09.000000 lab-partner-0.7.36/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.225418 lab-partner-0.7.36/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.233418 lab-partner-0.7.36/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.233418 lab-partner-0.7.36/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 17:12:09.000000 lab-partner-0.7.36/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      647 2023-05-29 17:12:09.000000 lab-partner-0.7.36/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 17:12:09.000000 lab-partner-0.7.36/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 17:12:09.000000 lab-partner-0.7.36/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 17:12:34.245418 lab-partner-0.7.36/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.225418 lab-partner-0.7.36/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.237418 lab-partner-0.7.36/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.237418 lab-partner-0.7.36/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2562 2023-05-29 17:12:09.000000 lab-partner-0.7.36/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.237418 lab-partner-0.7.36/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 17:12:34.000000 lab-partner-0.7.36/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.241418 lab-partner-0.7.36/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.225418 lab-partner-0.7.36/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.241418 lab-partner-0.7.36/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.241418 lab-partner-0.7.36/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 17:12:09.000000 lab-partner-0.7.36/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.241418 lab-partner-0.7.36/utils/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/README.md
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/run.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.225418 lab-partner-0.7.36/utils/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:34.241418 lab-partner-0.7.36/utils/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 17:12:09.000000 lab-partner-0.7.36/utils/src/lab_partner_utils/utils.py
```

### Comparing `lab-partner-0.7.35/.github/workflows/build-deploy.yml` & `lab-partner-0.7.36/.github/workflows/build-deploy.yml`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,21 @@
   Build-and-Deploy:
     runs-on: ubuntu-20.04
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Add GITHUB_SHA_SHORT to env
         run: echo "GITHUB_SHA_SHORT=$(echo $GITHUB_SHA | cut -c 1-6)" >> $GITHUB_ENV
+      - name: Add DOCKERHUB_USERNAME to env
+        run: echo "DOCKERHUB_USERNAME=enclarify" >> $GITHUB_ENV
       - name: Login to Docker Hub
+        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: docker/login-action@v2
         with:
-          username: ${{ vars.DOCKERHUB_USERNAME }}
+          username: ${{ env.DOCKERHUB_USERNAME }}
           password: ${{ secrets.DOCKERHUB_TOKEN }}
       - name: Set up Docker Buildx
         uses: docker/setup-buildx-action@v2
       - name: Setup docker build cache
         uses: actions/cache@v2
         with:
           path: /tmp/.buildx-cache
@@ -28,33 +31,35 @@
           cache-to: type=local,dest=/tmp/.buildx-cache
           build-args: |
             LAB_VERSION=${{ github.ref_name }}
           file: ./Dockerfile
           push: false
           load: true
           target: lab_packages
-          tags: ${{ vars.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}
+          tags: ${{ env.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}
       - name: Copy python wheels from docker image
         run: |
-          container_id=$(docker create ${{ vars.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}) \
+          container_id=$(docker create ${{ env.DOCKERHUB_USERNAME }}/lab-partner-packages:${{ github.ref_name }}) \
           && mkdir -p dist \
           && docker cp ${container_id}:/opt/lab/dist/init/. dist/ \
           && docker cp ${container_id}:/opt/lab/dist/utils/. dist/ \
           && docker rm -f ${container_id}
       - name: Publish package distributions to PyPI
+        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           verbose: true
           print-hash: true
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Publish lab cli docker image
+        if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: docker/build-push-action@v4
         with:
           context: .
           cache-from: type=local,src=/tmp/.buildx-cache
           cache-to: type=local,dest=/tmp/.buildx-cache
           build-args: |
             LAB_VERSION=${{ github.ref_name }}
           file: ./Dockerfile
           push: true
           target: lab_cli
-          tags: ${{ vars.DOCKERHUB_USERNAME }}/lab-partner-cli:${{ github.ref_name }}
+          tags: ${{ env.DOCKERHUB_USERNAME }}/lab-partner-cli:${{ github.ref_name }}
```

### Comparing `lab-partner-0.7.35/.gitignore` & `lab-partner-0.7.36/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/Dockerfile` & `lab-partner-0.7.36/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 
 RUN echo "Installing Docker client" \
   && curl -sSL https://download.docker.com/linux/static/stable/$(uname -m)/docker-${DOCKER_VERSION}.tgz > /tmp/docker-latest.tgz \
   && tar -xf /tmp/docker-latest.tgz -C /tmp \
   && cp -R /tmp/docker/* /usr/bin \
   && rm -rf /tmp/docker*
 
+COPY --from=docker/buildx-bin /buildx /usr/libexec/docker/cli-plugins/docker-buildx
+
 RUN echo "Installing Docker Compose" \
   && curl -sSL https://github.com/docker/compose/releases/download/v${DOCKER_COMPOSE_VERSION}/docker-compose-$(uname -s)-$(uname -m) > /usr/bin/docker-compose \
   && chmod +x /usr/bin/docker-compose
 
 RUN echo "Installing act to run github workflows locally" \
   && curl -sSL https://github.com/nektos/act/releases/download/v${ACT_VERSION}/act_$(uname -s)_$(uname -m).tar.gz > /tmp/act.tar.gz \
   && tar -xf /tmp/act.tar.gz -C /tmp \
```

### Comparing `lab-partner-0.7.35/LICENSE.md` & `lab-partner-0.7.36/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/PKG-INFO` & `lab-partner-0.7.36/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.35
+Version: 0.7.36
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.35/build.sh` & `lab-partner-0.7.36/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/docker-compose.yml` & `lab-partner-0.7.36/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.36/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.36/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.36/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.36/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.36/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/images/cli/bashrc` & `lab-partner-0.7.36/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.36/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/install_from_source.sh` & `lab-partner-0.7.36/install_from_source.sh`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 echo "Pushing Docker images to Docker Hub"
 docker push enclarify/lab-partner-cli:$(version)
 #docker push enclarify/lab-partner-jupyter:$(version)
 
 echo "Installing lab-partner on host"
 pip3 install --upgrade --force-reinstall /tmp/lab_partner-$(version)-py3-none-any.whl
 
-#pip3 install --upgrade --force-reinstall lab_partner==0.7.34
+#pip3 install --upgrade --force-reinstall lab_partner
```

### Comparing `lab-partner-0.7.35/pyproject.toml` & `lab-partner-0.7.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.36/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.36/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.36/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/src/lab_partner/process_utils.py` & `lab-partner-0.7.36/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/src/lab_partner/start_cli.py` & `lab-partner-0.7.36/src/lab_partner/start_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         .with_env('LAB_WORKSPACE', WORKSPACE) \
         .with_env('LAB_WORKSPACE_DATA', WORKSPACE_DATA) \
         .with_env('LAB_NETWORK_NAME', NETWORK_NAME) \
         .with_env('LAB_VERSION', version()) \
         .with_bind_mount(user_info.home_subdir('.gitconfig'), '/opt/lab/home/.gitconfig') \
         .with_bind_mount(user_info.home_subdir('.vim'), '/opt/lab/home/.vim') \
         .with_bind_mount(user_info.home_subdir('.vimrc'), '/opt/lab/home/.vimrc') \
+        .with_bind_mount(user_info.home_subdir('.actrc'), '/opt/lab/home/.actrc') \
         .with_bind_mount(user_info.home_subdir('.aws'), '/opt/lab/home/.aws') \
         .with_bind_mount(user_info.home_subdir('.ssh'), '/opt/lab/home/.ssh') \
         .with_bind_mount(WORKSPACE, WORKSPACE) \
         .with_bind_mount(docker_daemon_info.docker_socket(), '/var/run/docker.sock', False) \
         .with_workdir(WORKSPACE)
 
     cmd = shlex.split(cli_cmd.build())
```

### Comparing `lab-partner-0.7.35/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.36/src/lab_partner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.35
+Version: 0.7.36
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.35/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.36/src/lab_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/pyproject.toml` & `lab-partner-0.7.36/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/setup.cfg` & `lab-partner-0.7.36/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.36/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.36/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.36/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.36/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/LICENSE.md` & `lab-partner-0.7.36/utils/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/pyproject.toml` & `lab-partner-0.7.36/utils/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-0.7.36/utils/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/src/lab_partner_utils/command_builder.py` & `lab-partner-0.7.36/utils/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/src/lab_partner_utils/commands.py` & `lab-partner-0.7.36/utils/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-0.7.36/utils/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.35/utils/src/lab_partner_utils/utils.py` & `lab-partner-0.7.36/utils/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*


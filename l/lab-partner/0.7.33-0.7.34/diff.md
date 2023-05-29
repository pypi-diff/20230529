# Comparing `tmp/lab-partner-0.7.33.tar.gz` & `tmp/lab-partner-0.7.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.7.33.tar", last modified: Mon May 29 15:06:37 2023, max compression
+gzip compressed data, was "lab-partner-0.7.34.tar", last modified: Mon May 29 15:09:19 2023, max compression
```

## Comparing `lab-partner-0.7.33.tar` & `lab-partner-0.7.34.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.661715 lab-partner-0.7.33/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.645714 lab-partner-0.7.33/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.649715 lab-partner-0.7.33/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-29 15:06:14.000000 lab-partner-0.7.33/.github/workflows/build-deploy.yml
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 15:06:14.000000 lab-partner-0.7.33/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4000 2023-05-29 15:06:14.000000 lab-partner-0.7.33/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 15:06:14.000000 lab-partner-0.7.33/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 15:06:37.661715 lab-partner-0.7.33/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 15:06:14.000000 lab-partner-0.7.33/README.md
--rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 15:06:14.000000 lab-partner-0.7.33/build.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.645714 lab-partner-0.7.33/environments/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.649715 lab-partner-0.7.33/environments/local/
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.649715 lab-partner-0.7.33/environments/local/telemetry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.649715 lab-partner-0.7.33/environments/local/telemetry/certs/
--rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/certs/demo-data-prepper.crt
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/certs/demo-data-prepper.key
--rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/certs/root-ca.pem
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/certs/test_keystore.p12
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/data-prepper-config.yaml
--rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/otel-collector-config.yml
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 15:06:14.000000 lab-partner-0.7.33/environments/local/telemetry/pipelines.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.645714 lab-partner-0.7.33/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.653715 lab-partner-0.7.33/images/cli/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/cli/bashrc
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/cli/cli_sudoers
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/cli/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/cli/start-cli.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.653715 lab-partner-0.7.33/images/jupyter/
--rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/jupyter/jupyter_lab_config.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/jupyter/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 15:06:14.000000 lab-partner-0.7.33/images/jupyter/start-jupyter.sh
--rwxr-xr-x   0 root         (0) root         (0)      776 2023-05-29 15:06:14.000000 lab-partner-0.7.33/install_from_source.sh
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 15:06:14.000000 lab-partner-0.7.33/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 15:06:14.000000 lab-partner-0.7.33/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 15:06:37.661715 lab-partner-0.7.33/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.645714 lab-partner-0.7.33/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.653715 lab-partner-0.7.33/src/lab_partner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/src/lab_partner/docker/
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/docker/daemon_info.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/docker/rootless_container.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/docker/run_builder.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/process_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     2478 2023-05-29 15:06:14.000000 lab-partner-0.7.33/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 15:06:37.000000 lab-partner-0.7.33/src/lab_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/tools/
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/README.md
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.645714 lab-partner-0.7.33/tools/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/tools/src/lab_partner_tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/src/lab_partner_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/tools/src/lab_partner_tools/compose/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/src/lab_partner_tools/dist.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/src/lab_partner_tools/services.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 15:06:14.000000 lab-partner-0.7.33/tools/src/lab_partner_tools/web_proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.657715 lab-partner-0.7.33/utils/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/README.md
--rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/run.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.649715 lab-partner-0.7.33/utils/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:06:37.661715 lab-partner-0.7.33/utils/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 15:06:14.000000 lab-partner-0.7.33/utils/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.760924 lab-partner-0.7.34/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.744923 lab-partner-0.7.34/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-05-29 15:08:54.000000 lab-partner-0.7.34/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 15:08:54.000000 lab-partner-0.7.34/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-05-29 15:08:54.000000 lab-partner-0.7.34/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 15:08:55.000000 lab-partner-0.7.34/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 15:09:19.760924 lab-partner-0.7.34/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 15:08:55.000000 lab-partner-0.7.34/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 15:08:55.000000 lab-partner-0.7.34/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.744923 lab-partner-0.7.34/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.744923 lab-partner-0.7.34/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.744923 lab-partner-0.7.34/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 15:08:55.000000 lab-partner-0.7.34/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.748924 lab-partner-0.7.34/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.748924 lab-partner-0.7.34/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 15:08:55.000000 lab-partner-0.7.34/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      776 2023-05-29 15:08:55.000000 lab-partner-0.7.34/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 15:08:55.000000 lab-partner-0.7.34/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 15:08:55.000000 lab-partner-0.7.34/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 15:09:19.760924 lab-partner-0.7.34/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.752924 lab-partner-0.7.34/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.752924 lab-partner-0.7.34/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2478 2023-05-29 15:08:55.000000 lab-partner-0.7.34/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.752924 lab-partner-0.7.34/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 15:09:19.000000 lab-partner-0.7.34/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.756924 lab-partner-0.7.34/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.756924 lab-partner-0.7.34/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.756924 lab-partner-0.7.34/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 15:08:55.000000 lab-partner-0.7.34/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.756924 lab-partner-0.7.34/utils/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/README.md
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/run.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.740924 lab-partner-0.7.34/utils/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 15:09:19.756924 lab-partner-0.7.34/utils/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 15:08:55.000000 lab-partner-0.7.34/utils/src/lab_partner_utils/utils.py
```

### Comparing `lab-partner-0.7.33/.github/workflows/build-deploy.yml` & `lab-partner-0.7.34/.github/workflows/build-deploy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -52,10 +52,9 @@
           context: .
           cache-from: type=local,src=/tmp/.buildx-cache
           cache-to: type=local,dest=/tmp/.buildx-cache
           build-args: |
             LAB_VERSION=${{ github.ref_name }}
           file: ./Dockerfile
           push: true
-          load: true
           target: lab_cli
           tags: ${{ vars.DOCKERHUB_USERNAME }}/lab-partner-cli:${{ github.ref_name }}
```

### Comparing `lab-partner-0.7.33/.gitignore` & `lab-partner-0.7.34/.gitignore`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/Dockerfile` & `lab-partner-0.7.34/Dockerfile`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/LICENSE.md` & `lab-partner-0.7.34/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/PKG-INFO` & `lab-partner-0.7.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.33
+Version: 0.7.34
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.33/build.sh` & `lab-partner-0.7.34/build.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/docker-compose.yml` & `lab-partner-0.7.34/environments/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/telemetry/certs/demo-data-prepper.crt` & `lab-partner-0.7.34/environments/local/telemetry/certs/demo-data-prepper.crt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/telemetry/certs/demo-data-prepper.key` & `lab-partner-0.7.34/environments/local/telemetry/certs/demo-data-prepper.key`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/telemetry/certs/root-ca.pem` & `lab-partner-0.7.34/environments/local/telemetry/certs/root-ca.pem`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/telemetry/certs/test_keystore.p12` & `lab-partner-0.7.34/environments/local/telemetry/certs/test_keystore.p12`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/environments/local/telemetry/pipelines.yaml` & `lab-partner-0.7.34/environments/local/telemetry/pipelines.yaml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/images/cli/bashrc` & `lab-partner-0.7.34/images/cli/bashrc`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/images/jupyter/jupyter_lab_config.py` & `lab-partner-0.7.34/images/jupyter/jupyter_lab_config.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/install_from_source.sh` & `lab-partner-0.7.34/install_from_source.sh`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/pyproject.toml` & `lab-partner-0.7.34/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner/docker/daemon_info.py` & `lab-partner-0.7.34/src/lab_partner/docker/daemon_info.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner/docker/rootless_container.py` & `lab-partner-0.7.34/src/lab_partner/docker/rootless_container.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner/docker/run_builder.py` & `lab-partner-0.7.34/src/lab_partner/docker/run_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner/process_utils.py` & `lab-partner-0.7.34/src/lab_partner/process_utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner/start_cli.py` & `lab-partner-0.7.34/src/lab_partner/start_cli.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/src/lab_partner.egg-info/PKG-INFO` & `lab-partner-0.7.34/src/lab_partner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner
-Version: 0.7.33
+Version: 0.7.34
 Summary: A toolkit that partners with you to build software projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-0.7.33/src/lab_partner.egg-info/SOURCES.txt` & `lab-partner-0.7.34/src/lab_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/pyproject.toml` & `lab-partner-0.7.34/tools/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/setup.cfg` & `lab-partner-0.7.34/tools/setup.cfg`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml` & `lab-partner-0.7.34/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/src/lab_partner_tools/dist.py` & `lab-partner-0.7.34/tools/src/lab_partner_tools/dist.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/src/lab_partner_tools/services.py` & `lab-partner-0.7.34/tools/src/lab_partner_tools/services.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/tools/src/lab_partner_tools/web_proxy.py` & `lab-partner-0.7.34/tools/src/lab_partner_tools/web_proxy.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/LICENSE.md` & `lab-partner-0.7.34/utils/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/pyproject.toml` & `lab-partner-0.7.34/utils/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-0.7.34/utils/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/src/lab_partner_utils/command_builder.py` & `lab-partner-0.7.34/utils/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/src/lab_partner_utils/commands.py` & `lab-partner-0.7.34/utils/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-0.7.34/utils/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-0.7.33/utils/src/lab_partner_utils/utils.py` & `lab-partner-0.7.34/utils/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*


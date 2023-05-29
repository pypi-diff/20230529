# Comparing `tmp/lab-partner-0.5.25.tar.gz` & `tmp/lab-partner-0.7.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-0.5.25.tar", last modified: Sun Sep  4 17:18:52 2022, max compression
+gzip compressed data, was "lab-partner-0.7.32.tar", last modified: Mon May 29 14:46:13 2023, max compression
```

## Comparing `lab-partner-0.5.25.tar` & `lab-partner-0.7.32.tar`

### file list

```diff
@@ -1,15 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:18:52.103716 lab-partner-0.5.25/
--rw-r--r--   0 root         (0) root         (0)      473 2022-09-04 17:18:52.103716 lab-partner-0.5.25/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      103 2022-09-03 23:06:23.000000 lab-partner-0.5.25/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)      791 2022-09-04 17:18:52.103716 lab-partner-0.5.25/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:18:52.099716 lab-partner-0.5.25/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:18:52.103716 lab-partner-0.5.25/src/lab_partner/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-08-09 16:52:06.000000 lab-partner-0.5.25/src/lab_partner/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1854 2022-09-03 20:51:35.000000 lab-partner-0.5.25/src/lab_partner/start_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-04 17:18:52.103716 lab-partner-0.5.25/src/lab_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)      473 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      317 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-04 17:18:52.000000 lab-partner-0.5.25/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.812257 lab-partner-0.7.32/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-05-29 14:45:51.000000 lab-partner-0.7.32/.github/workflows/build-deploy.yml
+-rw-r--r--   0 root         (0) root         (0)     3537 2023-05-29 14:45:51.000000 lab-partner-0.7.32/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-05-29 14:45:51.000000 lab-partner-0.7.32/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 14:45:51.000000 lab-partner-0.7.32/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 14:46:13.812257 lab-partner-0.7.32/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-29 14:45:51.000000 lab-partner-0.7.32/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      841 2023-05-29 14:45:51.000000 lab-partner-0.7.32/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/environments/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/environments/local/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/environments/local/telemetry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/environments/local/telemetry/certs/
+-rw-r--r--   0 root         (0) root         (0)      985 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/certs/demo-data-prepper.crt
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/certs/demo-data-prepper.key
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/certs/root-ca.pem
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/certs/test_keystore.p12
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/data-prepper-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/otel-collector-config.yml
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-29 14:45:51.000000 lab-partner-0.7.32/environments/local/telemetry/pipelines.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/images/cli/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/cli/bashrc
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/cli/cli_sudoers
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/cli/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)       35 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/cli/start-cli.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.804257 lab-partner-0.7.32/images/jupyter/
+-rw-r--r--   0 root         (0) root         (0)    33547 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/jupyter/jupyter_lab_config.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/jupyter/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)      363 2023-05-29 14:45:51.000000 lab-partner-0.7.32/images/jupyter/start-jupyter.sh
+-rwxr-xr-x   0 root         (0) root         (0)      776 2023-05-29 14:45:51.000000 lab-partner-0.7.32/install_from_source.sh
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 14:45:51.000000 lab-partner-0.7.32/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      280 2023-05-29 14:45:51.000000 lab-partner-0.7.32/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 14:46:13.812257 lab-partner-0.7.32/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.808257 lab-partner-0.7.32/src/lab_partner/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.808257 lab-partner-0.7.32/src/lab_partner/docker/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/docker/daemon_info.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/docker/rootless_container.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/docker/run_builder.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/process_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     2478 2023-05-29 14:45:51.000000 lab-partner-0.7.32/src/lab_partner/start_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.808257 lab-partner-0.7.32/src/lab_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-29 14:46:13.000000 lab-partner-0.7.32/src/lab_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.808257 lab-partner-0.7.32/tools/
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/README.md
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/tools/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.812257 lab-partner-0.7.32/tools/src/lab_partner_tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/src/lab_partner_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.812257 lab-partner-0.7.32/tools/src/lab_partner_tools/compose/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/src/lab_partner_tools/compose/docker-compose-web-proxy.yml
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/src/lab_partner_tools/dist.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/src/lab_partner_tools/services.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-05-29 14:45:51.000000 lab-partner-0.7.32/tools/src/lab_partner_tools/web_proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.812257 lab-partner-0.7.32/utils/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/README.md
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/run.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.800257 lab-partner-0.7.32/utils/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:46:13.812257 lab-partner-0.7.32/utils/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 14:45:51.000000 lab-partner-0.7.32/utils/src/lab_partner_utils/utils.py
```

### Comparing `lab-partner-0.5.25/setup.cfg` & `lab-partner-0.7.32/tools/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 [metadata]
-name = lab-partner
-version = 0.5.25
+name = lab-partner-tools
+version = 0.5.2
 author = Anthony Schexnaildre
 author_email = aps@enclarify.com
-description = Lab Partner
+description = Lab Partner Tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/enclarify/lab-partner
-project_urls = 
-	Bug Tracker = https://github.com/enclarify/lab-partner/issues
-classifiers = 
-	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
-	Operating System :: OS Independent
-description_file = README.md
-license_files = LICENSE.md
+project_urls =
+    Bug Tracker = https://github.com/enclarify/lab-partner/issues
+classifiers =
+    Programming Language :: Python :: 3
+    License :: OSI Approved :: MIT License
+    Operating System :: OS Independent
+description_file=README.md
+license_files=LICENSE.md
 
 [options]
 package_dir = = src
 packages = find:
-python_requires = >=3.6
-install_requires = 
-	click==8.0.1
+python_requires = >=3.8
+install_requires =
+    click==8.0.1
+    twine==3.4.2
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
-console_scripts = 
-	lab = lab_partner.start_cli:start_cli
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+lab_partner.cli_plugins =
+    services = lab_partner_tools.services:services
+    dist = lab_partner_tools.dist:dist
```


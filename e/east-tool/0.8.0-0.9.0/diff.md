# Comparing `tmp/east-tool-0.8.0.tar.gz` & `tmp/east-tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "east-tool-0.8.0.tar", last modified: Mon Mar 20 13:31:29 2023, max compression
+gzip compressed data, was "east-tool-0.9.0.tar", last modified: Mon Mar 27 07:07:10 2023, max compression
```

## Comparing `east-tool-0.8.0.tar` & `east-tool-0.9.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.409252 east-tool-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.393251 east-tool-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/ISSUE_TEMPLATE/requirement.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/workflows/draft-new-release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-03-20 13:31:15.000000 east-tool-0.8.0/.github/workflows/publish-new-release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-03-20 13:31:15.000000 east-tool-0.8.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/.tox/
--rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:15.000000 east-tool-0.8.0/.tox/.package.lock
--rw-r--r--   0 runner    (1001) docker     (122)     6780 2023-03-20 13:31:15.000000 east-tool-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-20 13:31:15.000000 east-tool-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-20 13:31:29.405252 east-tool-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-03-20 13:31:15.000000 east-tool-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)    11023 2023-03-20 13:31:15.000000 east-tool-0.8.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-03-20 13:31:15.000000 east-tool-0.8.0/docs/development_guide.md
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2023-03-20 13:31:15.000000 east-tool-0.8.0/docs/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (122)     9064 2023-03-20 13:31:15.000000 east-tool-0.8.0/docs/how_east_works.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.397251 east-tool-0.8.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (122)    61164 2023-03-20 13:31:15.000000 east-tool-0.8.0/docs/images/nrf_toolchain_manager_app.png
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-20 13:31:15.000000 east-tool-0.8.0/makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-03-20 13:31:15.000000 east-tool-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-20 13:31:15.000000 east-tool-0.8.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.401252 east-tool-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/Dockerfile_after_sys_setup
--rwxr-xr-x   0 runner    (1001) docker     (122)      277 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/docker_build
--rwxr-xr-x   0 runner    (1001) docker     (122)       97 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/docker_run
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-20 13:31:15.000000 east-tool-0.8.0/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-20 13:31:29.409252 east-tool-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.393251 east-tool-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.401252 east-tool-0.8.0/src/east/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2172 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/configuration-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    15737 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/east_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/east_yml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9686 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.401252 east-tool-0.8.0/src/east/system_commands/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/system_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5470 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/system_commands/sys_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     3246 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/system_commands/util_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.405252 east-tool-0.8.0/src/east/workspace_commands/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/workspace_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/workspace_commands/basic_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    10409 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/workspace_commands/build_type_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)    15309 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/workspace_commands/release_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-03-20 13:31:15.000000 east-tool-0.8.0/src/east/workspace_commands/update_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.405252 east-tool-0.8.0/src/east_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-20 13:31:29.000000 east-tool-0.8.0/src/east_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:29.405252 east-tool-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     8256 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    28923 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/test_build_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    10069 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-03-20 13:31:15.000000 east-tool-0.8.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-03-20 13:31:15.000000 east-tool-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.951484 east-tool-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.943484 east-tool-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/ISSUE_TEMPLATE/requirement.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/workflows/draft-new-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-03-27 07:06:57.000000 east-tool-0.9.0/.github/workflows/publish-new-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-03-27 07:06:57.000000 east-tool-0.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/.tox/
+-rwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:06:57.000000 east-tool-0.9.0/.tox/.package.lock
+-rw-r--r--   0 runner    (1001) docker     (122)     7616 2023-03-27 07:06:57.000000 east-tool-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-27 07:06:57.000000 east-tool-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-27 07:07:10.951484 east-tool-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-03-27 07:06:57.000000 east-tool-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)    11023 2023-03-27 07:06:57.000000 east-tool-0.9.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-03-27 07:06:57.000000 east-tool-0.9.0/docs/development_guide.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-03-27 07:06:57.000000 east-tool-0.9.0/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9064 2023-03-27 07:06:57.000000 east-tool-0.9.0/docs/how_east_works.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (122)    61164 2023-03-27 07:06:57.000000 east-tool-0.9.0/docs/images/nrf_toolchain_manager_app.png
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-03-27 07:06:57.000000 east-tool-0.9.0/makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1016 2023-03-27 07:06:57.000000 east-tool-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-27 07:06:57.000000 east-tool-0.9.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/Dockerfile_after_sys_setup
+-rwxr-xr-x   0 runner    (1001) docker     (122)      277 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/docker_build
+-rwxr-xr-x   0 runner    (1001) docker     (122)       97 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/docker_run
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-27 07:06:57.000000 east-tool-0.9.0/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 07:07:10.951484 east-tool-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.943484 east-tool-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/src/east/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2338 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/configuration-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15751 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/east_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4192 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/east_yml.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10804 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.947484 east-tool-0.9.0/src/east/system_commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/system_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5469 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/system_commands/sys_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/system_commands/util_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.951484 east-tool-0.9.0/src/east/workspace_commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/workspace_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8159 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/workspace_commands/basic_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10407 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/workspace_commands/build_type_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15310 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/workspace_commands/release_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-03-27 07:06:57.000000 east-tool-0.9.0/src/east/workspace_commands/update_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.951484 east-tool-0.9.0/src/east_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1557 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-27 07:07:10.000000 east-tool-0.9.0/src/east_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 07:07:10.951484 east-tool-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8256 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28923 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/test_build_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10069 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-03-27 07:06:57.000000 east-tool-0.9.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-03-27 07:06:57.000000 east-tool-0.9.0/tox.ini
```

### Comparing `east-tool-0.8.0/.github/ISSUE_TEMPLATE/feature-request.md` & `east-tool-0.9.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `east-tool-0.9.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/.github/workflows/draft-new-release.yaml` & `east-tool-0.9.0/.github/workflows/draft-new-release.yaml`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/.github/workflows/publish-new-release.yaml` & `east-tool-0.9.0/.github/workflows/publish-new-release.yaml`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/CHANGELOG.md` & `east-tool-0.9.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,36 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 
 ## [Unreleased]
 
+## [0.9.0] - 2023-03-27
+
+### Added
+
+-   `util rtt` command now supports `--logfile` with which you can specify file
+    into which to store RTT logs (#42).
+-   `debug` command which uses `west debug` or (`west attach`) to connect to the
+    board and start a debugging session.
+
+### Changed
+
+-   Add back functionality to provide `cmake_args` after `--` marker for `build`
+    command. Now it is possible to provide custom `-D` define values to the
+    CMake. Commands `flash`, `bypass` already provided option for extra
+    arguments after `--`, however they did it incorrectly for very edge cases,
+    as they removed double quotes from all arguments passed after `--` marker
+    (#56).
+
+### Fixed
+
+-   Ton of spelling mistakes in the code and comments.
+
 ## [0.8.0] - 2023-03-20
 
 ### Added
 
 -   `compile_commands.json` is now also copied to the top west directory. This 
     enables clangd to work as intended in `ncs` and `zephyr` folders (#53).
 -   Section in docs/configuration.md document describing `release` build type.
@@ -163,15 +185,17 @@
 -   Styling look with rich click module.
 -   Use newer pyproject.toml format for metadata specification.
 -   MIT license file.
 -   Makefile for development.
 -   Docker scripts for building and running docker containers, for development
     purposes.
 
-[Unreleased]: https://github.com/IRNAS/irnas-east-software/compare/v0.8.0...HEAD
+[Unreleased]: https://github.com/IRNAS/irnas-east-software/compare/v0.9.0...HEAD
+
+[0.9.0]: https://github.com/IRNAS/irnas-east-software/compare/v0.8.0...v0.9.0
 
 [0.8.0]: https://github.com/IRNAS/irnas-east-software/compare/v0.7.0...v0.8.0
 
 [0.7.0]: https://github.com/IRNAS/irnas-east-software/compare/v0.6.2...v0.7.0
 
 [0.6.2]: https://github.com/IRNAS/irnas-east-software/compare/v0.6.1...v0.6.2
```

### Comparing `east-tool-0.8.0/LICENSE` & `east-tool-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/PKG-INFO` & `east-tool-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: east-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool built on top of West for managing nRF Connect SDK projects.
 Author-email: Marko Sagadin <marko.sagadin42@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `east-tool-0.8.0/README.md` & `east-tool-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/docs/configuration.md` & `east-tool-0.9.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/docs/development_guide.md` & `east-tool-0.9.0/docs/development_guide.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/docs/getting_started.md` & `east-tool-0.9.0/docs/getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 To view RTT logs:
 
 ```bash
 # Run in first terminal window
 east util connect
 
-# Run in second, new terminal window
+# Run in second, new, terminal window
 east util rtt
 ```
 
 ## Creating a release
 
 `east release` command, performs a release process consisting of a series of
 `east build` commands to build applications and samples listed in the `east.yml`
```

### Comparing `east-tool-0.8.0/docs/how_east_works.md` & `east-tool-0.9.0/docs/how_east_works.md`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/docs/images/nrf_toolchain_manager_app.png` & `east-tool-0.9.0/docs/images/nrf_toolchain_manager_app.png`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/pyproject.toml` & `east-tool-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/scripts/Dockerfile` & `east-tool-0.9.0/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/scripts/Dockerfile_after_sys_setup` & `east-tool-0.9.0/scripts/Dockerfile_after_sys_setup`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/src/east/__main__.py` & `east-tool-0.9.0/src/east/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import click
 import rich_click
 
 from .east_context import EastContext, east_group_settings
 from .system_commands import sys_setup, util
-from .workspace_commands import build, bypass, clean, flash, release, update
+from .workspace_commands import build, bypass, clean, debug, flash, release, update
 
 rich_click.rich_click.MAX_WIDTH = 80
 rich_click.rich_click.USE_RICH_MARKUP = True
 rich_click.rich_click.STYLE_HELPTEXT = "italic dim"
 
 rich_click.rich_click.COMMAND_GROUPS = {
     "east": [
         {
             "name": "Workspace commands",
-            "commands": ["build", "flash", "clean", "update", "bypass", "release"],
+            "commands": [
+                "build",
+                "flash",
+                "clean",
+                "debug",
+                "update",
+                "bypass",
+                "release",
+            ],
         },
         {
             "name": "System commands",
             "commands": ["sys-setup", "util"],
         },
     ],
     "east update": [{"name": "Subcommands", "commands": ["west", "env", "toolchain"]}],
@@ -64,14 +72,15 @@
 cli.add_command(bypass)
 cli.add_command(flash)
 cli.add_command(clean)
 cli.add_command(update)
 cli.add_command(sys_setup)
 cli.add_command(util)
 cli.add_command(release)
+cli.add_command(debug)
 
 
 def main():
     cli()
 
 
 if __name__ == "__main__":
```

### Comparing `east-tool-0.8.0/src/east/configuration-schema.yaml` & `east-tool-0.9.0/src/east/configuration-schema.yaml`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/src/east/constants.py` & `east-tool-0.9.0/src/east/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Path to the toolchain executable, ignore the .exe extension, this works as it should
 NRF_TOOLCHAIN_MANAGER_PATH = os.path.join(EAST_DIR, "nrfutil-toolchain-manager.exe")
 
 # Directory will all Conda stuff
 MINICONDA_DIR = os.path.join(HOME_DIR, "miniconda3")
 
-# Path to the Conda executable, this can be used when the conda is not yet on PATH
+# Path to the Conda executable, this can be used when the Conda is not yet on PATH
 CONDA_PATH = os.path.join(MINICONDA_DIR, "bin", "conda")
 
 const_paths = {
     "home_dir": HOME_DIR,
     "cache_dir": CACHE_DIR,
     "east_dir": EAST_DIR,
     "nrf_toolchain_manager_path": NRF_TOOLCHAIN_MANAGER_PATH,
```

### Comparing `east-tool-0.8.0/src/east/east_context.py` & `east-tool-0.9.0/src/east/east_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     west_topdir,
 )
 
 # Needs to be exposed like this so it can be set to False in tests.
 RICH_CONSOLE_ENABLE_MARKUP = True
 
 """
-Convenience dicts for storing settings that are indentical across Click's commands and
+Convenience dicts for storing settings that are identical across Click's commands and
 groups.
 """
 east_command_settings = {
     "cls": RichCommand,
     "options_metavar": "[options]",
 }
 
@@ -55,15 +55,15 @@
         """Create a new context object.
 
         Args:
             echo (bool): If True `.run` prints the command string to local stdout prior
             to executing it. Default: ``False``.
         """
 
-        # This init will be called on true command invocation, --help flag or similiar
+        # This init will be called on true command invocation, --help flag or similar
         # do not count.
         self.cwd = os.getcwd()
         self.echo = echo
         self.consts = const_paths
 
         # Create EAST_DIR and its parents, if they do not exist
         os.makedirs(self.consts["east_dir"], exist_ok=True)
@@ -151,15 +151,15 @@
 
     def run(
         self,
         command: str,
         exit_on_error: bool = True,
         return_output: bool = False,
         silent: bool = False,
-    ) -> str:
+    ) -> dict:
         """
         Executes given command in shell as a process. This is a blocking call, process
         needs to finish before this command can return;
 
         Args:
             command (str):  Command to execute.
 
@@ -170,25 +170,25 @@
                                     might be no colorcodes in the terminal output and
                                     no strerr, due
                                     to piping.
 
             silent (bool):          Do not print command's output.
 
         Returns:
-            If exit_on_error is False then dict with two keys is returned:
+            Dict with two keys is always returned:
                 output(str):        Contains stdout of the process that run, if
                                     return_output is True, otherwise empty string.
                 returncode(int):    Return code of the process that run
         """
 
         if self.echo:
             self.print_info(command)
 
         if return_output:
-            # Prepare varibale for later assingment
+            # Prepare variable for later assignment
             returncode = None
 
             # This works but it has no color and no stderr
             def execute(cmd, exit_on_error):
                 """Helper function that correctly executes the process and returns
                 output.
                 """
@@ -253,15 +253,15 @@
         Returns:
             Check .run
         """
 
         cmd = f"west {west_command}"
 
         if self.ncs_version_installed:
-            # Run west command as arbitary command through manager
+            # Run west command as arbitrary command through manager
             return self._run_arbi_manager(cmd, **kwargs)
         else:
             return self.run(cmd, **kwargs)
 
     def run_manager(self, command, **kwargs):
         """Executes a command with Nordic's Toolchain manager executable.
 
@@ -276,49 +276,49 @@
             Check .run
         """
         cmd = f"{self.consts['nrf_toolchain_manager_path']} {command}"
 
         return self.run(cmd, **kwargs)
 
     def _run_arbi_manager(
-        self, arbitary_command: str, exit_on_error: bool = True, **kwargs
+        self, arbitrary_command: str, exit_on_error: bool = True, **kwargs
     ):
-        """Run an arbitary command through Nordic's Toolchain Manager
+        """Run an arbitrary command through Nordic's Toolchain Manager
 
-        This method should be used when passing any arbitary command, like west command.
+        This method should be used when passing any arbitrary command, like west command.
 
-        To properly execute an arbitary command and propagate its return code to the
+        To properly execute an arbitrary command and propagate its return code to the
         caller we have do a bit of a bash shell dancing, as Nordic's Toolchain Manager
         does not do this for some commands (if west build fails then return code is not
         propagated, but issuing non-existing command does propagate up).
 
-        What we do is that we run as a total arbitary command following:
+        What we do is that we run as a total arbitrary command following:
 
-            bash -c '{arbitary_command} && touch success.txt'
+            bash -c '{arbitrary_command} && touch success.txt'
 
-        if arbitary_command inside it fails, then `touch success.txt` is not executed.
+        if arbitrary_command inside it fails, then `touch success.txt` is not executed.
 
         So we are checking for success.txt file after every call and exit if it does not
         exist.
 
-        We also need to be carefull what quotes we are using.
+        We also need to be careful what quotes we are using.
 
         Args:
-            arbitary_command (str):
+            arbitrary_command (str):
             **kwargs:
 
         Returns:
             Check .run
         """
 
-        arbitary_command = arbitary_command.replace("'", '"')
+        arbitrary_command = arbitrary_command.replace("'", '"')
 
         cmd = (
             f"{self.consts['nrf_toolchain_manager_path']} launch --ncs-version"
-            f" {self.detected_ncs_version} -- bash -c '{arbitary_command} "
+            f" {self.detected_ncs_version} -- bash -c '{arbitrary_command} "
             "&& touch success.txt'"
         )
 
         # Clean any success.txt file from before
         def cleanup():
             try:
                 os.remove("success.txt")
@@ -334,15 +334,15 @@
         else:
             returncode = 1
             if exit_on_error:
                 self.exit()
 
         cleanup()
 
-        # Patch opver the correct returncode
+        # Patch over the correct returncode
         result["returncode"] = returncode
 
         return result
 
     def check_exe(self, exe: str, on_fail_exit: bool = False) -> bool:
         """
         Checks if the given executable can be found by the which command.
@@ -350,15 +350,15 @@
         If on_fail_exit is true it exits the program.
 
         Args:
             exe (str):              executable to find
             on_fail_exit (bool):    If true it exits cli on exit
 
         Returns:
-            True if given executable was found.
+            True if given executable was found, false otherwise.
         """
         if not which(exe):
             if on_fail_exit:
                 self.exit()
             return False
 
         return True
@@ -366,15 +366,16 @@
     def check_version(self, exe, expected_version, version_cmd="--version"):
         """
         Checks for version of provided exe program and compares it against
         provided one.
 
         """
 
-        # WARN: Checkk version was not yet anywhere, behaviour yet needs to be verified
+        # WARN: Check version is not yet used anywhere, behaviour yet needs to be
+        # verified
         response = self.run(f"{exe} {version_cmd}", silent=True, return_output=True)
 
         return True if expected_version in response["output"] else False
 
     def pre_workspace_command_check(
         self,
         ignore_uninstalled_ncs: bool = False,
@@ -394,15 +395,15 @@
                                             Toolchain Manager. Workspace commands such
                                             as build, flash, clean should set this to
                                             False. Update command should set this to
                                             True.
 
             ignore_unsupported_ncs (bool):  When true, self.does not exit if detected
                                             NCS version is not supported by the
-                                            Toolchain Managaer. Workspace commands such
+                                            Toolchain Manager. Workspace commands such
                                             as build, flash, clean should set this to
                                             True. Update command should set this to
                                             false.
         """
         # Exit if we are not inside west workspace
         if not self.west_dir_path:
             self.print(not_in_west_workspace_msg, highlight=False)
```

### Comparing `east-tool-0.8.0/src/east/east_yml.py` & `east-tool-0.9.0/src/east/east_yml.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return (
         "An [bold red]error[/] occurred when trying to load [bold yellow]east.yml[/]"
         f" file!\n\n[italic yellow]{exception_msg}[/]\n"
     )
 
 
 def load_east_yml(project_dir: str):
-    """Try to load east.yml. If that succeds validate it.
+    """Try to load east.yml. If that succeeds validate it.
 
         project_dir (str): Path to project directory, where east.yml should be located.
 
     Returns:
         dict with east.yml contents if east.yml is found and correctly validated. If it
         can not be found it returns None.
```

### Comparing `east-tool-0.8.0/src/east/helper_functions.py` & `east-tool-0.9.0/src/east/helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,25 +93,25 @@
                 progress.update(task_id, advance=len(chunk))
                 f.write(chunk)
 
 
 def download_files(urls: List[str], dest_dir: str) -> List[str]:
     """Download concurrently multiple files from the internet to the given directory.
 
-    Function expects a list of urls that point to the files.
+    Function expects a list of URLs that point to the files.
 
     After all files were downloaded the function returns a list of paths to the
     downloaded files in the same order as they were given.
 
-    Downloaded files are not renamed, they have the same name as in the url. Only
+    Downloaded files are not renamed, they have the same name as in the URL. Only
     exception to this rule are raw files from the GitHub, they end with '?raw=true', so
     that part is removed.
 
     Args:
-        urls (List[strl]):      Url that points to a file to be downloaded.
+        urls (List[strl]):      URL that points to a file to be downloaded.
 
     Return:
         files (List[str]):      List of paths to the downloaded files.
     """
 
     file_paths = []
 
@@ -302,7 +302,36 @@
     hw_versions = [
         ".".join(m.split(".")[0].replace(west_board, "").split("_")[1:])
         for m in matches
     ]
     boards = ["@".join([west_board, hw]) for hw in sorted(hw_versions)]
 
     return boards if boards else [west_board]
+
+
+def clean_up_extra_args(args):
+    """
+    Clean up extra args, by adding back double quotes to the define assignments.
+
+    Click argument automatically strips double quotes from anything that is given
+    after "--". We can not know for sure from where double quotes were removed,
+    however we know that CMake in at least one case requires them.
+    For example, double quotes are needed, if you are assigning a list of tokens to the
+    define value, like so: -DFILES="file1.txt;file2.txt".
+    Double quotes are also added if there is an assignment to a flag, like:
+    --some-flag=something.
+    If this line gets to Cmake without double quotes, it will not be parsed
+    correctly.
+
+        args ():    Extra args, passed after '--' as Click argument.
+
+    Returns:
+        cleaned up args, already formatted as a string.
+    """
+
+    def add_back_double_quotes(arg):
+        if (arg.startswith("-D") or arg.startswith("--")) and "=" in arg:
+            split = arg.split("=")
+            arg = f'{split[0]}="{split[1]}"'
+        return arg
+
+    return f"{' '.join(list(map(add_back_double_quotes, args)))}"
```

### Comparing `east-tool-0.8.0/src/east/system_commands/sys_setup.py` & `east-tool-0.9.0/src/east/system_commands/sys_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from ..constants import NRF_TOOLCHAIN_MANAGER_PATH
 from ..east_context import EastContext, east_command_settings
 from ..helper_functions import check_python_version, download_files
 
 
 def _get_conda_download_link():
-    """Construct download link for conda installer script based on system python
+    """Construct download link for Conda installer script based on system python
     version"""
 
-    # Link to the conda installer script. Two big Xs will be later replaced with python
+    # Link to the Conda installer script. Two big Xs will be later replaced with python
     # version, like 39 or 38.
     link = "https://repo.anaconda.com/miniconda/Miniconda3-pyXX_4.12.0-Linux-x86_64.sh"
     py_ver = str(sys.version_info.major) + str(sys.version_info.minor)
     return re.sub("XX", py_ver, link)
 
 
 def _install_conda(east: EastContext, installer_path: str):
@@ -80,15 +80,15 @@
 • source ~/.zshrc
 • source ~/.config/fish/config.fish
 """
 
 toolchain_installed_msg = """
 [bold green]Nordic's Toolchain Manager install done![/]
 
-East will now smartly use Nordic's Toolechain Manager whenever it can.
+East will now smartly use Nordic's Toolchain Manager whenever it can.
 
 [bold]Note:[/] You still need to run [italic bold blue]east update toolchain[/] inside
 of a [yellow bold]West workspace[/] to get the actual toolchain.
 """
 
 packages = [
     {
```

### Comparing `east-tool-0.8.0/src/east/system_commands/util_commands.py` & `east-tool-0.9.0/src/east/system_commands/util_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 @click.pass_obj
 def connect(east, device, jlink_id, rtt_port):
 
     """Connects to a device and creates a RTT server with [bold cyan]JLinkExe[/].
 
 
     \b
-    \n\nRTT server will emmit any RTT messages produced by the device over its dedicated port. Execute [bold magenta]east util rtt[/] command in the separate window to observe these messages.
+    \n\nRTT server will emit any RTT messages produced by the device over its dedicated port. Execute [bold magenta]east util rtt[/] command in the separate window to observe these messages.
 
     """
 
     if not east.check_exe("JLinkExe"):
         east.print(no_jlink_tool_msg("JLinkExe"), highlight=False)
         east.exit()
 
@@ -93,34 +93,45 @@
 @click.option(
     "-p",
     "--rtt-port",
     type=int,
     default=19021,
     help=("Sets the RTT Telnet port. Default: 19021."),
 )
+@click.option(
+    "-l",
+    "--logfile",
+    type=str,
+    help="Relative path to a log file into which to save RTT output.",
+)
 @click.pass_obj
-def rtt(east, local_echo, rtt_port):
+def rtt(east, local_echo, rtt_port, logfile):
     """Runs a RTT client which connects to a running RTT server.
 
 
     \b
     \n\nAny messages that RTT server creates are printed. RTT server can be created with an [bold magenta]east util connect[/] command.
     """
 
     if not east.check_exe("JLinkRTTClient"):
         east.print(no_jlink_tool_msg("JLinkRTTClient"), highlight=False)
         east.exit()
 
     local_echo = "On" if local_echo else "Off"
 
-    east.run(f"JLinkRTTClient -LocalEcho {local_echo} -RTTTelnetPort {rtt_port}")
+    rtt_cmd = f"JLinkRTTClient -LocalEcho {local_echo} -RTTTelnetPort {rtt_port} "
+
+    if logfile:
+        rtt_cmd += f"| tee {logfile}"
+
+    east.run(rtt_cmd)
 
 
 @click.group(**east_group_settings, subcommand_metavar="Subcommands")
 @click.pass_obj
-def util(east):
+def util(_):
     """Command with several subcommands related to utilities."""
     pass
 
 
 util.add_command(connect)
 util.add_command(rtt)
```

### Comparing `east-tool-0.8.0/src/east/workspace_commands/basic_commands.py` & `east-tool-0.9.0/src/east/workspace_commands/basic_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import shutil as sh
 
 import click
 
 from ..east_context import east_command_settings
+from ..helper_functions import clean_up_extra_args
 from .build_type_flag import construct_extra_cmake_arguments
 
 
 @click.command(**east_command_settings)
 @click.pass_obj
 def clean(east):
     """Clean the build folder in current directory.
@@ -40,26 +41,26 @@
         "Build directory to create or use. If the --build-dir directory is not set, the"
         " default is [bold]build[/] unless the build.dir-fmt configuration variable is"
         " set. The current directory is checked after that. If either is a Zephyr build"
         " directory, it is used. "
     ),
 )
 @click.option("-t", "--target", type=str, help="Run this build system target.")
-# @click.argument("cmake-args", nargs=-1, type=str, metavar="-- [cmake-args]")
+@click.argument("cmake-args", nargs=-1, type=str, metavar="-- [cmake-args]")
 @click.option(
     "-s",
     "--source-dir",
     type=str,
     help=(
         "Relative path to a directory that should be used as application source"
         " directory."
     ),
 )
 @click.pass_obj
-def build(east, board, build_type, build_dir, target, source_dir):
+def build(east, board, build_type, build_dir, target, source_dir, cmake_args):
     """
     Build firmware in the current directory.
 
     \b
     \n\nInternally runs [magenta bold]west build[/] command in current directory if --source-dir is not set.
 
     \n\nTo pass additional arguments to the [bold]CMake[/] invocation performed by the [magenta
@@ -76,15 +77,15 @@
 
     \n\n[bold]Note:[/] This command can be only run from inside of a [bold yellow]West workspace[/].
     """
 
     east.pre_workspace_command_check()
 
     build_cmd = create_build_command(
-        east, board, build_type, build_dir, target, source_dir
+        east, board, build_type, build_dir, target, source_dir, cmake_args
     )
 
     east.run_west(build_cmd)
 
     compile_file = os.path.join("build", "compile_commands.json")
     if os.path.isfile(compile_file):
         sh.copyfile(
@@ -98,45 +99,52 @@
 def create_build_command(
     east,
     board=None,
     build_type=None,
     build_dir=None,
     target=None,
     source_dir=None,
+    cmake_args=None,
     silence_diagnostic=False,
 ):
-    """Creates build command. This is needed so it can also be reused by release command"""
-    build_cmd = "build"
-
-    if board:
-        build_cmd += f" -b {board}"
-    if build_dir:
-        build_cmd += f" -d {build_dir}"
-    if target:
-        build_cmd += f" -t {target}"
-    if source_dir:
-        build_cmd += f" {source_dir}"
-
-    # WARN: cmake args are making some problems in this form.
-    # if cmake_args:
-    #     build_cmd += f" -- \"{' '.join(cmake_args)}\""
+    """Helper for creating a build command. This extra helper is needed so it can also
+    be reused by release command.
+    """
 
     build_type_args, diagnostic = construct_extra_cmake_arguments(
         east,
         build_type,
         board,
         build_dir,
         source_dir,
     )
 
     if diagnostic and not silence_diagnostic:
         east.print(diagnostic)
 
+    build_cmd = "build"
+
+    if board:
+        build_cmd += f" -b {board}"
+    if build_dir:
+        build_cmd += f" -d {build_dir}"
+    if target:
+        build_cmd += f" -t {target}"
+    if source_dir:
+        build_cmd += f" {source_dir}"
+
+    # Some flags need to be passed as extra parameters to the west tool
+    if build_type_args or cmake_args:
+        build_cmd += " --"
+
     if build_type_args:
-        build_cmd += f" -- {build_type_args}"
+        build_cmd += f" {build_type_args}"
+
+    if cmake_args:
+        build_cmd += f" {clean_up_extra_args(cmake_args)}"
 
     return build_cmd
 
 
 @click.command(**east_command_settings)
 @click.option("-d", "--build-dir", type=str, help="Build directory to create or use.")
 @click.option(
@@ -180,24 +188,20 @@
     flash_cmd = "flash "
 
     if build_dir:
         flash_cmd += f"-d {build_dir} "
     if runner:
         flash_cmd += f"-r {runner} "
 
-    # Some flags need to be passed as extra parameters to the west tool
-    if verify or jlink_id or extra_args:
-        flash_cmd += "-- "
-
     if verify:
         flash_cmd += "--verify "
     if jlink_id:
         flash_cmd += f"-i {jlink_id} "
     if extra_args:
-        flash_cmd += f"\"{' '.join(extra_args)}\" "
+        flash_cmd += f" {clean_up_extra_args(extra_args)}"
 
     east.run_west(flash_cmd)
 
 
 @click.command(**east_command_settings)
 @click.argument("args", nargs=-1, type=str, metavar="-- [args]")
 @click.pass_obj
@@ -219,18 +223,52 @@
     \n\n[bold]Note:[/] This command can be only run from inside of a [bold yellow]West workspace[/].
     """
     east.pre_workspace_command_check()
 
     if not args:
         east.exit()
 
-    # Click argument automatically strips double quotes from anything that is given
-    # after "--". Double quotes are needed if specifying define values (-D) to the cmake
-    # args, below list comprehension adds them back.
-    def add_back_double_quotes(arg):
-        splited = arg.split("=")
-        return f'{splited[0]}="{splited[1]}"'
+    cmd = clean_up_extra_args(args)
+
+    east.run_west(cmd)
+
+
+@click.command(**east_command_settings)
+@click.pass_obj
+@click.option(
+    "-t",
+    "--tui",
+    is_flag=True,
+    help="If given GDB uses Text User Interface",
+)
+@click.option(
+    "-a",
+    "--attach",
+    is_flag=True,
+    help=(
+        "If given only connect to the board and start a debugging session, skip "
+        "flashing (uses [bold magenta]west attach[/] instead of [bold magenta]west "
+        "debug[/])."
+    ),
+)
+@click.argument("extra_args", nargs=-1, type=str, metavar="-- [args]")
+def debug(east, tui, attach, extra_args):
+    """Connect to the board, flash the program, and start a debugging session.
+
+    \b
+    \n\nPassing any set of commands after double dash [bold]--[/] will pass them directly to
+    the [bold magenta]west[/] tool (run east debug -- --help to see all possible options).
+
 
-    args = [add_back_double_quotes(arg) if "=" in arg else arg for arg in args]
+    \n\n[bold]Note:[/] This command can be only run from inside of a [bold yellow]West workspace[/].
+    """
+    east.pre_workspace_command_check()
+
+    cmd = "attach " if attach else "debug "
+
+    if tui:
+        cmd += "--tui "
+
+    if extra_args:
+        cmd += f"{clean_up_extra_args(extra_args)} "
 
-    cmd = f"{' '.join(args)} "
     east.run_west(cmd)
```

### Comparing `east-tool-0.8.0/src/east/workspace_commands/build_type_flag.py` & `east-tool-0.9.0/src/east/workspace_commands/build_type_flag.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     prefix = f"{path_prefix}/" if path_prefix else ""
     # We always use common.conf
     cmake_args = f"-DCONF_FILE={prefix}conf/common.conf"
 
     overlay_configs = []
 
     # If a west board is given search for board specific config file and add it to the
-    # the start of overlay_configs, if it is found.
+    # start of overlay_configs, if it is found.
     if board:
         # Sanitize the board input, user might gave hv version
         board = board.split("@")[0]
 
         # Location of the board file depends on the source_dir and prefix
         board_prefix = f"{source_dir}/{prefix}" if source_dir else f"{prefix}"
         board_conf = f"{board_prefix}conf/{board}.conf"
@@ -113,15 +113,15 @@
 [bold yellow]east.yml[/] not found in project's root directory, option [bold
 cyan]-/u--build-type[/] needs it to determine [bold]Kconfig[/] overlay files, exiting!"""
 
 build_type_misuse_msg = """
 Option [bold cyan]--build-type[/] can only be used inside of the application folder, exiting!"""
 
 build_type_misuse_no_app_msg = """
-Option [bold cyan]--build-type[/] can only be used when apps key in [bold yellow]east.yml[/] has atleast one
+Option [bold cyan]--build-type[/] can only be used when apps key in [bold yellow]east.yml[/] has at least one
 application entry!"""
 
 
 def no_build_type_msg(build_type):
     return (
         f"\nGiven --build-type [bold]{build_type}[/] does [bold red]not"
         " exist[/] for this app!"
@@ -162,15 +162,15 @@
             # west behaviour: no cmake args
             return ("", "")
         else:
             east.print(build_type_misuse_no_east_yml_msg)
             east.exit()
 
     # Modify current working dir, if source_dir is used, rstrip is needed cause
-    # path.join adds one "/" if joning empty string.
+    # path.join adds one "/" if joining empty string.
     source_dir = source_dir if source_dir else ""
     cwd = os.path.join(east.cwd, source_dir).rstrip("/")
 
     # Does the relative path contain app or samples string
     relpath = os.path.relpath(cwd, start=east.project_dir)
     inside_app = "app" in relpath
     inside_sample = "samples" in relpath
```

### Comparing `east-tool-0.8.0/src/east/workspace_commands/release_commands.py` & `east-tool-0.9.0/src/east/workspace_commands/release_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     east ():            East context.
     job ():             Job to run.
     dry_run ():         If true then don't actually build, only show what commands
                         would run.
     verbose():          If true the Cmake output is shown.
 
     Return:
-        Bool            True, if job succeded, false if it did not.
+        Bool            True, if job succeeded, false if it did not.
     """
 
     build_cmd = create_build_command(
         east,
         board=job["board"],
         build_type=job["build_type"],
         source_dir=job["src_dir"],
@@ -288,15 +288,15 @@
     apps = east.east_yml.get("apps", [])
     samples = east.east_yml.get("samples", [])
 
     # We inject app and samples with additional key/value pairs in below two for loops
     # so the logic afterwards for detection of jobs can be common/simpler.
     # We also do some existence checks.
 
-    # Small adjusment for projects which only have one single app
+    # Small adjustment for projects which only have one single app
     apps_in_dir = apps[0]["name"] if len(apps) == 1 else os.listdir("app")
 
     for app in apps:
         # Check, if the app even exists before building for it
         if app["name"] not in apps_in_dir:
             east.print(non_existing_app_msg_fmt(app["name"]))
             east.exit()
@@ -312,15 +312,15 @@
             east.print(non_existing_sample_msg_fmt(sample["name"]))
             east.exit()
         # Add parent to mark from where this key comes from
         sample.update({"parent": "samples"})
         # Add "release" build type which for samples does nothing.
         sample.update({"build-types": [{"type": None}]})
 
-    # Apps and samples become targets, which can be handled in similiar way.
+    # Apps and samples become targets, which can be handled in similar way.
     targets = apps + samples
 
     jobs = []
     for target in targets:
         for board in target["west-boards"]:
             for board in find_all_boards(east, board):
                 # Extract build type names from dictionaries
```

### Comparing `east-tool-0.8.0/src/east/workspace_commands/update_commands.py` & `east-tool-0.9.0/src/east/workspace_commands/update_commands.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/src/east_tool.egg-info/PKG-INFO` & `east-tool-0.9.0/src/east_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: east-tool
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool built on top of West for managing nRF Connect SDK projects.
 Author-email: Marko Sagadin <marko.sagadin42@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `east-tool-0.8.0/src/east_tool.egg-info/SOURCES.txt` & `east-tool-0.9.0/src/east_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/conftest.py` & `east-tool-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/helpers.py` & `east-tool-0.9.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/test_build_type.py` & `east-tool-0.9.0/tests/test_build_type.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/test_clean.py` & `east-tool-0.9.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/test_configuration.py` & `east-tool-0.9.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `east-tool-0.8.0/tests/test_release.py` & `east-tool-0.9.0/tests/test_release.py`

 * *Files identical despite different names*


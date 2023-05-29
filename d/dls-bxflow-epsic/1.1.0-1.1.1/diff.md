# Comparing `tmp/dls-bxflow-epsic-1.1.0.tar.gz` & `tmp/dls-bxflow-epsic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-epsic-1.1.0.tar", last modified: Thu Feb 16 12:39:07 2023, max compression
+gzip compressed data, was "dls-bxflow-epsic-1.1.1.tar", last modified: Mon May 29 17:00:59 2023, max compression
```

## Comparing `dls-bxflow-epsic-1.1.0.tar` & `dls-bxflow-epsic-1.1.1.tar`

### file list

```diff
@@ -1,109 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.636076 dls-bxflow-epsic-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.616077 dls-bxflow-epsic-1.1.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.616077 dls-bxflow-epsic-1.1.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.616077 dls-bxflow-epsic-1.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.616077 dls-bxflow-epsic-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.608077 dls-bxflow-epsic-1.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/Makefile-conda
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-02-16 12:39:07.636076 dls-bxflow-epsic-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.608077 dls-bxflow-epsic-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.620077 dls-bxflow-epsic-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.624076 dls-bxflow-epsic-1.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/images/workflow_of_tasks.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/images/workflow_of_tasks.drawio.png
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.624076 dls-bxflow-epsic-1.1.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.624076 dls-bxflow-epsic-1.1.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/01-personal_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/50-naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/explanations/60-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.624076 dls-bxflow-epsic-1.1.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/how-to/under_construction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.624076 dls-bxflow-epsic-1.1.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.628076 dls-bxflow-epsic-1.1.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.628076 dls-bxflow-epsic-1.1.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/01-installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.612077 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.628076 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/
--rw-r--r--   0 runner    (1001) docker     (123)    55338 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/finish.png
--rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/post_submit.png
--rw-r--r--   0 runner    (1001) docker     (123)    24403 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/pre_submit.png
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/start.png
--rw-r--r--   0 runner    (1001) docker     (123)    54940 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/docs/user/tutorials/images/submitting_gui/stdout.png
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 12:39:07.636076 dls-bxflow-epsic-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.628076 dls-bxflow-epsic-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.632076 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.632076 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/algorithms/mib_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.632076 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/collectors/mib_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/epsic_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/epsic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.632076 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-16 12:39:07.000000 dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:39:07.636076 dls-bxflow-epsic-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-16 12:38:59.000000 dls-bxflow-epsic-1.1.0/tests/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.183571 dls-bxflow-epsic-1.1.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/Makefile-conda
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.191572 dls-bxflow-epsic-1.1.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.187572 dls-bxflow-epsic-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/mib_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/mib_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 17:00:59.000000 dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:59.195572 dls-bxflow-epsic-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 17:00:49.000000 dls-bxflow-epsic-1.1.1/tests/test_stub.py
```

### Comparing `dls-bxflow-epsic-1.1.0/.dae-devops/Makefile` & `dls-bxflow-epsic-1.1.1/.dae-devops/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint d2fb8e61f884f1a612b221b3ba854350
+# dae_devops_fingerprint 3b85c3a25ea43c17608be0e3c8193fbb
```

### Comparing `dls-bxflow-epsic-1.1.0/.dae-devops/docs/developing.rst` & `dls-bxflow-epsic-1.1.1/.dae-devops/docs/developing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
-    $ git clone None/dls-bxflow-epsic.git
+    $ cd <your development area>
+    $ git clone https://github.com/DiamondLightSource/dls-bxflow-epsic.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
 Make sure to have at least python version 3.9 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-bxflow-epsic
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
-    $ pip install -e .[dev]
+    $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
-|
 
-If you plan to modify the docs, you will need to::
-
-    $ pip install -e .[docs]
-
-    
-
-
-.. # dae_devops_fingerprint b02a221e876b2001c489aafa8f7bbfa4
+.. # dae_devops_fingerprint 7826bc083f17254f3dd7ee314d804d35
```

### Comparing `dls-bxflow-epsic-1.1.0/.dae-devops/docs/docs_structure.rst` & `dls-bxflow-epsic-1.1.1/.dae-devops/docs/docs_structure.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 2e30b83c623d1a0ebe5970adf5436b59
+.. # dae_devops_fingerprint fce0ce4536d0dcfc0d47fb1feab4d1fb
```

### Comparing `dls-bxflow-epsic-1.1.0/.dae-devops/docs/installing.rst` & `dls-bxflow-epsic-1.1.1/.dae-devops/docs/installing.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 Installing
 =======================================================================
 
 
 You will need python 3.9 or later. 
@@ -20,24 +20,23 @@
 installation will not interfere with any existing Python software::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use ``pip`` to install the package and its dependencies::
 
-    $ export PIP_FIND_LINKS=/dls_sw/apps/bxflow/artifacts
     $ python3 -m pip install dls-bxflow-epsic
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
-    $ python3 -m pip install git+None/dls-bxflow-epsic.git
+    $ python3 -m pip install git+https://github.com/DiamondLightSource/dls-bxflow-epsic.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-bxflow-epsic --version
     $ dls-bxflow-epsic --version-json
 
-.. # dae_devops_fingerprint c2d1dd060a19ee7d8f64de4e6fc349c7
+.. # dae_devops_fingerprint 48af32ed4de39d505677bee06a605da4
```

### Comparing `dls-bxflow-epsic-1.1.0/.devcontainer/Dockerfile` & `dls-bxflow-epsic-1.1.1/.devcontainer/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-bxflow-epsic"]
 CMD ["--version"]
 
-# dae_devops_fingerprint c4601ef0db4565e3cf9175fd1cccf836
+# dae_devops_fingerprint 4835daca5f07a878b649008c9ec2ce14
```

### Comparing `dls-bxflow-epsic-1.1.0/.devcontainer/devcontainer.json` & `dls-bxflow-epsic-1.1.1/.devcontainer/devcontainer.json`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.1.
+// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 // ********** For repository_name dls-bxflow-epsic
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint f4c5a8ffa913bdd98b121cc85b15a606
+// dae_devops_fingerprint 20df0a5b867cb7653ba9649dca1c1a00
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/CONTRIBUTING.rst` & `dls-bxflow-epsic-1.1.1/.github/CONTRIBUTING.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow-epsic
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-bxflow-epsic/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 4f7317683170497994c2a1367937d07f
+.. # dae_devops_fingerprint 13ac2e6d5f664ef7ea332d28c6398ae0
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/actions/install_requirements/action.yml` & `dls-bxflow-epsic-1.1.1/.github/actions/install_requirements/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint 89f9814e0c532dfd4b5b2495dd2ad96a
+# dae_devops_fingerprint 37fd36735c2ec4d41ec70face6534498
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/pages/make_switcher.py` & `dls-bxflow-epsic-1.1.1/.github/pages/make_switcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint 8b096e04511a4341cf8142cbb16f0bce
+# dae_devops_fingerprint d97331bf5a58b1b73441792890268408
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/workflows/code.yml` & `dls-bxflow-epsic-1.1.1/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -35,15 +35,15 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.10", "3.11"]
+        python: ["3.10"]
         install: ["-e .[dev,docs]"]
         # Make one version be non-editable to test both paths of version code
         include:
           - os: "ubuntu-latest"
             python: "3.9"
             install: ".[dev,docs]"
 
@@ -65,14 +65,18 @@
           python_version: ${{ matrix.python }}
           requirements_file: requirements-test-${{ matrix.os }}-${{ matrix.python }}.txt
           install_options: ${{ matrix.install }}
 
       - name: List dependency tree
         run: pipdeptree
 
+      # TODO: Make startup of MySQL able to be configured.
+      - name: Start up the MySQL that comes with Unbuntu
+        run: sudo /etc/init.d/mysql start
+
       - name: Run tests
         run: |
           sudo apt install environment-modules
           export MODULESHOME=/usr/share/modules
           source $MODULESHOME/init/bash
           pytest
 
@@ -208,8 +212,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint dd7f0f18a8a46f81699bee29afa4381e
+# dae_devops_fingerprint 10ebf277e974272f2bc4b2ee40a5f388
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/workflows/docs.yml` & `dls-bxflow-epsic-1.1.1/.github/workflows/docs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint 9f2aa1ea17c5016c908a0256958f38e1
+# dae_devops_fingerprint 767f4954a6780516de4c325fa18e8d43
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/workflows/docs_clean.yml` & `dls-bxflow-epsic-1.1.1/.github/workflows/docs_clean.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint db77329612b0b00679e6466418644f86
+# dae_devops_fingerprint 4d17fd267a29eb07bc8fc18a9404ad7e
```

### Comparing `dls-bxflow-epsic-1.1.0/.github/workflows/linkcheck.yml` & `dls-bxflow-epsic-1.1.1/.github/workflows/linkcheck.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 name: Link Check
 
 on:
   workflow_dispatch:
   schedule:
@@ -23,8 +23,8 @@
         with:
           requirements_file: requirements-dev-3.x.txt
           install_options: -e .[dev]
 
       - name: Check links
         run: tox -e docs build -- -b linkcheck
 
-# dae_devops_fingerprint 88acfec9f0648cf634437da23e2b0c42
+# dae_devops_fingerprint 274a0b744b9a9a06dac8b2c8e47e7b45
```

### Comparing `dls-bxflow-epsic-1.1.0/.gitignore` & `dls-bxflow-epsic-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/.gitlab-ci.yml` & `dls-bxflow-epsic-1.1.1/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint b38987b05905a2da4e0865e405239307
+# dae_devops_fingerprint f39b28a4f448224c75d3e2aaf02a2255
```

### Comparing `dls-bxflow-epsic-1.1.0/.vscode/launch.json` & `dls-bxflow-epsic-1.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/LICENSE` & `dls-bxflow-epsic-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/Makefile` & `dls-bxflow-epsic-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/Makefile-conda` & `dls-bxflow-epsic-1.1.1/Makefile-conda`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/PKG-INFO` & `dls-bxflow-epsic-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,19 +222,10 @@
 
 Bxflow beamline library for B24.
 
 Wraps core science algorithms as runnable tasks for workflow execution.
 
 Also implements the filesystem naming conventions at the beamline.
 
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-bxflow-epsic-workflows/index.html for how to install and run workflows.
-
 ..
     Anything below this line is used when viewing README.rst and will be replaced
     when included in index.rst
-
-
-Documentation
------------------------------------------------------------------------
-
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-bxflow-epsic/index.html for more detailed documentation on this package.
-
```

### Comparing `dls-bxflow-epsic-1.1.0/docs/conf.py` & `dls-bxflow-epsic-1.1.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -146,15 +146,15 @@
 ]
 
 # Theme options for pydata_sphinx_theme
 html_theme_options = dict(
     logo=dict(
         text=project,
     ),
-    gitlab_url="None/dls-bxflow-epsic",
+    gitlab_url="https://github.com/DiamondLightSource/dls-bxflow-epsic",
     icon_links=[],
     navbar_end=["theme-switcher", "icon-links"],
 )
 
 # A dictionary of values to pass into the template engine’s context for all pages
 html_context = dict(
     doc_path="docs",
@@ -183,18 +183,18 @@
 
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "dls-bxflow-epsic",
     "$" + "{package_name}": "dls_bxflow_epsic",
-    "$" + "{git_url}": "None",
+    "$" + "{git_url}": "https://github.com/DiamondLightSource",
     "$" + "{python_version_at_least}": "3.9",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 3e7235c51f320375fb661b9275563a7b
+# dae_devops_fingerprint 771750311240a1d0e5a5ff2021d97ae7
```

### Comparing `dls-bxflow-epsic-1.1.0/docs/images/dls-favicon.ico` & `dls-bxflow-epsic-1.1.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/docs/images/dls-logo.svg` & `dls-bxflow-epsic-1.1.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/docs/user/explanations/50-naming_conventions.rst` & `dls-bxflow-epsic-1.1.1/.dae-devops/docs/conventions.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+.. # ********** Please don't edit this file!
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
+.. # ********** For repository_name dls-bxflow-epsic
+
 Naming conventions
 =======================================================================
 
-Here we discuss the naming conventions used within the bxflow source code.
+Here are the naming conventions used within the source code.
 
 variables
     lowercase, underscores
 
 constants
     uppercase, underscores
 
 classes
     camel case
 
 class methods
     lowercase, underscores
 
 imports
-    require fully qualified package name (impore <package> does nothing)
+    require fully qualified package name (import <package> does nothing)
 
     exception: top-level packages __init__.py will have __version__ defined in them
 
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
+
+.. # dae_devops_fingerprint 349e0c44ef1e1149e92045fdf14e6954
```

### Comparing `dls-bxflow-epsic-1.1.0/pyproject.toml` & `dls-bxflow-epsic-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow-epsic
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -30,14 +30,15 @@
     "Flake8-pyproject",
     "pipdeptree",
     "pre-commit",
     "pytest-cov",
     "pydocstyle[toml]",
     "tox-direct",
     "types-mock",
+    "types-PyYAML",
 ]
 docs = [
     "pydata-sphinx-theme>=0.12",
     "sphinx-argparse",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
@@ -97,8 +98,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint e3e62774b0e3496735879f6172030143
+# dae_devops_fingerprint 672bc5399adbec5a8ff773c50f9fcffd
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/algorithms/mib_converter.py` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/algorithms/mib_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 
 # -----------------------------------------------------------------------------------
 class MibConverter:
     """
     Class which converts a single mib file to hdf5.
     Uses the method "convert" imported from mib2hdfConvert package in https://github.com/ePSIC-DLS/epsic_tools.
-    This is called via mib_convert task run method, by main_isolated on the cluster.
+    This class is called from the EpsicWorkflow::add_mib_convert_task method.
+    This runs in the cluster.
     """
 
     def __init__(self, mib_filename, bx_task=None):
         if bx_task is None:
             raise RuntimeError(
                 f"MibConverter has not been given a bx_task instance for mib_filename {mib_filename}"
             )
@@ -63,15 +64,15 @@
             self.__mib_filename
         )
 
     # ------------------------------------------------------------------------------
     async def run(self):
         """
         Run the conversion.
-        Even though async, this caller knows this be long-blocking.
+        Even though async, the caller knows this be long-blocking.
         """
 
         if self.has_any_converted_filenames():
             logger.info(f"the conversion is apparently done for {self.__mib_filename}")
         else:
             # If we want the data stored under a subdirectory with the material name,
             # then we have to give a folder.
@@ -90,15 +91,15 @@
 
             # Importing from mib2hdf_watch_convert drags in a lot of dependencies
             # which can produce a lot of logging.
             for handler in logging.getLogger().handlers:
                 # Filter out the unwanted log lines.
                 handler.addFilter(_logging_filter())
 
-            # We use the module load bxflow/epsic/latest to set the PYTHONPATH for this.
+            # Presume the "module load bxflow/epsic/latest" sets the PYTHONPATH for this import.
             from batch_mib_convert.mib2hdf_watch_convert import convert
 
             convert(
                 self.__beamline,
                 self.__year,
                 self.__visit,
                 [self.__mib_filename],
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/collectors/mib_scraper.py` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/collectors/mib_scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         BxFlowScraper.__init__(self, specification, predefined_uuid=predefined_uuid)
 
         self.set_thing_type = thing_type
 
     # ----------------------------------------------------------------------------------------
     def derive_data_label(self, data_filename):
         """
-        Data label, such as scan number, derived from specification data_filename.
+        Returns a data label, such as scan number, derived from specification data_filename.
         This method fulfills the abstract method on the base class.
         """
 
         # Data label is derived from mib_filename by using material plus the date_stamp.
         data_label = is_done_filename_2_data_label(data_filename)
 
         return data_label
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/epsic_workflow.py` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/epsic_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import logging
+from typing import Dict, Optional, Union
 
 # Filestore interface.
 from dls_bxflow_lib.bx_filestores.bx_filestores import bx_filestores_get_default
+
+# Base class for workflows.
 from dls_bxflow_lib.bx_workflows.base import Base as BxWorkflowBase
 
 # Object managers.
 from dls_bxflow_run.bx_tasks.bx_tasks import BxTasks
 from dls_bxflow_run.bx_tasks.constants import Types as BxTaskTypes
-from dls_utilpack.callsign import callsign
-from dls_utilpack.require import require
 
 # Utilities.
+from dls_utilpack.callsign import callsign
+from dls_utilpack.require import require
 from dls_utilpack.search_file import search_file
 
 # Output location convention.
 from dls_bxflow_epsic.utilities import data_label_2_filestore_directory
 
 # Versions of things.
 from dls_bxflow_epsic.version import meta as dls_bxflow_epsic_meta
@@ -27,17 +30,17 @@
 
 
 class EpsicWorkflow(BxWorkflowBase):
     """
     This class provides some beamline-specific helper methods.
 
     It makes some assumptions:
-    - tasks are added in order, and only depend on the one coming before to finish
-    - the final task ends the job with either of its standard gates
-    - any failure gate ends the job
+        - tasks are added in order, and only depend on the one coming before to finish
+        - the final task ends the job with either of its standard gates
+        - any failure gate ends the job
     """
 
     # ------------------------------------------------------------------
     def __init__(self, **kwargs):
 
         # Put versions into the log.
         meta_dict = dls_bxflow_epsic_meta()
@@ -63,45 +66,48 @@
             # Tell the workflow builder where the output files should go.
             bx_filestores_get_default().set_directory(filestore_directory)
 
             logger.info(
                 f"{callsign(self)} sets filestore_directory to {filestore_directory}"
             )
 
-        # -----------------------------------------------------------------------------
         # Init the base class only AFTER the filestore_directory is set.
-
         BxWorkflowBase.__init__(self, **kwargs)
 
         # There might be no data label in the constructor kwargs.
         if hasattr(self, "data_label"):
             # Modify the job's data_label.
             self.bx_job.set_data_label(self.data_label)
 
     # ------------------------------------------------------------------
     def add_notebook_task(
         self,
-        notebook_name,
-        modify_cells=None,
-        remex_hints=None,
-        label_suffix=None,
+        notebook_name: str,
+        modify_cells: Optional[Dict] = None,
+        remex_hints: Optional[Union[Dict, str]] = None,
+        label_suffix: Optional[str] = None,
     ):
+
         """
         Add a notebook task.
 
         Args:
             notebook_name (str): name of the notebook, without root directory or .ipynb suffix
-            cells ({str: str}, optional): Python code to be put into cells. Defaults to None, which means don't replace.
-            label_suffix (str, optional): Suffix to be appended to notebook name for task label, for example when multiple of the same task class are done on the same inputs Defaults to None.
+            modify_cells (Optional[Dict]): Python code to be put into cells.
+                Defaults to None, which means don't replace.
+                This argument is a dict whose keys are the cell numbers.
+            remex_hints (Optional[Dict]): Dictionary specifying the remote execution hints for this task.
+            label_suffix (Optional[str]): Suffix to be appended to notebook name for task label,
+                for example when multiple of the same task class are done on the same inputs Defaults to None.
 
         Raises:
             RuntimeError: Any kind of error in this method.
 
         Returns:
-            BxTask: task object.
+            BxTask task object.
         """
 
         label = notebook_name
         try:
             # Make full path to the notebook to run.
             ipynb_filename = search_file(
                 self.bx_configurator.require("epsic.notebook_paths"),
@@ -126,15 +132,14 @@
                 "type_specific_tbd": {
                     "ipynb_filename": ipynb_filename,
                     "modify_cells": modify_cells,
                 },
             }
 
             # Assemble remex_hints from task and configuration.
-            # TODO: Find a way to avoid manually doing assemble_remex_hints for every task.
             self.assemble_remex_hints(bx_task_specification)
 
             # Build the task.
             bx_task = BxTasks().build_object(
                 bx_task_specification,
             )
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/utilities.py` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import glob
 import logging
 import os
+from typing import Optional, Tuple
 
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------
-def is_done_filename_2_data_label(is_done_filename):
+def is_done_filename_2_data_label(is_done_filename: str) -> str:
     """
-    Given a full mib (or is_done) filename path, derive a data label from it.
+    Given a full "is_done" filename path, derive a data label from it.
 
     Rules:
-    1. the data_filename must have /Merlin/ somwhere in the path.
-    2. the final directory in the path is ignored.
-    3. whatever is between /Merlin/ and that final directory, is the data_label.
-    4. this works for is_done files whose name differ from their mib files by suffix only.
+        1. the data_filename must have /Merlin/ somwhere in the path.
+        2. the final directory in the path is ignored.
+        3. whatever is between /Merlin/ and that final directory, is the data_label.
+        4. this works for is_done files whose name differ from their mib files by suffix only.
     """
 
     # There should be one Merlin somewhere in the scraped filename.
     parts = is_done_filename.split("/Merlin/")
 
     if len(parts) == 1:
         raise RuntimeError(f"no /Merlin/ in is_done_filename {is_done_filename}")
     if len(parts) > 2:
         raise RuntimeError(f"multiple /Merlin/ in is_done_filename {is_done_filename}")
 
     # Everything past the Merlin.
-    parts = parts[1]
+    part1 = parts[1]
     # Split into subdirectories.
-    parts = parts.split("/")
+    parts = part1.split("/")
 
     if len(parts) < 2:
         raise RuntimeError(
             f"no material after /Merlin/ in is_done_filename {is_done_filename}"
         )
 
     # Material is everything between Merlin and the filename.
@@ -48,37 +49,37 @@
     # Data label is made up of material plus the date_stamp of the filename.
     data_label = f"{material}/{date_stamp}"
 
     return data_label
 
 
 # ------------------------------------------------------------------------------------------
-def mib_filename_2_data_label(mib_filename):
+def mib_filename_2_data_label(mib_filename: str) -> str:
     """
-    Given a full mib (or is_done) filename path, derive a data label from it.
+    Given a full mib filename path, derive a data label from it.
 
     Rules:
-    1. the data_filename must have /Merlin/ somwhere in the path.
-    2. the final directory in the path is ignored.
-    3. whatever is between /Merlin/ and that final directory, is the data_label.
-    4. this works for is_done files whose name differ from their mib files by suffix only.
+        1. the data_filename must have /Merlin/ somwhere in the path.
+        2. the final directory in the path is ignored.
+        3. whatever is between /Merlin/ and that final directory, is the data_label.
+        4. this works for is_done files whose name differ from their mib files by suffix only.
     """
 
     # There should be one Merlin somewhere in the scraped filename.
     parts = mib_filename.split("/Merlin/")
 
     if len(parts) == 1:
         raise RuntimeError(f"no /Merlin/ in mib_filename {mib_filename}")
     if len(parts) > 2:
         raise RuntimeError(f"multiple /Merlin/ in mib_filename {mib_filename}")
 
     # Everything past the Merlin.
-    parts = parts[1]
+    part1 = parts[1]
     # Split into subdirectories.
-    parts = parts.split("/")
+    parts = part1.split("/")
 
     if len(parts) < 3:
         raise RuntimeError(f"no material after /Merlin/ in mib_filename {mib_filename}")
 
     # Material is everything between Merlin and last subdirectory and filename.
     material = "/".join(parts[:-2])
 
@@ -92,16 +93,18 @@
     # Data label is made up of material plus the date_stamp of the filename.
     data_label = f"{material}/{date_stamp}"
 
     return data_label
 
 
 # ------------------------------------------------------------------------------------------
-def data_label_2_mib_filename(data_label):
-    """ """
+def data_label_2_mib_filename(data_label: str) -> str:
+    """
+    Given a data label, compose a full filename path to the mib file.
+    """
 
     beamline, year, visit = configuration_2_byv()
 
     data_filename = f"/dls/{beamline}/data/{year}/{visit}/Merlin/{data_label}_data.mib"
 
     glob_search = (
         f"{os.path.dirname(data_filename)}/*/{os.path.basename(data_filename)}"
@@ -121,19 +124,21 @@
     if not os.path.isfile(data_filename):
         raise RuntimeError(f"data_filename is not a file: {data_filename}")
 
     return data_filename
 
 
 # ------------------------------------------------------------------------------------------
-def data_label_2_processing(data_label, nickname=None):
+def data_label_2_processing(data_label: str, nickname: Optional[str] = None) -> str:
     """
-    Give processing directory where data_label stuff is saved.
+    Return processing directory where data_label stuff is saved.
     This area is outside any task's specific instance directory.
     That is, all tasks of all jobs ever run share reading and writing into this directory.
+
+    If nickname is provided, it is used to customize the actual filename produced for the data label.
     """
 
     beamline, year, visit = configuration_2_byv()
 
     visit_directory = f"/dls/{beamline}/data/{year}/{visit}"
 
     processing = f"{visit_directory}/processing/Merlin/{data_label}"
@@ -157,30 +162,42 @@
     else:
         raise RuntimeError(f"nickname '{nickname}' is not among [{repr(nicknames)}]")
 
     return filename
 
 
 # ----------------------------------------------------------------------------------------
-def configuration_2_byv():
+def configuration_2_byv() -> Tuple[str, str, str]:
+    """
+    Returns the beamline, year and visit indicated by the configuration.
+
+    Returns:
+        Tuple[str, str, str]: beamline, year, visit
+    """
 
     # Configurator interface.
     from dls_bxflow_lib.bx_configurators.bx_configurators import (
         bx_configurators_get_default,
     )
 
     beamline = bx_configurators_get_default().require("visit.beamline")
     year = bx_configurators_get_default().require("visit.year")
     visit = bx_configurators_get_default().require("visit.visit")
 
     return (beamline, year, visit)
 
 
 # ----------------------------------------------------------------------------------------
-def data_filename_2_byv(data_filename):
+def data_filename_2_byv(data_filename: str) -> Tuple[str, str, str]:
+    """
+    Returns the beamline, year and visit indicated by the filename.
+
+    Returns:
+        Tuple[str, str, str]: beamline, year, visit
+    """
 
     error = "nonconformant data filename"
 
     parts = data_filename.split("/")
 
     if len(parts) < 7:
         raise ValueError(
@@ -199,15 +216,24 @@
     if literal_data != "data":
         raise ValueError(f"{error}: third path segment not 'data' in {data_filename}")
 
     return (beamline, year, visit)
 
 
 # ----------------------------------------------------------------------------------------
-def mib_filename_2_filestore_directory(mib_filename):
+def mib_filename_2_filestore_directory(mib_filename: str) -> str:
+    """
+    From the mib_filename, derive the associated directory name where execution results can be written.
+
+    Args:
+        mib_filename (str): full path to mib filename
+
+    Returns:
+        str: directory in the visit's procecssing area, with data label as leaf
+    """
 
     data_label = mib_filename_2_data_label(mib_filename)
 
     beamline, year, visit = data_filename_2_byv(mib_filename)
 
     visit_directory = f"/dls/{beamline}/data/{year}/{visit}"
 
@@ -219,19 +245,27 @@
         f"data_label {mib_filename} derives filestore_directory is {filestore_directory}"
     )
 
     return filestore_directory
 
 
 # ----------------------------------------------------------------------------------------
-def data_label_2_filestore_directory(data_label):
+def data_label_2_filestore_directory(data_label: str) -> str:
+    """
+    From the data_label, derive the associated directory name where execution results can be written.
+
+    Args:
+        data_label (str): data_label for this dataset
+
+    Returns:
+        str: directory in the visit's procecssing area, with data label as leaf
+    """
 
     # This needs configurator to give beamline, year and visit.
     # So is not available under main_isolated.
-    # TODO: Let main_isolated create a filestore.
     mib_filename = data_label_2_mib_filename(data_label)
 
     filestore_directory = mib_filename_2_filestore_directory(mib_filename)
 
     logger.debug(f"data_label {data_label} implies mib_filename {mib_filename}")
     logger.debug(
         f"mib_filename {mib_filename} implies"
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic/version.py` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/PKG-INFO` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow-epsic
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bxflow beamline code for ePSIC.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,19 +222,10 @@
 
 Bxflow beamline library for B24.
 
 Wraps core science algorithms as runnable tasks for workflow execution.
 
 Also implements the filesystem naming conventions at the beamline.
 
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-bxflow-epsic-workflows/index.html for how to install and run workflows.
-
 ..
     Anything below this line is used when viewing README.rst and will be replaced
     when included in index.rst
-
-
-Documentation
------------------------------------------------------------------------
-
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-bxflow-epsic/index.html for more detailed documentation on this package.
-
```

### Comparing `dls-bxflow-epsic-1.1.0/src/dls_bxflow_epsic.egg-info/SOURCES.txt` & `dls-bxflow-epsic-1.1.1/src/dls_bxflow_epsic.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
 .dae-devops/docs/docs_structure.rst
+.dae-devops/docs/documenting.rst
 .dae-devops/docs/installing.rst
 .dae-devops/docs/testing.rst
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
@@ -29,37 +30,32 @@
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
+docs/explanations/conventions.rst
+docs/explanations/docs_structure.rst
+docs/explanations/index.rst
+docs/explanations/todo.rst
+docs/how-to/developing.rst
+docs/how-to/devops.rst
+docs/how-to/documenting.rst
+docs/how-to/index.rst
+docs/how-to/installing.rst
+docs/how-to/testing.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
-docs/images/workflow_of_tasks.drawio
-docs/images/workflow_of_tasks.drawio.png
-docs/user/index.rst
-docs/user/explanations/01-personal_configuration.rst
-docs/user/explanations/22-developing.rst
-docs/user/explanations/23-testing.rst
-docs/user/explanations/24-devops.rst
-docs/user/explanations/50-naming_conventions.rst
-docs/user/explanations/60-docs-structure.rst
-docs/user/how-to/under_construction.rst
-docs/user/reference/api.rst
-docs/user/reference/api/classes.rst
-docs/user/reference/api/command_line.rst
-docs/user/reference/api/modules.rst
-docs/user/tutorials/01-installing.rst
-docs/user/tutorials/images/submitting_gui/finish.png
-docs/user/tutorials/images/submitting_gui/post_submit.png
-docs/user/tutorials/images/submitting_gui/pre_submit.png
-docs/user/tutorials/images/submitting_gui/start.png
-docs/user/tutorials/images/submitting_gui/stdout.png
-src/__init__.py
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 src/dls_bxflow_epsic/__init__.py
 src/dls_bxflow_epsic/__main__.py
 src/dls_bxflow_epsic/_version.py
 src/dls_bxflow_epsic/epsic_main.py
 src/dls_bxflow_epsic/epsic_workflow.py
 src/dls_bxflow_epsic/utilities.py
 src/dls_bxflow_epsic/version.py
```

### Comparing `dls-bxflow-epsic-1.1.0/tests/base_tester.py` & `dls-bxflow-epsic-1.1.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-epsic-1.1.0/tests/conftest.py` & `dls-bxflow-epsic-1.1.1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     """
     Fixture to set up python log formatting and filtering for the tests.
 
     Yields:
         None
     """
 
-    # TODO: Better way to get a newline in conftest after pytest emits the test class name.
     print("")
 
     formatter = DlsLogformatter(type="long")
     logger = logging.StreamHandler()
     logger.setFormatter(formatter)
     logging.getLogger().addHandler(logger)
```

### Comparing `dls-bxflow-epsic-1.1.0/tests/test_stub.py` & `dls-bxflow-epsic-1.1.1/tests/test_stub.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Run the test science outside of any bxflow workflow framework.
 
         Instantiates the txrm science class and runs it.
 
         Args:
             logging_setup (Any): logging setup created by the fixture
             output_directory (str): output directory assigned by the fixture.
-                The output directory is typically in /tmp/dls-bxflow-b24.
+                The output directory is typically in /tmp/dls-bxflow-epsic.
                 It is wiped clean before the test, but left standing after the test.
 
         The output directory is set up as the current working directory
         before the science class is called.
         """
 
         self.main(output_directory)
```


# Comparing `tmp/dls-bxflow-2.2.0.tar.gz` & `tmp/dls-bxflow-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-2.2.0.tar", last modified: Tue May 16 13:40:42 2023, max compression
+gzip compressed data, was "dls-bxflow-2.3.0.tar", last modified: Mon May 29 16:53:55 2023, max compression
```

## Comparing `dls-bxflow-2.2.0.tar` & `dls-bxflow-2.3.0.tar`

### file list

```diff
@@ -1,426 +1,446 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/remex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/dataface_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/news_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/find_xanes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/fire_i22.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_dcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    28516 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/scandir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40092 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/curses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/island.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/popener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/bx_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/overall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/parser1.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/bx_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/module_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/symlink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/bx_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/main_isolated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/backend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/filestore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ispyb-local.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/dawn2_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/tests/datafiles/gaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow1/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow2/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/i22-4996.nxs
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/gda_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/gda_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/execute.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/jupyter1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/jupyter_bad_cell.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/notebooks/c.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qacct
--rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qstat
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qsub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/stub_commands/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/dawn
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/mpirun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_collector_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_extract_error_lines_dawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_extract_error_lines_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_gaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_a_bc_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_pubcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_logstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_protocolj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_scheduler_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/workflows/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/a/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/b/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/c/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/e/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/f/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/f/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/f/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/g/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/g/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.161045 dls-bxflow-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.113044 dls-bxflow-2.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-05-29 16:53:55.161045 dls-bxflow-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.113044 dls-bxflow-2.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.121044 dls-bxflow-2.3.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/explanations/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:53:55.161045 dls-bxflow-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.117044 dls-bxflow-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:53:55.000000 dls-bxflow-2.3.0/src/dls_bxflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/remex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.125044 dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/dataface_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/news_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.129044 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/find_xanes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/fire_i22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/report_dcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.129044 dls-bxflow-2.3.0/src/dls_bxflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 16:53:54.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.129044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.129044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.129044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30124 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/scandir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40200 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/curses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.133044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.117044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.117044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.117044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.137045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24162 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/island.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/popener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.141044 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/bx_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_lib/dummies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/dummies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/dummies/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/overall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/parser1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.145045 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/bx_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.149045 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/execution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/module_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/symlink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.149045 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/bx_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/src/dls_bxflow_run/main_isolated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.153045 dls-bxflow-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.153045 dls-bxflow-2.3.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/configurations/backend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/configurations/filestore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/configurations/ispyb-local.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.153045 dls-bxflow-2.3.0/tests/configurations/ptypy_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.153045 dls-bxflow-2.3.0/tests/configurations/ptyrex_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.153045 dls-bxflow-2.3.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/datafiles/dawn2_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.117044 dls-bxflow-2.3.0/tests/datafiles/gaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/datafiles/gaml/workflow1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/datafiles/gaml/workflow1/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/datafiles/gaml/workflow2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/datafiles/gaml/workflow2/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/datafiles/i22-4996.nxs
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/gda_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/gda_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/jupyter/execute.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/jupyter/jupyter1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/jupyter/jupyter2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/jupyter/jupyter_bad_cell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/jupyter/random_string.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/notebooks/c.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/qacct
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/qstat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/qsub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/stub_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/stub_commands/dawn
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/stub_commands/mpirun
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_collector_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_dataface_revision5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_extract_error_lines_dawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_extract_error_lines_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_gaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_job_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_job_a_bc_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_job_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_job_pubcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_job_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_launcher_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_launcher_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_launcher_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_launcher_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_logstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_protocolj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_scheduler_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/test_workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/a/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/b/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/c/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/e/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.157045 dls-bxflow-2.3.0/tests/workflows/f/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/f/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/f/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:55.161045 dls-bxflow-2.3.0/tests/workflows/g/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/g/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 16:53:44.000000 dls-bxflow-2.3.0/tests/workflows/utilities.py
```

### Comparing `dls-bxflow-2.2.0/.dae-devops/Makefile` & `dls-bxflow-2.3.0/.dae-devops/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint ace7b2331dc490eea0a624c6a70f9801
+# dae_devops_fingerprint e6429d30b68cdf1d9bf59cd6ba82a897
```

### Comparing `dls-bxflow-2.2.0/.dae-devops/docs/developing.rst` & `dls-bxflow-2.3.0/.dae-devops/docs/developing.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
 Make sure to have at least python version 3.9 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-bxflow
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
-.. # dae_devops_fingerprint c6d12d2fc58a09bafbe3b215154a75b3
+.. # dae_devops_fingerprint 11f0213ef0b324cda0df9d9d4e83e45e
```

### Comparing `dls-bxflow-2.2.0/.dae-devops/docs/installing.rst` & `dls-bxflow-2.3.0/.dae-devops/docs/installing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow
 
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
     $ python3 -m pip install dls-bxflow
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-bxflow --version
     $ dls-bxflow --version-json
 
-.. # dae_devops_fingerprint 4bea84b87f4db70a5ddf45d34db12a75
+.. # dae_devops_fingerprint 4774d104322125c03718fda80e51341b
```

### Comparing `dls-bxflow-2.2.0/.dae-devops/docs/testing.rst` & `dls-bxflow-2.3.0/.dae-devops/docs/testing.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow
 
 Testing
 =======================================================================
 
 The package uses pytest for unit testing.
 
 If you want to run the tests, first get a copy of the code per the instructions in the Developing section.
 
 Then you can run all tests by::
 
-    $ pytest
-
-Or this, which is the command used by the CI runner.
-
-    $ make -f .dae-devops/Makefile validate_pytest
+    $ tox -q -e pytest
 
 To run a single test you can do::
 
     $ pytest tests/the_test_you_want.py
 
-If you want to see more output of the test while it's running you can do:
+If you want to see more output of the test while it's running you can do::
 
     $ pytest -sv -ra --tb=line tests/the_test_you_want.py
 
 Each test will write files into its own directory::
 
-    /tmp/dls-bxflow/tests/....
+    /tmp/dls-bxflow/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint a08072081a8239fba2532476e6ea8916
+.. # dae_devops_fingerprint 58ccb8ff8aa55ed529e1d7942f96bd3c
```

### Comparing `dls-bxflow-2.2.0/.dae-devops/project.yaml` & `dls-bxflow-2.3.0/.dae-devops/project.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Primary information needed for devops.
 primary:
   repository_name: dls-bxflow
   package_name: dls_bxflow_lib
-  one_line_description: "Distributed beamline data processing workflow engine and gui platform core."
+  one_line_description: "Distributed beamline automated data processing workflow engine and gui platform core."
   author:
     name: David Erb
     email: david.erb@diamond.ac.uk
   project_urls:
     gitlab: https://gitlab.diamond.ac.uk/scisoft/bxflow
   project_scripts:
     dls-bxflow: "dls_bxflow_lib.__main__:main"
@@ -35,7 +35,9 @@
         - nbformat
         - pika
         - prettytable
         - pyyaml
         - ruamel.yaml
         - stomp.py
         - workflows
+        # TODO: Change configuration so that certain depdendencies are marked for unit testing.
+        - beautifulsoup4
```

### Comparing `dls-bxflow-2.2.0/.devcontainer/Dockerfile` & `dls-bxflow-2.3.0/.devcontainer/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-bxflow"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 803d20273c1c0b2a6a3200b8c6410702
+# dae_devops_fingerprint 4b16385a09d58128346881a6b53ef58a
```

### Comparing `dls-bxflow-2.2.0/.devcontainer/devcontainer.json` & `dls-bxflow-2.3.0/.devcontainer/devcontainer.json`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.1.
+// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 // ********** For repository_name dls-bxflow
 
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
 
-// dae_devops_fingerprint dc724afa6ae33cf3b1857868c5df57b5
+// dae_devops_fingerprint 8ee55efb6c475521fa40db01bb2eb177
```

### Comparing `dls-bxflow-2.2.0/.github/CONTRIBUTING.rst` & `dls-bxflow-2.3.0/.github/CONTRIBUTING.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.1.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-bxflow
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-bxflow/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 71d2f17cb32f218d0675ee6a2e61f2c8
+.. # dae_devops_fingerprint 12687dadc26b00ae0ff61a410a4e6ff1
```

### Comparing `dls-bxflow-2.2.0/.github/actions/install_requirements/action.yml` & `dls-bxflow-2.3.0/.github/actions/install_requirements/action.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
 
-# dae_devops_fingerprint 9887b75a50fea7fd75ad093e7e1b6db6
+# dae_devops_fingerprint a5800c88a9ba24077377747d0c06fb25
```

### Comparing `dls-bxflow-2.2.0/.github/dependabot.yml` & `dls-bxflow-2.3.0/.github/dependabot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint a1a3891fe3d1481471148898f3578de4
+# dae_devops_fingerprint 3e961ff662b90c708fef894a672a209d
```

### Comparing `dls-bxflow-2.2.0/.github/pages/make_switcher.py` & `dls-bxflow-2.3.0/.github/pages/make_switcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
-# dae_devops_fingerprint 48879aaa58911c1ca5af9ca2afa0766e
+# dae_devops_fingerprint d522d9d0c207340dbb11712b0fc3a203
```

### Comparing `dls-bxflow-2.2.0/.github/workflows/code.yml` & `dls-bxflow-2.3.0/.github/workflows/code.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
-# dae_devops_fingerprint 4bf15474960f346219ccfb234a0874d3
+# dae_devops_fingerprint 2496a94da8547d2fde5764df660161fd
```

### Comparing `dls-bxflow-2.2.0/.github/workflows/docs.yml` & `dls-bxflow-2.3.0/.github/workflows/docs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
-# dae_devops_fingerprint 617afa97687949aa9f835190c7da8e6c
+# dae_devops_fingerprint 2fe29e6e6518358f37cbab02c9e4e875
```

### Comparing `dls-bxflow-2.2.0/.github/workflows/docs_clean.yml` & `dls-bxflow-2.3.0/.github/workflows/docs_clean.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
-# dae_devops_fingerprint fee1f59e35578c03a42a63b5d063e089
+# dae_devops_fingerprint 1dbde6e7935c64316f9a184d42056d54
```

### Comparing `dls-bxflow-2.2.0/.gitignore` & `dls-bxflow-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/.gitlab-ci.yml` & `dls-bxflow-2.3.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
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
 
-# dae_devops_fingerprint 3cf449f0923f8b3d3d68663278369f50
+# dae_devops_fingerprint 5af5158b679b480e93d4a7acac724eb2
```

### Comparing `dls-bxflow-2.2.0/.vscode/launch.json` & `dls-bxflow-2.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/LICENSE` & `dls-bxflow-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/PKG-INFO` & `dls-bxflow-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.2.0
-Summary: Distributed beamline data processing workflow engine and gui platform core.
+Version: 2.3.0
+Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,54 +208,20 @@
 Project-URL: gitlab, https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-bxflow
 =======================================================================
 
-Distributed beamline data processing workflow engine and gui platform core.
+Distributed beamline automated data processing workflow engine and gui platform core.
 
-Intended advantages:
-
-- develop and manage automated data processing workflows
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git 
-
-    dls_bxflow --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-bxflow for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git 
-    cd dls-bxflow
-    virtualenv /scratch/$USER/venv/dls-bxflow
-    source /scratch/$USER/venv/dls-bxflow/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-bxflow/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-bxflow/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Support beamline-specific science algorithms as workflow tasks.
 
+For documentation see: https://diamondlightsource.github.io/dls-bxflow
```

### Comparing `dls-bxflow-2.2.0/docs/conf.py` & `dls-bxflow-2.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint a5136b9d758a5fc90e1452ecb285256e
+# dae_devops_fingerprint 08922598dd967c3d6e3355939a1f96e9
```

### Comparing `dls-bxflow-2.2.0/docs/images/dls-favicon.ico` & `dls-bxflow-2.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/docs/images/dls-logo.svg` & `dls-bxflow-2.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/pyproject.toml` & `dls-bxflow-2.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.1.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-bxflow
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -11,15 +11,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-description = "Distributed beamline data processing workflow engine and gui platform core."
+description = "Distributed beamline automated data processing workflow engine and gui platform core."
 dependencies = [
     "aio-pika",
     "dask[distributed]",
     "dls-servbase",
     "dls-mainiac",
     "dls-multiconf",
     "dls-utilpack",
@@ -36,18 +36,19 @@
     "nbformat",
     "pika",
     "prettytable",
     "pyyaml",
     "ruamel.yaml",
     "stomp.py",
     "workflows",
+    "beautifulsoup4",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "black==22.12.0",
     "mypy",
     "flake8-isort",
@@ -123,8 +124,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 32c67ec7b2a3de3d46988bba8c8821ef
+# dae_devops_fingerprint 3d46ccde71c7d5ba0b6ddc5950201db4
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow.egg-info/PKG-INFO` & `dls-bxflow-2.3.0/src/dls_bxflow.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.2.0
-Summary: Distributed beamline data processing workflow engine and gui platform core.
+Version: 2.3.0
+Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,54 +208,20 @@
 Project-URL: gitlab, https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-bxflow
 =======================================================================
 
-Distributed beamline data processing workflow engine and gui platform core.
+Distributed beamline automated data processing workflow engine and gui platform core.
 
-Intended advantages:
-
-- develop and manage automated data processing workflows
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git 
-
-    dls_bxflow --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-bxflow for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/bxflow/dls-bxflow.git 
-    cd dls-bxflow
-    virtualenv /scratch/$USER/venv/dls-bxflow
-    source /scratch/$USER/venv/dls-bxflow/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-bxflow/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-bxflow/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Support beamline-specific science algorithms as workflow tasks.
 
+For documentation see: https://diamondlightsource.github.io/dls-bxflow
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow.egg-info/SOURCES.txt` & `dls-bxflow-2.3.0/src/dls_bxflow.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
-README.rst
+README.md
 pyproject.toml
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
@@ -27,20 +28,33 @@
 .vscode/extensions.json
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/conf.py
 docs/index.rst
 docs/_static/css/custom.css
-docs/api/classes.rst
-docs/api/command_line.rst
-docs/api/index.rst
-docs/api/modules.rst
+docs/explanations/conventions.rst
+docs/explanations/docs_structure.rst
+docs/explanations/index.rst
+docs/explanations/jobs.rst
+docs/explanations/todo.rst
+docs/how-to/developing.rst
+docs/how-to/devops.rst
+docs/how-to/documenting.rst
+docs/how-to/index.rst
+docs/how-to/installing.rst
+docs/how-to/testing.rst
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
+docs/reference/classes.rst
+docs/reference/command_line.rst
+docs/reference/index.rst
+docs/reference/modules.rst
+docs/tutorials/index.rst
+docs/tutorials/tbd.rst
 src/dls_bxflow.egg-info/PKG-INFO
 src/dls_bxflow.egg-info/SOURCES.txt
 src/dls_bxflow.egg-info/dependency_links.txt
 src/dls_bxflow.egg-info/entry_points.txt
 src/dls_bxflow.egg-info/requires.txt
 src/dls_bxflow.egg-info/top_level.txt
 src/dls_bxflow_api/__init__.py
@@ -97,17 +111,15 @@
 src/dls_bxflow_lib/bx_collectors/scraper.py
 src/dls_bxflow_lib/bx_composers/__init__.py
 src/dls_bxflow_lib/bx_composers/bx_composers.py
 src/dls_bxflow_lib/bx_composers/html.py
 src/dls_bxflow_lib/bx_composers/prettyhelper.py
 src/dls_bxflow_lib/bx_composers/text.py
 src/dls_bxflow_lib/bx_configurators/__init__.py
-src/dls_bxflow_lib/bx_configurators/base.py
 src/dls_bxflow_lib/bx_configurators/bx_configurators.py
-src/dls_bxflow_lib/bx_configurators/yaml.py
 src/dls_bxflow_lib/bx_contexts/__init__.py
 src/dls_bxflow_lib/bx_contexts/base.py
 src/dls_bxflow_lib/bx_contexts/bx_contexts.py
 src/dls_bxflow_lib/bx_contexts/classic.py
 src/dls_bxflow_lib/bx_databases/__init__.py
 src/dls_bxflow_lib/bx_databases/aiosqlite.py
 src/dls_bxflow_lib/bx_databases/bx_databases.py
@@ -246,14 +258,15 @@
 src/dls_bxflow_run/bx_tasks/base.py
 src/dls_bxflow_run/bx_tasks/bx_tasks.py
 src/dls_bxflow_run/bx_tasks/constants.py
 src/dls_bxflow_run/bx_tasks/dawn1.py
 src/dls_bxflow_run/bx_tasks/dawn2.py
 src/dls_bxflow_run/bx_tasks/dawn_base.py
 src/dls_bxflow_run/bx_tasks/dummy.py
+src/dls_bxflow_run/bx_tasks/execution_summary.py
 src/dls_bxflow_run/bx_tasks/filename_classname.py
 src/dls_bxflow_run/bx_tasks/jupyter.py
 src/dls_bxflow_run/bx_tasks/module_classname.py
 src/dls_bxflow_run/bx_tasks/pickled_class.py
 src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
 src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
 src/dls_bxflow_run/bx_tasks/shell.py
@@ -277,23 +290,25 @@
 tests/test_catalog.py
 tests/test_collector.py
 tests/test_collector_scraper.py
 tests/test_composer.py
 tests/test_configurator.py
 tests/test_database.py
 tests/test_dataface.py
+tests/test_dataface_revision5.py
 tests/test_dawn1.py
 tests/test_dawn2.py
 tests/test_extract_error_lines_dawn.py
 tests/test_extract_error_lines_dummy.py
 tests/test_filestore.py
 tests/test_gaml.py
 tests/test_gui.py
 tests/test_job_a.py
 tests/test_job_a_bc_d.py
+tests/test_job_notebook.py
 tests/test_job_pubcon.py
 tests/test_job_x.py
 tests/test_jupyter.py
 tests/test_launcher.py
 tests/test_launcher_capacity.py
 tests/test_launcher_direct.py
 tests/test_launcher_multiple.py
@@ -316,15 +331,17 @@
 tests/configurations/ptyrex_configfiles/region_p4_p6.json
 tests/datafiles/dawn2_configuration.json
 tests/datafiles/i22-4996.nxs
 tests/datafiles/gaml/workflow1/settings.yaml
 tests/datafiles/gaml/workflow2/settings.yaml
 tests/jupyter/execute.sh
 tests/jupyter/jupyter1.ipynb
+tests/jupyter/jupyter2.ipynb
 tests/jupyter/jupyter_bad_cell.ipynb
+tests/jupyter/random_string.png
 tests/notebooks/c.ipynb
 tests/stub_commands/dawn
 tests/stub_commands/mpirun
 tests/stub_commands/ptychotools.ptypy_mpi_recipe
 tests/task_classes/task_z.py
 tests/workflows/__init__.py
 tests/workflows/base.py
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow.egg-info/requires.txt` & `dls-bxflow-2.3.0/src/dls_bxflow.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 nbformat
 pika
 prettytable
 pyyaml
 ruamel.yaml
 stomp.py
 workflows
+beautifulsoup4
 
 [dev]
 black==22.12.0
 mypy
 flake8-isort
 Flake8-pyproject
 pipdeptree
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/constants.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/bx_databases/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     DIRECTORY = "directory"
     BEAMLINE = "beamline"
     VISIT = "visit"
     BX_CATALOG_UUID = "bx_catalog_uuid"
     BX_WORKFLOW_UUID = "bx_workflow_uuid"
     COMMENT = "comment"
     RATING = "rating"
+    EXECUTION_SUMMARY = "execution_summary"
 
 
 # ----------------------------------------------------------------------------------------
 class BxGateFieldnames:
     UUID = "uuid"
     CREATED_ON = "created_on"
     TYPE = "type"
@@ -63,14 +64,15 @@
     launch_info = "launch_info"
     STATE = "state"
     SPECIFICATION = "specification"
     LABEL = "label"
     DIRECTORY = "directory"
     EXIT_CODE = "exit_code"
     ERROR_LINES = "error_lines"
+    EXECUTION_SUMMARY = "execution_summary"
 
 
 # ----------------------------------------------------------------------------------------
 class RelationFieldnames:
     LHS = "lhs"
     RHS = "rhs"
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,29 @@
 
     # ----------------------------------------------------------------------------------------
     async def update_bx_job(self, row):
         """"""
         return await self.__send_protocolj("update_bx_job", row)
 
     # ----------------------------------------------------------------------------------------
+    async def update_bx_job_execution_summary(
+        self,
+        bx_job_uuid,
+        task_execution_summary,
+        why=None,
+    ):
+        """"""
+        return await self.__send_protocolj(
+            "update_bx_job_execution_summary",
+            bx_job_uuid,
+            task_execution_summary,
+            why=why,
+        )
+
+    # ----------------------------------------------------------------------------------------
     async def cancel_bx_job(self, bx_job_uuid):
         """"""
         return await self.__send_protocolj("cancel_bx_job", bx_job_uuid)
 
     # ----------------------------------------------------------------------------------------
     async def delete_bx_job(self, bx_job_uuid):
         """ """
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/exceptions.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/remex.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/remex.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/thing.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_api/things.py` & `dls-bxflow-2.3.0/src/dls_bxflow_api/things.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/dataface_client.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/dataface_client.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/filestore.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/news_consumer.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/contexts/news_consumer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/main.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/execute_workflow.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/find_xanes.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/find_xanes.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/fire_i22.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/fire_i22.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/recipe_parser.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/recipe_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_dcg.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/report_dcg.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_ispyb.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/report_ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/start_services.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/submit.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/subcommands/submit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_cli/version.py` & `dls-bxflow-2.3.0/src/dls_bxflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/__main__.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gdascan.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/gdascan.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/manual.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/manual.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/scraper.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_collectors/scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/bx_composers.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/bx_composers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/html.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,15 +354,23 @@
                 f"<div class='T_cell'"
                 f" workflow_filename_classname='{workflow_filename_classname}'"
                 f" data_label='{data_label}'"
                 f" job_label='{job_label}'"
                 f" class='{action_class}'>"
             )
 
-        html_lines.append(f"<div class='T_box T_clickable T_{state}'></div>")
+        html_lines.append(f"<div class='T_box T_{state}'></div>")
+        execution_summary = data_cell.get("execution_summary")
+        if execution_summary is None:
+            execution_summary = ""
+        else:
+            execution_summary = execution_summary.strip()
+
+        html_lines.append(f"<div class='T_execution_summary'>{execution_summary}</div>")
+
         html_lines.append("</div>")
 
         composed = "".join(html_lines)
 
         return composed
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         table = prettytable.PrettyTable()
         table.field_names = [
             "created_on",
             "job",
             "task",
             "topic",
-            # TODO: Compose news details to open under click.
+            # TODO: Compose news details to open under click or hover.
             # "details",
         ]
 
         rows = []
         for record in records:
             row = []
             topic = record["topic"]
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/text.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_composers/text.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/classic.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     NewsFieldnames,
     RelationFieldnames,
     RevisionFieldnames,
 )
 
 logger = logging.getLogger(__name__)
 
-LATEST_REVISION = 4
+LATEST_REVISION = 5
 
 
 # ----------------------------------------------------------------------------------------
 class Aiosqlite:
     """
     Class with coroutines for creating and querying a sqlite database.
     """
@@ -157,14 +157,23 @@
                 % (
                     "bx_launchers",
                     BxLauncherFieldnames.REMEX_CLUSTER,
                     "bx_launchers",
                     BxLauncherFieldnames.REMEX_CLUSTER,
                 )
             )
+        if revision == 5:
+            await self.execute(
+                f"ALTER TABLE bx_jobs ADD COLUMN {BxJobFieldnames.EXECUTION_SUMMARY} TEXT",
+                why="for revision 5",
+            )
+            await self.execute(
+                f"ALTER TABLE bx_tasks ADD COLUMN {BxTaskFieldnames.EXECUTION_SUMMARY} TEXT",
+                why="for revision 5",
+            )
 
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
 
         if self._connection is not None:
             await self._connection.close()
 
@@ -428,14 +437,18 @@
         self._fields[BxJobFieldnames.DIRECTORY] = {"type": "TEXT", "index": True}
         self._fields[BxJobFieldnames.BEAMLINE] = {"type": "TEXT", "index": True}
         self._fields[BxJobFieldnames.VISIT] = {"type": "TEXT", "index": True}
         self._fields[BxJobFieldnames.BX_CATALOG_UUID] = {"type": "TEXT", "index": True}
         self._fields[BxJobFieldnames.BX_WORKFLOW_UUID] = {"type": "TEXT", "index": True}
         self._fields[BxJobFieldnames.COMMENT] = {"type": "TEXT", "index": False}
         self._fields[BxJobFieldnames.RATING] = {"type": "INTEGER", "index": True}
+        self._fields[BxJobFieldnames.EXECUTION_SUMMARY] = {
+            "type": "TEXT",
+            "index": False,
+        }
 
 
 # ----------------------------------------------------------------------------------------
 class BxGatesTable(BaseTable):
     # ----------------------------------------------------------------------------------------
     def __init__(self, database):
         BaseTable.__init__(self, database, "bx_gates")
@@ -494,14 +507,18 @@
         }
         self._fields[BxTaskFieldnames.STATE] = {"type": "TEXT", "index": True}
         self._fields[BxTaskFieldnames.SPECIFICATION] = {"type": "TEXT", "index": False}
         self._fields[BxTaskFieldnames.LABEL] = {"type": "TEXT", "index": True}
         self._fields[BxTaskFieldnames.DIRECTORY] = {"type": "TEXT", "index": True}
         self._fields[BxTaskFieldnames.EXIT_CODE] = {"type": "INTEGER", "index": True}
         self._fields[BxTaskFieldnames.ERROR_LINES] = {"type": "TEXT", "index": False}
+        self._fields[BxTaskFieldnames.EXECUTION_SUMMARY] = {
+            "type": "TEXT",
+            "index": False,
+        }
 
 
 # ----------------------------------------------------------------------------------------
 class BxTaskDependencyBxGatesTable(BaseTable):
     # ----------------------------------------------------------------------------------------
     def __init__(self, database):
         BaseTable.__init__(self, database, "bx_task_dependency_bx_gates")
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/bx_databases.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_databases/bx_databases.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 import shutil
 
+# Specific fields we want to access by symbolic constant.
+from dls_bxflow_api.bx_databases.constants import BxJobFieldnames
+
 # Base class for generic things.
 from dls_bxflow_api.thing import Thing
 
 # Database manager.
 from dls_bxflow_lib.bx_databases.bx_databases import BxDatabases
 
 # News producer.
@@ -474,14 +477,50 @@
 
         if count > 0:
             await self.__news_producer.update_bx_job(row, why=why)
 
         return {"count": count}
 
     # ----------------------------------------------------------------------------------------
+    async def update_bx_job_execution_summary(
+        self,
+        bx_job_uuid,
+        task_execution_summary,
+        why=None,
+    ):
+        """
+        Add a task's execution summary to the job's execution summary.
+
+        Called when task is finished.
+        """
+        await self.establish_database_connection()
+
+        # Get the current job's record.
+        record = await self.get_bx_job(bx_job_uuid)
+
+        if record is not None:
+            # Append the task's execution summary to the job's existing one.
+            # No spacing or newlines are added since the caller is responsible to format everything.
+            # TODO: Use ExecutionSummary class to manage the merging of a tasks' summary into a job's.
+            job_execution_summary = record[BxJobFieldnames.EXECUTION_SUMMARY]
+            if job_execution_summary is not None:
+                job_execution_summary += task_execution_summary
+            else:
+                job_execution_summary = task_execution_summary
+
+            # Update the job record with the new value.
+            # TODO: Lock against multiple threads calling update_bx_job_execution_summary.
+            row = {BxJobFieldnames.EXECUTION_SUMMARY: job_execution_summary}
+            await self.__database.bx_jobs_table.update(
+                row,
+                f"uuid = '{bx_job_uuid}'",
+                why=why,
+            )
+
+    # ----------------------------------------------------------------------------------------
     async def cancel_bx_job(self, bx_job_uuid):
         """"""
         return await self.update_bx_job(
             {"uuid": bx_job_uuid, "state": BxJobStates.CANCELLED}
         )
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/explicit.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/explicit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/scandir.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_filestores/scandir.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/html.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_gamls/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import asyncio
 import inspect
 import json
 import logging
 import multiprocessing
 import threading
 
+from dls_multiconf_lib.exceptions import NotFound as MulticonfNotFound
+
 # Utilities.
 from dls_utilpack.callsign import callsign, callsign_html
 from dls_utilpack.describe import describe
 from dls_utilpack.import_class import import_class
 from dls_utilpack.require import require
 
 # Database field names.
@@ -515,36 +517,36 @@
         )
 
         # Get the columns as specified from the configurator.
         try:
             prepend_job_labels = bx_configurators_get_default().require(
                 "gui.job_data_grid.prepend_job_labels"
             )
-        except NotFound:
+        except MulticonfNotFound:
             prepend_job_labels = None
 
         try:
             append_job_labels = bx_configurators_get_default().require(
                 "gui.job_data_grid.append_job_labels"
             )
-        except NotFound:
+        except MulticonfNotFound:
             append_job_labels = None
 
         try:
             specific_job_labels = bx_configurators_get_default().require(
                 "gui.job_data_grid.specific_job_labels"
             )
-        except NotFound:
+        except MulticonfNotFound:
             specific_job_labels = None
 
         try:
             exclude_job_labels = bx_configurators_get_default().require(
                 "gui.job_data_grid.exclude_job_labels"
             )
-        except NotFound:
+        except MulticonfNotFound:
             exclude_job_labels = None
 
         # Compose the html using prettytable, with special cell composer method.
         html = bx_composers_get_default().compose_bx_jobs_data_grid(
             records,
             append_job_labels=append_job_labels,
             prepend_job_labels=prepend_job_labels,
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/bx_guis.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/bx_guis.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/constants.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/curses.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/curses.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/index.html` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/standard.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_jobs/standard.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         self.__bx_dataface = bx_datafaces_get_default()
 
         self._bx_jobs = BxJobs()
 
         self._bx_tasks = BxTasks()
 
         # Number of concurrent tasks we will support.
-        # TODO: In aiohttp rBxLauncher, make task count max configurable.
         self.__task_count_max = specification["type_specific_tbd"].get(
             "task_count_max", 10
         )
         self.__task_count_now = 0
 
         # This flag will stop the ticking async task.
         self.__keep_ticking = True
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import yaml
 
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain, explain_cause_chain_error_lines
 from dls_utilpack.require import require
 
+# Specific field names we want to use symobolic constants.
+from dls_bxflow_api.bx_databases.constants import BxTaskFieldnames
+
 # Global bx_dataface.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Exceptions.
 from dls_bxflow_api.exceptions import CapacityReached
 
 # Base class which maps flask bx_tasks to methods.
@@ -32,14 +35,15 @@
 from dls_bxflow_lib.bx_launchers.states import States as BxLauncherStates
 
 # BxTasks manager.
 from dls_bxflow_run.bx_tasks.bx_tasks import BxTasks
 
 # BxTask configuration keywords.
 from dls_bxflow_run.bx_tasks.constants import Keywords as BxTaskKeywords
+from dls_bxflow_run.bx_tasks.execution_summary import ExecutionSummary
 from dls_bxflow_run.bx_tasks.states import States as BxTaskStates
 
 
 class EXIT_CODES:
     PREPARE_ENVIRONMENT = 252
 
 
@@ -156,15 +160,15 @@
 
     async def presubmit(
         self, bx_job_uuid, bx_job_specification, bx_task_uuid, bx_task_specification
     ):
         # Increment task count.
         if self.__task_count_now == self.__task_count_max:
             # Reply to client.
-            # TODO: In aiohttp rBxLauncher, give special http status to indicate task count max exceeded.
+            # TODO: In aiohttp BxLauncher, give special http status to indicate task count max exceeded.
             raise CapacityReached(
                 callsign(
                     self,
                     f"[TASKCNT] cannot submit a new task because {self.__task_count_max} already underway in this launcher",
                 )
             )
 
@@ -437,29 +441,42 @@
         """
 
         try:
             # Catalog any artefacts left by the task.
             await self._catalog_artefacts(bx_job, bx_task)
 
             # Get the task post-run information for the database record.
-            exit_code, error_lines, gate_label = self.get_post_run_fields_after_run(
+            (
+                exit_code,
+                error_lines,
+                gate_label,
+                execution_summary,
+            ) = self.get_post_run_fields_after_run(
                 bx_job,
                 bx_task,
             )
 
             # Update the state of the bx_task we ran.
             await self.__bx_dataface.update_bx_task(
                 {
                     "uuid": bx_task.uuid(),
                     "state": BxTaskStates.FINISHED,
                     "exit_code": exit_code,
                     "error_lines": "\n".join(error_lines),
+                    BxTaskFieldnames.EXECUTION_SUMMARY: execution_summary,
                 }
             )
 
+            # Append the task's execution summary to the bx_job's.
+            if execution_summary is not None:
+                await self.__bx_dataface.update_bx_job_execution_summary(
+                    bx_task.bx_job_uuid(),
+                    execution_summary,
+                )
+
             # Update the gate which allows other tasks to run and/or the job to block.
             await self.__bx_dataface.open_bx_gate(bx_task.uuid(), gate_label)
 
             # Update the bx_job state if it is now blocked.
             await self.__bx_dataface.update_bx_job_if_blocked_by_bx_gates(
                 bx_task.bx_job_uuid()
             )
@@ -521,15 +538,24 @@
             gate_label = "success"
 
         else:
             # Get task post-run fields after the task finished running.
             error_lines = bx_task.extract_error_lines()
             gate_label = "failure"
 
-        return exit_code, error_lines, gate_label
+        execution_summary_filename = (
+            f"{runtime_directory}/{ExecutionSummary().filename}"
+        )
+        if os.path.exists(execution_summary_filename):
+            with open(execution_summary_filename, "r") as stream:
+                execution_summary = stream.read()
+        else:
+            execution_summary = None
+
+        return exit_code, error_lines, gate_label, execution_summary
 
     # ------------------------------------------------------------------------------------------
 
     def get_post_run_fields_after_launch_fail(
         self, bx_job, bx_task, arrived_future_exception
     ):
         """
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/island.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/island.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/popener.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/popener.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/qsubber.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_launchers/qsubber.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/graylogger.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_logstores/graylogger.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aio_pika.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/aio_pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/bx_news.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/bx_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/constants.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/pika.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/context.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/dask.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/dask.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/naive.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/boolean.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/boolean.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/bx_settings.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/bx_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/float.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/float.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/integer.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/integer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/string.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_settings/string.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/main.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/writer.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/dummies/writer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/envvar.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/overall.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/overall.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/parser1.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/recipe_parser/parser1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_lib/version.py` & `dls-bxflow-2.3.0/src/dls_bxflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/bx_gates.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_gates/bx_gates.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/constants.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn1.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn2.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn_base.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dawn_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dummy.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/filename_classname.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/filename_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/jupyter.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/jupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,29 @@
 
 
 class Jupyter(Base):
     """ """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None, predefined_uuid=None):
-        Base.__init__(self, thing_type, specification, predefined_uuid=predefined_uuid)
+        Base.__init__(
+            self,
+            thing_type,
+            specification,
+            predefined_uuid=predefined_uuid,
+        )
 
         self.state(States.PREPARED)
 
         self.__modify_cells = None
 
     # ----------------------------------------------------------------------------------------
     def modify_notebook(self, notebook):
         """
-        Offer opportunity to modify notebook.
+        Modify the notebook's cells.
         """
 
         if self.__modify_cells is None:
             return notebook
 
         for index, contents in self.__modify_cells.items():
             index = int(index)
@@ -70,19 +75,23 @@
             os.environ["PYDEVD_DISABLE_FILE_VALIDATION"] = "1"
 
         # Jupyter.
         import nbformat
         from nbconvert import HTMLExporter
 
         type_specific_tbd = require(
-            f"{callsign(self)} specification", self.specification(), "type_specific_tbd"
+            f"{callsign(self)} specification",
+            self.specification(),
+            "type_specific_tbd",
         )
 
         ipynb_filename = require(
-            f"{callsign(self)} specification", type_specific_tbd, "ipynb_filename"
+            f"{callsign(self)} specification",
+            type_specific_tbd,
+            "ipynb_filename",
         )
 
         self.__modify_cells = type_specific_tbd.get("modify_cells")
 
         # Read the notebook into memory.
         logger.debug(f"reading notebook template from {ipynb_filename}")
         with open(ipynb_filename, "r") as stream:
@@ -95,15 +104,15 @@
         sanitized_label = sanitize(self.label())
         # cwd_ipynb_filename = f"{sanitized_label}-{os.path.basename(ipynb_filename)}"
         cwd_ipynb_filename = f"{sanitized_label}.ipynb"
 
         execution_exception = None
 
         # The task specification contains a command?
-        if "command" in self.specification()["type_specific_tbd"]:
+        if "command" in type_specific_tbd:
             try:
                 # Execute the notebook from within a shell script.
                 await self.execute_in_script(notebook, cwd_ipynb_filename)
             except Exception as exception:
                 logger.warning(
                     explain2(exception, "executing notebook in a shell script"),
                     exc_info=exception,
```

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/module_classname.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/module_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/pickled_class.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/pickled_class.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/shell.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/symlink.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_tasks/symlink.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/bx_variables.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/bx_variables/bx_variables.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/src/dls_bxflow_run/main_isolated.py` & `dls-bxflow-2.3.0/src/dls_bxflow_run/main_isolated.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/base.py` & `dls-bxflow-2.3.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/base_context_tester.py` & `dls-bxflow-2.3.0/tests/base_context_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import asyncio
 import logging
 import multiprocessing
 import os
 
 import pytest
+
+# Configuration manager for multi-service systems.
 from dls_multiconf_lib.constants import ThingTypes as MulticonfThingTypes
 
 # Object managers we interact with.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Results composers.
 from dls_bxflow_lib.bx_composers.bx_composers import BxComposers
```

### Comparing `dls-bxflow-2.2.0/tests/base_specification_tester.py` & `dls-bxflow-2.3.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/base_tester.py` & `dls-bxflow-2.3.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/configurations/backend.yaml` & `dls-bxflow-2.3.0/tests/configurations/backend.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,17 @@
     type_specific_tbd:
         # The remote dataface server access.
         aiohttp_specification:
             server: *DLS_SERVBASE_DATAFACE_SERVER
             client: *DLS_SERVBASE_DATAFACE_CLIENT
         # The local implementation of the dataface.
         actual_dataface_specification:
-            type: "dls_servbase_lib.datafaces.aiosqlite"
+            type: "dls_servbase_lib.datafaces.normsql"
             database:
-                type: "dls_servbase_lib.databases.aiosqlite"
+                type: "dls_normsql.aiosqlite"
                 filename: "${output_directory}/dls_servbase_dataface.sqlite"
                 log_level: "WARNING"
     context:
         start_as: process
 
 # The bx_dataface client/server composite.
 bx_dataface_specification: &BX_DATAFACE_SPECIFICATION
```

### Comparing `dls-bxflow-2.2.0/tests/configurations/filestore.yaml` & `dls-bxflow-2.3.0/tests/configurations/filestore.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml` & `dls-bxflow-2.3.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json` & `dls-bxflow-2.3.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/conftest.py` & `dls-bxflow-2.3.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     logging.getLogger("dls_bxflow_lib.base_aiohttp").setLevel("INFO")
 
     # Messages about starting tasks and isolation.
     logging.getLogger("dls_bxflow_lib.bx_launchers.aiohttp").setLevel("INFO")
     logging.getLogger("dls_bxflow_lib.bx_launchers.base").setLevel("INFO")
 
     # All bxflow database sql commands.
-    logging.getLogger("dls_bxflow_lib.bx_databases.aiosqlite").setLevel("INFO")
+    # logging.getLogger("dls_bxflow_lib.bx_databases.aiosqlite").setLevel("INFO")
 
     # All ispyb database sql commands.
     # logging.getLogger("dls_bxflow_lib.bx_catalogs.ispyb").setLevel("INFO")
 
     logging.getLogger("dls_bxflow_lib.bx_contexts.classic").setLevel("INFO")
     logging.getLogger("dls_bxflow_lib.bx_news.context").setLevel("INFO")
     logging.getLogger("dls_bxflow_lib.bx_datafaces.context").setLevel("INFO")
```

### Comparing `dls-bxflow-2.2.0/tests/datafiles/dawn2_configuration.json` & `dls-bxflow-2.3.0/tests/datafiles/dawn2_configuration.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/datafiles/i22-4996.nxs` & `dls-bxflow-2.3.0/tests/datafiles/i22-4996.nxs`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/gda_parser.py` & `dls-bxflow-2.3.0/tests/gda_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/gda_workflow.py` & `dls-bxflow-2.3.0/tests/gda_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/jupyter/jupyter1.ipynb` & `dls-bxflow-2.3.0/tests/jupyter/jupyter1.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/jupyter/jupyter_bad_cell.ipynb` & `dls-bxflow-2.3.0/tests/jupyter/jupyter_bad_cell.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/notebooks/c.ipynb` & `dls-bxflow-2.3.0/tests/notebooks/c.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/qacct` & `dls-bxflow-2.3.0/tests/qacct`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/qstat` & `dls-bxflow-2.3.0/tests/qstat`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe` & `dls-bxflow-2.3.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_catalog.py` & `dls-bxflow-2.3.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_collector.py` & `dls-bxflow-2.3.0/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_collector_scraper.py` & `dls-bxflow-2.3.0/tests/test_collector_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_composer.py` & `dls-bxflow-2.3.0/tests/test_composer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from bs4 import BeautifulSoup
+
 # Object managing datafaces.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Results composers.
 from dls_bxflow_lib.bx_composers.bx_composers import BxComposers
 
 # Context creator.
@@ -63,14 +65,15 @@
                         bx_job_dict = {
                             "created_on": "2022-08-27 13:30:21",
                             "uuid": bx_job_uuid,
                             "bx_workflow_uuid": bx_workflow_uuid,
                             "label": f"job{job_number}",
                             "data_label": f"data{data_number}",
                             "state": "GOOD",
+                            "execution_summary": f"summary for data {data_number}, job {job_number}",
                         }
                     bx_job_dicts.append(bx_job_dict)
 
                     # Add a workflow for every job.
                     bx_workflow_dict = {
                         "uuid": bx_workflow_uuid,
                         "bx_job_uuid": bx_job_uuid,
@@ -149,14 +152,31 @@
                 prepend_job_labels=prepend_job_labels,
                 append_job_labels=append_job_labels,
                 exclude_job_labels=exclude_job_labels,
             )
 
             logger.debug(f"composed html\n{html}")
 
+            soup = BeautifulSoup(html, "html.parser")
+
+            # Find the table element.
+            table = soup.find("table")
+
+            # Count the number of rows in the table.
+            rows = table.find_all("tr")
+
+            # Assert that the row count is equal to the expected value.
+            assert len(rows) == 5
+
+            # Check the first row's columns.
+            # Wells are injected with increasing crystal counts, so default sorting is in reverse order.
+            row = rows[1]
+            columns = row.find_all("td")
+            assert len(columns) == 6
+
             # -----------------------------------------------------------------
             # Grid with no records.
             records = {}
 
             text_composer = BxComposers().build_object(
                 {"type": "dls_bxflow_lib.bx_composers.text"}
             )
```

### Comparing `dls-bxflow-2.2.0/tests/test_configurator.py` & `dls-bxflow-2.3.0/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_database.py` & `dls-bxflow-2.3.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_dataface.py` & `dls-bxflow-2.3.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_dawn1.py` & `dls-bxflow-2.3.0/tests/test_dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_dawn2.py` & `dls-bxflow-2.3.0/tests/test_dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_extract_error_lines_dawn.py` & `dls-bxflow-2.3.0/tests/test_extract_error_lines_dawn.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_extract_error_lines_dummy.py` & `dls-bxflow-2.3.0/tests/test_extract_error_lines_dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_filestore.py` & `dls-bxflow-2.3.0/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_gaml.py` & `dls-bxflow-2.3.0/tests/test_gaml.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_gui.py` & `dls-bxflow-2.3.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_job_a.py` & `dls-bxflow-2.3.0/tests/test_job_a.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import logging
 import os
 
 # Utilities.
 from dls_utilpack.describe import describe
 
+from dls_bxflow_api.bx_databases.constants import BxJobFieldnames
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Remote execution.
 from dls_bxflow_api.remex import Clusters as RemexClusters
 from dls_bxflow_api.remex import Keywords as RemexKeywords
 
 # Context creator.
@@ -25,20 +26,23 @@
 
 # News events.
 from dls_bxflow_lib.bx_news.constants import Topics as BxNewsTopics
 
 # Object managing bx_tasks.
 from dls_bxflow_run.bx_tasks.bx_tasks import BxTasks
 from dls_bxflow_run.bx_tasks.constants import Keywords as BxTaskKeywords
+from dls_bxflow_run.bx_tasks.execution_summary import ExecutionSummary
 
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
+SOME_EXECUTION_SUMMARY_TEXT = "some text"
+
 
 # ----------------------------------------------------------------------------------------
 class TestJobALaptop:
     def test(self, constants, logging_setup, output_directory):
         """ """
 
         configuration_file = "tests/configurations/backend.yaml"
@@ -55,14 +59,16 @@
         self.outfile = outfile
         self.algorithm = algorithm
 
     async def run(self):
         logger.info("running Aclass")
         with open(self.outfile, "wt") as stream:
             stream.write(self.algorithm)
+        # Append some raw text to execution summary.
+        ExecutionSummary().append_raw(SOME_EXECUTION_SUMMARY_TEXT)
 
 
 # Pythonpath where the Aclass can be found
 aclass_pythonpath = "%s:%s" % (
     os.path.dirname(os.path.dirname(__file__)),
     os.environ.get("PYTHONPATH", ""),
 )
@@ -157,14 +163,27 @@
             # Verify the output file contents from the task.
             self._assert_execution_output(
                 "aclass_datafile.txt",
                 self.tasks_execution_outputs[aclass_bx_task.uuid()],
                 expected_content=aclass_algorithm,
             )
 
+            # Verify the output file contents from the execution summary written by the task.
+            self._assert_execution_output(
+                ExecutionSummary().filename,
+                self.tasks_execution_outputs[aclass_bx_task.uuid()],
+                expected_content=SOME_EXECUTION_SUMMARY_TEXT,
+            )
+
+            # Verify that the bx_job record has the execution summary from the task.
+            record = await bx_datafaces_get_default().get_bx_job(bx_job.uuid())
+            assert (
+                record[BxJobFieldnames.EXECUTION_SUMMARY] == SOME_EXECUTION_SUMMARY_TEXT
+            )
+
             # Delete the job and all related records and directories.
             await bx_datafaces_get_default().delete_bx_job(bx_job.uuid())
 
             assert not os.path.exists(bx_job.get_directory())
             for bx_task in bx_job.bx_tasks.list():
                 assert not os.path.exists(bx_task.get_directory())
             records = await bx_datafaces_get_default().get_bx_jobs()
```

### Comparing `dls-bxflow-2.2.0/tests/test_job_a_bc_d.py` & `dls-bxflow-2.3.0/tests/test_job_a_bc_d.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,14 @@
         """ """
 
         configuration_file = "tests/configurations/backend.yaml"
         JobABcDTester().main(constants, configuration_file, output_directory)
 
 
 # ----------------------------------------------------------------------------------------
-class Aclass:
-    """
-    This is a user-defined class which gets instantiated and called at runtime.
-    """
-
-    def __init__(self, outfile, algorithm=None):
-        self.outfile = outfile
-        self.algorithm = algorithm
-
-    async def run(self):
-        logger.info("running Aclass")
-        with open(self.outfile, "wt") as stream:
-            stream.write(self.algorithm)
-
-
-# ----------------------------------------------------------------------------------------
 class JobABcDTester(BaseContextTester):
     """
     Class to test diamond-shaped dag job creation and running directly, without a workflow involved.
     """
 
     async def _main_coroutine(self, constants, output_directory):
         """ """
```

### Comparing `dls-bxflow-2.2.0/tests/test_job_pubcon.py` & `dls-bxflow-2.3.0/tests/test_job_pubcon.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_job_x.py` & `dls-bxflow-2.3.0/tests/test_job_x.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_jupyter.py` & `dls-bxflow-2.3.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_launcher.py` & `dls-bxflow-2.3.0/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_launcher_capacity.py` & `dls-bxflow-2.3.0/tests/test_launcher_capacity.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_launcher_direct.py` & `dls-bxflow-2.3.0/tests/test_launcher_direct.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_launcher_multiple.py` & `dls-bxflow-2.3.0/tests/test_launcher_multiple.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_launcher_restart.py` & `dls-bxflow-2.3.0/tests/test_launcher_restart.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_logstore.py` & `dls-bxflow-2.3.0/tests/test_logstore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_news.py` & `dls-bxflow-2.3.0/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_protocolj.py` & `dls-bxflow-2.3.0/tests/test_protocolj.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_ptypy_mpi.py` & `dls-bxflow-2.3.0/tests/test_ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_ptyrex_mpi.py` & `dls-bxflow-2.3.0/tests/test_ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_scheduler_naive.py` & `dls-bxflow-2.3.0/tests/test_scheduler_naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_settings.py` & `dls-bxflow-2.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_shell.py` & `dls-bxflow-2.3.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_task.py` & `dls-bxflow-2.3.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_workflow.py` & `dls-bxflow-2.3.0/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/test_workflow_finder.py` & `dls-bxflow-2.3.0/tests/test_workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/a/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/a/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/b/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/b/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/base.py` & `dls-bxflow-2.3.0/tests/workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/c/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/c/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/e/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/e/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/f/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/f/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/g/workflow.py` & `dls-bxflow-2.3.0/tests/workflows/g/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.2.0/tests/workflows/utilities.py` & `dls-bxflow-2.3.0/tests/workflows/utilities.py`

 * *Files identical despite different names*


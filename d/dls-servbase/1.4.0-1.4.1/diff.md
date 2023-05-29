# Comparing `tmp/dls-servbase-1.4.0.tar.gz` & `tmp/dls-servbase-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.4.0.tar", last modified: Fri May 26 07:16:01 2023, max compression
+gzip compressed data, was "dls-servbase-1.4.1.tar", last modified: Mon May 29 14:11:43 2023, max compression
```

## Comparing `dls-servbase-1.4.0.tar` & `dls-servbase-1.4.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.554571 dls-servbase-1.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/good_config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:16:01.566571 dls-servbase-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.550571 dls-servbase-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 07:16:01.000000 dls-servbase-1.4.0/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.558571 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:16:01.562571 dls-servbase-1.4.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/configurations/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/configurations/sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-26 07:15:51.000000 dls-servbase-1.4.0/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.166787 dls-servbase-1.4.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.166787 dls-servbase-1.4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/good_config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.170787 dls-servbase-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_gui.py
```

### Comparing `dls-servbase-1.4.0/.dae-devops/Makefile` & `dls-servbase-1.4.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/conventions.rst` & `dls-servbase-1.4.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/developing.rst` & `dls-servbase-1.4.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/devops.rst` & `dls-servbase-1.4.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.4.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/installing.rst` & `dls-servbase-1.4.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/docs/testing.rst` & `dls-servbase-1.4.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.dae-devops/project.yaml` & `dls-servbase-1.4.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.devcontainer/Dockerfile` & `dls-servbase-1.4.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.devcontainer/devcontainer.json` & `dls-servbase-1.4.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/CONTRIBUTING.rst` & `dls-servbase-1.4.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/actions/install_requirements/action.yml` & `dls-servbase-1.4.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/dependabot.yml` & `dls-servbase-1.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/pages/make_switcher.py` & `dls-servbase-1.4.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/workflows/code.yml` & `dls-servbase-1.4.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/workflows/docs.yml` & `dls-servbase-1.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/workflows/docs_clean.yml` & `dls-servbase-1.4.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.github/workflows/linkcheck.yml` & `dls-servbase-1.4.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.gitignore` & `dls-servbase-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.gitlab-ci.yml` & `dls-servbase-1.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/.vscode/launch.json` & `dls-servbase-1.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/LICENSE` & `dls-servbase-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/PKG-INFO` & `dls-servbase-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.4.0/README.rst` & `dls-servbase-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/docs/conf.py` & `dls-servbase-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/docs/images/dls-favicon.ico` & `dls-servbase-1.4.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/docs/images/dls-logo.svg` & `dls-servbase-1.4.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/pyproject.toml` & `dls-servbase-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.4.1/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-servbase-1.4.0/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.4.1/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.4.1/src/dls_servbase_api/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/databases/database_definition.py` & `dls-servbase-1.4.1/src/dls_servbase_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/databases/table_definitions.py` & `dls-servbase-1.4.1/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_cli/main.py` & `dls-servbase-1.4.1/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_cli/subcommands/start_services.py` & `dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_cli/version.py` & `dls-servbase-1.4.1/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/base_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/base.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/classic.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/contexts/contexts.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         )
 
         self.__actual_dls_servbase_dataface = None
 
     # ----------------------------------------------------------------------------------------
     def callsign(self):
         """"""
-        return "%s %s" % ("Dataface.Aiohttp", BaseAiohttp.callsign(self))
+        return "%s %s" % ("Servbase.Dataface", BaseAiohttp.callsign(self))
 
     # ----------------------------------------------------------------------------------------
     def activate_process(self):
         """"""
 
         try:
             multiprocessing.current_process().name = "servbase-dataface"
@@ -64,15 +64,15 @@
     # ----------------------------------------------------------------------------------------
     def activate_thread(self, loop):
         """
         Called from inside a newly created thread.
         """
 
         try:
-            threading.current_thread().name = "dls_servbase_dataface"
+            threading.current_thread().name = "servbase_dataface"
 
             self.activate_thread_base(loop)
 
         except Exception as exception:
             logger.exception(
                 f"unable to start {callsign(self)} thread", exc_info=exception
             )
@@ -95,15 +95,24 @@
             await self.__actual_dls_servbase_dataface.start()
 
             logger.debug(f"calling coro of {callsign(self)}")
 
             await self.activate_coro_base(route_tuples)
 
         except Exception:
-            raise RuntimeError(f"unable to start {callsign(self)} server coro")
+            # We managed to get a dataface alive?
+            if self.__actual_dls_servbase_dataface is not None:
+                # Need to disconnect it so outer asyncio loop will quit.
+                logger.debug(
+                    f"[THRDIEP] {callsign(self)} disconnecting after failure to activate coro"
+                )
+
+                await self.__actual_dls_servbase_dataface.disconnect()
+
+            raise RuntimeError(f"{callsign(self)}  was unable to activate_coro")
 
     # ----------------------------------------------------------------------------------------
     async def direct_shutdown(self):
         """"""
         try:
             # Disconnect our local dataface connection, i.e. the one which holds the database connection.
             await self.__actual_dls_servbase_dataface.disconnect()
```

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/datafaces/normsql.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     async def start(self):
         # Connect to the database to create the schemas if they don't exist already.
         await self.establish_database_connection()
 
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
         if self.__database is not None:
+            logger.debug(
+                "[DISSHU] disconnecting from actual servbase dataface normsql implementation"
+            )
             await self.__database.disconnect()
             self.__database = None
 
     # ----------------------------------------------------------------------------------------
     async def establish_database_connection(self):
 
         if self.__database is None:
```

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/src/dls_servbase_lib/version.py` & `dls-servbase-1.4.1/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/base.py` & `dls-servbase-1.4.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/base_context_tester.py` & `dls-servbase-1.4.1/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/base_specification_tester.py` & `dls-servbase-1.4.1/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/base_tester.py` & `dls-servbase-1.4.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/configurations/mysql.yaml` & `dls-servbase-1.4.1/tests/configurations/mysql.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/configurations/sqlite.yaml` & `dls-servbase-1.4.1/tests/configurations/sqlite.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/conftest.py` & `dls-servbase-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/test_aiohttp.py` & `dls-servbase-1.4.1/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/test_database.py` & `dls-servbase-1.4.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/test_dataface.py` & `dls-servbase-1.4.1/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/test_dataface_takeover.py` & `dls-servbase-1.4.1/tests/test_dataface_takeover.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.0/tests/test_gui.py` & `dls-servbase-1.4.1/tests/test_gui.py`

 * *Files identical despite different names*


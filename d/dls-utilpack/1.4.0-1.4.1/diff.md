# Comparing `tmp/dls-utilpack-1.4.0.tar.gz` & `tmp/dls-utilpack-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-utilpack-1.4.0.tar", last modified: Thu May 18 09:58:09 2023, max compression
+gzip compressed data, was "dls-utilpack-1.4.1.tar", last modified: Mon May 29 08:01:23 2023, max compression
```

## Comparing `dls-utilpack-1.4.0.tar` & `dls-utilpack-1.4.1.tar`

### file list

```diff
@@ -1,114 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.007123 dls-utilpack-1.4.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.007123 dls-utilpack-1.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.011123 dls-utilpack-1.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.015123 dls-utilpack-1.4.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.015123 dls-utilpack-1.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.007123 dls-utilpack-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.015123 dls-utilpack-1.4.0/src/dls_utilpack/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/global_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/isodatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/modify_process_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/qualname.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/require.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/search_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/visit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/src/dls_utilpack/whatenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-18 09:58:09.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 09:58:08.000000 dls-utilpack-1.4.0/src/dls_utilpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:58:09.019123 dls-utilpack-1.4.0/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_sigint1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_sigint2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_visit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-18 09:58:00.000000 dls-utilpack-1.4.0/tests/test_whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.339478 dls-utilpack-1.4.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.339478 dls-utilpack-1.4.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.343478 dls-utilpack-1.4.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.347478 dls-utilpack-1.4.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.347478 dls-utilpack-1.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.347478 dls-utilpack-1.4.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.347478 dls-utilpack-1.4.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.339478 dls-utilpack-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/src/dls_utilpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/global_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/isodatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/modify_process_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/require.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/search_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/src/dls_utilpack/whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 08:01:23.000000 dls-utilpack-1.4.1/src/dls_utilpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:01:23.351478 dls-utilpack-1.4.1/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_sigint1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_sigint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-29 08:01:10.000000 dls-utilpack-1.4.1/tests/test_whatenv.py
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/Makefile` & `dls-utilpack-1.4.1/.dae-devops/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint d63e047529404daf652476f24688ea34
+# dae_devops_fingerprint 9fb607f8a0919f7698390f71e8c16af4
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/conventions.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/conventions.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint 8dbc3a8375bfa18c5de367f43e940baa
+.. # dae_devops_fingerprint 5db630d2d15362b79c3189cffb34b1fe
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/developing.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/developing.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
 Make sure to have at least python version 3.9 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-utilpack
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
-.. # dae_devops_fingerprint 10795db3a0e161045debf0c89348bb24
+.. # dae_devops_fingerprint af2c010da25ab38673d57f4b32fc6704
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/devops.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/devops.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
 Devops
 =======================================================================
 
-There exists a a configuration file called ``.dae-devops/project.yaml``.
+In the top level of the repository there exists a configuration file called ``.dae-devops/project.yaml``.
 
 This file defines the project information needed for CI/CD.
 
 It is parsed by the ``dae_devops.force`` command which creates these files:
 
 - pyproject.toml
+- .githib/*
 - .gitlab-ci.yml
 - .dae-devops/Makefile
 - .dae-devops/docs/*
 
 Local CI/CD execution
------------------------------------------------------------------------
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 All the CI/CD ops which are run by the git server can be run at the command line.
 
 Running these ops before pushing to the git server can make the turnaround quicker to fix things.
 
 Follow the steps in the Developing section.  Then you can run the following commands.
 
 Validation of the code::
 
     $ make -f .dae-devops/Makefile validate_pre_commit
     $ make -f .dae-devops/Makefile validate_mypy
     $ make -f .dae-devops/Makefile validate_pytest
     $ make -f .dae-devops/Makefile validate_docs
 
-Packaging:: 
+Packaging (for the Diamond intranet):: 
 
     $ make -f .dae-devops/Makefile package_pip
 
-Publishing::
+Publishing (for the Diamond intranet)::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
+The Diamond intranet commands are not used for production. The production packaging and publishing are handled in the GitHub Actions workflows mechanism.
 
-
-.. # dae_devops_fingerprint d2bca688da0d1b2a93392bca1d74bcf9
+.. # dae_devops_fingerprint 322b02a91652f7af8cf6b5fce4f890c7
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/docs_structure.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/docs_structure.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint df17fb0c73cb2f5162b27c5689074969
+.. # dae_devops_fingerprint 8b513434fc0d2243c4577ba326cd01a7
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/installing.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/installing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
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
     $ python3 -m pip install dls-utilpack
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git
 
-The library should now be installed and the commandline interface on your path.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-utilpack --version
     $ dls-utilpack --version-json
 
-.. # dae_devops_fingerprint fa480c2e4f59a68b0ef91bf12e5f6b58
+.. # dae_devops_fingerprint b78ff60b9b00c9fbed98165726b1e7c3
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/docs/testing.rst` & `dls-utilpack-1.4.1/.dae-devops/docs/testing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
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
 
-    /tmp/dls-utilpack/tests/....
+    /tmp/dls-utilpack/tests/*
 
 The tests clear their directory when they start, but not when they finish.
-This allows peeking in there to see what's been written by the test.
+This allows you to examine what's been written by the test.
 
     
 
 
-.. # dae_devops_fingerprint 17ae8c603ffe73c0fbdfcda48e7881bb
+.. # dae_devops_fingerprint a922750b6063d262e4cc226776e7811b
```

### Comparing `dls-utilpack-1.4.0/.dae-devops/project.yaml` & `dls-utilpack-1.4.1/.dae-devops/project.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Primary information needed for devops.
 primary:
   repository_name: dls-utilpack
   package_name: dls_utilpack
-  one_line_description: "Collection of various useful Python classes and functions."
+  one_line_description: "Library of various useful Python classes and functions."
   author:
     name: David Erb
     email: david.erb@diamond.ac.uk
   project_urls:
     GitLab: https://gitlab.diamond.ac.uk/scisoft
   project_scripts:
     dls-utilpack: "dls_utilpack.__main__:main"
```

### Comparing `dls-utilpack-1.4.0/.devcontainer/Dockerfile` & `dls-utilpack-1.4.1/.devcontainer/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-utilpack"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 29e344c513daf6f125ee4e8388a06736
+# dae_devops_fingerprint 8bf76cbeec0f857b783974a6da52cdf6
```

### Comparing `dls-utilpack-1.4.0/.devcontainer/devcontainer.json` & `dls-utilpack-1.4.1/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.2.
+// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 // ********** For repository_name dls-utilpack
 
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
 
-// dae_devops_fingerprint 6f0e3415b3a297d5ce22f28b8dfbbd23
+// dae_devops_fingerprint 5288f44124d88a93c17aa2dd407c4070
```

### Comparing `dls-utilpack-1.4.0/.github/CONTRIBUTING.rst` & `dls-utilpack-1.4.1/.github/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.2.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-utilpack
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-utilpack/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint e29f699b807ff29198e97d0163468ccd
+.. # dae_devops_fingerprint 3fc775c530563a4170bd6898f939025a
```

### Comparing `dls-utilpack-1.4.0/.github/actions/install_requirements/action.yml` & `dls-utilpack-1.4.1/.github/actions/install_requirements/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
 
-# dae_devops_fingerprint ef652e9abab51b9fbb68a1010da09af7
+# dae_devops_fingerprint 383023749da2ee5e51e832d12c7c5bce
```

### Comparing `dls-utilpack-1.4.0/.github/dependabot.yml` & `dls-utilpack-1.4.1/.github/dependabot.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 9ddfc76e95e202063eea84301051a6f9
+# dae_devops_fingerprint 8b399a57f20ca5eae651fd5b5c4832f8
```

### Comparing `dls-utilpack-1.4.0/.github/pages/make_switcher.py` & `dls-utilpack-1.4.1/.github/pages/make_switcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 9de9ab0e7e88db7736d4bdc5b33bfe89
+# dae_devops_fingerprint ead516754f070c15d69e9d3ee8f2c2e2
```

### Comparing `dls-utilpack-1.4.0/.github/workflows/code.yml` & `dls-utilpack-1.4.1/.github/workflows/code.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 97cce24d579fe2cf6cc302e06dbd4836
+# dae_devops_fingerprint 4ab8a18cc4ae386356af332362670f74
```

### Comparing `dls-utilpack-1.4.0/.github/workflows/docs.yml` & `dls-utilpack-1.4.1/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 23b156a03b2f52b3c08ea9d4f6e622db
+# dae_devops_fingerprint 383dc518cf892cbcd0d00aed2bb77b78
```

### Comparing `dls-utilpack-1.4.0/.github/workflows/docs_clean.yml` & `dls-utilpack-1.4.1/.github/workflows/docs_clean.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 6906b07d0aafb39f92a25b57699a6cdd
+# dae_devops_fingerprint c6e4247b915efefed59258685bc6a04d
```

### Comparing `dls-utilpack-1.4.0/.github/workflows/linkcheck.yml` & `dls-utilpack-1.4.1/.github/workflows/linkcheck.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
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
 
-# dae_devops_fingerprint 7e1bfd21182cf87c73f3bdc1e1bf9044
+# dae_devops_fingerprint 4a0d076fe76b55b94ff172cc021cae4e
```

### Comparing `dls-utilpack-1.4.0/.gitignore` & `dls-utilpack-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/.gitlab-ci.yml` & `dls-utilpack-1.4.1/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -85,8 +85,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 8d2d1323dcc73040d4e9d57e50ec8fdc
+# dae_devops_fingerprint f43e642ab97b449962eae8963c80a5e4
```

### Comparing `dls-utilpack-1.4.0/.vscode/launch.json` & `dls-utilpack-1.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/LICENSE` & `dls-utilpack-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/Makefile` & `dls-utilpack-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/PKG-INFO` & `dls-utilpack-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.4.0
-Summary: Collection of various useful Python classes and functions.
+Version: 1.4.1
+Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,67 +208,20 @@
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/scisoft/dls-utilpack
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
-License-File: LICENSE.txt
 
 dls-utilpack
 =======================================================================
 
-Collection of various useful Python classes and functions
+Library of various useful Python classes and functions.
 
-Intended advantages:
-
-- reusable components
-- hide complexity of oft-used patterns
-- focused testing
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git 
-
-    dls-utilpack --version
-
-Summary
--------------------------------------------------
-
-callsign functions
-    Extract and compose object identification used in logging.
-
-datatype functions
-    Validate strings according to expected data types.
-    
-
-Documentation
------------------------------------------------------------------------
-
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-utilpack/index.html for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git 
-    cd dls-utilpack
-    virtualenv /scratch/$USER/venv/dls-utilpack
-    source /scratch/$USER/venv/dls-utilpack/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-utilpack/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-utilpack/build/html/index.html
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
+Reusable components which hide complexity of oft-used patterns and allow focused testing.
 
+For documentation see: https://diamondlightsource.github.io/dls-utilpack
```

### Comparing `dls-utilpack-1.4.0/docs/api/modules.rst` & `dls-utilpack-1.4.1/docs/reference/modules.rst`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,17 @@
 
 datatype functions
 -----------------------------------------------------------------------
 .. automodule:: dls_utilpack.datatypes
     :members:
 
 
+formatting functions
+-----------------------------------------------------------------------
+.. automodule:: dls_utilpack.describe
+    :members:
+
+
 version functions
 -----------------------------------------------------------------------
 .. automodule:: dls_utilpack.version
     :members:
```

### Comparing `dls-utilpack-1.4.0/docs/conf.py` & `dls-utilpack-1.4.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -193,8 +193,8 @@
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 82dcaf368fc09480cbf4ba8fbc9487b9
+# dae_devops_fingerprint 3cabbfa805a1ad4bc2a912809c6f65de
```

### Comparing `dls-utilpack-1.4.0/docs/images/dls-favicon.ico` & `dls-utilpack-1.4.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/docs/images/dls-logo.svg` & `dls-utilpack-1.4.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/pyproject.toml` & `dls-utilpack-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.2.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-utilpack
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
@@ -11,19 +11,19 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-description = "Collection of various useful Python classes and functions."
+description = "Library of various useful Python classes and functions."
 dependencies = ["dls-logformatter", "prettytable", "ruamel.yaml", "setproctitle"]
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
@@ -98,8 +98,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 4a6d99b68e007d2d4fe317fd9625ae8c
+# dae_devops_fingerprint 3f8324294fa7cfc47eb371d6ae8bdc9a
```

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/__main__.py` & `dls-utilpack-1.4.1/src/dls_utilpack/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/bash_composer.py` & `dls-utilpack-1.4.1/src/dls_utilpack/bash_composer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import stat
 from typing import List, Optional
 
 
 # ---------------------------------------------------------------------
 class Element:
+    """
+    Base class for other elements.
+    """
+
     def compose(self) -> List[str]:
         return []
 
 
 # ---------------------------------------------------------------------
 class Prolog(Element):
     def __init__(self):
@@ -79,16 +83,16 @@
 # ---------------------------------------------------------------------
 class LoadModules(Element):
     def __init__(self, directories: List[str], modules: List[str]):
         """
         Create object which composed to load linux environment modules in the bash script.
 
         Args:
-            directories (List[str]): List of directories for the "module use" command.
-            modules (List[str]): List of names for the "module load" command.
+            directories: List of directories for the "module use" command.
+            modules: List of names for the "module load" command.
 
         Returns:
             List[str]: Lines to be added to the bash script.
         """
         self.__directories = directories
         self.__modules = modules
 
@@ -119,61 +123,83 @@
         composer.add(Print("------ end of modules_load_bash_lines ------"))
 
         return composer.compose_lines()
 
 
 # ---------------------------------------------------------------------
 class BashComposer:
+    """
+    Class which helps with composing bash scripts consistently and reliably.
+    """
+
     def __init__(self, should_include_prolog: Optional[bool] = True):
+        """
+        Args:
+            should_include_prolog: True if should emit a prolog on this bash script. Defaults to True.
+        """
         self.__elements: List[Element] = []
         if should_include_prolog:
             self.add(Prolog())
 
     # -----------------------------------------------------------------
     def add(self, element: Element) -> None:
+        """
+        Add element to be included in the bash script.
+
+        Possible element classes are: Print, Raw, Command, Prolog and LoadModules.
+
+        Args:
+            element (Element): Element object.
+        """
         self.__elements.append(element)
 
     # -----------------------------------------------------------------
-    def add_print(self, message) -> None:
+    def add_print(self, message: str) -> None:
+        """
+        Add print element to bash script.
+
+        Args:
+            message (str): Message to be printed.
+        """
         self.add(Print(message))
 
     # -----------------------------------------------------------------
     def add_command(self, command: str, expected_rc: Optional[int] = 0) -> None:
         self.add(Command(command, expected_rc))
 
     # -----------------------------------------------------------------
     def add_load_modules(self, directories: List[str], modules: List[str]) -> None:
         """
         Add shell commands for loading linux environment modules.
 
         Args:
-            directories (List[str]): List of directories for the "module use" command.
-            modules (List[str]): List of names for the "module load" command.
+            directories: List of directories for the "module use" command.
+            modules: List of names for the "module load" command.
         """
         self.add(LoadModules(directories, modules))
 
     # -----------------------------------------------------------------
     def compose_lines(self) -> List[str]:
         """
-        Return bash script lines.
+        Return bash script as list of lines.
 
         Returns:
-            List[str]: The complete bash script.
+            The complete bash script.
         """
 
         lines = []
         for element in self.__elements:
             lines.extend(element.compose())
 
         return lines
 
     # -----------------------------------------------------------------
     def compose_string(self) -> str:
         """
-        Return composed bash script lines.
+        Return composed bash script as a string.
 
         Returns:
             str: The complete bash script.
         """
 
         lines = []
         for element in self.__elements:
```

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/callsign.py` & `dls-utilpack-1.4.1/src/dls_utilpack/callsign.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # ----------------------------------------------------------------------------------------
 def callsign(something: object, message: Optional[str] = None) -> str:
     """
     Return the callsign of the object.  If a message is given,
     then return a full message with the callsign prepended.
 
     Args:
-        something (object): object for which the callsign is desired
-        message (Optional[str]): message body if a full message is desired
+        something: object for which the callsign is desired
+        message: message body if a full message is desired
 
     Returns:
         str: callsign or callsign with message appended
 
     If the something object has a callsign method, then this is used.
     Otherwise, use the object's module and type name.
     """
@@ -55,20 +55,24 @@
     if message is None or message == "":
         return callsign
     else:
         return "%s says %s" % (callsign, message)
 
 
 # ----------------------------------------------------------------------------------------
-def callsign_html(something: object, message: Optional[str] = None) -> str:
+def callsign_html(the_object: object, message: Optional[str] = None) -> str:
     """
     Return the callsign of the object wrapped in an html div with css class T_callsign.
 
     See the callsign method for argument details.
 
     Any html thus composed will have the callsign identifiers embedded in it.
 
     The idea is that the css class normally be ``display: none;`` unless debugging.
+
+    Args:
+        the_object: the object whose callsign is wanted.
+        message : Extra bit of message text if desired. Defaults to None.
     """
 
-    text = html.escape(callsign(something, message))
+    text = html.escape(callsign(the_object, message))
     return f"<div class='T_callsign'>html generated by python class {text}</div>"
```

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/datatypes.py` & `dls-utilpack-1.4.1/src/dls_utilpack/datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/envvar.py` & `dls-utilpack-1.4.1/src/dls_utilpack/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/exceptions.py` & `dls-utilpack-1.4.1/src/dls_utilpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/explain.py` & `dls-utilpack-1.4.1/src/dls_utilpack/explain.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/hazzathread.py` & `dls-utilpack-1.4.1/src/dls_utilpack/hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/ignore.py` & `dls-utilpack-1.4.1/src/dls_utilpack/ignore.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/import_class.py` & `dls-utilpack-1.4.1/src/dls_utilpack/import_class.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/module.py` & `dls-utilpack-1.4.1/src/dls_utilpack/module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/profiler.py` & `dls-utilpack-1.4.1/src/dls_utilpack/profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/require.py` & `dls-utilpack-1.4.1/src/dls_utilpack/require.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/sanitize.py` & `dls-utilpack-1.4.1/src/dls_utilpack/sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/search_file.py` & `dls-utilpack-1.4.1/src/dls_utilpack/search_file.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/signal.py` & `dls-utilpack-1.4.1/src/dls_utilpack/signal.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/substitute.py` & `dls-utilpack-1.4.1/src/dls_utilpack/substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/thing.py` & `dls-utilpack-1.4.1/src/dls_utilpack/thing.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/things.py` & `dls-utilpack-1.4.1/src/dls_utilpack/things.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/version.py` & `dls-utilpack-1.4.1/src/dls_utilpack/version.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/visit.py` & `dls-utilpack-1.4.1/src/dls_utilpack/visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack/whatenv.py` & `dls-utilpack-1.4.1/src/dls_utilpack/whatenv.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/src/dls_utilpack.egg-info/PKG-INFO` & `dls-utilpack-1.4.1/src/dls_utilpack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.4.0
-Summary: Collection of various useful Python classes and functions.
+Version: 1.4.1
+Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -208,67 +208,20 @@
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/scisoft/dls-utilpack
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
-License-File: LICENSE.txt
 
 dls-utilpack
 =======================================================================
 
-Collection of various useful Python classes and functions
+Library of various useful Python classes and functions.
 
-Intended advantages:
-
-- reusable components
-- hide complexity of oft-used patterns
-- focused testing
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git 
-
-    dls-utilpack --version
-
-Summary
--------------------------------------------------
-
-callsign functions
-    Extract and compose object identification used in logging.
-
-datatype functions
-    Validate strings according to expected data types.
-    
-
-Documentation
------------------------------------------------------------------------
-
-See http://www.cs.diamond.ac.uk/reports/gitlab-ci/dls-utilpack/index.html for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/scisoft/dls-utilpack.git 
-    cd dls-utilpack
-    virtualenv /scratch/$USER/venv/dls-utilpack
-    source /scratch/$USER/venv/dls-utilpack/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-utilpack/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-utilpack/build/html/index.html
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
+Reusable components which hide complexity of oft-used patterns and allow focused testing.
 
+For documentation see: https://diamondlightsource.github.io/dls-utilpack
```

### Comparing `dls-utilpack-1.4.0/tests/base.py` & `dls-utilpack-1.4.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/base_tester.py` & `dls-utilpack-1.4.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/conftest.py` & `dls-utilpack-1.4.1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     yield None
 
 
 # --------------------------------------------------------------------------------
 @pytest.fixture(scope="function")
 def output_directory(request):
-    # TODO: Get a newline in conftest after pytest emits class name.
     print("")
 
     # Tmp directory which we can write into.
     output_directory = "/tmp/%s/%s/%s" % (
         "/".join(__file__.split("/")[-3:-1]),
         request.cls.__name__,
         request.function.__name__,
```

### Comparing `dls-utilpack-1.4.0/tests/test_bash_composer.py` & `dls-utilpack-1.4.1/tests/test_bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_callsign.py` & `dls-utilpack-1.4.1/tests/test_callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_datatypes.py` & `dls-utilpack-1.4.1/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_hazzathread.py` & `dls-utilpack-1.4.1/tests/test_hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_import.py` & `dls-utilpack-1.4.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_module.py` & `dls-utilpack-1.4.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_profiler.py` & `dls-utilpack-1.4.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_sanitize.py` & `dls-utilpack-1.4.1/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_sigint1.py` & `dls-utilpack-1.4.1/tests/test_sigint1.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_sigint2.py` & `dls-utilpack-1.4.1/tests/test_sigint2.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_substitute.py` & `dls-utilpack-1.4.1/tests/test_substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_visit.py` & `dls-utilpack-1.4.1/tests/test_visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.4.0/tests/test_whatenv.py` & `dls-utilpack-1.4.1/tests/test_whatenv.py`

 * *Files identical despite different names*


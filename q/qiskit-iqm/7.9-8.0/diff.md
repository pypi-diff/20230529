# Comparing `tmp/qiskit-iqm-7.9.tar.gz` & `tmp/qiskit-iqm-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-7.9.tar", last modified: Tue Apr  4 13:24:37 2023, max compression
+gzip compressed data, was "qiskit-iqm-8.0.tar", last modified: Mon May 29 07:59:47 2023, max compression
```

## Comparing `qiskit-iqm-7.9.tar` & `qiskit-iqm-8.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.223974 qiskit-iqm-7.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.227975 qiskit-iqm-7.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.223974 qiskit-iqm-7.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 13:24:37.000000 qiskit-iqm-7.9/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:24:37.231975 qiskit-iqm-7.9/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-04 13:23:30.000000 qiskit-iqm-7.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.429058 qiskit-iqm-8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_facade_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tox.ini
```

### Comparing `qiskit-iqm-7.9/.github/workflows/ci.yml` & `qiskit-iqm-8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/.github/workflows/publish.yml` & `qiskit-iqm-8.0/.github/workflows/publish.yml`

 * *Files 19% similar despite different names*

```diff
@@ -60,7 +60,33 @@
           tox -e docs
           touch build/sphinx/html/.nojekyll  # allow underscores in URL path
       - name: Publish to gh-pages
         uses: JamesIves/github-pages-deploy-action@4.1.4
         with:
           branch: gh-pages
           folder: build/sphinx/html
+
+  gen_licenses_info:
+    runs-on: ubuntu-latest
+
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+      - name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.9'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -e ".[dev]"
+          pip install pip-licenses
+      - name: Generate license information for dependencies
+        run: |
+          pip-licenses --format=confluence --with-urls > licenses.txt
+          cat -n licenses.txt | sort -uk2 | sort -n | cut -f2- > tmp && mv tmp licenses.txt  # remove duplicate lines
+      - name: Upload license information artifact
+        uses: actions/upload-artifact@v3
+        with:
+          name: dependencies-licenses
+          path: licenses.txt
```

### Comparing `qiskit-iqm-7.9/.github/workflows/tag_and_release.yml` & `qiskit-iqm-8.0/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/CHANGELOG.rst` & `qiskit-iqm-8.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,48 @@
 =========
 Changelog
 =========
 
+
+Version 8.0
+===========
+
+* Update the README `#58 <https://github.com/iqm-finland/qiskit-on-iqm/pull/58>`_ and `#60 <https://github.com/iqm-finland/qiskit-on-iqm/pull/60>`_
+* Clarify the example script `#62 <https://github.com/iqm-finland/qiskit-on-iqm/pull/62>`_
+
+Version 7.15
+============
+
+* Add info about custom calibration set to user guide `#59 <https://github.com/iqm-finland/qiskit-on-iqm/pull/59>`_
+
+Version 7.14
+============
+
+* Generate license information for dependencies on every release `#57 <https://github.com/iqm-finland/qiskit-on-iqm/pull/57>`_
+
+Version 7.13
+============
+
+* Upgrade to IQMClient version 12.2 `#56 <https://github.com/iqm-finland/qiskit-on-iqm/pull/56>`_
+
+Version 7.12
+============
+
+* Upgrade to IQMClient version 12.0 `#55 <https://github.com/iqm-finland/qiskit-on-iqm/pull/55>`_
+
+Version 7.11
+============
+
+* Bump Qiskit dependency to `~= 0.42.1` `#54 <https://github.com/iqm-finland/qiskit-on-iqm/pull/54>`_
+
+Version 7.10
+============
+
+* Add facade backend for Adonis by introducing ``facade_adonis`` backend type `#53 <https://github.com/iqm-finland/qiskit-on-iqm/pull/53>`_
+
 Version 7.9
 ===========
 
 * Add request into result metadata `#51 <https://github.com/iqm-finland/qiskit-on-iqm/pull/51>`_
 
 Version 7.8
 ===========
```

### Comparing `qiskit-iqm-7.9/CONTRIBUTING.rst` & `qiskit-iqm-8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/LICENSE` & `qiskit-iqm-8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/PKG-INFO` & `qiskit-iqm-8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 7.9
+Version: 8.0
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -229,21 +229,25 @@
 .. |Release badge| image:: https://img.shields.io/github/release/iqm-finland/qiskit-on-iqm.svg
 .. |Black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 Qiskit on IQM
 #############
 
-`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum architectures.
+`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum computers.
 
 
 What is it good for?
 ====================
 
-Currently Qiskit on IQM can run a compatible Qiskit quantum circuit on an IQM quantum computer.
+With Qiskit on IQM, you can for example:
+
+* Transpile arbitrary quantum circuits for IQM quantum architectures
+* Simulate execution with an IQM-specific noise model
+* Execute quantum circuits on an IQM quantum computer
 
 
 Installation
 ============
 
 The recommended way is to install the distribution package ``qiskit-iqm`` directly from the
 Python Package Index (PyPI):
@@ -264,8 +268,8 @@
 
 
 Copyright
 =========
 
 Qiskit on IQM is free software, released under the Apache License, version 2.0.
 
-Copyright 2022 Qiskit on IQM developers.
+Copyright 2022-2023 Qiskit on IQM developers.
```

### Comparing `qiskit-iqm-7.9/README.rst` & `qiskit-iqm-8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 .. |Release badge| image:: https://img.shields.io/github/release/iqm-finland/qiskit-on-iqm.svg
 .. |Black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 Qiskit on IQM
 #############
 
-`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum architectures.
+`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum computers.
 
 
 What is it good for?
 ====================
 
-Currently Qiskit on IQM can run a compatible Qiskit quantum circuit on an IQM quantum computer.
+With Qiskit on IQM, you can for example:
+
+* Transpile arbitrary quantum circuits for IQM quantum architectures
+* Simulate execution with an IQM-specific noise model
+* Execute quantum circuits on an IQM quantum computer
 
 
 Installation
 ============
 
 The recommended way is to install the distribution package ``qiskit-iqm`` directly from the
 Python Package Index (PyPI):
@@ -39,8 +43,8 @@
 
 
 Copyright
 =========
 
 Qiskit on IQM is free software, released under the Apache License, version 2.0.
 
-Copyright 2022 Qiskit on IQM developers.
+Copyright 2022-2023 Qiskit on IQM developers.
```

### Comparing `qiskit-iqm-7.9/docs/Makefile` & `qiskit-iqm-8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_static/images/favicon.ico` & `qiskit-iqm-8.0/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_static/images/logo.png` & `qiskit-iqm-8.0/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-8.0/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-8.0/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_templates/page.html` & `qiskit-iqm-8.0/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/_templates/versioning.html` & `qiskit-iqm-8.0/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/conf.py` & `qiskit-iqm-8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/index.rst` & `qiskit-iqm-8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/docs/user_guide.rst` & `qiskit-iqm-8.0/docs/user_guide.rst`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 Hello, world!
 -------------
 
 Here's the quickest and easiest way to execute a small computation on an IQM quantum computer and check that
 things are set up correctly:
 
-1. Download the `bell_measure.py example file <https://raw.githubusercontent.com/iqm-finland/qiskit-on-iqm/main/examples/bell_measure.py>`_ (Save Page As...)
+1. Download the `bell_measure.py example file <https://raw.githubusercontent.com/iqm-finland/qiskit-on-iqm/28b614461cfe952fe3ce63bee222e4b48037012c/examples/bell_measure.py>`_ (Save Page As...)
 2. Install Qiskit on IQM as instructed below (feel free to skip the import statement)
 3. Install Cortex CLI and log in as instructed in the `documentation <https://iqm-finland.github.io/cortex-cli/readme.html#installing-cortex-cli>`__
 4. Set the environment variable as instructed by Cortex CLI after logging in
-5. Run ``$ python bell_measure.py --server_url https://demo.qc.iqm.fi/cocos`` – replace the example URL with the correct one
+5. Run ``$ python bell_measure.py --cortex_server_url https://demo.qc.iqm.fi/cocos`` – replace the example URL with the correct one
 6. If you're connecting to a real quantum computer, the output should show almost half of the measurements resulting in '00' and almost half in '11' – if this is the case, things are set up correctly!
 
 
 Installation
 ------------
 
 The recommended way is to install the distribution package ``qiskit-iqm`` directly from the
@@ -93,14 +93,23 @@
 
     job = execute(qc, backend, shots=1000)
 
     print(job.result().get_counts())
 
 Note that the code snippet above assumes that you have set the variable ``iqm_server_url``.
 
+You can optionally set IQM backend specific settings as additional keyword arguments to the ``execute`` method (which
+passes the values down to :meth:`.IQMBackend.run`). For example, an IQM server uses the best available calibration set
+automatically; however, if you know an ID (UUID4) of a specific calibration set that you want to use, you can provide it
+as follows:
+
+.. code-block:: python
+
+    job = execute(circuit, backend, shots=1000, calibration_set_id="f7d9642e-b0ca-4f2d-af2a-30195bd7a76d")
+
 If the IQM server you are connecting to requires authentication, you will also have to use
 `Cortex CLI <https://github.com/iqm-finland/cortex-cli>`_ to retrieve and automatically refresh access tokens,
 then set the ``IQM_TOKENS_FILE`` environment variable to use those tokens.
 See Cortex CLI's `documentation <https://iqm-finland.github.io/cortex-cli/readme.html>`__ for details.
 Alternatively, authorize with the IQM_AUTH_SERVER, IQM_AUTH_USERNAME and IQM_AUTH_PASSWORD environment variables
 or pass them as arguments to the constructor of :class:`.IQMProvider`, however this approach is less secure
 and considered as deprecated.
@@ -188,16 +197,17 @@
            meas_2: ═══════════════════════════════════════════════════════════════════════════╩═
 
 
 Simulating the execution of a transpiled circuit locally
 --------------------------------------------------------
 
 The execution of circuits can be simulated locally, with a noise model to mimic the real hardware as much as possible.
-To this end, Qiskit on IQM provides the class  :class:`.IQMFakeBackend` that can be instantiated with properties of a certain QPU,
-or subclasses of it such as :class:`.IQMFakeAdonis` that represent certain quantum architectures with pre-populated properties and noise model.
+To this end, Qiskit on IQM provides the class  :class:`.IQMFakeBackend` that can be instantiated with properties of a
+certain QPU, or subclasses of it such as :class:`.IQMFakeAdonis` that represent certain quantum architectures with
+pre-populated properties and noise model.
 
 .. code-block:: python
 
     from qiskit import execute, QuantumCircuit
     from qiskit_iqm import IQMFakeAdonis
 
     circuit = QuantumCircuit(2)
@@ -206,24 +216,59 @@
     circuit.measure_all()
 
     backend = IQMFakeAdonis()
     job = execute(circuit, backend, shots=1000)
     job.result().get_counts()
 
 
-Above, we use an :class:`.IQMFakeAdonis` instance to run a noisy simulation of ``circuit`` on a simulated 5-qubit Adonis chip.
-If you want to customize the noise model instead of using the default one provided by :class:`.IQMFakeAdonis`, you can create
-a copy of the fake Adonis instance with updated error profile:
+Above, we use an :class:`.IQMFakeAdonis` instance to run a noisy simulation of ``circuit`` on a simulated 5-qubit Adonis
+chip. If you want to customize the noise model instead of using the default one provided by :class:`.IQMFakeAdonis`, you
+can create a copy of the fake Adonis instance with updated error profile:
 
 .. code-block:: python
 
     error_profile = backend.error_profile
     error_profile.t1s['QB2'] = 30000.0  # Change T1 time of QB2 as example
     custom_fake_backend = backend.copy_with_error_profile(error_profile)
 
+Running a quantum circuit on a facade backend
+---------------------------------------------
+
+Circuits can be executed against a mock environment: an IQM server that has no real quantum computer hardware.
+Results from such executions are random bits. This may be useful when developing and testing software integrations.
+
+Qiskit on IQM contains :class:`.IQMFacadeBackend`, which allows to combine the mock remote execution with a local
+noisy quantum circuit simulation. This way you can both validate your integration as well as get an idea of the expected circuit execution results.
+
+To run a circuit this way, use the `facade_adonis` backend retrieved from the provider. Note that the provider must be
+initialized with the URL of a quantum computer with the equivalent architecture (i.e. names of qubits, their
+connectivity, and the native gateset should match the 5-qubit Adonis architecture).
+
+.. code-block:: python
+
+    from qiskit import execute, QuantumCircuit
+    from qiskit_iqm import IQMProvider
+
+    circuit = QuantumCircuit(2)
+    circuit.h(0)
+    circuit.cx(0, 1)
+    circuit.measure_all()
+
+    provider = IQMProvider("https://demo.qc.iqm.fi/cocos/")
+    backend = provider.get_backend('facade_adonis')
+    job = execute(circuit, backend, shots=1000)
+    job.result().get_counts()
+
+.. note::
+
+   When a classical register is added to the circuit, Qiskit fills it with classical bits of value 0 by default. If the
+   register is not used later, and the circuit is submitted to the IQM server, the results will not contain those
+   0-filled bits. To make sure the facade backend returns results in the same format as a real IQM server,
+   :meth:`.IQMFacadeBackend.run` checks for the presence of unused classical registers, and fails with an error if there
+   are any.
 
 More advanced examples
 ----------------------
 
 In this section we demonstrate some less simple examples of using Qiskit on IQM and its interoperability with various
 tools available in Qiskit.
```

### Comparing `qiskit-iqm-7.9/examples/bell_measure.py` & `qiskit-iqm-8.0/examples/bell_measure.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 import argparse
 
 from qiskit import QuantumCircuit, execute
 
 from qiskit_iqm import IQMProvider
 
 argparser = argparse.ArgumentParser()
-argparser.add_argument('--server_url', help='URL of the IQM server', default='https://demo.qc.iqm.fi/cocos')
+argparser.add_argument(
+    '--cortex_server_url',
+    help='URL of the IQM Cortex server',
+    default='https://demo.qc.iqm.fi/cocos',
+)
 server_url = argparser.parse_args().server_url
 
 circuit = QuantumCircuit(2)
 circuit.h(0)
 circuit.cx(0, 1)
 circuit.measure_all()
```

### Comparing `qiskit-iqm-7.9/pyproject.toml` & `qiskit-iqm-8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,16 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.9, <3.11"
 dependencies = [
     "numpy",
-    "qiskit ~= 0.39.1",
-    "iqm-client >= 11.7, < 12.0"
-
+    "qiskit ~= 0.42.1",
+    "iqm-client >= 12.2, < 13.0"
 ]
 
 [project.urls]
 homepage = "https://github.com/iqm-finland/qiskit-on-iqm"
 documentation = "https://iqm-finland.github.io/qiskit-on-iqm"
 repository = "https://github.com/iqm-finland/qiskit-on-iqm.git"
 changelog = "https://github.com/iqm-finland/qiskit-on-iqm/blob/main/CHANGELOG.rst"
```

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/__init__.py` & `qiskit-iqm-8.0/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-8.0/src/qiskit_iqm/iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-8.0/src/qiskit_iqm/iqm_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from typing import Optional, Union
 import warnings
 
 from iqm_client import Circuit, Instruction, IQMClient
 from iqm_client.util import to_json_dict
 import numpy as np
 from qiskit import QuantumCircuit
-from qiskit.providers import Options
+from qiskit.providers import JobStatus, JobV1, Options
 
+from qiskit_iqm.fake_backends import IQMFakeAdonis
 from qiskit_iqm.iqm_backend import IQMBackendBase
 from qiskit_iqm.iqm_job import IQMJob
 from qiskit_iqm.qiskit_to_iqm import MeasurementKey
 
 
 class IQMBackend(IQMBackendBase):
     """Backend for executing quantum circuits on IQM quantum computers.
@@ -134,14 +135,61 @@
                 f'Metadata of circuit {circuit.name} was dropped because it could not be serialised to JSON.',
             )
             metadata = None
 
         return Circuit(name=circuit.name, instructions=instructions, metadata=metadata)
 
 
+class IQMFacadeBackend(IQMBackend):
+    """Facade backend for mimicking the execution of quantum circuits on IQM quantum computers. Allows to submit a
+     circuit to the IQM server, and if the execution was successful, performs a simulation with a respective IQM noise
+     model locally, then returns the simulated results.
+
+    Args:
+        client: client instance for communicating with an IQM server
+        **kwargs: optional arguments to be passed to the parent Backend initializer
+    """
+
+    def __init__(self, client: IQMClient, **kwargs):
+        self.fake_adonis = IQMFakeAdonis()
+        target_architecture = client.get_quantum_architecture()
+
+        if not self.fake_adonis.validate_compatible_architecture(target_architecture):
+            raise ValueError('Quantum architecture of the remote quantum computer does not match Adonis.')
+
+        super().__init__(client, **kwargs)
+        self.client = client
+
+    def _validate_no_empty_cregs(self, circuit):
+        """Returns True if given circuit has no empty (unused) classical registers, False otherwise."""
+        cregs_utilization = dict.fromkeys(circuit.cregs, 0)
+        used_cregs = [circuit.find_bit(i.clbits[0]).registers[0][0] for i in circuit.data if len(i.clbits) > 0]
+        for creg in used_cregs:
+            cregs_utilization[creg] += 1
+
+        if 0 in cregs_utilization.values():
+            return False
+        return True
+
+    def run(self, run_input: Union[QuantumCircuit, list[QuantumCircuit]], **options) -> JobV1:
+        circuits = [run_input] if isinstance(run_input, QuantumCircuit) else run_input
+        circuits_validated_cregs: list[bool] = [self._validate_no_empty_cregs(circuit) for circuit in circuits]
+        if not all(circuits_validated_cregs):
+            raise ValueError(
+                'One or more circuits contain unused classical registers. This is not allowed for Facade simulation, '
+                'see user guide.'
+            )
+
+        iqm_backend_job = super().run(run_input, **options)
+        iqm_backend_job.result()  # get and discard results
+        if iqm_backend_job.status() == JobStatus.ERROR:
+            raise RuntimeError('Remote execution did not succeed.')
+        return self.fake_adonis.run(run_input, **options)
+
+
 class IQMProvider:
     """Provider for IQM backends.
 
     Args:
         url: URL of the IQM Cortex server
 
     Keyword Args:
@@ -153,11 +201,17 @@
             Can also be set in the ``IQM_AUTH_PASSWORD`` environment variable.
     """
 
     def __init__(self, url: str, **user_auth_args):  # contains keyword args auth_server_url, username, password
         self.url = url
         self.user_auth_args = user_auth_args
 
-    def get_backend(self) -> IQMBackend:
-        """An IQMBackend instance associated with this provider."""
+    def get_backend(self, name=None) -> Union[IQMBackend, IQMFacadeBackend]:
+        """An IQMBackend instance associated with this provider.
+
+        Args:
+            name: optional name of a custom facade backend
+        """
         client = IQMClient(self.url, client_signature=f'qiskit-iqm {version("qiskit-iqm")}', **self.user_auth_args)
+        if name == 'facade_adonis':
+            return IQMFacadeBackend(client)
         return IQMBackend(client)
```

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-8.0/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-8.0/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 7.9
+Version: 8.0
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -229,21 +229,25 @@
 .. |Release badge| image:: https://img.shields.io/github/release/iqm-finland/qiskit-on-iqm.svg
 .. |Black badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
 Qiskit on IQM
 #############
 
-`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum architectures.
+`Qiskit <https://qiskit.org/>`_ adapter for `IQM's <https://www.meetiqm.com>`_ quantum computers.
 
 
 What is it good for?
 ====================
 
-Currently Qiskit on IQM can run a compatible Qiskit quantum circuit on an IQM quantum computer.
+With Qiskit on IQM, you can for example:
+
+* Transpile arbitrary quantum circuits for IQM quantum architectures
+* Simulate execution with an IQM-specific noise model
+* Execute quantum circuits on an IQM quantum computer
 
 
 Installation
 ============
 
 The recommended way is to install the distribution package ``qiskit-iqm`` directly from the
 Python Package Index (PyPI):
@@ -264,8 +268,8 @@
 
 
 Copyright
 =========
 
 Qiskit on IQM is free software, released under the Apache License, version 2.0.
 
-Copyright 2022 Qiskit on IQM developers.
+Copyright 2022-2023 Qiskit on IQM developers.
```

### Comparing `qiskit-iqm-7.9/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-8.0/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 src/qiskit_iqm/fake_backends/__init__.py
 src/qiskit_iqm/fake_backends/fake_adonis.py
 src/qiskit_iqm/fake_backends/iqm_fake_backend.py
 tests/.pylintrc
 tests/__init__.py
 tests/conftest.py
 tests/test_iqm_backend.py
+tests/test_iqm_facade_backend.py
 tests/test_iqm_job.py
 tests/test_iqm_provider.py
 tests/test_qiskit_to_iqm.py
 tests/fake_backends/__init__.py
 tests/fake_backends/conftest.py
 tests/fake_backends/test_fake_adonis.py
 tests/fake_backends/test_iqm_fake_backend.py
```

### Comparing `qiskit-iqm-7.9/tag-from-pipeline.sh` & `qiskit-iqm-8.0/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tests/conftest.py` & `qiskit-iqm-8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tests/fake_backends/conftest.py` & `qiskit-iqm-8.0/tests/fake_backends/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-8.0/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-8.0/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tests/test_iqm_backend.py` & `qiskit-iqm-8.0/tests/test_iqm_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,7 +67,16 @@
     cmap = backend.coupling_map.get_edges()
     for instruction, qubits, _ in circuit_transpiled.data:
         assert instruction.name in ('r', 'cz')
         if instruction.name == 'cz':
             idx1 = circuit_transpiled.find_bit(qubits[0]).index
             idx2 = circuit_transpiled.find_bit(qubits[1]).index
             assert ((idx1, idx2) in cmap) or ((idx2, idx1) in cmap)
+
+
+def test_validate_compatible_architecture(
+    adonis_architecture, adonis_architecture_shuffled_names, linear_architecture_3q
+):
+    backend = TestIQMBackend(adonis_architecture)
+    assert backend.validate_compatible_architecture(adonis_architecture) is True
+    assert backend.validate_compatible_architecture(adonis_architecture_shuffled_names) is True
+    assert backend.validate_compatible_architecture(linear_architecture_3q) is False
```

### Comparing `qiskit-iqm-7.9/tests/test_iqm_job.py` & `qiskit-iqm-8.0/tests/test_iqm_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Testing IQMJob.
 """
 import uuid
 
-from iqm_client import IQMClient, RunResult, RunStatus, SingleQubitMapping, Status
+from iqm_client import Instruction, IQMClient, RunResult, RunStatus, SingleQubitMapping, Status
 import mockito
 from mockito import mock, when
 import pytest
 from qiskit import QuantumCircuit
 from qiskit.providers import JobStatus
 from qiskit.result import Counts
 from qiskit.result import Result as QiskitResult
@@ -44,19 +44,20 @@
 @pytest.fixture()
 def iqm_result_two_registers():
     return {'c_2_0_0': [[1], [0], [1], [0]], 'c_2_0_1': [[1], [1], [0], [1]], 'd_4_1_2': [[1], [1], [1], [1]]}
 
 
 @pytest.fixture()
 def iqm_metadata():
+    measurement = Instruction(name='measurement', implementation=None, qubits=('0',), args={'key': 'm1'})
     return {
         'calibration_set_id': 'df124054-f6d8-41f9-b880-8487f90018f9',
         'request': {
             'shots': 4,
-            'circuits': [{'name': 'circuit_1', 'instructions': [], 'metadata': {'a': 'b'}}],
+            'circuits': [{'name': 'circuit_1', 'instructions': (measurement,), 'metadata': {'a': 'b'}}],
             'calibration_set_id': 'df124054-f6d8-41f9-b880-8487f90018f9',
             'qubit_mapping': [
                 SingleQubitMapping(logical_name='0', physical_name='QB1'),
                 SingleQubitMapping(logical_name='1', physical_name='QB2'),
             ],
         },
     }
@@ -83,16 +84,17 @@
 def test_status_done(job, iqm_metadata):
     client_result = RunResult(status=Status.READY, measurements=None, metadata=iqm_metadata)
     when(job._client).get_run_status(uuid.UUID(job.job_id())).thenReturn(client_result)
     assert job.status() == JobStatus.DONE
     assert job._result is None
 
 
-def test_status_running(job):
-    when(job._client).get_run_status(uuid.UUID(job.job_id())).thenReturn(RunStatus(status=Status.PENDING))
+@pytest.mark.parametrize('run_status', [Status.PENDING_COMPILATION, Status.PENDING_EXECUTION])
+def test_status_running(job, run_status):
+    when(job._client).get_run_status(uuid.UUID(job.job_id())).thenReturn(RunStatus(status=run_status))
     assert job.status() == JobStatus.RUNNING
 
 
 def test_status_fail(job):
     when(job._client).get_run_status(uuid.UUID(job.job_id())).thenReturn(RunStatus(status=Status.FAILED))
     assert job.status() == JobStatus.ERROR
 
@@ -120,21 +122,22 @@
     result = job.result()
     assert isinstance(result, QiskitResult)
     assert job.status() == JobStatus.DONE
     mockito.verify(job._client, times=1).wait_for_results(uuid.UUID(job.job_id()))
 
 
 def test_result_multiple_circuits(job, iqm_result_two_registers):
+    instruction_meta = [{'name': 'measurement', 'qubits': ['0'], 'args': {'key': 'm1'}}]
     iqm_metadata_multiple_circuits = {
         'calibration_set_id': '9d75904b-0c93-461f-b1dc-bd200cfad1f1',
         'request': {
             'shots': 4,
             'circuits': [
-                {'name': 'circuit_1', 'instructions': [], 'metadata': {'a': 0}},
-                {'name': 'circuit_2', 'instructions': [], 'metadata': {'a': 1}},
+                {'name': 'circuit_1', 'instructions': instruction_meta, 'metadata': {'a': 0}},
+                {'name': 'circuit_2', 'instructions': instruction_meta, 'metadata': {'a': 1}},
             ],
             'calibration_set_id': '9d75904b-0c93-461f-b1dc-bd200cfad1f1',
             'qubit_mapping': [
                 SingleQubitMapping(logical_name='0', physical_name='QB1'),
                 SingleQubitMapping(logical_name='1', physical_name='QB2'),
                 SingleQubitMapping(logical_name='2', physical_name='QB3'),
             ],
```

### Comparing `qiskit-iqm-7.9/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-8.0/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-7.9/tox.ini` & `qiskit-iqm-8.0/tox.ini`

 * *Files identical despite different names*


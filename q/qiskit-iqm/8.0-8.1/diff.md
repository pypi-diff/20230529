# Comparing `tmp/qiskit-iqm-8.0.tar.gz` & `tmp/qiskit-iqm-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-iqm-8.0.tar", last modified: Mon May 29 07:59:47 2023, max compression
+gzip compressed data, was "qiskit-iqm-8.1.tar", last modified: Mon May 29 08:27:56 2023, max compression
```

## Comparing `qiskit-iqm-8.0.tar` & `qiskit-iqm-8.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.429058 qiskit-iqm-8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/API.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/examples/bell_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:59:47.441059 qiskit-iqm-8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.433058 qiskit-iqm-8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/src/qiskit_iqm/qiskit_to_iqm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 07:59:47.000000 qiskit-iqm-8.0/src/qiskit_iqm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:59:47.437058 qiskit-iqm-8.0/tests/fake_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/test_fake_adonis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/fake_backends/test_iqm_fake_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_facade_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_iqm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tests/test_qiskit_to_iqm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-29 07:58:47.000000 qiskit-iqm-8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.722275 qiskit-iqm-8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/API.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   194362 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16696 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.726276 qiskit-iqm-8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/examples/bell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.722275 qiskit-iqm-8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/src/qiskit_iqm/qiskit_to_iqm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.730276 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 08:27:56.000000 qiskit-iqm-8.1/src/qiskit_iqm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:56.734276 qiskit-iqm-8.1/tests/fake_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/test_fake_adonis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/fake_backends/test_iqm_fake_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_facade_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_iqm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tests/test_qiskit_to_iqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-29 08:26:47.000000 qiskit-iqm-8.1/tox.ini
```

### Comparing `qiskit-iqm-8.0/.github/workflows/ci.yml` & `qiskit-iqm-8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/.github/workflows/publish.yml` & `qiskit-iqm-8.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/.github/workflows/tag_and_release.yml` & `qiskit-iqm-8.1/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/CHANGELOG.rst` & `qiskit-iqm-8.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 8.1
+===========
+
+* Upgrade to IQMClient version 12.4 `#61 <https://github.com/iqm-finland/qiskit-on-iqm/pull/61>`_
+* Add parameter ``circuit_duration_check`` allowing to control server-side maximum circuit duration check `#61 <https://github.com/iqm-finland/qiskit-on-iqm/pull/61>`_
 
 Version 8.0
 ===========
 
 * Update the README `#58 <https://github.com/iqm-finland/qiskit-on-iqm/pull/58>`_ and `#60 <https://github.com/iqm-finland/qiskit-on-iqm/pull/60>`_
 * Clarify the example script `#62 <https://github.com/iqm-finland/qiskit-on-iqm/pull/62>`_
```

### Comparing `qiskit-iqm-8.0/CONTRIBUTING.rst` & `qiskit-iqm-8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/LICENSE` & `qiskit-iqm-8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/PKG-INFO` & `qiskit-iqm-8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.0
+Version: 8.1
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.0/README.rst` & `qiskit-iqm-8.1/README.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/Makefile` & `qiskit-iqm-8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_static/images/favicon.ico` & `qiskit-iqm-8.1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_static/images/logo.png` & `qiskit-iqm-8.1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_templates/autosummary-class-template.rst` & `qiskit-iqm-8.1/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_templates/autosummary-module-template.rst` & `qiskit-iqm-8.1/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_templates/page.html` & `qiskit-iqm-8.1/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/_templates/versioning.html` & `qiskit-iqm-8.1/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/conf.py` & `qiskit-iqm-8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/index.rst` & `qiskit-iqm-8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/docs/user_guide.rst` & `qiskit-iqm-8.1/docs/user_guide.rst`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,25 @@
 automatically; however, if you know an ID (UUID4) of a specific calibration set that you want to use, you can provide it
 as follows:
 
 .. code-block:: python
 
     job = execute(circuit, backend, shots=1000, calibration_set_id="f7d9642e-b0ca-4f2d-af2a-30195bd7a76d")
 
+Another example is disabling the server-side circuit duration check. If any circuit in a job would take too long to
+execute compared to the coherence time of the QPU, the server will disqualify the job and not execute any circuits.
+In some special cases, you may want to disable this as follows:
+
+.. code-block:: python
+
+    job = execute(circuit, backend, shots=1000, circuit_duration_check=False)
+
+Disabling the circuit duration check may be limited to certain users or groups, depending on the server settings.
+In normal use, the circuit duration check should always remain enabled.
+
 If the IQM server you are connecting to requires authentication, you will also have to use
 `Cortex CLI <https://github.com/iqm-finland/cortex-cli>`_ to retrieve and automatically refresh access tokens,
 then set the ``IQM_TOKENS_FILE`` environment variable to use those tokens.
 See Cortex CLI's `documentation <https://iqm-finland.github.io/cortex-cli/readme.html>`__ for details.
 Alternatively, authorize with the IQM_AUTH_SERVER, IQM_AUTH_USERNAME and IQM_AUTH_PASSWORD environment variables
 or pass them as arguments to the constructor of :class:`.IQMProvider`, however this approach is less secure
 and considered as deprecated.
```

### Comparing `qiskit-iqm-8.0/examples/bell_measure.py` & `qiskit-iqm-8.1/examples/bell_measure.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/pyproject.toml` & `qiskit-iqm-8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License"
 ]
 requires-python = ">=3.9, <3.11"
 dependencies = [
     "numpy",
     "qiskit ~= 0.42.1",
-    "iqm-client >= 12.2, < 13.0"
+    "iqm-client >= 12.4, < 13.0"
 ]
 
 [project.urls]
 homepage = "https://github.com/iqm-finland/qiskit-on-iqm"
 documentation = "https://iqm-finland.github.io/qiskit-on-iqm"
 repository = "https://github.com/iqm-finland/qiskit-on-iqm.git"
 changelog = "https://github.com/iqm-finland/qiskit-on-iqm/blob/main/CHANGELOG.rst"
```

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/__init__.py` & `qiskit-iqm-8.1/src/qiskit_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/__init__.py` & `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/fake_adonis.py` & `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/fake_backends/iqm_fake_backend.py` & `qiskit-iqm-8.1/src/qiskit_iqm/fake_backends/iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/iqm_backend.py` & `qiskit-iqm-8.1/src/qiskit_iqm/iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/iqm_job.py` & `qiskit-iqm-8.1/src/qiskit_iqm/iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/iqm_provider.py` & `qiskit-iqm-8.1/src/qiskit_iqm/iqm_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     def __init__(self, client: IQMClient, **kwargs):
         super().__init__(client.get_quantum_architecture(), **kwargs)
         self.client = client
 
     @classmethod
     def _default_options(cls) -> Options:
-        return Options(shots=1024, calibration_set_id=None)
+        return Options(shots=1024, calibration_set_id=None, circuit_duration_check=True)
 
     @property
     def max_circuits(self) -> Optional[int]:
         return None
 
     def run(self, run_input: Union[QuantumCircuit, list[QuantumCircuit]], **options) -> IQMJob:
         if self.client is None:
@@ -57,22 +57,27 @@
         circuits = [run_input] if isinstance(run_input, QuantumCircuit) else run_input
 
         if len(circuits) == 0:
             raise ValueError('Empty list of circuits submitted for execution.')
 
         shots = options.get('shots', self.options.shots)
         calibration_set_id = options.get('calibration_set_id', self.options.calibration_set_id)
+        circuit_duration_check = options.get('circuit_duration_check', self.options.circuit_duration_check)
 
         circuits_serialized: list[Circuit] = [self.serialize_circuit(circuit) for circuit in circuits]
         used_indices: set[int] = reduce(
             lambda qubits, circuit: qubits.union(set(int(q) for q in circuit.all_qubits())), circuits_serialized, set()
         )
         qubit_mapping = {str(idx): qb for idx, qb in self._idx_to_qb.items() if idx in used_indices}
         uuid = self.client.submit_circuits(
-            circuits_serialized, qubit_mapping=qubit_mapping, calibration_set_id=calibration_set_id, shots=shots
+            circuits_serialized,
+            qubit_mapping=qubit_mapping,
+            calibration_set_id=calibration_set_id,
+            shots=shots,
+            circuit_duration_check=circuit_duration_check,
         )
         job = IQMJob(self, str(uuid), shots=shots)
         job.circuit_metadata = [c.metadata for c in circuits]
         return job
 
     def retrieve_job(self, job_id: str) -> IQMJob:
         """Create and return an IQMJob instance associated with this backend with given job id."""
```

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm/qiskit_to_iqm.py` & `qiskit-iqm-8.1/src/qiskit_iqm/qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm.egg-info/PKG-INFO` & `qiskit-iqm-8.1/src/qiskit_iqm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-iqm
-Version: 8.0
+Version: 8.1
 Summary: Qiskit adapter for IQM's quantum architectures
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qiskit-iqm-8.0/src/qiskit_iqm.egg-info/SOURCES.txt` & `qiskit-iqm-8.1/src/qiskit_iqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tag-from-pipeline.sh` & `qiskit-iqm-8.1/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/conftest.py` & `qiskit-iqm-8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/fake_backends/conftest.py` & `qiskit-iqm-8.1/tests/fake_backends/conftest.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/fake_backends/test_fake_adonis.py` & `qiskit-iqm-8.1/tests/fake_backends/test_fake_adonis.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/fake_backends/test_iqm_fake_backend.py` & `qiskit-iqm-8.1/tests/fake_backends/test_iqm_fake_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/test_iqm_backend.py` & `qiskit-iqm-8.1/tests/test_iqm_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/test_iqm_facade_backend.py` & `qiskit-iqm-8.1/tests/test_iqm_facade_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/test_iqm_job.py` & `qiskit-iqm-8.1/tests/test_iqm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tests/test_iqm_provider.py` & `qiskit-iqm-8.1/tests/test_iqm_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
 def test_run_single_circuit(backend, circuit):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
     some_id = uuid.uuid4()
     shots = 10
     when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots
+        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots, circuit_duration_check=True
     ).thenReturn(some_id)
     job = backend.run(circuit, shots=shots)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
 
     # Should also work if the circuit is passed inside a list
     job = backend.run([circuit], shots=shots)
@@ -261,32 +261,52 @@
 def test_run_with_custom_calibration_set_id(backend, circuit):
     circuit.measure(0, 0)
     circuit_ser = backend.serialize_circuit(circuit)
     some_id = uuid.uuid4()
     shots = 10
     calibration_set_id = '67e77465-d90e-4839-986e-9270f952b743'
     when(backend.client).submit_circuits(
-        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=calibration_set_id, shots=shots
+        [circuit_ser],
+        qubit_mapping={'0': 'QB1'},
+        calibration_set_id=calibration_set_id,
+        shots=shots,
+        circuit_duration_check=True,
     ).thenReturn(some_id)
 
     backend.run([circuit], calibration_set_id=calibration_set_id, shots=shots)
 
 
+def test_run_with_duration_check_disabled(backend, circuit):
+    circuit.measure(0, 0)
+    circuit_ser = backend.serialize_circuit(circuit)
+    some_id = uuid.uuid4()
+    shots = 10
+    when(backend.client).submit_circuits(
+        [circuit_ser], qubit_mapping={'0': 'QB1'}, calibration_set_id=None, shots=shots, circuit_duration_check=False
+    ).thenReturn(some_id)
+
+    backend.run([circuit], shots=shots, circuit_duration_check=False)
+
+
 def test_run_batch_of_circuits(backend, circuit):
     theta = Parameter('theta')
     theta_range = np.linspace(0, 2 * np.pi, 3)
     shots = 10
     some_id = uuid.uuid4()
     circuit.cz(0, 1)
     circuit.r(theta, 0, 0)
     circuit.cz(0, 1)
     circuits = [circuit.bind_parameters({theta: t}) for t in theta_range]
     circuits_serialized = [backend.serialize_circuit(circuit) for circuit in circuits]
     when(backend.client).submit_circuits(
-        circuits_serialized, qubit_mapping={'0': 'QB1', '1': 'QB2'}, calibration_set_id=None, shots=shots
+        circuits_serialized,
+        qubit_mapping={'0': 'QB1', '1': 'QB2'},
+        calibration_set_id=None,
+        shots=shots,
+        circuit_duration_check=True,
     ).thenReturn(some_id)
 
     job = backend.run(circuits, shots=shots)
     assert isinstance(job, IQMJob)
     assert job.job_id() == str(some_id)
 
 
@@ -362,15 +382,17 @@
                 ],
             }
         },
     }
     result_status = {'status': 'failed'}
 
     when(IQMClient).get_quantum_architecture().thenReturn(adonis_architecture)
-    when(IQMClient).submit_circuits(ANY, qubit_mapping=ANY, calibration_set_id=ANY, shots=ANY).thenReturn(uuid.uuid4())
+    when(IQMClient).submit_circuits(
+        ANY, qubit_mapping=ANY, calibration_set_id=ANY, shots=ANY, circuit_duration_check=ANY
+    ).thenReturn(uuid.uuid4())
     when(IQMClient).get_run(ANY).thenReturn(RunResult.from_dict(result))
     when(IQMClient).get_run_status(ANY).thenReturn(RunStatus.from_dict(result_status))
 
     provider = IQMProvider(url)
     backend = provider.get_backend('facade_adonis')
 
     with pytest.raises(RuntimeError):
```

### Comparing `qiskit-iqm-8.0/tests/test_qiskit_to_iqm.py` & `qiskit-iqm-8.1/tests/test_qiskit_to_iqm.py`

 * *Files identical despite different names*

### Comparing `qiskit-iqm-8.0/tox.ini` & `qiskit-iqm-8.1/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/django-clone-5.3.1.tar.gz` & `tmp/django-clone-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/django-clone/django-clone/dist/.tmp-8vou2zqs/django-clone-5.3.1.tar", last modified: Wed Mar 22 18:26:38 2023, max compression
+gzip compressed data, was "/home/runner/work/django-clone/django-clone/dist/.tmp-5v93ez8j/django-clone-5.3.2.tar", last modified: Mon May 29 04:14:09 2023, max compression
```

## Comparing `django-clone-5.3.1.tar` & `django-clone-5.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)   106173 2023-03-22 18:26:09.000000 django-clone-5.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-03-22 18:26:09.000000 django-clone-5.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-22 18:26:09.000000 django-clone-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-22 18:26:09.000000 django-clone-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-03-22 18:26:38.000000 django-clone-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-03-22 18:26:09.000000 django-clone-5.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 18:26:38.000000 django-clone-5.3.1/django_clone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/model_clone/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-22 18:26:24.000000 django-clone-5.3.1/model_clone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28928 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/model_clone/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/model_clone/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/templates/admin/change_form_object_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:26:38.000000 django-clone-5.3.1/model_clone/templates/clone/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/templates/clone/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-03-22 18:26:09.000000 django-clone-5.3.1/model_clone/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-22 18:26:09.000000 django-clone-5.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-22 18:26:38.000000 django-clone-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-22 18:26:24.000000 django-clone-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)   108930 2023-05-29 04:13:41.000000 django-clone-5.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-05-29 04:13:41.000000 django-clone-5.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 04:13:41.000000 django-clone-5.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 04:13:41.000000 django-clone-5.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-05-29 04:14:09.000000 django-clone-5.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-29 04:13:41.000000 django-clone-5.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 04:14:09.000000 django-clone-5.3.2/django_clone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 04:13:57.000000 django-clone-5.3.2/model_clone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28928 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/templates/admin/change_form_object_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:14:09.000000 django-clone-5.3.2/model_clone/templates/clone/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/templates/clone/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-05-29 04:13:41.000000 django-clone-5.3.2/model_clone/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-29 04:13:41.000000 django-clone-5.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-29 04:14:09.000000 django-clone-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-29 04:13:57.000000 django-clone-5.3.2/setup.py
```

### Comparing `django-clone-5.3.1/CHANGELOG.md` & `django-clone-5.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,47 @@
 # Changelog
 
+## [v5.3.1](https://github.com/tj-django/django-clone/tree/v5.3.1) (2023-03-18)
+
+[Full Changelog](https://github.com/tj-django/django-clone/compare/v5.3.0...v5.3.1)
+
+**Closed issues:**
+
+- Dependency Dashboard [\#198](https://github.com/tj-django/django-clone/issues/198)
+
+**Merged pull requests:**
+
+- chore\(deps\): update tj-actions/verify-changed-files action to v14 [\#772](https://github.com/tj-django/django-clone/pull/772) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update actions/checkout action to v3.4.0 [\#771](https://github.com/tj-django/django-clone/pull/771) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update peter-evans/create-pull-request action to v4.2.4 [\#770](https://github.com/tj-django/django-clone/pull/770) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate [\#769](https://github.com/tj-django/django-clone/pull/769) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- chore\(deps\): update tj-actions/github-changelog-generator action to v1.18 [\#768](https://github.com/tj-django/django-clone/pull/768) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update codacy/codacy-analysis-cli-action action to v4.3.0 [\#767](https://github.com/tj-django/django-clone/pull/767) ([renovate[bot]](https://github.com/apps/renovate))
+- Updated docs [\#766](https://github.com/tj-django/django-clone/pull/766) ([github-actions[bot]](https://github.com/apps/github-actions))
+- Updated README.md [\#765](https://github.com/tj-django/django-clone/pull/765) ([jackton1](https://github.com/jackton1))
+- Updated README.md [\#764](https://github.com/tj-django/django-clone/pull/764) ([jackton1](https://github.com/jackton1))
+- chore\(deps\): update pascalgn/automerge-action action to v0.15.6 [\#763](https://github.com/tj-django/django-clone/pull/763) ([renovate[bot]](https://github.com/apps/renovate))
+- chore\(deps\): update dependency django to v4.1.7 [\#762](https://github.com/tj-django/django-clone/pull/762) ([renovate[bot]](https://github.com/apps/renovate))
+- \[pre-commit.ci\] pre-commit autoupdate [\#761](https://github.com/tj-django/django-clone/pull/761) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- chore\(deps\): update dependency django to v4.1.6 [\#760](https://github.com/tj-django/django-clone/pull/760) ([renovate[bot]](https://github.com/apps/renovate))
+- Updated docs [\#759](https://github.com/tj-django/django-clone/pull/759) ([github-actions[bot]](https://github.com/apps/github-actions))
+- Upgraded v5.2.0 → v5.3.0 [\#758](https://github.com/tj-django/django-clone/pull/758) ([jackton1](https://github.com/jackton1))
+- Updated docs [\#757](https://github.com/tj-django/django-clone/pull/757) ([github-actions[bot]](https://github.com/apps/github-actions))
+
 ## [v5.3.0](https://github.com/tj-django/django-clone/tree/v5.3.0) (2023-01-30)
 
 [Full Changelog](https://github.com/tj-django/django-clone/compare/v5.2.0...v5.3.0)
 
 **Implemented enhancements:**
 
 - \[Feature\] Create m2m relations with existing objects new.m2mfield.set\(old.m2mfield.all\(\)\) [\#703](https://github.com/tj-django/django-clone/issues/703)
 
 **Closed issues:**
 
 - CVE-2022-40899 \(Medium\) detected in future-0.18.2.tar.gz - autoclosed [\#726](https://github.com/tj-django/django-clone/issues/726)
-- Dependency Dashboard [\#198](https://github.com/tj-django/django-clone/issues/198)
 
 **Merged pull requests:**
 
 - Updated README.md [\#756](https://github.com/tj-django/django-clone/pull/756) ([jackton1](https://github.com/jackton1))
 - Updated docs [\#755](https://github.com/tj-django/django-clone/pull/755) ([github-actions[bot]](https://github.com/apps/github-actions))
 - docs: add DanielSchaffer as a contributor for code, and test [\#754](https://github.com/tj-django/django-clone/pull/754) ([allcontributors[bot]](https://github.com/apps/allcontributors))
 - fix: error running pre-commit [\#753](https://github.com/tj-django/django-clone/pull/753) ([jackton1](https://github.com/jackton1))
```

### Comparing `django-clone-5.3.1/CODE_OF_CONDUCT.md` & `django-clone-5.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/LICENSE` & `django-clone-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/MANIFEST.in` & `django-clone-5.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/PKG-INFO` & `django-clone-5.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clone
-Version: 5.3.1
+Version: 5.3.2
 Summary: Create a clone of a django model instance.
 Home-page: https://github.com/tj-django/django-clone.git
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 Maintainer: Tonye Jack
 Maintainer-email: jtonye@ymail.com
 License: MIT/Apache-2.0
@@ -41,15 +41,15 @@
 
 <p align="center"> 
     <img width="466" alt="4FC889E9-FF59-4E44-9EB6-2AF7DC034C74" src="https://user-images.githubusercontent.com/17484350/215616634-17439a58-7bd8-4e9c-989f-e6bef7c73e48.png">
 </p>
 
 |  Python   | Django  |  Downloads  |   Code Style   |
 |:---------:|:-------:|:-----------:|:--------------:|
-| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/3.2/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/dev/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 |    PyPI         | Test | Vulnerabilities | Coverage | Code Quality  |  Pre-Commit   |
 |:---------------:|:----:|:---------------:|:--------:|:-------------:|:-------------:|
 | [![PyPI version](https://badge.fury.io/py/django-clone.svg)](https://badge.fury.io/py/django-clone) | [![Test](https://github.com/tj-django/django-clone/workflows/Test/badge.svg)](https://github.com/tj-django/django-clone/actions?query=workflow%3ATest) | [![Known Vulnerabilities](https://snyk.io/test/github/tj-django/django-clone/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/tj-django/django-clone?targetFile=requirements.txt) | [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Coverage) <br/> [![codecov](https://codecov.io/gh/tj-django/django-clone/branch/main/graph/badge.svg?token=2NE21Oe50Q)](https://codecov.io/gh/tj-django/django-clone)| [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Grade) |  [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tj-django/django-clone/main.svg)](https://results.pre-commit.ci/latest/github/tj-django/django-clone/main) |
 
 ## django-clone
 
@@ -65,14 +65,16 @@
 *   Restrict fields used for creating a duplicate instance.
 *   Detects unique fields and naively adds a suffix `copy {count}` to each duplicate instance (for supported fields only).
 *   Optionally differentiate between a duplicate instance and the original by appending a **copy** suffix to non unique fields (for supported fields only).
 
 ## Table of Contents
 
 *   [Installation](#installation)
+    *   [pip](#pip)
+    *   [poetry](#poetry)
 *   [Usage](#usage)
     *   [Subclassing the `CloneModel`](#subclassing-the-clonemodel)
     *   [Using the `CloneMixin`](#using-the-clonemixin)
     *   [Duplicating a model instance](#duplicating-a-model-instance)
     *   [Bulk cloning a model](#bulk-cloning-a-model)
     *   [Creating clones without subclassing `CloneMixin`.](#creating-clones-without-subclassing-clonemixin)
     *   [CloneMixin attributes](#clonemixin-attributes)
@@ -93,15 +95,25 @@
 *   [Compatibility](#compatibility)
 *   [Running locally](#running-locally)
 *   [Found a Bug?](#found-a-bug)
 *   [Contributors ✨](#contributors-)
 
 ## Installation
 
-![](https://user-images.githubusercontent.com/17484350/221386740-aa66df70-eed0-40ed-9c5f-1d3b6c9045c2.png)
+### pip
+
+```bash
+pip install django-clone
+```
+
+### poetry
+
+```bash
+poetry add django-clone
+```
 
 ## Usage
 
 ### Subclassing the `CloneModel`
 
 ![](https://user-images.githubusercontent.com/17484350/221387430-efd5508a-2597-4320-9750-5a4c56833edb.png)
```

### Comparing `django-clone-5.3.1/README.md` & `django-clone-5.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center"> 
     <img width="466" alt="4FC889E9-FF59-4E44-9EB6-2AF7DC034C74" src="https://user-images.githubusercontent.com/17484350/215616634-17439a58-7bd8-4e9c-989f-e6bef7c73e48.png">
 </p>
 
 |  Python   | Django  |  Downloads  |   Code Style   |
 |:---------:|:-------:|:-----------:|:--------------:|
-| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/3.2/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/dev/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 |    PyPI         | Test | Vulnerabilities | Coverage | Code Quality  |  Pre-Commit   |
 |:---------------:|:----:|:---------------:|:--------:|:-------------:|:-------------:|
 | [![PyPI version](https://badge.fury.io/py/django-clone.svg)](https://badge.fury.io/py/django-clone) | [![Test](https://github.com/tj-django/django-clone/workflows/Test/badge.svg)](https://github.com/tj-django/django-clone/actions?query=workflow%3ATest) | [![Known Vulnerabilities](https://snyk.io/test/github/tj-django/django-clone/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/tj-django/django-clone?targetFile=requirements.txt) | [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Coverage) <br/> [![codecov](https://codecov.io/gh/tj-django/django-clone/branch/main/graph/badge.svg?token=2NE21Oe50Q)](https://codecov.io/gh/tj-django/django-clone)| [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Grade) |  [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tj-django/django-clone/main.svg)](https://results.pre-commit.ci/latest/github/tj-django/django-clone/main) |
 
 ## django-clone
 
@@ -24,14 +24,16 @@
 *   Restrict fields used for creating a duplicate instance.
 *   Detects unique fields and naively adds a suffix `copy {count}` to each duplicate instance (for supported fields only).
 *   Optionally differentiate between a duplicate instance and the original by appending a **copy** suffix to non unique fields (for supported fields only).
 
 ## Table of Contents
 
 *   [Installation](#installation)
+    *   [pip](#pip)
+    *   [poetry](#poetry)
 *   [Usage](#usage)
     *   [Subclassing the `CloneModel`](#subclassing-the-clonemodel)
     *   [Using the `CloneMixin`](#using-the-clonemixin)
     *   [Duplicating a model instance](#duplicating-a-model-instance)
     *   [Bulk cloning a model](#bulk-cloning-a-model)
     *   [Creating clones without subclassing `CloneMixin`.](#creating-clones-without-subclassing-clonemixin)
     *   [CloneMixin attributes](#clonemixin-attributes)
@@ -52,15 +54,25 @@
 *   [Compatibility](#compatibility)
 *   [Running locally](#running-locally)
 *   [Found a Bug?](#found-a-bug)
 *   [Contributors ✨](#contributors-)
 
 ## Installation
 
-![](https://user-images.githubusercontent.com/17484350/221386740-aa66df70-eed0-40ed-9c5f-1d3b6c9045c2.png)
+### pip
+
+```bash
+pip install django-clone
+```
+
+### poetry
+
+```bash
+poetry add django-clone
+```
 
 ## Usage
 
 ### Subclassing the `CloneModel`
 
 ![](https://user-images.githubusercontent.com/17484350/221387430-efd5508a-2597-4320-9750-5a4c56833edb.png)
```

### Comparing `django-clone-5.3.1/django_clone.egg-info/PKG-INFO` & `django-clone-5.3.2/django_clone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-clone
-Version: 5.3.1
+Version: 5.3.2
 Summary: Create a clone of a django model instance.
 Home-page: https://github.com/tj-django/django-clone.git
 Author: Tonye Jack
 Author-email: jtonye@ymail.com
 Maintainer: Tonye Jack
 Maintainer-email: jtonye@ymail.com
 License: MIT/Apache-2.0
@@ -41,15 +41,15 @@
 
 <p align="center"> 
     <img width="466" alt="4FC889E9-FF59-4E44-9EB6-2AF7DC034C74" src="https://user-images.githubusercontent.com/17484350/215616634-17439a58-7bd8-4e9c-989f-e6bef7c73e48.png">
 </p>
 
 |  Python   | Django  |  Downloads  |   Code Style   |
 |:---------:|:-------:|:-----------:|:--------------:|
-| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/3.2/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
+| [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django_clone.svg)](https://pypi.org/project/django-clone) | [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django_clone.svg)](https://docs.djangoproject.com/en/dev/releases/) | [![Downloads](https://pepy.tech/badge/django-clone)](https://pepy.tech/project/django-clone) | [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
 
 |    PyPI         | Test | Vulnerabilities | Coverage | Code Quality  |  Pre-Commit   |
 |:---------------:|:----:|:---------------:|:--------:|:-------------:|:-------------:|
 | [![PyPI version](https://badge.fury.io/py/django-clone.svg)](https://badge.fury.io/py/django-clone) | [![Test](https://github.com/tj-django/django-clone/workflows/Test/badge.svg)](https://github.com/tj-django/django-clone/actions?query=workflow%3ATest) | [![Known Vulnerabilities](https://snyk.io/test/github/tj-django/django-clone/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/tj-django/django-clone?targetFile=requirements.txt) | [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Coverage) <br/> [![codecov](https://codecov.io/gh/tj-django/django-clone/branch/main/graph/badge.svg?token=2NE21Oe50Q)](https://codecov.io/gh/tj-django/django-clone)| [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b33dd02dbb034d7fa9886a99f5383ea6)](https://www.codacy.com/gh/tj-django/django-clone?utm_source=github.com\&utm_medium=referral\&utm_content=tj-django/django-clone\&utm_campaign=Badge_Grade) |  [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tj-django/django-clone/main.svg)](https://results.pre-commit.ci/latest/github/tj-django/django-clone/main) |
 
 ## django-clone
 
@@ -65,14 +65,16 @@
 *   Restrict fields used for creating a duplicate instance.
 *   Detects unique fields and naively adds a suffix `copy {count}` to each duplicate instance (for supported fields only).
 *   Optionally differentiate between a duplicate instance and the original by appending a **copy** suffix to non unique fields (for supported fields only).
 
 ## Table of Contents
 
 *   [Installation](#installation)
+    *   [pip](#pip)
+    *   [poetry](#poetry)
 *   [Usage](#usage)
     *   [Subclassing the `CloneModel`](#subclassing-the-clonemodel)
     *   [Using the `CloneMixin`](#using-the-clonemixin)
     *   [Duplicating a model instance](#duplicating-a-model-instance)
     *   [Bulk cloning a model](#bulk-cloning-a-model)
     *   [Creating clones without subclassing `CloneMixin`.](#creating-clones-without-subclassing-clonemixin)
     *   [CloneMixin attributes](#clonemixin-attributes)
@@ -93,15 +95,25 @@
 *   [Compatibility](#compatibility)
 *   [Running locally](#running-locally)
 *   [Found a Bug?](#found-a-bug)
 *   [Contributors ✨](#contributors-)
 
 ## Installation
 
-![](https://user-images.githubusercontent.com/17484350/221386740-aa66df70-eed0-40ed-9c5f-1d3b6c9045c2.png)
+### pip
+
+```bash
+pip install django-clone
+```
+
+### poetry
+
+```bash
+poetry add django-clone
+```
 
 ## Usage
 
 ### Subclassing the `CloneModel`
 
 ![](https://user-images.githubusercontent.com/17484350/221387430-efd5508a-2597-4320-9750-5a4c56833edb.png)
```

### Comparing `django-clone-5.3.1/django_clone.egg-info/SOURCES.txt` & `django-clone-5.3.2/django_clone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/model_clone/admin.py` & `django-clone-5.3.2/model_clone/admin.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/model_clone/mixin.py` & `django-clone-5.3.2/model_clone/mixin.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/model_clone/utils.py` & `django-clone-5.3.2/model_clone/utils.py`

 * *Files identical despite different names*

### Comparing `django-clone-5.3.1/setup.py` & `django-clone-5.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     with io.open(README_PATH, encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 else:
     LONG_DESCRIPTION = ""
 
 setup(
     name="django-clone",
-    version="5.3.1",
+    version="5.3.2",
     description="Create a clone of a django model instance.",
     python_requires=">=3.6",
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESCRIPTION_TYPE,
     author="Tonye Jack",
     author_email="jtonye@ymail.com",
     maintainer="Tonye Jack",
```


# Comparing `tmp/nitpick-0.33.1.tar.gz` & `tmp/nitpick-0.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitpick-0.33.1.tar", max compression
+gzip compressed data, was "nitpick-0.33.2.tar", max compression
```

## Comparing `nitpick-0.33.1.tar` & `nitpick-0.33.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     1080 2023-03-29 18:52:34.028277 nitpick-0.33.1/LICENSE
--rw-r--r--   0        0        0    17274 2023-03-29 18:53:05.782781 nitpick-0.33.1/README.rst
--rw-r--r--   0        0        0     4342 2023-03-29 18:53:05.786781 nitpick-0.33.1/pyproject.toml
--rw-r--r--   0        0        0      213 2023-03-29 18:53:05.786781 nitpick-0.33.1/src/nitpick/__init__.py
--rw-r--r--   0        0        0      316 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/__main__.py
--rw-r--r--   0        0        0    25317 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/blender.py
--rw-r--r--   0        0        0     5459 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/cli.py
--rw-r--r--   0        0        0      325 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/compat.py
--rw-r--r--   0        0        0      603 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/config.py
--rw-r--r--   0        0        0     1660 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/constants.py
--rw-r--r--   0        0        0     4850 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/core.py
--rw-r--r--   0        0        0     1181 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/enums.py
--rw-r--r--   0        0        0     2671 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/exceptions.py
--rw-r--r--   0        0        0     2631 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/fields.py
--rw-r--r--   0        0        0     3112 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/flake8.py
--rw-r--r--   0        0        0     3637 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/generic.py
--rw-r--r--   0        0        0     1197 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/__init__.py
--rw-r--r--   0        0        0     6690 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/base.py
--rw-r--r--   0        0        0      893 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/info.py
--rw-r--r--   0        0        0    12591 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/ini.py
--rw-r--r--   0        0        0     4366 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/json.py
--rw-r--r--   0        0        0     2646 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/text.py
--rw-r--r--   0        0        0     2643 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/toml.py
--rw-r--r--   0        0        0     5441 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/plugins/yaml.py
--rw-r--r--   0        0        0     8391 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/project.py
--rw-r--r--   0        0        0       84 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/__init__.py
--rw-r--r--   0        0        0       31 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/__init__.py
--rw-r--r--   0        0        0      672 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/codeclimate.toml
--rw-r--r--   0        0        0      277 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/commitizen.toml
--rw-r--r--   0        0        0      473 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/commitlint.toml
--rw-r--r--   0        0        0      762 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/editorconfig.toml
--rw-r--r--   0        0        0      226 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/git-legal.toml
--rw-r--r--   0        0        0      256 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/markdownlint.toml
--rw-r--r--   0        0        0      525 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/pre-commit-hooks.toml
--rw-r--r--   0        0        0      250 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/any/prettier.toml
--rw-r--r--   0        0        0       29 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/javascript/__init__.py
--rw-r--r--   0        0        0      231 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/javascript/package-json.toml
--rw-r--r--   0        0        0       25 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/kotlin/__init__.py
--rw-r--r--   0        0        0      301 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/kotlin/ktlint.toml
--rw-r--r--   0        0        0       21 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/presets/__init__.py
--rw-r--r--   0        0        0     1547 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/presets/nitpick.toml
--rw-r--r--   0        0        0       33 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/proto/__init__.py
--rw-r--r--   0        0        0      251 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/proto/protolint.toml
--rw-r--r--   0        0        0       98 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/python/310.toml
--rw-r--r--   0        0        0       98 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/python/311.toml
--rw-r--r--   0        0        0       96 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/python/37.toml
--rw-r--r--   0        0        0       96 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/python/38.toml
--rw-r--r--   0        0        0       96 2023-03-29 18:52:34.032277 nitpick-0.33.1/src/nitpick/resources/python/39.toml
--rw-r--r--   0        0        0       25 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/__init__.py
--rw-r--r--   0        0        0      452 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/absent.toml
--rw-r--r--   0        0        0      359 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/autoflake.toml
--rw-r--r--   0        0        0      385 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/bandit.toml
--rw-r--r--   0        0        0      470 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/black.toml
--rw-r--r--   0        0        0     1206 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/flake8.toml
--rw-r--r--   0        0        0     1112 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/github-workflow.toml
--rw-r--r--   0        0        0      149 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/ipython.toml
--rw-r--r--   0        0        0      567 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/isort.toml
--rw-r--r--   0        0        0      752 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/mypy.toml
--rw-r--r--   0        0        0      420 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/poetry-editable.toml
--rw-r--r--   0        0        0      242 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/poetry.toml
--rw-r--r--   0        0        0      864 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/pre-commit-hooks.toml
--rw-r--r--   0        0        0     2777 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/pylint.toml
--rw-r--r--   0        0        0      294 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/radon.toml
--rw-r--r--   0        0        0      357 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/readthedocs.toml
--rw-r--r--   0        0        0      208 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/sonar-python.toml
--rw-r--r--   0        0        0      217 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/stable.toml
--rw-r--r--   0        0        0      825 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/python/tox.toml
--rw-r--r--   0        0        0       32 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/shell/__init__.py
--rw-r--r--   0        0        0      332 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/shell/bashate.toml
--rw-r--r--   0        0        0      726 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/shell/shellcheck.toml
--rw-r--r--   0        0        0      299 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/resources/shell/shfmt.toml
--rw-r--r--   0        0        0     3160 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/schemas.py
--rw-r--r--   0        0        0      179 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/__init__.py
--rw-r--r--   0        0        0     1576 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/cache.py
--rw-r--r--   0        0        0     2871 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/config.py
--rw-r--r--   0        0        0    10218 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/core.py
--rw-r--r--   0        0        0     4213 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/__init__.py
--rw-r--r--   0        0        0     2310 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/base.py
--rw-r--r--   0        0        0     1547 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/file.py
--rw-r--r--   0        0        0     5991 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/github.py
--rw-r--r--   0        0        0     1575 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/http.py
--rw-r--r--   0        0        0     4683 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/style/fetchers/pypackage.py
--rw-r--r--   0        0        0      804 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/typedefs.py
--rw-r--r--   0        0        0     5054 2023-03-29 18:52:34.036277 nitpick-0.33.1/src/nitpick/violations.py
--rw-r--r--   0        0        0    20098 1970-01-01 00:00:00.000000 nitpick-0.33.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-29 15:13:52.349178 nitpick-0.33.2/LICENSE
+-rw-r--r--   0        0        0    17274 2023-05-29 15:14:20.985303 nitpick-0.33.2/README.rst
+-rw-r--r--   0        0        0     6465 2023-05-29 15:14:20.989304 nitpick-0.33.2/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-05-29 15:14:20.989304 nitpick-0.33.2/src/nitpick/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/__main__.py
+-rw-r--r--   0        0        0    25395 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/blender.py
+-rw-r--r--   0        0        0     5474 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/cli.py
+-rw-r--r--   0        0        0      345 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/compat.py
+-rw-r--r--   0        0        0      603 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/config.py
+-rw-r--r--   0        0        0     1664 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/constants.py
+-rw-r--r--   0        0        0     4872 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/core.py
+-rw-r--r--   0        0        0     1181 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/enums.py
+-rw-r--r--   0        0        0     2717 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/exceptions.py
+-rw-r--r--   0        0        0     2734 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/fields.py
+-rw-r--r--   0        0        0     3127 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/flake8.py
+-rw-r--r--   0        0        0     3679 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/generic.py
+-rw-r--r--   0        0        0     1212 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/__init__.py
+-rw-r--r--   0        0        0     6795 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/base.py
+-rw-r--r--   0        0        0      893 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/info.py
+-rw-r--r--   0        0        0    12599 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/ini.py
+-rw-r--r--   0        0        0     4408 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/json.py
+-rw-r--r--   0        0        0     2684 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/text.py
+-rw-r--r--   0        0        0     3062 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/toml.py
+-rw-r--r--   0        0        0     5483 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/plugins/yaml.py
+-rw-r--r--   0        0        0     8418 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/project.py
+-rw-r--r--   0        0        0       84 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/__init__.py
+-rw-r--r--   0        0        0      672 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/codeclimate.toml
+-rw-r--r--   0        0        0      277 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/commitizen.toml
+-rw-r--r--   0        0        0      473 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/commitlint.toml
+-rw-r--r--   0        0        0      762 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/editorconfig.toml
+-rw-r--r--   0        0        0      226 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/git-legal.toml
+-rw-r--r--   0        0        0      256 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/markdownlint.toml
+-rw-r--r--   0        0        0      525 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/pre-commit-hooks.toml
+-rw-r--r--   0        0        0      250 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/any/prettier.toml
+-rw-r--r--   0        0        0       29 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/javascript/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/javascript/package-json.toml
+-rw-r--r--   0        0        0       25 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/kotlin/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/kotlin/ktlint.toml
+-rw-r--r--   0        0        0       21 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/presets/__init__.py
+-rw-r--r--   0        0        0     1238 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/presets/nitpick.toml
+-rw-r--r--   0        0        0       33 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/proto/__init__.py
+-rw-r--r--   0        0        0      251 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/proto/protolint.toml
+-rw-r--r--   0        0        0       98 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/310.toml
+-rw-r--r--   0        0        0       98 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/311.toml
+-rw-r--r--   0        0        0       96 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/37.toml
+-rw-r--r--   0        0        0       96 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/38.toml
+-rw-r--r--   0        0        0       96 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/39.toml
+-rw-r--r--   0        0        0       25 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/absent.toml
+-rw-r--r--   0        0        0      359 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/autoflake.toml
+-rw-r--r--   0        0        0      385 2023-05-29 15:13:52.353178 nitpick-0.33.2/src/nitpick/resources/python/bandit.toml
+-rw-r--r--   0        0        0      470 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/black.toml
+-rw-r--r--   0        0        0     1206 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/flake8.toml
+-rw-r--r--   0        0        0     1128 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/github-workflow.toml
+-rw-r--r--   0        0        0      149 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/ipython.toml
+-rw-r--r--   0        0        0      567 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/isort.toml
+-rw-r--r--   0        0        0      752 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/mypy.toml
+-rw-r--r--   0        0        0      420 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/poetry-editable.toml
+-rw-r--r--   0        0        0      242 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/poetry.toml
+-rw-r--r--   0        0        0      487 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/pre-commit-hooks.toml
+-rw-r--r--   0        0        0     2777 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/pylint.toml
+-rw-r--r--   0        0        0      294 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/radon.toml
+-rw-r--r--   0        0        0      357 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/readthedocs.toml
+-rw-r--r--   0        0        0      208 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/sonar-python.toml
+-rw-r--r--   0        0        0      217 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/stable.toml
+-rw-r--r--   0        0        0      825 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/python/tox.toml
+-rw-r--r--   0        0        0       32 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/shell/__init__.py
+-rw-r--r--   0        0        0      332 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/shell/bashate.toml
+-rw-r--r--   0        0        0      726 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/shell/shellcheck.toml
+-rw-r--r--   0        0        0      299 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/resources/shell/shfmt.toml
+-rw-r--r--   0        0        0     3160 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/schemas.py
+-rw-r--r--   0        0        0      179 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/cache.py
+-rw-r--r--   0        0        0     2871 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/config.py
+-rw-r--r--   0        0        0    10479 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/core.py
+-rw-r--r--   0        0        0     4245 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/__init__.py
+-rw-r--r--   0        0        0     2371 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/base.py
+-rw-r--r--   0        0        0     1559 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/file.py
+-rw-r--r--   0        0        0     6018 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/github.py
+-rw-r--r--   0        0        0     1663 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/http.py
+-rw-r--r--   0        0        0     4764 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/style/fetchers/pypackage.py
+-rw-r--r--   0        0        0      804 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/typedefs.py
+-rw-r--r--   0        0        0     5004 2023-05-29 15:13:52.357178 nitpick-0.33.2/src/nitpick/violations.py
+-rw-r--r--   0        0        0    20098 1970-01-01 00:00:00.000000 nitpick-0.33.2/PKG-INFO
```

### Comparing `nitpick-0.33.1/LICENSE` & `nitpick-0.33.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/README.rst` & `nitpick-0.33.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you use `pre-commit <https://pre-commit.com/>`_ on your project, add
 this to the ``.pre-commit-config.yaml`` in your repository::
 
     repos:
       - repo: https://github.com/andreoliwa/nitpick
-        rev: v0.33.1
+        rev: v0.33.2
         hooks:
           - id: nitpick
 
 There are 3 available hook IDs:
 
 - ``nitpick`` and ``nitpick-fix`` both run the ``nitpick fix`` command;
 - ``nitpick-check`` runs ``nitpick check``.
@@ -399,15 +399,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you use `MegaLinter <https://megalinter.github.io/>`_ you can run Nitpick as a plugin. Add the following two entries to your ``.mega-linter.yml`` configuration file:
 
 .. code-block:: yaml
 
     PLUGINS:
-      - https://raw.githubusercontent.com/andreoliwa/nitpick/v0.33.1/mega-linter-plugin-nitpick/nitpick.megalinter-descriptor.yml
+      - https://raw.githubusercontent.com/andreoliwa/nitpick/v0.33.2/mega-linter-plugin-nitpick/nitpick.megalinter-descriptor.yml
     ENABLE_LINTERS:
       - NITPICK
 
 
 More information
 ----------------
```

### Comparing `nitpick-0.33.1/src/nitpick/blender.py` & `nitpick-0.33.2/src/nitpick/blender.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 
 import abc
 import json
 import re
 import shlex
 from functools import partial
 from pathlib import Path
-from typing import Any, Callable, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 
 import dictdiffer
 import jmespath
 import toml
 import tomlkit
 from attr import define  # type: ignore[attr-defined]
 from autorepr import autorepr
 from flatten_dict import flatten, unflatten
-from jmespath.parser import ParsedResult
 from ruamel.yaml import YAML, RoundTripRepresenter, StringIO
 from sortedcontainers import SortedDict
 from tomlkit import items
 
-from nitpick.config import SpecialConfig
 from nitpick.typedefs import ElementData, JsonDict, ListOrCommentedSeq, PathOrStr, YamlObject, YamlValue
 
+if TYPE_CHECKING:
+    from jmespath.parser import ParsedResult
+
+    from nitpick.config import SpecialConfig
+
 # Generic type for classes that inherit from BaseDoc
 TBaseDoc = TypeVar("TBaseDoc", bound="BaseDoc")
 
 SINGLE_QUOTE = "'"
 DOUBLE_QUOTE = '"'
 
 SEPARATOR_DOT = "."
@@ -148,17 +151,16 @@
 
     def find_by_key(self, desired: ElementDetail) -> ElementDetail | None:
         """Find an element by key."""
         for actual in self.elements:
             if isinstance(desired.key, list):
                 if set(desired.key).issubset(set(actual.key)):
                     return actual
-            else:
-                if desired.key == actual.key:
-                    return actual
+            elif desired.key == actual.key:
+                return actual
         return None
 
 
 def set_key_if_not_empty(dict_: JsonDict, key: str, value: Any) -> None:
     """Update the dict if the value is valid."""
     if not value:
         return
@@ -187,15 +189,15 @@
         return string_.split(separator)
 
     quoted_regex = re.compile(
         f"([{SINGLE_QUOTE}{DOUBLE_QUOTE}][^{SINGLE_QUOTE}{DOUBLE_QUOTE}]+[{SINGLE_QUOTE}{DOUBLE_QUOTE}])"
     )
 
     def remove_quotes(match):
-        return match.group(0).strip("".join([SINGLE_QUOTE, DOUBLE_QUOTE])).replace(separator, SEPARATOR_QUOTED_SPLIT)
+        return match.group(0).strip(f"{SINGLE_QUOTE}{DOUBLE_QUOTE}").replace(separator, SEPARATOR_QUOTED_SPLIT)
 
     return [
         part.replace(SEPARATOR_QUOTED_SPLIT, separator)
         for part in quoted_regex.sub(remove_quotes, string_).split(separator)
     ]
 
 
@@ -238,16 +240,16 @@
     return _inner_custom_reducer
 
 
 def custom_splitter(separator: str) -> Callable:
     """Custom splitter for :py:meth:`flatten_dict.flatten_dict.unflatten()` accepting a separator."""
 
     def _inner_custom_splitter(flat_key) -> tuple[str, ...]:
-        keys = tuple(flat_key.split(separator))
-        return keys
+        """Return a tuple of keys split by the separator."""
+        return tuple(flat_key.split(separator))
 
     return _inner_custom_splitter
 
 
 # TODO: refactor: use only tomlkit and remove uiri/toml
 #  - tomlkit preserves comments
 #  - uiri/toml looks abandoned https://github.com/uiri/toml/issues/361
@@ -358,15 +360,15 @@
                     ListDetail.from_data(expected_value, jmes_key),
                 )
             elif expected_value != actual:
                 set_key_if_not_empty(self.diff_dict, key, expected_value)
 
         return self
 
-    def _compare_list_elements(  # pylint: disable=too-many-arguments
+    def _compare_list_elements(  # pylint: disable=too-many-arguments # noqa: PLR0913
         self, key: str, parent_key: str, child_key: str, actual_detail: ListDetail, expected_detail: ListDetail
     ) -> None:
         """Compare list elements by their keys or hashes."""
         display = []
         replace = actual_detail.data.copy()
         for expected_element in expected_detail.elements:
             actual_element = actual_detail.find_by_key(expected_element)
@@ -560,15 +562,15 @@
 
 class SensibleYAML(YAML):
     """YAML with sensible defaults but an inefficient dump to string.
 
     `Output of dump() as a string <https://yaml.readthedocs.io/en/latest/example.html#output-of-dump-as-a-string>`_.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.map_indent = 2
         self.sequence_indent = 4
         self.sequence_dash_offset = 2
         self.preserve_quotes = True
 
     def loads(self, string: str):
```

### Comparing `nitpick-0.33.1/src/nitpick/cli.py` & `nitpick-0.33.2/src/nitpick/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 @click.option(
     f"--{OptionEnum.OFFLINE.name.lower()}",  # pylint: disable=no-member
     is_flag=True,
     default=False,
     help=OptionEnum.OFFLINE.value,
 )
 @click.version_option()
-def nitpick_cli(project: Path | None = None, offline=False):  # pylint: disable=unused-argument
+def nitpick_cli(project: Path | None = None, offline=False):  # pylint: disable=unused-argument # noqa: ARG001
     """Enforce the same settings across multiple language-independent projects."""
 
 
 def get_nitpick(context: click.Context) -> Nitpick:
     """Create a Nitpick instance from the click context parameters."""
     project = None
     offline = False
```

### Comparing `nitpick-0.33.1/src/nitpick/config.py` & `nitpick-0.33.2/src/nitpick/config.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/constants.py` & `nitpick-0.33.2/src/nitpick/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     REQUIREMENTS_STAR_TXT,
     PIPFILE_STAR,
     TOX_INI,
     PACKAGE_JSON,
     CARGO_STAR,
     GO_MOD,
     GO_SUM,
-) + ROOT_PYTHON_FILES
+    *ROOT_PYTHON_FILES,
+)
 CONFIG_FILES = (DOT_NITPICK_TOML, PYPROJECT_TOML)
 
 # Config sections and keys
 TOOL_KEY = "tool"
 TOOL_NITPICK_KEY = f"{TOOL_KEY}.{PROJECT_NAME}"
 
 # JMESPath expressions
```

### Comparing `nitpick-0.33.1/src/nitpick/core.py` & `nitpick-0.33.2/src/nitpick/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
     _allow_init = False
 
     project: Project
 
     def __init__(self) -> None:
         if not self._allow_init:
-            raise TypeError("This class cannot be instantiated directly. Use Nitpick.singleton().init(...) instead")
+            msg = "This class cannot be instantiated directly. Use Nitpick.singleton().init(...) instead"
+            raise TypeError(msg)
 
         self.offline: bool = False
 
     @classmethod
     @lru_cache()
     def singleton(cls) -> "Nitpick":
         """Return a single instance of the class."""
```

### Comparing `nitpick-0.33.1/src/nitpick/enums.py` & `nitpick-0.33.2/src/nitpick/enums.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/exceptions.py` & `nitpick-0.33.2/src/nitpick/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Nitpick exceptions."""
+from __future__ import annotations
+
 import warnings
-from typing import Any, Dict, List, Union
+from typing import TYPE_CHECKING, Any
 
 from more_itertools import always_iterable
 
 from nitpick.constants import PRE_COMMIT_CONFIG_YAML, PROJECT_NAME
-from nitpick.violations import Fuss
+
+if TYPE_CHECKING:
+    from nitpick.violations import Fuss
 
 
 class QuitComplainingError(Exception):
     """Quit complaining and exit the application."""
 
-    def __init__(self, violations: Union[Fuss, List[Fuss]]) -> None:
+    def __init__(self, violations: Fuss | list[Fuss]) -> None:
         super().__init__()
-        self.violations: List[Fuss] = list(always_iterable(violations))
+        self.violations: list[Fuss] = list(always_iterable(violations))
 
 
 class Deprecation:
     """All deprecation messages in a single class.
 
     When it's time to break compatibility, remove a method/warning below,
     and older config files will trigger validation errors on Nitpick.
@@ -33,15 +37,15 @@
                 stacklevel=2,
             )
             return True
 
         return False
 
     @staticmethod
-    def jsonfile_section(style_errors: Dict[str, Any]) -> bool:
+    def jsonfile_section(style_errors: dict[str, Any]) -> bool:
         """The [nitpick.JSONFile] is not needed anymore; JSON files are now detected by the extension."""
         has_nitpick_jsonfile_section = style_errors.get(PROJECT_NAME, {}).pop("JSONFile", None)
         if has_nitpick_jsonfile_section:
             style_errors.pop(PROJECT_NAME)
             warnings.warn(
                 "The [nitpick.JSONFile] section is not needed anymore; just declare your JSON files directly",
                 DeprecationWarning,
@@ -65,8 +69,8 @@
             stacklevel=2,
         )
         return True
 
 
 def pretty_exception(err: Exception, message: str = ""):
     """Return a pretty error message with the full path of the Exception."""
-    return f"{message} ({err.__module__}.{err.__class__.__name__}: {str(err)})"
+    return f"{message} ({err.__module__}.{err.__class__.__name__}: {err!s})"
```

### Comparing `nitpick-0.33.1/src/nitpick/fields.py` & `nitpick-0.33.2/src/nitpick/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from more_itertools import always_iterable
 
 from nitpick.constants import DOT
 from nitpick.exceptions import pretty_exception
 
 __all__ = ("Dict", "Field", "List", "Nested", "String", "URL")
 
+MAX_PARTS = 2
+
 
 def is_valid_json(json_string: str) -> bool:
     """Validate the string as JSON."""
     try:
         json.loads(json_string)
     except json.JSONDecodeError as err:
         raise ValidationError(pretty_exception(err, "Invalid JSON")) from err
@@ -28,49 +30,53 @@
         """Validate the trimmed string."""
         return super().__call__(value.strip())
 
 
 class NonEmptyString(fields.String):
     """A string field that must not be empty even after trimmed."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         validate = list(always_iterable(kwargs.pop("validate", None)))
         validate.append(TrimmedLength(min=1))
         super().__init__(validate=validate, **kwargs)
 
 
 class JsonString(fields.String):
     """A string field with valid JSON content."""
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         validate = kwargs.pop("validate", [])
         validate.append(is_valid_json)
         super().__init__(validate=validate, **kwargs)
 
 
-def string_or_list_field(object_dict, parent_object_dict):  # pylint: disable=unused-argument
+def string_or_list_field(object_dict, parent_object_dict):  # pylint: disable=unused-argument # noqa: ARG001
     """Detect if the field is a string or a list."""
     if isinstance(object_dict, list):
         return fields.List(NonEmptyString(required=True, allow_none=False))
     return NonEmptyString()
 
 
 def validate_section_dot_field(section_field: str) -> bool:
     """Validate if the combination section/field has a dot separating them."""
     common = "Use <section_name>.<field_name>"
+    msg = ""
     if DOT not in section_field:
-        raise ValidationError(f"Dot is missing. {common}")
-    parts = section_field.split(DOT)
-    if len(parts) > 2:
-        raise ValidationError(f"There's more than one dot. {common}")
-    if not parts[0].strip():
-        raise ValidationError(f"Empty section name. {common}")
-    if not parts[1].strip():
-        raise ValidationError(f"Empty field name. {common}")
+        msg = f"Dot is missing. {common}"
+    else:
+        parts = section_field.split(DOT)
+        if len(parts) > MAX_PARTS:
+            msg = f"There's more than one dot. {common}"
+        elif not parts[0].strip():
+            msg = f"Empty section name. {common}"
+        elif not parts[1].strip():
+            msg = f"Empty field name. {common}"
+    if msg:
+        raise ValidationError(msg)
     return True
 
 
-def boolean_or_dict_field(object_dict, parent_object_dict):  # pylint: disable=unused-argument
+def boolean_or_dict_field(object_dict, parent_object_dict):  # pylint: disable=unused-argument # noqa: ARG001
     """Detect if the field is a boolean or a dict."""
     if isinstance(object_dict, dict):
         return fields.Dict
     return fields.Bool
```

### Comparing `nitpick-0.33.1/src/nitpick/flake8.py` & `nitpick-0.33.2/src/nitpick/flake8.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def add_options(option_manager: OptionManager):
         """Add the offline option."""
         option_manager.add_option(
             OptionEnum.OFFLINE.as_flake8_flag(), action="store_true", help=OptionEnum.OFFLINE.value
         )
 
     @staticmethod
-    def parse_options(option_manager: OptionManager, options, args):  # pylint: disable=unused-argument
+    def parse_options(option_manager: OptionManager, options, args):  # pylint: disable=unused-argument # noqa: ARG004
         """Create the Nitpick app, set logging from the verbose flags, set offline mode.
 
         This function is called only once by flake8, so it's a good place to create the app.
         """
         log_mapping = {1: logging.INFO, 2: logging.DEBUG}
         logging.basicConfig(level=log_mapping.get(options.verbose, logging.WARNING))
```

### Comparing `nitpick-0.33.1/src/nitpick/generic.py` & `nitpick-0.33.2/src/nitpick/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
     from nitpick.generic import *
 """
 from __future__ import annotations
 
 import sys
 from pathlib import Path, PosixPath, WindowsPath
-from typing import Iterable
-
-from furl import furl
+from typing import TYPE_CHECKING, Iterable
 
 from nitpick.constants import DOT, PROJECT_NAME
-from nitpick.typedefs import PathOrStr
+
+if TYPE_CHECKING:
+    from furl import furl
+
+    from nitpick.typedefs import PathOrStr
 
 
 def version_to_tuple(version: str | None = None) -> tuple[int, ...]:
     """Transform a version number into a tuple of integers, for comparison.
 
     >>> version_to_tuple("")
     ()
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/__init__.py` & `nitpick-0.33.2/src/nitpick/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 
 @hookspec
 def plugin_class() -> type[NitpickPlugin]:  # type: ignore[empty-body]
     """Return your plugin class here (it should inherit from :py:class:`nitpick.plugins.base.NitpickPlugin`)."""
 
 
 @hookspec
-def can_handle(info: FileInfo) -> type[NitpickPlugin] | None:  # pylint: disable=unused-argument
+def can_handle(info: FileInfo) -> type[NitpickPlugin] | None:  # pylint: disable=unused-argument # noqa: ARG001
     """Return a valid :py:class:`nitpick.plugins.base.NitpickPlugin` instance or ``None``.
 
     :return: A plugin instance if your plugin handles this file info (path or any of its ``identify`` tags).
         Return ``None`` if your plugin doesn't handle this file or file type.
     """
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/base.py` & `nitpick-0.33.2/src/nitpick/plugins/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """Base class for file checkers."""
 from __future__ import annotations
 
 import abc
 import fnmatch
-from pathlib import Path
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator
 
 from autorepr import autotext
 from loguru import logger
-from marshmallow import Schema
 
 from nitpick.blender import BaseDoc, flatten_quotes, search_json
 from nitpick.config import SpecialConfig
 from nitpick.constants import DUNDER_LIST_KEYS
-from nitpick.plugins.info import FileInfo
 from nitpick.typedefs import JsonDict, mypy_property
 from nitpick.violations import Fuss, Reporter, SharedViolations
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from marshmallow import Schema
+
+    from nitpick.plugins.info import FileInfo
+
 
 class NitpickPlugin(metaclass=abc.ABCMeta):  # pylint: disable=too-many-instance-attributes
     """Base class for Nitpick plugins.
 
     :param data: File information (project, path, tags).
     :param expected_config: Expected configuration for the file
     :param autofix: Flag to modify files, if the plugin supports it (default: True).
@@ -130,15 +134,18 @@
         logger.info(f"{self}: Suggest initial contents for {self.filename}")
 
         if suggestion:
             yield self.reporter.make_fuss(SharedViolations.CREATE_FILE_WITH_SUGGESTION, suggestion, fixed=self.autofix)
         else:
             yield self.reporter.make_fuss(SharedViolations.CREATE_FILE)
 
-    def write_file(self, file_exists: bool) -> Fuss | None:  # pylint: disable=unused-argument,no-self-use
+    def write_file(  # pylint: disable=no-self-use
+        self,
+        file_exists: bool,  # pylint: disable=unused-argument # noqa: ARG002
+    ) -> Fuss | None:
         """Hook to write the new file when autofix mode is on. Should be used by inherited classes."""
         return None
 
     @abc.abstractmethod
     def enforce_rules(self) -> Iterator[Fuss]:
         """Enforce rules for this file. It must be overridden by inherited classes if needed."""
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/info.py` & `nitpick-0.33.2/src/nitpick/plugins/info.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/plugins/ini.py` & `nitpick-0.33.2/src/nitpick/plugins/ini.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """INI files."""
 from __future__ import annotations
 
 from configparser import ConfigParser, DuplicateOptionError, Error, MissingSectionHeaderError, ParsingError
 from io import StringIO
-from typing import Any, Iterator
+from typing import TYPE_CHECKING, Any, Iterator
 
 import dictdiffer
 from configupdater import ConfigUpdater, Space
 
 from nitpick.plugins import hookimpl
 from nitpick.plugins.base import NitpickPlugin
-from nitpick.plugins.info import FileInfo
 from nitpick.violations import Fuss, ViolationEnum
 
+if TYPE_CHECKING:
+    from nitpick.plugins.info import FileInfo
+
 COMMA_SEPARATED_VALUES = "comma_separated_values"
 SECTION_SEPARATOR = "."
 TOP_SECTION = "__TEMPORARY_TOP_SECTION__"
 
 
 class Violations(ViolationEnum):
     """Violations for this plugin."""
@@ -58,15 +60,15 @@
         self.comma_separated_values = set(self.nitpick_file_dict.get(COMMA_SEPARATED_VALUES, []))
 
         if not self.needs_top_section:
             return
         if all(isinstance(v, dict) for v in self.expected_config.values()):
             return
 
-        new_config = dict({TOP_SECTION: {}})
+        new_config = {TOP_SECTION: {}}
         for key, value in self.expected_config.items():
             if isinstance(value, dict):
                 new_config[key] = value
                 continue
             new_config[TOP_SECTION][key] = value
         self.expected_config = new_config
 
@@ -286,16 +288,15 @@
             self.updater[section].last_block.add_after.space(1)
 
     @staticmethod
     def get_example_cfg(parser: ConfigParser) -> str:
         """Print an example of a config parser in a string instead of a file."""
         string_stream = StringIO()
         parser.write(string_stream)
-        output = string_stream.getvalue().strip()
-        return output
+        return string_stream.getvalue().strip()
 
 
 @hookimpl
 def plugin_class() -> type[NitpickPlugin]:
     """Handle INI files."""
     return IniPlugin
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/json.py` & `nitpick-0.33.2/src/nitpick/plugins/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """JSON files."""
 from __future__ import annotations
 
 import json
 from itertools import chain
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator
 
 from loguru import logger
 
 from nitpick import fields
 from nitpick.blender import BaseDoc, Comparison, JsonDoc, flatten_quotes, unflatten_quotes
 from nitpick.plugins import hookimpl
 from nitpick.plugins.base import NitpickPlugin
-from nitpick.plugins.info import FileInfo
 from nitpick.schemas import BaseNitpickSchema
-from nitpick.typedefs import JsonDict
 from nitpick.violations import Fuss, SharedViolations, ViolationEnum
 
+if TYPE_CHECKING:
+    from nitpick.plugins.info import FileInfo
+    from nitpick.typedefs import JsonDict
+
 KEY_CONTAINS_KEYS = "contains_keys"
 KEY_CONTAINS_JSON = "contains_json"
 VALUE_PLACEHOLDER = "<some value here>"
 
 
 class JsonFileSchema(BaseNitpickSchema):
     """Validation schema for any JSON file added to the style."""
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/text.py` & `nitpick-0.33.2/src/nitpick/plugins/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Text files."""
 from __future__ import annotations
 
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator
 
 from marshmallow import Schema
 from marshmallow.orderedset import OrderedSet
 
 from nitpick import fields
 from nitpick.plugins import hookimpl
 from nitpick.plugins.base import NitpickPlugin
-from nitpick.plugins.info import FileInfo
 from nitpick.schemas import help_message
 from nitpick.violations import Fuss, ViolationEnum
 
+if TYPE_CHECKING:
+    from nitpick.plugins.info import FileInfo
+
 TEXT_FILE_RTFD_PAGE = "plugins.html#text-files"
 KEY_CONTAINS = "contains"
 
 
 class TextItemSchema(Schema):
     """Validation schema for the object inside ``contains``."""
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/toml.py` & `nitpick-0.33.2/src/nitpick/plugins/toml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """TOML files."""
 from __future__ import annotations
 
 from itertools import chain
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator, cast
 
 from tomlkit import dumps, parse
-from tomlkit.toml_document import TOMLDocument
 
-from nitpick.blender import BaseDoc, Comparison, TomlDoc, traverse_toml_tree
+from nitpick.blender import Comparison, TomlDoc, traverse_toml_tree
 from nitpick.plugins import hookimpl
 from nitpick.plugins.base import NitpickPlugin
-from nitpick.plugins.info import FileInfo
 from nitpick.violations import Fuss, SharedViolations, ViolationEnum
 
+if TYPE_CHECKING:
+    from tomlkit.toml_document import TOMLDocument
+
+    from nitpick.plugins.info import FileInfo
+
 
 class TomlPlugin(NitpickPlugin):
     """Enforce configurations and autofix TOML files.
 
     E.g.: `pyproject.toml (PEP 518) <https://www.python.org/dev/peps/pep-0518/#file-format>`_.
 
     See also `the [tool.poetry] section of the pyproject.toml file
@@ -35,28 +38,42 @@
         toml_doc = TomlDoc(path=self.file_path)
         comparison = Comparison(toml_doc, self.expected_config, self.special_config)()
         if not comparison.has_changes:
             return
 
         document = parse(toml_doc.as_string) if self.autofix else None
         yield from chain(
-            self.report(SharedViolations.DIFFERENT_VALUES, document, comparison.diff),
-            self.report(SharedViolations.MISSING_VALUES, document, comparison.missing),
+            self.report(SharedViolations.DIFFERENT_VALUES, document, cast(TomlDoc, comparison.diff)),
+            self.report(
+                SharedViolations.MISSING_VALUES,
+                document,
+                cast(TomlDoc, comparison.missing),
+                cast(TomlDoc, comparison.replace),
+            ),
         )
         if self.autofix and self.dirty:
             self.file_path.write_text(dumps(document))
 
-    def report(self, violation: ViolationEnum, document: TOMLDocument | None, change: BaseDoc | None):
+    def report(
+        self,
+        violation: ViolationEnum,
+        document: TOMLDocument | None,
+        change: TomlDoc | None,
+        replacement: TomlDoc | None = None,
+    ):
         """Report a violation while optionally modifying the TOML document."""
-        if not change:
+        if not (change or replacement):
             return
-        if document:
-            traverse_toml_tree(document, change.as_object)
+        if self.autofix:
+            real_change = cast(TomlDoc, replacement or change)
+            traverse_toml_tree(document, real_change.as_object)
             self.dirty = True
-        yield self.reporter.make_fuss(violation, change.reformatted.strip(), prefix="", fixed=self.autofix)
+
+        to_display = cast(TomlDoc, change or replacement)
+        yield self.reporter.make_fuss(violation, to_display.reformatted.strip(), prefix="", fixed=self.autofix)
 
     @property
     def initial_contents(self) -> str:
         """Suggest the initial content for this missing file."""
         return self.write_initial_contents(TomlDoc)
```

### Comparing `nitpick-0.33.1/src/nitpick/plugins/yaml.py` & `nitpick-0.33.2/src/nitpick/plugins/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """YAML files."""
 from __future__ import annotations
 
 from itertools import chain
-from typing import Iterator, cast
+from typing import TYPE_CHECKING, Iterator, cast
 
 from nitpick.blender import Comparison, YamlDoc, traverse_yaml_tree
 from nitpick.config import SpecialConfig
 from nitpick.constants import PRE_COMMIT_CONFIG_YAML
 from nitpick.exceptions import Deprecation
 from nitpick.plugins import hookimpl
 from nitpick.plugins.base import NitpickPlugin
-from nitpick.plugins.info import FileInfo
 from nitpick.plugins.text import KEY_CONTAINS
-from nitpick.typedefs import JsonDict, YamlObject
 from nitpick.violations import Fuss, SharedViolations, ViolationEnum
 
+if TYPE_CHECKING:
+    from nitpick.plugins.info import FileInfo
+    from nitpick.typedefs import JsonDict, YamlObject
+
 KEY_REPOS = "repos"
 KEY_YAML = "yaml"
 KEY_HOOKS = "hooks"
 KEY_REPO = "repo"
 KEY_ID = "id"
```

### Comparing `nitpick-0.33.1/src/nitpick/project.py` & `nitpick-0.33.2/src/nitpick/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """A project to be nitpicked."""
 from __future__ import annotations
 
 import itertools
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterable, Iterator
+from typing import TYPE_CHECKING, Iterable, Iterator
 
 import tomlkit
 from autorepr import autorepr
 from loguru import logger
 from marshmallow_polyfield import PolyField
 from more_itertools.more import always_iterable
 from pluggy import PluginManager
 from tomlkit.items import KeyType, SingleKey
-from tomlkit.toml_document import TOMLDocument
 
 from nitpick import fields, plugins
 from nitpick.blender import TomlDoc, search_json
 from nitpick.constants import (
     CONFIG_FILES,
     DOT_NITPICK_TOML,
     MANAGE_PY,
@@ -29,17 +28,21 @@
     ROOT_PYTHON_FILES,
     TOOL_NITPICK_JMEX,
     TOOL_NITPICK_KEY,
 )
 from nitpick.exceptions import QuitComplainingError
 from nitpick.generic import version_to_tuple
 from nitpick.schemas import BaseNitpickSchema, flatten_marshmallow_errors, help_message
-from nitpick.typedefs import JsonDict, PathOrStr
 from nitpick.violations import Fuss, ProjectViolations, Reporter, StyleViolations
 
+if TYPE_CHECKING:
+    from tomlkit.toml_document import TOMLDocument
+
+    from nitpick.typedefs import JsonDict, PathOrStr
+
 
 def glob_files(dir_: Path, file_patterns: Iterable[str]) -> set[Path]:
     """Search a directory looking for file patterns."""
     for pattern in file_patterns:
         found_files = set(dir_.glob(pattern))
         if found_files:
             return found_files
@@ -218,8 +221,8 @@
         tool_nitpick = tomlkit.table()
         tool_nitpick.add(tomlkit.comment("Generated by the 'nitpick init' command"))
         tool_nitpick.add(tomlkit.comment(f"More info at {READ_THE_DOCS_URL}configuration.html"))
         tool_nitpick.add("style", tomlkit.array([tomlkit.string(url) for url in style_urls]))
         doc.add(SingleKey(TOOL_NITPICK_KEY, KeyType.Bare), tool_nitpick)
 
         # config.file will always have a value at this point, but mypy can't see it.
-        config.file.write_text(tomlkit.dumps(doc, sort_keys=True))  # type: ignore
+        config.file.write_text(tomlkit.dumps(doc, sort_keys=True))
```

### Comparing `nitpick-0.33.1/src/nitpick/resources/any/codeclimate.toml` & `nitpick-0.33.2/src/nitpick/resources/any/codeclimate.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/any/editorconfig.toml` & `nitpick-0.33.2/src/nitpick/resources/any/editorconfig.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/any/pre-commit-hooks.toml` & `nitpick-0.33.2/src/nitpick/resources/any/pre-commit-hooks.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/presets/nitpick.toml` & `nitpick-0.33.2/src/nitpick/resources/presets/nitpick.toml`

 * *Files 19% similar despite different names*

```diff
@@ -7,38 +7,31 @@
 
 [nitpick.styles]
 include = [
     # Suggest the current stable Python version for projects
     "py://nitpick/resources/python/39",
 
     "py://nitpick/resources/python/absent",
-    "py://nitpick/resources/python/bandit",
     "py://nitpick/resources/python/black",
-    "py://nitpick/resources/python/flake8",
     "py://nitpick/resources/python/pre-commit-hooks",
-    "py://nitpick/resources/python/isort",
     "py://nitpick/resources/python/mypy",
     "py://nitpick/resources/python/poetry",
     "py://nitpick/resources/python/pylint",
     "py://nitpick/resources/python/radon",
     "py://nitpick/resources/python/readthedocs",
     "py://nitpick/resources/python/sonar-python",
     "py://nitpick/resources/python/tox",
     "py://nitpick/resources/python/github-workflow",
-    "py://nitpick/resources/python/autoflake",
 
     "py://nitpick/resources/any/prettier",
     "py://nitpick/resources/any/codeclimate",
     "py://nitpick/resources/any/commitizen",
     "py://nitpick/resources/any/editorconfig",
     "py://nitpick/resources/any/git-legal",
     "py://nitpick/resources/any/pre-commit-hooks",
     "py://nitpick/resources/any/markdownlint",
 
     "py://nitpick/resources/shell/bashate",
     "py://nitpick/resources/shell/shellcheck",
 
     "py://nitpick/resources/javascript/package-json",
 ]
-
-[nitpick.files."setup.cfg"]
-comma_separated_values = ["flake8.ignore", "flake8.exclude", "isort.skip", "isort.known_first_party"]
```

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/flake8.toml` & `nitpick-0.33.2/src/nitpick/resources/python/flake8.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/github-workflow.toml` & `nitpick-0.33.2/src/nitpick/resources/python/github-workflow.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [nitpick.meta]
 name = "GitHub Workflow for Python"
 url = "https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions"
 
 [".github/workflows/python.yaml"]
 name = "Python"
-on = ["push"]
+on = ["push", "pull_request"]
 
 [".github/workflows/python.yaml".jobs.build.strategy]
 fail-fast = false
 
 [".github/workflows/python.yaml".jobs.build.strategy.matrix]
 os = ["ubuntu-latest", "windows-latest", "macos-latest"]
 python-version = ["3.11", "3.10", "3.9", "3.8", "3.7"]
```

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/isort.toml` & `nitpick-0.33.2/src/nitpick/resources/python/isort.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/mypy.toml` & `nitpick-0.33.2/src/nitpick/resources/python/mypy.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/pylint.toml` & `nitpick-0.33.2/src/nitpick/resources/python/pylint.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/python/tox.toml` & `nitpick-0.33.2/src/nitpick/resources/python/tox.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/resources/shell/shellcheck.toml` & `nitpick-0.33.2/src/nitpick/resources/shell/shellcheck.toml`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/schemas.py` & `nitpick-0.33.2/src/nitpick/schemas.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/style/cache.py` & `nitpick-0.33.2/src/nitpick/style/cache.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/style/config.py` & `nitpick-0.33.2/src/nitpick/style/config.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/style/core.py` & `nitpick-0.33.2/src/nitpick/style/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Style files."""
 from __future__ import annotations
 
 from contextlib import suppress
 from dataclasses import dataclass, field
-from pathlib import Path
-from typing import Iterable, Iterator, Sequence, Set, Type
+from typing import TYPE_CHECKING, Iterable, Iterator, Sequence, Set, Type
 
-import dpath.util
 from flatten_dict import flatten, unflatten
 from furl import furl
 from identify import identify
 from loguru import logger
 from more_itertools import always_iterable
 from slugify import slugify
 from toml import TomlDecodeError
@@ -31,17 +29,30 @@
 from nitpick.plugins.base import NitpickPlugin
 from nitpick.plugins.info import FileInfo
 from nitpick.project import Project, glob_files
 from nitpick.schemas import BaseStyleSchema, flatten_marshmallow_errors
 from nitpick.style.config import ConfigValidator
 from nitpick.style.fetchers import Scheme, StyleFetcherManager
 from nitpick.style.fetchers.github import GitHubURL
-from nitpick.typedefs import JsonDict
 from nitpick.violations import Fuss, Reporter, StyleViolations
 
+try:
+    # DeprecationWarning: The dpath.util package is being deprecated.
+    # All util functions have been moved to dpath package top level.
+    from dpath import merge as dpath_merge
+except ImportError:
+    from dpath.util import merge as dpath_merge
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from nitpick.typedefs import JsonDict
+
+MAX_ATTEMPTS = 5
+
 Plugins = Set[Type[NitpickPlugin]]
 
 
 @dataclass()
 class StyleManager:  # pylint: disable=too-many-instance-attributes
     """Include styles recursively from one another."""
 
@@ -151,24 +162,23 @@
         toml_dict, validation_errors = self._config_validator.validate(read_toml_dict)
 
         if validation_errors:
             yield Reporter(FileInfo(self.project, display_name)).make_fuss(
                 StyleViolations.INVALID_CONFIG, flatten_marshmallow_errors(validation_errors)
             )
 
-        dpath.util.merge(self._merged_styles, flatten(toml_dict, custom_reducer(SEPARATOR_FLATTEN)))
+        dpath_merge(self._merged_styles, flatten(toml_dict, custom_reducer(SEPARATOR_FLATTEN)))
 
         yield from self.include_multiple_styles(sub_styles)
 
     def _read_toml(self, file_contents: str, display_name: str) -> JsonDict:
         toml = TomlDoc(string=file_contents)
         try:
             read_toml_dict = toml.as_object
-        # TODO: refactor: replace by this error when using tomlkit only in the future:
-        #  except TOMLKitError as err:
+        # TODO: refactor: replace by TOMLKitError when using tomlkit only in the future:
         except TomlDecodeError as err:
             # If the TOML itself could not be parsed, we can't go on
             raise QuitComplainingError(
                 Reporter(FileInfo(self.project, display_name)).make_fuss(
                     StyleViolations.INVALID_TOML, exception=pretty_exception(err)
                 )
             ) from err
@@ -178,15 +188,15 @@
         """Merge all included styles into a TOML (actually JSON) dictionary."""
         merged_dict = unflatten(self._merged_styles, custom_splitter(SEPARATOR_FLATTEN))
         # TODO: fix: check if the merged style file is still needed
         merged_style_path: Path = self.cache_dir / MERGED_STYLE_TOML
         toml = TomlDoc(obj=merged_dict)
 
         attempt = 1
-        while attempt < 5:
+        while attempt < MAX_ATTEMPTS:
             try:
                 merged_style_path.write_text(toml.reformatted)
                 break
             except OSError:
                 attempt += 1
 
         return merged_dict
@@ -228,15 +238,15 @@
             new_files_found.update(self.file_field_pair(subclass.filename, subclass))
 
         # Only recreate the schema if new fields were found.
         if new_files_found:
             self._dynamic_schema_class = type("DynamicStyleSchema", (self._dynamic_schema_class,), new_files_found)
 
     def _find_subclasses(self, data, handled_tags, new_files_found):
-        for possible_file in data.keys():
+        for possible_file in data:
             found_subclasses = []
             for file_tag in identify.tags_from_filename(possible_file):
                 handler_subclass = handled_tags.get(file_tag)
                 if handler_subclass:
                     found_subclasses.append(handler_subclass)
 
             for found_subclass in found_subclasses:
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/__init__.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Style fetchers with protocol support."""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import auto
-from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Iterator
 
-from furl import furl
 from requests_cache import CachedSession
 from strenum import LowercaseStrEnum
 
 from nitpick.enums import CachingEnum
 from nitpick.style import parse_cache_option
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
+    from furl import furl
+
     from nitpick.style.fetchers.base import StyleFetcher
 
 
 class Scheme(LowercaseStrEnum):
     """URL schemes."""
 
     FILE = auto()
@@ -90,15 +92,16 @@
         Try a fetcher by domain first, then by protocol scheme.
 
         """
         fetcher = self.fetchers.get(url.host) if url.host else None
         if not fetcher:
             fetcher = self.fetchers.get(url.scheme)
         if not fetcher:
-            raise RuntimeError(f"URL protocol {url.scheme!r} is not supported")
+            msg = f"URL protocol {url.scheme!r} is not supported"
+            raise RuntimeError(msg)
         return fetcher
 
 
 def _get_fetchers(session: CachedSession) -> dict[str, StyleFetcher]:
     # pylint: disable=import-outside-toplevel
     from nitpick.style.fetchers.file import FileFetcher
     from nitpick.style.fetchers.github import GitHubFetcher
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/base.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Base class for fetchers that wrap inner fetchers with caching ability."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import ClassVar
-
-from furl import furl
-from requests_cache import CachedSession
+from typing import TYPE_CHECKING, ClassVar
 
 from nitpick.constants import TOML_EXTENSION
 
+if TYPE_CHECKING:
+    from furl import furl
+    from requests_cache import CachedSession
+
 
 @dataclass(frozen=True)
 class StyleFetcher:
     """Base class of all fetchers, it encapsulates get/fetch from a specific source."""
 
     requires_connection: ClassVar[bool] = False
 
@@ -20,15 +21,16 @@
     session: CachedSession | None = None
     protocols: tuple[str, ...] = ()
     domains: tuple[str, ...] = ()
 
     def __post_init__(self):
         """Validate that session has been passed in for requires_connection == True."""
         if self.requires_connection and self.session is None:
-            raise ValueError("session is required")
+            msg = "session is required"
+            raise ValueError(msg)
 
     def preprocess_relative_url(self, url: str) -> str:  # pylint: disable=no-self-use
         """Preprocess a relative URL.
 
         Only called for urls that lack a scheme (at the very least), being resolved
         against a base URL that matches this specific fetcher.
 
@@ -58,8 +60,8 @@
         new_scheme = self._normalize_scheme(url.scheme)
         if new_scheme != url.scheme:
             url = url.copy().set(scheme=new_scheme)
         return self._normalize_url_path(url)
 
     def fetch(self, url: furl) -> str:
         """Fetch a style from a specific fetcher."""
-        raise NotImplementedError()
+        raise NotImplementedError
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/file.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from nitpick.style.fetchers.base import StyleFetcher
 
 
 @dataclass(frozen=True)
 class FileFetcher(StyleFetcher):  # pylint: disable=too-few-public-methods
     """Fetch a style from a local file."""
 
-    protocols: tuple[str, ...] = (Scheme.FILE,)  # type: ignore
+    protocols: tuple[str, ...] = (Scheme.FILE,)  # type: ignore[assignment]
 
     def preprocess_relative_url(self, url: str) -> str:
         """Preprocess a relative URL.
 
         Only called for urls that lack a scheme (at the very least), being resolved
         against a base URL that matches this specific fetcher.
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/github.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from nitpick.constants import GIT_AT_REFERENCE
 from nitpick.style.fetchers import Scheme
 from nitpick.style.fetchers.http import HttpFetcher
 
 GITHUB_COM = "github.com"
 API_GITHUB_COM = "api.github.com"
 RAW_GITHUB_COM = "raw.githubusercontent.com"
-QUERY_STRING_TOKEN = "token"  # nosec
+QUERY_STRING_TOKEN = "token"  # nosec # noqa: S105
 
 
 @dataclass(frozen=True)
 class GitHubURL:
     """Represent a GitHub URL, created from a URL or from its parts."""
 
     owner: str
@@ -29,16 +29,15 @@
     path: tuple[str, ...] = ()
     auth_token: str | None = None
     query_params: tuple[tuple[str, str], ...] | None = None
 
     @property
     def default_branch(self) -> str:
         """Default GitHub branch."""
-        # get_default_branch() is memoized
-        return get_default_branch(self.api_url.url, token=self.token)
+        return get_default_branch(self.api_url.url, token=self.token)  # function is memoized
 
     @property
     def token(self) -> str | None:
         """Token encoded in this URL.
 
         If present and it starts with a ``$``, it will be replaced with the
         value of the environment corresponding to the remaining part of the
@@ -99,15 +98,15 @@
             owner = url.host
             repo_with_git_reference, *path = url.path.segments
             repo, _, git_reference = repo_with_git_reference.partition(GIT_AT_REFERENCE)
         else:  # github.com URL (raw.githubusercontent.com is handled by the HTTP fetcher)
             # Skip the 'blob' component in the github.com URL.
             owner, repo, _, git_reference, *path = url.path.segments
 
-        if path and path[-1] == "":
+        if path and not path[-1]:
             # strip trailing slashes
             *path, _ = path
 
         return cls(owner, repo, git_reference, tuple(path), auth_token, query_params)
 
     @property
     def api_url(self) -> furl:
@@ -154,18 +153,18 @@
     return response.json()["default_branch"]
 
 
 @dataclass(frozen=True)
 class GitHubFetcher(HttpFetcher):  # pylint: disable=too-few-public-methods
     """Fetch styles from GitHub repositories."""
 
-    protocols: tuple[str, ...] = (Scheme.GH, Scheme.GITHUB)  # type: ignore
+    protocols: tuple[str, ...] = (Scheme.GH, Scheme.GITHUB)  # type: ignore[assignment,has-type]
     domains: tuple[str, ...] = (GITHUB_COM,)
 
     def _normalize_scheme(self, scheme: str) -> str:  # pylint: disable=no-self-use
         # Use github:// instead of gh:// in the canonical URL
-        return Scheme.GITHUB if scheme == Scheme.GH else scheme  # type: ignore
+        return Scheme.GITHUB if scheme == Scheme.GH else scheme  # type: ignore[return-value]
 
     def _download(self, url: furl, **kwargs) -> str:
         github_url = GitHubURL.from_furl(url)
         kwargs.setdefault("auth", github_url.credentials)
         return super()._download(github_url.raw_content_url, **kwargs)
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/http.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """Base HTTP fetcher, other fetchers can inherit from this to wrap http errors."""
 from __future__ import annotations
 
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 import click
 import requests
-from furl import furl
 from loguru import logger
 
 from nitpick.enums import OptionEnum
 from nitpick.style.fetchers import Scheme
 from nitpick.style.fetchers.base import StyleFetcher
 
+if TYPE_CHECKING:
+    from furl import furl
+
 
 @dataclass(frozen=True)
 class HttpFetcher(StyleFetcher):
     """Fetch a style from an http/https server."""
 
     requires_connection = True
 
-    protocols: tuple[str, ...] = (Scheme.HTTP, Scheme.HTTPS)  # type: ignore
+    protocols: tuple[str, ...] = (Scheme.HTTP, Scheme.HTTPS)  # type: ignore[has-type]
 
     def fetch(self, url: furl) -> str:
         """Fetch the style from a web location."""
         try:
             contents = self._download(url)
         except requests.ConnectionError as err:
             logger.exception(f"Request failed with {err}")
@@ -36,11 +39,12 @@
             )
             return ""
         return contents
 
     def _download(self, url: furl, **kwargs) -> str:
         logger.info(f"Downloading style from {url}")
         if self.session is None:
-            raise RuntimeError("No session provided to fetcher")
+            msg = "No session provided to fetcher"
+            raise RuntimeError(msg)
         response = self.session.get(url.url, **kwargs)
         response.raise_for_status()
         return response.text
```

### Comparing `nitpick-0.33.1/src/nitpick/style/fetchers/pypackage.py` & `nitpick-0.33.2/src/nitpick/style/fetchers/pypackage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Support for ``py`` schemes."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from functools import lru_cache
-from pathlib import Path
-from typing import Iterable, cast
+from typing import TYPE_CHECKING, Iterable, cast
 
 import attr
 import tomlkit
 from furl import furl
 
 from nitpick import PROJECT_NAME, compat
 from nitpick.constants import DOT
 from nitpick.style.fetchers import Scheme
 from nitpick.style.fetchers.base import StyleFetcher
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @lru_cache()
 def builtin_resources_root() -> Path:
     """Built-in resources root."""
     return compat.files("nitpick.resources")
 
 
@@ -45,42 +47,41 @@
         """Create an instance from a parsed URL in any accepted format.
 
         See the code for ``test_parsing_python_package_urls()`` for more examples.
 
         """
         package_name = url.host
         resource_path = url.path.segments
-        if resource_path and resource_path[-1] == "":
+        if resource_path and not resource_path[-1]:
             # strip trailing slash
             *resource_path, _ = resource_path
 
         *resource_path, resource_name = resource_path
         return cls(import_path=DOT.join([package_name, *resource_path]), resource_name=resource_name)
 
     @property
     def content_path(self) -> Path:
         """Raw path of resource file."""
         return compat.files(self.import_path) / self.resource_name
 
 
 @dataclass(frozen=True)
 class PythonPackageFetcher(StyleFetcher):  # pylint: disable=too-few-public-methods
-    """
-    Fetch a style from an installed Python package.
+    """Fetch a style from an installed Python package.
 
     URL schemes:
     - ``py://import/path/of/style/file/<style_file_name>``
     - ``pypackage://import/path/of/style/file/<style_file_name>``
 
     E.g. ``py://some_package/path/nitpick.toml``.
     """
 
-    protocols: tuple[str, ...] = (Scheme.PY, Scheme.PYPACKAGE)  # type: ignore
+    protocols: tuple[str, ...] = (Scheme.PY, Scheme.PYPACKAGE)  # type: ignore[assignment]
 
-    def _normalize_scheme(self, scheme: str) -> str:
+    def _normalize_scheme(self, scheme: str) -> str:  # noqa: ARG002
         # Always use the shorter py:// scheme name in the canonical URL.
         return cast(str, Scheme.PY)
 
     def fetch(self, url: furl) -> str:
         """Fetch the style from a Python package."""
         package_url = PythonPackageURL.from_furl(url)
         return package_url.content_path.read_text(encoding="UTF-8")
@@ -130,9 +131,10 @@
 
         try:
             # Intentionally break the doc generation when styles don't have [nitpick.meta]name
             meta = toml_dict["nitpick"]["meta"]
             bis.name = meta["name"]
             bis.url = meta.get("url")
         except KeyError as err:
-            raise SyntaxError(f"Style file missing [nitpick.meta] information: {bis}") from err
+            msg = f"Style file missing [nitpick.meta] information: {bis}"
+            raise SyntaxError(msg) from err
         return bis
```

### Comparing `nitpick-0.33.1/src/nitpick/typedefs.py` & `nitpick-0.33.2/src/nitpick/typedefs.py`

 * *Files identical despite different names*

### Comparing `nitpick-0.33.1/src/nitpick/violations.py` & `nitpick-0.33.2/src/nitpick/violations.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         """Suggestion with color."""
         return click.style(f"\n{self.suggestion.rstrip()}", fg="green") if self.suggestion else ""
 
     @property
     def pretty(self) -> str:
         """Message to be used on the CLI."""
         filename_plus_line = f"{self.filename}:{self.lineno}: " if self.filename.strip() else ""
-        return f"{filename_plus_line}{FLAKE8_PREFIX}{self.code:03}" f" {self.message.rstrip()}{self.colored_suggestion}"
+        return f"{filename_plus_line}{FLAKE8_PREFIX}{self.code:03} {self.message.rstrip()}{self.colored_suggestion}"
 
     def __lt__(self, other: Fuss) -> bool:
         """Sort Fuss instances."""
         return (self.filename, self.code, self.message, self.suggestion, self.lineno) < (
             other.filename,
             other.code,
             other.message,
@@ -109,18 +109,15 @@
 
     def __init__(self, info: FileInfo | None = None, violation_base_code: int = 0) -> None:
         self.info: FileInfo | None = info
         self.violation_base_code = violation_base_code
 
     def make_fuss(self, violation: ViolationEnum, suggestion: str = "", fixed=False, **kwargs) -> Fuss:
         """Make a fuss."""
-        if kwargs:
-            formatted = violation.message.format(**kwargs)
-        else:
-            formatted = violation.message
+        formatted = violation.message.format(**kwargs) if kwargs else violation.message
         base = self.violation_base_code if violation.add_code else 0
         Reporter.increment(fixed)
         # Remove right whitespace from suggestion (new lines, spaces, etc.)
         return Fuss(
             fixed, self.info.path_from_root if self.info else "", base + violation.code, formatted, suggestion.rstrip()
         )
```

### Comparing `nitpick-0.33.1/PKG-INFO` & `nitpick-0.33.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitpick
-Version: 0.33.1
+Version: 0.33.2
 Summary: Enforce the same settings across multiple language-independent projects
 Home-page: https://github.com/andreoliwa/nitpick
 License: MIT
 Keywords: python3,flake8,linter,styleguide
 Author: W. Augusto Andreoli
 Author-email: andreoliwa@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -446,15 +446,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you use `pre-commit <https://pre-commit.com/>`_ on your project, add
 this to the ``.pre-commit-config.yaml`` in your repository::
 
     repos:
       - repo: https://github.com/andreoliwa/nitpick
-        rev: v0.33.1
+        rev: v0.33.2
         hooks:
           - id: nitpick
 
 There are 3 available hook IDs:
 
 - ``nitpick`` and ``nitpick-fix`` both run the ``nitpick fix`` command;
 - ``nitpick-check`` runs ``nitpick check``.
@@ -472,15 +472,15 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you use `MegaLinter <https://megalinter.github.io/>`_ you can run Nitpick as a plugin. Add the following two entries to your ``.mega-linter.yml`` configuration file:
 
 .. code-block:: yaml
 
     PLUGINS:
-      - https://raw.githubusercontent.com/andreoliwa/nitpick/v0.33.1/mega-linter-plugin-nitpick/nitpick.megalinter-descriptor.yml
+      - https://raw.githubusercontent.com/andreoliwa/nitpick/v0.33.2/mega-linter-plugin-nitpick/nitpick.megalinter-descriptor.yml
     ENABLE_LINTERS:
       - NITPICK
 
 
 More information
 ----------------
```


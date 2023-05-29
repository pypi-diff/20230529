# Comparing `tmp/poetry_plugin_export-1.3.1.tar.gz` & `tmp/poetry_plugin_export-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_export-1.3.1.tar", max compression
+gzip compressed data, was "poetry_plugin_export-1.4.0.tar", max compression
```

## Comparing `poetry_plugin_export-1.3.1.tar` & `poetry_plugin_export-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1062 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/LICENSE
--rw-r--r--   0        0        0     1800 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/README.md
--rw-r--r--   0        0        0     2035 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      168 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/__init__.py
--rw-r--r--   0        0        0     3678 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/command.py
--rw-r--r--   0        0        0     7264 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/exporter.py
--rw-r--r--   0        0        0      957 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/plugins.py
--rw-r--r--   0        0        0     9933 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/src/poetry_plugin_export/walker.py
--rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/__init__.py
--rw-r--r--   0        0        0     2549 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/conftest.py
--rw-r--r--   0        0        0     7819 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/command/test_command_export.py
--rw-r--r--   0        0        0     5325 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1116 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      961 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0      264 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 14:40:05.811764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0       22 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1495 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1106 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
--rw-r--r--   0        0        0     1320 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0      771 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     3174 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/helpers.py
--rw-r--r--   0        0        0     1262 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/markers.py
--rw-r--r--   0        0        0    84039 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/test_exporter.py
--rw-r--r--   0        0        0      995 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/test_walker.py
--rw-r--r--   0        0        0     1010 2023-04-17 14:40:05.815764 poetry_plugin_export-1.3.1/tests/types.py
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 poetry_plugin_export-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1800 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/README.md
+-rw-r--r--   0        0        0     2719 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/src/poetry_plugin_export/__init__.py
+-rw-r--r--   0        0        0     3678 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/src/poetry_plugin_export/command.py
+-rw-r--r--   0        0        0     7268 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/src/poetry_plugin_export/exporter.py
+-rw-r--r--   0        0        0      957 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/src/poetry_plugin_export/plugins.py
+-rw-r--r--   0        0        0     9933 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/src/poetry_plugin_export/walker.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/tests/command/__init__.py
+-rw-r--r--   0        0        0     2549 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/tests/command/conftest.py
+-rw-r--r--   0        0        0     7819 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/tests/command/test_command_export.py
+-rw-r--r--   0        0        0     5325 2023-05-29 08:49:08.978796 poetry_plugin_export-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1116 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      961 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0      264 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0       22 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1495 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1106 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
+-rw-r--r--   0        0        0     1320 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      771 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     3174 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/helpers.py
+-rw-r--r--   0        0        0     1262 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/markers.py
+-rw-r--r--   0        0        0    85429 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/test_exporter.py
+-rw-r--r--   0        0        0      995 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/test_walker.py
+-rw-r--r--   0        0        0      994 2023-05-29 08:49:08.982796 poetry_plugin_export-1.4.0/tests/types.py
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 poetry_plugin_export-1.4.0/PKG-INFO
```

### Comparing `poetry_plugin_export-1.3.1/LICENSE` & `poetry_plugin_export-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/README.md` & `poetry_plugin_export-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/pyproject.toml` & `poetry_plugin_export-1.4.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-export"
-version = "1.3.1"
+version = "1.4.0"
 description = "Poetry plugin to export the dependencies to various formats"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://python-poetry.org/"
 repository = "https://github.com/python-poetry/poetry-plugin-export"
 
@@ -14,16 +14,16 @@
 
 include = [
     { path = "tests", format = "sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = "^1.3.0"
-poetry-core = "^1.3.0"
+poetry = "^1.5.0"
+poetry-core = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.18"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 pytest-mock = "^3.9"
 pytest-randomly = "^3.12"
@@ -35,27 +35,57 @@
 optional = true
 [tool.poetry.group.github-actions.dependencies]
 pytest-github-actions-annotate-failures = "^0.1.7"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 export = "poetry_plugin_export.plugins:ExportApplicationPlugin"
 
+
+[tool.ruff]
+fix = true
+unfixable = [
+    "ERA", # do not autoremove commented out code
+]
+target-version = "py37"
+line-length = 88
+extend-select = [
+    "B",   # flake8-bugbear
+    "C4",  # flake8-comprehensions
+    "ERA", # flake8-eradicate/eradicate
+    "I",   # isort
+    "N",   # pep8-naming
+    "PIE", # flake8-pie
+    "PGH", # pygrep
+    "RUF", # ruff checks
+    "SIM", # flake8-simplify
+    "TCH", # flake8-type-checking
+    "TID", # flake8-tidy-imports
+    "UP",  # pyupgrade
+]
+extend-exclude = [
+    "docs/*",
+    # External to the project's coding standards
+    "tests/**/fixtures/*",
+]
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.isort]
+force-single-line = true
+lines-between-types = 1
+lines-after-imports = 2
+known-first-party = ["poetry_plugin_export"]
+required-imports = ["from __future__ import annotations"]
+
+
 [tool.black]
 target-version = ['py37']
 preview = true
 
-[tool.isort]
-profile = "black"
-force_single_line = true
-atomic = true
-include_trailing_comma = true
-lines_after_imports = 2
-lines_between_types = 1
-use_parentheses = true
-
 [tool.mypy]
 namespace_packages = true
 show_error_codes = true
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
```

### Comparing `poetry_plugin_export-1.3.1/src/poetry_plugin_export/command.py` & `poetry_plugin_export-1.4.0/src/poetry_plugin_export/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/src/poetry_plugin_export/exporter.py` & `poetry_plugin_export-1.4.0/src/poetry_plugin_export/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
         if indexes and self._with_urls:
             # If we have extra indexes, we add them to the beginning of the output
             indexes_header = ""
             for index in sorted(indexes):
                 repositories = [
                     r
-                    for r in self._poetry.pool.repositories
+                    for r in self._poetry.pool.all_repositories
                     if isinstance(r, HTTPRepository) and r.url == index.rstrip("/")
                 ]
                 if not repositories:
                     continue
                 repository = repositories[0]
                 if (
                     self._poetry.pool.has_default()
```

### Comparing `poetry_plugin_export-1.3.1/src/poetry_plugin_export/plugins.py` & `poetry_plugin_export-1.4.0/src/poetry_plugin_export/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/src/poetry_plugin_export/walker.py` & `poetry_plugin_export-1.4.0/src/poetry_plugin_export/walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/command/conftest.py` & `poetry_plugin_export-1.4.0/tests/command/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/command/test_command_export.py` & `poetry_plugin_export-1.4.0/tests/command/test_command_export.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/conftest.py` & `poetry_plugin_export-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry_plugin_export-1.4.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry_plugin_export-1.4.0/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/sample_project/pyproject.toml` & `poetry_plugin_export-1.4.0/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz` & `poetry_plugin_export-1.4.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry_plugin_export-1.4.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/fixtures/simple_project/pyproject.toml` & `poetry_plugin_export-1.4.0/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/helpers.py` & `poetry_plugin_export-1.4.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/markers.py` & `poetry_plugin_export-1.4.0/tests/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/test_exporter.py` & `poetry_plugin_export-1.4.0/tests/test_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from cleo.io.null_io import NullIO
 from poetry.core.packages.dependency import Dependency
 from poetry.core.packages.dependency_group import MAIN_GROUP
 from poetry.core.version.markers import parse_marker
 from poetry.factory import Factory
 from poetry.packages import Locker as BaseLocker
 from poetry.repositories.legacy_repository import LegacyRepository
+from poetry.repositories.repository_pool import Priority
 
 from poetry_plugin_export.exporter import Exporter
 from tests.markers import MARKER_CPYTHON
 from tests.markers import MARKER_DARWIN
 from tests.markers import MARKER_LINUX
 from tests.markers import MARKER_PY
 from tests.markers import MARKER_PY27
@@ -1803,23 +1804,23 @@
     )
     poetry.pool.add_repository(
         LegacyRepository(
             "custom-b",
             "https://b.example.com/simple",
             config=poetry.config,
         ),
-        default=True,
+        priority=Priority.DEFAULT,
     )
     poetry.pool.add_repository(
         LegacyRepository(
             "custom-a",
             "https://a.example.com/simple",
             config=poetry.config,
         ),
-        secondary=True,
+        priority=Priority.SECONDARY,
     )
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
@@ -2095,35 +2096,25 @@
     poetry._package = root
 
     exporter = Exporter(poetry, NullIO())
     exporter.only_groups([MAIN_GROUP, "dev"])
     io = BufferedIO()
     exporter.export("requirements.txt", tmp_path, io)
 
-    expected_legacy = f"""\
-celery==5.1.2 ; {MARKER_PY36_ONLY}
-celery==5.2.3 ; {MARKER_PY37}
-click-didyoumean==0.0.3 ; {MARKER_PY36_PY362}
-click-didyoumean==0.3.0 ; {MARKER_PY362_PY40}
-click-plugins==1.1.1 ; {MARKER_PY36}
-click==7.1.2 ; python_version < "3.7" and python_version >= "3.6"
-click==8.0.3 ; {MARKER_PY37}
-"""
-
     expected = f"""\
 celery==5.1.2 ; {MARKER_PY36_ONLY}
 celery==5.2.3 ; {MARKER_PY37}
 click-didyoumean==0.0.3 ; {MARKER_PY36_PY362}
 click-didyoumean==0.3.0 ; {MARKER_PY362_PY40}
 click-plugins==1.1.1 ; {MARKER_PY36}
 click==7.1.2 ; {MARKER_PY36_ONLY}
 click==8.0.3 ; {MARKER_PY37}
 """
 
-    assert io.fetch_output() in {expected, expected_legacy}
+    assert io.fetch_output() == expected
 
 
 def test_exporter_handles_extras_next_to_non_extras(
     tmp_path: Path, poetry: Poetry
 ) -> None:
     # Testcase similar to the solver testcase added at #5305.
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
@@ -2668,7 +2659,64 @@
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
     expected = f"""\
 foo[baz]==1.2.3 ; {MARKER_PY27} or {MARKER_PY36}
 """
     assert content == expected
+
+
+def test_exporter_exports_extra_index_url_and_trusted_host(
+    tmp_path: Path, poetry: Poetry
+) -> None:
+    poetry.pool.add_repository(
+        LegacyRepository(
+            "custom",
+            "http://example.com/simple",
+        ),
+        priority=Priority.EXPLICIT,
+    )
+    poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
+        {
+            "package": [
+                {
+                    "name": "foo",
+                    "version": "1.2.3",
+                    "optional": False,
+                    "python-versions": "*",
+                    "dependencies": {"bar": "*"},
+                },
+                {
+                    "name": "bar",
+                    "version": "4.5.6",
+                    "optional": False,
+                    "python-versions": "*",
+                    "source": {
+                        "type": "legacy",
+                        "url": "http://example.com/simple",
+                        "reference": "",
+                    },
+                },
+            ],
+            "metadata": {
+                "python-versions": "*",
+                "content-hash": "123456789",
+                "files": {"foo": [], "bar": []},
+            },
+        }
+    )
+    set_package_requires(poetry)
+
+    exporter = Exporter(poetry, NullIO())
+    exporter.export("requirements.txt", tmp_path, "requirements.txt")
+
+    with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
+        content = f.read()
+
+    expected = f"""\
+--trusted-host example.com
+--extra-index-url http://example.com/simple
+
+bar==4.5.6 ; {MARKER_PY}
+foo==1.2.3 ; {MARKER_PY}
+"""
+    assert content == expected
```

### Comparing `poetry_plugin_export-1.3.1/tests/test_walker.py` & `poetry_plugin_export-1.4.0/tests/test_walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.3.1/tests/types.py` & `poetry_plugin_export-1.4.0/tests/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
-from typing import Protocol  # noqa: TYP001
+from typing import Protocol
 
 
 if TYPE_CHECKING:
     from cleo.testers.command_tester import CommandTester
     from poetry.installation import Installer
     from poetry.installation.executor import Executor
     from poetry.poetry import Poetry
```

### Comparing `poetry_plugin_export-1.3.1/PKG-INFO` & `poetry_plugin_export-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-export
-Version: 1.3.1
+Version: 1.4.0
 Summary: Poetry plugin to export the dependencies to various formats
 Home-page: https://python-poetry.org/
 License: MIT
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.3.0,<2.0.0)
-Requires-Dist: poetry-core (>=1.3.0,<2.0.0)
+Requires-Dist: poetry (>=1.5.0,<2.0.0)
+Requires-Dist: poetry-core (>=1.6.0,<2.0.0)
 Project-URL: Repository, https://github.com/python-poetry/poetry-plugin-export
 Description-Content-Type: text/markdown
 
 # Poetry Plugin: Export
 
 This package is a plugin that allows the export of locked packages to various formats.
```


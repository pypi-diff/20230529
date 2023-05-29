# Comparing `tmp/poetry_plugin_bundle-1.2.0.tar.gz` & `tmp/poetry_plugin_bundle-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_bundle-1.2.0.tar", max compression
+gzip compressed data, was "poetry_plugin_bundle-1.3.0.tar", max compression
```

## Comparing `poetry_plugin_bundle-1.2.0.tar` & `poetry_plugin_bundle-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2101 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/README.md
--rw-r--r--   0        0        0     1494 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/__init__.py
--rw-r--r--   0        0        0      278 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/bundler.py
--rw-r--r--   0        0        0     1232 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/bundler_manager.py
--rw-r--r--   0        0        0     8140 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/venv_bundler.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/bundle/__init__.py
--rw-r--r--   0        0        0     1217 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/bundle/bundle_command.py
--rw-r--r--   0        0        0     1447 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/bundle/venv.py
--rw-r--r--   0        0        0       84 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/exceptions.py
--rw-r--r--   0        0        0     1597 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/plugin.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/bundlers/__init__.py
--rw-r--r--   0        0        0     1381 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/bundlers/test_bundler_manager.py
--rw-r--r--   0        0        0    10024 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/bundlers/test_venv_bundler.py
--rw-r--r--   0        0        0     1794 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/console/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/console/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/console/commands/bundle/__init__.py
--rw-r--r--   0        0        0     2464 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/console/commands/bundle/test_venv.py
--rw-r--r--   0        0        0      962 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/console/conftest.py
--rw-r--r--   0        0        0       22 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0      271 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project/poetry.lock
--rw-r--r--   0        0        0      669 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_dev_dep/README.rst
--rw-r--r--   0        0        0      271 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_dev_dep/poetry.lock
--rw-r--r--   0        0        0      716 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_dev_dep/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_dev_dep/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_no_module/README.rst
--rw-r--r--   0        0        0      271 2023-03-19 14:30:30.640323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_no_module/poetry.lock
--rw-r--r--   0        0        0      669 2023-03-19 14:30:30.644323 poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_no_module/pyproject.toml
--rw-r--r--   0        0        0     1713 2023-03-19 14:30:30.644323 poetry_plugin_bundle-1.2.0/tests/helpers.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 poetry_plugin_bundle-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2101 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/README.md
+-rw-r--r--   0        0        0     2189 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/bundler.py
+-rw-r--r--   0        0        0     1232 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/bundler_manager.py
+-rw-r--r--   0        0        0     7910 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/venv_bundler.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.332027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/bundle/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/bundle/bundle_command.py
+-rw-r--r--   0        0        0     1447 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/bundle/venv.py
+-rw-r--r--   0        0        0       84 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/exceptions.py
+-rw-r--r--   0        0        0     1597 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/bundlers/__init__.py
+-rw-r--r--   0        0        0     1381 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/bundlers/test_bundler_manager.py
+-rw-r--r--   0        0        0    10024 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/bundlers/test_venv_bundler.py
+-rw-r--r--   0        0        0     1789 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/console/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/console/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/console/commands/bundle/__init__.py
+-rw-r--r--   0        0        0     2464 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/console/commands/bundle/test_venv.py
+-rw-r--r--   0        0        0      962 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/console/conftest.py
+-rw-r--r--   0        0        0       22 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0      271 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project/poetry.lock
+-rw-r--r--   0        0        0      728 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_dev_dep/README.rst
+-rw-r--r--   0        0        0      271 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_dev_dep/poetry.lock
+-rw-r--r--   0        0        0      716 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_dev_dep/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_dev_dep/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_no_module/README.rst
+-rw-r--r--   0        0        0      271 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_no_module/poetry.lock
+-rw-r--r--   0        0        0      669 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_no_module/pyproject.toml
+-rw-r--r--   0        0        0     1707 2023-05-29 20:34:29.336027 poetry_plugin_bundle-1.3.0/tests/helpers.py
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 poetry_plugin_bundle-1.3.0/PKG-INFO
```

### Comparing `poetry_plugin_bundle-1.2.0/README.md` & `poetry_plugin_bundle-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/bundler_manager.py` & `poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/bundler_manager.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/bundlers/venv_bundler.py` & `poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/bundlers/venv_bundler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import subprocess
 import sys
 
+from pathlib import Path
 from subprocess import CalledProcessError
 from typing import TYPE_CHECKING
 
 from poetry_plugin_bundle.bundlers.bundler import Bundler
 
 
 if TYPE_CHECKING:
-    from pathlib import Path
-
     from cleo.io.io import IO
     from cleo.io.outputs.section_output import SectionOutput
     from poetry.core.constraints.version import Version
     from poetry.poetry import Poetry
 
 
 class VenvBundler(Bundler):
@@ -28,15 +27,15 @@
         self._activated_groups: set[str] | None = None
 
     def set_path(self, path: Path) -> VenvBundler:
         self._path = path
 
         return self
 
-    def set_executable(self, executable: str) -> VenvBundler:
+    def set_executable(self, executable: str | None) -> VenvBundler:
         self._executable = executable
 
         return self
 
     def set_activated_groups(self, activated_groups: set[str]) -> VenvBundler:
         self._activated_groups = activated_groups
 
@@ -61,18 +60,18 @@
         from poetry.utils.env import EnvManager
         from poetry.utils.env import SystemEnv
         from poetry.utils.env import VirtualEnv
 
         warnings = []
 
         manager = EnvManager(poetry)
-        executable = self._executable
-        if self._executable is not None:
+        if self._executable:
             executable, python_version = self._get_executable_info(self._executable)
         else:
+            executable = None
             version_info = SystemEnv(Path(sys.prefix)).get_version_info()
             python_version = Version.parse(".".join(str(v) for v in version_info[:3]))
 
         message = self._get_message(poetry, self._path)
         if io.is_decorated() and not io.is_debug():
             io = io.section()  # type: ignore[assignment]
 
@@ -89,39 +88,39 @@
                 or env_python_version != python_version
                 or self._remove
             ):
                 self._write(
                     io, f"{message}: <info>Removing existing virtual environment</info>"
                 )
 
-                manager.remove_venv(str(self._path))
+                manager.remove_venv(self._path)
 
                 self._write(
                     io,
                     (
                         f"{message}: <info>Creating a virtual environment using Python"
                         f" <b>{python_version}</b></info>"
                     ),
                 )
 
-                manager.build_venv(str(self._path), executable=executable)
+                manager.build_venv(self._path, executable=executable)
             else:
                 self._write(
                     io, f"{message}: <info>Using existing virtual environment</info>"
                 )
         else:
             self._write(
                 io,
                 (
                     f"{message}: <info>Creating a virtual environment using Python"
                     f" <b>{python_version}</b></info>"
                 ),
             )
 
-            manager.build_venv(str(self._path), executable=executable)
+            manager.build_venv(self._path, executable=executable)
 
         env = VirtualEnv(self._path)
 
         self._write(io, f"{message}: <info>Installing dependencies</info>")
 
         installer = Installer(
             NullIO() if not io.is_debug() else io,
@@ -130,18 +129,14 @@
             poetry.locker,
             poetry.pool,
             poetry.config,
         )
         if self._activated_groups is not None:
             installer.only_groups(self._activated_groups)
         installer.requires_synchronization()
-        use_executor = poetry.config.get("experimental.new-installer", False)
-        if not use_executor:
-            # only set if false because the method is deprecated
-            installer.use_executor(False)
 
         return_code = installer.run()
         if return_code:
             self._write(
                 io,
                 self._get_message(poetry, self._path, error=True)
                 + ": <error>Failed</> at step <b>Installing dependencies</b>",
@@ -210,15 +205,15 @@
 
         if io.is_debug() or not io.is_decorated() or not isinstance(io, SectionOutput):
             io.write_line(message)
             return
 
         io.overwrite(message)
 
-    def _get_executable_info(self, executable: str) -> tuple[str, Version]:
+    def _get_executable_info(self, executable: str) -> tuple[Path, Version]:
         from poetry.core.constraints.version import Version
 
         try:
             python_version = Version.parse(executable)
             executable = f"python{python_version.major}"
             if python_version.precision > 1:
                 executable += f".{python_version.minor}"
@@ -236,12 +231,12 @@
                         " sys.version_info[:3]]))"
                     ),
                 ]
             ).decode()
         except CalledProcessError as e:
             from poetry.utils.env import EnvCommandError
 
-            raise EnvCommandError(e)
+            raise EnvCommandError(e) from None
 
         python_version = Version.parse(python_version_str.strip())
 
-        return executable, python_version
+        return Path(executable), python_version
```

### Comparing `poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/bundle/bundle_command.py` & `poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/bundle/bundle_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     def set_bundler_manager(self, bundler_manager: BundlerManager) -> None:
         self._bundler_manager = bundler_manager
 
     def configure_bundler(self, bundler: Bundler) -> None:
         """
         Configure the given bundler based on command specific options and arguments.
         """
-        pass
 
     def handle(self) -> int:
         self.line("")
 
         assert self._bundler_manager is not None
         bundler = self._bundler_manager.bundler(self.bundler_name)
```

### Comparing `poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/console/commands/bundle/venv.py` & `poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/console/commands/bundle/venv.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/src/poetry_plugin_bundle/plugin.py` & `poetry_plugin_bundle-1.3.0/src/poetry_plugin_bundle/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/bundlers/test_bundler_manager.py` & `poetry_plugin_bundle-1.3.0/tests/bundlers/test_bundler_manager.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/bundlers/test_venv_bundler.py` & `poetry_plugin_bundle-1.3.0/tests/bundlers/test_venv_bundler.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/conftest.py` & `poetry_plugin_bundle-1.3.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,13 +69,13 @@
     return c
 
 
 @pytest.fixture
 def tmp_venv(tmp_path: Path) -> Iterator[VirtualEnv]:
     venv_path = tmp_path / "venv"
 
-    EnvManager.build_venv(str(venv_path))
+    EnvManager.build_venv(venv_path)
 
     venv = VirtualEnv(venv_path)
     yield venv
 
     shutil.rmtree(str(venv.path))
```

### Comparing `poetry_plugin_bundle-1.2.0/tests/console/commands/bundle/test_venv.py` & `poetry_plugin_bundle-1.3.0/tests/console/commands/bundle/test_venv.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/console/conftest.py` & `poetry_plugin_bundle-1.3.0/tests/console/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project/pyproject.toml` & `poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_no_module/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_dev_dep/pyproject.toml` & `poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project_with_dev_dep/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_bundle-1.2.0/tests/fixtures/simple_project_with_no_module/pyproject.toml` & `poetry_plugin_bundle-1.3.0/tests/fixtures/simple_project/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,14 @@
 ]
 
 # Requirements
 [tool.poetry.dependencies]
 python = "~2.7 || ^3.4"
 foo = "^1.0.0"
 
+[tool.poetry.group.dev]
+optional = true
+dependencies = {}
+
 [tool.poetry.scripts]
 foo = "foo:bar"
 baz = "bar:baz.boom.bim"
```

### Comparing `poetry_plugin_bundle-1.2.0/tests/helpers.py` & `poetry_plugin_bundle-1.3.0/tests/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self._poetry.set_config(poetry.config)
         self._poetry.set_locker(
             TestLocker(poetry.locker.lock, self._poetry.local_config)
         )
 
 
 class TestLocker(Locker):
-    def __init__(self, lock: str | Path, local_config: dict[str, Any]) -> None:
+    def __init__(self, lock: Path, local_config: dict[str, Any]) -> None:
         super().__init__(lock, local_config)
         self._locked = False
         self._write = False
 
     def write(self, write: bool = True) -> None:
         self._write = write
```

### Comparing `poetry_plugin_bundle-1.2.0/PKG-INFO` & `poetry_plugin_bundle-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-bundle
-Version: 1.2.0
+Version: 1.3.0
 Summary: Poetry plugin to bundle projects into various formats
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
-Requires-Dist: poetry (>=1.4.0,<2.0.0)
+Requires-Dist: poetry (>=1.5.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Poetry Plugin: Bundle
 
 This package is a plugin that allows the bundling of Poetry projects into various formats.
 
 ## Installation
```


# Comparing `tmp/hatch_build_scripts-0.0.1.tar.gz` & `tmp/hatch_build_scripts-0.0.2.tar.gz`

## Comparing `hatch_build_scripts-0.0.1.tar` & `hatch_build_scripts-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/hatch_build_scripts/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/hatch_build_scripts/hooks.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/hatch_build_scripts/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/tests/test_plugin.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/tests/utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/LICENSE
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/README.md
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/435c9e25cb5ee1fb
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/4586f2c83492ef12
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/63153e74ae9448e3
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/74fc00111a6357de
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/c7e9480ae051d10c
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/fc26102941cba458
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/hooks.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/test_plugin.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/PKG-INFO
```

### Comparing `hatch_build_scripts-0.0.1/tests/utils.py` & `hatch_build_scripts-0.0.2/tests/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
-from pathlib import Path
 import subprocess
 import sys
-from typing import Sequence, Iterator
-import toml
 import zipfile
-from dataclasses import asdict
 from contextlib import contextmanager
+from dataclasses import asdict
+from pathlib import Path
+from typing import Iterator, Sequence
 
-import hatch_build_scripts
-from hatch_build_scripts.plugin import ScriptConfig
+import toml
 
+import hatch_build_scripts
+from hatch_build_scripts.plugin import OneScriptConfig
 
 ROOT_DIR = Path(__file__).parent.parent
 
 
-def create_project(path: Path | str, scripts: Sequence[ScriptConfig]) -> FakeProject:
+def create_project(path: Path | str, scripts: Sequence[OneScriptConfig]) -> FakeProject:
     path = Path(path)
 
     full_config = {
         "project": {
             "name": "test-project",
             "version": "0.0.0",
             "description": "A test project",
@@ -49,17 +49,28 @@
 
 class FakeProject:
     def __init__(self, path: Path) -> None:
         self.path = path
 
     def build(self) -> None:
         subprocess.run(
-            [sys.executable, "-m", "pip", "cache", "remove", hatch_build_scripts.__name__], cwd=self.path, check=True
+            [  # noqa: S603
+                sys.executable,
+                "-m",
+                "pip",
+                "cache",
+                "remove",
+                hatch_build_scripts.__name__,
+            ],
+            cwd=self.path,
+            check=True,
+        )
+        subprocess.run(
+            [sys.executable, "-m", "hatch", "build"], cwd=self.path, check=True  # noqa: S603
         )
-        subprocess.run([sys.executable, "-m", "hatch", "build"], cwd=self.path, check=True)
 
     @contextmanager
     def dist(self) -> Iterator[zipfile.ZipFile]:
         files = list((self.path / "dist").glob("*.whl"))
         assert len(files) == 1
         with zipfile.ZipFile(str(files[0])) as whl:
             yield whl
```

### Comparing `hatch_build_scripts-0.0.1/.gitignore` & `hatch_build_scripts-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.1/LICENSE` & `hatch_build_scripts-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.1/pyproject.toml` & `hatch_build_scripts-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["pathspec", "hatchling"]
 
 [project.urls]
-Documentation = "https://github.com/unknown/hatch-build-scripts#readme"
-Issues = "https://github.com/unknown/hatch-build-scripts/issues"
-Source = "https://github.com/unknown/hatch-build-scripts"
+Documentation = "https://github.com/rmorshea/hatch-build-scripts#readme"
+Issues = "https://github.com/rmorshea/hatch-build-scripts/issues"
+Source = "https://github.com/rmorshea/hatch-build-scripts"
 
 [tool.hatch.version]
 path = "hatch_build_scripts/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
@@ -77,20 +77,20 @@
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
 target-version = ["py37"]
-line-length = 120
+line-length = 100
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py37"
-line-length = 120
+line-length = 100
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
```


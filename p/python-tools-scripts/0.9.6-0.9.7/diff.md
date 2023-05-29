# Comparing `tmp/python-tools-scripts-0.9.6.tar.gz` & `tmp/python-tools-scripts-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jan 23 12:51:01 2023, max compression
+gzip compressed data, last modified: Wed Jan 25 07:01:57 2023, max compression
```

## Comparing `python-tools-scripts-0.9.6.tar` & `python-tools-scripts-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0 root         (0) root         (0)     1888 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3848 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/.pre-commit-hooks.yaml
--rw-r--r--   0 root         (0) root         (0)     2743 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3494 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2368 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/changelog/.gitkeep
--rw-r--r--   0 root         (0) root         (0)     6192 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      144 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/lint.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     2288 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      111 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/
--rw-r--r--   0 root         (0) root         (0)      178 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3708 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/logs.py
--rw-r--r--   0 root         (0) root         (0)    15430 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/parser.py
--rw-r--r--   0 root         (0) root         (0)     8641 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/process.py
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/ptscripts/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3494 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      275 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-23 12:51:01.000000 python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3848 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      156 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/.pre-commit-hooks.yaml
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/changelog/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/
+-rw-r--r--   0 root         (0) root         (0)       11 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/lint.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      111 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      592 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/logs.py
+-rw-r--r--   0 root         (0) root         (0)    15470 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/parser.py
+-rw-r--r--   0 root         (0) root         (0)     8679 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/process.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/ptscripts/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      275 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-01-25 07:01:57.000000 python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/top_level.txt
```

### Comparing `python-tools-scripts-0.9.6/.gitignore` & `python-tools-scripts-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/.pre-commit-config.yaml` & `python-tools-scripts-0.9.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/CHANGELOG.rst` & `python-tools-scripts-0.9.7/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 Backward incompatible (breaking) changes will only be introduced in major versions with advance notice in the
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
+0.9.7 (2023-01-25)
+==================
+
+Features
+--------
+
+- Forward `ctx.run(..., **kwargs)` to the underlying subprocess call. (`#14 <https://github.com/s0undt3ch/python-tools-scripts/issues/14>`_)
+
+
 0.9.6 (2023-01-23)
 ==================
 
 Bug Fixes
 ---------
 
 - Cleanup conflicting parser CLI options (`#12 <https://github.com/s0undt3ch/python-tools-scripts/issues/12>`_)
```

### Comparing `python-tools-scripts-0.9.6/LICENSE` & `python-tools-scripts-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/PKG-INFO` & `python-tools-scripts-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tools-scripts
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python Tools Scripts
 Home-page: https://github.com/s0undt3ch/python-tools-scripts
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/s0undt3ch/python-tools-scripts
 Project-URL: Tracker, https://github.com/s0undt3ch/python-tools-scripts/issues
```

### Comparing `python-tools-scripts-0.9.6/README.md` & `python-tools-scripts-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/noxfile.py` & `python-tools-scripts-0.9.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/pyproject.toml` & `python-tools-scripts-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/setup.cfg` & `python-tools-scripts-0.9.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/src/ptscripts/__main__.py` & `python-tools-scripts-0.9.7/src/ptscripts/__main__.py`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/src/ptscripts/logs.py` & `python-tools-scripts-0.9.7/src/ptscripts/logs.py`

 * *Files identical despite different names*

### Comparing `python-tools-scripts-0.9.6/src/ptscripts/parser.py` & `python-tools-scripts-0.9.7/src/ptscripts/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,25 +145,27 @@
         self,
         *cmdline,
         check=True,
         timeout_secs: int | None = None,
         no_output_timeout_secs: int | None = None,
         capture: bool = False,
         interactive: bool = False,
+        **kwargs,
     ) -> CompletedProcess[str]:
         """
         Run a subprocess.
         """
         return process.run(
             *cmdline,
             check=check,
             timeout_secs=timeout_secs,
             no_output_timeout_secs=no_output_timeout_secs,
             capture=capture,
             interactive=interactive,
+            **kwargs,
         )
 
     @contextmanager
     def chdir(self, path: pathlib.Path) -> Iterator[pathlib.Path]:
         """
         Change the current working directory to the provided path.
         """
```

### Comparing `python-tools-scripts-0.9.6/src/ptscripts/process.py` & `python-tools-scripts-0.9.7/src/ptscripts/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,18 +202,18 @@
     future,
     cmdline,
     check=True,
     timeout_secs: int | None = None,
     no_output_timeout_secs: int | None = None,
     capture: bool = False,
     interactive: bool = False,
+    **kwargs,
 ):
     stdout = subprocess.PIPE
     stderr = subprocess.PIPE
-    kwargs = {}
     if interactive is False:
         # Run in a separate program group
         if sys.platform.startswith("win"):
             kwargs["creationflags"] = subprocess.CREATE_NEW_PROCESS_GROUP
         else:
             kwargs["preexec_fn"] = os.setpgrp
     proc = await _create_subprocess_exec(
@@ -245,14 +245,15 @@
 def run(
     *cmdline,
     check=True,
     timeout_secs: int | None = None,
     no_output_timeout_secs: int | None = None,
     capture: bool = False,
     interactive: bool = False,
+    **kwargs,
 ) -> subprocess.CompletedProcess[str]:
     """
     Run a command.
     """
     loop = asyncio.new_event_loop()
     future = loop.create_future()
     try:
@@ -261,14 +262,15 @@
                 future,
                 cmdline,
                 check,
                 timeout_secs=timeout_secs,
                 no_output_timeout_secs=no_output_timeout_secs,
                 capture=capture,
                 interactive=interactive,
+                **kwargs,
             )
         )
         result = future.result()
         if check is True:
             result.check_returncode()
         return cast(subprocess.CompletedProcess[str], result)
     finally:
```

### Comparing `python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/PKG-INFO` & `python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tools-scripts
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python Tools Scripts
 Home-page: https://github.com/s0undt3ch/python-tools-scripts
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/s0undt3ch/python-tools-scripts
 Project-URL: Tracker, https://github.com/s0undt3ch/python-tools-scripts/issues
```

### Comparing `python-tools-scripts-0.9.6/src/python_tools_scripts.egg-info/SOURCES.txt` & `python-tools-scripts-0.9.7/src/python_tools_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/belay-0.9.2.tar.gz` & `tmp/belay-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "belay-0.9.2.tar", max compression
+gzip compressed data, was "belay-0.9.3.tar", max compression
```

## Comparing `belay-0.9.2.tar` & `belay-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0    11357 2022-10-24 16:08:28.707037 belay-0.9.2/LICENSE
--rw-r--r--   0        0        0     3927 2022-10-24 16:08:28.707037 belay-0.9.2/README.rst
--rw-r--r--   0        0        0      542 2022-10-24 16:09:20.667590 belay-0.9.2/belay/__init__.py
--rw-r--r--   0        0        0       50 2022-10-24 16:08:28.707037 belay-0.9.2/belay/__main__.py
--rw-r--r--   0        0        0     2509 2022-10-24 16:08:28.707037 belay-0.9.2/belay/_minify.py
--rw-r--r--   0        0        0       55 2022-10-24 16:08:28.707037 belay-0.9.2/belay/cli/__init__.py
--rw-r--r--   0        0        0     4753 2022-10-24 16:08:28.707037 belay-0.9.2/belay/cli/main.py
--rw-r--r--   0        0        0    24895 2022-10-24 16:08:28.707037 belay-0.9.2/belay/device.py
--rw-r--r--   0        0        0      710 2022-10-24 16:08:28.707037 belay-0.9.2/belay/exceptions.py
--rw-r--r--   0        0        0     1153 2022-10-24 16:08:28.707037 belay-0.9.2/belay/inspect.py
--rw-r--r--   0        0        0    27913 2022-10-24 16:08:28.707037 belay-0.9.2/belay/pyboard.py
--rw-r--r--   0        0        0        0 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/__init__.py
--rw-r--r--   0        0        0       94 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/convenience_imports_circuitpython.py
--rw-r--r--   0        0        0      129 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/convenience_imports_micropython.py
--rw-r--r--   0        0        0      574 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/startup.py
--rw-r--r--   0        0        0     1377 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/sync_begin.py
--rw-r--r--   0        0        0      209 2022-10-24 16:08:28.707037 belay-0.9.2/belay/snippets/sync_end.py
--rw-r--r--   0        0        0     9772 2022-10-24 16:08:28.707037 belay-0.9.2/belay/webrepl.py
--rw-r--r--   0        0        0     1968 2022-10-24 16:09:20.663590 belay-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 belay-0.9.2/setup.py
--rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 belay-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-24 18:37:52.199331 belay-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3927 2022-10-24 18:37:52.199331 belay-0.9.3/README.rst
+-rw-r--r--   0        0        0      542 2022-10-24 18:39:03.829954 belay-0.9.3/belay/__init__.py
+-rw-r--r--   0        0        0       50 2022-10-24 18:37:52.203331 belay-0.9.3/belay/__main__.py
+-rw-r--r--   0        0        0     2509 2022-10-24 18:37:52.203331 belay-0.9.3/belay/_minify.py
+-rw-r--r--   0        0        0       55 2022-10-24 18:37:52.203331 belay-0.9.3/belay/cli/__init__.py
+-rw-r--r--   0        0        0     4753 2022-10-24 18:37:52.203331 belay-0.9.3/belay/cli/main.py
+-rw-r--r--   0        0        0    26524 2022-10-24 18:37:52.203331 belay-0.9.3/belay/device.py
+-rw-r--r--   0        0        0      710 2022-10-24 18:37:52.203331 belay-0.9.3/belay/exceptions.py
+-rw-r--r--   0        0        0     1153 2022-10-24 18:37:52.203331 belay-0.9.3/belay/inspect.py
+-rw-r--r--   0        0        0    27913 2022-10-24 18:37:52.203331 belay-0.9.3/belay/pyboard.py
+-rw-r--r--   0        0        0        0 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/__init__.py
+-rw-r--r--   0        0        0       94 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/convenience_imports_circuitpython.py
+-rw-r--r--   0        0        0      129 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/convenience_imports_micropython.py
+-rw-r--r--   0        0        0      129 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/emitter_check.py
+-rw-r--r--   0        0        0      426 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/hf.py
+-rw-r--r--   0        0        0      446 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/hf_native.py
+-rw-r--r--   0        0        0      541 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/hf_viper.py
+-rw-r--r--   0        0        0      149 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/ilistdir_circuitpython.py
+-rw-r--r--   0        0        0       31 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/ilistdir_micropython.py
+-rw-r--r--   0        0        0      578 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/startup.py
+-rw-r--r--   0        0        0      812 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/sync_begin.py
+-rw-r--r--   0        0        0      209 2022-10-24 18:37:52.203331 belay-0.9.3/belay/snippets/sync_end.py
+-rw-r--r--   0        0        0     9772 2022-10-24 18:37:52.203331 belay-0.9.3/belay/webrepl.py
+-rw-r--r--   0        0        0     1968 2022-10-24 18:39:03.829954 belay-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 belay-0.9.3/setup.py
+-rw-r--r--   0        0        0     4611 1970-01-01 00:00:00.000000 belay-0.9.3/PKG-INFO
```

### Comparing `belay-0.9.2/LICENSE` & `belay-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/README.rst` & `belay-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/__init__.py` & `belay-0.9.3/belay/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __all__ = [
     "AuthenticationError",
     "minify",
     "Device",
     "SpecialFunctionNameError",
     "PyboardException",
```

### Comparing `belay-0.9.2/belay/_minify.py` & `belay-0.9.3/belay/_minify.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/cli/main.py` & `belay-0.9.3/belay/cli/main.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/device.py` & `belay-0.9.3/belay/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 import concurrent.futures
 import importlib.resources as pkg_resources
 import linecache
+import re
 import secrets
 import string
 import subprocess  # nosec
 import sys
 import tempfile
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
@@ -413,19 +414,22 @@
         Type of python running on device.
         One of ``{"micropython", "circuitpython"}``.
     version: Tuple[int, int, int]
         ``(major, minor, patch)`` Semantic versioning of device's firmware.
     platform: str
         Board identifier. May not be consistent from MicroPython to CircuitPython.
         e.g. The Pi Pico is "rp2" in MicroPython, but "RP2040"  in CircuitPython.
+    emitters: tuple[str]
+        Tuple of available emitters on-device ``{"native", "viper"}``.
     """
 
     name: str
     version: Tuple[int, int, int]
     platform: str
+    emitters: Tuple[str]
 
 
 class Device:
     """Belay interface into a micropython device.
 
     Attributes
     ----------
@@ -466,25 +470,53 @@
         self.implementation = Implementation(
             *self(
                 'print("_BELAYR("'
                 '+ repr(sys.implementation.name) + ","'
                 '+ repr(sys.implementation.version) + ","'
                 '+ repr(sys.platform) + ","'
                 '+")")'
-            )
+            ),
+            emitters=self._emitter_check(),
         )
 
         if startup is None:
             if self.implementation.name == "circuitpython":
                 self._exec_snippet("convenience_imports_circuitpython")
             else:
                 self._exec_snippet("convenience_imports_micropython")
         elif startup:
             self(startup)
 
+    def _emitter_check(self):
+        # Detect which emitters are available
+        emitters = []
+        try:
+            self._exec_snippet("emitter_check")
+        except PyboardException as e:
+            if "invalid micropython decorator" not in str(e):
+                raise e
+            # Get line of exception
+            line_e = int(re.findall(r"line (\d+)", str(e))[-1])
+            if line_e == 1:
+                # No emitters available
+                pass
+            else:
+                emitters.append("native")
+                if line_e == 3:
+                    # viper is not available
+                    pass
+                else:
+                    raise Exception(f"Unknown emitter line {line_e}.")
+        else:
+            emitters.append("native")
+            emitters.append("viper")
+            self("del __belay_emitter_test")
+
+        return tuple(emitters)
+
     def _connect_to_board(self, **kwargs):
         self._board = Pyboard(**kwargs)
         if isinstance(self._board.serial, WebreplToSerial):
             soft_reset = False
         else:
             soft_reset = True
         self._board.enter_raw_repl(soft_reset=soft_reset)
@@ -607,17 +639,31 @@
             dst = dst.rstrip("/")
 
         if not folder.exists():
             raise ValueError(f'"{folder}" does not exist.')
 
         # Create a list of all files and dirs (on-device).
         # This is so we know what to clean up after done syncing.
+        snippets_to_execute = []
+
         if progress_update:
             progress_update(description="Bootstrapping sync...")
-        self._exec_snippet("sync_begin")
+        if "viper" in self.implementation.emitters:
+            snippets_to_execute.append("hf_viper")
+        elif "native" in self.implementation.emitters:
+            snippets_to_execute.append("hf_native")
+        else:
+            snippets_to_execute.append("hf")
+
+        if self.implementation.name == "circuitpython":
+            snippets_to_execute.append("ilistdir_circuitpython")
+        else:
+            snippets_to_execute.append("ilistdir_micropython")
+        snippets_to_execute.append("sync_begin")
+        self._exec_snippet(*snippets_to_execute)
 
         # Remove the keep files from the on-device ``all_files`` set
         # so they don't get deleted.
         keep_all = folder.is_file() or keep is True
         keep = _preprocess_keep(keep, dst)
         ignore = _preprocess_ignore(ignore)
```

### Comparing `belay-0.9.2/belay/exceptions.py` & `belay-0.9.3/belay/exceptions.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/inspect.py` & `belay-0.9.3/belay/inspect.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/pyboard.py` & `belay-0.9.3/belay/pyboard.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/belay/snippets/startup.py` & `belay-0.9.3/belay/snippets/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import sys
+import os, sys
 def __belay(name):
     def inner(f):
         def func_wrapper(*args, **kwargs):
             res = f(*args, **kwargs)
             print("_BELAYR" + repr(res))
             return res
         def gen_wrapper(*args, **kwargs):
```

### Comparing `belay-0.9.2/belay/webrepl.py` & `belay-0.9.3/belay/webrepl.py`

 * *Files identical despite different names*

### Comparing `belay-0.9.2/pyproject.toml` & `belay-0.9.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "belay"
-version = "0.9.2"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "0.9.3"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/belay"
 repository = "https://github.com/BrianPugh/belay"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "belay"}]
```

### Comparing `belay-0.9.2/setup.py` & `belay-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['pathspec', 'pyserial>=3.1,<4.0', 'typer[all]>=0.6,<0.7']
 
 entry_points = \
 {'console_scripts': ['belay = belay.cli.main:app']}
 
 setup_kwargs = {
     'name': 'belay',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': '',
     'long_description': '.. image:: https://raw.githubusercontent.com/BrianPugh/belay/main/assets/logo_white_400w.png\n\n|Python compat| |PyPi| |GHA tests| |readthedocs|\n\n\nBelay\n=====\n\n.. inclusion-marker-do-not-remove\n\nBelay is a library that enables the rapid development of projects that interact with hardware via a MicroPython or CircuitPython compatible board.\n\nBelay works by interacting with the REPL interface of a MicroPython board from Python code running on PC.\n\nBelay supports wired serial connections (USB) and wireless connections via WebREPL over WiFi.\n\n`Quick Video of Belay in 22 seconds.`_\n\nSee `the documentation`_ for usage and other details.\n\nWho is Belay For?\n=================\n\nBelay is for people creating a software project that needs to interact with hardware.\nExamples include:\n\n* Control a motor so a webcam is always pointing at a person.\n\n* Turn on an LED when you receive a notification.\n\n* Read a potentiometer to control system volume.\n\nIf you have no need to run Python code on PC, then Belay is not for you.\n\n\nWhat Problems Does Belay Solve?\n===============================\n\nTypically, having a python script interact with hardware involves 3 major challenges:\n\n1. On-device firmware (usually C or MicroPython) for directly handling hardware interactions. Typically this is developed, compiled, and uploaded as a (nearly) independent project.\n\n2. A program on your computer that performs the tasks specified and interacts with the device.\n\n3. Computer-to-device communication protocol. How are commands and results transferred? How does the device execute those commands?\n\n\nThis is lot of work if you just want your computer to do something simple like turn on an LED.\nBelay simplifies all of this by merging steps 1 and 2 into the same codebase, and manages step 3 for you.\nCode is automatically synced at the beginning of script execution.\n\nInstallation\n============\n\nBelay requires Python ``>=3.8`` and can be installed via:\n\n.. code-block:: bash\n\n   pip install belay\n\nThe MicroPython-compatible board only needs MicroPython installed; no additional preparation is required.\nIf using CircuitPython, and additional modification needs to be made to ``boot.py``. See `documentation <https://belay.readthedocs.io/en/latest/CircuitPython.html>`_ for details.\n\nExamples\n========\n\nTurning on an LED with Belay takes only 6 lines of code.\nFunctions decorated with the ``task`` decorator are sent to the device and interpreted by the MicroPython interpreter.\nCalling the decorated function on-host sends a command to the device to execute the actual function.\n\n.. code-block:: python\n\n   import belay\n\n   device = belay.Device("/dev/ttyUSB0")\n\n\n   @device.task\n   def set_led(state):\n       print(f"Printing from device; turning LED to {state}.")\n       Pin(25, Pin.OUT).value(state)\n\n\n   set_led(True)\n\nOutputs from ``print`` calls from on-device user-code are forwarded to host ``stdout``.\n\n`For more examples, see the examples folder.`_\n\n\n.. |GHA tests| image:: https://github.com/BrianPugh/belay/workflows/tests/badge.svg\n   :target: https://github.com/BrianPugh/belay/actions?query=workflow%3Atests\n   :alt: GHA Status\n.. |Codecov report| image:: https://codecov.io/github/BrianPugh/belay/coverage.svg?branch=main\n   :target: https://codecov.io/github/BrianPugh/belay?branch=main\n   :alt: Coverage\n.. |readthedocs| image:: https://readthedocs.org/projects/belay/badge/?version=latest\n        :target: https://belay.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n.. |Python compat| image:: https://img.shields.io/badge/>=python-3.8-blue.svg\n.. |PyPi| image:: https://img.shields.io/pypi/v/belay.svg\n        :target: https://pypi.python.org/pypi/belay\n.. _Quick Video of Belay in 22 seconds.: https://www.youtube.com/watch?v=wq3cyjSE8ek\n.. _the documentation: https://belay.readthedocs.io\n.. _For more examples, see the examples folder.:  https://github.com/BrianPugh/belay/tree/main/examples\n',
     'author': 'Brian Pugh',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/BrianPugh/belay',
```

### Comparing `belay-0.9.2/PKG-INFO` & `belay-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belay
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Home-page: https://github.com/BrianPugh/belay
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


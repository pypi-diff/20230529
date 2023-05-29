# Comparing `tmp/pytest-xvfb-2.0.0.tar.gz` & `tmp/pytest-xvfb-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-xvfb-2.0.0.tar", last modified: Tue Jun  9 17:16:19 2020, max compression
+gzip compressed data, was "pytest-xvfb-3.0.0.tar", last modified: Mon May 29 11:54:26 2023, max compression
```

## Comparing `pytest-xvfb-2.0.0.tar` & `pytest-xvfb-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-09 17:16:19.892358 pytest-xvfb-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1249 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)       51 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5123 2020-06-09 17:16:19.892358 pytest-xvfb-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3305 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-09 17:16:19.888358 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5123 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      336 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       31 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       36 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-06-09 17:16:19.000000 pytest-xvfb-2.0.0/pytest_xvfb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3232 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/pytest_xvfb.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-06-09 17:16:19.892358 pytest-xvfb-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-09 17:16:19.888358 pytest-xvfb-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     5933 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/tests/test_xvfb.py
--rw-r--r--   0 runner    (1001) docker     (116)      270 2020-06-09 17:16:09.000000 pytest-xvfb-2.0.0/tests/test_xvfb_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:54:26.292681 pytest-xvfb-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-29 11:54:26.292681 pytest-xvfb-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:54:26.292681 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 11:54:26.000000 pytest-xvfb-3.0.0/pytest_xvfb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/pytest_xvfb.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:54:26.292681 pytest-xvfb-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:54:26.292681 pytest-xvfb-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/tests/test_qtwe_xio_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/tests/test_xvfb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-29 11:54:19.000000 pytest-xvfb-3.0.0/tests/test_xvfb_windows.py
```

### Comparing `pytest-xvfb-2.0.0/PKG-INFO` & `pytest-xvfb-3.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,124 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-xvfb
-Version: 2.0.0
-Summary: A pytest plugin to run Xvfb for tests.
-Home-page: https://github.com/The-Compiler/pytest-xvfb
-Author: Florian Bruhin
-Author-email: me@the-compiler.org
-Maintainer: Florian Bruhin
-Maintainer-email: me@the-compiler.org
+Version: 3.0.0
+Summary: A pytest plugin to run Xvfb (or Xephyr/Xvnc) for tests.
+Author-email: Florian Bruhin <me@the-compiler.org>
+Maintainer-email: Florian Bruhin <me@the-compiler.org>
 License: MIT
-Description: pytest-xvfb
-        ===================================
-        
-        .. image:: https://travis-ci.org/The-Compiler/pytest-xvfb.svg?branch=master
-            :target: https://travis-ci.org/The-Compiler/pytest-xvfb
-            :alt: See Build Status on Travis CI
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/github/The-Compiler/pytest-xvfb?branch=master
-            :target: https://ci.appveyor.com/project/The-Compiler/pytest-xvfb/branch/master
-            :alt: See Build Status on AppVeyor
-        
-        A pytest plugin to run Xvfb for tests.
-        
-        ----
-        
-        Installation
-        ------------
-        
-        You can install "`pytest-xvfb`_" via `pip`_ from `PyPI`_::
-        
-            $ pip install pytest-xvfb
-        
-        
-        Usage
-        -----
-        
-        With Xvfb and the plugin installed, your testsuite automatically runs with `Xvfb`_. This allows tests to be run without windows popping up during GUI tests or on systems without a display (like a CI).
-        
-        If Xvfb is not installed, the plugin does not run and your tests will still work as normal. However,
-        a warning message will print to standard output letting you know that Xvfb is not installed.
-        
-        If you're currently using ``xvfb-run`` in something like ``.travis.yml``,
-        simply remove it and install this plugin instead - then you'll also have the
-        benefits of Xvfb locally.
-        
-        Features
-        --------
-        
-        You can pass ``--no-xvfb`` to explicitly turn off Xvfb (e.g. to visually
-        inspect a failure).
-        
-        You can mark tests with ``@pytest.mark.no_xvfb`` to skip them when they're
-        running with Xvfb.
-        
-        A ``xvfb`` fixture is available with the following attributes:
-        
-        - ``width``: The configured width of the screen.
-        - ``height``: The configured height of the screen.
-        - ``colordepth``: The configured colordepth of the screen.
-        - ``args``: The arguments to be passed to Xvfb.
-        - ``display``: The display number (as int) which is used.
-        
-        Contributing
-        ------------
-        
-        Contributions are very welcome. Tests can be run with `tox`_, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        License
-        -------
-        
-        Distributed under the terms of the `MIT`_ license, "pytest-xvfb" is free and open source software
-        
-        Thanks
-        ------
-        
-        This `pytest`_ plugin was generated with `Cookiecutter`_ along with
-        `@hackebrot`_'s `Cookiecutter-pytest-plugin`_ template.
-        
-        Thanks to `@cgoldberg`_ for `xvfbwrapper`_ which was the inspiration for this
-        project.
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`pytest-xvfb`: https://pypi.python.org/pypi/pytest-xvfb/
-        .. _`Xvfb`: http://www.x.org/releases/X11R7.6/doc/man/man1/Xvfb.1.xhtml
-        .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-        .. _`@hackebrot`: https://github.com/hackebrot
-        .. _`@cgoldberg`: https://github.com/cgoldberg
-        .. _`xvfbwrapper`: https://github.com/cgoldberg/xvfbwrapper
-        .. _`MIT`: http://opensource.org/licenses/MIT
-        .. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
-        .. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
-        .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
-        .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-        .. _`file an issue`: https://github.com/The-Compiler/pytest-xvfb/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: https://tox.readthedocs.org/en/latest/
-        .. _`pip`: https://pypi.python.org/pypi/pip/
-        .. _`PyPI`: https://pypi.python.org/pypi
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/The-Compiler/pytest-xvfb
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.5
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+pytest-xvfb
+===================================
+
+A pytest plugin to run `Xvfb`_ (or `Xephyr`_/`Xvnc`_) for tests.
+
+----
+
+Installation
+------------
+
+You can install "`pytest-xvfb`_" via `pip`_ from `PyPI`_::
+
+    $ pip install pytest-xvfb
+
+
+Usage
+-----
+
+With Xvfb and the plugin installed, your testsuite automatically runs with `Xvfb`_. This allows tests to be run without windows popping up during GUI tests or on systems without a display (like a CI).
+
+The plugin sees Xvfb being installed as "optional", since the tests can still
+run without it installed. If it's unavailable, it will show an informational
+message, if on Linux and a ``DISPLAY`` is available. When using
+``--xvfb-backend xvfb``, this message will turn into a hard error instead.
+
+If you're currently using ``xvfb-run`` in something like a GitHub Actions YAML
+file simply remove the wrapper and install this plugin instead - then you'll
+also have the benefits of Xvfb locally.
+
+Features
+--------
+
+You can pass ``--no-xvfb`` to explicitly turn off Xvfb (e.g. to visually
+inspect a failure).
+
+With ``--xvfb-backend xephyr`` or ``--xvfb-backend xvnc``, you can use Xephyr
+or Xvnc in place of Xvfb, e.g. to visually inspect failures.
+
+**NOTE:** Support for ``xvnc`` is currently experimental and not tested on CI,
+due to incompatibilities with PyVirtualDisplay and Ubuntu 22.04's tightvncserver.
+
+You can mark tests with ``@pytest.mark.no_xvfb`` to skip them when they're
+running with Xvfb.
+
+A ``xvfb`` fixture is available with the following attributes:
+
+- ``width``: The configured width of the screen.
+- ``height``: The configured height of the screen.
+- ``colordepth``: The configured colordepth of the screen.
+- ``args``: The arguments to be passed to Xvfb.
+- ``display``: The display number (as int) which is used.
+- ``backend``: Either ``None`` (Xvfb), ``"xvfb"``, ``"xephyr"``, or ``"xvnc"``.
+
+In a pytest.ini, ``xvfb_width``, ``xvfb_height``, ``xvfb_colordepth`` and
+``xvfb_args`` can be used to configure the respective values. In addition,
+``xvfb_xauth`` can be set to ``true`` to generate an ``Xauthority`` token.
+
+Contributing
+------------
+
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+License
+-------
+
+Distributed under the terms of the `MIT`_ license, "pytest-xvfb" is free and open source software
+
+Thanks
+------
+
+This `pytest`_ plugin was generated with `Cookiecutter`_ along with
+`@hackebrot`_'s `Cookiecutter-pytest-plugin`_ template.
+
+Thanks to `@cgoldberg`_ for `xvfbwrapper`_ which was the inspiration for this
+project.
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`pytest-xvfb`: https://pypi.python.org/pypi/pytest-xvfb/
+.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
+.. _`@hackebrot`: https://github.com/hackebrot
+.. _`@cgoldberg`: https://github.com/cgoldberg
+.. _`xvfbwrapper`: https://github.com/cgoldberg/xvfbwrapper
+.. _`MIT`: http://opensource.org/licenses/MIT
+.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
+.. _`file an issue`: https://github.com/The-Compiler/pytest-xvfb/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: https://tox.readthedocs.org/en/latest/
+.. _`pip`: https://pypi.python.org/pypi/pip/
+.. _`PyPI`: https://pypi.python.org/pypi
+.. _`Xvfb`: https://en.wikipedia.org/wiki/Xvfb
+.. _`Xephyr`: https://www.freedesktop.org/wiki/Software/Xephyr/
+.. _`Xvnc`: https://tigervnc.org/doc/Xvnc.html
```

### Comparing `pytest-xvfb-2.0.0/README.rst` & `pytest-xvfb-3.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 pytest-xvfb
 ===================================
 
-.. image:: https://travis-ci.org/The-Compiler/pytest-xvfb.svg?branch=master
-    :target: https://travis-ci.org/The-Compiler/pytest-xvfb
-    :alt: See Build Status on Travis CI
-
-.. image:: https://ci.appveyor.com/api/projects/status/github/The-Compiler/pytest-xvfb?branch=master
-    :target: https://ci.appveyor.com/project/The-Compiler/pytest-xvfb/branch/master
-    :alt: See Build Status on AppVeyor
-
-A pytest plugin to run Xvfb for tests.
+A pytest plugin to run `Xvfb`_ (or `Xephyr`_/`Xvnc`_) for tests.
 
 ----
 
 Installation
 ------------
 
 You can install "`pytest-xvfb`_" via `pip`_ from `PyPI`_::
@@ -22,37 +14,50 @@
 
 
 Usage
 -----
 
 With Xvfb and the plugin installed, your testsuite automatically runs with `Xvfb`_. This allows tests to be run without windows popping up during GUI tests or on systems without a display (like a CI).
 
-If Xvfb is not installed, the plugin does not run and your tests will still work as normal. However,
-a warning message will print to standard output letting you know that Xvfb is not installed.
-
-If you're currently using ``xvfb-run`` in something like ``.travis.yml``,
-simply remove it and install this plugin instead - then you'll also have the
-benefits of Xvfb locally.
+The plugin sees Xvfb being installed as "optional", since the tests can still
+run without it installed. If it's unavailable, it will show an informational
+message, if on Linux and a ``DISPLAY`` is available. When using
+``--xvfb-backend xvfb``, this message will turn into a hard error instead.
+
+If you're currently using ``xvfb-run`` in something like a GitHub Actions YAML
+file simply remove the wrapper and install this plugin instead - then you'll
+also have the benefits of Xvfb locally.
 
 Features
 --------
 
 You can pass ``--no-xvfb`` to explicitly turn off Xvfb (e.g. to visually
 inspect a failure).
 
+With ``--xvfb-backend xephyr`` or ``--xvfb-backend xvnc``, you can use Xephyr
+or Xvnc in place of Xvfb, e.g. to visually inspect failures.
+
+**NOTE:** Support for ``xvnc`` is currently experimental and not tested on CI,
+due to incompatibilities with PyVirtualDisplay and Ubuntu 22.04's tightvncserver.
+
 You can mark tests with ``@pytest.mark.no_xvfb`` to skip them when they're
 running with Xvfb.
 
 A ``xvfb`` fixture is available with the following attributes:
 
 - ``width``: The configured width of the screen.
 - ``height``: The configured height of the screen.
 - ``colordepth``: The configured colordepth of the screen.
 - ``args``: The arguments to be passed to Xvfb.
 - ``display``: The display number (as int) which is used.
+- ``backend``: Either ``None`` (Xvfb), ``"xvfb"``, ``"xephyr"``, or ``"xvnc"``.
+
+In a pytest.ini, ``xvfb_width``, ``xvfb_height``, ``xvfb_colordepth`` and
+``xvfb_args`` can be used to configure the respective values. In addition,
+``xvfb_xauth`` can be set to ``true`` to generate an ``Xauthority`` token.
 
 Contributing
 ------------
 
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
@@ -72,22 +77,21 @@
 
 Issues
 ------
 
 If you encounter any problems, please `file an issue`_ along with a detailed description.
 
 .. _`pytest-xvfb`: https://pypi.python.org/pypi/pytest-xvfb/
-.. _`Xvfb`: http://www.x.org/releases/X11R7.6/doc/man/man1/Xvfb.1.xhtml
 .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
 .. _`@hackebrot`: https://github.com/hackebrot
 .. _`@cgoldberg`: https://github.com/cgoldberg
 .. _`xvfbwrapper`: https://github.com/cgoldberg/xvfbwrapper
 .. _`MIT`: http://opensource.org/licenses/MIT
-.. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
-.. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
-.. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
 .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
 .. _`file an issue`: https://github.com/The-Compiler/pytest-xvfb/issues
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: https://tox.readthedocs.org/en/latest/
 .. _`pip`: https://pypi.python.org/pypi/pip/
 .. _`PyPI`: https://pypi.python.org/pypi
+.. _`Xvfb`: https://en.wikipedia.org/wiki/Xvfb
+.. _`Xephyr`: https://www.freedesktop.org/wiki/Software/Xephyr/
+.. _`Xvnc`: https://tigervnc.org/doc/Xvnc.html
```

### Comparing `pytest-xvfb-2.0.0/pytest_xvfb.egg-info/PKG-INFO` & `pytest-xvfb-3.0.0/pytest_xvfb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,120 +1,124 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-xvfb
-Version: 2.0.0
-Summary: A pytest plugin to run Xvfb for tests.
-Home-page: https://github.com/The-Compiler/pytest-xvfb
-Author: Florian Bruhin
-Author-email: me@the-compiler.org
-Maintainer: Florian Bruhin
-Maintainer-email: me@the-compiler.org
+Version: 3.0.0
+Summary: A pytest plugin to run Xvfb (or Xephyr/Xvnc) for tests.
+Author-email: Florian Bruhin <me@the-compiler.org>
+Maintainer-email: Florian Bruhin <me@the-compiler.org>
 License: MIT
-Description: pytest-xvfb
-        ===================================
-        
-        .. image:: https://travis-ci.org/The-Compiler/pytest-xvfb.svg?branch=master
-            :target: https://travis-ci.org/The-Compiler/pytest-xvfb
-            :alt: See Build Status on Travis CI
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/github/The-Compiler/pytest-xvfb?branch=master
-            :target: https://ci.appveyor.com/project/The-Compiler/pytest-xvfb/branch/master
-            :alt: See Build Status on AppVeyor
-        
-        A pytest plugin to run Xvfb for tests.
-        
-        ----
-        
-        Installation
-        ------------
-        
-        You can install "`pytest-xvfb`_" via `pip`_ from `PyPI`_::
-        
-            $ pip install pytest-xvfb
-        
-        
-        Usage
-        -----
-        
-        With Xvfb and the plugin installed, your testsuite automatically runs with `Xvfb`_. This allows tests to be run without windows popping up during GUI tests or on systems without a display (like a CI).
-        
-        If Xvfb is not installed, the plugin does not run and your tests will still work as normal. However,
-        a warning message will print to standard output letting you know that Xvfb is not installed.
-        
-        If you're currently using ``xvfb-run`` in something like ``.travis.yml``,
-        simply remove it and install this plugin instead - then you'll also have the
-        benefits of Xvfb locally.
-        
-        Features
-        --------
-        
-        You can pass ``--no-xvfb`` to explicitly turn off Xvfb (e.g. to visually
-        inspect a failure).
-        
-        You can mark tests with ``@pytest.mark.no_xvfb`` to skip them when they're
-        running with Xvfb.
-        
-        A ``xvfb`` fixture is available with the following attributes:
-        
-        - ``width``: The configured width of the screen.
-        - ``height``: The configured height of the screen.
-        - ``colordepth``: The configured colordepth of the screen.
-        - ``args``: The arguments to be passed to Xvfb.
-        - ``display``: The display number (as int) which is used.
-        
-        Contributing
-        ------------
-        
-        Contributions are very welcome. Tests can be run with `tox`_, please ensure
-        the coverage at least stays the same before you submit a pull request.
-        
-        License
-        -------
-        
-        Distributed under the terms of the `MIT`_ license, "pytest-xvfb" is free and open source software
-        
-        Thanks
-        ------
-        
-        This `pytest`_ plugin was generated with `Cookiecutter`_ along with
-        `@hackebrot`_'s `Cookiecutter-pytest-plugin`_ template.
-        
-        Thanks to `@cgoldberg`_ for `xvfbwrapper`_ which was the inspiration for this
-        project.
-        
-        Issues
-        ------
-        
-        If you encounter any problems, please `file an issue`_ along with a detailed description.
-        
-        .. _`pytest-xvfb`: https://pypi.python.org/pypi/pytest-xvfb/
-        .. _`Xvfb`: http://www.x.org/releases/X11R7.6/doc/man/man1/Xvfb.1.xhtml
-        .. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
-        .. _`@hackebrot`: https://github.com/hackebrot
-        .. _`@cgoldberg`: https://github.com/cgoldberg
-        .. _`xvfbwrapper`: https://github.com/cgoldberg/xvfbwrapper
-        .. _`MIT`: http://opensource.org/licenses/MIT
-        .. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause
-        .. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt
-        .. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0
-        .. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
-        .. _`file an issue`: https://github.com/The-Compiler/pytest-xvfb/issues
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: https://tox.readthedocs.org/en/latest/
-        .. _`pip`: https://pypi.python.org/pypi/pip/
-        .. _`PyPI`: https://pypi.python.org/pypi
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/The-Compiler/pytest-xvfb
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.5
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+pytest-xvfb
+===================================
+
+A pytest plugin to run `Xvfb`_ (or `Xephyr`_/`Xvnc`_) for tests.
+
+----
+
+Installation
+------------
+
+You can install "`pytest-xvfb`_" via `pip`_ from `PyPI`_::
+
+    $ pip install pytest-xvfb
+
+
+Usage
+-----
+
+With Xvfb and the plugin installed, your testsuite automatically runs with `Xvfb`_. This allows tests to be run without windows popping up during GUI tests or on systems without a display (like a CI).
+
+The plugin sees Xvfb being installed as "optional", since the tests can still
+run without it installed. If it's unavailable, it will show an informational
+message, if on Linux and a ``DISPLAY`` is available. When using
+``--xvfb-backend xvfb``, this message will turn into a hard error instead.
+
+If you're currently using ``xvfb-run`` in something like a GitHub Actions YAML
+file simply remove the wrapper and install this plugin instead - then you'll
+also have the benefits of Xvfb locally.
+
+Features
+--------
+
+You can pass ``--no-xvfb`` to explicitly turn off Xvfb (e.g. to visually
+inspect a failure).
+
+With ``--xvfb-backend xephyr`` or ``--xvfb-backend xvnc``, you can use Xephyr
+or Xvnc in place of Xvfb, e.g. to visually inspect failures.
+
+**NOTE:** Support for ``xvnc`` is currently experimental and not tested on CI,
+due to incompatibilities with PyVirtualDisplay and Ubuntu 22.04's tightvncserver.
+
+You can mark tests with ``@pytest.mark.no_xvfb`` to skip them when they're
+running with Xvfb.
+
+A ``xvfb`` fixture is available with the following attributes:
+
+- ``width``: The configured width of the screen.
+- ``height``: The configured height of the screen.
+- ``colordepth``: The configured colordepth of the screen.
+- ``args``: The arguments to be passed to Xvfb.
+- ``display``: The display number (as int) which is used.
+- ``backend``: Either ``None`` (Xvfb), ``"xvfb"``, ``"xephyr"``, or ``"xvnc"``.
+
+In a pytest.ini, ``xvfb_width``, ``xvfb_height``, ``xvfb_colordepth`` and
+``xvfb_args`` can be used to configure the respective values. In addition,
+``xvfb_xauth`` can be set to ``true`` to generate an ``Xauthority`` token.
+
+Contributing
+------------
+
+Contributions are very welcome. Tests can be run with `tox`_, please ensure
+the coverage at least stays the same before you submit a pull request.
+
+License
+-------
+
+Distributed under the terms of the `MIT`_ license, "pytest-xvfb" is free and open source software
+
+Thanks
+------
+
+This `pytest`_ plugin was generated with `Cookiecutter`_ along with
+`@hackebrot`_'s `Cookiecutter-pytest-plugin`_ template.
+
+Thanks to `@cgoldberg`_ for `xvfbwrapper`_ which was the inspiration for this
+project.
+
+Issues
+------
+
+If you encounter any problems, please `file an issue`_ along with a detailed description.
+
+.. _`pytest-xvfb`: https://pypi.python.org/pypi/pytest-xvfb/
+.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter
+.. _`@hackebrot`: https://github.com/hackebrot
+.. _`@cgoldberg`: https://github.com/cgoldberg
+.. _`xvfbwrapper`: https://github.com/cgoldberg/xvfbwrapper
+.. _`MIT`: http://opensource.org/licenses/MIT
+.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin
+.. _`file an issue`: https://github.com/The-Compiler/pytest-xvfb/issues
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: https://tox.readthedocs.org/en/latest/
+.. _`pip`: https://pypi.python.org/pypi/pip/
+.. _`PyPI`: https://pypi.python.org/pypi
+.. _`Xvfb`: https://en.wikipedia.org/wiki/Xvfb
+.. _`Xephyr`: https://www.freedesktop.org/wiki/Software/Xephyr/
+.. _`Xvnc`: https://tigervnc.org/doc/Xvnc.html
```


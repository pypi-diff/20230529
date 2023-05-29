# Comparing `tmp/creativecontrol-circuitpython-ltc166x-0.1.1rc2.tar.gz` & `tmp/creativecontrol-circuitpython-ltc166x-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creativecontrol-circuitpython-ltc166x-0.1.1rc2.tar", last modified: Mon May 29 17:37:20 2023, max compression
+gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.1.tar", last modified: Mon May 29 17:40:35 2023, max compression
```

## Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2.tar` & `creativecontrol-circuitpython-ltc166x-1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.038471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.034471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.034471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.034471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.034471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-29 17:37:20.038471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.038471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-29 17:37:20.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 17:37:20.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:37:20.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 17:37:20.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:37:20.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-29 17:37:11.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:37:20.038471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-29 17:37:11.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/examples/creativecontrol_circuitpython_ltc166x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-29 17:37:11.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 17:37:02.000000 creativecontrol-circuitpython-ltc166x-0.1.1rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:37:20.038471 creativecontrol-circuitpython-ltc166x-0.1.1rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/setup.cfg
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/release_gh.yml` & `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.github/workflows/release_pypi.yml` & `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.gitignore` & `creativecontrol-circuitpython-ltc166x-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.pre-commit-config.yaml` & `creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/.pylintrc` & `creativecontrol-circuitpython-ltc166x-1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/CODE_OF_CONDUCT.md` & `creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSE` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/CC-BY-4.0.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/MIT.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/LICENSES/Unlicense.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 0.1.1rc2
+Version: 1.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/README.rst` & `creativecontrol-circuitpython-ltc166x-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 0.1.1rc2
+Version: 1.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/creativecontrol_circuitpython_ltc166x.py` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 """
 
 import microcontroller
 from busio import SPI
 import digitalio
 from adafruit_bus_device.spi_device import SPIDevice
 
-__version__ = "0.1.1-rc2"
+__version__ = "01.1"
 __repo__ = (
     "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X.git"
 )
 
 
 class LTC166X:
     """
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/examples/creativecontrol_circuitpython_ltc166x_simpletest.py` & `creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.1.1rc2/pyproject.toml` & `creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "creativecontrol-circuitpython-ltc166x"
 description = "CircuitPython library for control of LTC166X 8-bit and 10-bit DACs."
-version = "0.1.1-rc2"
+version = "01.1"
 readme = "README.rst"
 authors = [
     {name = "creativecontrol", email = "t@creativecontrol.cc"}
 ]
 urls = {Homepage = "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X"}
 keywords = [
     "adafruit",
```


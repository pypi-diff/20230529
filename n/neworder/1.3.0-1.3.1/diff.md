# Comparing `tmp/neworder-1.3.0.tar.gz` & `tmp/neworder-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neworder-1.3.0.tar", last modified: Sun Apr  2 07:35:49 2023, max compression
+gzip compressed data, was "neworder-1.3.1.tar", last modified: Mon May 29 09:36:30 2023, max compression
```

## Comparing `neworder-1.3.0.tar` & `neworder-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.854714 neworder-1.3.0/
--rw-rw-r--   0 az        (1000) az        (1000)     1085 2023-01-06 19:30:47.000000 neworder-1.3.0/LICENCE.md
--rw-rw-r--   0 az        (1000) az        (1000)      107 2023-04-02 07:19:22.000000 neworder-1.3.0/MANIFEST.in
--rw-rw-r--   0 az        (1000) az        (1000)     4957 2023-04-02 07:35:49.854714 neworder-1.3.0/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)     4509 2023-03-14 08:06:56.000000 neworder-1.3.0/README.md
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.850714 neworder-1.3.0/neworder/
--rw-rw-r--   0 az        (1000) az        (1000)      334 2023-02-25 10:00:20.000000 neworder-1.3.0/neworder/__init__.py
--rw-rw-r--   0 az        (1000) az        (1000)    15911 2023-01-22 10:16:05.000000 neworder-1.3.0/neworder/__init__.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     1290 2022-08-17 09:35:42.000000 neworder-1.3.0/neworder/df.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     7660 2022-08-17 09:35:47.000000 neworder-1.3.0/neworder/domain.py
--rw-rw-r--   0 az        (1000) az        (1000)     2783 2023-01-22 10:16:05.000000 neworder-1.3.0/neworder/graph.py
--rw-rw-r--   0 az        (1000) az        (1000)      383 2022-08-17 19:43:06.000000 neworder-1.3.0/neworder/mc.py
--rw-rw-r--   0 az        (1000) az        (1000)      298 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/mpi.pyi
--rw-rw-r--   0 az        (1000) az        (1000)        0 2022-03-13 13:41:33.000000 neworder-1.3.0/neworder/py.typed
--rw-rw-r--   0 az        (1000) az        (1000)     1328 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/stats.pyi
--rw-rw-r--   0 az        (1000) az        (1000)     1164 2022-08-17 09:36:56.000000 neworder-1.3.0/neworder/time.pyi
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.850714 neworder-1.3.0/neworder.egg-info/
--rw-rw-r--   0 az        (1000) az        (1000)     4957 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)      741 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/SOURCES.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/dependency_links.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2022-03-13 10:10:41.000000 neworder-1.3.0/neworder.egg-info/not-zip-safe
--rw-rw-r--   0 az        (1000) az        (1000)       45 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/requires.txt
--rw-rw-r--   0 az        (1000) az        (1000)       24 2023-04-02 07:35:49.000000 neworder-1.3.0/neworder.egg-info/top_level.txt
--rw-rw-r--   0 az        (1000) az        (1000)      228 2023-03-13 18:45:48.000000 neworder-1.3.0/pyproject.toml
--rw-rw-r--   0 az        (1000) az        (1000)      290 2023-04-02 07:35:49.854714 neworder-1.3.0/setup.cfg
--rwxrwxr-x   0 az        (1000) az        (1000)     1625 2023-01-22 10:16:05.000000 neworder-1.3.0/setup.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-02 07:35:49.854714 neworder-1.3.0/src/
--rw-rw-r--   0 az        (1000) az        (1000)     4097 2022-01-15 09:49:56.000000 neworder-1.3.0/src/ArrayHelpers.h
--rw-rw-r--   0 az        (1000) az        (1000)     5789 2021-06-27 21:14:58.000000 neworder-1.3.0/src/DataFrame.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      633 2020-09-18 10:07:40.000000 neworder-1.3.0/src/DataFrame.h
--rw-rw-r--   0 az        (1000) az        (1000)      410 2020-10-21 18:49:46.000000 neworder-1.3.0/src/Error.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      547 2020-09-07 20:08:04.000000 neworder-1.3.0/src/Error.h
--rw-rw-r--   0 az        (1000) az        (1000)      577 2021-11-13 15:52:34.000000 neworder-1.3.0/src/Log.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     2313 2021-11-13 15:46:23.000000 neworder-1.3.0/src/Log.h
--rw-rw-r--   0 az        (1000) az        (1000)     3232 2021-11-13 15:53:53.000000 neworder-1.3.0/src/Model.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      893 2021-06-29 19:32:00.000000 neworder-1.3.0/src/Model.h
--rw-rw-r--   0 az        (1000) az        (1000)    12404 2022-08-17 19:54:21.000000 neworder-1.3.0/src/Module.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      662 2021-03-21 12:01:03.000000 neworder-1.3.0/src/Module.h
--rw-rw-r--   0 az        (1000) az        (1000)    14430 2022-03-13 13:41:33.000000 neworder-1.3.0/src/Module_docstr.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     9890 2023-01-07 19:45:30.000000 neworder-1.3.0/src/MonteCarlo.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     2949 2022-08-17 19:43:06.000000 neworder-1.3.0/src/MonteCarlo.h
--rw-rw-r--   0 az        (1000) az        (1000)      643 2021-07-05 18:31:34.000000 neworder-1.3.0/src/NPArray.cpp
--rw-rw-r--   0 az        (1000) az        (1000)      526 2021-07-05 18:32:01.000000 neworder-1.3.0/src/NPArray.h
--rw-rw-r--   0 az        (1000) az        (1000)      393 2020-10-22 08:16:54.000000 neworder-1.3.0/src/NewOrder.h
--rw-rw-r--   0 az        (1000) az        (1000)    11492 2021-06-29 19:31:41.000000 neworder-1.3.0/src/Timeline.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     5911 2021-06-29 19:31:41.000000 neworder-1.3.0/src/Timeline.h
--rw-rw-r--   0 az        (1000) az        (1000)      550 2022-01-14 19:17:46.000000 neworder-1.3.0/src/Timer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:36:30.763673 neworder-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 09:36:19.000000 neworder-1.3.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-29 09:36:19.000000 neworder-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-29 09:36:30.763673 neworder-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-29 09:36:19.000000 neworder-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:36:30.755672 neworder-1.3.1/neworder/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-29 09:36:23.000000 neworder-1.3.1/neworder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/df.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/mc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/mpi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-29 09:36:19.000000 neworder-1.3.1/neworder/time.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:36:30.755672 neworder-1.3.1/neworder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 09:36:30.000000 neworder-1.3.1/neworder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-29 09:36:19.000000 neworder-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 09:36:30.763673 neworder-1.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1607 2023-05-29 09:36:19.000000 neworder-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:36:30.763673 neworder-1.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-29 09:36:19.000000 neworder-1.3.1/src/ArrayHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5789 2023-05-29 09:36:19.000000 neworder-1.3.1/src/DataFrame.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-29 09:36:19.000000 neworder-1.3.1/src/DataFrame.h
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Error.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Error.h
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Log.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Model.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Module.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Module_docstr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-05-29 09:36:19.000000 neworder-1.3.1/src/MonteCarlo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-29 09:36:19.000000 neworder-1.3.1/src/MonteCarlo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-29 09:36:19.000000 neworder-1.3.1/src/NPArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 09:36:19.000000 neworder-1.3.1/src/NPArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-29 09:36:19.000000 neworder-1.3.1/src/NewOrder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Timeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Timeline.h
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-29 09:36:19.000000 neworder-1.3.1/src/Timer.h
```

### Comparing `neworder-1.3.0/LICENCE.md` & `neworder-1.3.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/PKG-INFO` & `neworder-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neworder
-Version: 1.3.0
+Version: 1.3.1
 Summary: A dynamic microsimulation framework
 Home-page: https://neworder.readthedocs.io
 Author: Andrew P Smith
 Author-email: andrew@friarswood.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,16 @@
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/neworder/badges/version.svg)](https://anaconda.org/conda-forge/neworder)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/neworder/badges/downloads.svg)](https://anaconda.org/conda-forge/neworder)
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/111997710.svg)](https://zenodo.org/badge/latestdoi/111997710)
 [![status](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9/status.svg)](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9)
 
-[![PyPI build](https://github.com/virgesmith/neworder/actions/workflows/pip-package.yml/badge.svg)]()
-[![Conda build](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
+[![Build and test](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml)
+[![Conda](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
 [![codecov](https://codecov.io/gh/virgesmith/neworder/branch/main/graph/badge.svg?token=g5mDOcjGTD)](https://codecov.io/gh/virgesmith/neworder)
 [![Documentation Status](https://readthedocs.org/projects/neworder/badge/?version=latest)](https://neworder.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/2f3d4cbf0d174b07b527c64b700db77f)](https://www.codacy.com/app/virgesmith/neworder?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/neworder&amp;utm_campaign=Badge_Grade)
 
 [//]: # (!readme!)
 
 *neworder* is a microsimulation framework inspired by [openm++](https://openmpp.org/), [MODGEN](https://www.statcan.gc.ca/eng/microsimulation/modgen/modgen) and, to a lesser extent, the python-based [LIAM2](http://liam2.plan.be/pages/about.html) tool, and can be thought of as a powerful best-of-both-worlds hybrid of MODGEN and LIAM2. Modellers can define their models in a simple, well-known language, yet benefit from the efficiency of compiled code and parallel execution:
@@ -43,20 +43,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
+*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the module will work perfectly well in serial mode without these.
+but the package works perfectly well in serial mode.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -70,16 +70,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +
-docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +local:
+docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
```

### Comparing `neworder-1.3.0/README.md` & `neworder-1.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/neworder/badges/version.svg)](https://anaconda.org/conda-forge/neworder)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/neworder/badges/downloads.svg)](https://anaconda.org/conda-forge/neworder)
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/111997710.svg)](https://zenodo.org/badge/latestdoi/111997710)
 [![status](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9/status.svg)](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9)
 
-[![PyPI build](https://github.com/virgesmith/neworder/actions/workflows/pip-package.yml/badge.svg)]()
-[![Conda build](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
+[![Build and test](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml)
+[![Conda](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
 [![codecov](https://codecov.io/gh/virgesmith/neworder/branch/main/graph/badge.svg?token=g5mDOcjGTD)](https://codecov.io/gh/virgesmith/neworder)
 [![Documentation Status](https://readthedocs.org/projects/neworder/badge/?version=latest)](https://neworder.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/2f3d4cbf0d174b07b527c64b700db77f)](https://www.codacy.com/app/virgesmith/neworder?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/neworder&amp;utm_campaign=Badge_Grade)
 
 [//]: # (!readme!)
 
 *neworder* is a microsimulation framework inspired by [openm++](https://openmpp.org/), [MODGEN](https://www.statcan.gc.ca/eng/microsimulation/modgen/modgen) and, to a lesser extent, the python-based [LIAM2](http://liam2.plan.be/pages/about.html) tool, and can be thought of as a powerful best-of-both-worlds hybrid of MODGEN and LIAM2. Modellers can define their models in a simple, well-known language, yet benefit from the efficiency of compiled code and parallel execution:
@@ -28,20 +28,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
+*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the module will work perfectly well in serial mode without these.
+but the package works perfectly well in serial mode.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -55,16 +55,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +
-docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +local:
+docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
```

### Comparing `neworder-1.3.0/neworder/__init__.pyi` & `neworder-1.3.1/neworder/__init__.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 A dynamic microsimulation framework";
 """
 from __future__ import annotations
-from typing import overload, TypeVar
+import typing
 import datetime
 import numpy as np
+import numpy.typing as npt
 
 import df  # type: ignore
 import mpi # type: ignore
-from .time import *
+from . import time
 import stats # type: ignore
 from .domain import *
-from .graph import *
 
-T = TypeVar("T")
-nparray = np.ndarray[T, np.dtype[T]]
+date_t = datetime.datetime | datetime.date
+FloatArray1d = NPFloatArray | list[float]
+NPIntArray = npt.NDArray[np.int64]
+IntArray1d = NPIntArray | list[int]
+
 
 __all__ = [
     "CalendarTimeline",
     "LinearTimeline",
     "Model",
     "MonteCarlo",
     "NoTimeline",
@@ -32,70 +35,92 @@
     "stats",
     "time",
     "verbose"
 ]
 
 
 class Timeline():
-    pass
-class LinearTimeline(Timeline):
-    """
-    An equally-spaced non-calendar timeline .
-    """
-    @overload
-    def __init__(self, start: float, end: float, nsteps: int) -> None:
-        """
-        Constructs a timeline from start to end, with the given number of steps.
-
-
-        Constructs an open-ended timeline give a start value and a step size. NB the model will run until the Model.halt() method is explicitly called
-        (from inside the step() method). Note also that nsteps() will return -1 for timelines constructed this way
-        """
-    @overload
-    def __init__(self, start: float, step: float) -> None: ...
+    def __init__(self) -> None: ...
     def __repr__(self) -> str:
         """
-        Prints a human-readable representation of the timeline
+        Prints a human-readable representation of the timeline object
         """
+    @property
     def at_end(self) -> bool:
         """
-        Returns True if the current step is the end of the timeline
+            Returns True if the current step is the end of the timeline
+
+        :type: bool
         """
+    @property
     def dt(self) -> float:
         """
-        Returns the step size size of the timeline
+            Returns the step size size of the timeline
+
+        :type: float
         """
+    @property
     def end(self) -> object:
         """
-        Returns the time of the end of the timeline
+            Returns the time of the end of the timeline
+
+        :type: object
         """
+    @property
     def index(self) -> int:
         """
-        Returns the index of the current step in the timeline
+            Returns the index of the current step in the timeline
+
+        :type: int
         """
+    @property
     def nsteps(self) -> int:
         """
-        Returns the number of steps in the timeline (or -1 if open-ended)
+            Returns the number of steps in the timeline (or -1 if open-ended)
+
+        :type: int
         """
+    @property
     def start(self) -> object:
         """
-        Returns the time of the start of the timeline
+            Returns the time of the start of the timeline
+
+        :type: object
         """
+    @property
     def time(self) -> object:
         """
-        Returns the time of the current step in the timeline
+            Returns the time of the current step in the timeline
+
+        :type: object
         """
     pass
+class LinearTimeline(Timeline):
+    """
+    An equally-spaced non-calendar timeline .
+    """
+    @typing.overload
+    def __init__(self, start: float, end: float, nsteps: int) -> None:
+        """
+        Constructs a timeline from start to end, with the given number of steps.
+        """
+    @typing.overload
+    def __init__(self, start: float, step: float) -> None:
+        """
+        Constructs an open-ended timeline give a start value and a step size. NB the model will run until the Model.halt() method is explicitly called
+        (from inside the step() method). Note also that nsteps() will return -1 for timelines constructed this way
+        """
+        pass
 class Model():
     """
     The base model class from which all neworder models should be subclassed
     """
-    def __init__(self, timeline: Timeline, seeder: function) -> None:
+    def __init__(self, timeline: Timeline, seeder: typing.Callable[[int], int] = MonteCarlo.deterministic_independent_stream) -> None:
         """
-        Constructs a model object with a timeline and a seeder function
+        Constructs a model object with a timeline and (optionally) a seeder function for the random stream(s)
         """
     def check(self) -> bool:
         """
         User-overridable method used to check internal state at each timestep.
         Default behaviour is to simply return True.
         Returning False will halt the model run.
         This function should not be called directly, it is used by the Model.run() function
@@ -127,15 +152,15 @@
         This function should not be called directly, it is used by the Model.run() function
         """
     @property
     def mc(self) -> MonteCarlo:
         """
             The model's Monte-Carlo engine
 
-        :type: no::MonteCarlo
+        :type: MonteCarlo
         """
     @property
     def timeline(self) -> Timeline:
         """
             The model's timeline object
 
         :type: Timeline
@@ -145,268 +170,177 @@
     """
     The model's Monte-Carlo engine with configurable options for parallel execution
     """
     def __repr__(self) -> str:
         """
         Prints a human-readable representation of the MonteCarlo engine
         """
-    def arrivals(self, lambda_: nparray[np.float64], dt: float, n: int, mingap: float) -> nparray[np.float64]:
+    def arrivals(self, lambda_: FloatArray1d, dt: float, n: int, mingap: float) -> NPFloatArray:
         """
         Returns an array of n arrays of multiple arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with a minimum separation between events of mingap. Sampling uses the Lewis-Shedler "thinning" algorithm
         The final value of lambda must be zero, and thus arrivals don't always occur, indicated by a value of neworder.time.never()
         The inner dimension of the returned 2d array is governed by the the maximum number of arrivals sampled, and will thus vary
         """
-    def counts(self, lambda_: nparray[np.float64], dt: float) -> nparray[np.int64]:
+    def counts(self, lambda_: FloatArray1d, dt: float) -> NPIntArray:
         """
         Returns an array of simulated arrival counts (within time dt) for each intensity in lambda
         """
     @staticmethod
     def deterministic_identical_stream(r: int) -> int:
         """
         Returns a deterministic seed (19937). Input argument is ignored
         """
     @staticmethod
     def deterministic_independent_stream(r: int) -> int:
         """
         Returns a deterministic seed that is a function of the input (19937+r).
         The model uses the MPI rank as the input argument, allowing for differently seeded streams in each process
         """
-    @overload
-    def first_arrival(self, lambda_: nparray[np.float64], dt: float, n: int) -> nparray[np.float64]:
+    @typing.overload
+    def first_arrival(self, lambda_: FloatArray1d, dt: float, n: int) -> NPFloatArray:
         """
         Returns an array of length n of first arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with a minimum start time of minval. Sampling uses the Lewis-Shedler "thinning" algorithm
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
-
-
+        """
+    @typing.overload
+    def first_arrival(self, lambda_: FloatArray1d, dt: float, n: int, minval: float) -> NPFloatArray:
+        """
         Returns an array of length n of first arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with no minimum start time. Sampling uses the Lewis-Shedler "thinning" algorithm
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
-    @overload
-    def first_arrival(self, lambda_: nparray[np.float64], dt: float, n: int, minval: float) -> nparray[np.float64]: ...
-    @overload
-    def hazard(self, p: float, n: int) -> nparray[np.float64]:
+    @typing.overload
+    def hazard(self, p: float, n: int) -> NPFloatArray:
         """
         Returns an array of ones (with hazard rate lambda) or zeros of length n
-
-
+        """
+    @typing.overload
+    def hazard(self, p: NPFloatArray) -> NPFloatArray:
+        """
         Returns an array of ones (with hazard rate lambda[i]) or zeros for each element in p
         """
-    @overload
-    def hazard(self, p: nparray[np.float64]) -> nparray[np.float64]: ...
-    @overload
-    def next_arrival(self, startingpoints: nparray[np.float64], lambda_: nparray[np.float64], dt: float) -> nparray[np.float64]:
+    @typing.overload
+    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float) -> NPFloatArray:
         """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints with a minimum offset of mingap. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the relative flag is True, then lambda[0] corresponds to start time + mingap, not to absolute time
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
-
-
+        """
+    @typing.overload
+    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float, relative: bool) -> NPFloatArray:
+        """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the relative flag is True, then lambda[0] corresponds to start time, not to absolute time
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
-
-
+        """
+    @typing.overload
+    def next_arrival(self, startingpoints: FloatArray1d, lambda_: FloatArray1d, dt: float, relative: bool, minsep: float) -> NPFloatArray:
+        """
         Returns an array of length n of subsequent arrival times from a nonhomogeneous Poisson process (with hazard rate lambda[i], time interval dt),
         with start times given by startingpoints. Sampling uses the Lewis-Shedler "thinning" algorithm.
         If the final value of lambda is zero, no arrival is indicated by a value of neworder.time.never()
         """
-    @overload
-    def next_arrival(self, startingpoints: nparray[np.float64], lambda_: nparray[np.float64], dt: float, relative: bool) -> nparray[np.float64]: ...
-    @overload
-    def next_arrival(self, startingpoints: nparray[np.float64], lambda_: nparray[np.float64], dt: float, relative: bool, minsep: float) -> nparray[np.float64]: ...
     @staticmethod
     def nondeterministic_stream(r: int) -> int:
         """
         Returns a random seed from the platform's random_device. Input argument is ignored
         """
     def raw(self) -> int:
         """
         Returns a random 64-bit unsigned integer. Useful for seeding other generators.
         """
     def reset(self) -> None:
         """
         Resets the generator using the original seed.
         Use with care, esp in multi-process models with identical streams
         """
-    def sample(self, n: int, cat_weights: nparray[np.float64]) -> nparray[np.int64]:
+    def sample(self, n: int, cat_weights: NPFloatArray) -> NPIntArray:
         """
         Returns an array of length n containing randomly sampled categorical values, weighted according to cat_weights
         """
     def seed(self) -> int:
         """
         Returns the seed used to initialise the random stream
         """
     def state(self) -> int:
         """
         Returns a hash of the internal state of the generator. Avoids the extra complexity of tranmitting variable-length strings over MPI.
         """
-    @overload
-    def stopping(self, lambda_: float, n: int) -> nparray[np.float64]:
+    @typing.overload
+    def stopping(self, lambda_: float, n: int) -> NPFloatArray:
         """
         Returns an array of stopping times (with hazard rate lambda) of length n
-
-
+        """
+    @typing.overload
+    def stopping(self, lambda_: NPFloatArray) -> NPFloatArray:
+        """
         Returns an array of stopping times (with hazard rate lambda[i]) for each element in lambda
         """
-    @overload
-    def stopping(self, lambda_: nparray[np.float64]) -> nparray[np.float64]: ...
-    def ustream(self, n: int) -> nparray[np.float64]:
+    def ustream(self, n: int) -> NPFloatArray:
         """
         Returns an array of uniform random [0,1) variates of length n
         """
     pass
 class NoTimeline(Timeline):
     """
     An arbitrary one step timeline, for continuous-time models with no explicit (discrete) timeline
     """
     def __init__(self) -> None:
         """
         Constructs an arbitrary one step timeline, where the start and end times are undefined and there is a single step of size zero. Useful for continuous-time models
         """
-    def __repr__(self) -> str:
-        """
-        Prints a human-readable representation of the timeline
-        """
-    def at_end(self) -> bool:
-        """
-        Returns True if the current step is the end of the timeline
-        """
-    def dt(self) -> float:
-        """
-        Returns the step size size of the timeline
-        """
-    def end(self) -> object:
-        """
-        Returns the time of the end of the timeline
-        """
-    def index(self) -> int:
-        """
-        Returns the index of the current step in the timeline
-        """
-    def nsteps(self) -> int:
-        """
-        Returns the number of steps in the timeline (or -1 if open-ended)
-        """
-    def start(self) -> object:
-        """
-        Returns the time of the start of the timeline
-        """
-    def time(self) -> object:
-        """
-        Returns the time of the current step in the timeline
-        """
     pass
 class NumericTimeline(Timeline):
     """
     An custom non-calendar timeline where the user explicitly specifies the time points, which must be monotonically increasing.
     """
-    def __init__(self, times: list[float]) -> None:
+    def __init__(self, times: typing.List[float]) -> None:
         """
         Constructs a timeline from an array of time points.
         """
-    def __repr__(self) -> str:
-        """
-        Prints a human-readable representation of the timeline
-        """
-    def at_end(self) -> bool:
-        """
-        Returns True if the current step is the end of the timeline
-        """
-    def dt(self) -> float:
-        """
-        Returns the step size size of the timeline
-        """
-    def end(self) -> object:
-        """
-        Returns the time of the end of the timeline
-        """
-    def index(self) -> int:
-        """
-        Returns the index of the current step in the timeline
-        """
-    def nsteps(self) -> int:
-        """
-        Returns the number of steps in the timeline (or -1 if open-ended)
-        """
-    def start(self) -> object:
-        """
-        Returns the time of the start of the timeline
-        """
-    def time(self) -> object:
-        """
-        Returns the time of the current step in the timeline
-        """
     pass
 class CalendarTimeline(Timeline):
     """
     A calendar-based timeline
     """
-    @overload
-    def __init__(self, start: datetime.datetime, end: datetime.datetime, step: int, unit: str) -> None:
+    @typing.overload
+    def __init__(self, start: date_t, end: date_t, step: int, unit: str) -> None:
         """
         Constructs a calendar-based timeline, given start and end dates, an increment specified as a multiple of days, months or years
-
-
+        """
+    @typing.overload
+    def __init__(self, start: date_t, step: int, unit: str) -> None:
+        """
         Constructs an open-ended calendar-based timeline, given a start date and an increment specified as a multiple of days, months or years.
          NB the model will run until the Model.halt() method is explicitly called (from inside the step() method). Note also that nsteps() will
          return -1 for timelines constructed this way
         """
-    @overload
-    def __init__(self, start: datetime.datetime, step: int, unit: str) -> None: ...
-    def __repr__(self) -> str:
-        """
-        Prints a human-readable representation of the timeline
-        """
-    def at_end(self) -> bool:
-        """
-        Returns True if the current step is the end of the timeline
-        """
-    def dt(self) -> float:
-        """
-        Returns the step size size of the timeline
-        """
-    def end(self) -> object:
-        """
-        Returns the time of the end of the timeline
-        """
-    def index(self) -> int:
-        """
-        Returns the index of the current step in the timeline
-        """
-    def nsteps(self) -> int:
-        """
-        Returns the number of steps in the timeline (or -1 if open-ended)
-        """
-    def start(self) -> object:
-        """
-        Returns the time of the start of the timeline
-        """
-    def time(self) -> object:
-        """
-        Returns the time of the current step in the timeline
-        """
     pass
 def checked(checked: bool = True) -> None:
     """
     Sets the checked flag, which determines whether the model runs checks during execution
     """
 def log(obj: object) -> None:
     """
     The logging function. Prints obj to the console, annotated with process information
     """
-def run(model: object) -> bool:
+def run(model: Model) -> bool:
     """
     Runs the model. If the model has previously run it will resume from the point at which it was given the "halt" instruction. This is useful
     for external processing of model data, and/or feedback from external sources. If the model has already reached the end of the timeline, this
     function will have no effect. To re-run the model from the start, you must construct a new model object.
     Returns:
         True if model succeeded, False otherwise
     """
 def verbose(verbose: bool = True) -> None:
     """
     Sets the verbose flag, which toggles detailed runtime logs
     """
+
+def as_np(mc: MonteCarlo) -> np.random.Generator:
+  """
+  Returns an adapter enabling the MonteCarlo object to be used with numpy random functionality
+  """
```

### Comparing `neworder-1.3.0/neworder/df.pyi` & `neworder-1.3.1/neworder/df.pyi`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/neworder/domain.py` & `neworder-1.3.1/neworder/domain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Spatial structures for positioning and moving entities and computing distances
 """
 
 from __future__ import annotations
-from typing import Union, Optional, Any, Callable
+from typing import Union, Optional, Any, Callable, TypeVar
 from enum import Enum, auto
 import numpy as np
+import numpy.typing as npt
 from scipy import signal  # type: ignore
 
+NPFloatArray = npt.NDArray[np.float64]
+
 class Edge(Enum):
   """
   Edge behaviour
   """
   UNBOUNDED = auto()
   WRAP = auto()
   CONSTRAIN = auto()
@@ -53,35 +56,35 @@
 
   @staticmethod
   def unbounded(dim: int) -> Space:
     """ Construct an unbounded Space """
     assert dim > 0
     return Space(np.full(dim, -np.inf), np.full(dim, +np.inf), edge=Edge.UNBOUNDED)
 
-  def __init__(self, min: np.ndarray, max: np.ndarray, edge: Edge=Edge.CONSTRAIN):
+  def __init__(self, min: NPFloatArray, max: NPFloatArray, edge: Edge=Edge.CONSTRAIN):
     assert len(min) and len(min) == len(max)
     super().__init__(len(min), edge, True)
 
     # Space supports all edge behaviours
     assert edge in [Edge.UNBOUNDED, Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]
 
     assert np.all(max > min)
 
     self.min = min
     self.max = max
 
   @property
-  def extent(self) -> tuple[np.ndarray, np.ndarray]:
+  def extent(self) -> tuple[NPFloatArray, NPFloatArray]:
     """ The extent of the space in terms of two opposing points """
     return self.min, self.max
 
   def move(self, positions: Any,
                  velocities: Any,
                  delta_t: float,
-                 ungroup: bool=False) -> tuple[np.ndarray, np.ndarray]:
+                 ungroup: bool=False) -> tuple[NPFloatArray, NPFloatArray]:
     """ Returns translated positions AND velocities """
     # group tuples into a single array if necessary
     if isinstance(positions, tuple):
       positions = np.column_stack(positions)
     if isinstance(velocities, tuple):
       velocities = np.column_stack(velocities)
 
@@ -114,15 +117,15 @@
       v = velocities
 
     if ungroup:
       p = np.split(p, self.dim, axis=1)
       v = np.split(v, self.dim, axis=1)
     return p, v
 
-  def dists2(self, positions: Union[tuple[np.ndarray, ...], np.ndarray], to_points: Optional[np.ndarray]=None) -> tuple[np.ndarray, Any]:
+  def dists2(self, positions: Union[tuple[NPFloatArray, ...], NPFloatArray], to_points: Optional[NPFloatArray]=None) -> tuple[NPFloatArray, Any]:
     """ The squared distance between points and separations along each axis """
     # group tuples into a single array if necessary
     if isinstance(positions, tuple):
       positions = np.column_stack(positions)
     if isinstance(to_points, tuple):
       to_points = np.column_stack(to_points)
     # distances w.r.t. self if to_points not explicitly specified
@@ -147,69 +150,96 @@
         delta = np.where(delta > r / 2, delta - r, delta)
         delta = np.where(delta < -r / 2, delta + r, delta)
         separations += (delta,)
         d2 += delta * delta
 
     return d2, separations
 
-  def dists(self, positions: Union[tuple[np.ndarray, ...], np.ndarray], to_points: Optional[np.ndarray]=None) -> np.ndarray:
+  def dists(self, positions: Union[tuple[NPFloatArray, ...], NPFloatArray], to_points: Optional[NPFloatArray]=None) -> NPFloatArray:
     """ Returns distances between the points"""
     return np.sqrt(self.dists2(positions, to_points)[0])
 
-  def in_range(self, distance: Any, positions: Any, count: Optional[bool]=False) -> np.ndarray:
+  def in_range(self, distance: Any, positions: Any, count: Optional[bool]=False) -> NPFloatArray:
     """ Returns either indices or counts of points within the specified distance from each point """
     ind = np.where(self.dists2(positions)[0] < distance * distance, 1, 0)
     # fill diagonal so as not to include self - TODO how does this work if to_points!=positions
     np.fill_diagonal(ind, 0)
     return ind if not count else np.sum(ind, axis=1)
 
   def __repr__(self) -> str:
     return "%s dim=%d min=%s max=%s edge=%s" % (self.__class__.__name__, self.dim, self.min, self.max, self.edge)
 
+def _bounce(i: int, N: int) -> int:
+  s = (i // N) % 2
+  k = i % N
+  return N * s + (-1) ** s * k
 
 class StateGrid(Domain):
   """
   Discrete rectangular n-dimensional finite grid domain with each cell having an integer state.
   Allows for counting of neighbours according to the supported edge behaviours:
     CONSTRAIN (no neighburs over edge), WRAP (toroidal), BOUNCE (reflect)
   """
 
   __mode_lookup: dict[Edge, str] = {
     Edge.CONSTRAIN: "constant",
     Edge.WRAP: "wrap",
     Edge.BOUNCE: "reflect"
   }
 
-  def __init__(self, initial_values: np.ndarray, edge: Edge=Edge.CONSTRAIN):
+  def __init__(self, initial_values: NPFloatArray, edge: Edge=Edge.CONSTRAIN):
     super().__init__(initial_values.ndim, edge, False)
 
     # StateGrid supports two edge behaviours
-    if edge not in [Edge.WRAP, Edge.CONSTRAIN]:
-      raise ValueError("edge policy must be one of Edge.WRAP, Edge.CONSTRAIN")
+    if edge not in [Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE]:
+      raise ValueError("edge policy must be one of Edge.WRAP, Edge.CONSTRAIN, Edge.BOUNCE")
 
     if initial_values.ndim < 1:
       raise ValueError("state array must have dimension of 1 or above")
     if initial_values.size < 1:
       raise ValueError("state array must have size of 1 or above in every dimension")
 
     self.state = initial_values
 
     # int neighbour kernel (not including self)
     self.kernel = np.ones([3] * self.dim)
     self.kernel[(1,) * self.dim] = 0
 
+  def __get_point(self, p: tuple[int, ...]) -> tuple[int, ...]:
+    assert len(p) == self.state.ndim, f"dimensionality mismatch: {len(p)} but grid has {self.state.ndim}"
+    match self.edge:
+      case Edge.WRAP:
+        p = tuple(p[i] % self.state.shape[i] for i in range(len(p)))
+      case Edge.CONSTRAIN:
+        p = tuple(np.clip(p[i], 0, self.state.shape[i] - 1) for i in range(len(p)))
+      case Edge.BOUNCE:
+        p = tuple(_bounce(p[i], self.state.shape[i] - 1) for i in range(len(p)))
+    return p
+
+  def __getitem__(self, p: tuple[int, ...]) -> Any:
+    return self.state[self.__get_point(p)]
+
+  def __setitem__(self, p: tuple[int, ...], value: Any) -> None:
+    self.state[self.__get_point(p)] = value
+
+  def shift(self, position: tuple[int, ...], delta: tuple[int, ...]) -> tuple[int, ...]:
+    """This translates a point according to the grid's edge behaviour. It does *not* change any state"""
+    point = self.__get_point(position)
+    p = tuple(point[i] + delta[i] for i in range(self.dim))
+    return self.__get_point(p)
+
   @property
   def extent(self) -> Any:
     """ The extent of the space in terms of two opposing points """
     return self.state.shape
 
-  def count_neighbours(self, indicator: Callable[[float], bool]=lambda x: x == 1) -> np.ndarray:
+  def count_neighbours(self, indicator: Callable[[float], bool]=lambda x: x == 1) -> NPFloatArray:
     """ Counts neighbouring cells with a state indicated by supplied indicator function """
 
-    ind: np.ndarray = np.array([indicator(x) for x in self.state]).astype(int)  # automagically preserves shape
+    ind: NPFloatArray = np.array([indicator(x) for x in self.state]).astype(int)  # automagically preserves shape
     # pad with boundary according to edge policy
     bounded = np.pad(ind, pad_width=1, mode=self.__mode_lookup[self.edge])  # type: ignore # bug?
 
     # count neighbours, drop padding, covert to int
     count = signal.convolve(bounded, self.kernel, mode="same", method="direct")[(slice(1, -1),) * self.dim].astype(int)
 
     return count
```

### Comparing `neworder-1.3.0/neworder/stats.pyi` & `neworder-1.3.1/neworder/stats.pyi`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/neworder/time.pyi` & `neworder-1.3.1/neworder/time.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
     Temporal values and comparison
 """
 from __future__ import annotations
-from typing import overload, TypeVar
+import typing
 import numpy as np
-
-T = TypeVar("T")
-nparray = np.ndarray[T, np.dtype[T]]
-
+import numpy.typing as npt
 
 __all__ = [
     "distant_past",
     "far_future",
     "isnever",
     "never"
 ]
@@ -21,24 +18,23 @@
     """
     Returns a value that compares less than any other value but itself and "never"
     """
 def far_future() -> float:
     """
     Returns a value that compares greater than any other value but itself and "never"
     """
-@overload
+@typing.overload
 def isnever(t: float) -> bool:
     """
     Returns whether the value of t corresponds to "never". As "never" is implemented as a floating-point NaN,
     direct comparison will always fail, since NaN != NaN.
-
-
+    """
+@typing.overload
+def isnever(t: npt.NDArray[np.float64] | list[float]) -> npt.NDArray[np.bool8]:
+    """
     Returns an array of booleans corresponding to whether the element of an array correspond to "never". As "never" is
     implemented as a floating-point NaN, direct comparison will always fails, since NaN != NaN.
     """
-@overload
-def isnever(t: nparray[np.float64]) -> nparray[np.bool8]:
-    pass
 def never() -> float:
     """
-    Returns a value that compares unequal to any value, including but itself.
+    Returns a value that compares unequal to any value, including itself.
     """
```

### Comparing `neworder-1.3.0/neworder.egg-info/PKG-INFO` & `neworder-1.3.1/neworder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neworder
-Version: 1.3.0
+Version: 1.3.1
 Summary: A dynamic microsimulation framework
 Home-page: https://neworder.readthedocs.io
 Author: Andrew P Smith
 Author-email: andrew@friarswood.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -21,16 +21,16 @@
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/neworder/badges/version.svg)](https://anaconda.org/conda-forge/neworder)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/neworder/badges/downloads.svg)](https://anaconda.org/conda-forge/neworder)
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/111997710.svg)](https://zenodo.org/badge/latestdoi/111997710)
 [![status](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9/status.svg)](https://joss.theoj.org/papers/4b7cc8402819ff48fc7403c0e9a265e9)
 
-[![PyPI build](https://github.com/virgesmith/neworder/actions/workflows/pip-package.yml/badge.svg)]()
-[![Conda build](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
+[![Build and test](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/build-test.yml)
+[![Conda](https://github.com/virgesmith/neworder/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/neworder/actions/workflows/conda.yml)
 [![codecov](https://codecov.io/gh/virgesmith/neworder/branch/main/graph/badge.svg?token=g5mDOcjGTD)](https://codecov.io/gh/virgesmith/neworder)
 [![Documentation Status](https://readthedocs.org/projects/neworder/badge/?version=latest)](https://neworder.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/2f3d4cbf0d174b07b527c64b700db77f)](https://www.codacy.com/app/virgesmith/neworder?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/neworder&amp;utm_campaign=Badge_Grade)
 
 [//]: # (!readme!)
 
 *neworder* is a microsimulation framework inspired by [openm++](https://openmpp.org/), [MODGEN](https://www.statcan.gc.ca/eng/microsimulation/modgen/modgen) and, to a lesser extent, the python-based [LIAM2](http://liam2.plan.be/pages/about.html) tool, and can be thought of as a powerful best-of-both-worlds hybrid of MODGEN and LIAM2. Modellers can define their models in a simple, well-known language, yet benefit from the efficiency of compiled code and parallel execution:
@@ -43,20 +43,20 @@
 - **reproducibility**: built-in, customisable random generator seeding strategies
 - **speed**: the module is predominantly written in optimised C++ and provides fast Monte-Carlo, statistical and data manipulation functions.
 - **compatibility**: operate directly on *numpy* arrays and *pandas* DataFrames
 - **scalability**: can be run on a desktop or a HPC cluster, supporting parallel execution using MPI.
 
 ## System Requirements
 
-*neworder* requires python 3.6 or above and runs on 64-bit linux, OSX and Windows platforms. In order to take advantage of the parallel execution functionality, the following are also required:
+*neworder* requires python 3.10 or above and runs on 64-bit linux, OSX and Windows platforms. To take advantage of the  parallel execution functionality, you may also need to install:
 
 - an MPI implementation, such as [mpich](https://www.mpich.org/), [open-mpi](https://www.open-mpi.org/) or [ms-mpi](https://docs.microsoft.com/en-us/message-passing-interface/microsoft-mpi)
 - the [mpi4py](https://mpi4py.readthedocs.io/en/stable/) package that provides python MPI bindings
 
-but the module will work perfectly well in serial mode without these.
+but the package works perfectly well in serial mode.
 
 ## Installation
 
 ### PyPI
 
 ```bash
 pip install neworder
@@ -70,16 +70,16 @@
 
 ### Docker
 
 The docker image contains all the examples, and should be run interactively. Some of the examples require permission to connect to the host's graphical display.
 
 ```bash
 docker pull virgesmith/neworder
-xhost +
-docker run -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
+xhost +local:
+docker run --net=host -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY -it virgesmith/neworder
 ```
 
 NB The above works on ubuntu but may require modification on other OSs.
 
 Then in the container, e.g.
 
 ```bash
```

### Comparing `neworder-1.3.0/neworder.egg-info/SOURCES.txt` & `neworder-1.3.1/neworder.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 neworder/__init__.py
 neworder/__init__.pyi
 neworder/df.pyi
 neworder/domain.py
-neworder/graph.py
 neworder/mc.py
 neworder/mpi.pyi
 neworder/py.typed
 neworder/stats.pyi
 neworder/time.pyi
 neworder.egg-info/PKG-INFO
 neworder.egg-info/SOURCES.txt
@@ -21,14 +20,15 @@
 neworder.egg-info/requires.txt
 neworder.egg-info/top_level.txt
 src/ArrayHelpers.h
 src/DataFrame.cpp
 src/DataFrame.h
 src/Error.cpp
 src/Error.h
+src/Helpers.h
 src/Log.cpp
 src/Log.h
 src/Model.cpp
 src/Model.h
 src/Module.cpp
 src/Module.h
 src/Module_docstr.cpp
```

### Comparing `neworder-1.3.0/setup.py` & `neworder-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
   url='https://neworder.readthedocs.io',
   description='A dynamic microsimulation framework',
   long_description=readme(),
   long_description_content_type="text/markdown",
   packages=["neworder"],
   package_data={"neworder": ["py.typed", "*.pyi"]},
   ext_modules=ext_modules,
-  install_requires=['pandas>=1.0.5', 'scipy', 'networkx', 'osmnx', 'geopandas'],
+  install_requires=['pandas>=1.0.5', 'pandas-stubs', 'scipy'],
   setup_requires=['pybind11>=2.5.0', 'pytest-runner', 'numpy>=1.19.1'],
   tests_require=['pytest', 'mpi4py>=3.0.3'],
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
```

### Comparing `neworder-1.3.0/src/ArrayHelpers.h` & `neworder-1.3.1/src/ArrayHelpers.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/DataFrame.cpp` & `neworder-1.3.1/src/DataFrame.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/DataFrame.h` & `neworder-1.3.1/src/DataFrame.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/Error.h` & `neworder-1.3.1/src/Error.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/Log.cpp` & `neworder-1.3.1/src/Log.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 
 #include "Log.h"
 #include "Module.h"
 
+std::string std::to_string(char c)
+{
+  return std::string(1, c);
+}
 
 std::string std::to_string(const std::string& v)
 {
   return v;
 }
 
 std::string std::to_string(const py::object& o)
```

### Comparing `neworder-1.3.0/src/Log.h` & `neworder-1.3.1/src/Log.h`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 //#include <chrono>
 #include <iomanip>
 
 using namespace std::string_literals;
 
 namespace std
 {
+// forces char to be printed (rather than number)
+std::string to_string(char c);
+
 std::string to_string(const std::string& str);
 
 std::string to_string(const py::object& o);
 
 template<typename T>
 std::string to_string(const std::vector<T>& v)
 {
```

### Comparing `neworder-1.3.0/src/Model.cpp` & `neworder-1.3.1/src/Model.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 #include "Model.h"
 #include "NewOrder.h"
 #include "Timeline.h"
 #include "Module.h"
 #include "Timer.h"
 #include "Log.h"
 #include "Error.h"
+#include "Helpers.h"
 
 #include <pybind11/pybind11.h>
 
-// take a copy of the (const) timeline and clone it (original object may get deleted)
-no::Model::Model(const Timeline& timeline, const py::function& seeder)
-  : m_timeline(timeline.clone()), m_monteCarlo(seeder(no::env::rank.load(std::memory_order_relaxed)).cast<int32_t>())
+no::Model::Model(no::Timeline& timeline, const py::function& seeder)
+  : m_timeline(timeline), m_timeline_handle(py::cast(&timeline)),
+  m_monteCarlo(seeder(no::env::rank.load(std::memory_order_relaxed)).cast<int32_t>())
 {
-  no::log("model init: timeline=%% mc=%%"s % m_timeline->repr() % m_monteCarlo.repr());
+  no::log("model init: timeline=%% mc=%%"s % m_timeline.repr() % m_monteCarlo.repr());
 }
 
 
 void no::Model::modify(int)
 {
   // verbose only
   no::log("defaulted to no-op Model::modify()");
 }
 
-void no::Model::step()
-{
-  PYBIND11_OVERLOAD_PURE(void, Model, step);
-}
-
 void no::Model::halt()
 {
   no::log("sending halt signal to Model::run()");
   no::env::halt = true;
 }
 
 bool no::Model::check()
@@ -43,74 +39,74 @@
 void no::Model::finalise()
 {
   // verbose only
   no::log("defaulted to no-op Model::finalise()");
 }
 
 
-bool no::Model::run(py::object& model_subclass)
+bool no::Model::run(Model& model)
 {
-  // extract the base class
-  no::Model& base = model_subclass.cast<no::Model&>();
   Timer timer;
-
   int rank = no::env::rank.load(std::memory_order_relaxed);
-
   if (rank < 0)
   {
     throw std::runtime_error("environment is not correctly initialised, model will not be run");
   }
 
-  const std::string& subclass_name = py::str(model_subclass).cast<std::string>();
+  // access the timeline properties via the python object for consistency
+  // (we can use the methods for C++ implementations, but not for python implementations)
+  auto pytimeline = PyAccessor(model.timeline());
+
+  // get the Model class name
+  const std::string& model_name = py::cast(&model).attr("__class__").attr("__name__").cast<std::string>();
 
-  no::log("starting model run. start time=%%"s % base.timeline().start());
+  no::log("starting %% model run. start time=%%"s % model_name % pytimeline.get("start"));
 
   // apply the modifier, if implemented in the derived class
-  no::log("t=%%(%%) %%.modify(%%)"s % base.timeline().time() % base.timeline().index() % subclass_name % rank);
-  model_subclass.attr("modify")(rank);
+  no::log("t=%%(%%) %%.modify(%%)"s % pytimeline.get("time") % pytimeline.get("index") % model_name % rank);
+  model.modify(rank);
 
   // Loop over timeline
   bool ok = true;
-  while (!base.timeline().at_end())
+  while (!pytimeline.get_as<bool>("at_end"))
   {
-    py::object t = base.timeline().time();
-    size_t timeindex = base.timeline().index();
+    py::object t = pytimeline.get("time");
+    int64_t timeindex = pytimeline.get_as<int64_t>("index");
 
-    // call the step method, then incement the timeline
-    no::log("t=%%(%%) %%.step()"s % t % timeindex % subclass_name);
-    model_subclass.attr("step")();
+    // call the step method, then increment the timeline
+    no::log("t=%%(%%) %%.step()"s % t % timeindex % model_name);
+    model.step();
 
-    base.timeline().next();
+    model.timeline().next();
 
     // call the check method and stop if necessary
     if (no::env::checked)
     {
-      ok = model_subclass.attr("check")().cast<bool>();
-      no::log("t=%%(%%) %%.check(): %%"s % t % timeindex % subclass_name % (ok? "ok": "FAILED"));
+      ok = model.check();
+      no::log("t=%%(%%) %%.check(): %%"s % t % timeindex % model_name % (ok? "ok": "FAILED"));
       if (!ok)
       {
         // emit warning as well on failure (since the above message only appears when verbose mode is on)
-        no::warn("check() FAILED in %%, halting model run at t=%%(%%)"s % subclass_name % t % timeindex);
+        no::warn("check() FAILED in %%, halting model run at t=%%(%%)"s % model_name % t % timeindex);
         break;
       }
     }
 
     // check python hasn't signalled early termination
     if (no::env::halt)
     {
       no::log("t=%%(%%) received halt signal"s % t % timeindex);
       // reset the flag so that subsequent model runs don't halt immediately
       no::env::halt = false;
       break;
     }
   }
   // call the finalise method (if not explicitly halted mid-timeline)
-  if (base.timeline().at_end())
+  if (pytimeline.get_as<bool>("at_end"))
   {
-    no::log("t=%%(%%) %%.finalise()"s % base.timeline().time() % base.timeline().index() % subclass_name );
-    model_subclass.attr("finalise")();
-    no::log("%% exec time=%%s"s % (ok ? "SUCCESS": "ERRORED") % timer.elapsed_s());
+    no::log("t=%%(%%) %%.finalise()"s % pytimeline.get("time") % pytimeline.get("index") % model_name );
+    model.finalise();
   }
+  no::log("%% exec time=%%s"s % (ok ? "SUCCESS": "ERRORED") % timer.elapsed_s());
   return ok;
 }
 
-
```

### Comparing `neworder-1.3.0/src/Module.cpp` & `neworder-1.3.1/src/Module.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -48,106 +48,64 @@
   int r = no::env::rank.load(std::memory_order_relaxed);
   int s = no::env::size.load(std::memory_order_relaxed);
   no::env::logPrefix[no::env::Context::CPP] = "[no %%/%%]"s % r % s;
   no::env::logPrefix[no::env::Context::PY] = "[py %%/%%]"s % r % s;
 }
 
 
+
 // python-visible log function defined above
 PYBIND11_MODULE(_neworder_core, m)
 {
   // py::options options;
   // options.disable_function_signatures();
 #include "Module_docstr.cpp"
 
   m.doc() = module_docstr;
 
-  // model control plus utility/diagnostics
-
-  m.def("log", log_obj, log_docstr, "obj"_a)
-   .def("run", no::Model::run, run_docstr, "model"_a)
-   .def("verbose", [](bool v = true) { no::env::verbose.store(v, std::memory_order_relaxed); }, verbose_docstr, "verbose"_a = true)
-   .def("checked", [](bool c = true) { no::env::checked.store(c, std::memory_order_relaxed); }, checked_docstr, "checked"_a = true);
-
   // time-related module
-
   m.def_submodule("time", time_docstr)
     .def("distant_past", no::time::distant_past, time_distant_past_docstr)
     .def("far_future", no::time::far_future, time_far_future_docstr)
     .def("never", no::time::never, time_never_docstr)
     .def("isnever", no::time::isnever, time_isnever_docstr, "t"_a) // scalar
     .def("isnever", no::time::isnever_a, time_isnever_a_docstr, "t"_a); // array
 
   // register abstract base class
-  py::class_<no::Timeline>(m, "Timeline");
+  py::class_<no::Timeline, no::PyTimeline>(m, "Timeline")
+    .def(py::init<>())
+    .def_property_readonly("time", &no::Timeline::time, timeline_time_docstr)
+    .def_property_readonly("start", &no::Timeline::start, timeline_start_docstr)
+    .def_property_readonly("end", &no::Timeline::end, timeline_end_docstr)
+    .def_property_readonly("index", &no::Timeline::index, timeline_index_docstr)
+    .def_property_readonly("nsteps", &no::Timeline::nsteps, timeline_nsteps_docstr)
+    .def_property_readonly("dt", &no::Timeline::dt, timeline_dt_docstr)
+    .def_property_readonly("at_end", &no::Timeline::at_end, timeline_at_end_docstr)
+    .def("__repr__", &no::Timeline::repr, timeline_repr_docstr)
+    ;
 
   py::class_<no::NoTimeline, no::Timeline>(m, "NoTimeline", notimeline_docstr)
-    .def(py::init<>(), notimeline_init_docstr)
-    .def("start", &no::NoTimeline::start, timeline_start_docstr)
-    .def("end", &no::NoTimeline::end, timeline_end_docstr)
-    .def("index", &no::NoTimeline::index, timeline_index_docstr)
-    .def("time", &no::NoTimeline::time, timeline_time_docstr)
-    .def("dt", &no::NoTimeline::dt, timeline_dt_docstr)
-    .def("nsteps", &no::NoTimeline::nsteps, timeline_nsteps_docstr)
-    .def("at_end", &no::NoTimeline::at_end, timeline_at_end_docstr)
-    .def("__repr__", &no::NoTimeline::repr, timeline_repr_docstr);
+    .def(py::init<>(), notimeline_init_docstr);
 
   py::class_<no::LinearTimeline, no::Timeline>(m, "LinearTimeline", lineartimeline_docstr)
     .def(py::init<double, double, size_t>(), lineartimeline_init_docstr, "start"_a, "end"_a, "nsteps"_a)
-    .def(py::init<double, double>(), lineartimeline_init_open_docstr, "start"_a, "step"_a)
-    .def("start", &no::LinearTimeline::start, timeline_start_docstr)
-    .def("end", &no::LinearTimeline::end, timeline_end_docstr)
-    .def("index", &no::LinearTimeline::index, timeline_index_docstr)
-    .def("time", &no::LinearTimeline::time, timeline_time_docstr)
-    .def("dt", &no::LinearTimeline::dt, timeline_dt_docstr)
-    .def("nsteps", &no::LinearTimeline::nsteps, timeline_nsteps_docstr)
-    .def("at_end", &no::LinearTimeline::at_end, timeline_at_end_docstr)
-    .def("__repr__", &no::LinearTimeline::repr, timeline_repr_docstr);
+    .def(py::init<double, double>(), lineartimeline_init_open_docstr, "start"_a, "step"_a);
 
   py::class_<no::NumericTimeline, no::Timeline>(m, "NumericTimeline", numerictimeline_docstr)
-    .def(py::init<const std::vector<double>&>(), numerictimeline_init_docstr, "times"_a)
-    .def("start", &no::NumericTimeline::start, timeline_start_docstr)
-    .def("end", &no::NumericTimeline::end, timeline_end_docstr)
-    .def("index", &no::NumericTimeline::index, timeline_index_docstr)
-    .def("time", &no::NumericTimeline::time, timeline_time_docstr)
-    .def("dt", &no::NumericTimeline::dt, timeline_dt_docstr)
-    .def("nsteps", &no::NumericTimeline::nsteps, timeline_nsteps_docstr)
-    .def("at_end", &no::NumericTimeline::at_end, timeline_at_end_docstr)
-    .def("__repr__", &no::NumericTimeline::repr, timeline_repr_docstr);
+    .def(py::init<const std::vector<double>&>(), numerictimeline_init_docstr, "times"_a);
 
   py::class_<no::CalendarTimeline, no::Timeline>(m, "CalendarTimeline", calendartimeline_docstr)
     .def(py::init<std::chrono::system_clock::time_point, std::chrono::system_clock::time_point, size_t, char>(),
       calendartimeline_init_docstr, "start"_a, "end"_a, "step"_a, "unit"_a)
     .def(py::init<std::chrono::system_clock::time_point, size_t, char>(),
-      calendartimeline_init_open_docstr, "start"_a, "step"_a, "unit"_a)
-    .def("start", &no::CalendarTimeline::start, timeline_start_docstr)
-    .def("end", &no::CalendarTimeline::end, timeline_end_docstr)
-    .def("index", &no::CalendarTimeline::index, timeline_index_docstr)
-    .def("time", &no::CalendarTimeline::time, timeline_time_docstr)
-    .def("dt", &no::CalendarTimeline::dt, timeline_dt_docstr)
-    .def("nsteps", &no::CalendarTimeline::nsteps, timeline_nsteps_docstr)
-    .def("at_end", &no::CalendarTimeline::at_end, timeline_at_end_docstr)
-    .def("__repr__", &no::CalendarTimeline::repr, timeline_repr_docstr);
-
-  // Microsimulation (or ABM) model class
-  py::class_<no::Model>(m, "Model", model_docstr)
-    .def(py::init<no::Timeline&, const py::function&>(), model_init_docstr,"timeline"_a, "seeder"_a)
-    // properties are readonly only in the sense you can't assign to them; you CAN call their mutable methods
-    .def_property_readonly("timeline", &no::Model::timeline, model_timeline_docstr)
-    .def_property_readonly("mc", &no::Model::mc, model_mc_docstr)
-    .def("modify", &no::Model::modify, model_modify_docstr, "r"_a)
-    .def("step", &no::Model::step, model_step_docstr)
-    .def("check", &no::Model::check, model_check_docstr)
-    .def("finalise", &no::Model::finalise, model_finalise_docstr)
-    .def("halt", &no::Model::halt, model_halt_docstr);
-    // NB the all-important run function is not exposed to python, it can only be executed via the `neworder.run` function
+      calendartimeline_init_open_docstr, "start"_a, "step"_a, "unit"_a);
 
   // MC
   py::class_<no::MonteCarlo>(m, "MonteCarlo", mc_docstr)
-    // constructor is NOT exposed to python, can only be created withing a model
+    // constructor is NOT exposed to python, can only be created within a model
     .def_static("deterministic_identical_stream", &no::MonteCarlo::deterministic_identical_stream, mc_deterministic_identical_stream_docstr, "r"_a)
     .def_static("deterministic_independent_stream", &no::MonteCarlo::deterministic_independent_stream, mc_deterministic_independent_stream_docstr, "r"_a)
     .def_static("nondeterministic_stream", &no::MonteCarlo::nondeterministic_stream, mc_nondeterministic_stream_docstr, "r"_a)
     .def("init_bitgen", &no::MonteCarlo::init_bitgen, "internal helper function used by as_np")
     .def("seed", &no::MonteCarlo::seed, mc_seed_docstr)
     .def("reset", &no::MonteCarlo::reset, mc_reset_docstr)
     .def("state", &no::MonteCarlo::state, mc_state_docstr)
@@ -192,17 +150,27 @@
     .def("next_arrival", [](no::MonteCarlo& self, const py::array_t<double>& startingpoints, const py::array_t<double>& lambda_t, double dt) {
                            return self.next_arrival(startingpoints, lambda_t, dt, false, 0.0);
                          },
                          mc_next_arrival3_docstr,
                          "startingpoints"_a, "lambda_"_a, "dt"_a)
     .def("__repr__", &no::MonteCarlo::repr, mc_repr_docstr);
 
-    // .def("first_arrival", [](no::MonteCarlo& mc, const py::array_t<double>& lambda_t, double dt, size_t n) {
-    //   return mc.first_arrival(lambda_t, dt, n, 0.0);
-    // })
+  // Microsimulation (or ABM) model class
+  py::class_<no::Model, no::PyModel>(m, "Model", model_docstr)
+    .def(py::init<no::Timeline&, const py::function&>(), model_init_docstr,"timeline"_a,
+       "seeder"_a = py::cpp_function(no::MonteCarlo::deterministic_independent_stream))
+    // properties are readonly only in the sense you can't assign to them; you CAN call their mutable methods
+    .def_property_readonly("timeline", &no::Model::timeline, model_timeline_docstr)
+    .def_property_readonly("mc", &no::Model::mc, model_mc_docstr)
+    .def("modify", &no::Model::modify, model_modify_docstr, "r"_a)
+    .def("step", &no::Model::step, model_step_docstr)
+    .def("check", &no::Model::check, model_check_docstr)
+    .def("finalise", &no::Model::finalise, model_finalise_docstr)
+    .def("halt", &no::Model::halt, model_halt_docstr);
+    // NB the all-important run function is not exposed to python, it can only be executed via the `neworder.run` function
 
   // statistical utils
   m.def_submodule("stats", stats_docstr)
     .def("logistic", no::logistic,
                      stats_logistic_docstr,
                      "x"_a, "x0"_a, "k"_a)
     .def("logistic", [](const py::array_t<double>& a, double k) { return no::logistic(a, 0.0, k); },
@@ -223,16 +191,22 @@
     //.def("linked_change", no::df::linked_change, py::return_value_policy::take_ownership);
 
   // MPI submodule
   m.def_submodule("mpi", mpi_docstr)
     .def("rank", []() { return no::env::rank.load(std::memory_order_relaxed); }, mpi_rank_docstr)
     .def("size", []() { return no::env::size.load(std::memory_order_relaxed); }, mpi_size_docstr);
 
-  // Map custom C++ exceptions to python ones - wrap in a lambda as its an rvalue reference
-  py::register_exception_translator(std::move(no::exception_translator));
+  // model control plus utility/diagnostics
+  m.def("log", log_obj, log_docstr, "obj"_a)
+   .def("run", no::Model::run, run_docstr, "model"_a)
+   .def("verbose", [](bool v = true) { no::env::verbose.store(v, std::memory_order_relaxed); }, verbose_docstr, "verbose"_a = true)
+   .def("checked", [](bool c = true) { no::env::checked.store(c, std::memory_order_relaxed); }, checked_docstr, "checked"_a = true);
+
+  // Map custom C++ exceptions to python ones
+  py::register_exception_translator(no::exception_translator);
 
   init_env();
 }
 
 // initially set to invalid values (so that if model is not properly initialised its immediately apparent)
 std::atomic_int no::env::rank = -1;
 std::atomic_int no::env::size = -1;
```

### Comparing `neworder-1.3.0/src/Module.h` & `neworder-1.3.1/src/Module.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/Module_docstr.cpp` & `neworder-1.3.1/src/Module_docstr.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 )docstr";
 
 const char* timeline_at_end_docstr = R"docstr(
     Returns True if the current step is the end of the timeline
 )docstr";
 
 const char* timeline_repr_docstr = R"docstr(
-    Prints a human-readable representation of the timeline
+    Prints a human-readable representation of the timeline object
 )docstr";
 
 // MonteCarlo
 
 const char* mc_docstr = R"docstr(
     The model's Monte-Carlo engine with configurable options for parallel execution
 )docstr";
@@ -212,15 +212,15 @@
 // The Model class
 
 const char* model_docstr = R"docstr(
     The base model class from which all neworder models should be subclassed
 )docstr";
 
 const char* model_init_docstr = R"docstr(
-    Constructs a model object with a timeline and a seeder function
+    Constructs a model object with a timeline and (optionally) a seeder function for the random stream(s)
 )docstr";
 
 const char* model_timeline_docstr = R"docstr(
     The model's timeline object
 )docstr";
 const char* model_mc_docstr = R"docstr(
     The model's Monte-Carlo engine
```

### Comparing `neworder-1.3.0/src/MonteCarlo.cpp` & `neworder-1.3.1/src/MonteCarlo.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/MonteCarlo.h` & `neworder-1.3.1/src/MonteCarlo.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/NPArray.cpp` & `neworder-1.3.1/src/NPArray.cpp`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/NPArray.h` & `neworder-1.3.1/src/NPArray.h`

 * *Files identical despite different names*

### Comparing `neworder-1.3.0/src/Timeline.cpp` & `neworder-1.3.1/src/Timeline.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-
 #include "Timeline.h"
 #include "Log.h"
 #include "Error.h"
 
-//#include "NewOrder.h"
-
 #include <pybind11/chrono.h>
 
 #include <algorithm>
 
-
 py::object no::NoTimeline::time() const { return py::float_(time::never()); }
 py::object no::NoTimeline::start() const { return py::float_(time::never()); }
 py::object no::NoTimeline::end() const { return py::float_(time::never()); }
 
-int64_t no::NoTimeline::index() const { return static_cast<size_t>(m_stepped); }
 int64_t no::NoTimeline::nsteps() const { return 1; }
 double no::NoTimeline::dt() const { return 0.0; }
 
-void no::NoTimeline::next() { m_stepped = true; }
+void no::NoTimeline::_next() { /* nothing to do, base class increments index */ }
 
-bool no::NoTimeline::at_end() const { return m_stepped; }
-
-std::unique_ptr<no::Timeline> no::NoTimeline::clone() const
-{
-  return std::make_unique<no::NoTimeline>();
-}
+bool no::NoTimeline::at_end() const { return m_index > 0; }
 
 // used by python __repr__
-std::string no::NoTimeline::repr() const { return "<NoTimeline stepped=%%>"s % (m_stepped ? "True": "False"); }
+std::string no::NoTimeline::repr() const { return "<neworder.NoTimeline stepped=%%>"s % (m_index > 0 ? "True": "False"); }
 
 
 no::LinearTimeline::LinearTimeline(double start, double end, size_t steps)
-  : m_index(0), m_start(start), m_end(end), m_steps(steps)
+  : m_start(start), m_end(end), m_steps(steps)
 {
   // validate
   // negative timesteps are disallowed as MC functions will misbehave with dt<0
   if (m_end <= m_start)
   {
     throw py::value_error("end time (%%) must be after the start time (%%)"s % m_end % m_start);
   }
@@ -48,71 +38,57 @@
 
   // set to start
   m_index = 0;
   m_dt = (m_end - m_start) / m_steps;
 }
 
 no::LinearTimeline::LinearTimeline(double start, double step)
-  : m_index(0), m_start(start), m_end(no::time::far_future()), m_dt(step), m_steps(-1)
+  : m_start(start), m_end(no::time::far_future()), m_dt(step), m_steps(-1)
 {
   // validate
   if (m_dt <= 0.0)
   {
     throw py::value_error("timeline must have a positive step size, got %%"s % m_dt);
   }
 }
 
-int64_t no::LinearTimeline::index() const
-{
-  return m_index;
-}
-
 double no::LinearTimeline::dt() const
 {
   return m_dt;
 }
 
 int64_t no::LinearTimeline::nsteps() const
 {
   return m_steps;
 }
 
-void no::LinearTimeline::next()
+void no::LinearTimeline::_next()
 {
-  if (m_steps == 0 || (m_steps > 0 && m_index < m_steps))
-  {
-    ++m_index;
-  }
 }
 
 bool no::LinearTimeline::at_end() const
 {
   return m_steps > 0 && m_index >= m_steps;
 }
 
 py::object no::LinearTimeline::time() const { return py::float_(m_start + m_dt * m_index); }
 py::object no::LinearTimeline::start() const { return py::float_(m_start); }
 py::object no::LinearTimeline::end() const { return py::float_(m_end); }
 
-std::unique_ptr<no::Timeline> no::LinearTimeline::clone() const
-{
-  return std::make_unique<no::LinearTimeline>(*this);
-}
-
 
 std::string no::LinearTimeline::repr() const
 {
   return m_end == no::time::far_future()
     ? "<neworder.LinearTimeline start=%% end=never dt=%% steps=inf time=%% index=%%>"s % m_start % m_dt % time() % m_index
     : "<neworder.LinearTimeline start=%% end=%% dt=%% steps=%% time=%% index=%%>"s % m_start % m_end % m_dt % m_steps % time() % m_index;
 }
 
 
 no::NumericTimeline::NumericTimeline(const std::vector<double>& times)
-  : m_index(0), m_times(times)
+  : m_times(times)
 {
   if (m_times.size() < 2)
   {
     throw py::value_error("timeline must have at least 2 points");
   }
   // check ascending
   for (size_t i = 1; i < m_times.size(); ++i)
@@ -123,67 +99,53 @@
         % i % m_times[i] % m_times[i-1]);
     }
   }
 }
 
 py::object no::NumericTimeline::time() const
 {
-  return py::float_(m_times[m_index]);
+  return at_end() ? end() : py::float_(m_times[m_index]);
 }
 
 py::object no::NumericTimeline::start() const
 {
   return py::float_(m_times.front());
 }
 
 py::object no::NumericTimeline::end() const
 {
   return py::float_(m_times.back());
 }
 
-int64_t no::NumericTimeline::index() const
-{
-  return m_index;
-}
-
 int64_t no::NumericTimeline::nsteps() const
 {
   return m_times.size() - 1;
 }
 
 double no::NumericTimeline::dt() const
 {
-  if (m_index == m_times.size() - 1)
+  if (m_index >= m_times.size() - 1)
     return 0.0;
   return m_times[m_index+1] - m_times[m_index];
 }
 
-void no::NumericTimeline::next()
+void no::NumericTimeline::_next()
 {
-  if (m_index < m_times.size())
-  {
-    ++m_index;
-  }
 }
 
 bool no::NumericTimeline::at_end() const
 {
   return m_index >= m_times.size() - 1;
 }
 
-std::unique_ptr<no::Timeline> no::NumericTimeline::clone() const
-{
-  return std::make_unique<no::NumericTimeline>(*this);
-}
-
 
 std::string no::NumericTimeline::repr() const
 {
   return "<neworder.NumericTimeline times=%% steps=%% time=%% index=%%>"s
-          % m_times % (m_times.size() - 1) % m_times[m_index] % m_index;
+          % m_times % (m_times.size() - 1) % time() % m_index;
 }
 
 
 
 namespace {
 
 // for incrementing time in months preserving day of month
@@ -275,15 +237,15 @@
     default: // m_unit has already been validated
     case 'y': return addMonths(time, m_step * 12, m_refDay); // ensures we deal with leap years correctly
   }
 }
 
 
 no::CalendarTimeline::CalendarTimeline(time_point start, time_point end, size_t step, char unit)
-  : m_index(0), m_step(step), m_unit(tolower(unit)), m_times(1, start)
+  : m_step(step), m_unit(tolower(unit)), m_times(1, start)
 {
   if (m_times[0] >= end)
   {
     throw py::value_error("start time (%%) must be after end time (%%)"s % py::cast(start) % py::cast(end));
   }
 
   if (m_step < 1)
@@ -305,25 +267,19 @@
   {
     time = advance(time);
     if (time >= end)
       break;
     m_times.push_back(time);
   }
   m_times.push_back(end);
-
-  // for (const auto& t: m_m_endTimestimes)
-  // {
-  //   std::time_t tt = std::chrono::system_clock::to_time_t(t);
-  //   no::log(std::ctime(&tt));
-  // }
 }
 
 // open-ended timeline
 no::CalendarTimeline::CalendarTimeline(time_point start, size_t step, char unit)
-  : m_index(0), m_step(step), m_unit(tolower(unit)), m_times(1, start)
+  : m_step(step), m_unit(tolower(unit)), m_times(1, start)
 {
   if (m_step < 1)
   {
     throw py::value_error("time unit step (%%) must be at least 1"s % step);
   }
 
   if (m_unit != 'd' && m_unit != 'm' && m_unit != 'y')
@@ -335,38 +291,24 @@
   tm* local_tm = std::localtime(&t);
   m_refDay = local_tm->tm_mday;
 
   m_currentStep = {start, advance(start) };
 
 }
 
-
-int64_t no::CalendarTimeline::index() const
-{
-  return m_index;
-}
-
 bool no::CalendarTimeline::at_end() const
 {
   return m_times.size() > 1 && m_index >= m_times.size() - 1;
 }
 
-void no::CalendarTimeline::next()
+void no::CalendarTimeline::_next()
 {
   if (m_times.size() < 2)
   {
     m_currentStep = { std::get<1>(m_currentStep), advance(std::get<1>(m_currentStep)) };
-    ++m_index;
-  }
-  else
-  {
-    if (m_index < m_times.size())
-    {
-      ++m_index;
-    }
   }
 }
 
 
 double no::CalendarTimeline::dt() const
 {
   static const double years_per_sec = 1.0 / (365.2475 * 86400);
@@ -389,15 +331,15 @@
 
 py::object no::CalendarTimeline::time() const
 {
   if (m_times.size() < 2)
   {
     return py::cast(std::get<0>(m_currentStep));
   }
-  return py::cast(m_times[m_index]);
+  return at_end() ? end() : py::cast(m_times[m_index]);
 }
 
 py::object no::CalendarTimeline::start() const
 {
   return py::cast(m_times[0]);
 }
 
@@ -406,33 +348,27 @@
   if (m_times.size() < 2)
   {
     return py::float_(no::time::far_future());
   }
   return py::cast(m_times.back());
 }
 
-std::unique_ptr<no::Timeline> no::CalendarTimeline::clone() const
-{
-  return std::make_unique<no::CalendarTimeline>(*this);
-}
-
 
 std::string no::CalendarTimeline::repr() const
 {
   if (m_times.size() < 2)
   {
     return "<neworder.CalendarTimeline start=%% end=never step=%%%% nsteps=inf time=%% index=%%>"s
             % start() % m_step % m_unit % time() % m_index;
   }
   else
   {
     return "<neworder.CalendarTimeline start=%% end=%% step=%%%% nsteps=%% time=%% index=%%>"s
             % start() % end() % m_step % m_unit % (m_times.size() - 1) % time() % m_index;
   }
-
 }
 
 
 // returns a floating point number that compares less than any other number
 double no::time::distant_past()
 {
   return -std::numeric_limits<double>::infinity();
```

### Comparing `neworder-1.3.0/src/Timeline.h` & `neworder-1.3.1/src/Timeline.h`

 * *Files 8% similar despite different names*

```diff
@@ -14,71 +14,94 @@
 namespace no {
 
 // Abstract base class for timelines - implements the basic stepping functionality
 class Timeline
 {
 public:
 
-  Timeline() { }
+  Timeline() : m_index(0) { }
 
   virtual ~Timeline() = default;
 
   // times may have different types, depending on implementation
   virtual py::object time() const = 0;
   virtual py::object start() const = 0;
   virtual py::object end() const = 0;
 
-  virtual int64_t index() const = 0;
+  int64_t index() { return m_index; };
   virtual int64_t nsteps() const = 0;
   virtual double dt() const = 0;
 
-  virtual void next() = 0;
+  virtual void _next() = 0;
 
   virtual bool at_end() const = 0;
 
-  virtual std::unique_ptr<Timeline> clone() const = 0;
+  // used by python __repr__, default implementation
+  virtual std::string repr() const {
+    return "<%% index=%%>"s % py::cast(this).attr("__class__").attr("__name__").cast<std::string>() % m_index;
+  }
 
-  // used by python __repr__
-  virtual std::string repr() const = 0;
+protected:
+  size_t m_index;
+
+private:
+  friend class Model;
+  // this is called internally to ensure index is incremented
+  void next()
+  {
+    ++m_index;
+    _next();
+  }
+};
+
+class PyTimeline: public Timeline
+{
+  using Timeline::Timeline;
+  using Timeline::operator=;
+
+  // trampoline methods
+  py::object time() const override { PYBIND11_OVERRIDE_PURE(py::object, Timeline, time); }
+  py::object start() const override { PYBIND11_OVERRIDE_PURE(py::object, Timeline, start); }
+  py::object end() const override { PYBIND11_OVERRIDE_PURE(py::object, Timeline, end); }
+
+  int64_t nsteps() const override { PYBIND11_OVERRIDE_PURE(int64_t, Timeline, nsteps); }
+  double dt() const override { PYBIND11_OVERRIDE_PURE(double, Timeline, dt); }
 
+  void _next() override { PYBIND11_OVERRIDE_PURE(void, Timeline, _next); }
+
+  bool at_end() const override { PYBIND11_OVERRIDE_PURE(bool, Timeline, at_end); }
+  std::string repr() const override { PYBIND11_OVERRIDE_NAME(std::string, Timeline, "__repr__", repr); }
 };
 
+
 // An empty (one arbitrary step) timeline. The model's step method will each be called once only
 class NEWORDER_EXPORT NoTimeline final : public Timeline
 {
 public:
-  NoTimeline() : m_stepped(false) { }
+  NoTimeline() { }
 
   ~NoTimeline() override = default;
   NoTimeline(const NoTimeline&) = default;
   NoTimeline& operator=(const NoTimeline&) = default;
   NoTimeline(NoTimeline&&) = default;
   NoTimeline& operator=(NoTimeline&&) = default;
 
   // the actual types may differ in derived classes
   py::object time() const override;
   py::object start() const override;
   py::object end() const override;
 
-  int64_t index() const override;
   int64_t nsteps() const override;
   double dt() const override;
 
-  void next() override;
+  void _next() override;
 
   bool at_end() const override;
 
-  virtual std::unique_ptr<Timeline> clone() const override;
-
-  // used by python __repr__
   std::string repr() const override;
-
-private:
-  // flag whether we've done the arbitrary step
-  bool m_stepped;
 };
 
 // An equally-spaced timeline between 2 numeric time points
 class NEWORDER_EXPORT LinearTimeline final : public Timeline
 {
 public:
 
@@ -95,29 +118,24 @@
   LinearTimeline(LinearTimeline&&) = default;
   LinearTimeline& operator=(LinearTimeline&&) = default;
 
   py::object time() const override;
   py::object start() const override;
   py::object end() const override;
 
-  int64_t index() const override;
   int64_t nsteps() const override;
   double dt() const override;
 
-  void next() override;
+  void _next() override;
 
   bool at_end() const override;
 
-  virtual std::unique_ptr<Timeline> clone() const override;
-
-  // used by python __repr__
   std::string repr() const override;
 
 private:
-  size_t m_index;
   double m_start;
   double m_end;
   double m_dt; // store both dt and steps as (re)computing steps from dt is prone to rounding errors
   size_t m_steps;
 };
 
 
@@ -134,28 +152,24 @@
   NumericTimeline(NumericTimeline&&) = default;
   NumericTimeline& operator=(NumericTimeline&&) = default;
 
   py::object time() const override;
   py::object start() const override;
   py::object end() const override;
 
-  int64_t index() const override;
   int64_t nsteps() const override;
   double dt() const override;
 
-  void next() override;
+  void _next() override;
 
   bool at_end() const override;
 
-  virtual std::unique_ptr<Timeline> clone() const override;
-
   std::string repr() const override;
 
 private:
-  size_t m_index;
   std::vector<double> m_times;
 };
 
 // A timeline based on calendar dates and intervals (no intraday resolution, ignores DST adjustments)
 class NEWORDER_EXPORT CalendarTimeline final : public Timeline
 {
 public:
@@ -174,32 +188,28 @@
   CalendarTimeline(CalendarTimeline&&) = default;
   CalendarTimeline& operator=(CalendarTimeline&&) = default;
 
   py::object time() const override;
   py::object start() const override;
   py::object end() const override;
 
-  int64_t index() const override;
   int64_t nsteps() const override;
   double dt() const override;
 
-  void next() override;
+  void _next() override;
 
   bool at_end() const override;
 
-  virtual std::unique_ptr<Timeline> clone() const override;
-
   std::string repr() const override;
 
 private:
 
   // advance to next point
   time_point advance(const time_point& time) const;
 
-  size_t m_index;
   size_t m_step;
   char m_unit;
   int m_refDay;
 
   // this caches timesteps when the end is known (so we know total number of steps)
   std::vector<time_point> m_times;
   // otherwise just store the current step start and end, and a reference day (for monthly increments)
```

### Comparing `neworder-1.3.0/src/Timer.h` & `neworder-1.3.1/src/Timer.h`

 * *Files identical despite different names*


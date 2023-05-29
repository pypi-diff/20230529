# Comparing `tmp/pymc-experimental-0.0.2.tar.gz` & `tmp/pymc-experimental-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.2.tar", last modified: Mon Apr  3 13:02:16 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.3.tar", last modified: Mon May 29 09:55:34 2023, max compression
```

## Comparing `pymc-experimental-0.0.2.tar` & `pymc-experimental-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,69 @@
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.134676 pymc-experimental-0.0.2/
--rw-r--r--   0 michalraczycki   (501) staff       (20)    11720 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/LICENSE
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4542 2023-04-03 13:02:16.134489 pymc-experimental-0.0.2/PKG-INFO
--rw-r--r--   0 michalraczycki   (501) staff       (20)     3324 2023-04-03 12:52:35.000000 pymc-experimental-0.0.2/README.md
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.125664 pymc-experimental-0.0.2/pymc_experimental/
--rw-r--r--   0 michalraczycki   (501) staff       (20)     1010 2023-03-31 10:11:12.000000 pymc-experimental-0.0.2/pymc_experimental/__init__.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.128194 pymc-experimental-0.0.2/pymc_experimental/distributions/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      797 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     7354 2023-03-30 13:59:24.000000 pymc-experimental-0.0.2/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     5629 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.128893 pymc-experimental-0.0.2/pymc_experimental/gp/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      716 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/gp/__init__.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     8610 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.129787 pymc-experimental-0.0.2/pymc_experimental/inference/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      653 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/inference/__init__.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     1159 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/inference/fit.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4576 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)    20459 2023-03-31 08:31:00.000000 pymc-experimental-0.0.2/pymc_experimental/marginal_model.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)    12353 2023-04-03 08:37:32.000000 pymc-experimental-0.0.2/pymc_experimental/model_builder.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.132344 pymc-experimental-0.0.2/pymc_experimental/tests/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      659 2023-03-31 09:40:25.000000 pymc-experimental-0.0.2/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.132818 pymc-experimental-0.0.2/pymc_experimental/tests/distributions/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      749 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4564 2023-03-30 13:55:21.000000 pymc-experimental-0.0.2/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4680 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)    13922 2023-03-31 08:31:00.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     6971 2023-04-03 08:37:32.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     1726 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)      698 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     5371 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     2613 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.134144 pymc-experimental-0.0.2/pymc_experimental/utils/
--rw-r--r--   0 michalraczycki   (501) staff       (20)      784 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/utils/__init__.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)    10096 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     1862 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     6844 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/utils/prior.py
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4819 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pymc_experimental/utils/spline.py
-drwxr-xr-x   0 michalraczycki   (501) staff       (20)        0 2023-04-03 13:02:16.127056 pymc-experimental-0.0.2/pymc_experimental.egg-info/
--rw-r--r--   0 michalraczycki   (501) staff       (20)     4542 2023-04-03 13:02:16.000000 pymc-experimental-0.0.2/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 michalraczycki   (501) staff       (20)     1332 2023-04-03 13:02:16.000000 pymc-experimental-0.0.2/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 michalraczycki   (501) staff       (20)        1 2023-04-03 13:02:16.000000 pymc-experimental-0.0.2/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 michalraczycki   (501) staff       (20)      144 2023-04-03 13:02:16.000000 pymc-experimental-0.0.2/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 michalraczycki   (501) staff       (20)       18 2023-04-03 13:02:16.000000 pymc-experimental-0.0.2/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 michalraczycki   (501) staff       (20)      300 2023-02-16 13:51:23.000000 pymc-experimental-0.0.2/pyproject.toml
--rw-r--r--   0 michalraczycki   (501) staff       (20)       38 2023-04-03 13:02:16.134734 pymc-experimental-0.0.2/setup.cfg
--rw-r--r--   0 michalraczycki   (501) staff       (20)     3540 2023-04-03 13:02:10.000000 pymc-experimental-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.528601 pymc-experimental-0.0.3/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.536601 pymc-experimental-0.0.3/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.540601 pymc-experimental-0.0.3/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.540601 pymc-experimental-0.0.3/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.544601 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.544601 pymc-experimental-0.0.3/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.532600 pymc-experimental-0.0.3/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 09:55:34.000000 pymc-experimental-0.0.3/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 09:55:34.548601 pymc-experimental-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-29 09:55:19.000000 pymc-experimental-0.0.3/setup.py
```

### Comparing `pymc-experimental-0.0.2/LICENSE` & `pymc-experimental-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/PKG-INFO` & `pymc-experimental-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.2
+Version: 0.0.3
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -28,14 +28,18 @@
 # Welcome to `pymc-experimental`
 <a href="https://gitpod.io/#https://github.com/pymc-devs/pymc-experimental">
   <img
     src="https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod"
     alt="Contribute with Gitpod"
   />
 </a>
+<img
+  src="https://codecov.io/gh/pymc-devs/pymc-experimental/branch/main/graph/badge.svg"
+  alt="Codecov Badge"
+/>
 
 As PyMC continues to mature and expand its functionality to accommodate more domains of application, we increasingly see cutting-edge methodologies, highly specialized statistical distributions, and complex models appear.
 While this adds to the functionality and relevance of the project, it can also introduce instability and impose a burden on testing and quality control.
 To reduce the burden on the main `pymc` repository, this `pymc-experimental` repository can become the aggregator and testing ground for new additions to PyMC.
 This may include unusual probability distributions, advanced model fitting algorithms, innovative yet not fully tested methods or any code that may be inappropriate to include in the `pymc` repository, but may want to be made available to users.
 
 The `pymc-experimental` repository can be understood as the first step in the PyMC development pipeline, where all novel code is introduced until it is obvious that it belongs in the main repository.
@@ -77,11 +81,9 @@
 For example, `pymc-experimental` may just include methods that are not fully developed, tested and trusted, while code that is known to work well and has adequate test coverage, but is still too specialized to become part of `pymc` could reside in a `pymc-extras` (or similar) repository.
 
 
 ### Unanswered questions & ToDos
 This project is still young and many things have not been answered or implemented.
 Please get involved!
 
-* What are guidlines for organizing submodules?
+* What are guidelines for organizing submodules?
   * Proposal: No default imports of WIP/unstable submodules. By importing manually we can avoid breaking the package if a submodule breaks, for example because of an updated dependency.
-* How can we minimize the additional burden of additional project repositories?
-* ToDo: Setting up a basic CI pipeline
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.2 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.3 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -10,49 +10,47 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dask_histogram
 Provides-Extra: histogram Provides-Extra: complete Provides-Extra: dev License-
-File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod] As PyMC
-continues to mature and expand its functionality to accommodate more domains of
-application, we increasingly see cutting-edge methodologies, highly specialized
-statistical distributions, and complex models appear. While this adds to the
-functionality and relevance of the project, it can also introduce instability
-and impose a burden on testing and quality control. To reduce the burden on the
-main `pymc` repository, this `pymc-experimental` repository can become the
-aggregator and testing ground for new additions to PyMC. This may include
-unusual probability distributions, advanced model fitting algorithms,
-innovative yet not fully tested methods or any code that may be inappropriate
-to include in the `pymc` repository, but may want to be made available to
-users. The `pymc-experimental` repository can be understood as the first step
-in the PyMC development pipeline, where all novel code is introduced until it
-is obvious that it belongs in the main repository. We hope that this
-organization improves the stability and streamlines the testing overhead of the
-`pymc` repository, while allowing users and developers to test and evaluate
-cutting-edge methods and not yet fully mature features. `pymc-experimental`
-would be designed to mirror the namespaces in `pymc` to make usage and
-migration as easy as possible. For example, a `ParabolicFractal` distribution
-could be used analogously to those in `pymc`: ```python import pymc as pm
-import pymc_experimental as pmx with pm.Model(): alpha = pmx.ParabolicFractal
-('alpha', b=1, c=1) ... ``` ## Questions ### What belongs in `pymc-
-experimental`? - newly-implemented statistical methods, for example step
-methods or model construction helpers - distributions that are tricky to sample
-from or test - infrequently-used fitting methods or distributions - any code
-that requires additional optimization before it can be used in practice ###
-What does not belong in `pymc-experimental`? - Case studies - Implementations
-that cannot be applied generically, for example because they are tied to
-variables from a toy example ### Should there be more than one add-on
-repository? Since there is a lot of code that we may not want in the main
+File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod]
+[Codecov Badge] As PyMC continues to mature and expand its functionality to
+accommodate more domains of application, we increasingly see cutting-edge
+methodologies, highly specialized statistical distributions, and complex models
+appear. While this adds to the functionality and relevance of the project, it
+can also introduce instability and impose a burden on testing and quality
+control. To reduce the burden on the main `pymc` repository, this `pymc-
+experimental` repository can become the aggregator and testing ground for new
+additions to PyMC. This may include unusual probability distributions, advanced
+model fitting algorithms, innovative yet not fully tested methods or any code
+that may be inappropriate to include in the `pymc` repository, but may want to
+be made available to users. The `pymc-experimental` repository can be
+understood as the first step in the PyMC development pipeline, where all novel
+code is introduced until it is obvious that it belongs in the main repository.
+We hope that this organization improves the stability and streamlines the
+testing overhead of the `pymc` repository, while allowing users and developers
+to test and evaluate cutting-edge methods and not yet fully mature features.
+`pymc-experimental` would be designed to mirror the namespaces in `pymc` to
+make usage and migration as easy as possible. For example, a `ParabolicFractal`
+distribution could be used analogously to those in `pymc`: ```python import
+pymc as pm import pymc_experimental as pmx with pm.Model(): alpha =
+pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ## Questions ### What belongs
+in `pymc-experimental`? - newly-implemented statistical methods, for example
+step methods or model construction helpers - distributions that are tricky to
+sample from or test - infrequently-used fitting methods or distributions - any
+code that requires additional optimization before it can be used in practice
+### What does not belong in `pymc-experimental`? - Case studies -
+Implementations that cannot be applied generically, for example because they
+are tied to variables from a toy example ### Should there be more than one add-
+on repository? Since there is a lot of code that we may not want in the main
 repository, does it make sense to have more than one additional repository? For
 example, `pymc-experimental` may just include methods that are not fully
 developed, tested and trusted, while code that is known to work well and has
 adequate test coverage, but is still too specialized to become part of `pymc`
 could reside in a `pymc-extras` (or similar) repository. ### Unanswered
 questions & ToDos This project is still young and many things have not been
-answered or implemented. Please get involved! * What are guidlines for
+answered or implemented. Please get involved! * What are guidelines for
 organizing submodules? * Proposal: No default imports of WIP/unstable
 submodules. By importing manually we can avoid breaking the package if a
-submodule breaks, for example because of an updated dependency. * How can we
-minimize the additional burden of additional project repositories? * ToDo:
-Setting up a basic CI pipeline
+submodule breaks, for example because of an updated dependency.
```

### Comparing `pymc-experimental-0.0.2/README.md` & `pymc-experimental-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Welcome to `pymc-experimental`
 <a href="https://gitpod.io/#https://github.com/pymc-devs/pymc-experimental">
   <img
     src="https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod"
     alt="Contribute with Gitpod"
   />
 </a>
+<img
+  src="https://codecov.io/gh/pymc-devs/pymc-experimental/branch/main/graph/badge.svg"
+  alt="Codecov Badge"
+/>
 
 As PyMC continues to mature and expand its functionality to accommodate more domains of application, we increasingly see cutting-edge methodologies, highly specialized statistical distributions, and complex models appear.
 While this adds to the functionality and relevance of the project, it can also introduce instability and impose a burden on testing and quality control.
 To reduce the burden on the main `pymc` repository, this `pymc-experimental` repository can become the aggregator and testing ground for new additions to PyMC.
 This may include unusual probability distributions, advanced model fitting algorithms, innovative yet not fully tested methods or any code that may be inappropriate to include in the `pymc` repository, but may want to be made available to users.
 
 The `pymc-experimental` repository can be understood as the first step in the PyMC development pipeline, where all novel code is introduced until it is obvious that it belongs in the main repository.
@@ -50,11 +54,9 @@
 For example, `pymc-experimental` may just include methods that are not fully developed, tested and trusted, while code that is known to work well and has adequate test coverage, but is still too specialized to become part of `pymc` could reside in a `pymc-extras` (or similar) repository.
 
 
 ### Unanswered questions & ToDos
 This project is still young and many things have not been answered or implemented.
 Please get involved!
 
-* What are guidlines for organizing submodules?
+* What are guidelines for organizing submodules?
   * Proposal: No default imports of WIP/unstable submodules. By importing manually we can avoid breaking the package if a submodule breaks, for example because of an updated dependency.
-* How can we minimize the additional burden of additional project repositories?
-* ToDo: Setting up a basic CI pipeline
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-# Welcome to `pymc-experimental` [Contribute_with_Gitpod] As PyMC continues to
-mature and expand its functionality to accommodate more domains of application,
-we increasingly see cutting-edge methodologies, highly specialized statistical
-distributions, and complex models appear. While this adds to the functionality
-and relevance of the project, it can also introduce instability and impose a
-burden on testing and quality control. To reduce the burden on the main `pymc`
-repository, this `pymc-experimental` repository can become the aggregator and
-testing ground for new additions to PyMC. This may include unusual probability
-distributions, advanced model fitting algorithms, innovative yet not fully
-tested methods or any code that may be inappropriate to include in the `pymc`
-repository, but may want to be made available to users. The `pymc-experimental`
-repository can be understood as the first step in the PyMC development
-pipeline, where all novel code is introduced until it is obvious that it
-belongs in the main repository. We hope that this organization improves the
-stability and streamlines the testing overhead of the `pymc` repository, while
-allowing users and developers to test and evaluate cutting-edge methods and not
-yet fully mature features. `pymc-experimental` would be designed to mirror the
-namespaces in `pymc` to make usage and migration as easy as possible. For
-example, a `ParabolicFractal` distribution could be used analogously to those
-in `pymc`: ```python import pymc as pm import pymc_experimental as pmx with
-pm.Model(): alpha = pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ##
-Questions ### What belongs in `pymc-experimental`? - newly-implemented
-statistical methods, for example step methods or model construction helpers -
-distributions that are tricky to sample from or test - infrequently-used
-fitting methods or distributions - any code that requires additional
-optimization before it can be used in practice ### What does not belong in
-`pymc-experimental`? - Case studies - Implementations that cannot be applied
-generically, for example because they are tied to variables from a toy example
-### Should there be more than one add-on repository? Since there is a lot of
-code that we may not want in the main repository, does it make sense to have
-more than one additional repository? For example, `pymc-experimental` may just
-include methods that are not fully developed, tested and trusted, while code
-that is known to work well and has adequate test coverage, but is still too
-specialized to become part of `pymc` could reside in a `pymc-extras` (or
-similar) repository. ### Unanswered questions & ToDos This project is still
-young and many things have not been answered or implemented. Please get
-involved! * What are guidlines for organizing submodules? * Proposal: No
-default imports of WIP/unstable submodules. By importing manually we can avoid
-breaking the package if a submodule breaks, for example because of an updated
-dependency. * How can we minimize the additional burden of additional project
-repositories? * ToDo: Setting up a basic CI pipeline
+# Welcome to `pymc-experimental` [Contribute_with_Gitpod] [Codecov Badge] As
+PyMC continues to mature and expand its functionality to accommodate more
+domains of application, we increasingly see cutting-edge methodologies, highly
+specialized statistical distributions, and complex models appear. While this
+adds to the functionality and relevance of the project, it can also introduce
+instability and impose a burden on testing and quality control. To reduce the
+burden on the main `pymc` repository, this `pymc-experimental` repository can
+become the aggregator and testing ground for new additions to PyMC. This may
+include unusual probability distributions, advanced model fitting algorithms,
+innovative yet not fully tested methods or any code that may be inappropriate
+to include in the `pymc` repository, but may want to be made available to
+users. The `pymc-experimental` repository can be understood as the first step
+in the PyMC development pipeline, where all novel code is introduced until it
+is obvious that it belongs in the main repository. We hope that this
+organization improves the stability and streamlines the testing overhead of the
+`pymc` repository, while allowing users and developers to test and evaluate
+cutting-edge methods and not yet fully mature features. `pymc-experimental`
+would be designed to mirror the namespaces in `pymc` to make usage and
+migration as easy as possible. For example, a `ParabolicFractal` distribution
+could be used analogously to those in `pymc`: ```python import pymc as pm
+import pymc_experimental as pmx with pm.Model(): alpha = pmx.ParabolicFractal
+('alpha', b=1, c=1) ... ``` ## Questions ### What belongs in `pymc-
+experimental`? - newly-implemented statistical methods, for example step
+methods or model construction helpers - distributions that are tricky to sample
+from or test - infrequently-used fitting methods or distributions - any code
+that requires additional optimization before it can be used in practice ###
+What does not belong in `pymc-experimental`? - Case studies - Implementations
+that cannot be applied generically, for example because they are tied to
+variables from a toy example ### Should there be more than one add-on
+repository? Since there is a lot of code that we may not want in the main
+repository, does it make sense to have more than one additional repository? For
+example, `pymc-experimental` may just include methods that are not fully
+developed, tested and trusted, while code that is known to work well and has
+adequate test coverage, but is still too specialized to become part of `pymc`
+could reside in a `pymc-extras` (or similar) repository. ### Unanswered
+questions & ToDos This project is still young and many things have not been
+answered or implemented. Please get involved! * What are guidelines for
+organizing submodules? * Proposal: No default imports of WIP/unstable
+submodules. By importing manually we can avoid breaking the package if a
+submodule breaks, for example because of an updated dependency.
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
-
-
-__version__ = "0.0.2"
-
 import logging
 
+from pymc_experimental.version import __version__
+
 _log = logging.getLogger("pmx")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
         _log.addHandler(handler)
 
-
 from pymc_experimental import distributions, gp, utils
 from pymc_experimental.inference.fit import fit
 from pymc_experimental.marginal_model import MarginalModel
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.3/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.3/pymc_experimental/distributions/histogram_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,35 +15,29 @@
 
 from typing import Dict
 
 import numpy as np
 import pymc as pm
 from numpy.typing import ArrayLike
 
-try:
-    import dask.array
-    import dask.dataframe
-except ImportError:
-    dask = None
-
-try:
-    import xhistogram.core
-except ImportError:
-    xhistogram = None
-
-
 __all__ = ["quantile_histogram", "discrete_histogram", "histogram_approximation"]
 
 
 def quantile_histogram(
     data: ArrayLike, n_quantiles=1000, zero_inflation=False
 ) -> Dict[str, ArrayLike]:
-    if xhistogram is None:
-        raise RuntimeError("quantile_histogram requires xhistogram package")
-
+    try:
+        import xhistogram.core
+    except ImportError as e:
+        raise RuntimeError("quantile_histogram requires xhistogram package") from e
+    try:
+        import dask.array
+        import dask.dataframe
+    except ImportError:
+        dask = None
     if dask and isinstance(data, (dask.dataframe.Series, dask.dataframe.DataFrame)):
         data = data.to_dask_array(lengths=True)
     if zero_inflation:
         zeros = (data == 0).sum(0)
         mdata = np.ma.masked_where(data == 0, data)
         qdata = data[data > 0]
     else:
@@ -70,16 +64,23 @@
         mid=(lower + upper) / 2,
         count=count,
     )
     return result
 
 
 def discrete_histogram(data: ArrayLike, min_count=None) -> Dict[str, ArrayLike]:
-    if xhistogram is None:
-        raise RuntimeError("discrete_histogram requires xhistogram package")
+    try:
+        import xhistogram.core
+    except ImportError as e:
+        raise RuntimeError("discrete_histogram requires xhistogram package") from e
+    try:
+        import dask.array
+        import dask.dataframe
+    except ImportError:
+        dask = None
 
     if dask and isinstance(data, (dask.dataframe.Series, dask.dataframe.DataFrame)):
         data = data.to_dask_array(lengths=True)
     mid, count_uniq = np.unique(data, return_counts=True)
     if min_count is not None:
         mid = mid[count_uniq >= min_count]
         count_uniq = count_uniq[count_uniq >= min_count]
@@ -143,14 +144,19 @@
     ...     m = pm.Normal("m", dims="tests")
     ...     s = pm.LogNormal("s", dims="tests")
     ...     pot = pmx.distributions.histogram_approximation(
     ...         "pot", pm.Normal.dist(m, s),
     ...         observed=measurements, n_quantiles=50, zero_inflation=True
     ...     )
     """
+    try:
+        import dask.array
+        import dask.dataframe
+    except ImportError:
+        dask = None
     if dask and isinstance(observed, (dask.dataframe.Series, dask.dataframe.DataFrame)):
         observed = observed.to_dask_array(lengths=True)
     if np.issubdtype(observed.dtype, np.integer):
         histogram = discrete_histogram(observed, **h_kwargs)
     else:
         histogram = quantile_histogram(observed, **h_kwargs)
     if dask is not None:
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/gp/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
-from pymc_experimental.gp.latent_approx import (
-    HSGP,
-    KarhunenLoeveExpansion,
-    ProjectedProcess,
-)
+from pymc_experimental.gp.latent_approx import KarhunenLoeveExpansion, ProjectedProcess
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.3/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.3/pymc_experimental/inference/pathfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     _, rng_key = random.split(rng_key)
     print("Running pathfinder...", file=sys.stdout)
     _, (_, samples) = inference_loop(rng_key, pathfinder.step, state, iterations)
 
     dims = {
         var_name: [dim for dim in dims if dim is not None]
-        for var_name, dims in model.RV_dims.items()
+        for var_name, dims in model.named_vars_to_dims.items()
     }
 
     idata = convert_flat_trace_to_idata(
         samples, postprocessing_backend=postprocessing_backend, coords=model.coords, dims=dims
     )
 
     return idata
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.3/pymc_experimental/marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
+import platform
 
 import numpy as np
 import pymc as pm
 
 # general imports
 import pytensor
 import pytest
@@ -46,42 +47,54 @@
     """
 
     @pytest.mark.xfail(
         condition=(pytensor.config.floatX == "float32"),
         reason="PyMC underflows earlier than scipy on float32",
     )
     def test_logp(self):
+        def ref_logp(value, mu, sigma, xi):
+            if 1 + xi * (value - mu) / sigma > 0:
+                return sp.genextreme.logpdf(value, c=-xi, loc=mu, scale=sigma)
+            else:
+                return -np.inf
+
         check_logp(
             GenExtreme,
             R,
             {
                 "mu": R,
                 "sigma": Rplusbig,
                 "xi": Domain([-1, -0.99, -0.5, 0, 0.5, 0.99, 1]),
             },
-            lambda value, mu, sigma, xi: sp.genextreme.logpdf(value, c=-xi, loc=mu, scale=sigma)
-            if 1 + xi * (value - mu) / sigma > 0
-            else -np.inf,
+            ref_logp,
         )
 
         if pytensor.config.floatX == "float32":
             raise Exception("Flaky test: It passed this time, but XPASS is not allowed.")
 
+    @pytest.mark.skipif(
+        (pytensor.config.floatX == "float32" and platform.system() == "Windows"),
+        reason="Scipy gives different results on Windows and does not match with desired accuracy",
+    )
     def test_logcdf(self):
+        def ref_logcdf(value, mu, sigma, xi):
+            if 1 + xi * (value - mu) / sigma > 0:
+                return sp.genextreme.logcdf(value, c=-xi, loc=mu, scale=sigma)
+            else:
+                return -np.inf
+
         check_logcdf(
             GenExtreme,
             R,
             {
                 "mu": R,
                 "sigma": Rplusbig,
                 "xi": Domain([-1, -0.99, -0.5, 0, 0.5, 0.99, 1]),
             },
-            lambda value, mu, sigma, xi: sp.genextreme.logcdf(value, c=-xi, loc=mu, scale=sigma)
-            if 1 + xi * (value - mu) / sigma > 0
-            else -np.inf,
+            ref_logcdf,
             decimal=select_by_precision(float64=6, float32=2),
         )
 
     @pytest.mark.parametrize(
         "mu, sigma, xi, size, expected",
         [
             (0, 1, 0, None, 0),
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_model_builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,185 +11,172 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import hashlib
 import sys
 import tempfile
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 import pymc as pm
 import pytest
 
 from pymc_experimental.model_builder import ModelBuilder
 
 
 class test_ModelBuilder(ModelBuilder):
     _model_type = "LinearModel"
     version = "0.1"
 
-    def build(self):
+    def build_model(self, data=None, model_config=None):
 
         with pm.Model() as self.model:
-            if self.data is not None:
-                x = pm.MutableData("x", self.data["input"].values)
-                y_data = pm.MutableData("y_data", self.data["output"].values)
+            if data is None:
+                data = test_ModelBuilder.generate_model_data()
+            if model_config is None:
+                model_config = self.default_model_config
+            x = pm.MutableData("x", data["input"].values)
+            y_data = pm.MutableData("y_data", data["output"].values)
 
             # prior parameters
-            a_loc = self.model_config["a_loc"]
-            a_scale = self.model_config["a_scale"]
-            b_loc = self.model_config["b_loc"]
-            b_scale = self.model_config["b_scale"]
-            obs_error = self.model_config["obs_error"]
+            a_loc = model_config["a"]["loc"]
+            a_scale = model_config["a"]["scale"]
+            b_loc = model_config["b"]["loc"]
+            b_scale = model_config["b"]["scale"]
+            obs_error = model_config["obs_error"]
 
             # priors
             a = pm.Normal("a", a_loc, sigma=a_scale)
             b = pm.Normal("b", b_loc, sigma=b_scale)
             obs_error = pm.HalfNormal("σ_model_fmc", obs_error)
 
             # observed data
-            if self.data is not None:
-                y_model = pm.Normal("y_model", a + b * x, obs_error, shape=x.shape, observed=y_data)
+            y_model = pm.Normal("y_model", a + b * x, obs_error, shape=x.shape, observed=y_data)
+            self.output_var = "y_model"
 
-    def _data_setter(self, data: pd.DataFrame):
+    def _data_setter(self, x: pd.Series, y: pd.Series = None):
         with self.model:
-            pm.set_data({"x": data["input"].values})
-            if "output" in data.columns:
-                pm.set_data({"y_data": data["output"].values})
+            pm.set_data({"x": x.values})
+            if y is not None:
+                pm.set_data({"y_data": y.values})
+
+    @property
+    def _serializable_model_config(self):
+        return self.model_config
 
     @classmethod
-    def create_sample_input(self):
+    def generate_model_data(cls, data=None):
         x = np.linspace(start=0, stop=1, num=100)
         y = 5 * x + 3
         y = y + np.random.normal(0, 1, len(x))
         data = pd.DataFrame({"input": x, "output": y})
+        return data
 
-        model_config = {
-            "a_loc": 0,
-            "a_scale": 10,
-            "b_loc": 0,
-            "b_scale": 10,
+    @property
+    def default_model_config(self) -> Dict:
+        return {
+            "a": {"loc": 0, "scale": 10},
+            "b": {"loc": 0, "scale": 10},
             "obs_error": 2,
         }
 
-        sampler_config = {
+    @property
+    def default_sampler_config(self) -> Dict:
+        return {
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
-        return data, model_config, sampler_config
-
     @staticmethod
     def initial_build_and_fit(check_idata=True) -> ModelBuilder:
-        data, model_config, sampler_config = test_ModelBuilder.create_sample_input()
-        model_builder = test_ModelBuilder(
-            model_config=model_config, sampler_config=sampler_config, data=data
-        )
-        model_builder.idata = model_builder.fit(data=data)
+        data = test_ModelBuilder.generate_model_data()
+        model_builder = test_ModelBuilder()
+        model_builder.idata = model_builder.fit(X=data["input"], y=data["output"])
         if check_idata:
             assert model_builder.idata is not None
             assert "posterior" in model_builder.idata.groups()
         return model_builder
 
 
-def test_empty_model_config():
-    data, model_config, sampler_config = test_ModelBuilder.create_sample_input()
+def test_save_without_fit_raises_runtime_error():
+    model_builder = test_ModelBuilder()
+    with pytest.raises(RuntimeError):
+        model_builder.save("saved_model")
+
+
+def test_empty_sampler_config_fit():
     sampler_config = {}
-    model_builder = test_ModelBuilder(
-        model_config=model_config, sampler_config=sampler_config, data=data
-    )
-    model_builder.idata = model_builder.fit(data=data)
+    model_builder = test_ModelBuilder(sampler_config=sampler_config)
+    data = test_ModelBuilder.generate_model_data()
+    model_builder.idata = model_builder.fit(X=data["input"], y=data["output"])
     assert model_builder.idata is not None
     assert "posterior" in model_builder.idata.groups()
 
 
-def test_empty_model_config():
-    data, model_config, sampler_config = test_ModelBuilder.create_sample_input()
-    model_config = {}
-    model_builder = test_ModelBuilder(
-        model_config=model_config, sampler_config=sampler_config, data=data
-    )
-    assert model_builder.model_config == {}
-
-
 def test_fit():
     model = test_ModelBuilder.initial_build_and_fit()
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.predict(prediction_data)
-    assert "y_model" in pred.keys()
-    post_pred = model.predict_posterior(prediction_data)
-    assert "y_model" in post_pred.keys()
+    pred = model.predict(prediction_data["input"])
+    post_pred = model.sample_posterior_predictive(
+        prediction_data["input"], extend_idata=True, combined=True
+    )
+    post_pred.y_model.shape[0] == prediction_data.input.shape
 
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
 )
 def test_save_load():
     test_builder = test_ModelBuilder.initial_build_and_fit()
     temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
     test_builder.save(temp.name)
     test_builder2 = test_ModelBuilder.load(temp.name)
     assert test_builder.idata.groups() == test_builder2.idata.groups()
 
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred1 = test_builder.predict(prediction_data)
-    pred2 = test_builder2.predict(prediction_data)
-    assert pred1["y_model"].shape == pred2["y_model"].shape
+    pred1 = test_builder.predict(prediction_data["input"])
+    pred2 = test_builder2.predict(prediction_data["input"])
+    assert pred1.shape == pred2.shape
     temp.close()
 
 
 def test_predict():
     model = test_ModelBuilder.initial_build_and_fit()
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.predict(prediction_data)
-    assert "y_model" in pred
-    assert isinstance(pred, dict)
-    assert len(prediction_data.input.values) == len(pred["y_model"])
-    assert isinstance(pred["y_model"][0], (np.float32, np.float64))
+    pred = model.predict(prediction_data["input"])
+    # Perform elementwise comparison using numpy
+    assert type(pred) == np.ndarray
+    assert len(pred) > 0
 
 
-def test_predict_posterior():
+@pytest.mark.parametrize("combined", [True, False])
+def test_sample_posterior_predictive(combined):
     model = test_ModelBuilder.initial_build_and_fit()
-    x_pred = np.random.uniform(low=0, high=1, size=100)
+    n_pred = 100
+    x_pred = np.random.uniform(low=0, high=1, size=n_pred)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.predict_posterior(prediction_data)
-    assert "y_model" in pred
-    assert isinstance(pred, dict)
-    assert len(prediction_data.input.values) == len(pred["y_model"][0])
-    assert isinstance(pred["y_model"][0], np.ndarray)
-
-
-def test_extract_samples():
-    # create a fake InferenceData object
-    with pm.Model() as model:
-        x = pm.Normal("x", mu=0, sigma=1)
-        intercept = pm.Normal("intercept", mu=0, sigma=1)
-        y_model = pm.Normal("y_model", mu=x * intercept, sigma=1, observed=[0, 1, 2])
-
-        idata = pm.sample(1000, tune=1000)
-        post_pred = pm.sample_posterior_predictive(idata)
-
-    # call the function and get the output
-    samples_dict = test_ModelBuilder._extract_samples(post_pred)
-
-    # assert that the keys and values are correct
-    assert len(samples_dict) == len(post_pred.posterior_predictive)
-    for key in post_pred.posterior_predictive:
-        expected_value = post_pred.posterior_predictive[key].to_numpy()[0]
-        assert np.array_equal(samples_dict[key], expected_value)
+    pred = model.sample_posterior_predictive(
+        prediction_data["input"], combined=combined, extend_idata=True
+    )
+    chains = model.idata.sample_stats.dims["chain"]
+    draws = model.idata.sample_stats.dims["draw"]
+    expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
+    assert pred["y_model"].shape == expected_shape
+    assert np.issubdtype(pred["y_model"].dtype, np.floating)
 
 
 def test_id():
-    data, model_config, sampler_config = test_ModelBuilder.create_sample_input()
-    model = test_ModelBuilder(model_config=model_config, sampler_config=sampler_config, data=data)
-
+    model = test_ModelBuilder()
     expected_id = hashlib.sha256(
-        str(model_config.values()).encode() + model.version.encode() + model._model_type.encode()
+        str(model.model_config.values()).encode()
+        + model.version.encode()
+        + model._model_type.encode()
     ).hexdigest()[:16]
 
     assert model.id == expected_id
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_pathfinder.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
     with pm.Model() as model:
 
         mu = pm.Normal("mu", mu=0.0, sigma=10.0)
         tau = pm.HalfCauchy("tau", 5.0)
 
         theta = pm.Normal("theta", mu=0, sigma=1, shape=J)
-        theta_1 = mu + tau * theta
-        obs = pm.Normal("obs", mu=theta, sigma=sigma, shape=J, observed=y)
+        obs = pm.Normal("obs", mu=mu + tau * theta, sigma=sigma, shape=J, observed=y)
 
         idata = pmx.fit(method="pathfinder", iterations=100)
 
         assert idata is not None
         assert "theta" in idata.posterior._variables.keys()
         assert "tau" in idata.posterior._variables.keys()
         assert "mu" in idata.posterior._variables.keys()
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,7 +159,13 @@
     with pm.Model(coords=coords) as model:
         priors = pmx.utils.prior.prior_from_idata(
             idata, var_names=user_param_cfg[0], **user_param_cfg[1]
         )
         test_prior = pm.sample_prior_predictive(1)
     names = [p["name"] for p in param_cfg.values()]
     assert set(model.named_vars) == {"trace_prior_", *names}
+
+
+def test_empty(idata, coords):
+    with pm.Model(coords=coords):
+        priors = pmx.utils.prior.prior_from_idata(idata)
+        assert not priors
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.3/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.3/pymc_experimental/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,9 +11,15 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 
 from pymc_experimental.utils import prior, spline
 from pymc_experimental.utils.linear_cg import linear_cg
+from pymc_experimental.utils.model_fgraph import clone_model
 
-# from pymc_experimental.utils.pivoted_cholesky import pivoted_cholesky
+__all__ = (
+    "clone_model",
+    "linear_cg",
+    "prior",
+    "spline",
+)
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.3/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.3/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.3/pymc_experimental/utils/prior.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     return result
 
 
 def prior_from_idata(
     idata: arviz.InferenceData,
     name="trace_prior_",
     *,
-    var_names: Sequence[str],
+    var_names: Sequence[str] = (),
     **kwargs: Union[ParamCfg, RVTransform, str, Tuple]
 ) -> Dict[str, pt.TensorVariable]:
     """
     Create a prior from posterior using MvNormal approximation.
 
     The approximation uses MvNormal distribution.
     Keep in mind that this function will only work well for unimodal
@@ -188,9 +188,11 @@
     ...
     ...                                 # set a name, assign a dim and apply simplex transform
     ...         f=dict(name="new_f", dims="options", transform=transforms.simplex)
     ...     )
     ...     trace1 = pm.sample_prior_predictive(100)
     """
     param_cfg = _parse_args(var_names=var_names, **kwargs)
+    if not param_cfg:
+        return {}
     flat_info = _flatten(idata, **param_cfg)
     return _mvn_prior_from_flat_info(name, flat_info)
```

### Comparing `pymc-experimental-0.0.2/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.3/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.2/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.3/pymc_experimental.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.2
+Version: 0.0.3
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -28,14 +28,18 @@
 # Welcome to `pymc-experimental`
 <a href="https://gitpod.io/#https://github.com/pymc-devs/pymc-experimental">
   <img
     src="https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod"
     alt="Contribute with Gitpod"
   />
 </a>
+<img
+  src="https://codecov.io/gh/pymc-devs/pymc-experimental/branch/main/graph/badge.svg"
+  alt="Codecov Badge"
+/>
 
 As PyMC continues to mature and expand its functionality to accommodate more domains of application, we increasingly see cutting-edge methodologies, highly specialized statistical distributions, and complex models appear.
 While this adds to the functionality and relevance of the project, it can also introduce instability and impose a burden on testing and quality control.
 To reduce the burden on the main `pymc` repository, this `pymc-experimental` repository can become the aggregator and testing ground for new additions to PyMC.
 This may include unusual probability distributions, advanced model fitting algorithms, innovative yet not fully tested methods or any code that may be inappropriate to include in the `pymc` repository, but may want to be made available to users.
 
 The `pymc-experimental` repository can be understood as the first step in the PyMC development pipeline, where all novel code is introduced until it is obvious that it belongs in the main repository.
@@ -77,11 +81,9 @@
 For example, `pymc-experimental` may just include methods that are not fully developed, tested and trusted, while code that is known to work well and has adequate test coverage, but is still too specialized to become part of `pymc` could reside in a `pymc-extras` (or similar) repository.
 
 
 ### Unanswered questions & ToDos
 This project is still young and many things have not been answered or implemented.
 Please get involved!
 
-* What are guidlines for organizing submodules?
+* What are guidelines for organizing submodules?
   * Proposal: No default imports of WIP/unstable submodules. By importing manually we can avoid breaking the package if a submodule breaks, for example because of an updated dependency.
-* How can we minimize the additional burden of additional project repositories?
-* ToDo: Setting up a basic CI pipeline
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.2 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.3 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -10,49 +10,47 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: dask_histogram
 Provides-Extra: histogram Provides-Extra: complete Provides-Extra: dev License-
-File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod] As PyMC
-continues to mature and expand its functionality to accommodate more domains of
-application, we increasingly see cutting-edge methodologies, highly specialized
-statistical distributions, and complex models appear. While this adds to the
-functionality and relevance of the project, it can also introduce instability
-and impose a burden on testing and quality control. To reduce the burden on the
-main `pymc` repository, this `pymc-experimental` repository can become the
-aggregator and testing ground for new additions to PyMC. This may include
-unusual probability distributions, advanced model fitting algorithms,
-innovative yet not fully tested methods or any code that may be inappropriate
-to include in the `pymc` repository, but may want to be made available to
-users. The `pymc-experimental` repository can be understood as the first step
-in the PyMC development pipeline, where all novel code is introduced until it
-is obvious that it belongs in the main repository. We hope that this
-organization improves the stability and streamlines the testing overhead of the
-`pymc` repository, while allowing users and developers to test and evaluate
-cutting-edge methods and not yet fully mature features. `pymc-experimental`
-would be designed to mirror the namespaces in `pymc` to make usage and
-migration as easy as possible. For example, a `ParabolicFractal` distribution
-could be used analogously to those in `pymc`: ```python import pymc as pm
-import pymc_experimental as pmx with pm.Model(): alpha = pmx.ParabolicFractal
-('alpha', b=1, c=1) ... ``` ## Questions ### What belongs in `pymc-
-experimental`? - newly-implemented statistical methods, for example step
-methods or model construction helpers - distributions that are tricky to sample
-from or test - infrequently-used fitting methods or distributions - any code
-that requires additional optimization before it can be used in practice ###
-What does not belong in `pymc-experimental`? - Case studies - Implementations
-that cannot be applied generically, for example because they are tied to
-variables from a toy example ### Should there be more than one add-on
-repository? Since there is a lot of code that we may not want in the main
+File: LICENSE # Welcome to `pymc-experimental` [Contribute_with_Gitpod]
+[Codecov Badge] As PyMC continues to mature and expand its functionality to
+accommodate more domains of application, we increasingly see cutting-edge
+methodologies, highly specialized statistical distributions, and complex models
+appear. While this adds to the functionality and relevance of the project, it
+can also introduce instability and impose a burden on testing and quality
+control. To reduce the burden on the main `pymc` repository, this `pymc-
+experimental` repository can become the aggregator and testing ground for new
+additions to PyMC. This may include unusual probability distributions, advanced
+model fitting algorithms, innovative yet not fully tested methods or any code
+that may be inappropriate to include in the `pymc` repository, but may want to
+be made available to users. The `pymc-experimental` repository can be
+understood as the first step in the PyMC development pipeline, where all novel
+code is introduced until it is obvious that it belongs in the main repository.
+We hope that this organization improves the stability and streamlines the
+testing overhead of the `pymc` repository, while allowing users and developers
+to test and evaluate cutting-edge methods and not yet fully mature features.
+`pymc-experimental` would be designed to mirror the namespaces in `pymc` to
+make usage and migration as easy as possible. For example, a `ParabolicFractal`
+distribution could be used analogously to those in `pymc`: ```python import
+pymc as pm import pymc_experimental as pmx with pm.Model(): alpha =
+pmx.ParabolicFractal('alpha', b=1, c=1) ... ``` ## Questions ### What belongs
+in `pymc-experimental`? - newly-implemented statistical methods, for example
+step methods or model construction helpers - distributions that are tricky to
+sample from or test - infrequently-used fitting methods or distributions - any
+code that requires additional optimization before it can be used in practice
+### What does not belong in `pymc-experimental`? - Case studies -
+Implementations that cannot be applied generically, for example because they
+are tied to variables from a toy example ### Should there be more than one add-
+on repository? Since there is a lot of code that we may not want in the main
 repository, does it make sense to have more than one additional repository? For
 example, `pymc-experimental` may just include methods that are not fully
 developed, tested and trusted, while code that is known to work well and has
 adequate test coverage, but is still too specialized to become part of `pymc`
 could reside in a `pymc-extras` (or similar) repository. ### Unanswered
 questions & ToDos This project is still young and many things have not been
-answered or implemented. Please get involved! * What are guidlines for
+answered or implemented. Please get involved! * What are guidelines for
 organizing submodules? * Proposal: No default imports of WIP/unstable
 submodules. By importing manually we can avoid breaking the package if a
-submodule breaks, for example because of an updated dependency. * How can we
-minimize the additional burden of additional project repositories? * ToDo:
-Setting up a basic CI pipeline
+submodule breaks, for example because of an updated dependency.
```

### Comparing `pymc-experimental-0.0.2/setup.py` & `pymc-experimental-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import itertools
-import re
 from codecs import open
 from os.path import dirname, join, realpath
 
 from setuptools import find_packages, setup
 
 DISTNAME = "pymc-experimental"
 DESCRIPTION = "A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users."
@@ -48,41 +47,43 @@
 
 REQUIREMENTS_FILE = join(PROJECT_ROOT, "requirements.txt")
 DEV_REQUIREMENTS_FILE = join(PROJECT_ROOT, "requirements-dev.txt")
 
 with open(REQUIREMENTS_FILE) as f:
     install_reqs = f.read().splitlines()
 
+
 with open(DEV_REQUIREMENTS_FILE) as f:
     dev_install_reqs = f.read().splitlines()
 
 
-def get_version():
-    VERSIONFILE = join("pymc_experimental", "__init__.py")
-    lines = open(VERSIONFILE).readlines()
-    version_regex = r"^__version__ = ['\"]([^'\"]*)['\"]"
-    for line in lines:
-        mo = re.search(version_regex, line, re.M)
-        if mo:
-            return mo.group(1)
-    raise RuntimeError(f"Unable to find version in {VERSIONFILE}.")
-
-
 extras_require = dict(
     dask_histogram=["dask[complete]", "xhistogram"],
     histogram=["xhistogram"],
 )
 extras_require["complete"] = sorted(set(itertools.chain.from_iterable(extras_require.values())))
 extras_require["dev"] = dev_install_reqs
 
+import os
+
+from setuptools import find_packages, setup
+
+
+def read_version():
+    here = os.path.abspath(os.path.dirname(__file__))
+    with open(os.path.join(here, "pymc_experimental", "version.txt")) as f:
+        version = f.read().strip()
+    return version
+
 
 if __name__ == "__main__":
+
     setup(
-        name=DISTNAME,
-        version=get_version(),
+        name="pymc-experimental",
+        version=read_version(),
         maintainer=AUTHOR,
         maintainer_email=AUTHOR_EMAIL,
         description=DESCRIPTION,
         license=LICENSE,
         url=URL,
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
```


# Comparing `tmp/frds-1.1.0.tar.gz` & `tmp/frds-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "frds-1.3.0.tar", last modified: Mon May 29 01:31:09 2023, max compression
```

## Comparing `frds-1.1.0.tar` & `frds-1.3.0.tar`

### file list

```diff
@@ -1,49 +1,33 @@
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 frds-1.1.0/.pylintrc
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 frds-1.1.0/mkdocs.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 frds-1.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 frds-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 frds-1.1.0/docs/CNAME
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 frds-1.1.0/docs/index.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 frds-1.1.0/docs/algorithms/dcc_garch.md
--rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_icon.png
--rw-r--r--   0        0        0    58143 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_icon_white.png
--rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_logo.png
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/absorption_ratio.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/contingent_claim_analysis.md
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/distress_insurance_premium.md
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/long_run_mes.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/marginal_expected_shortfall.md
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/srisk.md
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/systemic_expected_shortfall.md
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/z_score.md
--rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.1.0/images/frds_icon.png
--rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.1.0/images/frds_logo.png
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 frds-1.1.0/includes/abbreviations.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/algorithms/__init__.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/algorithms/dcc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/absorption_ratio.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/contingent_claim_analysis.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/distress_insurance_premium.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/long_run_mes.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/marginal_expected_shortfall.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/srisk.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/systemic_expected_shortfall.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/z_score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_absorption_ratio.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_distress_insurance_premium.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_marginal_expected_shortfall.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_systemic_expected_shortfall.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_z_score.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 frds-1.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 frds-1.1.0/LICENSE
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 frds-1.1.0/README.md
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 frds-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 frds-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.893170 frds-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 01:30:57.000000 frds-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-29 01:31:09.893170 frds-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-29 01:30:57.000000 frds-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-29 01:30:57.000000 frds-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 01:31:09.893170 frds-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 01:30:57.000000 frds-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.885170 frds-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.885170 frds-1.3.0/src/frds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.889170 frds-1.3.0/src/frds/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/algorithms/dcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.889170 frds-1.3.0/src/frds/algorithms/isolation_forest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/algorithms/isolation_forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/algorithms/isolation_forest/iforest_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.893170 frds-1.3.0/src/frds/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/absorption_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/contingent_claim_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/distress_insurance_premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/lob_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/long_run_mes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/marginal_expected_shortfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/srisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/systemic_expected_shortfall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 01:30:57.000000 frds-1.3.0/src/frds/measures/z_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:31:09.889170 frds-1.3.0/src/frds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-29 01:31:09.000000 frds-1.3.0/src/frds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-29 01:31:09.000000 frds-1.3.0/src/frds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:31:09.000000 frds-1.3.0/src/frds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 01:31:09.000000 frds-1.3.0/src/frds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 01:31:09.000000 frds-1.3.0/src/frds.egg-info/top_level.txt
```

### Comparing `frds-1.1.0/docs/index.md` & `frds-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,94 @@
-# `frds` - *for better and easier finance research*
-
-![LICENSE](https://img.shields.io/github/license/mgao6767/frds?color=blue) ![DOWNLOADS](https://img.shields.io/pypi/dm/frds?label=PyPI%20downloads) [![Test](https://github.com/mgao6767/frds/actions/workflows/test.yml/badge.svg)](https://github.com/mgao6767/frds/actions/workflows/test.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-[`frds`](https://github.com/mgao6767/frds/) is a Python package for computing [a collection of academic measures](/measures/) used in the finance literature. It is developed by [Dr. Mingze Gao](https://mingze-gao.com) from the University of Sydney, as a personal project during his postdoctoral research fellowship.
+Metadata-Version: 2.1
+Name: frds
+Version: 1.3.0
+Summary: Financial Research Data Services
+Author-email: Mingze Gao <adrian.gao@outlook.com>
+License: MIT License
+Project-URL: homepage, https://github.com/mgao6767/frds
+Project-URL: documentation, https://frds.io
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![frds](https://github.com/mgao6767/frds/raw/main/images/frds_logo.png)
 
-## Installation
+# FRDS - Financial Research Data Services
 
-=== "Install via `pip`"
+![LICENSE](https://img.shields.io/github/license/mgao6767/frds?color=blue) ![DOWNLOADS](https://img.shields.io/pypi/dm/frds?label=PyPI%20downloads) [![Test](https://github.com/mgao6767/frds/actions/workflows/test.yml/badge.svg)](https://github.com/mgao6767/frds/actions/workflows/test.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-    frds is available on PyPI and can be installed via `pip`.
+[frds](https://github.com/mgao6767/frds/) is an open-sourced Python package for computing [a collection of major academic measures](https://frds.io/measures/) used in the finance literature in a simple and straightforward way.
 
-    ```bash
-    pip install frds
-    ```
+## Installation
 
-=== "Install from source"
+```bash
+pip install frds
+```
 
-    Sometimes new measures are added and available on GitHub but not yet published to PyPI.
+## Note
 
-    In this case, it may be useful to install directly from source.
+This library is still under development and breaking changes may be expected.
 
-    ``` bash
-    git clone https://github.com/mgao6767/frds.git
-    ```
+If there's any issue (likely), please contact me at [mingze.gao@sydney.edu.au](mailto:mingze.gao@sydney.edu.au)
 
-    Build and install the package locally.
+## Supported measures
 
-    ``` bash
-    cd frds
-    pip install -e .
-    ```
+More to be added. For a complete list of supported built-in measures, please check [frds.io/measures/](https://frds.io/measures/).
 
-## Built-in measures
+* [Absorption Ratio](https://frds.io/measures/absorption_ratio/)
+* [Contingent Claim Analysis](https://frds.io/measures/contingent_claim_analysis/)
+* [Distress Insurance Premium](https://frds.io/measures/distress_insurance_premium/)
+* [Long-Run MES](https://frds.io/measures/long_run_mes/)
+* [Marginal Expected Shortfall (MES)](https://frds.io/measures/marginal_expected_shortfall/)
+* [SRISK](https://frds.io/measures/srisk/)
+* [Systemic Expected Shortfall (SES)](https://frds.io/measures/systemic_expected_shortfall/)
+* [Z-score](https://frds.io/measures/z_score)
 
-The primary purpose of `frds` is to offer ready-to-use functions.
 
-=== "Example: Absorption Ratio"
+## Examples
 
-    For example, Kritzman, Li, Page, and Rigobon (2010) propose an [Absorption Ratio](/measures/absorption_ratio/) that measures the fraction of the total variance of a set of asset returns explained or absorbed by a fixed number of eigenvectors. It captures the extent to which markets are unified or tightly coupled.
+The primary purpose of `frds` is to offer ready-to-use functions.
 
-    ``` python title="Example: Absorption Ratio"
-    >>> import numpy as np
-    >>> from frds.measures import absorption_ratio # (1)
-    >>> data = np.array( # (2)
-    ...             [
-    ...                 [0.015, 0.031, 0.007, 0.034, 0.014, 0.011],
-    ...                 [0.012, 0.063, 0.027, 0.023, 0.073, 0.055],
-    ...                 [0.072, 0.043, 0.097, 0.078, 0.036, 0.083],
-    ...             ]
-    ...         )
-    >>> absorption_ratio.estimate(data, fraction_eigenvectors=0.2)
-    0.7746543307660252
-    ```
-
-    1. We could also import directly the `estimate` function in `#!python absorption_ratio`. 
-    
-        ``` python
-        from frds.measures.absorption_ratio import estimate
-        ```
-        
-        :octicons-light-bulb-16: Tip: You can use ++tab++ to navigate annotations.
-
-    2. Hypothetical 6 daily returns of 3 assets.
-
-=== "Example: Distress Insurance Premium"
-
-    Another example, [Distress Insurance Premium (DIP)](/measures/distress_insurance_premium/) proposed by Huang, Zhou, and Zhu (2009) as a systemic risk measure of a hypothetical insurance premium against a systemic financial distress, defined as total losses that exceed a given threshold, say 15%, of total bank liabilities.
-
-    ``` python title="Example: Distress Insurance Premium"
-    >>> from frds.measures import distress_insurance_premium as dip
-    >>> # hypothetical implied default probabilities of 6 banks
-    >>> default_probabilities = np.array([0.02, 0.10, 0.03, 0.20, 0.50, 0.15] 
-    >>> correlations = np.array(
-    ...     [
-    ...         [ 1.000, -0.126, -0.637, 0.174,  0.469,  0.283],
-    ...         [-0.126,  1.000,  0.294, 0.674,  0.150,  0.053],
-    ...         [-0.637,  0.294,  1.000, 0.073, -0.658, -0.085],
-    ...         [ 0.174,  0.674,  0.073, 1.000,  0.248,  0.508],
-    ...         [ 0.469,  0.150, -0.658, 0.248,  1.000, -0.370],
-    ...         [ 0.283,  0.053, -0.085, 0.508, -0.370,  1.000],
-    ...     ]
-    ... )
-    >>> dip.estimate(default_probabilities, correlations)       
-    0.28661995758
-    ```
+For example, Kritzman, Li, Page, and Rigobon (2010) propose an [Absorption Ratio](https://frds.io/measures/absorption_ratio/) that measures the fraction of the total variance of a set of asset returns explained or absorbed by a fixed number of eigenvectors. It captures the extent to which markets are unified or tightly coupled.
 
-For a complete list of supported built-in measures, please check [frds.io/measures/](/measures/).
+``` python
+>>> import numpy as np
+>>> from frds.measures import absorption_ratio
+>>> data = np.array( # Hypothetical 6 daily returns of 3 assets.
+...             [
+...                 [0.015, 0.031, 0.007, 0.034, 0.014, 0.011],
+...                 [0.012, 0.063, 0.027, 0.023, 0.073, 0.055],
+...                 [0.072, 0.043, 0.097, 0.078, 0.036, 0.083],
+...             ]
+...         )
+>>> absorption_ratio.estimate(data, fraction_eigenvectors=0.2)
+0.7746543307660252
+```
+
+Another example, [Distress Insurance Premium (DIP)](https://frds.io/measures/distress_insurance_premium/) proposed by Huang, Zhou, and Zhu (2009) as a systemic risk measure of a hypothetical insurance premium against a systemic financial distress, defined as total losses that exceed a given threshold, say 15%, of total bank liabilities.
+
+``` python
+>>> from frds.measures import distress_insurance_premium
+>>> # hypothetical implied default probabilities of 6 banks
+>>> default_probabilities = np.array([0.02, 0.10, 0.03, 0.20, 0.50, 0.15] 
+>>> correlations = np.array(
+...     [
+...         [ 1.000, -0.126, -0.637, 0.174,  0.469,  0.283],
+...         [-0.126,  1.000,  0.294, 0.674,  0.150,  0.053],
+...         [-0.637,  0.294,  1.000, 0.073, -0.658, -0.085],
+...         [ 0.174,  0.674,  0.073, 1.000,  0.248,  0.508],
+...         [ 0.469,  0.150, -0.658, 0.248,  1.000, -0.370],
+...         [ 0.283,  0.053, -0.085, 0.508, -0.370,  1.000],
+...     ]
+... )
+>>> distress_insurance_premium.estimate(default_probabilities, correlations)       
+0.28661995758
+```
```

### Comparing `frds-1.1.0/src/frds/algorithms/dcc.py` & `frds-1.3.0/src/frds/algorithms/dcc.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/absorption_ratio.py` & `frds-1.3.0/src/frds/measures/absorption_ratio.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/contingent_claim_analysis.py` & `frds-1.3.0/src/frds/measures/contingent_claim_analysis.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/distress_insurance_premium.py` & `frds-1.3.0/src/frds/measures/distress_insurance_premium.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/long_run_mes.py` & `frds-1.3.0/src/frds/measures/long_run_mes.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/marginal_expected_shortfall.py` & `frds-1.3.0/src/frds/measures/marginal_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/srisk.py` & `frds-1.3.0/src/frds/measures/srisk.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/systemic_expected_shortfall.py` & `frds-1.3.0/src/frds/measures/systemic_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/src/frds/measures/z_score.py` & `frds-1.3.0/src/frds/measures/z_score.py`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/LICENSE` & `frds-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/README.md` & `frds-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `frds-1.1.0/PKG-INFO` & `frds-1.3.0/src/frds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: frds
-Version: 1.1.0
+Version: 1.3.0
 Summary: Financial Research Data Services
-Project-URL: homepage, https://github.com/mgao6767/frds
-Project-URL: documentation, https://frds.io
 Author-email: Mingze Gao <adrian.gao@outlook.com>
 License: MIT License
-License-File: LICENSE
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
+Project-URL: homepage, https://github.com/mgao6767/frds
+Project-URL: documentation, https://frds.io
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
-Requires-Dist: arch
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ![frds](https://github.com/mgao6767/frds/raw/main/images/frds_logo.png)
 
 # FRDS - Financial Research Data Services
 
 ![LICENSE](https://img.shields.io/github/license/mgao6767/frds?color=blue) ![DOWNLOADS](https://img.shields.io/pypi/dm/frds?label=PyPI%20downloads) [![Test](https://github.com/mgao6767/frds/actions/workflows/test.yml/badge.svg)](https://github.com/mgao6767/frds/actions/workflows/test.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```


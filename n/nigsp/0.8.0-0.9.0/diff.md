# Comparing `tmp/nigsp-0.8.0.tar.gz` & `tmp/nigsp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nigsp-0.8.0.tar", last modified: Thu Aug 25 13:25:20 2022, max compression
+gzip compressed data, was "dist/nigsp-0.9.0.tar", last modified: Wed Oct 12 11:32:42 2022, max compression
```

## Comparing `nigsp-0.8.0.tar` & `nigsp-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1923 2022-08-25 13:25:20.000000 nigsp-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      372 2022-08-25 13:25:06.000000 nigsp-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-08-25 13:25:06.000000 nigsp-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6797 2022-08-25 13:25:20.000000 nigsp-0.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     6797 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      499 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1030 2022-08-25 13:25:19.000000 nigsp-0.8.0/nigsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2022-08-25 13:25:06.000000 nigsp-0.8.0/versioneer.py
--rw-r--r--   0 runner    (1001) docker     (116)     5167 2022-08-25 13:25:06.000000 nigsp-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      110 2022-08-25 13:25:06.000000 nigsp-0.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp/
--rw-r--r--   0 runner    (1001) docker     (116)     4800 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     3645 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)      994 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     2700 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)      941 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (116)     6394 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)     6528 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_surrogates.py
--rw-r--r--   0 runner    (1001) docker     (116)     3880 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5367 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_nifti.py
--rw-r--r--   0 runner    (1001) docker     (116)     2303 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3329 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     3129 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (116)     3800 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)    14233 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/io.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp/operations/
--rw-r--r--   0 runner    (1001) docker     (116)     9366 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/nifti.py
--rw-r--r--   0 runner    (1001) docker     (116)     1629 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     1853 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (116)     6061 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)      946 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11396 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (116)    16825 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/operations/surrogates.py
--rw-r--r--   0 runner    (1001) docker     (116)     8842 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/objects.py
--rw-r--r--   0 runner    (1001) docker     (116)    17693 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/workflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     6855 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     8554 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      529 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3804 2022-08-25 13:25:06.000000 nigsp-0.8.0/nigsp/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-08-25 13:25:20.000000 nigsp-0.8.0/nigsp/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-08-25 13:25:06.000000 nigsp-0.8.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2022-10-12 11:32:29.000000 nigsp-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      110 2022-10-12 11:32:29.000000 nigsp-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    68751 2022-10-12 11:32:29.000000 nigsp-0.9.0/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5166 2022-10-12 11:32:29.000000 nigsp-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      381 2022-10-12 11:32:29.000000 nigsp-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6812 2022-10-12 11:32:42.000000 nigsp-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp/
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      529 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1885 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2838 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1243 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1043 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2225 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3888 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3103 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6944 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6381 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3315 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3866 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3526 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5366 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/tests/test_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7040 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6779 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/viz.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4920 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (116)      237 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/references.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3783 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2046 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/due.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8801 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14424 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17756 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp/operations/
+-rw-r--r--   0 runner    (1001) docker     (116)      869 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9497 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11318 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16694 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1628 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6165 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3016 2022-10-12 11:32:29.000000 nigsp-0.9.0/nigsp/operations/laplacian.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      651 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       48 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1063 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     6812 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-12 11:32:42.000000 nigsp-0.9.0/nigsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)     2404 2022-10-12 11:32:42.000000 nigsp-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-10-12 11:32:29.000000 nigsp-0.9.0/LICENSE
```

### Comparing `nigsp-0.8.0/setup.cfg` & `nigsp-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = nigsp
 url = https://github.com/MIPLabCH/nigsp
 download_url = https://github.com/MIPLabCH/nigsp
 author = Stefano Moia
 maintainer = Stefano Moia
 maintainer_email = s.moia.research@gmail.com
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -22,14 +22,15 @@
 provides = 
 	nigsp
 
 [options]
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.17
+	duecredit
 tests_require = 
 	pytest >=3.6
 test_suite = pytest
 zip_safe = False
 packages = find:
 include_package_data = True
 
@@ -43,55 +44,87 @@
 	matplotlib>=3.1.1
 	nilearn>=0.7.0
 all = 
 	%(nifti)s
 	%(mat)s
 	%(viz)s
 doc = 
-	sphinx >=2.0
+	sphinx>=2.0
 	sphinx-argparse
 	sphinx_rtd_theme
 	myst-parser
 style = 
-	flake8>=3.7
+	flake8>=4.0
+	black<23.0.0
+	isort<6.0.0
+	pydocstyle
 test = 
 	%(all)s
 	%(style)s
 	pytest-cov
 	coverage
+devtools = 
+	pre-commit
 dev = 
+	%(devtools)s
 	%(doc)s
 	%(test)s
 
 [options.entry_points]
 console_scripts = 
 	nigsp=nigsp.workflow:_main
 
 [flake8]
 doctest = True
 exclude = 
-	*build/
-	tests
-ignore = E126, E402, W503
-max-line-length = 99
+	_version.py
+	./nigsp/cli/__init__.py
+	./nigsp/tests/*
+	versioneer.py
+ignore = E126, E402, W503, F401, F811
+max-line-length = 88
+extend-ignore = E203, E501
+extend-select = B950
 per-file-ignores = 
-	*/__init__.py:F401
+	workflow.py:D401
+
+[isort]
+profile = black
+skip_gitignore = true
+extend_skip = 
+	.autorc
+	.coverage*
+	.readthedocs.yml
+	.zenodo.json
+	codecov.yml
+	setup.py
+	versioneer.py
+	nigsp/_version.py
+skip_glob = 
+	docs/*
+
+[pydocstyle]
+convention = numpy
+match = 
+	nigsp/*.py
+match_dir = nigsp/[^tests]*
 
 [tool:pytest]
 doctest_optionflags = NORMALIZE_WHITESPACE
 xfail_strict = true
 addopts = -rx
 
 [coverage:run]
 branch = True
 omit = 
 	nigsp/tests/*
 	docs/*
 	setup.py
 	versioneer.py
+	doi.py
 	__init__.py
 	*/__init__.py
 	*/*/__init__.py
 
 [versioneer]
 vcs = git
 style = pep440
```

### Comparing `nigsp-0.8.0/LICENSE` & `nigsp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nigsp-0.8.0/PKG-INFO` & `nigsp-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigsp
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python library (and toolbox!) to run Graph Signal Processing on multimodal MRI data.
 Home-page: https://github.com/MIPLabCH/nigsp
 Author: Stefano Moia
 Maintainer: Stefano Moia
 Maintainer-email: s.moia.research@gmail.com
 License: Apache-2.0
 Download-URL: https://github.com/MIPLabCH/nigsp
@@ -76,28 +76,28 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
-        
 Platform: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: nigsp
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: viz
 Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: nifti
+Provides-Extra: devtools
 Provides-Extra: style
+Provides-Extra: viz
 Provides-Extra: doc
 Provides-Extra: mat
-Provides-Extra: nifti
 Provides-Extra: all
-Provides-Extra: dev
```

### Comparing `nigsp-0.8.0/nigsp.egg-info/PKG-INFO` & `nigsp-0.9.0/nigsp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nigsp
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python library (and toolbox!) to run Graph Signal Processing on multimodal MRI data.
 Home-page: https://github.com/MIPLabCH/nigsp
 Author: Stefano Moia
 Maintainer: Stefano Moia
 Maintainer-email: s.moia.research@gmail.com
 License: Apache-2.0
 Download-URL: https://github.com/MIPLabCH/nigsp
@@ -76,28 +76,28 @@
         
         Unless required by applicable law or agreed to in writing, software
         distributed under the License is distributed on an "AS IS" BASIS,
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
         
-        
 Platform: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides: nigsp
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: viz
 Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: nifti
+Provides-Extra: devtools
 Provides-Extra: style
+Provides-Extra: viz
 Provides-Extra: doc
 Provides-Extra: mat
-Provides-Extra: nifti
 Provides-Extra: all
-Provides-Extra: dev
```

### Comparing `nigsp-0.8.0/nigsp.egg-info/SOURCES.txt` & `nigsp-0.9.0/nigsp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 nigsp/__init__.py
 nigsp/_version.py
 nigsp/blocks.py
+nigsp/due.py
 nigsp/io.py
 nigsp/objects.py
+nigsp/references.py
 nigsp/utils.py
 nigsp/viz.py
 nigsp/workflow.py
 nigsp.egg-info/PKG-INFO
 nigsp.egg-info/SOURCES.txt
 nigsp.egg-info/dependency_links.txt
 nigsp.egg-info/entry_points.txt
```

### Comparing `nigsp-0.8.0/versioneer.py` & `nigsp-0.9.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,33 +304,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(me), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -344,14 +348,15 @@
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +373,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +423,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +1000,86 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s*" % tag_prefix,
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1094,55 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
+        0
+    ].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1190,30 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1234,30 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1281,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1395,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1421,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1450,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1506,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1561,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1594,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1623,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1656,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1693,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1751,41 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        EnvironmentError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1819,18 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(
+            " appending versionfile_source ('%s') to MANIFEST.in"
+            % cfg.versionfile_source
+        )
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

### Comparing `nigsp-0.8.0/README.md` & `nigsp-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,8 +65,7 @@
 http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
-
```

### Comparing `nigsp-0.8.0/nigsp/blocks.py` & `nigsp-0.9.0/nigsp/blocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 import logging
 
 from nigsp import io, viz
 from nigsp.operations import nifti
 
-
 LGR = logging.getLogger(__name__)
 
 
 def nifti_to_timeseries(fname, atlasname):
     """
     Read a nifti file and returns a normalised timeseries from an atlas.
 
@@ -67,35 +66,39 @@
     0
         If everything goes well
     """
     if outext in io.EXT_NIFTI:
         try:
             import nibabel as _
         except ImportError:
-            LGR.warning('The necessary library for nifti export (nibabel) '
-                        'was not found. Exporting metrics in CSV format instead.')
-            outext = '.csv'
+            LGR.warning(
+                "The necessary library for nifti export (nibabel) "
+                "was not found. Exporting metrics in CSV format instead."
+            )
+            outext = ".csv"
         if scgraph.img is None:
-            LGR.warning('A necessary atlas nifti image was not found. '
-                        'Exporting metrics in CSV format instead.')
-            outext = '.csv'
+            LGR.warning(
+                "A necessary atlas nifti image was not found. "
+                "Exporting metrics in CSV format instead."
+            )
+            outext = ".csv"
 
     if scgraph.sdi is not None:
         if outext in io.EXT_NIFTI:
             data = nifti.unfold_atlas(scgraph.sdi, scgraph.atlas)
-            io.export_nifti(data, scgraph.img, f'{outprefix}sdi{outext}')
+            io.export_nifti(data, scgraph.img, f"{outprefix}sdi{outext}")
         else:
-            io.export_mtx(scgraph.sdi, f'{outprefix}sdi{outext}')
+            io.export_mtx(scgraph.sdi, f"{outprefix}sdi{outext}")
     elif scgraph.gsdi is not None:
         for k in scgraph.gsdi.keys():
             if outext in io.EXT_NIFTI:
                 data = nifti.unfold_atlas(scgraph.gsdi[k], scgraph.atlas)
-                io.export_nifti(data, scgraph.img, f'{outprefix}gsdi_{k}{outext}')
+                io.export_nifti(data, scgraph.img, f"{outprefix}gsdi_{k}{outext}")
             else:
-                io.export_mtx(scgraph.gsdi[k], f'{outprefix}gsdi_{k}{outext}')
+                io.export_mtx(scgraph.gsdi[k], f"{outprefix}gsdi_{k}{outext}")
 
     return 0
 
 
 def plot_metric(scgraph, outprefix, atlas=None, thr=None):
     """
     If possible, plot metrics as markerplot.
@@ -119,27 +122,33 @@
         atlas_plot = atlas
     except AttributeError:
         try:
             atlas.min()
             if atlas.ndim == 2 and atlas.shape[1] == 3:
                 atlas_plot = atlas
         except AttributeError:
-            LGR.warning('The provided atlas is not in a format supported for '
-                        'markerplots.')
+            LGR.warning(
+                "The provided atlas is not in a format supported for " "markerplots."
+            )
             atlas_plot = None
 
     # If it is, plot.
     if atlas_plot is not None:
         if scgraph.sdi is not None:
-            viz.plot_nodes(scgraph.sdi, atlas_plot,
-                           filename=f'{outprefix}sdi.png', thr=thr)
+            viz.plot_nodes(
+                scgraph.sdi, atlas_plot, filename=f"{outprefix}sdi.png", thr=thr
+            )
         elif scgraph.gsdi is not None:
             for k in scgraph.gsdi.keys():
-                viz.plot_nodes(scgraph.gsdi[k], atlas_plot,
-                               filename=f'{outprefix}gsdi_{k}.png', thr=thr)
+                viz.plot_nodes(
+                    scgraph.gsdi[k],
+                    atlas_plot,
+                    filename=f"{outprefix}gsdi_{k}.png",
+                    thr=thr,
+                )
 
     return 0
 
 
 """
 Copyright 2022, Stefano Moia.
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_timeseries.py` & `nigsp-0.9.0/nigsp/tests/test_timeseries.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from nigsp.operations import timeseries
 from nigsp.utils import prepare_ndim_iteration
 
 
 # ### Unit tests
 def test_normalise_ts():
     ts = rand(3, 20)
-    z = ((ts - ts.mean(axis=1)[:, np.newaxis, ...]) /
-         ts.std(axis=1, ddof=1)[:, np.newaxis, ...])
+    z = (ts - ts.mean(axis=1)[:, np.newaxis, ...]) / ts.std(axis=1, ddof=1)[
+        :, np.newaxis, ...
+    ]
     z[np.isnan(z)] = 0
 
     tsz = timeseries.normalise_ts(ts)
 
     assert (tsz == z).all()
 
 
@@ -33,52 +34,52 @@
     ts = rand(3, 6, 2, 2)
     tsr, pr = prepare_ndim_iteration(ts, 2)
 
     for i in range(tsr.shape[-1]):
         pr[:, :, i] = ev.conj().T @ np.squeeze(tsr[:, :, i])
     pr = pr.reshape(ts.shape)
     prm = pr.mean(axis=1)
-    engm = (pr ** 2).mean(axis=1)
+    engm = (pr**2).mean(axis=1)
 
     proj = timeseries.graph_fourier_transform(ts, ev, mean=True)
     eng = timeseries.graph_fourier_transform(ts, ev, energy=True, mean=True)
 
     assert (proj == prm).all()
     assert (eng == engm).all()
 
 
 def test_median_cutoff_frequency_idx():
-    energy = np.array([[0, 3], [1, 2], [0, 1], [.5, .5]])
+    energy = np.array([[0, 3], [1, 2], [0, 1], [0.5, 0.5]])
     freq_t = 2
 
     freq_idx = timeseries.median_cutoff_frequency_idx(energy)
 
     assert freq_t == freq_idx
 
 
 def test_graph_filter():
     ts = rand(4, 10)
     ev = rand(4, 4)
 
-    keys = ['hi', 'ho']
+    keys = ["hi", "ho"]
     freq_idx = 2
 
     ev_s = dict.fromkeys(keys)
     ts_s = dict.fromkeys(keys)
 
-    ev_s['hi'] = np.append(ev[:, :freq_idx],
-                           np.zeros_like(ev[:, freq_idx:],
-                                         dtype='float32'), axis=-1)
-    ev_s['ho'] = np.append(np.zeros_like(ev[:, :freq_idx],
-                                         dtype='float32'),
-                           ev[:, freq_idx:], axis=-1)
+    ev_s["hi"] = np.append(
+        ev[:, :freq_idx], np.zeros_like(ev[:, freq_idx:], dtype="float32"), axis=-1
+    )
+    ev_s["ho"] = np.append(
+        np.zeros_like(ev[:, :freq_idx], dtype="float32"), ev[:, freq_idx:], axis=-1
+    )
 
     fcf = timeseries.graph_fourier_transform(ts, ev)
-    ts_s['ho'] = timeseries.graph_fourier_transform(fcf, ev_s['ho'].T)
-    ts_s['hi'] = timeseries.graph_fourier_transform(fcf, ev_s['hi'].T)
+    ts_s["ho"] = timeseries.graph_fourier_transform(fcf, ev_s["ho"].T)
+    ts_s["hi"] = timeseries.graph_fourier_transform(fcf, ev_s["hi"].T)
 
     evec_split, ts_split = timeseries.graph_filter(ts, ev, freq_idx, keys)
 
     assert all(item in keys for item in list(evec_split.keys()))
     assert all(item in keys for item in list(ts_split.keys()))
     for k in keys:
         assert (ev_s[k] == evec_split[k]).all()
@@ -87,44 +88,40 @@
 
 def test_functional_connectivity():
     assert timeseries.functional_connectivity(rand(6)) == 1
 
     ts = rand(3, 6, 2, 2)
 
     tst, _ = prepare_ndim_iteration(ts, 2)
-    fc = np.empty(([tst.shape[0]] * 2 + [tst.shape[-1]]), dtype='float32')
+    fc = np.empty(([tst.shape[0]] * 2 + [tst.shape[-1]]), dtype="float32")
     for i in range(tst.shape[-1]):
         fc[:, :, i] = np.corrcoef(tst[..., i])
 
     ns = (ts.shape[0],) * 2 + ts.shape[2:]
     fc = fc.reshape(ns).mean(axis=2).squeeze()
 
     fc_t = timeseries.functional_connectivity(ts, mean=True)
 
     assert (fc == fc_t).all()
 
-    tsd = {'hi': rand(3, 6), 'lo': rand(3, 6)}
+    tsd = {"hi": rand(3, 6), "lo": rand(3, 6)}
 
     fcd = timeseries.functional_connectivity(tsd)
 
     assert all(item in list(tsd.keys()) for item in list(fcd.keys()))
 
     for k in fcd.keys():
         assert (fcd[k] == np.corrcoef(tsd[k])).all()
 
 
 # ### Break tests
 def test_break_median_cutoff_frequency_idx():
     with raises(NotImplementedError) as errorinfo:
         timeseries.median_cutoff_frequency_idx(rand(2, 3, 4))
-    assert 'have 3 dimensions' in str(errorinfo.value)
+    assert "have 3 dimensions" in str(errorinfo.value)
 
 
-@mark.parametrize('freq', [
-    (0),
-    (2),
-    (4)
-])
+@mark.parametrize("freq", [(0), (2), (4)])
 def test_break_graph_filter(freq):
     with raises(IndexError) as errorinfo:
         timeseries.graph_filter(rand(2, 3), rand(2, 2), freq)
-    assert f'index {freq} is not valid' in str(errorinfo.value)
+    assert f"index {freq} is not valid" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_graph.py` & `nigsp-0.9.0/nigsp/tests/test_graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 
 from nigsp.operations import graph
 
 
 # ### Unit tests
 def test_zerocross():
     """Test zerocross with legendre polynomials."""
+
     def _bonnet(d, x):
-        if(d == 0):
+        if d == 0:
             return np.ones_like(x)
-        elif(d == 1):
+        elif d == 1:
             return x
         else:
-            return ((2*d-1)*x*_bonnet(d-1, x)-(d-1)*_bonnet(d-2, x))/d
+            return (
+                (2 * d - 1) * x * _bonnet(d - 1, x) - (d - 1) * _bonnet(d - 2, x)
+            ) / d
 
     x = np.linspace(-1, 1, 100)
-    legendre = np.empty([100, 5], dtype='float32')
+    legendre = np.empty([100, 5], dtype="float32")
     for n in range(5):
         legendre[:, n] = _bonnet(n, x)
 
     zx = np.linspace(0, 4, 5)
 
     assert all(zx == graph.zerocross(legendre))
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_integration.py` & `nigsp-0.9.0/nigsp/tests/test_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,71 @@
 #!/usr/bin/env python3
 """Integration test."""
 import shutil
-
-from os.path import isfile, isdir, join
+from os.path import isdir, isfile, join
 
 import numpy as np
 
 from nigsp.workflow import _main
 
 
 # ### Integration tests
 def test_integration(timeseries, sc_mtx, atlas, mean_fc, sdi, testdir):
     """Integration test for FULL workflow."""
-    testdir = join(testdir, 'testdir')
+    testdir = join(testdir, "testdir")
     mean_fc_mat = np.genfromtxt(mean_fc)
     # Compared to original SDI, now we log2 it).
     sdi_mat = np.log2(np.genfromtxt(sdi))
 
     # Run workflow
-    _main(['-f', timeseries, '-s', sc_mtx, '-a', atlas, '-odir', testdir,
-          '-ofile', 'testfile.tsv', '-sci', '-n', '4', '-seed', '42'])
-
+    # fmt: off
+    _main(
+        [
+            "-f", timeseries,
+            "-s", sc_mtx,
+            "-a", atlas,
+            "-odir", testdir,
+            "-ofile", "testfile.tsv",
+            "-sci",
+            "-n", "4",
+            "-seed", "42",
+        ]
+    )
+    # fmt: on
     # Check that files were created
     assert isdir(testdir)
-    assert isdir(join(testdir, 'logs'))
-    assert isdir(join(testdir, 'testfile_timeseries_low'))
-    assert isdir(join(testdir, 'testfile_timeseries_high'))
-    assert isfile(join(testdir, 'testfile_timeseries_low', '000.tsv'))
-    assert isfile(join(testdir, 'testfile_timeseries_high', '000.tsv'))
-    assert isfile(join(testdir, 'testfile_fc.tsv'))
-    assert isfile(join(testdir, 'testfile_fc_low.tsv'))
-    assert isfile(join(testdir, 'testfile_fc_high.tsv'))
-    assert isfile(join(testdir, 'testfile_eigenval.tsv'))
-    assert isfile(join(testdir, 'testfile_eigenvec.tsv'))
-    assert isfile(join(testdir, 'testfile_eigenvec_low.tsv'))
-    assert isfile(join(testdir, 'testfile_eigenvec_high.tsv'))
-    assert isfile(join(testdir, 'testfile_sdi.tsv'))
-    assert isfile(join(testdir, 'testfile_mkd_sdi.tsv'))
-    assert isfile(join(testdir, 'testfile_laplacian.png'))
-    assert isfile(join(testdir, 'testfile_sc.png'))
-    assert isfile(join(testdir, 'testfile_fc.png'))
-    assert isfile(join(testdir, 'testfile_fc_low.png'))
-    assert isfile(join(testdir, 'testfile_fc_high.png'))
-    assert isfile(join(testdir, 'testfile_grayplot.png'))
-    assert isfile(join(testdir, 'testfile_grayplot_low.png'))
-    assert isfile(join(testdir, 'testfile_grayplot_high.png'))
-    assert isfile(join(testdir, 'testfile_sdi.png'))
-    assert isfile(join(testdir, 'testfile_mkd_sdi.png'))
+    assert isdir(join(testdir, "logs"))
+    assert isdir(join(testdir, "testfile_timeseries_low"))
+    assert isdir(join(testdir, "testfile_timeseries_high"))
+    assert isfile(join(testdir, "testfile_timeseries_low", "000.tsv"))
+    assert isfile(join(testdir, "testfile_timeseries_high", "000.tsv"))
+    assert isfile(join(testdir, "testfile_fc.tsv"))
+    assert isfile(join(testdir, "testfile_fc_low.tsv"))
+    assert isfile(join(testdir, "testfile_fc_high.tsv"))
+    assert isfile(join(testdir, "testfile_eigenval.tsv"))
+    assert isfile(join(testdir, "testfile_eigenvec.tsv"))
+    assert isfile(join(testdir, "testfile_eigenvec_low.tsv"))
+    assert isfile(join(testdir, "testfile_eigenvec_high.tsv"))
+    assert isfile(join(testdir, "testfile_sdi.tsv"))
+    assert isfile(join(testdir, "testfile_mkd_sdi.tsv"))
+    assert isfile(join(testdir, "testfile_laplacian.png"))
+    assert isfile(join(testdir, "testfile_sc.png"))
+    assert isfile(join(testdir, "testfile_fc.png"))
+    assert isfile(join(testdir, "testfile_fc_low.png"))
+    assert isfile(join(testdir, "testfile_fc_high.png"))
+    assert isfile(join(testdir, "testfile_grayplot.png"))
+    assert isfile(join(testdir, "testfile_grayplot_low.png"))
+    assert isfile(join(testdir, "testfile_grayplot_high.png"))
+    assert isfile(join(testdir, "testfile_sdi.png"))
+    assert isfile(join(testdir, "testfile_mkd_sdi.png"))
 
-    sdi_pyt = np.genfromtxt(join(testdir, 'testfile_sdi.tsv'))
-    sdi_mkd = np.genfromtxt(join(testdir, 'testfile_mkd_sdi.tsv'))
+    sdi_pyt = np.genfromtxt(join(testdir, "testfile_sdi.tsv"))
+    sdi_mkd = np.genfromtxt(join(testdir, "testfile_mkd_sdi.tsv"))
 
-    mean_fc_pyt = np.genfromtxt(join(testdir, 'testfile_fc.tsv'))
+    mean_fc_pyt = np.genfromtxt(join(testdir, "testfile_fc.tsv"))
     # Check that each cell in the result is comparable to matlab's.
     # There's a bunch of rounding due to np.round and numerical difference between matlab and python
     assert abs(mean_fc_pyt.round(6) - mean_fc_mat.round(6)).max().round(6) <= 0.000001
     assert abs(sdi_pyt.round(5) - sdi_mat.round(5)).max().round(5) <= 0.00001
     assert (sdi_pyt != sdi_mkd).any()
 
     # Clean up!
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_io.py` & `nigsp-0.9.0/nigsp/tests/test_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,82 @@
 #!/usr/bin/env python3
 """Tests for io."""
 
 import sys
-
 from os import remove
 from os.path import isfile
 
 import nibabel
-import scipy
 import pymatreader
-
-from numpy import empty, asarray, genfromtxt, savetxt
+import scipy
+from numpy import asarray, empty, genfromtxt, savetxt
 from numpy.random import rand
 from pytest import mark, raises
 
 from nigsp import io
 
-
 # ### Unit tests
 
+
 def test_check_ext():
     """Text check_ext."""
     all_ext = io.EXT_1D + io.EXT_MAT + io.EXT_NIFTI
     for ext_in in all_ext:
-        fname_in = f'shiny{ext_in}'
+        fname_in = f"shiny{ext_in}"
 
         for fname in [fname_in, fname_in.upper()]:
             has_ext, fname_out = io.check_ext(all_ext, fname)
 
             assert has_ext is True
             assert fname_out == fname
 
             has_ext, fname_out, ext_out = io.check_ext(all_ext, fname, remove=True)
 
             assert has_ext is True
-            assert fname_out == fname[:-len(ext_in)]
+            assert fname_out == fname[: -len(ext_in)]
             assert ext_out == ext_in
 
     # #!# Missing scan option
 
-    fname_in = 'shiny.mal'
+    fname_in = "shiny.mal"
     for fname in [fname_in, fname_in.upper()]:
-        has_ext, fname_out = io.check_ext('.inara', fname)
+        has_ext, fname_out = io.check_ext(".inara", fname)
 
         assert has_ext is False
         assert fname_out == fname
 
-        has_ext, fname_out, ext_out = io.check_ext('.inara', fname, remove=True)
+        has_ext, fname_out, ext_out = io.check_ext(".inara", fname, remove=True)
 
         assert has_ext is False
         assert fname_out == fname
-        assert ext_out == ''
+        assert ext_out == ""
 
 
-@mark.parametrize('data', [
-    (rand(3, 4)),
-    (rand(3, 4, 1)),
-    (rand(3, 1, 4))
-])
+@mark.parametrize("data", [(rand(3, 4)), (rand(3, 4, 1)), (rand(3, 1, 4))])
 def test_check_nifti_dim(data):
     """Test check_nifti_dim."""
-    data_out = io.check_nifti_dim('kaylee', data, dim=2)
+    data_out = io.check_nifti_dim("kaylee", data, dim=2)
 
     assert (data_out == data.squeeze()).all()
     assert data_out.ndim == 2
 
 
-@mark.parametrize('data', [
-    (rand(3, 4)),
-    (rand(3, 4, 1)),
-    (rand(3, 1, 4))
-])
+@mark.parametrize("data", [(rand(3, 4)), (rand(3, 4, 1)), (rand(3, 1, 4))])
 def test_check_mtx_dim(data):
     """Test check_mtx_dim."""
-    data_out = io.check_mtx_dim('wash', data)
+    data_out = io.check_mtx_dim("wash", data)
 
     assert (data_out == data.squeeze()).all()
     assert data_out.ndim == 2
 
 
-@mark.parametrize('data, shape', [
-    (rand(3), 'rectangle'),
-    (rand(3, 3), 'square')
-])
+@mark.parametrize("data, shape", [(rand(3), "rectangle"), (rand(3, 3), "square")])
 def test_check_mtx_dim_cases(data, shape):
     """Test check_mtx_dim for specific shapes."""
-    data_out = io.check_mtx_dim('wash', data, shape=shape)
+    data_out = io.check_mtx_dim("wash", data, shape=shape)
 
     assert (data_out.squeeze() == data).all()
     assert data_out.ndim == 2
 
 
 def test_load_nifti_get_mask(atlas):
     """Test load_nifti_get_mask."""
@@ -97,156 +84,156 @@
     data = img.get_fdata()
     mask = data.any(axis=-1).squeeze()
 
     d, m, i = io.load_nifti_get_mask(atlas, ndim=3)
 
     assert (data == d).all()
     assert (mask == m).all()
-    assert (img.header['dim'] == i.header['dim']).all()
+    assert (img.header["dim"] == i.header["dim"]).all()
 
     remove(atlas)
 
 
 def test_load_txt():
     """Test load_txt."""
     a = rand(5)
-    n = 'zoe'
+    n = "zoe"
     savetxt(n, a)
     b = io.load_txt(n)
 
     assert (a == b).all()
 
     remove(n)
 
 
 def test_load_mat():
     """Test load_mat."""
     a = rand(5)
-    b = 'likealeaf'
-    n = 'inthewind'
+    b = "likealeaf"
+    n = "inthewind"
 
-    scipy.io.savemat(n, {'data': a, 'other': b})
+    scipy.io.savemat(n, {"data": a, "other": b})
 
     c = io.load_mat(n)
 
     assert (a == c).all()
     remove(n)
 
 
 def test_export_nifti(atlas):
     """Test export_nifti."""
     img = nibabel.load(atlas)
     shape = img.get_fdata().shape
-    io.export_nifti(empty(shape), img, 'book')
-    assert isfile('book.nii.gz')
-    remove('book.nii.gz')
+    io.export_nifti(empty(shape), img, "book")
+    assert isfile("book.nii.gz")
+    remove("book.nii.gz")
     remove(atlas)
 
 
-@mark.parametrize('ext_in, ext_out', [
-    ('.1D', '.1D'),
-    ('.csv', '.csv'),
-    ('.tsv', '.tsv'),
-    ('', '.csv'),
-    ('.mat', '.mat')
-])
+@mark.parametrize(
+    "ext_in, ext_out",
+    [
+        (".1D", ".1D"),
+        (".csv", ".csv"),
+        (".tsv", ".tsv"),
+        ("", ".csv"),
+        (".mat", ".mat"),
+    ],
+)
 def test_export_mtx(ext_in, ext_out):
     """Test export_mtx."""
     data = asarray([[1, 1, 2], [3, 5, 8]])
-    io.export_mtx(data, 'serenity', ext=ext_in)
-    assert isfile(f'serenity{ext_out}')
+    io.export_mtx(data, "serenity", ext=ext_in)
+    assert isfile(f"serenity{ext_out}")
 
-    if ext_out in ['.csv']:
-        data_in = genfromtxt(f'serenity{ext_out}', delimiter=',')
-    if ext_out in ['.tsv', '.1D']:
-        data_in = genfromtxt(f'serenity{ext_out}')
-
-    if ext_out in ['.mat']:
-        data_in = pymatreader.read_mat(f'serenity{ext_out}')
-        data_in = data_in['data']
+    if ext_out in [".csv"]:
+        data_in = genfromtxt(f"serenity{ext_out}", delimiter=",")
+    if ext_out in [".tsv", ".1D"]:
+        data_in = genfromtxt(f"serenity{ext_out}")
+
+    if ext_out in [".mat"]:
+        data_in = pymatreader.read_mat(f"serenity{ext_out}")
+        data_in = data_in["data"]
 
     assert (data_in == data).all()
     # remove data
-    remove(f'serenity{ext_out}')
+    remove(f"serenity{ext_out}")
 
 
 # ### Break tests
-@mark.parametrize('data', [
-    (rand(3)),
-    (rand(3, 4, 2))
-])
+@mark.parametrize("data", [(rand(3)), (rand(3, 4, 2))])
 def test_break_check_nifti_dim(data):
     """Break check_nifti_dim."""
     with raises(ValueError) as errorinfo:
-        io.check_nifti_dim('jayne', data, dim=2)
-    assert f'jayne is {data.ndim}D' in str(errorinfo.value)
+        io.check_nifti_dim("jayne", data, dim=2)
+    assert f"jayne is {data.ndim}D" in str(errorinfo.value)
 
 
 def test_break_check_mtx_dim():
     """Break check_mtx_dim."""
     with raises(ValueError) as errorinfo:
-        io.check_mtx_dim('river', empty(0))
-    assert 'river is empty' in str(errorinfo.value)
+        io.check_mtx_dim("river", empty(0))
+    assert "river is empty" in str(errorinfo.value)
 
     with raises(NotImplementedError) as errorinfo:
-        io.check_mtx_dim('river', rand(3, 4, 5, 6))
-    assert '3D are supported' in str(errorinfo.value)
+        io.check_mtx_dim("river", rand(3, 4, 5, 6))
+    assert "3D are supported" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
-        io.check_mtx_dim('river', rand(3, 4), shape='square')
-    assert 'river matrix has shape (3, 4)' in str(errorinfo.value)
+        io.check_mtx_dim("river", rand(3, 4), shape="square")
+    assert "river matrix has shape (3, 4)" in str(errorinfo.value)
 
 
 def test_break_load_nifti_get_mask():
     """Break load_nifti_get_mask."""
-    sys.modules['nibabel'] = None
+    sys.modules["nibabel"] = None
     with raises(ImportError) as errorinfo:
-        io.load_nifti_get_mask('reavers')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['nibabel'] = nibabel
+        io.load_nifti_get_mask("reavers")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["nibabel"] = nibabel
 
 
 def test_break_load_mat():
     """Break load_mat."""
-    sys.modules['pymatreader'] = None
+    sys.modules["pymatreader"] = None
     with raises(ImportError) as errorinfo:
-        io.load_mat('simon')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['pymatreader'] = pymatreader
-
-    a = 'heart'
-    n = 'ofgold'
-    scipy.io.savemat(n, {'data': a})
+        io.load_mat("simon")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["pymatreader"] = pymatreader
+
+    a = "heart"
+    n = "ofgold"
+    scipy.io.savemat(n, {"data": a})
 
     with raises(EOFError) as errorinfo:
         io.load_mat(n)
-    assert f'{n} does not seem' in str(errorinfo.value)
+    assert f"{n} does not seem" in str(errorinfo.value)
     remove(n)
 
 
 def test_break_load_xls():
     """Break load_xls."""
     with raises(NotImplementedError) as errorinfo:
-        io.load_xls('firefly')
-    assert 'loading is not' in str(errorinfo.value)
+        io.load_xls("firefly")
+    assert "loading is not" in str(errorinfo.value)
 
 
 def test_break_export_nifti():
     """Break export_nifti."""
-    sys.modules['nibabel'] = None
+    sys.modules["nibabel"] = None
     with raises(ImportError) as errorinfo:
-        io.export_nifti(rand(3), None, 'reavers')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['nibabel'] = nibabel
+        io.export_nifti(rand(3), None, "reavers")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["nibabel"] = nibabel
 
 
 def test_break_export_mtx():
     """Break export_mtx."""
     with raises(NotImplementedError) as errorinfo:
-        io.export_mtx(rand(3, 4), 'lostinthewoods', ext='.xls')
-    assert 'output is not' in str(errorinfo.value)
+        io.export_mtx(rand(3, 4), "lostinthewoods", ext=".xls")
+    assert "output is not" in str(errorinfo.value)
 
-    sys.modules['scipy'] = None
+    sys.modules["scipy"] = None
     with raises(ImportError) as errorinfo:
-        io.export_mtx(rand(3, 4), 'lostinthewoods', ext='.mat')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['scipy'] = scipy
+        io.export_mtx(rand(3, 4), "lostinthewoods", ext=".mat")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["scipy"] = scipy
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_surrogates.py` & `nigsp-0.9.0/nigsp/tests/test_surrogates.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 #!/usr/bin/env python3
 """Tests for operations.surrogates."""
 import numpy as np
-from numpy.random import rand, default_rng
+from numpy.random import default_rng, rand
 from pytest import raises
 
-from nigsp.operations import surrogates, graph_fourier_transform, decomposition
+from nigsp.operations import decomposition, graph_fourier_transform, surrogates
 
 
 # ### Unit tests
 def test_random_sign():
     n_surr = 4
     random_seed = 2
     eigenvec = rand(20)
 
     rs = surrogates.random_sign(eigenvec, n_surr, random_seed, stack=True)
 
     # For the moment, replicate code inside function.
     rng = default_rng(random_seed)
-    rand_evec = np.empty((eigenvec.shape + (n_surr,)), dtype='float32')
+    rand_evec = np.empty((eigenvec.shape + (n_surr,)), dtype="float32")
     for i in range(n_surr):
         r_sign = rng.integers(0, 1, eigenvec.shape[0], endpoint=True)
         r_sign[r_sign == 0] = -1
         rand_evec[..., i] = eigenvec * r_sign
     rand_evec = np.append(rand_evec, eigenvec[..., np.newaxis], axis=-1)
 
     assert rs.ndim == 2
     assert rs.shape == eigenvec.shape + (n_surr + 1,)
     assert (rand_evec == rs).all()
 
     # #!# Implement stricter checks on signs
-    pass 
+    pass
+
 
 def test_create_surr():
     eigenvec = rand(2, 2)
     timeseries = rand(2, 4)
     n_surr = 3
     seed = 2
 
     cs = surrogates._create_surr(timeseries, eigenvec, n_surr, seed, stack=True)
 
     rand_evec = surrogates.random_sign(eigenvec, n_surr, seed, stack=True)
-    surr = np.empty((timeseries.shape + (n_surr+1,)), dtype='float32')
+    surr = np.empty((timeseries.shape + (n_surr + 1,)), dtype="float32")
     fourier_coeff = graph_fourier_transform(timeseries, eigenvec)
 
-    for i in range(n_surr+1):
+    for i in range(n_surr + 1):
         surr[..., i] = graph_fourier_transform(fourier_coeff, rand_evec[..., i].T)
 
     assert cs.ndim == 3
     assert cs.shape == surr.shape
     assert (cs == surr).all()
 
 
@@ -69,109 +70,145 @@
     lapl_mtx = rand(2, 2)
     timeseries = rand(2, 4)
     n_surr = 3
     seed = 2
 
     symm_norm = np.eye(lapl_mtx.shape[0]) - lapl_mtx
     symm_norm_sum = symm_norm.sum(axis=-1)
-    conf_model = np.outer(symm_norm_sum,
-                          symm_norm_sum.T) / symm_norm.sum()
+    conf_model = np.outer(symm_norm_sum, symm_norm_sum.T) / symm_norm.sum()
     conf_lapl = np.diag(symm_norm_sum) - conf_model
     _, surr_eigenvec = decomposition(conf_lapl)
     surr = surrogates._create_surr(timeseries, surr_eigenvec, n_surr, seed, stack=True)
 
     cs = surrogates.sc_uninformed(timeseries, lapl_mtx, n_surr, seed, stack=True)
 
     assert cs.ndim == 3
     assert cs.shape == surr.shape
     assert (cs == surr).all()
 
 
 def test_test_significance():
     # Create surrogates so that one subject has 3 significant obervations over 4,
     # and in group 1 observation is significant over 5
-    surr = np.array([[[.1, .1, .1, .1, .4], [.1, .1, .1, .1, .4], [.1, .1, .1, .1, -.1], [.4, .4, .1, .1, .2]],
-                    [[.1, .1, .1, .1, .4], [.1, .1, .1, .1, .4], [.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2]],
-                    [[.1, .1, .1, .1, .4], [.1, .1, .1, .1, .4], [.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2]],
-                    [[.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2]],
-                    [[.1, .1, .1, .1, .4], [.1, .1, .1, .1, .4], [.4, .4, .1, .1, .2], [.4, .4, .1, .1, .2]]])
+    surr = np.array(
+        [
+            [
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.1, 0.1, 0.1, 0.1, -0.1],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+            ],
+            [
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+            ],
+            [
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+            ],
+            [
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+            ],
+            [
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.1, 0.1, 0.1, 0.1, 0.4],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+                [0.4, 0.4, 0.1, 0.1, 0.2],
+            ],
+        ]
+    )
 
     data = surr[..., -1]
     p_bernoulli = 0.35
     p = 0.4
     # Test frequentist method first
-    mask_freq = np.array([[True, True,  True, False],
-                         [True, True, False, False],
-                         [True, True, False, False],
-                         [False, False, False, False],
-                         [True, True, False, False]])
-    mask = surrogates.test_significance(surr, data, method='frequentist', p=p)
+    mask_freq = np.array(
+        [
+            [True, True, True, False],
+            [True, True, False, False],
+            [True, True, False, False],
+            [False, False, False, False],
+            [True, True, False, False],
+        ]
+    )
+    mask = surrogates.test_significance(surr, data, method="frequentist", p=p)
 
     assert (mask_freq == mask).all()
 
     # Test Bernoulli's method after (mask created flat in 1D for convenience)
     mask_bern = np.array([True, False, False, False, False])
     mask_bern = mask_bern[..., np.newaxis].repeat(surr.shape[1], axis=-1)
     mask = surrogates.test_significance(surr, p=p, p_bernoulli=p_bernoulli)
 
     assert (mask_bern == mask).all()
 
     # Test masked and average
     masked_data = np.ma.array(data=data, mask=np.invert(mask_freq), fill_value=0)
-    mask = surrogates.test_significance(surr, method='frequentist', p=p,
-                                        return_masked=True)
+    mask = surrogates.test_significance(
+        surr, method="frequentist", p=p, return_masked=True
+    )
 
     assert (masked_data == mask).all()
 
     masked_data_avg = masked_data.mean(axis=1)
-    mask_avg = surrogates.test_significance(surr, method='frequentist', p=p,
-                                            return_masked=True, mean=True)
+    mask_avg = surrogates.test_significance(
+        surr, method="frequentist", p=p, return_masked=True, mean=True
+    )
 
     assert (masked_data_avg == mask_avg).all()
 
 
 # ### Break tests
 def test_break_random_sign():
     with raises(NotImplementedError) as errorinfo:
         surrogates.random_sign(rand(2, 3, 4, 5))
-    assert 'has 4 dimensions' in str(errorinfo.value)
+    assert "has 4 dimensions" in str(errorinfo.value)
 
 
 def test_break_create_surr():
     with raises(NotImplementedError) as errorinfo:
         surrogates._create_surr(rand(2, 3, 4, 5), rand(2, 2), 1, 2, False)
-    assert 'timeseries of 4 dimension(s)' in str(errorinfo.value)
+    assert "timeseries of 4 dimension(s)" in str(errorinfo.value)
 
     with raises(NotImplementedError) as errorinfo:
         surrogates._create_surr(rand(2), rand(2, 2), 1, 2, False)
-    assert ('timeseries of 1 dimension(s) and eigenvector matrix of 2 dimension(s)'
-            in str(errorinfo.value))
+    assert (
+        "timeseries of 1 dimension(s) and eigenvector matrix of 2 dimension(s)"
+        in str(errorinfo.value)
+    )
 
 
 def test_break_sc_informed():
     with raises(NotImplementedError) as errorinfo:
         surrogates.sc_informed(rand(2, 3, 4, 5), rand(2, 2))
-    assert 'has 4 dimensions' in str(errorinfo.value)
+    assert "has 4 dimensions" in str(errorinfo.value)
 
 
 def test_break_sc_uninformed():
     with raises(NotImplementedError) as errorinfo:
         surrogates.sc_uninformed(rand(2, 3, 4, 5), rand(2, 2))
-    assert 'has 4 dimensions' in str(errorinfo.value)
+    assert "has 4 dimensions" in str(errorinfo.value)
 
 
 def test_break_test_significance():
     with raises(ValueError) as errorinfo:
         surrogates.test_significance(rand(2, 3, 5), rand(2, 4))
-    assert 'shapes do not agree' in str(errorinfo.value)
+    assert "shapes do not agree" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         surrogates.test_significance(rand(2, 4, 3), rand(2, 4), p=-0.1)
-    assert 'p values should always be between 0 and 1' in str(errorinfo.value)
+    assert "p values should always be between 0 and 1" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         surrogates.test_significance(rand(2, 4, 3), rand(2, 4), p=1.1)
-    assert 'p values should always be between 0 and 1' in str(errorinfo.value)
+    assert "p values should always be between 0 and 1" in str(errorinfo.value)
 
     with raises(NotImplementedError) as errorinfo:
-        surrogates.test_significance(rand(2, 3, 5), method='Baobab')
-    assert 'Other testing methods' in str(errorinfo.value)
+        surrogates.test_significance(rand(2, 3, 5), method="Baobab")
+    assert "Other testing methods" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_blocks.py` & `nigsp-0.9.0/nigsp/tests/test_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,114 +8,111 @@
 import nibabel
 import numpy as np
 from nilearn.plotting import find_parcellation_cut_coords
 from pymatreader import read_mat
 from pytest import mark
 
 from nigsp import blocks
-from nigsp.objects import SCGraph
 from nigsp.io import load_nifti_get_mask
+from nigsp.objects import SCGraph
 
 
 # ### Unit tests
 def test_nifti_to_timeseries(atlastime, atlas):
 
     img_in = nibabel.load(atlas)
     atlas_in = img_in.get_fdata()
     ts_out, atlas_out, img_out = blocks.nifti_to_timeseries(atlastime, atlas)
     ts_in = np.unique(atlas_in)[1:, np.newaxis]
     ts_in = np.repeat(ts_in, 2, axis=-1)
 
     assert (ts_in == ts_out).all()
     assert (atlas_in == atlas_out).all()
-    assert (img_in.header['dim'] == img_out.header['dim']).all()
+    assert (img_in.header["dim"] == img_out.header["dim"]).all()
 
     remove(atlastime)
     remove(atlas)
 
 
-@mark.parametrize('ext', [
-    ('.nii.gz'),
-    ('.csv')
-])
+@mark.parametrize("ext", [(".nii.gz"), (".csv")])
 def test_export_metrics_txt(ext, sc_mtx, atlas, sdi, testdir):
 
-    testdir = join(testdir, 'testdir')
+    testdir = join(testdir, "testdir")
     makedirs(testdir, exist_ok=True)
     atlas_in, mask, img = load_nifti_get_mask(atlas, ndim=3)
     mtx = read_mat(sc_mtx)
-    mtx = mtx['SC_avg56']
+    mtx = mtx["SC_avg56"]
     sdi_in = np.genfromtxt(sdi)
     ts = np.unique(atlas_in)[1:]
     ts = np.repeat(ts[..., np.newaxis], 2, axis=-1)
-    gsdi = dict.fromkeys(['hilo', 'himid'], sdi_in)
+    gsdi = dict.fromkeys(["hilo", "himid"], sdi_in)
     scgraph = SCGraph(mtx, ts, atlas=atlas_in, img=img, sdi=sdi_in)
-    blocks.export_metric(scgraph, ext, join(testdir, 'molly_'))
+    blocks.export_metric(scgraph, ext, join(testdir, "molly_"))
     scgraph = SCGraph(mtx, ts, atlas=atlas_in, img=img, gsdi=gsdi)
-    blocks.export_metric(scgraph, ext, join(testdir, 'cesar_'))
+    blocks.export_metric(scgraph, ext, join(testdir, "cesar_"))
 
-    assert isfile(join(testdir, f'molly_sdi{ext}'))
-    assert isfile(join(testdir, f'cesar_gsdi_hilo{ext}'))
-    assert isfile(join(testdir, f'cesar_gsdi_himid{ext}'))
+    assert isfile(join(testdir, f"molly_sdi{ext}"))
+    assert isfile(join(testdir, f"cesar_gsdi_hilo{ext}"))
+    assert isfile(join(testdir, f"cesar_gsdi_himid{ext}"))
 
     shutil.rmtree(testdir)
     remove(sc_mtx)
     remove(atlas)
     remove(sdi)
 
 
 def test_export_metrics_nifti(sc_mtx, atlas, sdi, testdir):
 
-    testdir = join(testdir, 'testdir')
+    testdir = join(testdir, "testdir")
     makedirs(testdir, exist_ok=True)
     atlas_in, mask, img = load_nifti_get_mask(atlas, ndim=3)
     mtx = read_mat(sc_mtx)
-    mtx = mtx['SC_avg56']
+    mtx = mtx["SC_avg56"]
     sdi_in = np.genfromtxt(sdi)
     ts = np.unique(atlas_in)[1:]
     ts = np.repeat(ts[..., np.newaxis], 2, axis=-1)
     scgraph = SCGraph(mtx, ts, atlas=atlas_in, sdi=sdi_in)
-    blocks.export_metric(scgraph, '.nii.gz', join(testdir, 'molly_'))
+    blocks.export_metric(scgraph, ".nii.gz", join(testdir, "molly_"))
 
-    assert isfile(join(testdir, 'molly_sdi.csv'))
+    assert isfile(join(testdir, "molly_sdi.csv"))
 
-    sys.modules['nibabel'] = None
+    sys.modules["nibabel"] = None
     scgraph = SCGraph(mtx, ts, atlas=atlas_in, img=img, sdi=sdi_in)
-    blocks.export_metric(scgraph, '.nii.gz', join(testdir, 'molly_'))
-    sys.modules['nibabel'] = nibabel
+    blocks.export_metric(scgraph, ".nii.gz", join(testdir, "molly_"))
+    sys.modules["nibabel"] = nibabel
 
-    assert isfile(join(testdir, 'molly_sdi.csv'))
+    assert isfile(join(testdir, "molly_sdi.csv"))
     shutil.rmtree(testdir)
     remove(sc_mtx)
     remove(atlas)
     remove(sdi)
 
 
 def test_plot_metrics(atlas, sc_mtx, sdi, testdir):
 
-    testdir = join(testdir, 'testdir')
+    testdir = join(testdir, "testdir")
     makedirs(testdir, exist_ok=True)
     atlas_in, _, img = load_nifti_get_mask(atlas, ndim=3)
     mtx = read_mat(sc_mtx)
-    mtx = mtx['SC_avg56']
+    mtx = mtx["SC_avg56"]
     sdi_in = np.genfromtxt(sdi)
     ts = np.unique(atlas_in)[1:]
     ts = np.repeat(ts[..., np.newaxis], 2, axis=-1)
-    gsdi = dict.fromkeys(['hilo', 'himid'], sdi_in)
+    gsdi = dict.fromkeys(["hilo", "himid"], sdi_in)
 
     scgraph = SCGraph(mtx, ts, sdi=sdi_in, img=img)
-    blocks.plot_metric(scgraph, join(testdir, 'maite_'), atlas=img)
-    assert isfile(join(testdir, join(testdir, 'maite_sdi.png')))
+    blocks.plot_metric(scgraph, join(testdir, "maite_"), atlas=img)
+    assert isfile(join(testdir, join(testdir, "maite_sdi.png")))
 
     atlas_in = find_parcellation_cut_coords(img)
     scgraph = SCGraph(mtx, ts, sdi=sdi_in, img=img)
-    blocks.plot_metric(scgraph, join(testdir, 'maite_'), atlas=atlas_in)
-    assert isfile(join(testdir, join(testdir, 'maite_sdi.png')))
+    blocks.plot_metric(scgraph, join(testdir, "maite_"), atlas=atlas_in)
+    assert isfile(join(testdir, join(testdir, "maite_sdi.png")))
 
     scgraph = SCGraph(mtx, ts, gsdi=gsdi, img=img)
-    blocks.plot_metric(scgraph, join(testdir, 'dimitri_'), atlas=img)
-    assert isfile(join(testdir, join(testdir, 'dimitri_gsdi_hilo.png')))
-    
+    blocks.plot_metric(scgraph, join(testdir, "dimitri_"), atlas=img)
+    assert isfile(join(testdir, join(testdir, "dimitri_gsdi_hilo.png")))
+
     shutil.rmtree(testdir)
     remove(sc_mtx)
     remove(atlas)
     remove(sdi)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_utils.py` & `nigsp-0.9.0/nigsp/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 from numpy.random import rand
 from pytest import mark, raises
 
 from nigsp import utils
 
 
 # ### Unit tests
-@mark.parametrize('var, dtype', [
-    (6, int),
-    (4.2, float),
-    ('hello', str),
-    (rand(3), ndarray),
-    ([1, 1, 2, 3, 5], list),
-    ('6', int),
-    (4, float),
-    (42, str),
-    ('hi', list),
-    ([1, 1, 2, 3, 5], ndarray)
-])
+@mark.parametrize(
+    "var, dtype",
+    [
+        (6, int),
+        (4.2, float),
+        ("hello", str),
+        (rand(3), ndarray),
+        ([1, 1, 2, 3, 5], list),
+        ("6", int),
+        (4, float),
+        (42, str),
+        ("hi", list),
+        ([1, 1, 2, 3, 5], ndarray),
+    ],
+)
 def test_change_var_type(var, dtype):
     """Test change_var_type."""
     # #!# Test logger!
     var_out = utils.change_var_type(var, dtype, stop=False)
 
     assert type(var_out) == dtype
 
 
 # ### Break tests
-@mark.parametrize('var, dtype', [
-    ('6', int),
-    (4, float),
-    (42, str),
-    ('hi', list),
-    ([1, 1, 2, 3, 5], ndarray)
-])
+@mark.parametrize(
+    "var, dtype",
+    [("6", int), (4, float), (42, str), ("hi", list), ([1, 1, 2, 3, 5], ndarray)],
+)
 def test_break_change_var_type(var, dtype):
     """Break change_var_type."""
     with raises(TypeError) as errorinfo:
         utils.change_var_type(var, dtype)
-    assert 'is not of type' in str(errorinfo.value)
+    assert "is not of type" in str(errorinfo.value)
 
 
 def test_break_change_var_type_dtype():
     """Break change_var_type."""
     with raises(NotImplementedError) as errorinfo:
         utils.change_var_type(6, bool, stop=False)
-    assert 'not supported' in str(errorinfo.value)
+    assert "not supported" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_nifti.py` & `nigsp-0.9.0/nigsp/tests/test_nifti.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 #!/usr/bin/env python3
 """Tests for operations.nifti."""
-from numpy import prod, asarray, zeros, unique
+from numpy import asarray, prod, unique, zeros
 from numpy.random import rand
-
 from pytest import raises
 
 from nigsp.operations import nifti
 
 
 # ### Unit tests
 def test_vol_to_mat():
     a = rand(3, 4, 5, 6)
     b = nifti.vol_to_mat(a)
-    c = b.reshape(a.shape, order='F')
+    c = b.reshape(a.shape, order="F")
 
     assert b.ndim == 2
     assert b.shape == ((prod(a.shape[:-1])), a.shape[-1])
     assert (a == c).all()
 
     a = rand(3, 4, 5)
     b = nifti.vol_to_mat(a)
-    c = b.reshape(a.shape, order='F')
+    c = b.reshape(a.shape, order="F")
 
     assert b.ndim == 1
     assert b.shape == prod(a.shape)
     assert (a == c).all()
 
 
 def test_mat_to_vol():
     a = rand(3, 4, 5, 6)
-    b = a.reshape((60, 6), order='F')
+    b = a.reshape((60, 6), order="F")
     c = nifti.mat_to_vol(b, asdata=a)
 
     assert c.ndim == 4
     assert c.shape == a.shape
     assert (a == c).all()
 
     c = nifti.mat_to_vol(b, shape=a.shape)
@@ -54,15 +53,15 @@
     b = nifti.apply_mask(a, m)
     assert (b == a[1, :]).all()
 
 
 def test_unmask():
     m = asarray([0, 1, 0])
     a = rand(3)
-    b = zeros([3, 3], dtype='float32')
+    b = zeros([3, 3], dtype="float32")
     b[1, :] = a
 
     c = nifti.unmask(a, m, shape=b.shape)
 
     assert c.ndim == 2
     assert c.shape == b.shape
     assert (c == b).all()
@@ -78,16 +77,16 @@
     assert c.shape == b.shape
 
 
 def test_apply_atlas():
     m = asarray([0, 1, 1, 1, 1, 1])
     a = asarray([1, 2, 2, 3, 3, 0])
     d = rand(6, 10)
-    c = zeros((3, 10), dtype='float32')
-    cm = zeros((2, 10), dtype='float32')
+    c = zeros((3, 10), dtype="float32")
+    cm = zeros((2, 10), dtype="float32")
     c[0, :] = d[0, :]
     c[1, :] = d[1:3, :].mean(axis=0)
     c[2, :] = d[3:5, :].mean(axis=0)
     cm[0, :] = d[1:3, :].mean(axis=0)
     cm[1, :] = d[3:5, :].mean(axis=0)
 
     r = nifti.apply_atlas(d, a)
@@ -101,16 +100,16 @@
 
 
 def test_unfold_atlas():
     m = asarray([0, 1, 1, 1, 1, 1])
     a = asarray([1, 2, 2, 3, 3, 0])
     c = rand(3, 10)
     cm = rand(2, 10)
-    da = zeros((6, 10), dtype='float32')
-    dm = zeros((6, 10), dtype='float32')
+    da = zeros((6, 10), dtype="float32")
+    dm = zeros((6, 10), dtype="float32")
     label = unique(a)
     label = label[label > 0]
     for n, l in enumerate(label):
         da[a == l] = c[n, :]
     label = label[label > 1]
     for n, l in enumerate(label):
         dm[a == l] = cm[n, :]
@@ -125,83 +124,83 @@
     assert (rm == dm).all()
 
 
 # ### Break tests
 def test_break_mat_to_vol():
     with raises(ValueError) as errorinfo:
         nifti.mat_to_vol(rand(3))
-    assert 'Both shape' in str(errorinfo.value)
+    assert "Both shape" in str(errorinfo.value)
 
 
 def test_break_apply_mask():
     a = rand(3, 2, 5)
     m = rand(2, 2)
     with raises(ValueError) as errorinfo:
         nifti.apply_mask(a, m)
-    assert f'shape {a.shape}' in str(errorinfo.value)
-    assert f'shape {m.shape}' in str(errorinfo.value)
+    assert f"shape {a.shape}" in str(errorinfo.value)
+    assert f"shape {m.shape}" in str(errorinfo.value)
 
 
 def test_break_unmask():
     a = rand(6, 5)
     m = rand(3)
     b = rand(2, 3, 5)
 
     with raises(ValueError) as errorinfo:
         nifti.unmask(a, m)
-    assert 'shape and asdata' in str(errorinfo.value)
+    assert "shape and asdata" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         nifti.unmask(a, m, shape=(2, 3))
-    assert 'shape (2, 3)' in str(errorinfo.value)
-    assert f'shape {m.shape}' in str(errorinfo.value)
+    assert "shape (2, 3)" in str(errorinfo.value)
+    assert f"shape {m.shape}" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         nifti.unmask(a, m, asdata=b)
-    assert f'shape {b.shape}' in str(errorinfo.value)
-    assert f'shape {m.shape}' in str(errorinfo.value)
+    assert f"shape {b.shape}" in str(errorinfo.value)
+    assert f"shape {m.shape}" in str(errorinfo.value)
 
     m = asarray([0, 0, 1, 0, 1, 1])
     with raises(ValueError) as errorinfo:
         nifti.unmask(a, m, shape=(6, 5))
-    assert f'{m.sum()} entries' in str(errorinfo.value)
+    assert f"{m.sum()} entries" in str(errorinfo.value)
 
 
 def test_break_apply_atlas():
     d = rand(2, 3, 4, 5)
     a = rand(3, 2, 4)
     b = rand(2, 3, 4)
     m = rand(3, 2, 4)
     with raises(NotImplementedError) as errorinfo:
         nifti.apply_atlas(d, d)
-    assert f'Files with {d.ndim}' in str(errorinfo.value)
+    assert f"Files with {d.ndim}" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         nifti.apply_atlas(d, b, m)
-    assert f'shape {d.shape}' in str(errorinfo.value)
-    assert f'mask with shape {m.shape}' in str(errorinfo.value)
+    assert f"shape {d.shape}" in str(errorinfo.value)
+    assert f"mask with shape {m.shape}" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         nifti.apply_atlas(d, a, b)
-    assert f'atlas with shape {a.shape}' in str(errorinfo.value)
-    assert f'shape {d.shape}' in str(errorinfo.value)
+    assert f"atlas with shape {a.shape}" in str(errorinfo.value)
+    assert f"shape {d.shape}" in str(errorinfo.value)
 
 
 def test_break_unfold_atlas():
     d = rand(6, 5)
     a = rand(2, 3, 4)
     m = rand(3)
     with raises(ValueError) as errorinfo:
         nifti.unfold_atlas(d, a, m)
-    assert f'{m.ndim}D mask on {a.ndim}D atlas' in str(errorinfo.value)
+    assert f"{m.ndim}D mask on {a.ndim}D atlas" in str(errorinfo.value)
 
     m = rand(3, 3)
     with raises(ValueError) as errorinfo:
         nifti.unfold_atlas(d, a, m)
-    assert f'atlas with shape {a.shape}' in str(errorinfo.value)
-    assert 'mask with shape (3, 3, 1)' in str(errorinfo.value)
+    assert f"atlas with shape {a.shape}" in str(errorinfo.value)
+    assert "mask with shape (3, 3, 1)" in str(errorinfo.value)
 
     a = asarray([0, 1, 2])
     with raises(ValueError) as errorinfo:
         nifti.unfold_atlas(d, a)
-    assert f'data with shape {d.shape}' in str(errorinfo.value)
-    assert '2 parcels' in str(errorinfo.value)
+    assert f"data with shape {d.shape}" in str(errorinfo.value)
+    assert "2 parcels" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/tests/conftest.py` & `nigsp-0.9.0/nigsp/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,58 +29,56 @@
     Returns
     -------
     full_path : str
         Full path to downloaded `filename`
     """
     # This restores the same behavior as before.
     # this three lines make tests dowloads work in windows
-    if os.name == 'nt':
+    if os.name == "nt":
         orig_sslsocket_init = ssl.SSLSocket.__init__
-        ssl.SSLSocket.__init__ = lambda *args, cert_reqs=ssl.CERT_NONE, **kwargs: orig_sslsocket_init(*args, cert_reqs=ssl.CERT_NONE, **kwargs)
+        ssl.SSLSocket.__init__ = (
+            lambda *args, cert_reqs=ssl.CERT_NONE, **kwargs: orig_sslsocket_init(
+                *args, cert_reqs=ssl.CERT_NONE, **kwargs
+            )
+        )
         ssl._create_default_https_context = ssl._create_unverified_context
-    url = 'https://osf.io/{}/download'.format(osf_id)
+    url = "https://osf.io/{}/download".format(osf_id)
     full_path = os.path.join(path, filename)
     if not os.path.isfile(full_path):
         urlretrieve(url, full_path)
     return full_path
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def testdir(tmp_path_factory):
     """Test path that will be used to download all files."""
     return tmp_path_factory.getbasetemp()
 
 
 @pytest.fixture
 def atlas(testdir):
-    return fetch_file('h6nj7', testdir,
-                      'atlas.nii.gz')
+    return fetch_file("h6nj7", testdir, "atlas.nii.gz")
 
 
 @pytest.fixture
 def atlastime(testdir):
-    return fetch_file('ts6a8', testdir,
-                      'ats.nii.gz')
+    return fetch_file("ts6a8", testdir, "ats.nii.gz")
 
 
 @pytest.fixture
 def mean_fc(testdir):
-    return fetch_file('jrg8d', testdir,
-                      'mean_fc_matlab.tsv')
+    return fetch_file("jrg8d", testdir, "mean_fc_matlab.tsv")
 
 
 @pytest.fixture
 def sdi(testdir):
-    return fetch_file('rs4dn', testdir,
-                      'SDI_matlab.tsv')
+    return fetch_file("rs4dn", testdir, "SDI_matlab.tsv")
 
 
 @pytest.fixture
 def sc_mtx(testdir):
-    return fetch_file('vwh75', testdir,
-                      'sc.mat')
+    return fetch_file("vwh75", testdir, "sc.mat")
 
 
 @pytest.fixture
 def timeseries(testdir):
-    return fetch_file('ay8df', testdir,
-                      'func.mat')
+    return fetch_file("ay8df", testdir, "func.mat")
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_metrics.py` & `nigsp-0.9.0/nigsp/tests/test_metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,82 +9,90 @@
 
 # ### Unit tests
 def test_sdi():
 
     ts1 = np.arange(1, 3)[..., np.newaxis]
     ts2 = np.arange(3, 5)[..., np.newaxis]
     ts3 = np.arange(5, 7)[..., np.newaxis]
-    sdi_in = np.log2(np.arange(3., 1., -1.))
+    sdi_in = np.log2(np.arange(3.0, 1.0, -1.0))
 
-    ts = {'low': ts1, 'high': ts2}
+    ts = {"low": ts1, "high": ts2}
     sdi_out = metrics.sdi(ts)
     assert (sdi_out == sdi_in).all()
 
-    ts = {'HIGH': ts2, 'LOW': ts1}
+    ts = {"HIGH": ts2, "LOW": ts1}
     sdi_out = metrics.sdi(ts)
     assert (sdi_out == sdi_in).all()
 
-    ts = {'alpha': ts1, 'beta': ts2, 'gamma': ts3}
-    sdi_out = metrics.sdi(ts, keys=['alpha', 'beta'])
+    ts = {"alpha": ts1, "beta": ts2, "gamma": ts3}
+    sdi_out = metrics.sdi(ts, keys=["alpha", "beta"])
     assert (sdi_out == sdi_in).all()
 
-    ts = {'low': np.repeat(np.repeat(ts1[..., np.newaxis], 3, axis=1), 3, axis=2),
-          'high': np.repeat(np.repeat(ts2[..., np.newaxis], 3, axis=1), 3, axis=2)}
+    ts = {
+        "low": np.repeat(np.repeat(ts1[..., np.newaxis], 3, axis=1), 3, axis=2),
+        "high": np.repeat(np.repeat(ts2[..., np.newaxis], 3, axis=1), 3, axis=2),
+    }
     sdi_out = metrics.sdi(ts, mean=True)
     sdi_out = np.around(sdi_out, decimals=15)
     assert (sdi_out == sdi_in).all()
 
 
 def test_gsdi():
     ts1 = np.arange(1, 3)[..., np.newaxis]
     ts2 = np.arange(3, 5)[..., np.newaxis]
     ts3 = np.arange(5, 7)[..., np.newaxis]
-    ts = {'alpha': ts1, 'beta': ts2, 'gamma': ts3}
-    gsdi_in = np.log2(np.arange(3., 1., -1.))
-    gsdi_and_in = np.log2(np.linalg.norm(ts1, axis=1) / np.linalg.norm(np.add(ts2, ts3), axis=1))
-    keys_in = ['alpha_over_beta', 'alpha_over_gamma', 'alpha_over_(beta_and_gamma)', 
+    ts = {"alpha": ts1, "beta": ts2, "gamma": ts3}
+    gsdi_in = np.log2(np.arange(3.0, 1.0, -1.0))
+    gsdi_and_in = np.log2(
+        np.linalg.norm(ts1, axis=1) / np.linalg.norm(np.add(ts2, ts3), axis=1)
+    )
+    # fmt: off
+    keys_in = ['alpha_over_beta', 'alpha_over_gamma', 'alpha_over_(beta_and_gamma)',
                'beta_over_alpha', 'beta_over_gamma', 'beta_over_(alpha_and_gamma)',
                'gamma_over_alpha', 'gamma_over_beta', 'gamma_over_(alpha_and_beta)']
+    # fmt: on
     gsdi_out = metrics.gsdi(ts)
 
     assert all(item in keys_in for item in list(gsdi_out.keys()))
-    assert (gsdi_out['beta_over_alpha'] == gsdi_in).all()
-    assert (gsdi_out['alpha_over_(beta_and_gamma)'] == gsdi_and_in).all()
+    assert (gsdi_out["beta_over_alpha"] == gsdi_in).all()
+    assert (gsdi_out["alpha_over_(beta_and_gamma)"] == gsdi_and_in).all()
 
-    gsdi_out = metrics.gsdi(ts, keys=['alpha', 'beta'])
-    assert all(item in list(gsdi_out.keys()) for item in ['alpha_over_beta',
-                                                          'beta_over_alpha'])
-    assert (gsdi_out['beta_over_alpha'] == gsdi_in).all()
-
-    ts = {'alpha': np.repeat(np.repeat(ts1[..., np.newaxis], 3, axis=1), 3, axis=2),
-          'beta': np.repeat(np.repeat(ts2[..., np.newaxis], 3, axis=1), 3, axis=2)}
+    gsdi_out = metrics.gsdi(ts, keys=["alpha", "beta"])
+    assert all(
+        item in list(gsdi_out.keys()) for item in ["alpha_over_beta", "beta_over_alpha"]
+    )
+    assert (gsdi_out["beta_over_alpha"] == gsdi_in).all()
+
+    ts = {
+        "alpha": np.repeat(np.repeat(ts1[..., np.newaxis], 3, axis=1), 3, axis=2),
+        "beta": np.repeat(np.repeat(ts2[..., np.newaxis], 3, axis=1), 3, axis=2),
+    }
     gsdi_out = metrics.gsdi(ts, mean=True)
-    gsdi_out['beta_over_alpha'] = np.around(gsdi_out['beta_over_alpha'],
-                                            decimals=15)
-    assert (gsdi_out['beta_over_alpha'] == gsdi_in).all()
+    gsdi_out["beta_over_alpha"] = np.around(gsdi_out["beta_over_alpha"], decimals=15)
+    assert (gsdi_out["beta_over_alpha"] == gsdi_in).all()
 
 
 # ### Break tests
 def test_break_sdi():
     ts1 = np.arange(1, 3)[..., np.newaxis]
     ts2 = np.arange(3, 5)[..., np.newaxis]
     ts3 = np.arange(5, 7)[..., np.newaxis]
-    ts = {'alpha': ts1, 'beta': ts2, 'gamma': ts3}
+    ts = {"alpha": ts1, "beta": ts2, "gamma": ts3}
 
     with raises(ValueError) as errorinfo:
-        metrics.sdi(ts, keys=['high', 'low'])
-    assert 'provided keys' in str(errorinfo.value)
+        metrics.sdi(ts, keys=["high", "low"])
+    assert "provided keys" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         metrics.sdi(ts)
-    assert 'exactly two' in str(errorinfo.value)
+    assert "exactly two" in str(errorinfo.value)
 
 
 def test_break_gsdi():
     ts1 = np.arange(1, 3)[..., np.newaxis]
     ts2 = np.arange(3, 5)[..., np.newaxis]
     ts3 = np.arange(5, 7)[..., np.newaxis]
-    ts = {'alpha': ts1, 'beta': ts2, 'gamma': ts3}
+    ts = {"alpha": ts1, "beta": ts2, "gamma": ts3}
 
     with raises(ValueError) as errorinfo:
-        metrics.gsdi(ts, keys=['physio', 'lambda', 'pi'])
-    assert 'provided keys' in str(errorinfo.value)
+        metrics.gsdi(ts, keys=["physio", "lambda", "pi"])
+    assert "provided keys" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_viz.py` & `nigsp-0.9.0/nigsp/tests/test_viz.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,105 +10,98 @@
 from numpy import genfromtxt
 from numpy.random import rand
 from pytest import mark, raises
 
 from nigsp import viz
 
 
-@mark.parametrize('mtx', [
-    (rand(3, 4)),
-    (rand(4, 4)),
-    (rand(4, 4, 3)),
-    (rand(4, 4, 3, 1))
-])
+@mark.parametrize(
+    "mtx", [(rand(3, 4)), (rand(4, 4)), (rand(4, 4, 3)), (rand(4, 4, 3, 1))]
+)
 # ### Unit tests
 def test_plot_connectivity(mtx):
-    viz.plot_connectivity(mtx, 'annie.png', closeplot=True)
+    viz.plot_connectivity(mtx, "annie.png", closeplot=True)
 
-    assert isfile('annie.png')
+    assert isfile("annie.png")
     matplotlib.pyplot.close()
-    remove('annie.png')
+    remove("annie.png")
 
 
-@mark.parametrize('timeseries', [
-    (rand(3, 50)),
-    (rand(3, 50, 3)),
-    (rand(3, 50, 4, 1))
-])
+@mark.parametrize("timeseries", [(rand(3, 50)), (rand(3, 50, 3)), (rand(3, 50, 4, 1))])
 def test_plot_grayplot(timeseries):
-    viz.plot_grayplot(timeseries, 'troy.png', closeplot=True)
+    viz.plot_grayplot(timeseries, "troy.png", closeplot=True)
 
-    assert isfile('troy.png')
+    assert isfile("troy.png")
     matplotlib.pyplot.close()
-    remove('troy.png')
+    remove("troy.png")
 
 
 def test_plot_nodes(sdi, atlas):
     ns = genfromtxt(sdi)
-    viz.plot_nodes(ns, atlas, 'abed.png', closeplot=True)
+    viz.plot_nodes(ns, atlas, "abed.png", closeplot=True)
 
-    assert isfile('abed.png')
+    assert isfile("abed.png")
     matplotlib.pyplot.close()
-    remove('abed.png')
+    remove("abed.png")
     remove(sdi)
     remove(atlas)
 
 
 # ### Break tests
 def test_break_plot_connectivity():
-    sys.modules['matplotlib'] = None
+    sys.modules["matplotlib"] = None
     with raises(ImportError) as errorinfo:
-        viz.plot_connectivity(rand(3, 3), 'craig.png')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['matplotlib'] = matplotlib
+        viz.plot_connectivity(rand(3, 3), "craig.png")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["matplotlib"] = matplotlib
 
     with raises(ValueError) as errorinfo:
-        viz.plot_connectivity(rand(3, 3, 3, 4), 'craig.png')
-    assert 'plot connectivity' in str(errorinfo.value)
+        viz.plot_connectivity(rand(3, 3, 3, 4), "craig.png")
+    assert "plot connectivity" in str(errorinfo.value)
 
     matplotlib.pyplot.close()
 
 
 def test_break_plot_grayplot():
-    sys.modules['matplotlib'] = None
+    sys.modules["matplotlib"] = None
     with raises(ImportError) as errorinfo:
-        viz.plot_grayplot(rand(3, 3), 'dan.png')
-    assert 'is required' in str(errorinfo.value)
-    sys.modules['matplotlib'] = matplotlib
+        viz.plot_grayplot(rand(3, 3), "dan.png")
+    assert "is required" in str(errorinfo.value)
+    sys.modules["matplotlib"] = matplotlib
 
     with raises(ValueError) as errorinfo:
-        viz.plot_grayplot(rand(3, 3, 3, 4), 'dan.png')
-    assert 'plot grayplots' in str(errorinfo.value)
+        viz.plot_grayplot(rand(3, 3, 3, 4), "dan.png")
+    assert "plot grayplots" in str(errorinfo.value)
 
     matplotlib.pyplot.close()
 
 
 def test_break_plot_nodes(atlas):
-    sys.modules['matplotlib'] = None
+    sys.modules["matplotlib"] = None
     with raises(ImportError) as errorinfo:
         viz.plot_nodes(rand(3), rand(3, 3))
-    assert 'are required' in str(errorinfo.value)
-    sys.modules['matplotlib'] = matplotlib
+    assert "are required" in str(errorinfo.value)
+    sys.modules["matplotlib"] = matplotlib
 
-    sys.modules['nilearn.plotting'] = None
+    sys.modules["nilearn.plotting"] = None
     with raises(ImportError) as errorinfo:
         viz.plot_nodes(rand(3), rand(3, 3))
-    assert 'are required' in str(errorinfo.value)
-    sys.modules['nilearn.plotting'] = nilearn.plotting
+    assert "are required" in str(errorinfo.value)
+    sys.modules["nilearn.plotting"] = nilearn.plotting
 
     with raises(ValueError) as errorinfo:
         viz.plot_nodes(rand(3, 3, 4), rand(3, 3))
-    assert 'plot node values' in str(errorinfo.value)
+    assert "plot node values" in str(errorinfo.value)
 
     with raises(NotImplementedError) as errorinfo:
         viz.plot_nodes(rand(3), rand(3, 3, 2))
-    assert 'atlases in nifti' in str(errorinfo.value)
+    assert "atlases in nifti" in str(errorinfo.value)
     with raises(NotImplementedError) as errorinfo:
         viz.plot_nodes(rand(3), rand(3, 4))
-    assert 'atlases in nifti' in str(errorinfo.value)
+    assert "atlases in nifti" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         viz.plot_nodes(rand(3), rand(4, 3))
-    assert 'different length' in str(errorinfo.value)
+    assert "different length" in str(errorinfo.value)
 
     matplotlib.pyplot.close()
     remove(atlas)
```

### Comparing `nigsp-0.8.0/nigsp/tests/test_objects.py` & `nigsp-0.9.0/nigsp/tests/test_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 #!/usr/bin/env python3
 """Tests for objects."""
 
 import numpy as np
 from numpy.random import rand
-
 from pytest import raises
 
 from nigsp import operations
 from nigsp.objects import SCGraph
 
 
 # ### Unit tests
 def test_SCGraph():
     """Test SCGraph, properties, and methods."""
     # # Initialise object
     # Initialise content
     mtx = rand(4, 4)
     timeseries = rand(4, 6)
     atlas = rand(4, 3)
-    filename = 'Laudna.nii.gz'
-    ts_split = {'high': rand(4, 6), 'low': rand(4, 6)}
+    filename = "Laudna.nii.gz"
+    ts_split = {"high": rand(4, 6), "low": rand(4, 6)}
     # Initialise eigenvec to check zerocross
     def _bonnet(d, x):
-        if(d == 0):
+        if d == 0:
             return np.ones_like(x)
-        elif(d == 1):
+        elif d == 1:
             return x
         else:
-            return ((2*d-1)*x*_bonnet(d-1, x)-(d-1)*_bonnet(d-2, x))/d
+            return (
+                (2 * d - 1) * x * _bonnet(d - 1, x) - (d - 1) * _bonnet(d - 2, x)
+            ) / d
 
     x = np.linspace(-1, 1, 4)
-    eigenvec = np.empty([4, 4], dtype='float32')
+    eigenvec = np.empty([4, 4], dtype="float32")
     for n in range(4):
         eigenvec[:, n] = _bonnet(n, x)
     zx = np.linspace(0, 3, 4)
 
     # Initialise SCGraph proper
-    scgraph = SCGraph(mtx, timeseries, atlas=atlas, filename=filename,
-                      eigenvec=eigenvec, ts_split=ts_split, index=2)
+    scgraph = SCGraph(
+        mtx,
+        timeseries,
+        atlas=atlas,
+        filename=filename,
+        eigenvec=eigenvec,
+        ts_split=ts_split,
+        index=2,
+    )
 
     # # Assert properties
     assert scgraph.nnodes == mtx.shape[1]
     assert scgraph.ntimepoints == timeseries.shape[1]
     assert (scgraph.zerocross == zx).all()
     assert all(item in scgraph.split_keys for item in list(ts_split.keys()))
 
@@ -53,60 +61,60 @@
     scgraph.split_graph()
     evs, tss = operations.graph_filter(timeseries, eigenvec, 2)
     # Update ts_split to be tss
     ts_split = tss
 
     assert all(item in list(evs.keys()) for item in list(scgraph.evec_split.keys()))
     assert all(item in list(tss.keys()) for item in list(scgraph.ts_split.keys()))
-    assert (evs['low'] == scgraph.evec_split['low']).all()
-    assert (tss['low'] == scgraph.ts_split['low']).all()
+    assert (evs["low"] == scgraph.evec_split["low"]).all()
+    assert (tss["low"] == scgraph.ts_split["low"]).all()
 
     scgraph.evec_split = {}
-    scgraph.index = 'median'
+    scgraph.index = "median"
     scgraph.split_graph(index=2)
 
-    assert (evs['low'] == scgraph.evec_split['low']).all()
+    assert (evs["low"] == scgraph.evec_split["low"]).all()
 
     # Test create_surrogates
-    scgraph.create_surrogates(sc_type='informed', n_surr=1, seed=6)
+    scgraph.create_surrogates(sc_type="informed", n_surr=1, seed=6)
     i_surr = operations.sc_informed(timeseries, eigenvec, n_surr=1, seed=6)
     assert (scgraph.surr == i_surr).all()
 
     scgraph.lapl_mtx = mtx
-    scgraph.create_surrogates(sc_type='uninformed', n_surr=1, seed=6)
+    scgraph.create_surrogates(sc_type="uninformed", n_surr=1, seed=6)
     u_surr = operations.sc_uninformed(timeseries, lapl_mtx=mtx, n_surr=1, seed=6)
     assert (scgraph.surr == u_surr).all()
 
     # Test compute_fc
     scgraph.compute_fc()
     fc = operations.functional_connectivity(timeseries)
-    fc_low = operations.functional_connectivity(ts_split['low'])
+    fc_low = operations.functional_connectivity(ts_split["low"])
 
     assert (fc == scgraph.fc).all()
-    assert all(item in ['high', 'low'] for item in list(scgraph.fc_split.keys()))
-    assert (fc_low == scgraph.fc_split['low']).all()
+    assert all(item in ["high", "low"] for item in list(scgraph.fc_split.keys()))
+    assert (fc_low == scgraph.fc_split["low"]).all()
 
 
 # ### Break tests
 def test_break_SCGraph():
     """Break SCGraph and its methods."""
     with raises(ValueError) as errorinfo:
         SCGraph(rand(3, 4), rand(4, 6))
-    assert 'square matrix' in str(errorinfo.value)
+    assert "square matrix" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         SCGraph(rand(4, 4), rand(3, 6))
-    assert 'number of parcels and nodes' in str(errorinfo.value)
+    assert "number of parcels and nodes" in str(errorinfo.value)
 
     with raises(ValueError) as errorinfo:
         SCGraph(rand(4, 4), rand(4, 6, 4, 5))
-    assert 'more than 3 dimensions' in str(errorinfo.value)
+    assert "more than 3 dimensions" in str(errorinfo.value)
 
-    scgraph = SCGraph(rand(4, 4), rand(4, 6), index='Chet')
+    scgraph = SCGraph(rand(4, 4), rand(4, 6), index="Chet")
     with raises(ValueError) as errorinfo:
         scgraph.split_graph()
-    assert 'Unknown option Chet' in str(errorinfo.value)
+    assert "Unknown option Chet" in str(errorinfo.value)
 
     scgraph = SCGraph(rand(4, 4), rand(4, 6))
     with raises(ValueError) as errorinfo:
-        scgraph.create_surrogates(sc_type='Fearne')
-    assert 'Unknown option Fearne' in str(errorinfo.value)
+        scgraph.create_surrogates(sc_type="Fearne")
+    assert "Unknown option Fearne" in str(errorinfo.value)
```

### Comparing `nigsp-0.8.0/nigsp/io.py` & `nigsp-0.9.0/nigsp/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,30 +13,28 @@
 EXT_XLS : list
     List of supported XLS-like file extensions, in lower case.
 LGR
     Logger
 """
 
 import logging
-
 from os import makedirs
 from os.path import exists, join
 
 import numpy as np
 
 from nigsp.utils import change_var_type
 
-
-EXT_1D = ['.txt', '.csv', '.tsv', '.1d', '.par', '.tsv.gz', '.csv.gz']
-EXT_XLS = ['.xls']
-EXT_MAT = ['.mat']
-EXT_NIFTI = ['.nii', '.nii.gz']
+EXT_1D = [".txt", ".csv", ".tsv", ".1d", ".par", ".tsv.gz", ".csv.gz"]
+EXT_XLS = [".xls"]
+EXT_MAT = [".mat"]
+EXT_NIFTI = [".nii", ".nii.gz"]
 EXT_ALL = EXT_1D + EXT_XLS + EXT_MAT + EXT_NIFTI
 
-EXT_DICT = {'1D': EXT_1D, 'xls': EXT_XLS, 'mat': EXT_MAT, 'nifti': EXT_NIFTI}
+EXT_DICT = {"1D": EXT_1D, "xls": EXT_XLS, "mat": EXT_MAT, "nifti": EXT_NIFTI}
 
 LGR = logging.getLogger(__name__)
 
 
 def check_ext(all_ext, fname, scan=False, remove=False):
     """
     Check which extension a file has, and possibly remove it.
@@ -65,32 +63,32 @@
             If both `remove` and `has_ext` are True, returns also found extension
     """
     has_ext = False
     all_ext = change_var_type(all_ext, list, stop=False, silent=True)
     for ext in all_ext:
         if fname.lower().endswith(ext):
             has_ext = True
-            LGR.debug(f'{fname} ends with extension {ext}')
+            LGR.debug(f"{fname} ends with extension {ext}")
             break
 
     if not has_ext and scan:
         for ext in all_ext:
-            if exists(f'{fname}{ext}'):
-                fname = f'{fname}{ext}'
-                LGR.warning(f'Found {fname}{ext}, using it as input henceforth')
+            if exists(f"{fname}{ext}"):
+                fname = f"{fname}{ext}"
+                LGR.warning(f"Found {fname}{ext}, using it as input henceforth")
                 has_ext = True
                 break
 
     obj_return = [has_ext]
 
     if remove:
         if has_ext:
-            obj_return += [fname[:-len(ext)], ext]  # case insensitive solution
+            obj_return += [fname[: -len(ext)], ext]  # case insensitive solution
         else:
-            obj_return += [fname, '']
+            obj_return += [fname, ""]
     else:
         obj_return += [fname]
 
     return obj_return[:]
 
 
 def check_nifti_dim(fname, data, dim=4):
@@ -115,16 +113,18 @@
     ------
     ValueError
         If `data` has different dimensions than `dim`
     """
     data = data.squeeze()
 
     if data.ndim != dim:
-        raise ValueError(f'A {dim}D nifti file is required, but {fname} is '
-                         f'{data.ndim}D. Please check the input file.')
+        raise ValueError(
+            f"A {dim}D nifti file is required, but {fname} is "
+            f"{data.ndim}D. Please check the input file."
+        )
 
     return data
 
 
 def check_mtx_dim(fname, data, shape=None):
     """
     Check dimensions of a matrix.
@@ -138,44 +138,50 @@
     shape : None, 'square', or 'rectangle'}, str, optional
         Shape of matrix, if empty, skip shape check
 
     Returns
     -------
     np.ndarray
         If `data.ndim` = 2, returns data.
-        If `data.ndim` = 1 and `shape` == 'rectangle', 
+        If `data.ndim` = 1 and `shape` == 'rectangle',
         Returns data with added empty axis.
 
     Raises
     ------
     NotImplementedError
         If `data` has more than 3 dimensions.
         If `shape` is not None but `data` is 3D.
     ValueError
         If `data` is empty
         If `shape` == 'square' and `data` dimensions have different lenghts.
     """
     data = data.squeeze()
-    LGR.info('Checking data shape.')
+    LGR.info("Checking data shape.")
 
     if data.shape[0] == 0:
-        raise ValueError(f'{fname} is empty!')
+        raise ValueError(f"{fname} is empty!")
     if data.ndim > 3:
-        raise NotImplementedError('Only matrices up to 3D are supported, but '
-                                  f'given matrix is {data.ndim}D.')
+        raise NotImplementedError(
+            "Only matrices up to 3D are supported, but "
+            f"given matrix is {data.ndim}D."
+        )
     if shape is not None:
         if data.ndim > 2:
-            raise NotImplementedError('Cannot check shape of 3D matrix.')
-        if data.ndim == 1 and shape == 'rectangle':
+            raise NotImplementedError("Cannot check shape of 3D matrix.")
+        if data.ndim == 1 and shape == "rectangle":
             data = data[..., np.newaxis]
-            LGR.warning(f'Rectangular matrix required, but {fname} is a vector. '
-                        'Adding empty dimension.')
-        if shape == 'square' and data.shape[0] != data.shape[1]:
-            raise ValueError(f'Square matrix required, but {fname} matrix has '
-                             f'shape {data.shape}.')
+            LGR.warning(
+                f"Rectangular matrix required, but {fname} is a vector. "
+                "Adding empty dimension."
+            )
+        if shape == "square" and data.shape[0] != data.shape[1]:
+            raise ValueError(
+                f"Square matrix required, but {fname} matrix has "
+                f"shape {data.shape}."
+            )
 
     return data
 
 
 def load_nifti_get_mask(fname, is_mask=False, ndim=4):
     """
     Load a nifti file and returns its data, its image, and a 3d mask.
@@ -202,28 +208,30 @@
     img : nib.img
         Image object from nibabel.
 
     """
     try:
         import nibabel as nib
     except ImportError:
-        raise ImportError('nibabel is required to import nifti files. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "nibabel is required to import nifti files. "
+            "Please see install instructions."
+        )
 
-    LGR.info(f'Loading {fname}.')
+    LGR.info(f"Loading {fname}.")
     img = nib.load(fname)
     data = img.get_fdata()
     data = check_nifti_dim(fname, data, dim=ndim)
 
     if is_mask:
-        mask = (data != 0)
-        LGR.info(f'{fname} loaded as mask.')
+        mask = data != 0
+        LGR.info(f"{fname} loaded as mask.")
     else:
         mask = data.any(axis=-1).squeeze()
-        LGR.info(f'Data loaded from {fname}.')
+        LGR.info(f"Data loaded from {fname}.")
 
     return data, mask, img
 
 
 def load_txt(fname, shape=None):
     """
     Read files in textual format.
@@ -240,40 +248,40 @@
     mtx : numpy.ndarray
         Data matrix
 
     See also
     --------
     check_mtx_dim
     """
-    LGR.info(f'Loading {fname}.')
+    LGR.info(f"Loading {fname}.")
 
     _, _, ext = check_ext(EXT_1D, fname, scan=True, remove=True)
 
-    if ext in ['.csv', '.csv.gz']:
-        delimiter = ','
-    elif ext in ['.tsv', '.tsv.gz']:
-        delimiter = '\t'
-    elif ext in ['.txt', '.1d', '.par']:
-        delimiter = ' '
+    if ext in [".csv", ".csv.gz"]:
+        delimiter = ","
+    elif ext in [".tsv", ".tsv.gz"]:
+        delimiter = "\t"
+    elif ext in [".txt", ".1d", ".par"]:
+        delimiter = " "
     else:
         delimiter = None
 
     mtx = np.genfromtxt(fname, delimiter=delimiter)
 
     mtx = check_mtx_dim(fname, mtx, shape)
 
     return mtx
 
 
 def load_mat(fname, shape=None):
     """
     Read files in matlab format.
 
-    Assumes the existence of a matrix/vector in the mat file, rendered as 
-    a numpy.ndarray. If there is more than a marix, the one with the largest 
+    Assumes the existence of a matrix/vector in the mat file, rendered as
+    a numpy.ndarray. If there is more than a marix, the one with the largest
     size will be selected.
 
     Parameters
     ----------
     fname : str or os.PathLike
         Path to the mat file
     shape : None, 'square', or 'rectangle'}, str, optional
@@ -298,48 +306,55 @@
         If the mat file does not contain matrix or vectors.
     ImportError
         If pymatreader is not installed or can't be read.
     """
     try:
         from pymatreader import read_mat
     except ImportError:
-        raise ImportError('pymatreader is required to import mat files. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "pymatreader is required to import mat files. "
+            "Please see install instructions."
+        )
 
-    LGR.info(f'Loading {fname}.')
+    LGR.info(f"Loading {fname}.")
     data = read_mat(fname)
 
     data_keys = []
     for k in data.keys():
         # Check data key only if it's not hidden
         # (skip '__header__', '__version__', '__global__')
-        if '__' not in k:
-            LGR.info(f'Checking {fname} key {str(k)} content for data (float array/matrices in MATLAB).')
+        if "__" not in k:
+            LGR.info(
+                f"Checking {fname} key {str(k)} content for data "
+                "(float array/matrices in MATLAB)."
+            )
             if type(data[k]) is np.ndarray:
                 data_keys.append(k)
 
     if len(data_keys) < 1:
-        raise EOFError(f'{fname} does not seem to contain a numeric matrix.')
+        raise EOFError(f"{fname} does not seem to contain a numeric matrix.")
     elif len(data_keys) > 1:
-        LGR.warning('Found multiple possible arrays to load. '
-                    'Selecting the biggest (highest pythonic size).')
+        LGR.warning(
+            "Found multiple possible arrays to load. "
+            "Selecting the biggest (highest pythonic size)."
+        )
 
     key = data_keys[0]
     for k in data_keys[1:]:
         if data[k].size > data[key].size:
             key = k
 
-    LGR.info(f'Selected data from MATLAB variable {key}')
+    LGR.info(f"Selected data from MATLAB variable {key}")
     mtx = data[key]
     mtx = check_mtx_dim(fname, mtx, shape)
 
     return mtx
 
 
-def load_xls(fname, shape=''):
+def load_xls(fname, shape=""):
     """
     Read files in xls format.
 
     Parameters
     ----------
     fname : str or os.PathLike
         Path to the mat file
@@ -355,15 +370,15 @@
     check_mtx_dim
 
     Raises
     ------
     NotImplementedError
         Spreadheet loading is not implemented yet.
     """
-    raise NotImplementedError('Spreadsheet loading is not implemented yet')
+    raise NotImplementedError("Spreadsheet loading is not implemented yet")
 
 
 def export_nifti(data, img, fname):
     """
     Export a nifti file.
 
     Parameters
@@ -374,28 +389,30 @@
         Nibabel image object
     fname : str or os.PathLike
         Name of the output file
     """
     try:
         import nibabel as nib
     except ImportError:
-        raise ImportError('nibabel is required to export nifti files. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "nibabel is required to export nifti files. "
+            "Please see install instructions."
+        )
 
     for e in EXT_NIFTI:
         has_ext, fname, ext = check_ext(e, fname, remove=True)
         if has_ext:
             break
 
-    if ext == '':
-        ext = '.nii.gz'
+    if ext == "":
+        ext = ".nii.gz"
 
-    LGR.info(f'Exporting nifti data into {fname}{ext}.')
+    LGR.info(f"Exporting nifti data into {fname}{ext}.")
     out_img = nib.Nifti1Image(data, img.affine, img.header)
-    out_img.to_filename(f'{fname}{ext}')
+    out_img.to_filename(f"{fname}{ext}")
 
     return 0
 
 
 def export_txt(data, fname, ext=None):
     """
     Export data into a text-like or mat file.
@@ -410,30 +427,34 @@
         Selected extension for export.
 
     Returns
     -------
     0
         On a successful run
     """
-    if ext.lower() in ['.csv', '.csv.gz', '', None]:
-        delimiter = ','
-    elif ext.lower() in ['.tsv', '.tsv.gz']:
-        delimiter = '\t'
-    elif ext.lower() in ['.txt', '.1d', '.par']:
-        delimiter = ' '
+    if ext.lower() in [".csv", ".csv.gz", "", None]:
+        delimiter = ","
+    elif ext.lower() in [".tsv", ".tsv.gz"]:
+        delimiter = "\t"
+    elif ext.lower() in [".txt", ".1d", ".par"]:
+        delimiter = " "
     else:
         delimiter = None
 
     if data.ndim < 3:
-        np.savetxt(f'{fname}{ext}', data, fmt='%.6f', delimiter=delimiter)
+        np.savetxt(f"{fname}{ext}", data, fmt="%.6f", delimiter=delimiter)
     elif data.ndim == 3:
         makedirs(fname, exist_ok=True)
         for i in range(data.shape[-1]):
-            np.savetxt(join(fname, f'{i:03d}{ext}'), data[:, :, i], fmt='%.6f',
-                       delimiter=delimiter)
+            np.savetxt(
+                join(fname, f"{i:03d}{ext}"),
+                data[:, :, i],
+                fmt="%.6f",
+                delimiter=delimiter,
+            )
 
     return 0
 
 
 def export_mtx(data, fname, ext=None):
     """
     Export data into a text-like or mat file.
@@ -473,37 +494,41 @@
             has_ext, fname, ext = check_ext(e, fname, remove=True)
             if has_ext:
                 break
     elif ext.lower() not in EXT_ALL:
         # Check if extension is supported.
         ext = None
 
-    if ext in [None, '']:
-        LGR.warning('Extension not specified, or specified extension not '
-                    'supported. Forcing export in CSV format.')
-        ext = '.csv'
+    if ext in [None, ""]:
+        LGR.warning(
+            "Extension not specified, or specified extension not "
+            "supported. Forcing export in CSV format."
+        )
+        ext = ".csv"
     elif ext.lower() in EXT_NIFTI:
-        LGR.warning('Found nifti extension, exporting data in .1D instead')
-        ext = '.1D'
+        LGR.warning("Found nifti extension, exporting data in .1D instead")
+        ext = ".1D"
 
-    LGR.info(f'Exporting data into {fname}{ext}.')
+    LGR.info(f"Exporting data into {fname}{ext}.")
     if ext.lower() in EXT_MAT:
         try:
             import scipy
         except ImportError:
-            raise ImportError('To export .mat files, scipy is required. '
-                              'Please install it.')
-        scipy.io.savemat(f'{fname}{ext}', {'data': data})
+            raise ImportError(
+                "To export .mat files, scipy is required. " "Please install it."
+            )
+        scipy.io.savemat(f"{fname}{ext}", {"data": data})
     elif ext.lower() in EXT_XLS:
-        raise NotImplementedError('Spreadsheet output is not implemented yet')
+        raise NotImplementedError("Spreadsheet output is not implemented yet")
     elif ext.lower() in EXT_1D:
         export_txt(data, fname, ext)
     else:
-        raise BrokenPipeError(f'This should not have happened: {ext} was the '
-                              'selected extension.')
+        raise BrokenPipeError(
+            f"This should not have happened: {ext} was the " "selected extension."
+        )
 
     return 0
 
 
 """
 Copyright 2022, Stefano Moia.
```

### Comparing `nigsp-0.8.0/nigsp/operations/nifti.py` & `nigsp-0.9.0/nigsp/operations/nifti.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Logger
 """
 
 import logging
 
 import numpy as np
 
-
 LGR = logging.getLogger(__name__)
 
 
 def vol_to_mat(data):
     """
     Reshape <3D in 1D or 4D into 2D.
 
@@ -26,16 +25,16 @@
         The data to be transformed into 2D.
 
     Returns
     -------
     numpy.ndarray
         2D reshaped data.
     """
-    LGR.info(f'Reshape {data.ndim}D volume into 1[+1]D (space[*time]) matrix.')
-    return data.reshape(((-1,) + data.shape[3:]), order='F')
+    LGR.info(f"Reshape {data.ndim}D volume into 1[+1]D (space[*time]) matrix.")
+    return data.reshape(((-1,) + data.shape[3:]), order="F")
 
 
 def mat_to_vol(data, shape=None, asdata=None):
     """
     Reshape nD data (normally 2D) using either shape or data shape).
 
     Parameters
@@ -55,23 +54,26 @@
     Raises
     ------
     ValueError
         If both shape and asdata are empty.
     """
     if asdata is not None:
         if shape is not None:
-            LGR.warning('Both shape and asdata were defined. '
-                        f'Overwriting shape {shape} with asdata {asdata.shape}')
+            LGR.warning(
+                "Both shape and asdata were defined. "
+                f"Overwriting shape {shape} with asdata {asdata.shape}"
+            )
         shape = asdata.shape
     elif shape is None:
-        raise ValueError('Both shape and asdata are empty. '
-                         'Must specify at least one')
+        raise ValueError(
+            "Both shape and asdata are empty. " "Must specify at least one"
+        )
 
-    LGR.info(f'Reshape {data.ndim}D matrix into volume with shape {shape}.')
-    return data.reshape(shape, order='F')
+    LGR.info(f"Reshape {data.ndim}D matrix into volume with shape {shape}.")
+    return data.reshape(shape, order="F")
 
 
 def apply_mask(data, mask):
     """
     Reduce shape and size of data based on mask.
 
     Uses the concept of "mask" as defined in neuroimaging, not in numpy:
@@ -90,23 +92,25 @@
         Masked (data.ndim-1 Dimensions) array.
 
     Raises
     ------
     ValueError
         If the first mask.ndim dimensions of data have a different shape from mask.
     """
-    if data.shape[:mask.ndim] != mask.shape:
-        raise ValueError(f'Cannot mask data with shape {data.shape} using mask '
-                         f'with shape {mask.shape}')
-    if (data.ndim-mask.ndim) > 1:
-        LGR.warning(f'Returning volume with {data.ndim-mask.ndim+1} dimensions.')
+    if data.shape[: mask.ndim] != mask.shape:
+        raise ValueError(
+            f"Cannot mask data with shape {data.shape} using mask "
+            f"with shape {mask.shape}"
+        )
+    if (data.ndim - mask.ndim) > 1:
+        LGR.warning(f"Returning volume with {data.ndim-mask.ndim+1} dimensions.")
     else:
-        LGR.info(f'Returning {data.ndim-mask.ndim+1}D array.')
+        LGR.info(f"Returning {data.ndim-mask.ndim+1}D array.")
 
-    mask = (mask != 0)
+    mask = mask != 0
     return data[mask]
 
 
 def unmask(data, mask, shape=None, asdata=None):
     """
     Unmask 1D or 2D into an nD based on shape or asdata.
 
@@ -127,38 +131,45 @@
     numpy.ndarray
         The unmasked nD array version of data.
 
     Raises
     ------
     ValueError
         If both `shape` and `asdata` are empty
-        If the first dimension of `data` and the number of available voxels in 
+        If the first dimension of `data` and the number of available voxels in
         mask do not match.
         If the mask shape does not match the first (mask)
     """
     if asdata is not None:
         if shape is not None:
-            LGR.warning('Both shape and asdata were defined. '
-                        f'Overwriting shape {shape} with asdata {asdata.shape}')
+            LGR.warning(
+                "Both shape and asdata were defined. "
+                f"Overwriting shape {shape} with asdata {asdata.shape}"
+            )
         shape = asdata.shape
     elif shape is None:
-        raise ValueError('Both shape and asdata are empty. '
-                         'Must specify at least one.')
-
-    if shape[:mask.ndim] != mask.shape:
-        raise ValueError(f'Cannot unmask data into shape {shape} using mask '
-                         f'with shape {mask.shape}')
+        raise ValueError(
+            "Both shape and asdata are empty. " "Must specify at least one."
+        )
+
+    if shape[: mask.ndim] != mask.shape:
+        raise ValueError(
+            f"Cannot unmask data into shape {shape} using mask "
+            f"with shape {mask.shape}"
+        )
     if data.ndim > 1 and (data.shape[0] != mask.sum()):
-        raise ValueError('Cannot unmask data with first dimension '
-                         f'{data.shape[0]} using mask with '
-                         f'{mask.sum()} entries)')
-
-    LGR.info(f'Unmasking matrix into volume of shape {shape}')
-    mask = (mask != 0)
-    out = np.zeros(shape, dtype='float32')
+        raise ValueError(
+            "Cannot unmask data with first dimension "
+            f"{data.shape[0]} using mask with "
+            f"{mask.sum()} entries)"
+        )
+
+    LGR.info(f"Unmasking matrix into volume of shape {shape}")
+    mask = mask != 0
+    out = np.zeros(shape, dtype="float32")
     out[mask] = data
     return out
 
 
 def apply_atlas(data, atlas, mask=None):
     """
     Extract average timeseries from an atlas.
@@ -184,39 +195,47 @@
     ValueError
         If atlas or mask have a different shape than the first dimensions of data
     """
     if mask is None:
         mask = (data != 0).any(axis=-1)
     else:
         # Ensure that mask is boolean
-        mask = (mask != 0)
+        mask = mask != 0
 
     # #!# Add nilearn's fetching atlases utility
 
     if atlas.ndim > 3:
-        raise NotImplementedError(f'Files with {atlas.ndim} dimensions are not supported as atlases.')
-    if data.shape[:mask.ndim] != mask.shape:
-        raise ValueError(f'Cannot mask data with shape {data.shape} using mask '
-                         f'with shape {mask.shape}')
-    if data.shape[:atlas.ndim] != atlas.shape:
-        raise ValueError(f'Cannot apply atlas with shape {atlas.shape} on data '
-                         f'with shape {data.shape}')
-    if (data.ndim-atlas.ndim) > 1:
-        LGR.warning(f'returning volume with {data.ndim-atlas.ndim+1} dimensions.')
+        raise NotImplementedError(
+            f"Files with {atlas.ndim} dimensions are not " "supported as atlases."
+        )
+    if data.shape[: mask.ndim] != mask.shape:
+        raise ValueError(
+            f"Cannot mask data with shape {data.shape} using mask "
+            f"with shape {mask.shape}"
+        )
+    if data.shape[: atlas.ndim] != atlas.shape:
+        raise ValueError(
+            f"Cannot apply atlas with shape {atlas.shape} on data "
+            f"with shape {data.shape}"
+        )
+    if (data.ndim - atlas.ndim) > 1:
+        LGR.warning(f"returning volume with {data.ndim-atlas.ndim+1} dimensions.")
     else:
-        LGR.info(f'Returning {data.ndim-atlas.ndim+1}D array of signal averages '
-                 f'in atlas {atlas}.')
+        LGR.info(
+            f"Returning {data.ndim-atlas.ndim+1}D array of signal averages "
+            f"in atlas {atlas}."
+        )
 
     # Mask data and atlas first
-    atlas = atlas*mask
+    atlas = atlas * mask
     labels = np.unique(atlas)
     labels = labels[labels > 0]
-    LGR.info(f'Labels: {labels}, numbers: {len(labels)}')
+    LGR.info(f"Labels: {labels}, numbers: {len(labels)}")
     # Initialise dataframe and dictionary for series
-    parcels = np.empty([len(labels), data.shape[-1]], dtype='float32')
+    parcels = np.empty([len(labels), data.shape[-1]], dtype="float32")
 
     # Compute averages
     for n, l in enumerate(labels):
         parcels[n, :] = data[atlas == l].mean(axis=0)
 
     return parcels
 
@@ -249,39 +268,43 @@
         If atlas and mask have dimensions that are too different (i.e. more than
         1 dimension of difference)
         If mask has different shapes from atlas.
         If the first dimension of the data is not equal to the amount of label
         in the atlas.
     """
     if mask is None:
-        mask = (atlas != 0)
+        mask = atlas != 0
     else:
         # Check that mask contains bool
-        mask = (mask != 0)
+        mask = mask != 0
 
     if (mask.ndim - atlas.ndim) == 1:
         atlas = atlas[..., np.newaxis]
     elif (atlas.ndim - mask.ndim) == 1:
         mask = mask[..., np.newaxis]
     elif abs(mask.ndim - atlas.ndim) > 1:
-        raise ValueError(f'Cannot use {mask.ndim}D mask on {atlas.ndim}D atlas.')
+        raise ValueError(f"Cannot use {mask.ndim}D mask on {atlas.ndim}D atlas.")
 
-    if atlas.shape[:mask.ndim] != mask.shape:
-        raise ValueError(f'Cannot mask atlas with shape {atlas.shape} using mask '
-                         f'with shape {mask.shape}')
-    atlas = atlas*mask
+    if atlas.shape[: mask.ndim] != mask.shape:
+        raise ValueError(
+            f"Cannot mask atlas with shape {atlas.shape} using mask "
+            f"with shape {mask.shape}"
+        )
+    atlas = atlas * mask
 
     labels = np.unique(atlas)
     labels = labels[labels > 0]
     if data.shape[0] != len(labels):
-        raise ValueError(f'Cannot unfold data with shape {data.shape} on atlas '
-                         f'with {len(labels)} parcels')
+        raise ValueError(
+            f"Cannot unfold data with shape {data.shape} on atlas "
+            f"with {len(labels)} parcels"
+        )
 
-    LGR.info(f'Unmasking data into atlas-like volume of {3+data.ndim-1} dimensions.')
-    out = np.zeros_like(atlas, dtype='float32')
+    LGR.info(f"Unmasking data into atlas-like volume of {3+data.ndim-1} dimensions.")
+    out = np.zeros_like(atlas, dtype="float32")
 
     for ax in range(1, data.ndim):
         if data.shape[ax] > 1:
             out = out[..., np.newaxis].repeat(data.shape[ax], axis=-1)
 
     for n, l in enumerate(labels):
         out[atlas == l] = data[n, ...]
```

### Comparing `nigsp-0.8.0/nigsp/operations/graph.py` & `nigsp-0.9.0/nigsp/operations/graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Logger
 """
 
 import logging
 
 from numpy import abs
 
-
 LGR = logging.getLogger(__name__)
 
 
 def zerocross(eigenvec):
     """
     Compute the amount of zero-crossing of an eigenvector matrix (for each eigenvector).
```

### Comparing `nigsp-0.8.0/nigsp/operations/metrics.py` & `nigsp-0.9.0/nigsp/operations/metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 Attributes
 ----------
 LGR
     Logger
 """
 
 import logging
-
 from itertools import combinations
 
 import numpy as np
 
+from nigsp import references
+from nigsp.due import due
 
 LGR = logging.getLogger(__name__)
 
 
+@due.dcite(references.PRETI_2019)
 def sdi(ts_split, mean=False, keys=None):
     """
     Compute the Structural Decoupling Index (SDI).
 
     i.e. the ratio between the norms of the "high" and the norm of the "low"
     "graph-filtered" timeseries.
 
@@ -33,15 +35,15 @@
 
     Parameters
     ----------
     ts_split : dict or numpy.ndarrays
         A dictionary containing two entries. If the two entries are "low" and
         "high", then SDI will be computed as the norm of the high vs the norm
         of the low, oterwise as the ratio between the second (second key in
-        sorted keys) and the first. 
+        sorted keys) and the first.
     mean : bool, optional
         If True, compute mean over the last axis (e.g. between subjects)
     keys : None or list of strings, optional
         Can be used to select two entries from a bigger dictionary
         and/or to specify the order in which the keys should be read (e.g.
         forcing a different order from teh sorted keys).
 
@@ -57,32 +59,36 @@
         If keys are not provided and the dictionary has more than 2 entries
     """
     # #!# Implement acceptance of two matrices and not only dictionary
     if keys is None:
         keys = list(ts_split.keys())
     else:
         if all(item in list(ts_split.keys()) for item in keys) is False:
-            raise ValueError(f'The provided keys {keys} do not match the '
-                             'keys of the provided dictionary '
-                             f'({list(ts_split.keys())})')
+            raise ValueError(
+                f"The provided keys {keys} do not match the "
+                "keys of the provided dictionary "
+                f"({list(ts_split.keys())})"
+            )
 
     if len(keys) != 2:
-        raise ValueError('`structural_decoupling_index` function requires '
-                         'a dictionary with exactly two timeseries as input.')
+        raise ValueError(
+            "`structural_decoupling_index` function requires "
+            "a dictionary with exactly two timeseries as input."
+        )
 
     check_keys = [item.lower() for item in keys]
-    if all(item in ['low', 'high'] for item in check_keys):
+    if all(item in ["low", "high"] for item in check_keys):
         # Case insensitively reorder the items of dictionary as ['low', 'high'].
-        keys = [keys[check_keys.index('low')], keys[check_keys.index('high')]]
+        keys = [keys[check_keys.index("low")], keys[check_keys.index("high")]]
 
     norm = dict.fromkeys(keys)
     for k in keys:
         norm[k] = np.linalg.norm(ts_split[k], axis=1)
 
-    LGR.info('Computing Structural Decoupling Index.')
+    LGR.info("Computing Structural Decoupling Index.")
     sdi = norm[keys[1]] / norm[keys[0]]
 
     if sdi.ndim >= 2 and mean:
         sdi = sdi.mean(axis=1)
 
     return np.log2(sdi)
 
@@ -116,43 +122,45 @@
     """
     # #!# Implement acceptance of N matrices and not only dictionary
     # #!# Check that this can overcome SDI
     if keys is None:
         keys = list(ts_split.keys())
     else:
         if all(item in list(ts_split.keys()) for item in keys) is False:
-            raise ValueError(f'The provided keys {keys} do not match the '
-                             'keys of the provided dictionary '
-                             f'({list(ts_split.keys())})')
+            raise ValueError(
+                f"The provided keys {keys} do not match the "
+                "keys of the provided dictionary "
+                f"({list(ts_split.keys())})"
+            )
 
     if len(keys) > 2:
-        LGR.info('Prepare combinations of timeseries')
+        LGR.info("Prepare combinations of timeseries")
         # Combining two or more "timeseries splits" means nothing more than
         # adding them in this case.
         for n in range(2, len(keys)):
             for c in combinations(keys, n):
                 comb_key = str(c).replace("'", "").replace(", ", "_and_")
 
-                ts_split[comb_key] = np.zeros_like(ts_split[keys[0]], dtype='float32')
+                ts_split[comb_key] = np.zeros_like(ts_split[keys[0]], dtype="float32")
                 for k in c:
                     ts_split[comb_key] = np.add(ts_split[comb_key], ts_split[k])
 
     # Obtain updated list of keys
     all_keys = list(ts_split.keys())
     norm = dict.fromkeys(all_keys)
-    LGR.info('Computing norm of timeseries')
+    LGR.info("Computing norm of timeseries")
     for k in all_keys:
         norm[k] = np.linalg.norm(ts_split[k], axis=1)
 
-    LGR.info('Computing generalised SDI')
+    LGR.info("Computing generalised SDI")
     gsdi = dict()
     for k in keys:
         for j in all_keys:
-            if not (k in j or f'({k}_' in j or f'_{k})' in j or f'_{k}_' in j):
-                gsdi[f'{k}_over_{j}'] = norm[k] / norm[j]
+            if not (k in j or f"({k}_" in j or f"_{k})" in j or f"_{k}_" in j):
+                gsdi[f"{k}_over_{j}"] = norm[k] / norm[j]
 
     if list(gsdi.values())[0].ndim >= 2 and mean:
         for k in gsdi.keys():
             gsdi[k] = gsdi[k].mean(axis=1)
 
     for k in gsdi.keys():
         gsdi[k] = np.log2(gsdi[k])
```

### Comparing `nigsp-0.8.0/nigsp/operations/__init__.py` & `nigsp-0.9.0/nigsp/operations/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 They are organised into modules by type of operation.
 
 Each function is callable through their respective module or directly
 as an `operations` function, and each module can be called directly as a
 `nigsp` module.
 
 For example, calling `nigsp.operations.metrics.sdi` is equivalent to calling
-`nigsp.operations.sdi` or `nigsp.metrisc.sdi`. 
+`nigsp.operations.sdi` or `nigsp.metrisc.sdi`.
 """
 
 
 # Import all operations.
-from .graph import zerocross, nodestrength
-from .laplacian import symmetric_normalisation, decomposition
-from .metrics import sdi, gsdi
-from .nifti import (vol_to_mat, mat_to_vol, apply_mask, unmask, apply_atlas,
-                    unfold_atlas)
-from .surrogates import (random_sign, sc_informed, sc_uninformed,
-                         test_significance)
-from .timeseries import (normalise_ts, graph_fourier_transform,
-                         median_cutoff_frequency_idx, graph_filter,
-                         functional_connectivity)
+from .graph import nodestrength, zerocross
+from .laplacian import decomposition, symmetric_normalisation
+from .metrics import gsdi, sdi
+from .nifti import apply_atlas, apply_mask, mat_to_vol, unfold_atlas, unmask, vol_to_mat
+from .surrogates import random_sign, sc_informed, sc_uninformed, test_significance
+from .timeseries import (
+    functional_connectivity,
+    graph_filter,
+    graph_fourier_transform,
+    median_cutoff_frequency_idx,
+    normalise_ts,
+)
```

### Comparing `nigsp-0.8.0/nigsp/operations/timeseries.py` & `nigsp-0.9.0/nigsp/operations/timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Logger
 """
 
 import logging
 
 import numpy as np
 
-from nigsp.utils import pairwise, change_var_type, prepare_ndim_iteration
+from nigsp.utils import change_var_type, pairwise, prepare_ndim_iteration
 
 LGR = logging.getLogger(__name__)
 
 
 def normalise_ts(timeseries):
     """
     Normalise given timeseries (i.e. mean=0, std=1).
@@ -34,20 +34,22 @@
     Returns
     -------
     numpy.ndarray
         The normalised timeseries (mean=0 std=1) if timeseries is not a 1D array.
         If timeseries is a 1D array, it is returned as is.
     """
     if timeseries.ndim < 2 or (timeseries.ndim == 2 and timeseries.shape[1] == 1):
-        LGR.warning('Given timeseries seems to be a single timepoint. '
-                    'Returning it as is.')
+        LGR.warning(
+            "Given timeseries seems to be a single timepoint. " "Returning it as is."
+        )
         return timeseries
 
-    z = ((timeseries - timeseries.mean(axis=1)[:, np.newaxis, ...]) /
-         timeseries.std(axis=1, ddof=1)[:, np.newaxis, ...])
+    z = (timeseries - timeseries.mean(axis=1)[:, np.newaxis, ...]) / timeseries.std(
+        axis=1, ddof=1
+    )[:, np.newaxis, ...]
     z[np.isnan(z)] = 0
 
     return z
 
 
 def graph_fourier_transform(timeseries, eigenvec, energy=False, mean=False):
     """
@@ -90,15 +92,15 @@
             proj = proj.reshape(timeseries.shape)
 
     if timeseries.ndim > 2 and mean and not energy:
         proj = proj.mean(axis=1)
 
     if energy:
         # Compute energy of the spectral density
-        energy = proj ** 2
+        energy = proj**2
         if proj.ndim > 2 and mean:
             energy = energy.mean(axis=1)
 
         return energy
 
     else:
         return proj
@@ -123,40 +125,44 @@
 
     Raises
     ------
     NotImplementedError
         If the provided array is 3D or more.
     """
     if energy.ndim > 2:
-        raise NotImplementedError('Provided energy spectral density data have '
-                                  f'{energy.ndim} dimensions, but arrays of more '
-                                  'than 2 dimensions are not supported yet')
+        raise NotImplementedError(
+            "Provided energy spectral density data have "
+            f"{energy.ndim} dimensions, but arrays of more "
+            "than 2 dimensions are not supported yet"
+        )
 
     if energy.ndim == 2:
         energy = energy.mean(axis=-1)
-    half_tot_auc = np.trapz(energy, axis=0)/2
-    LGR.debug(f'Total AUC = {half_tot_auc*2}, targetting half of total AUC')
+    half_tot_auc = np.trapz(energy, axis=0) / 2
+    LGR.debug(f"Total AUC = {half_tot_auc*2}, targetting half of total AUC")
 
     # Compute the AUC from first to one to last frequency,
     # skipping first component because AUC(1)=0.
     # Returns first idx for which AUC reaches half of total AUC.
     # It could be computed from high to low, but in theory
     # there would be more cycles, as #eigenvec(h) > #eigenvec(l).
     for freq_idx in range(1, energy.size):
-        LGR.debug(f'Frequency idx {freq_idx}, '
-                  f'AUC = {np.trapz(energy[:freq_idx])}, '
-                  f'target AUC = {half_tot_auc}')
+        LGR.debug(
+            f"Frequency idx {freq_idx}, "
+            f"AUC = {np.trapz(energy[:freq_idx])}, "
+            f"target AUC = {half_tot_auc}"
+        )
         if np.trapz(energy[:freq_idx]) >= half_tot_auc:
             break
 
-    LGR.info(f'Found {freq_idx} as splitting index')
+    LGR.info(f"Found {freq_idx} as splitting index")
     return freq_idx
 
 
-def graph_filter(timeseries, eigenvec, freq_idx, keys=['low', 'high']):
+def graph_filter(timeseries, eigenvec, freq_idx, keys=["low", "high"]):
     """
     Filter a graph decomposition into two parts based on freq_idx.
 
     Return the two eigenvector lists (high freq and low freq) that are equal
     to the original eigenvector list, but "low" is zero-ed for all frequencies
     >= of the given index, and "high" is zero-ed for all frequencies < to the
     given index.
@@ -190,54 +196,63 @@
     """
     # #!# Find better name
     # #!# Implement an index splitter
     freq_idx = change_var_type(freq_idx, list, stop=False, silent=True)
 
     for f in freq_idx:
         if f == 0 or f >= eigenvec.shape[0] - 1:
-            raise IndexError(f'Selected index {f} is not valid to split '
-                             f'eigenvector matrix of shape {eigenvec.shape}.')
+            raise IndexError(
+                f"Selected index {f} is not valid to split "
+                f"eigenvector matrix of shape {eigenvec.shape}."
+            )
 
-    LGR.info(f'Splitting graph into {len(freq_idx)+1} parts')
+    LGR.info(f"Splitting graph into {len(freq_idx)+1} parts")
 
     # Check that there is the right amount of keys
-    if len(keys) > len(freq_idx)+1:
-        LGR.warning(f'The declared keys list ({keys}) has {len(keys)} elements. '
-                    f'Since the frequency index list ({freq_idx}) has {len(freq_idx)}, '
-                    f'any keys after {keys[len(freq_idx)]} will be ignored.')
-        keys = keys[:len(freq_idx)+1]
-    elif len(keys) < len(freq_idx)+1:
-        LGR.warning(f'The declared keys list ({keys}) has {len(keys)} elements. '
-                    f'Since the frequency index list ({freq_idx}) has {len(freq_idx)}, '
-                    f'more keys will be created after {keys[len(freq_idx)]} .')
+    if len(keys) > len(freq_idx) + 1:
+        LGR.warning(
+            f"The declared keys list ({keys}) has {len(keys)} elements. "
+            f"Since the frequency index list ({freq_idx}) has {len(freq_idx)}, "
+            f"any keys after {keys[len(freq_idx)]} will be ignored."
+        )
+        keys = keys[: len(freq_idx) + 1]
+    elif len(keys) < len(freq_idx) + 1:
+        LGR.warning(
+            f"The declared keys list ({keys}) has {len(keys)} elements. "
+            f"Since the frequency index list ({freq_idx}) has {len(freq_idx)}, "
+            f"more keys will be created after {keys[len(freq_idx)]} ."
+        )
 
-        for i in range(len(keys), len(freq_idx)+1):
-            keys = keys + [f'key-{i+1:03d}']
+        for i in range(len(keys), len(freq_idx) + 1):
+            keys = keys + [f"key-{i+1:03d}"]
 
     # Add 0 and None to freq_idx to have full indexes
     freq_idx = [0] + freq_idx + [None]
 
     evec_split = dict.fromkeys(keys)
     ts_split = dict.fromkeys(keys)
 
     for n, idx in enumerate(pairwise(freq_idx)):
         i, j = idx
         k = j if j is not None else eigenvec.shape[-1]
-        evec_split[keys[n]] = np.append(np.append(np.zeros_like(eigenvec[:, :i],
-                                                                dtype='float32'),
-                                                  eigenvec[:, i:j], axis=-1),
-                                        np.zeros_like(eigenvec[:, k:],
-                                                      dtype='float32'),
-                                        axis=-1)
+        evec_split[keys[n]] = np.append(
+            np.append(
+                np.zeros_like(eigenvec[:, :i], dtype="float32"),
+                eigenvec[:, i:j],
+                axis=-1,
+            ),
+            np.zeros_like(eigenvec[:, k:], dtype="float32"),
+            axis=-1,
+        )
 
-    LGR.info('Compute graph fourier coefficients.')
+    LGR.info("Compute graph fourier coefficients.")
     fourier_coeff = graph_fourier_transform(timeseries, eigenvec)
 
     for k in keys:
-        LGR.info(f'Compute {k} part of timeseries.')
+        LGR.info(f"Compute {k} part of timeseries.")
         ts_split[k] = graph_fourier_transform(fourier_coeff, evec_split[k].T)
 
     return evec_split, ts_split
 
 
 def functional_connectivity(timeseries, mean=False):
     """
@@ -278,22 +293,24 @@
         Returns
         -------
         numpy.ndarray
             FC matrix
         """
         timeseries = timeseries.squeeze()
         if timeseries.ndim < 2:
-            LGR.warning('Computing functional connectivity of a 1D array (== 1)!')
+            LGR.warning("Computing functional connectivity of a 1D array (== 1)!")
             return 1
         elif timeseries.ndim == 2:
             return np.corrcoef(timeseries)
         else:
-            # reshape the array to allow reiteration on unknown dimensions of timeseries 
+            # reshape the array to allow reiteration on unknown dimensions of timeseries
             temp_ts, _ = prepare_ndim_iteration(timeseries, 2)
-            fcorr = np.empty(([temp_ts.shape[0]] * 2 + [temp_ts.shape[-1]]), dtype='float32')
+            fcorr = np.empty(
+                ([temp_ts.shape[0]] * 2 + [temp_ts.shape[-1]]), dtype="float32"
+            )
             for i in range(temp_ts.shape[-1]):
                 fcorr[:, :, i] = np.corrcoef(temp_ts[..., i])
 
             if timeseries.ndim > 3:
                 new_shape = (timeseries.shape[0],) * 2 + timeseries.shape[2:]
                 fcorr = fcorr.reshape(new_shape)
```

### Comparing `nigsp-0.8.0/nigsp/operations/surrogates.py` & `nigsp-0.9.0/nigsp/operations/surrogates.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 Attributes
 ----------
 LGR
     Logger
 """
 
 import logging
-
 from copy import deepcopy
-from math import factorial, floor, ceil
+from math import ceil, factorial, floor
 
 import numpy as np
 
-from nigsp.operations.timeseries import graph_fourier_transform
 from nigsp.operations.laplacian import decomposition
+from nigsp.operations.timeseries import graph_fourier_transform
 
 LGR = logging.getLogger(__name__)
-SURR_TYPE = ['informed', 'uninformed']
-STAT_METHOD = ['Bernoulli', 'frequentist']
+SURR_TYPE = ["informed", "uninformed"]
+STAT_METHOD = ["Bernoulli", "frequentist"]
 
 
 def random_sign(eigenvec, n_surr=1000, seed=42, stack=False):
     """
     Create surrogates by randomly switching signs of eigenvectors.
 
     Parameters
@@ -50,21 +49,22 @@
         If eigenvec is 4+ D.
     """
     # Reinitialise the random seed for repeatability
     rng = np.random.default_rng(seed)
 
     if eigenvec.ndim > 3:
         raise NotImplementedError(
-            f'Provided data has {eigenvec.ndim} dimensions, '
-            'but data of more than 3 dimensions are not '
-            'supported yet')
+            f"Provided data has {eigenvec.ndim} dimensions, "
+            "but data of more than 3 dimensions are not "
+            "supported yet"
+        )
 
-    rand_evec = np.empty((eigenvec.shape + (n_surr,)), dtype='float32')
+    rand_evec = np.empty((eigenvec.shape + (n_surr,)), dtype="float32")
 
-    LGR.info('Randomly switching signs of eigenvectors to create surrogates.')
+    LGR.info("Randomly switching signs of eigenvectors to create surrogates.")
     for i in range(n_surr):
         # #!# Check if two conditions can be merged.
         if eigenvec.ndim < 3:
             r_sign = rng.integers(0, 1, eigenvec.shape[0], endpoint=True)
             r_sign[r_sign == 0] = -1
             rand_evec[..., i] = eigenvec * r_sign
         else:
@@ -109,37 +109,39 @@
         If timeseries is 4+ D and/or eigenvector matrix has not enough dimensions.
     """
     rand_evec = random_sign(eigenvec, n_surr, seed, stack)
 
     if stack:
         n_surr += 1
 
-    surr = np.empty((timeseries.shape + (n_surr,)), dtype='float32')
+    surr = np.empty((timeseries.shape + (n_surr,)), dtype="float32")
 
     fourier_coeff = graph_fourier_transform(timeseries, eigenvec)
 
-    LGR.info('Projecting the timeseries onto the surrogate eigenvectors.')
+    LGR.info("Projecting the timeseries onto the surrogate eigenvectors.")
     for i in range(n_surr):
         if timeseries.ndim < 3 and rand_evec.ndim == timeseries.ndim + 1:
-            surr[..., i] = graph_fourier_transform(fourier_coeff,
-                                                   rand_evec[..., i].T)
+            surr[..., i] = graph_fourier_transform(fourier_coeff, rand_evec[..., i].T)
         elif timeseries.ndim == 3:
             if rand_evec.ndim < 4:
-                surr[..., i] = graph_fourier_transform(fourier_coeff,
-                                                       rand_evec[..., i].T)
+                surr[..., i] = graph_fourier_transform(
+                    fourier_coeff, rand_evec[..., i].T
+                )
             else:
                 for j in range(rand_evec.shape[2]):
-                    surr[:, :, j,
-                         i] = graph_fourier_transform(fourier_coeff,
-                                                      rand_evec[:, :, j, i].T)
+                    surr[:, :, j, i] = graph_fourier_transform(
+                        fourier_coeff, rand_evec[:, :, j, i].T
+                    )
         else:
-            raise NotImplementedError('No solution implemented for timeseries '
-                                      f'of {timeseries.ndim} dimension(s) and '
-                                      f'eigenvector matrix of {eigenvec.ndim} '
-                                      'dimension(s)')
+            raise NotImplementedError(
+                "No solution implemented for timeseries "
+                f"of {timeseries.ndim} dimension(s) and "
+                f"eigenvector matrix of {eigenvec.ndim} "
+                "dimension(s)"
+            )
     return surr
 
 
 def sc_informed(timeseries, eigenvec, n_surr=1000, seed=124, stack=False):
     """
     Create surrogates informed by the real structural connectivity.
 
@@ -163,17 +165,19 @@
 
     Raises
     ------
     NotImplementedError
         If timeseries is 4+ D.
     """
     if timeseries.ndim > 3:
-        raise NotImplementedError(f'Provided timeseries has {timeseries.ndim} '
-                                  'dimensions, but timeseries of more than 3 '
-                                  'dimensions are not supported yet.')
+        raise NotImplementedError(
+            f"Provided timeseries has {timeseries.ndim} "
+            "dimensions, but timeseries of more than 3 "
+            "dimensions are not supported yet."
+        )
 
     return _create_surr(timeseries, eigenvec, n_surr, seed, stack)
 
 
 def sc_uninformed(timeseries, lapl_mtx, n_surr=1000, seed=98, stack=False):
     """
     Create surrogates ignorant of the real structural connectivity.
@@ -198,37 +202,41 @@
 
     Raises
     ------
     NotImplementedError
         If timeseries is 4+ D.
     """
     if timeseries.ndim > 3:
-        raise NotImplementedError(f'Provided timeseries has {timeseries.ndim} '
-                                  'dimensions, but timeseries of more than 3 '
-                                  'dimensions are not supported yet.')
+        raise NotImplementedError(
+            f"Provided timeseries has {timeseries.ndim} "
+            "dimensions, but timeseries of more than 3 "
+            "dimensions are not supported yet."
+        )
 
     symm_norm = np.eye(lapl_mtx.shape[0]) - lapl_mtx
     symm_norm_sum = symm_norm.sum(axis=-1)
 
     conf_model = np.outer(symm_norm_sum, symm_norm_sum.T) / symm_norm.sum()
 
     conf_lapl = np.diag(symm_norm_sum) - conf_model
 
     _, surr_eigenvec = decomposition(conf_lapl)
 
     return _create_surr(timeseries, surr_eigenvec, n_surr, seed, stack)
 
 
-def test_significance(surr,
-                      data=None,
-                      method='Bernoulli',
-                      p=0.05,
-                      p_bernoulli=None,
-                      return_masked=False,
-                      mean=False):
+def test_significance(
+    surr,
+    data=None,
+    method="Bernoulli",
+    p=0.05,
+    p_bernoulli=None,
+    return_masked=False,
+    mean=False,
+):
     """
     Test the significance of the empirical data against surrogates.
 
     Two methods are implemented, 'Bernoulli' and 'frequentist'.
     - 'frequentist' is a group or single subject test. It tests that the
       empirical data are in the highest (or lowest) percentile (where the
       percentile is defined by p/2).
@@ -285,106 +293,121 @@
     NotImplementedError
         If any other method rather than those listed above is selected.
 
     """
     # #!# Check that the surrogate shape has parcels in the first axis!
     # If provided, append data to surr
     if data is not None:
-        if surr.shape[:data.ndim] != data.shape:
+        if surr.shape[: data.ndim] != data.shape:
             raise ValueError(
-                'Provided empirical data and surrogate data shapes '
-                f'do not agree, with shapes {data.shape} and '
-                f'{surr.shape[:data.ndim]} (last axis excluded)')
+                "Provided empirical data and surrogate data shapes "
+                f"do not agree, with shapes {data.shape} and "
+                f"{surr.shape[:data.ndim]} (last axis excluded)"
+            )
         if not (surr[..., -1] == data).all():
             # Check that data was not appended yet.
             surr = np.append(surr, data[..., np.newaxis], axis=-1)
 
     if p < 0 or p > 1:
-        raise ValueError('p values should always be between 0 and 1. The '
-                         f'provided value of {p} is out of these boundaries')
+        raise ValueError(
+            "p values should always be between 0 and 1. The "
+            f"provided value of {p} is out of these boundaries"
+        )
     elif p == 0 or p == 1:
-        LGR.warning(f'The selected p value of {p} is at the limits of the '
-                    'possible range of [0, 1]. Statistical thresholding might '
-                    'not be interpretable.')
+        LGR.warning(
+            f"The selected p value of {p} is at the limits of the "
+            "possible range of [0, 1]. Statistical thresholding might "
+            "not be interpretable."
+        )
 
     if surr.ndim < 3:
         LGR.warning(
-            f'Warning: surrogate dimensions ({surr.ndim}) are less than '
-            'the program expects - check that you mean to run a test on '
-            'an average or that you have enough surrogates.')
+            f"Warning: surrogate dimensions ({surr.ndim}) are less than "
+            "the program expects - check that you mean to run a test on "
+            "an average or that you have enough surrogates."
+        )
 
     # Reorder the surrogate matrix, then find where the real surrogate is
-    LGR.info('Reordering surrogates for test')
+    LGR.info("Reordering surrogates for test")
     real_idx = surr.shape[-1] - 1
-    reord_surr = (np.argsort(surr, axis=-1) == real_idx)
+    reord_surr = np.argsort(surr, axis=-1) == real_idx
 
-    LGR.info(f'Adopting {method} testing method.')
+    LGR.info(f"Adopting {method} testing method.")
     # Testing both tails requires to split p
-    if method == 'frequentist':
-        LGR.info(f'Testing for p={p} two-tails (p={p/2} each tail)')
+    if method == "frequentist":
+        LGR.info(f"Testing for p={p} two-tails (p={p/2} each tail)")
         p = p / 2
         # If there aren't enough surrogates, send a warning message on the real p
         # Then update p
         if 1 / surr.shape[-1] > p:
             LGR.warning(
-                'The generated surrogates are not enough to test for '
-                f'the selected p ({p*2} two-tails), since at least '
-                f'{ceil(1/p)-1} surrogates are required for the selected '
-                f'p value. Testing for p={1/surr.shape[-1]} two-tails instead.'
+                "The generated surrogates are not enough to test for "
+                f"the selected p ({p*2} two-tails), since at least "
+                f"{ceil(1/p)-1} surrogates are required for the selected "
+                f"p value. Testing for p={1/surr.shape[-1]} two-tails instead."
             )
             p = 1 / surr.shape[-1]
 
-    elif method == 'Bernoulli':
+    elif method == "Bernoulli":
         # If there aren't enough subjects, send a warning message on the real p
         # Then update group level p
         if p_bernoulli is None:
             p_bernoulli = deepcopy(p)
             p = 0.1
         if 1 / surr.shape[1] > p_bernoulli:
             LGR.warning(
-                'The provided subjects are not enough to test for '
-                f'p={p_bernoulli} one-tail at the group level, since '
-                f'at least {ceil(1/p_bernoulli)} subjects are required.')
+                "The provided subjects are not enough to test for "
+                f"p={p_bernoulli} one-tail at the group level, since "
+                f"at least {ceil(1/p_bernoulli)} subjects are required."
+            )
             p_bernoulli = 1 / surr.shape[1]
         # If there aren't enough surrogates, send a warning message on the real p
         # Then update subject level p
         if 1 / surr.shape[-1] > p:
-            LGR.warning('The generated surrogates are not enough to test for '
-                        f'p={p} two-tails at the subject level. '
-                        f'{ceil(1/p)-1} surrogates are required for p={p}.')
+            LGR.warning(
+                "The generated surrogates are not enough to test for "
+                f"p={p} two-tails at the subject level. "
+                f"{ceil(1/p)-1} surrogates are required for p={p}."
+            )
             p = 1 / surr.shape[-1]
 
         LGR.info(
-            f'Testing for p={p_bernoulli} one-tail at the group level and '
-            f'at p={p*2} two-tails (p={p} each tail) at the subject level.')
+            f"Testing for p={p_bernoulli} one-tail at the group level and "
+            f"at p={p*2} two-tails (p={p} each tail) at the subject level."
+        )
     else:
         raise NotImplementedError(
-            'Other testing methods than Bernoulli or '
-            'frequentist are not implemented at the moment.')
+            "Other testing methods than Bernoulli or "
+            "frequentist are not implemented at the moment."
+        )
 
     # First, and no matter what, apply frequentist approach to find where
     # the real data index (real_idx) is at the extremes of the matrix last axis
     # (with tolerance on the extremes depending on p).
     # real_idx serendipitously is the number of surrogates.
-    stat_mask = (reord_surr[..., :floor(real_idx * p) + 1].any(axis=-1) +
-                 reord_surr[..., -floor(real_idx * p) - 1:].any(axis=-1))
+    stat_mask = reord_surr[..., : floor(real_idx * p) + 1].any(axis=-1) + reord_surr[
+        ..., -floor(real_idx * p) - 1 :
+    ].any(axis=-1)
 
-    if method == 'Bernoulli' and surr.shape[1] > 1 and surr.ndim >= 3:
+    if method == "Bernoulli" and surr.shape[1] > 1 and surr.ndim >= 3:
         # The following computes the CDF of a binomial distribution
         # Difference with scipy's binom.cdf (100 samples) is: 5.066394802133445e-06
         # #!# See if there is a quicker way to get this (probably invert testing)
 
         def _pmf(x, n, p):
-            f = ((factorial(n) / (factorial(x) * factorial(n - x))) * p**x *
-                 (1 - p)**(n - x))
+            f = (
+                (factorial(n) / (factorial(x) * factorial(n - x)))
+                * p**x
+                * (1 - p) ** (n - x)
+            )
             return f
 
         x = np.arange(0, 100, 1)
         # Generate the PMF of the binomial distribution
-        y = np.asarray([_pmf(i, 100, p) for i in x], dtype='float32')
+        y = np.asarray([_pmf(i, 100, p) for i in x], dtype="float32")
         # Generate the CDF, then invert it.
         y = 1 - np.cumsum(y)
         # Find the number of subjects necessary to be statistically significant,
         # adjusted for the number of subjects in the surrogates.
         # Then find all parcels for which the real data is higher or lower
         # than all surrogates in enough subjects.
         # The +1 in thr is to be conservative on the number of subjects.
@@ -393,29 +416,34 @@
         thr = np.floor(surr.shape[1] / 100 * thr) + 1
         # On top of the frequentist approach, find the parcels that pop up
         # in the frequentist approach for enough subjects.
         stat_mask = stat_mask.sum(axis=1) > thr
         # repeat stat_mask for the number of subjects.
         stat_mask = stat_mask[..., np.newaxis].repeat(surr.shape[1], axis=-1)
     elif surr.shape[1] == 1 and surr.ndim >= 3:
-        LGR.warning('The "Bernoulli" method is a group test that requires '
-                    'multiple subjects to be run.')
+        LGR.warning(
+            'The "Bernoulli" method is a group test that requires '
+            "multiple subjects to be run."
+        )
     elif surr.ndim < 3:
-        LGR.warning('The dimensionality of the data is not enough to run '
-                    'the "Bernoulli" method.')
+        LGR.warning(
+            "The dimensionality of the data is not enough to run "
+            'the "Bernoulli" method.'
+        )
 
     if return_masked:
-        LGR.info('Returning masked empirical data')
-        stat_mask = np.ma.array(data=surr[..., -1], mask=np.invert(stat_mask),
-                                fill_value=np.NINF).squeeze()
+        LGR.info("Returning masked empirical data")
+        stat_mask = np.ma.array(
+            data=surr[..., -1], mask=np.invert(stat_mask), fill_value=np.NINF
+        ).squeeze()
     else:
-        LGR.info('Returning mask')
+        LGR.info("Returning mask")
 
     if mean and stat_mask.ndim >= 2:
-        LGR.info('Returning average across subjects (axis 1)')
+        LGR.info("Returning average across subjects (axis 1)")
         stat_mask = stat_mask.mean(axis=1)
 
     if return_masked:
         stat_mask = stat_mask.filled()
 
     return stat_mask
```

### Comparing `nigsp-0.8.0/nigsp/objects.py` & `nigsp-0.9.0/nigsp/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,43 +11,65 @@
 Attributes
 ----------
 LGR
     Logger
 """
 
 import logging
-
 from copy import deepcopy
 
 from nigsp import operations
 
-
 LGR = logging.getLogger(__name__)
 
 
-class SCGraph():
+class SCGraph:
+    """Main module object, containing all data representing the graph."""
 
-    def __init__(self, mtx, timeseries, atlas=None, filename=None, img=None,
-                 eigenval=None, eigenvec=None, energy=None, lapl_mtx=None,
-                 index='median', evec_split=None, ts_split=None, surr=None,
-                 surr_split=None, sdi=None, gsdi=None, fc=None, fc_split=None):
+    def __init__(
+        self,
+        mtx,
+        timeseries,
+        atlas=None,
+        filename=None,
+        img=None,
+        eigenval=None,
+        eigenvec=None,
+        energy=None,
+        lapl_mtx=None,
+        index="median",
+        evec_split=None,
+        ts_split=None,
+        surr=None,
+        surr_split=None,
+        sdi=None,
+        gsdi=None,
+        fc=None,
+        fc_split=None,
+    ):
         """Initialise SCGraph (see class docstring)."""
         if mtx.shape[1] != mtx.shape[0]:
-            raise ValueError('Graph matrix must be a square matrix, but '
-                             f'given matrix has {mtx.shape}!')
+            raise ValueError(
+                "Graph matrix must be a square matrix, but "
+                f"given matrix has {mtx.shape}!"
+            )
 
         if mtx.shape[1] != timeseries.shape[0]:
-            raise ValueError(f'Timeseries extracted from {timeseries.shape[0]} '
-                             f'parcels, but graph has {mtx.shape[1]} nodes. '
-                             'The number of parcels and nodes must be the same.')
+            raise ValueError(
+                f"Timeseries extracted from {timeseries.shape[0]} "
+                f"parcels, but graph has {mtx.shape[1]} nodes. "
+                "The number of parcels and nodes must be the same."
+            )
 
         if timeseries.ndim > 3:
-            raise ValueError('Timeseries of more than 3 dimensions are not supported '
-                             f'yet, but given timeseries has {timeseries.ndim} '
-                             'dimensions.')
+            raise ValueError(
+                "Timeseries of more than 3 dimensions are not supported "
+                f"yet, but given timeseries has {timeseries.ndim} "
+                "dimensions."
+            )
         self.mtx = deepcopy(mtx)
         self.timeseries = deepcopy(timeseries)
         self.atlas = deepcopy(atlas)
         self.filename = deepcopy(filename)
         self.img = deepcopy(img)
         self.eigenval = deepcopy(eigenval)
         self.eigenvec = deepcopy(eigenvec)
@@ -99,35 +121,38 @@
 
     def structural_decomposition(self):  # pragma: no cover
         """Implement both laplacian operations."""
         return self.symmetric_normalisation().decomposition()
 
     def compute_graph_energy(self, mean=False):  # pragma: no cover
         """Implement timeseries.graph_fourier_transform for energy as class method."""
-        self.energy = operations.graph_fourier_transform(self.timeseries, self.eigenvec,
-                                                         energy=True, mean=mean)
+        self.energy = operations.graph_fourier_transform(
+            self.timeseries, self.eigenvec, energy=True, mean=mean
+        )
         return self
 
-    def split_graph(self, index=None, keys=['low', 'high']):
+    def split_graph(self, index=None, keys=["low", "high"]):
         """Implement timeseries.median_cutoff_frequency_idx as class method."""
         if index is None:
             index = self.index
 
-        if index == 'median':  # pragma: no cover
+        if index == "median":  # pragma: no cover
             index = operations.median_cutoff_frequency_idx(self.energy)
 
         elif type(index) is not int:
-            raise ValueError(f'Unknown option {index} for frequency split index. '
-                             'Declared index must be either an integer or \'median\'')
-
-        self.evec_split, self.ts_split = operations.graph_filter(self.timeseries,
-                                                                 self.eigenvec,
-                                                                 index, keys)
+            raise ValueError(
+                f"Unknown option {index} for frequency split index. "
+                "Declared index must be either an integer or 'median'"
+            )
+
+        self.evec_split, self.ts_split = operations.graph_filter(
+            self.timeseries, self.eigenvec, index, keys
+        )
         if self.index != index:
-            LGR.warning(f'Updating stored index from {self.index} to {index}')
+            LGR.warning(f"Updating stored index from {self.index} to {index}")
             self.index = index
 
         return self
 
     def nodestrength(self, mean=False):  # pragma: no cover
         """Implement graph.nodestrength as class method."""
         self.ns = operations.nodestrength(self.mtx, mean)
@@ -139,67 +164,81 @@
         return self
 
     def compute_gsdi(self, mean=False, keys=None):  # pragma: no cover
         """Implement sdi.gsdi as class method."""
         self.gsdi = operations.gsdi(self.ts_split, mean, keys)
         return self
 
-    def create_surrogates(self, sc_type='informed', n_surr=1000, seed=None):
+    def create_surrogates(self, sc_type="informed", n_surr=1000, seed=None):
         """Implement surrogates.sc_informed and sc_uninformed as class method."""
-        sc_args = {'timeseries': self.timeseries, 'n_surr': n_surr}
+        sc_args = {"timeseries": self.timeseries, "n_surr": n_surr}
         if seed is not None:
-            sc_args['seed'] = seed
+            sc_args["seed"] = seed
 
-        if sc_type == 'informed':
-            sc_args['eigenvec'] = self.eigenvec
+        if sc_type == "informed":
+            sc_args["eigenvec"] = self.eigenvec
             self.surr = operations.sc_informed(**sc_args)
-        elif sc_type == 'uninformed':
-            sc_args['lapl_mtx'] = self.lapl_mtx
+        elif sc_type == "uninformed":
+            sc_args["lapl_mtx"] = self.lapl_mtx
             self.surr = operations.sc_uninformed(**sc_args)
         else:
-            raise ValueError(f'Unknown option {sc_type} for surrogate creation. '
-                             'Declared type must be either \'informed\' or '
-                             '\'uninformed\'')
+            raise ValueError(
+                f"Unknown option {sc_type} for surrogate creation. "
+                "Declared type must be either 'informed' or "
+                "'uninformed'"
+            )
         return self
 
-    def test_significance(self, method='Bernoulli', p=0.05,
-                          return_masked=False, mean=False):  # pragma: no cover
+    def test_significance(
+        self, method="Bernoulli", p=0.05, return_masked=False, mean=False
+    ):  # pragma: no cover
         """Implement surrogates.test_significance as class method."""
-        _, self.surr_split = operations.graph_filter(self.surr,
-                                                     self.eigenvec,
-                                                     self.index)
+        _, self.surr_split = operations.graph_filter(
+            self.surr, self.eigenvec, self.index
+        )
         if self.sdi is not None:
             surr_sdi = operations.sdi(self.surr_split, mean, keys=None)
-            self.sdi = operations.test_significance(surr=surr_sdi, data=self.sdi,
-                                                    method=method, p=p, return_masked=return_masked,
-                                                    mean=mean)
+            self.sdi = operations.test_significance(
+                surr=surr_sdi,
+                data=self.sdi,
+                method=method,
+                p=p,
+                return_masked=return_masked,
+                mean=mean,
+            )
         if self.gsdi is not None:
             surr_sdi = operations.gsdi(self.surr_split, mean, keys=None)
-            self.gsdi = operations.test_significance(surr=surr_sdi, data=self.gsdi,
-                                                     method=method, p=p, return_masked=return_masked,
-                                                     mean=mean)
+            self.gsdi = operations.test_significance(
+                surr=surr_sdi,
+                data=self.gsdi,
+                method=method,
+                p=p,
+                return_masked=return_masked,
+                mean=mean,
+            )
         return self
 
     def normalise_ts(self):  # pragma: no cover
         """Implement timeseries.normalise_ts for energy as class method."""
         self.timeseries = operations.normalise_ts(self.timeseries)
         return self
 
     def compute_fc(self, mean=False):
         """Implement timeseries.functional_connectivity as class method."""
         if self.timeseries is not None:
-            LGR.info('Compute FC of original timeseries.')
+            LGR.info("Compute FC of original timeseries.")
             self.fc = operations.functional_connectivity(self.timeseries, mean)
         if self.ts_split is not None:
             self.fc_split = dict.fromkeys(self.ts_split.keys())
-            LGR.info('Compute FC of split timeseries.')
+            LGR.info("Compute FC of split timeseries.")
             for k in self.ts_split.keys():
-                LGR.info(f'Compute FC of {k} timeseries.')
-                self.fc_split[k] = operations.functional_connectivity(self.ts_split[k],
-                                                                      mean)
+                LGR.info(f"Compute FC of {k} timeseries.")
+                self.fc_split[k] = operations.functional_connectivity(
+                    self.ts_split[k], mean
+                )
         return self
 
 
 """
 Copyright 2022, Stefano Moia.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `nigsp-0.8.0/nigsp/workflow.py` & `nigsp-0.9.0/nigsp/workflow.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 import datetime
 import logging
 import os
 import sys
 
 import numpy as np
 
-from nigsp import blocks, io, utils, viz, _version
+from nigsp import _version, blocks, io, references
 from nigsp import surrogates as surr
 from nigsp import timeseries as ts
+from nigsp import utils, viz
 from nigsp.cli.run import _get_parser
-# from nigsp.due import due, Doi
+from nigsp.due import due
 from nigsp.objects import SCGraph
 
-
 LGR = logging.getLogger(__name__)
 LGR.setLevel(logging.INFO)
 
 
 def save_bash_call(fname, outdir, outname):
     """
     Save the bash call into file `p2d_call.sh`.
@@ -45,36 +45,48 @@
             if len(fname) == 1:
                 outdir = os.path.dirname(fname[0])
             else:
                 outdir = os.path.commonpath(fname)
         else:
             outdir = os.path.split(outname)[0]
 
-        if outdir == '' or outdir == '/':
-            outdir = '.'
-        outdir = os.path.join(outdir, 'nigsp')
+        if outdir == "" or outdir == "/":
+            outdir = "."
+        outdir = os.path.join(outdir, "nigsp")
 
     outdir = os.path.abspath(outdir)
-    log_path = os.path.join(outdir, 'logs')
+    log_path = os.path.join(outdir, "logs")
     os.makedirs(log_path, exist_ok=True)
-    arg_str = ' '.join(sys.argv[1:])
-    call_str = f'nigsp {arg_str}'
+    arg_str = " ".join(sys.argv[1:])
+    call_str = f"nigsp {arg_str}"
     outdir = os.path.abspath(outdir)
-    log_path = os.path.join(outdir, 'logs')
+    log_path = os.path.join(outdir, "logs")
     os.makedirs(log_path, exist_ok=True)
-    isotime = datetime.datetime.now().strftime('%Y-%m-%dT%H%M%S')
-    f = open(os.path.join(log_path,
-                          f'nigsp_call_{isotime}.sh'), 'a')
-    f.write(f'#!bin/bash \n{call_str}')
+    isotime = datetime.datetime.now().strftime("%Y-%m-%dT%H%M%S")
+    f = open(os.path.join(log_path, f"nigsp_call_{isotime}.sh"), "a")
+    f.write(f"#!bin/bash \n{call_str}")
     f.close()
 
 
-def nigsp(fname, scname, atlasname=None, outname=None, outdir=None,
-          index='median', surr_type=None, n_surr=1000, method='Bernoulli',
-          p=0.05, seed=None, lgr_degree='info'):
+@due.dcite(references.PRETI_2019)
+@due.dcite(references.NIGSP)
+def nigsp(
+    fname,
+    scname,
+    atlasname=None,
+    outname=None,
+    outdir=None,
+    index="median",
+    surr_type=None,
+    n_surr=1000,
+    method="Bernoulli",
+    p=0.05,
+    seed=None,
+    lgr_degree="info",
+):
     """
     Main workflow for nigsp, following the methods described in [1].
 
     Parameters
     ----------
     fname : str or os.PathLike
         Path to the timeseries data file. It can be a text, nifti, or matlab file
@@ -163,61 +175,71 @@
             if len(fname) == 1:
                 outdir = os.path.dirname(fname[0])
             else:
                 outdir = os.path.commonpath(fname)
         else:
             outdir = os.path.split(outname)[0]
 
-        if outdir == '' or outdir == '/':
-            outdir = '.'
-        outdir = os.path.join(outdir, 'nigsp')
+        if outdir == "" or outdir == "/":
+            outdir = "."
+        outdir = os.path.join(outdir, "nigsp")
 
     outdir = os.path.abspath(outdir)
-    log_path = os.path.join(outdir, 'logs')
+    log_path = os.path.join(outdir, "logs")
     os.makedirs(log_path, exist_ok=True)
 
     # Create logfile name
-    basename = 'nigsp_'
-    extension = 'tsv'
-    isotime = datetime.datetime.now().strftime('%Y-%m-%dT%H%M%S')
-    logname = os.path.join(log_path, f'{basename}{isotime}.{extension}')
+    basename = "nigsp_"
+    extension = "tsv"
+    isotime = datetime.datetime.now().strftime("%Y-%m-%dT%H%M%S")
+    logname = os.path.join(log_path, f"{basename}{isotime}.{extension}")
 
     # Set logging format
     log_formatter = logging.Formatter(
-        '%(asctime)s\t%(name)-12s\t%(levelname)-8s\t%(message)s',
-        datefmt='%Y-%m-%dT%H:%M:%S')
+        "%(asctime)s\t%(name)-12s\t%(levelname)-8s\t%(message)s",
+        datefmt="%Y-%m-%dT%H:%M:%S",
+    )
 
     # Set up logging file and open it for writing
     log_handler = logging.FileHandler(logname)
     log_handler.setFormatter(log_formatter)
     sh = logging.StreamHandler()
 
-    if lgr_degree == 'quiet':
-        logging.basicConfig(level=logging.WARNING,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
-    elif lgr_degree == 'debug':
-        logging.basicConfig(level=logging.DEBUG,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
+    if lgr_degree == "quiet":
+        logging.basicConfig(
+            level=logging.WARNING,
+            handlers=[log_handler, sh],
+            format="%(levelname)-10s %(message)s",
+        )
+    elif lgr_degree == "debug":
+        logging.basicConfig(
+            level=logging.DEBUG,
+            handlers=[log_handler, sh],
+            format="%(levelname)-10s %(message)s",
+        )
     else:
-        logging.basicConfig(level=logging.INFO,
-                            handlers=[log_handler, sh], format='%(levelname)-10s %(message)s')
+        logging.basicConfig(
+            level=logging.INFO,
+            handlers=[log_handler, sh],
+            format="%(levelname)-10s %(message)s",
+        )
 
-    version_number = _version.get_versions()['version']
-    LGR.info(f'Currently running nigsp version {version_number}')
+    version_number = _version.get_versions()["version"]
+    LGR.info(f"Currently running nigsp version {version_number}")
 
     # #### Check input #### #
 
     # Check data files
-    LGR.info(f'Input structural connectivity file: {scname}')
+    LGR.info(f"Input structural connectivity file: {scname}")
     sc_is = dict.fromkeys(io.EXT_DICT.keys(), False)
-    LGR.info(f'Input functional file(s): {fname}')
-    func_is = dict.fromkeys(io.EXT_DICT.keys(), '')
+    LGR.info(f"Input functional file(s): {fname}")
+    func_is = dict.fromkeys(io.EXT_DICT.keys(), "")
     atlas_is = dict.fromkeys(io.EXT_DICT.keys(), False)
     if atlasname:
-        LGR.info(f'Input atlas file: {atlasname}')
+        LGR.info(f"Input atlas file: {atlasname}")
 
     # Check inputs type
     for k in io.EXT_DICT.keys():
         func_is[k] = []
         for f in fname:
             func_is[k] += [io.check_ext(io.EXT_DICT[k], f)[0]]
         # Check that func files are all of the same kind
@@ -225,214 +247,225 @@
 
         sc_is[k], _ = io.check_ext(io.EXT_DICT[k], scname)
 
         if atlasname is not None:
             atlas_is[k], _ = io.check_ext(io.EXT_DICT[k], atlasname)
 
     # Check that other inputs are supported
-    if index != 'median' and type(index) is not int:
-        raise ValueError(f'Index {index} of type {type(index)} is not valid.')
+    if index != "median" and type(index) is not int:
+        raise ValueError(f"Index {index} of type {type(index)} is not valid.")
     if method not in surr.STAT_METHOD and method is not None:
-        raise NotImplementedError(f'Method {method} is not supported. Supported '
-                                  f'methods are: {surr.STAT_METHOD}')
+        raise NotImplementedError(
+            f"Method {method} is not supported. Supported "
+            f"methods are: {surr.STAT_METHOD}"
+        )
     if surr_type not in surr.SURR_TYPE and surr_type is not None:
-        raise NotImplementedError(f'Surrogate type {surr_type} is not supported. '
-                                  f'Supported types are: {surr.SURR_TYPE}')
+        raise NotImplementedError(
+            f"Surrogate type {surr_type} is not supported. "
+            f"Supported types are: {surr.SURR_TYPE}"
+        )
     if p < 0 or p > 1:
-        raise ValueError(f'P value must be higher than 0 and lower than 1, but '
-                         f'p value {p} was provided instead.')
+        raise ValueError(
+            f"P value must be higher than 0 and lower than 1, but "
+            f"p value {p} was provided instead."
+        )
 
     # #### Read in data #### #
 
     # Read in structural connectivity matrix
-    if sc_is['1D']:
-        mtx = io.load_txt(scname, shape='square')
-    elif sc_is['mat']:
-        mtx = io.load_mat(scname, shape='square')
-    elif sc_is['xls']:
-        mtx = io.load_xls(scname, shape='square')
+    if sc_is["1D"]:
+        mtx = io.load_txt(scname, shape="square")
+    elif sc_is["mat"]:
+        mtx = io.load_mat(scname, shape="square")
+    elif sc_is["xls"]:
+        mtx = io.load_xls(scname, shape="square")
     else:
-        raise NotImplementedError(f'Input file {scname} is not of a supported type.')
+        raise NotImplementedError(f"Input file {scname} is not of a supported type.")
 
     # Read in atlas, if defined
     if atlasname is not None:
-        if (atlas_is['1D'] or atlas_is['mat']
-                or atlas_is['xls'] or atlas_is['nifti']) is False:
-            raise NotImplementedError(f'Input file {atlasname} is not of a '
-                                      'supported type.')
-        elif atlas_is['1D']:
+        if (
+            atlas_is["1D"] or atlas_is["mat"] or atlas_is["xls"] or atlas_is["nifti"]
+        ) is False:
+            raise NotImplementedError(
+                f"Input file {atlasname} is not of a " "supported type."
+            )
+        elif atlas_is["1D"]:
             atlas = io.load_txt(atlasname)
-        elif atlas_is['nifti']:
+        elif atlas_is["nifti"]:
             atlas, _, img = io.load_nifti_get_mask(atlasname, ndim=3)
-        elif atlas_is['mat']:
+        elif atlas_is["mat"]:
             atlas = io.load_mat(atlasname)
-        elif atlas_is['xls']:
+        elif atlas_is["xls"]:
             atlas = io.load_xls(atlasname)
     else:
-        LGR.warning('Atlas not provided. Some functionalities might not work.')
+        LGR.warning("Atlas not provided. Some functionalities might not work.")
         atlas, img = None, None
 
     # Read in functional timeseries, join them, and normalise them
     timeseries = []
     for f in fname:
-        if func_is['nifti'] and atlas_is['nifti']:
+        if func_is["nifti"] and atlas_is["nifti"]:
             t, atlas, img = blocks.nifti_to_timeseries(f, atlasname)
-        elif func_is['nifti'] and atlas_is['nifti'] is False:
-            raise NotImplementedError('To work with functional file(s) of nifti format, '
-                                      'specify an atlas file in nifti format.')
-        elif func_is['1D']:
+        elif func_is["nifti"] and atlas_is["nifti"] is False:
+            raise NotImplementedError(
+                "To work with functional file(s) of nifti format, "
+                "specify an atlas file in nifti format."
+            )
+        elif func_is["1D"]:
             t = io.load_txt(f)
-        elif func_is['mat']:
+        elif func_is["mat"]:
             t = io.load_mat(f)
-        elif func_is['xls']:
+        elif func_is["xls"]:
             t = io.load_xls(f)
         else:
-            raise NotImplementedError(f'Input file {f} is not of a supported type.')
+            raise NotImplementedError(f"Input file {f} is not of a supported type.")
 
         timeseries += [t[..., np.newaxis]]
 
     timeseries = np.concatenate(timeseries, axis=-1).squeeze()
     timeseries = ts.normalise_ts(timeseries)
 
     # #### Assign SCGraph object #### #
     scgraph = SCGraph(mtx, timeseries, atlas=atlas, img=img)
     # #### Compute SDI (split low vs high timeseries) and FC #### #
 
     # Run laplacian decomposition and actually filter timeseries.
-    LGR.info('Run laplacian decomposition of structural graph.')
+    LGR.info("Run laplacian decomposition of structural graph.")
     scgraph.structural_decomposition()
-    LGR.info('Compute the energy of the graph and split it in parts.')
+    LGR.info("Compute the energy of the graph and split it in parts.")
     scgraph.compute_graph_energy(mean=True).split_graph()
 
     # If there are more than two splits in the timeseries, compute Generalised SDI
     # This should not happen in this moment.
     if len(scgraph.split_keys) == 2:
-        metric_name = 'sdi'
+        metric_name = "sdi"
         scgraph.compute_sdi()
     elif len(scgraph.split_keys) > 2:
-        metric_name = 'gsdi'
+        metric_name = "gsdi"
         scgraph.compute_gsdi()
     else:
-        raise ValueError('Data is not splitted enough to compute SDI or similar '
-                         'indexes.')
+        raise ValueError(
+            "Data is not splitted enough to compute SDI or similar " "indexes."
+        )
 
-    LGR.info('Compute functional connectivity.')
+    LGR.info("Compute functional connectivity.")
     scgraph.compute_fc(mean=True)
 
     # #### Output results (pt. 1) #### #
 
     # Prepare outputs
     if outname is not None:
         _, outprefix, outext = io.check_ext(io.EXT_ALL, outname, remove=True)
-        outprefix = os.path.join(outdir, f'{os.path.split(outprefix)[1]}_')
+        outprefix = os.path.join(outdir, f"{os.path.split(outprefix)[1]}_")
     else:
-        outprefix = f'{outdir}{os.sep}'
-        outext = ''
+        outprefix = f"{outdir}{os.sep}"
+        outext = ""
 
     # Export non-thresholded metrics
-    LGR.info(f'Export non-thresholded version of {metric_name}.')
+    LGR.info(f"Export non-thresholded version of {metric_name}.")
     blocks.export_metric(scgraph, outext, outprefix)
 
     # Export eigenvalues, eigenvectors, and split timeseries and eigenvectors
     for k in scgraph.split_keys:
-        LGR.info(f'Export {k} timeseries.')
-        io.export_mtx(scgraph.ts_split[k], f'{outprefix}timeseries_{k}', ext=outext)
-        LGR.info(f'Export {k} eigenvectors.')
-        io.export_mtx(scgraph.evec_split[k], f'{outprefix}eigenvec_{k}', ext=outext)
-        LGR.info(f'Export {k} FC (data).')
-        io.export_mtx(scgraph.fc_split[k], f'{outprefix}fc_{k}', ext=outext)
-    LGR.info('Export original FC (data).')
-    io.export_mtx(scgraph.fc, f'{outprefix}fc', ext=outext)
-    LGR.info('Export original eigenvectors.')
-    io.export_mtx(scgraph.eigenvec, f'{outprefix}eigenvec', ext=outext)
-    LGR.info('Export original eigenvalues.')
-    io.export_mtx(scgraph.eigenval, f'{outprefix}eigenval', ext=outext)
+        LGR.info(f"Export {k} timeseries.")
+        io.export_mtx(scgraph.ts_split[k], f"{outprefix}timeseries_{k}", ext=outext)
+        LGR.info(f"Export {k} eigenvectors.")
+        io.export_mtx(scgraph.evec_split[k], f"{outprefix}eigenvec_{k}", ext=outext)
+        LGR.info(f"Export {k} FC (data).")
+        io.export_mtx(scgraph.fc_split[k], f"{outprefix}fc_{k}", ext=outext)
+    LGR.info("Export original FC (data).")
+    io.export_mtx(scgraph.fc, f"{outprefix}fc", ext=outext)
+    LGR.info("Export original eigenvectors.")
+    io.export_mtx(scgraph.eigenvec, f"{outprefix}eigenvec", ext=outext)
+    LGR.info("Export original eigenvalues.")
+    io.export_mtx(scgraph.eigenval, f"{outprefix}eigenval", ext=outext)
 
     # #### Additional steps #### #
 
     # If possible, create plots!
     try:
-        import nilearn as _
         import matplotlib as _
+        import nilearn as _
 
         # Plot original SC and Laplacian
-        LGR.info('Plot laplacian matrix.')
-        viz.plot_connectivity(scgraph.lapl_mtx, f'{outprefix}laplacian.png')
-        LGR.info('Plot structural connectivity matrix.')
-        viz.plot_connectivity(scgraph.mtx, f'{outprefix}sc.png')
+        LGR.info("Plot laplacian matrix.")
+        viz.plot_connectivity(scgraph.lapl_mtx, f"{outprefix}laplacian.png")
+        LGR.info("Plot structural connectivity matrix.")
+        viz.plot_connectivity(scgraph.mtx, f"{outprefix}sc.png")
         # Plot FC
-        LGR.info('Plot original functional connectivity matrix.')
-        viz.plot_connectivity(scgraph.fc, f'{outprefix}fc.png')
+        LGR.info("Plot original functional connectivity matrix.")
+        viz.plot_connectivity(scgraph.fc, f"{outprefix}fc.png")
         for k in scgraph.split_keys:
-            LGR.info(f'Plot {k} functional connectivity matrix.')
-            viz.plot_connectivity(scgraph.fc_split[k],
-                                  f'{outprefix}fc_{k}.png')
+            LGR.info(f"Plot {k} functional connectivity matrix.")
+            viz.plot_connectivity(scgraph.fc_split[k], f"{outprefix}fc_{k}.png")
         # Plot timeseries
-        LGR.info('Plot original timeseries.')
-        viz.plot_grayplot(scgraph.timeseries, f'{outprefix}grayplot.png')
+        LGR.info("Plot original timeseries.")
+        viz.plot_grayplot(scgraph.timeseries, f"{outprefix}grayplot.png")
         for k in scgraph.split_keys:
-            LGR.info(f'Plot {k} timeseries.')
-            viz.plot_grayplot(scgraph.ts_split[k],
-                              f'{outprefix}grayplot_{k}.png')
+            LGR.info(f"Plot {k} timeseries.")
+            viz.plot_grayplot(scgraph.ts_split[k], f"{outprefix}grayplot_{k}.png")
 
         if atlasname is not None:
-            LGR.info(f'Plot {metric_name} markerplot.')
+            LGR.info(f"Plot {metric_name} markerplot.")
             if img is not None:
                 blocks.plot_metric(scgraph, outprefix, img)
             elif atlas is not None:
                 blocks.plot_metric(scgraph, outprefix, atlas)
 
     except ImportError:
-        LGR.warning('The necessary libraries for graphics (nilearn, matplotlib) '
-                    'were not found. Skipping graphics.')
+        LGR.warning(
+            "The necessary libraries for graphics (nilearn, matplotlib) "
+            "were not found. Skipping graphics."
+        )
 
     # If required, create surrogates, test, and export masked metrics
     if surr_type is not None:
-        outprefix += 'mkd_'
+        outprefix += "mkd_"
         if scgraph.sdi is not None:
-            metric_name = 'sdi'
+            metric_name = "sdi"
         elif scgraph.gsdi is not None:
-            metric_name = 'gsdi'
-        LGR.info(f'Test significant {metric_name} against {n_surr} structurally '
-                 f'{surr_type} surrogates.')
-        scgraph.create_surrogates(sc_type=surr_type, n_surr=n_surr,
-                                  seed=seed)
-        scgraph.test_significance(method=method,
-                                  p=p, return_masked=True)
+            metric_name = "gsdi"
+        LGR.info(
+            f"Test significant {metric_name} against {n_surr} structurally "
+            f"{surr_type} surrogates."
+        )
+        scgraph.create_surrogates(sc_type=surr_type, n_surr=n_surr, seed=seed)
+        scgraph.test_significance(method=method, p=p, return_masked=True)
         # Export thresholded metrics
         blocks.export_metric(scgraph, outext, outprefix)
 
         try:
-            import nilearn as _
             import matplotlib as _
+            import nilearn as _
 
             if atlasname is not None:
-                LGR.info(f'Plot {metric_name} markerplot.')
+                LGR.info(f"Plot {metric_name} markerplot.")
                 if img is not None:
                     blocks.plot_metric(scgraph, outprefix, atlas=img, thr=0)
                 elif atlas is not None:
                     blocks.plot_metric(scgraph, outprefix, atlas=atlas, thr=0)
 
         except ImportError:
             pass
 
-    LGR.info(f'End of workflow, find results in {outdir}.')
+    LGR.info(f"End of workflow, find results in {outdir}.")
 
     return 0
 
 
 def _main(argv=None):
     options = _get_parser().parse_args(argv)
 
     save_bash_call(options.fname, options.outdir, options.outname)
 
     nigsp(**vars(options))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _main(sys.argv[1:])
 
 
 """
 Copyright 2022, Stefano Moia.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `nigsp-0.8.0/nigsp/viz.py` & `nigsp-0.9.0/nigsp/viz.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     DPI of the figure
 """
 
 import logging
 
 import numpy as np
 
-
 LGR = logging.getLogger(__name__)
 SET_DPI = 100
 FIGSIZE = (18, 10)
 
 
 def plot_connectivity(mtx, filename=None, closeplot=False):
     """
@@ -58,32 +57,34 @@
     Notes
     -----
     Requires `matplotlib`
     """
     try:
         import matplotlib.pyplot as plt
     except ImportError:
-        raise ImportError('matplotlib is required to plot connectivity matrices. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "matplotlib is required to plot connectivity matrices. "
+            "Please see install instructions."
+        )
 
     mtx = mtx.squeeze()
     if mtx.ndim > 3:
-        raise ValueError('Cannot plot connectivity matrices for matrix of '
-                         'dimensions > 3.')
+        raise ValueError(
+            "Cannot plot connectivity matrices for matrix of " "dimensions > 3."
+        )
     elif mtx.ndim == 3:
-        LGR.warning('Since matrix is 3D, averaging across last '
-                    'dimension.')
+        LGR.warning("Since matrix is 3D, averaging across last " "dimension.")
         mtx = mtx.mean(axis=-1)
 
     if mtx.shape[0] != mtx.shape[1]:
-        LGR.warning('Given matrix is not a square matrix!')
+        LGR.warning("Given matrix is not a square matrix!")
 
-    LGR.info('Creating connectivity plot.')
+    LGR.info("Creating connectivity plot.")
     plt.figure(figsize=FIGSIZE)
-    plt.imshow(mtx, cmap='RdBu')
+    plt.imshow(mtx, cmap="RdBu")
 
     if filename is not None:
         plt.savefig(filename, dpi=SET_DPI)
 
     if closeplot:
         plt.close()
 
@@ -121,31 +122,31 @@
     Notes
     -----
     Requires `matplotlib`
     """
     try:
         import matplotlib.pyplot as plt
     except ImportError:
-        raise ImportError('matplotlib is required to plot grayplots. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "matplotlib is required to plot grayplots. "
+            "Please see install instructions."
+        )
 
     timeseries = timeseries.squeeze()
     if timeseries.ndim > 3:
-        raise ValueError('Cannot plot grayplots for timeseries of '
-                         'dimensions > 3.')
+        raise ValueError("Cannot plot grayplots for timeseries of " "dimensions > 3.")
     elif timeseries.ndim == 3:
-        LGR.warning('Since timeseries is 3D, averaging across last '
-                    'dimension.')
+        LGR.warning("Since timeseries is 3D, averaging across last " "dimension.")
         timeseries = timeseries.mean(axis=-1)
 
-    LGR.info('Creating grayplot.')
+    LGR.info("Creating grayplot.")
     plt.figure(figsize=FIGSIZE)
     vmax = np.percentile(timeseries, 99)
     vmin = np.percentile(timeseries, 1)
-    plt.imshow(timeseries, cmap='gray', vmin=vmin, vmax=vmax)
+    plt.imshow(timeseries, cmap="gray", vmin=vmin, vmax=vmax)
 
     if filename is not None:
         plt.savefig(filename, dpi=SET_DPI)
 
     if closeplot:
         plt.close()
 
@@ -186,43 +187,46 @@
         If coordinates can't be extracted from atlas.
 
     Notes
     -----
     Requires `matplotlib` and `nilearn`
     """
     try:
-        from nilearn.plotting import find_parcellation_cut_coords, plot_markers
         import matplotlib.pyplot as plt
+        from nilearn.plotting import find_parcellation_cut_coords, plot_markers
     except ImportError:
-        raise ImportError('nilearn and matplotlib are required to plot node images. '
-                          'Please see install instructions.')
+        raise ImportError(
+            "nilearn and matplotlib are required to plot node images. "
+            "Please see install instructions."
+        )
     # First check that ns is a valid source of data.
     ns = ns.squeeze()
     if ns.ndim > 2:
-        raise ValueError('Cannot plot node values for matrix of '
-                         'dimensions > 2.')
+        raise ValueError("Cannot plot node values for matrix of " "dimensions > 2.")
     elif ns.ndim == 2:
-        LGR.warning('Given matrix has 2 dimensions, averaging across last '
-                    'dimension.')
+        LGR.warning(
+            "Given matrix has 2 dimensions, averaging across last " "dimension."
+        )
         ns = ns.mean(axis=-1)
 
     # Then treat atlas
     if type(atlas) is np.ndarray:
         if atlas.ndim > 2 or atlas.shape[1] != 3:
-            raise NotImplementedError('Only atlases in nifti format or '
-                                      'list of coordinates are supported.')
+            raise NotImplementedError(
+                "Only atlases in nifti format or " "list of coordinates are supported."
+            )
         else:
             coord = atlas
     else:
         coord = find_parcellation_cut_coords(atlas)
 
     if ns.shape[0] != coord.shape[0]:
-        raise ValueError('Node array and coordinates array have different length.')
+        raise ValueError("Node array and coordinates array have different length.")
 
-    LGR.info('Creating markerplot.')
+    LGR.info("Creating markerplot.")
     plt.figure(figsize=FIGSIZE)
     plot_markers(ns, coord, node_threshold=thr)
 
     if filename is not None:
         plt.savefig(filename, dpi=SET_DPI)
 
     if closeplot:
```

### Comparing `nigsp-0.8.0/nigsp/utils.py` & `nigsp-0.9.0/nigsp/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 LGR
     Logger
 """
 
 import logging
 from itertools import tee
 
-from numpy import asarray, ndarray, prod, empty
-
+from numpy import asarray, empty, ndarray, prod
 
 LGR = logging.getLogger(__name__)
 
 
 def pairwise(iterable):
     """
-    Recreate `itertools.pairwise()` behaviour for python < 3.10 compatibility.
+    Recreate `itertools.pairwise` behaviour for python < 3.10 compatibility.
 
     Parameters
     ----------
     iterable : any iterable object
         The object to iterate through
 
     Returns
@@ -38,16 +37,15 @@
     To be replaced by itertools' pairwise import once support for python < 3.10 is dropped
     """
     a, b = tee(iterable, 2)
     next(b, None)
     return zip(a, b)
 
 
-def change_var_type(var, dtype, varname='an input variable', stop=True,
-                    silent=False):
+def change_var_type(var, dtype, varname="an input variable", stop=True, silent=False):
     """
     Make sure `var` is of type `dtype`.
 
     Parameters
     ----------
     var : str, int, or float
         Variable to change type of
@@ -69,17 +67,17 @@
     ------
     NotImplementedError
         If dtype is not int, float, str, or list
     TypeError
         If variable var is not of type and stop is True
     """
     if type(var) is not dtype and stop:
-        if varname != 'an input variable':
-            varname = f'variable {varname}'
-        raise TypeError(f'{varname} is not of type {dtype}')
+        if varname != "an input variable":
+            varname = f"variable {varname}"
+        raise TypeError(f"{varname} is not of type {dtype}")
 
     if dtype is int:
         tmpvar = int(var)
     elif dtype is float:
         tmpvar = float(var)
     elif dtype is str:
         tmpvar = str(var)
@@ -87,20 +85,20 @@
         tmpvar = asarray(var)
     elif dtype is list:
         if type(var) is list:
             tmpvar = var
         else:
             tmpvar = [var]
     else:
-        raise NotImplementedError(f'Type {dtype.__name__} not supported')
+        raise NotImplementedError(f"Type {dtype.__name__} not supported")
 
     if type(tmpvar) is not type(var):
-        if varname != 'an input variable':
-            varname = f'variable {varname}'
-        msg = f'Changing type of {varname} from {type(var)} to {dtype}'
+        if varname != "an input variable":
+            varname = f"variable {varname}"
+        msg = f"Changing type of {varname} from {type(var)} to {dtype}"
 
         if silent:
             LGR.debug(msg)
         else:
             LGR.warning(msg)
 
     return tmpvar
@@ -121,19 +119,19 @@
         The number of dimensions that should be fixed
 
     Returns
     -------
     np.ndarray, np.ndarray
         The reshaped data and an empty array like it.
     """
-    if data.ndim > idx+1:
+    if data.ndim > idx + 1:
         new_shape = list(data.shape[:idx]) + [prod(data.shape[idx:])]
         data = data.reshape(new_shape)
 
-    return data, empty(data.shape, dtype='float32')
+    return data, empty(data.shape, dtype="float32")
 
 
 """
 Copyright 2022, Stefano Moia.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```


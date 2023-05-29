# Comparing `tmp/skytag-0.2.0.tar.gz` & `tmp/skytag-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytag-0.2.0.tar", last modified: Fri Apr 28 14:57:03 2023, max compression
+gzip compressed data, was "skytag-0.3.0.tar", last modified: Mon May 29 16:45:52 2023, max compression
```

## Comparing `skytag-0.2.0.tar` & `skytag-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.780961 skytag-0.2.0/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       64 2023-04-28 14:53:42.000000 skytag-0.2.0/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-04-28 14:53:42.000000 skytag-0.2.0/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-04-28 14:53:42.000000 skytag-0.2.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4311 2023-04-28 14:57:03.780961 skytag-0.2.0/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3676 2023-04-28 14:53:42.000000 skytag-0.2.0/README.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-04-28 14:57:03.780961 skytag-0.2.0/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1807 2023-04-28 14:53:42.000000 skytag-0.2.0/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.776961 skytag-0.2.0/skytag/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        2 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4128 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.780961 skytag-0.2.0/skytag/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       94 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5118 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/commonutils/prob_at_location.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/default_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      177 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/delete_me.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-04-28 14:53:42.000000 skytag-0.2.0/skytag/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-04-28 14:57:03.776961 skytag-0.2.0/skytag.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4311 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      553 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-04-28 14:56:27.000000 skytag-0.2.0/skytag.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       57 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-04-28 14:57:03.000000 skytag-0.2.0/skytag.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      307 2023-05-29 16:42:07.000000 skytag-0.3.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-29 16:42:07.000000 skytag-0.3.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-29 16:42:07.000000 skytag-0.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-29 16:45:52.853198 skytag-0.3.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4387 2023-05-29 16:42:07.000000 skytag-0.3.0/README.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-29 16:45:52.853198 skytag-0.3.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1857 2023-05-29 16:42:07.000000 skytag-0.3.0/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.849198 skytag-0.3.0/skytag/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      119 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4130 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/skytag/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       94 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5118 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/commonutils/prob_at_location.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2059 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/default_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2058 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-29 16:42:07.000000 skytag-0.3.0/skytag/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-29 16:45:52.853198 skytag-0.3.0/skytag.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5022 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      515 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-29 16:45:20.000000 skytag-0.3.0/skytag.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       57 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-29 16:45:52.000000 skytag-0.3.0/skytag.egg-info/top_level.txt
```

### Comparing `skytag-0.2.0/LICENSE` & `skytag-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/PKG-INFO` & `skytag-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,11 @@
-Metadata-Version: 2.1
-Name: skytag
-Version: 0.2.0
-Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
-Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.2.0.zip
-Author: David Young
-Author-email: d.r.young@qub.ac.uk
-License: MIT
-Keywords: astronomy
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # skytag
 
+[![](https://zenodo.org/badge/633485720.svg)](https://zenodo.org/badge/latestdoi/633485720) 
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/pypi/v/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/conda/vn/conda-forge/skytag)](https://anaconda.org/conda-forge/skytag)
 [![](https://pepy.tech/badge/skytag)](https://pepy.tech/project/skytag)
 [![](https://img.shields.io/github/license/thespacedoctor/skytag)](https://github.com/thespacedoctor/skytag)
@@ -95,11 +80,33 @@
 skytag 170.343532 -40.532255 60065.2232 bayestar.multiorder.fits
 ```
 
 We get:
 
 > This transient is found in the 74.55 credibility region, and occurred 2.85564 days after the map event.
 
+Finally, we can request the localised event distance for this specific sky-position be returned:
+
+```bash 
+skytag -d 170.343532 -40.532255 bayestar.multiorder.fits
+```
+
+> This transient is found in the 74.55% credibility region. At this sky-position the map event is localised to a distance of 75.03 (±19.72) Mpc.
+
 ## Python API
 
 To use skytag in your own Python code, [see here](_autosummary/skytag.commonutils.prob_at_location.html#skytag.commonutils.prob_at_location).
 
+## How to cite skytag
+
+If you use `skytag` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_skytag,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7977906},
+license = {GPL-3.0-only},
+title = {{skytag}},
+url = {https://github.com/thespacedoctor/skytag}
+}
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skytag-0.2.0/README.md` & `skytag-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,28 @@
+Metadata-Version: 2.1
+Name: skytag
+Version: 0.3.0
+Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
+Home-page: https://github.com/thespacedoctor/skytag
+Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.0.zip
+Author: David Young
+Author-email: d.r.young@qub.ac.uk
+License: MIT
+Keywords: astronomy
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # skytag
 
+[![](https://zenodo.org/badge/633485720.svg)](https://zenodo.org/badge/latestdoi/633485720) 
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/pypi/v/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/conda/vn/conda-forge/skytag)](https://anaconda.org/conda-forge/skytag)
 [![](https://pepy.tech/badge/skytag)](https://pepy.tech/project/skytag)
 [![](https://img.shields.io/github/license/thespacedoctor/skytag)](https://github.com/thespacedoctor/skytag)
@@ -78,11 +97,33 @@
 skytag 170.343532 -40.532255 60065.2232 bayestar.multiorder.fits
 ```
 
 We get:
 
 > This transient is found in the 74.55 credibility region, and occurred 2.85564 days after the map event.
 
+Finally, we can request the localised event distance for this specific sky-position be returned:
+
+```bash 
+skytag -d 170.343532 -40.532255 bayestar.multiorder.fits
+```
+
+> This transient is found in the 74.55% credibility region. At this sky-position the map event is localised to a distance of 75.03 (±19.72) Mpc.
+
 ## Python API
 
 To use skytag in your own Python code, [see here](_autosummary/skytag.commonutils.prob_at_location.html#skytag.commonutils.prob_at_location).
 
+## How to cite skytag
+
+If you use `skytag` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_skytag,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7977906},
+license = {GPL-3.0-only},
+title = {{skytag}},
+url = {https://github.com/thespacedoctor/skytag}
+}
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skytag-0.2.0/setup.py` & `skytag-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     'numpy',
     'pandas'
 ]
 
 # READ THE DOCS SERVERS
 exists = os.path.exists("/home/docs/")
 if exists:
+    install_requires = ['fundamentals']
     c_exclude_list = ['healpy', 'astropy',
-                      'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb']
+                      'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb', 'pandas']
     for e in c_exclude_list:
         try:
             install_requires.remove(e)
         except:
             pass
 
 setup(name="skytag",
```

### Comparing `skytag-0.2.0/skytag/cl_utils.py` & `skytag-0.3.0/skytag/cl_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,27 +100,27 @@
         )
 
         if deltas[0] < 0.:
             preposition = "before"
         else:
             preposition = "after"
 
-        print(f"This transient is found in the {prob[0]} credibility region, and occurred {deltas[0]} days {preposition} the map event.")
+        print(f"This transient is found in the {prob[0]}% credibility region, and occurred {deltas[0]} days {preposition} the map event.")
 
     else:
         # CALL FUNCTIONS/OBJECTS
         from skytag.commonutils import prob_at_location
         prob = prob_at_location(
             log=log,
             ra=float(a["ra"]),
             dec=float(a["dec"]),
             mapPath=a["mapPath"]
         )[0]
 
-        print(f"This location is found in the {prob} credibility region of the map.")
+        print(f"This location is found in the {prob}% credibility region of the map.")
 
     ## FINISH LOGGING ##
     endTime = times.get_now_sql_datetime()
     runningTime = times.calculate_time_difference(startTime, endTime)
     log.info('-- FINISHED ATTEMPT TO RUN THE cl_utils.py AT %s (RUNTIME: %s) --' %
              (endTime, runningTime, ))
```

### Comparing `skytag-0.2.0/skytag/commonutils/prob_at_location.py` & `skytag-0.3.0/skytag/commonutils/prob_at_location.py`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/skytag/default_settings.yaml` & `skytag-0.3.0/skytag/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/skytag/setup.cfg` & `skytag-0.3.0/skytag/setup.cfg`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/skytag/test_settings.yaml` & `skytag-0.3.0/skytag/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/skytag/utKit.py` & `skytag-0.3.0/skytag/utKit.py`

 * *Files identical despite different names*

### Comparing `skytag-0.2.0/skytag.egg-info/PKG-INFO` & `skytag-0.3.0/skytag.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: skytag
-Version: 0.2.0
+Version: 0.3.0
 Summary: Annotate transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
 Home-page: https://github.com/thespacedoctor/skytag
-Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.2.0.zip
+Download-URL: https://github.com/thespacedoctor/skytag/archive/v0.3.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # skytag
 
+[![](https://zenodo.org/badge/633485720.svg)](https://zenodo.org/badge/latestdoi/633485720) 
+
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/pypi/v/skytag)](https://pypi.org/project/skytag/)
 [![](https://img.shields.io/conda/vn/conda-forge/skytag)](https://anaconda.org/conda-forge/skytag)
 [![](https://pepy.tech/badge/skytag)](https://pepy.tech/project/skytag)
 [![](https://img.shields.io/github/license/thespacedoctor/skytag)](https://github.com/thespacedoctor/skytag)
@@ -95,11 +97,33 @@
 skytag 170.343532 -40.532255 60065.2232 bayestar.multiorder.fits
 ```
 
 We get:
 
 > This transient is found in the 74.55 credibility region, and occurred 2.85564 days after the map event.
 
+Finally, we can request the localised event distance for this specific sky-position be returned:
+
+```bash 
+skytag -d 170.343532 -40.532255 bayestar.multiorder.fits
+```
+
+> This transient is found in the 74.55% credibility region. At this sky-position the map event is localised to a distance of 75.03 (±19.72) Mpc.
+
 ## Python API
 
 To use skytag in your own Python code, [see here](_autosummary/skytag.commonutils.prob_at_location.html#skytag.commonutils.prob_at_location).
 
+## How to cite skytag
+
+If you use `skytag` in your work, please cite using the following BibTeX entry: 
+
+```bibtex
+@software{Young_skytag,
+author = {Young, David R.},
+doi = {10.5281/zenodo.7977906},
+license = {GPL-3.0-only},
+title = {{skytag}},
+url = {https://github.com/thespacedoctor/skytag}
+}
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `skytag-0.2.0/skytag.egg-info/SOURCES.txt` & `skytag-0.3.0/skytag.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-skytag/CHANGES.md
 skytag/__init__.py
 skytag/__version__.py
 skytag/cl_utils.py
 skytag/default_settings.yaml
-skytag/delete_me.md
 skytag/setup.cfg
 skytag/test_settings.yaml
 skytag/utKit.py
 skytag.egg-info/PKG-INFO
 skytag.egg-info/SOURCES.txt
 skytag.egg-info/dependency_links.txt
 skytag.egg-info/entry_points.txt
```


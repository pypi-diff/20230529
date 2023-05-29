# Comparing `tmp/tiledb_jupyter_bioimg-0.1.0.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.0.tar", last modified: Mon May 29 14:18:17 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.0a0.tar", last modified: Mon May 29 15:03:05 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.0.tar` & `tiledb_jupyter_bioimg-0.1.0a0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.538362 tiledb_jupyter_bioimg-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-29 14:18:17.538362 tiledb_jupyter_bioimg-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:18:17.538362 tiledb_jupyter_bioimg-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.534362 tiledb_jupyter_bioimg-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.534362 tiledb_jupyter_bioimg-0.1.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.534362 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.534362 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.538362 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)   726327 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
--rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/744.55143e2ed71d50019e05.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)   157248 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/939.a2e89434b8bd06a0be08.js
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.1c70cee84cd55593300d.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 14:17:51.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    90610 2023-05-29 14:18:16.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:18:17.534362 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-29 14:18:17.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-29 14:18:17.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:18:17.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:16:40.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 14:18:17.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 14:18:17.000000 tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 14:15:47.000000 tiledb_jupyter_bioimg-0.1.0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.236401 tiledb_jupyter_bioimg-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-29 15:03:05.236401 tiledb_jupyter_bioimg-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-29 15:01:00.000000 tiledb_jupyter_bioimg-0.1.0a0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:03:05.236401 tiledb_jupyter_bioimg-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.228401 tiledb_jupyter_bioimg-0.1.0a0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.228401 tiledb_jupyter_bioimg-0.1.0a0/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.228401 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.232401 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.236401 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   726327 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/744.b944551a62c6c9336934.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)   157248 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/939.a2e89434b8bd06a0be08.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.4d64dcbae56562d70173.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 15:02:39.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90610 2023-05-29 15:03:04.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:03:05.232401 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-29 15:03:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-29 15:03:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:03:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:01:59.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 15:03:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 15:03:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 14:59:05.000000 tiledb_jupyter_bioimg-0.1.0a0/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/LICENSE` & `tiledb_jupyter_bioimg-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tiledb_jupyter_bioimg
-Version: 0.1.0
+Name: tiledb-jupyter-bioimg
+Version: 0.1.0a0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/README.md` & `tiledb_jupyter_bioimg-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/package.json` & `tiledb_jupyter_bioimg-0.1.0a0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'0.1.0-alpha.0'"}*

```diff
@@ -65,9 +65,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.0-alpha.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/setup.py` & `tiledb_jupyter_bioimg-0.1.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/src/index.ts` & `tiledb_jupyter_bioimg-0.1.0a0/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/src/version.ts` & `tiledb_jupyter_bioimg-0.1.0a0/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.0a0/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731359649122806%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4d64dcbae56562d70173.js'}}",*

 * * "'version'": "'0.1.0-alpha.0'"}*

```diff
@@ -25,15 +25,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1c70cee84cd55593300d.js",
+            "load": "static/remoteEntry.4d64dcbae56562d70173.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -70,9 +70,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.0-alpha.0"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/744.55143e2ed71d50019e05.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/744.b944551a62c6c9336934.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -53,11 +53,11 @@
                         version: r,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.1.0","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.0.0-rc.13","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":true,"outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.0-alpha.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@jupyterlab/application":"^3.1.0","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.0.0-rc.13","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":true,"outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/939.a2e89434b8bd06a0be08.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/939.a2e89434b8bd06a0be08.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.1c70cee84cd55593300d.js` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.4d64dcbae56562d70173.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, i, o, d, l, u, f, c, s, p, h, b, v, m, g, y = {
+    var e, r, t, a, n, i, o, d, l, u, f, s, c, p, h, b, v, m, g, y = {
             3661: (e, r, t) => {
-                var n = {
+                var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     i = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
+                    get: () => n,
                     init: () => i
                 })
             }
         },
         w = {};
 
     function j(e) {
@@ -49,25 +49,25 @@
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "06c00f555d53e8ae5aa5",
         344: "9f46f7c199c824b38c64",
         446: "3bf34f45c93ace9c0f28",
         633: "770b26571c8b948a69e3",
         635: "024275f22a135fe53126",
-        744: "55143e2ed71d50019e05",
+        744: "b944551a62c6c9336934",
         747: "433530952542f03ebc71",
         790: "5c9aeadb005c014c315b",
         939: "a2e89434b8bd06a0be08"
     } [e] + ".js?v=" + {
         38: "06c00f555d53e8ae5aa5",
         344: "9f46f7c199c824b38c64",
         446: "3bf34f45c93ace9c0f28",
         633: "770b26571c8b948a69e3",
         635: "024275f22a135fe53126",
-        744: "55143e2ed71d50019e05",
+        744: "b944551a62c6c9336934",
         747: "433530952542f03ebc71",
         790: "5c9aeadb005c014c315b",
         939: "a2e89434b8bd06a0be08"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -75,173 +75,173 @@
             if ("object" == typeof window) return window
         }
     }(), j.hmd = e => ((e = Object.create(e)).children || (e.children = []), Object.defineProperty(e, "exports", {
         enumerable: !0,
         set: () => {
             throw new Error("ES Modules may not assign module.exports or exports.*, Use ESM export syntax, instead: " + e.id)
         }
-    }), e), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", j.l = (t, n, a, i) => {
-        if (e[t]) e[t].push(n);
+    }), e), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", j.l = (t, a, n, i) => {
+        if (e[t]) e[t].push(a);
         else {
             var o, d;
-            if (void 0 !== a)
+            if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
                     var f = l[u];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
                         o = f;
                         break
                     }
                 }
-            o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
-            var c = (r, n) => {
-                    o.onerror = o.onload = null, clearTimeout(s);
-                    var a = e[t];
-                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(n))), r) return r(n)
+            o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
+            var s = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(c);
+                    var n = e[t];
+                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(c.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), d && document.head.appendChild(o)
+            o.onerror = s.bind(null, o.onerror), o.onload = s.bind(null, o.onload), d && document.head.appendChild(o)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, j.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         j.S = {};
         var e = {},
             r = {};
-        j.I = (t, n) => {
-            n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+        j.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
                 var i = j.S[t],
                     o = "@tiledb-inc/jupyter-bioimage-viewer",
-                    d = (e, r, t, n) => {
-                        var a = i[e] = i[e] || {},
-                            d = a[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : o > d.from)) && (a[r] = {
+                    d = (e, r, t, a) => {
+                        var n = i[e] = i[e] || {},
+                            d = n[r];
+                        (!d || !d.loaded && (!a != !d.eager ? a : o > d.from)) && (n[r] = {
                             get: t,
                             from: o,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@jupyter-widgets/base", "6.0.4", (() => Promise.all([j.e(939), j.e(790), j.e(38)]).then((() => () => j(3790))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(939), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.0", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupyter-widgets/base", "6.0.4", (() => Promise.all([j.e(939), j.e(790), j.e(38)]).then((() => () => j(3790))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(939), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.0-alpha.0", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
+                for (var a = t.length - 1; a > -1 && !e;) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                i = (typeof a)[0];
-            if (n >= r.length) return "u" == i;
-            var o = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                i = (typeof n)[0];
+            if (a >= r.length) return "u" == i;
+            var o = r[a],
                 d = (typeof o)[0];
             if (i != d) return "o" == i && "n" == d || "s" == d || "u" == i;
-            if ("o" != i && "u" != i && a != o) return a < o;
-            n++
+            if ("o" != i && "u" != i && n != o) return n < o;
+            a++
         }
-    }, a = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(d = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var a = 1, i = 1; i < e.length; i++) a--, t += "u" == (typeof(d = e[i]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
         var o = [];
         for (i = 1; i < e.length; i++) {
             var d = e[i];
-            o.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? o.pop() + " " + o.pop() : a(d))
+            o.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? o.pop() + " " + o.pop() : n(d))
         }
         return l();
 
         function l() {
             return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
             for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, f, c = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (f = (typeof(u = r[o]))[0])) return !l || ("u" == c ? d > n && !a : "" == c != a);
+                var u, f, s = d < e.length ? (typeof e[d])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(u = r[o]))[0])) return !l || ("u" == s ? d > a && !n : "" == s != n);
                 if ("u" == f) {
-                    if (!l || "u" != c) return !1
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (c == f)
-                        if (d <= n) {
+                    if (s == f)
+                        if (d <= a) {
                             if (u != e[d]) return !1
                         } else {
-                            if (a ? u > e[d] : u < e[d]) return !1;
+                            if (n ? u > e[d] : u < e[d]) return !1;
                             u != e[d] && (l = !1)
                         }
-                else if ("s" != c && "n" != c) {
-                    if (a || d <= n) return !1;
+                else if ("s" != s && "n" != s) {
+                    if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= n || f < c != a) return !1;
+                    if (d <= a || f < s != n) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, d--)
+                } else "s" != s && "n" != s && (l = !1, d--)
             }
         }
-        var s = [],
-            p = s.pop.bind(s);
+        var c = [],
+            p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
         return !!p()
     }, o = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", u = (e, r, t, n) => {
-        var a = d(e, t);
-        return i(n, a) || c(l(e, t, a, n)), s(e[t][a])
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
+        var n = d(e, t);
+        return i(a, n) || s(l(e, t, n, a)), c(e[t][n])
     }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, c = e => {
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var i = j.I(r);
-        return i && i.then ? i.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
-    })(((e, r, t, n) => (o(e, t), u(r, 0, t, n)))), b = p(((e, r, t, n, a) => {
-        var i = r && j.o(r, t) && f(r, t, n);
-        return i ? s(i) : a()
+        return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
+    })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
+        var i = r && j.o(r, t) && f(r, t, a);
+        return i ? c(i) : n()
     })), v = {}, m = {
         883: () => b("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
@@ -260,57 +260,57 @@
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
-                n = r => {
+                a = r => {
                     delete v[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var a = m[e]();
-                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                var n = m[e]();
+                n.then ? r.push(v[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
-                n(e)
+                a(e)
             }
         }))
     }, (() => {
         j.b = document.baseURI || self.location.href;
         var e = {
             448: 0
         };
         j.f.j = (r, t) => {
-            var n = j.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
+            var a = j.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
                 else if (38 != r) {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
+                var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                t.push(a[2] = n);
                 var i = j.p + j.u(r),
                     o = new Error;
                 j.l(i, (t => {
-                    if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
+                    if (j.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                        var n = t && ("load" === t.type ? "missing" : t.type),
                             i = t && t.target && t.target.src;
-                        o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
+                        o.message = "Loading chunk " + r + " failed.\n(" + n + ": " + i + ")", o.name = "ChunkLoadError", o.type = n, o.request = i, a[1](o)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, a, [i, o, d] = t,
+                var a, n, [i, o, d] = t,
                     l = 0;
                 if (i.some((r => 0 !== e[r]))) {
-                    for (n in o) j.o(o, n) && (j.m[n] = o[n]);
+                    for (a in o) j.o(o, a) && (j.m[a] = o[a]);
                     d && d(j)
                 }
-                for (r && r(t); l < i.length; l++) a = i[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < i.length; l++) n = i[l], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
     var S = j(3661);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@tiledb-inc/jupyter-bioimage-viewer"] = S
 })();
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tiledb-jupyter-bioimg
-Version: 0.1.0
+Name: tiledb_jupyter_bioimg
+Version: 0.1.0a0
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.0a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
 tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js
 tiledb_jupyter_bioimg/labextension/static/344.9f46f7c199c824b38c64.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
 tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
 tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.55143e2ed71d50019e05.js
+tiledb_jupyter_bioimg/labextension/static/744.b944551a62c6c9336934.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
 tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js
 tiledb_jupyter_bioimg/labextension/static/790.5c9aeadb005c014c315b.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/939.a2e89434b8bd06a0be08.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.1c70cee84cd55593300d.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.4d64dcbae56562d70173.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.0/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.0a0/tsconfig.json`

 * *Files identical despite different names*


# Comparing `tmp/ipyfilite-0.1.3.tar.gz` & `tmp/ipyfilite-0.1.4.tar.gz`

## Comparing `ipyfilite-0.1.3.tar` & `ipyfilite-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/jest.config.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/examples/introduction.ipynb
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_manager.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_version.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/http.py
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/upload.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/480.d165bff0d974ce3e59d7.js
--rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/568.178bb820c7868260c822.js
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/remoteEntry.607fa641fe3dae437c71.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    28799 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/version.ts
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/jest.config.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_manager.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/_version.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/http.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/upload.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/480.47fe3e6cc3fce727815a.js
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/568.262a61b30c3863712d2a.js
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/remoteEntry.09a079dacd8ff0810e86.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    28799 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/version.ts
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 ipyfilite-0.1.4/PKG-INFO
```

### Comparing `ipyfilite-0.1.3/.eslintrc.js` & `ipyfilite-0.1.4/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/MANIFEST.in` & `ipyfilite-0.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/package.json` & `ipyfilite-0.1.4/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -87,9 +87,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `ipyfilite-0.1.3/tsconfig.json` & `ipyfilite-0.1.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/webpack.config.js` & `ipyfilite-0.1.4/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/Makefile` & `ipyfilite-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/make.bat` & `ipyfilite-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/source/conf.py` & `ipyfilite-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/source/develop-install.rst` & `ipyfilite-0.1.4/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/source/index.rst` & `ipyfilite-0.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/docs/source/installing.rst` & `ipyfilite-0.1.4/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/examples/introduction.ipynb` & `ipyfilite-0.1.4/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/__init__.py` & `ipyfilite-0.1.4/ipyfilite/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/_manager.py` & `ipyfilite-0.1.4/ipyfilite/_manager.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/http.py` & `ipyfilite-0.1.4/ipyfilite/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,30 +128,30 @@
     xhr.open("HEAD", url, False)
     xhr.send(None)
 
     content_length = xhr.getResponseHeader("content-length")
     content_length = int(content_length) if content_length else None
 
     accept_ranges = xhr.getResponseHeader("accept-ranges")
-    accept_ranges = accept_ranges.lower() if content_length else None
+    accept_ranges = accept_ranges.lower() if accept_ranges else None
 
     return (content_length, accept_ranges)
 
 
 def _get_content_length_accept_ranges_urllib(
     url: str,
 ) -> Tuple[Optional[int], Optional[str]]:
     with urllib.request.urlopen(
         urllib.request.Request(url, method="HEAD")
     ) as response:
         content_length = response.getheader("content-length", None)
         content_length = int(content_length) if content_length else None
 
         accept_ranges = response.getheader("accept-ranges", None)
-        accept_ranges = accept_ranges.lower() if content_length else None
+        accept_ranges = accept_ranges.lower() if accept_ranges else None
 
     return (content_length, accept_ranges)
 
 
 if _has_pyodide:
     _RawHTTPBlobPyodide = pyodide.code.run_js("""
 class _RawHTTPBlobPyodide {
```

### Comparing `ipyfilite-0.1.3/ipyfilite/upload.py` & `ipyfilite-0.1.4/ipyfilite/upload.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/labextension/package.json` & `ipyfilite-0.1.4/ipyfilite/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.09a079dacd8ff0810e86.js'}}",*

 * * "'version'": "'0.1.4'"}*

```diff
@@ -46,15 +46,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.607fa641fe3dae437c71.js"
+            "load": "static/remoteEntry.09a079dacd8ff0810e86.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -91,9 +91,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.4"
 }
```

### Comparing `ipyfilite-0.1.3/ipyfilite/labextension/static/480.d165bff0d974ce3e59d7.js` & `ipyfilite-0.1.4/ipyfilite/labextension/static/480.47fe3e6cc3fce727815a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -332,11 +332,11 @@
                         i = o
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.3","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.3/ipyfilite/labextension/static/568.178bb820c7868260c822.js` & `ipyfilite-0.1.4/ipyfilite/labextension/static/568.262a61b30c3863712d2a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -304,11 +304,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.3","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.3/ipyfilite/labextension/static/remoteEntry.607fa641fe3dae437c71.js` & `ipyfilite-0.1.4/ipyfilite/labextension/static/remoteEntry.09a079dacd8ff0810e86.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, f, l, u, s, c, p, d, h, v, g = {
+    var e, r, t, n, i, o, a, f, l, u, s, p, d, c, h, v, g = {
             229: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -37,20 +37,20 @@
     }
     b.m = g, b.c = m, b.d = (e, r) => {
         for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
-        480: "d165bff0d974ce3e59d7",
-        568: "178bb820c7868260c822",
+        480: "47fe3e6cc3fce727815a",
+        568: "262a61b30c3863712d2a",
         829: "989f6f56f2a9f465e0c8"
     } [e] + ".js?v=" + {
-        480: "d165bff0d974ce3e59d7",
-        568: "178bb820c7868260c822",
+        480: "47fe3e6cc3fce727815a",
+        568: "262a61b30c3863712d2a",
         829: "989f6f56f2a9f465e0c8"
     } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -64,24 +64,24 @@
                     var s = l[u];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + i) {
                         a = s;
                         break
                     }
                 }
             a || (f = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
-            var c = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(d);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(c.bind(null, void 0, {
+                d = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = c.bind(null, a.onerror), a.onload = c.bind(null, a.onload), f && document.head.appendChild(a)
+            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), f && document.head.appendChild(a)
         }
     }, (() => {
         b.S = {};
         var e = {},
             r = {};
         b.I = (t, n) => {
             n || (n = []);
@@ -96,15 +96,15 @@
                     var i = o[e] = o[e] || {},
                         f = i[r];
                     (!f || !f.loaded && (1 != !f.eager ? n : a > f.from)) && (i[r] = {
                         get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
                         from: a,
                         eager: !1
                     })
-                })("ipyfilite", "0.1.3"), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                })("ipyfilite", "0.1.4"), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -154,83 +154,83 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
             for (var a = 0, f = 1, l = !0;; f++, a++) {
-                var u, s, c = f < e.length ? (typeof e[f])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !l || ("u" == c ? f > n && !i : "" == c != i);
+                var u, s, p = f < e.length ? (typeof e[f])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !l || ("u" == p ? f > n && !i : "" == p != i);
                 if ("u" == s) {
-                    if (!l || "u" != c) return !1
+                    if (!l || "u" != p) return !1
                 } else if (l)
-                    if (c == s)
+                    if (p == s)
                         if (f <= n) {
                             if (u != e[f]) return !1
                         } else {
                             if (i ? u > e[f] : u < e[f]) return !1;
                             u != e[f] && (l = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != p && "n" != p) {
                     if (i || f <= n) return !1;
                     l = !1, f--
                 } else {
-                    if (f <= n || s < c != i) return !1;
+                    if (f <= n || s < p != i) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, f--)
+                } else "s" != p && "n" != p && (l = !1, f--)
             }
         }
-        var p = [],
-            d = p.pop.bind(p);
+        var d = [],
+            c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            p.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? o(h, r) : !d())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
-        return !!d()
+        return !!c()
     }, a = (e, r) => {
         var t = b.S[e];
         if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, f = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
         var i = f(e, t);
-        return o(n, i) || s(l(e, t, i, n)), c(e[t][i])
+        return o(n, i) || s(l(e, t, i, n)), p(e[t][i])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, i) {
+    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, i) {
         var o = b.I(r);
         return o && o.then ? o.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), d = {}, h = {
-        829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), c = {}, h = {
+        829: () => d("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
     }, v = {
         829: [829]
     }, b.f.consumes = (e, r) => {
         b.o(v, e) && v[e].forEach((e => {
-            if (b.o(d, e)) return r.push(d[e]);
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    d[e] = 0, b.m[e] = t => {
+                    c[e] = 0, b.m[e] = t => {
                         delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete d[e], b.m[e] = t => {
+                    delete c[e], b.m[e] = t => {
                         throw delete b.c[e], r
                     }
                 };
             try {
                 var i = h[e]();
-                i.then ? r.push(d[e] = i.then(t).catch(n)) : t(i)
+                i.then ? r.push(c[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             430: 0
```

### Comparing `ipyfilite-0.1.3/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.4/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/nbextension/index.js` & `ipyfilite-0.1.4/ipyfilite/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -327,15 +327,15 @@
             },
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.3","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.4","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         i = {};
 
     function n(e) {
         var s = i[e];
         if (void 0 !== s) return s.exports;
```

### Comparing `ipyfilite-0.1.3/ipyfilite/nbextension/index.js.map` & `ipyfilite-0.1.4/ipyfilite/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.4/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/extension.ts` & `ipyfilite-0.1.4/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/plugin.ts` & `ipyfilite-0.1.4/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/version.ts` & `ipyfilite-0.1.4/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/widget.ts` & `ipyfilite-0.1.4/src/widget.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/__tests__/index.spec.ts` & `ipyfilite-0.1.4/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/src/__tests__/utils.ts` & `ipyfilite-0.1.4/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/.gitignore` & `ipyfilite-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/LICENSE.txt` & `ipyfilite-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/README.md` & `ipyfilite-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.3/pyproject.toml` & `ipyfilite-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.1.3"
+version = "0.1.4"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -101,15 +101,15 @@
 ]
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "ipyfilite/_version.py" },
 ]
 
 [tool.tbump.version]
-current = "0.1.3"
+current = "0.1.4"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.3/PKG-INFO` & `ipyfilite-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.3
+Version: 0.1.4
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```


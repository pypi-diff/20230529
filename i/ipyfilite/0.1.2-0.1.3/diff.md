# Comparing `tmp/ipyfilite-0.1.2.tar.gz` & `tmp/ipyfilite-0.1.3.tar.gz`

## Comparing `ipyfilite-0.1.2.tar` & `ipyfilite-0.1.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/jest.config.js
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/examples/introduction.ipynb
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_pyodide.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/_version.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/upload.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/480.d8f11be59adb4b02a2b1.js
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/568.7493dd3e4afb6b5b893b.js
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/687.5f576dec2f11535ef5d4.js
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/remoteEntry.baad50c678f67758255b.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    21897 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    72707 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/version.ts
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 ipyfilite-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/jest.config.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_manager.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/_version.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/http.py
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/upload.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/480.d165bff0d974ce3e59d7.js
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/568.178bb820c7868260c822.js
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/remoteEntry.607fa641fe3dae437c71.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    28799 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/version.ts
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 ipyfilite-0.1.3/PKG-INFO
```

### Comparing `ipyfilite-0.1.2/.eslintrc.js` & `ipyfilite-0.1.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/MANIFEST.in` & `ipyfilite-0.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/package.json` & `ipyfilite-0.1.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9520833333333334%*

 * *Differences: {"'dependencies'": "{delete: ['uuid']}",*

 * * "'devDependencies'": "{delete: ['@types/uuid']}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -3,27 +3,25 @@
         "email": "juniper.tyree@helsinki.fi",
         "name": "Juniper Tyree"
     },
     "bugs": {
         "url": "https://github.com/juntyr/ipyfilite/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6",
-        "uuid": "^9.0.0"
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"
     },
     "description": "File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.",
     "devDependencies": {
         "@babel/core": "^7.5.0",
         "@babel/preset-env": "^7.5.0",
         "@jupyter-widgets/base-manager": "^1.0.2",
         "@jupyterlab/builder": "^3.0.0",
         "@lumino/application": "^1.6.0",
         "@lumino/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
-        "@types/uuid": "^9.0.1",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
         "eslint": "^7.4.0",
         "eslint-config-prettier": "^6.11.0",
@@ -89,9 +87,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `ipyfilite-0.1.2/tsconfig.json` & `ipyfilite-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/webpack.config.js` & `ipyfilite-0.1.3/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/Makefile` & `ipyfilite-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/make.bat` & `ipyfilite-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/source/conf.py` & `ipyfilite-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/source/develop-install.rst` & `ipyfilite-0.1.3/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/source/index.rst` & `ipyfilite-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/docs/source/installing.rst` & `ipyfilite-0.1.3/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/examples/introduction.ipynb` & `ipyfilite-0.1.3/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/ipyfilite/__init__.py` & `ipyfilite-0.1.3/ipyfilite/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # Copyright (c) Juniper Tyree.
 # Distributed under the terms of the Modified BSD License.
 
+from . import _manager  # noqa: F401
 from ._version import __version__, version_info  # noqa: F401
+from .http import HTTPFileIO  # noqa: F401
 from .upload import FileUploadLite  # noqa: F401
 
 
 def _jupyter_labextension_paths():
     """Called by Jupyter Lab Server to detect if it is a valid labextension
     and to install the widget
```

### Comparing `ipyfilite-0.1.2/ipyfilite/_pyodide.py` & `ipyfilite-0.1.3/ipyfilite/_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,78 @@
+from __future__ import annotations
+
 import uuid
 import warnings
 from pathlib import Path
 
+from IPython import get_ipython
+from traitlets import Instance
+from traitlets.config import SingletonConfigurable
+
+
+class IpyfiliteManager(SingletonConfigurable):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self._session = uuid.uuid4()
+
+        try:
+            import js  # noqa: F401
+            import pyodide  # noqa: F401
+            import pyodide_js  # noqa: F401
+        except ImportError:
+            warnings.warn(
+                "ipyfilite only works inside a Pyodide kernel in JupyterLite",
+                FutureWarning,
+            )
+        else:
+            self._channel = js.BroadcastChannel.new("ipyfilite")
+            self._channel.onmessage = self._on_file_upload
+
+    @property
+    def session(self) -> uuid.UUID:
+        return self._session
+
+    @classmethod
+    def instance(cls):
+        ip = get_ipython()
+
+        manager = super(IpyfiliteManager, cls).instance(parent=ip)
+
+        # Also make the manager accessible inside IPython
+        if ip is not None and not hasattr(ip, "ipyfilite_manager"):
+            ip.add_traits(
+                ipyfilite_manager=Instance(
+                    IpyfiliteManager, default_value=manager
+                )
+            )
+
+        return manager
 
-def _setup_pyodide_file_upload_channel() -> str:
-    try:
+    def _on_file_upload(self, event):
         import js
         import pyodide
         import pyodide_js
-    except ImportError:
-        warnings.warn(
-            "ipyfilite only works inside a Pyodide kernel in JupyterLite",
-            FutureWarning,
-        )
-
-        return str(uuid.uuid4())
 
-    if getattr(js, "ipyfilite", None) is not None:
-        return js.ipyfilite.session
-
-    def files_upload_callback(event):
         if (
             not getattr(event, "data", None)
             or not getattr(event.data, "files", None)
             or not getattr(event.data, "uuid", None)
             or not getattr(event.data, "session", None)
         ):
             return
 
-        if event.data.session != js.ipyfilite.session:
+        if event.data.session != str(self.session):
             return
 
         upload_path = Path("/uploads") / event.data.uuid
         upload_path.mkdir(parents=True, exist_ok=False)
 
         pyodide_js.FS.mount(
             pyodide_js.FS.filesystems.WORKERFS,
             pyodide.ffi.to_js(
                 {"files": event.data.files},
                 dict_converter=js.Object.fromEntries,
                 create_pyproxies=False,
             ),
             str(upload_path),
         )
-
-    js.ipyfilite = pyodide.ffi.to_js(
-        {
-            "channel": js.Reflect.construct(
-                js.BroadcastChannel,
-                pyodide.ffi.to_js(["ipyfilite"]),
-            ),
-            "session": str(uuid.uuid4()),
-        },
-        dict_converter=js.Object.fromEntries,
-        create_pyproxies=False,
-    )
-    js.ipyfilite.channel.onmessage = files_upload_callback
-
-    return js.ipyfilite.session
```

### Comparing `ipyfilite-0.1.2/ipyfilite/upload.py` & `ipyfilite-0.1.3/ipyfilite/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     widget_serialization,
 )
 from ipywidgets.widgets.trait_types import InstanceDict
 from ipywidgets.widgets.widget_description import DescriptionWidget
 from traitlets import Bool, Bunch, CaselessStrEnum, Dict, Unicode, default
 
 from ._frontend import module_name, module_version
-from ._pyodide import _setup_pyodide_file_upload_channel
-
-__session__ = _setup_pyodide_file_upload_channel()
+from ._manager import IpyfiliteManager
 
 
 def _deserialize_single_file(js):
     uploaded_file = Bunch()
     for attribute in ["name", "type", "size"]:
         uploaded_file[attribute] = js[attribute]
     uploaded_file["last_modified"] = dt.datetime.fromtimestamp(
@@ -143,15 +141,17 @@
     _model_module_version = Unicode(module_version).tag(sync=True)
 
     # Name of the widget view class in front-end
     _view_name = Unicode("FileUploadLiteView").tag(sync=True)
     _view_module = Unicode(module_name).tag(sync=True)
     _view_module_version = Unicode(module_version).tag(sync=True)
 
-    _session = Unicode(__session__, read_only=True).tag(sync=True)
+    _session = Unicode(
+        str(IpyfiliteManager.instance().session), read_only=True
+    ).tag(sync=True)
 
     # Widget specific propertyies, which are defined as traitlets.
     # Any property tagged with `sync=True` is automatically synced to the
     # frontend *any* time it changes in Python. It is synced back to Python
     # from the frontend *any* time the model is touched.
     accept = Unicode(help="File types to accept, empty string for all").tag(
         sync=True
```

### Comparing `ipyfilite-0.1.2/ipyfilite/labextension/package.json` & `ipyfilite-0.1.3/ipyfilite/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9511067708333334%*

 * *Differences: {"'dependencies'": "{delete: ['uuid']}",*

 * * "'devDependencies'": "{delete: ['@types/uuid']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.607fa641fe3dae437c71.js'}}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -3,27 +3,25 @@
         "email": "juniper.tyree@helsinki.fi",
         "name": "Juniper Tyree"
     },
     "bugs": {
         "url": "https://github.com/juntyr/ipyfilite/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6",
-        "uuid": "^9.0.0"
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"
     },
     "description": "File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.",
     "devDependencies": {
         "@babel/core": "^7.5.0",
         "@babel/preset-env": "^7.5.0",
         "@jupyter-widgets/base-manager": "^1.0.2",
         "@jupyterlab/builder": "^3.0.0",
         "@lumino/application": "^1.6.0",
         "@lumino/widgets": "^1.6.0",
         "@types/jest": "^26.0.0",
-        "@types/uuid": "^9.0.1",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
         "eslint": "^7.4.0",
         "eslint-config-prettier": "^6.11.0",
@@ -48,15 +46,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.baad50c678f67758255b.js"
+            "load": "static/remoteEntry.607fa641fe3dae437c71.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -93,9 +91,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `ipyfilite-0.1.2/ipyfilite/labextension/static/480.d8f11be59adb4b02a2b1.js` & `ipyfilite-0.1.3/ipyfilite/labextension/static/480.d165bff0d974ce3e59d7.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -57,63 +57,62 @@
         },
         367: (e, t, i) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FileUploadLiteView = t.FileUploadLiteModel = void 0;
             const n = i(829),
-                s = i(103),
-                l = i(657);
+                s = i(657);
             i(204);
-            class a extends n.DOMWidgetModel {
+            class l extends n.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: a.model_name,
-                        _model_module: a.model_module,
-                        _model_module_version: a.model_module_version,
-                        _view_name: a.view_name,
-                        _view_module: a.view_module,
-                        _view_module_version: a.view_module_version,
-                        _session: s.v4(),
+                        _model_name: l.model_name,
+                        _model_module: l.model_module,
+                        _model_module_version: l.model_module_version,
+                        _view_name: l.view_name,
+                        _view_module: l.view_module,
+                        _view_module_version: l.view_module_version,
+                        _session: n.uuid(),
                         accept: "",
                         description: "Upload",
                         disabled: !1,
                         icon: "upload",
                         button_style: "",
                         multiple: !1,
                         value: [],
                         style: null
                     })
                 }
             }
-            t.FileUploadLiteModel = a, a.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
+            t.FileUploadLiteModel = l, l.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
                 value: {
                     serialize: e => e
                 }
-            }), a.model_name = "FileUploadLiteModel", a.model_module = l.MODULE_NAME, a.model_module_version = l.MODULE_VERSION, a.view_name = "FileUploadLiteView", a.view_module = l.MODULE_NAME, a.view_module_version = l.MODULE_VERSION;
-            class r extends n.DOMWidgetView {
+            }), l.model_name = "FileUploadLiteModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "FileUploadLiteView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
+            class a extends n.DOMWidgetView {
                 preinitialize() {
                     this.tagName = "button"
                 }
                 render() {
                     super.render(), this.el.classList.add("jupyter-widgets"), this.el.classList.add("widget-upload-lite"), this.el.classList.add("jupyter-button"), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.style.display = "none", this.el.addEventListener("click", (() => {
                         this.fileInput.click()
                     })), this.fileInput.addEventListener("click", (() => {
                         this.fileInput.value = ""
                     })), this.fileInput.addEventListener("change", (() => {
                         var e;
-                        const t = s.v4(),
+                        const t = n.uuid(),
                             i = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
                                 name: e.name,
                                 type: e.type,
                                 size: e.size,
                                 last_modified: e.lastModified,
                                 path: `/uploads/${t}/${e.name}`
                             })));
-                        new BroadcastChannel("ipyfilite").postMessage({
+                        r.getBroadcastChannel().postMessage({
                             files: this.fileInput.files,
                             uuid: t,
                             session: this.model.get("_session")
                         }), this.model.set({
                             value: i
                         }), this.touch()
                     })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
@@ -129,27 +128,34 @@
                             e.classList.add("fa"), e.classList.add("fa-" + i), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
                         }
                         this.el.appendChild(document.createTextNode(t))
                     }
                     return this.fileInput.accept = this.model.get("accept"), this.fileInput.multiple = this.model.get("multiple"), super.update()
                 }
                 update_button_style() {
-                    this.update_mapped_classes(r.class_map, "button_style", this.el)
+                    this.update_mapped_classes(a.class_map, "button_style", this.el)
                 }
                 set_button_style() {
-                    this.set_mapped_classes(r.class_map, "button_style", this.el)
+                    this.set_mapped_classes(a.class_map, "button_style", this.el)
                 }
             }
-            t.FileUploadLiteView = r, r.class_map = {
-                primary: ["mod-primary"],
-                success: ["mod-success"],
-                info: ["mod-info"],
-                warning: ["mod-warning"],
-                danger: ["mod-danger"]
-            }
+            var r;
+            t.FileUploadLiteView = a, a.class_map = {
+                    primary: ["mod-primary"],
+                    success: ["mod-success"],
+                    info: ["mod-info"],
+                    warning: ["mod-warning"],
+                    danger: ["mod-danger"]
+                },
+                function(e) {
+                    const t = new BroadcastChannel("ipyfilite");
+                    e.getBroadcastChannel = function() {
+                        return t
+                    }
+                }(r || (r = {}))
         },
         889: (e, t, i) => {
             (t = i(645)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
         },
         645: e => {
             "use strict";
             e.exports = function(e) {
@@ -326,11 +332,11 @@
                         i = o
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.2","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.3","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.2/ipyfilite/labextension/static/568.7493dd3e4afb6b5b893b.js` & `ipyfilite-0.1.3/ipyfilite/labextension/static/568.178bb820c7868260c822.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -29,63 +29,62 @@
         },
         367: (e, t, i) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FileUploadLiteView = t.FileUploadLiteModel = void 0;
             const n = i(829),
-                s = i(103),
-                l = i(657);
+                s = i(657);
             i(204);
-            class a extends n.DOMWidgetModel {
+            class l extends n.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: a.model_name,
-                        _model_module: a.model_module,
-                        _model_module_version: a.model_module_version,
-                        _view_name: a.view_name,
-                        _view_module: a.view_module,
-                        _view_module_version: a.view_module_version,
-                        _session: s.v4(),
+                        _model_name: l.model_name,
+                        _model_module: l.model_module,
+                        _model_module_version: l.model_module_version,
+                        _view_name: l.view_name,
+                        _view_module: l.view_module,
+                        _view_module_version: l.view_module_version,
+                        _session: n.uuid(),
                         accept: "",
                         description: "Upload",
                         disabled: !1,
                         icon: "upload",
                         button_style: "",
                         multiple: !1,
                         value: [],
                         style: null
                     })
                 }
             }
-            t.FileUploadLiteModel = a, a.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
+            t.FileUploadLiteModel = l, l.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
                 value: {
                     serialize: e => e
                 }
-            }), a.model_name = "FileUploadLiteModel", a.model_module = l.MODULE_NAME, a.model_module_version = l.MODULE_VERSION, a.view_name = "FileUploadLiteView", a.view_module = l.MODULE_NAME, a.view_module_version = l.MODULE_VERSION;
-            class o extends n.DOMWidgetView {
+            }), l.model_name = "FileUploadLiteModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "FileUploadLiteView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
+            class a extends n.DOMWidgetView {
                 preinitialize() {
                     this.tagName = "button"
                 }
                 render() {
                     super.render(), this.el.classList.add("jupyter-widgets"), this.el.classList.add("widget-upload-lite"), this.el.classList.add("jupyter-button"), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.style.display = "none", this.el.addEventListener("click", (() => {
                         this.fileInput.click()
                     })), this.fileInput.addEventListener("click", (() => {
                         this.fileInput.value = ""
                     })), this.fileInput.addEventListener("change", (() => {
                         var e;
-                        const t = s.v4(),
+                        const t = n.uuid(),
                             i = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
                                 name: e.name,
                                 type: e.type,
                                 size: e.size,
                                 last_modified: e.lastModified,
                                 path: `/uploads/${t}/${e.name}`
                             })));
-                        new BroadcastChannel("ipyfilite").postMessage({
+                        o.getBroadcastChannel().postMessage({
                             files: this.fileInput.files,
                             uuid: t,
                             session: this.model.get("_session")
                         }), this.model.set({
                             value: i
                         }), this.touch()
                     })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
@@ -101,27 +100,34 @@
                             e.classList.add("fa"), e.classList.add("fa-" + i), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
                         }
                         this.el.appendChild(document.createTextNode(t))
                     }
                     return this.fileInput.accept = this.model.get("accept"), this.fileInput.multiple = this.model.get("multiple"), super.update()
                 }
                 update_button_style() {
-                    this.update_mapped_classes(o.class_map, "button_style", this.el)
+                    this.update_mapped_classes(a.class_map, "button_style", this.el)
                 }
                 set_button_style() {
-                    this.set_mapped_classes(o.class_map, "button_style", this.el)
+                    this.set_mapped_classes(a.class_map, "button_style", this.el)
                 }
             }
-            t.FileUploadLiteView = o, o.class_map = {
-                primary: ["mod-primary"],
-                success: ["mod-success"],
-                info: ["mod-info"],
-                warning: ["mod-warning"],
-                danger: ["mod-danger"]
-            }
+            var o;
+            t.FileUploadLiteView = a, a.class_map = {
+                    primary: ["mod-primary"],
+                    success: ["mod-success"],
+                    info: ["mod-info"],
+                    warning: ["mod-warning"],
+                    danger: ["mod-danger"]
+                },
+                function(e) {
+                    const t = new BroadcastChannel("ipyfilite");
+                    e.getBroadcastChannel = function() {
+                        return t
+                    }
+                }(o || (o = {}))
         },
         889: (e, t, i) => {
             (t = i(645)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
         },
         645: e => {
             "use strict";
             e.exports = function(e) {
@@ -298,11 +304,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.2","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","uuid":"^9.0.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/uuid":"^9.0.1","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.3","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.2/ipyfilite/labextension/static/remoteEntry.baad50c678f67758255b.js` & `ipyfilite-0.1.3/ipyfilite/labextension/static/remoteEntry.607fa641fe3dae437c71.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,286 +1,270 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, f, l, s, d, c, p, h, v, b, g, m, y = {
+    var e, r, t, n, i, o, a, f, l, u, s, c, p, d, h, v, g = {
             229: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(897), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(897), t.e(480)]).then((() => () => t(480)))
+                        "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                i = t.S[n];
+                            if (i && i !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => i
+                    get: () => i,
+                    init: () => o
                 })
             }
         },
-        w = {};
+        m = {};
 
-    function S(e) {
-        var r = w[e];
+    function b(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = w[e] = {
+        var t = m[e] = {
             id: e,
             exports: {}
         };
-        return y[e].call(t.exports, t, t.exports, S), t.exports
+        return g[e].call(t.exports, t, t.exports, b), t.exports
     }
-    S.m = y, S.c = w, S.d = (e, r) => {
-        for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
+    b.m = g, b.c = m, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        480: "d8f11be59adb4b02a2b1",
-        568: "7493dd3e4afb6b5b893b",
-        687: "5f576dec2f11535ef5d4",
-        897: "a37754fc002c48d6bb2f"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        480: "d165bff0d974ce3e59d7",
+        568: "178bb820c7868260c822",
+        829: "989f6f56f2a9f465e0c8"
     } [e] + ".js?v=" + {
-        480: "d8f11be59adb4b02a2b1",
-        568: "7493dd3e4afb6b5b893b",
-        687: "5f576dec2f11535ef5d4",
-        897: "a37754fc002c48d6bb2f"
-    } [e], S.g = function() {
+        480: "d165bff0d974ce3e59d7",
+        568: "178bb820c7868260c822",
+        829: "989f6f56f2a9f465e0c8"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", S.l = (t, n, o, i) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", b.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
-            if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var s = f[l];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+            var a, f;
+            if (void 0 !== i)
+                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
+                    var s = l[u];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + i) {
                         a = s;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+            a || (f = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            var c = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(p);
+                    var i = e[t];
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), u && document.head.appendChild(a)
+            a.onerror = c.bind(null, a.onerror), a.onload = c.bind(null, a.onload), f && document.head.appendChild(a)
         }
-    }, S.r = e => {
-        "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
-            value: "Module"
-        }), Object.defineProperty(e, "__esModule", {
-            value: !0
-        })
     }, (() => {
-        S.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        S.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
-                S.o(S.S, t) || (S.S[t] = {});
-                var i = S.S[t],
+            var i = r[t];
+            if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
+                if (n.push(i), e[t]) return e[t];
+                b.o(b.S, t) || (b.S[t] = {});
+                var o = b.S[t],
                     a = "ipyfilite",
-                    u = (e, r, t, n) => {
-                        var o = i[e] = i[e] || {},
-                            u = o[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : a > u.from)) && (o[r] = {
-                            get: t,
-                            from: a,
-                            eager: !!n
-                        })
-                    },
                     f = [];
-                return "default" === t && (u("ipyfilite", "0.1.2", (() => Promise.all([S.e(897), S.e(568)]).then((() => () => S(568))))), u("uuid", "9.0.0", (() => S.e(687).then((() => () => S(687)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                return "default" === t && ((e, r, t, n) => {
+                    var i = o[e] = o[e] || {},
+                        f = i[r];
+                    (!f || !f.loaded && (1 != !f.eager ? n : a > f.from)) && (i[r] = {
+                        get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
+                        from: a,
+                        eager: !1
+                    })
+                })("ipyfilite", "0.1.3"), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        S.g.importScripts && (e = S.g.location + "");
-        var r = S.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), S.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
+            var i = e[n],
+                o = (typeof i)[0];
+            if (n >= r.length) return "u" == o;
             var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                f = (typeof a)[0];
+            if (o != f) return "o" == o && "n" == f || "s" == f || "u" == o;
+            if ("o" != o && "u" != o && i != a) return i < a;
             n++
         }
-    }, o = e => {
+    }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(f = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, f);
             return t
         }
         var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + f() + ")" : 1 === u ? "(" + f() + " || " + f() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        for (o = 1; o < e.length; o++) {
+            var f = e[o];
+            a.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? a.pop() + " " + a.pop() : i(f))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
-            for (var a = 0, u = 1, f = !0;; u++, a++) {
-                var l, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(l = r[a]))[0])) return !f || ("u" == d ? u > n && !o : "" == d != o);
+                i = n < 0;
+            i && (n = -n - 1);
+            for (var a = 0, f = 1, l = !0;; f++, a++) {
+                var u, s, c = f < e.length ? (typeof e[f])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !l || ("u" == c ? f > n && !i : "" == c != i);
                 if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
-                    if (d == s)
-                        if (u <= n) {
-                            if (l != e[u]) return !1
+                    if (!l || "u" != c) return !1
+                } else if (l)
+                    if (c == s)
+                        if (f <= n) {
+                            if (u != e[f]) return !1
                         } else {
-                            if (o ? l > e[u] : l < e[u]) return !1;
-                            l != e[u] && (f = !1)
+                            if (i ? u > e[f] : u < e[f]) return !1;
+                            u != e[f] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (o || u <= n) return !1;
-                    f = !1, u--
+                else if ("s" != c && "n" != c) {
+                    if (i || f <= n) return !1;
+                    l = !1, f--
                 } else {
-                    if (u <= n || s < d != o) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, u--)
+                    if (f <= n || s < c != i) return !1;
+                    l = !1
+                } else "s" != c && "n" != c && (l = !1, f--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            d = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            p.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? o(h, r) : !d())
         }
-        return !!p()
+        return !!d()
     }, a = (e, r) => {
-        var t = S.S[e];
-        if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, u = (e, r) => {
+    }, f = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", l = (e, r, t, n) => {
-        var o = u(e, t);
-        return i(n, o) || d(f(e, t, o, n)), c(e[t][o])
-    }, s = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = e => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
+        var i = f(e, t);
+        return o(n, i) || s(l(e, t, i, n)), c(e[t][i])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
-        var i = S.I(r);
-        return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), l(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
-        var i = r && S.o(r, t) && s(r, t, n);
-        return i ? c(i) : o()
-    })), b = {}, g = {
-        103: () => v("default", "uuid", [1, 9, 0, 0], (() => S.e(687).then((() => () => S(687))))),
-        829: () => h("default", "@jupyter-widgets/base", [, [1, 6],
+    }, c = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, i) {
+        var o = b.I(r);
+        return o && o.then ? o.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), d = {}, h = {
+        829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
-    }, m = {
-        897: [103, 829]
-    }, S.f.consumes = (e, r) => {
-        S.o(m, e) && m[e].forEach((e => {
-            if (S.o(b, e)) return r.push(b[e]);
+    }, v = {
+        829: [829]
+    }, b.f.consumes = (e, r) => {
+        b.o(v, e) && v[e].forEach((e => {
+            if (b.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    b[e] = 0, S.m[e] = t => {
-                        delete S.c[e], t.exports = r()
+                    d[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], S.m[e] = t => {
-                        throw delete S.c[e], r
+                    delete d[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = g[e]();
-                o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
+                var i = h[e]();
+                i.then ? r.push(d[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             430: 0
         };
-        S.f.j = (r, t) => {
-            var n = S.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (897 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var i = S.p + S.u(r),
+                else if (829 != r) {
+                var i = new Promise(((t, i) => n = e[r] = [t, i]));
+                t.push(n[2] = i);
+                var o = b.p + b.u(r),
                     a = new Error;
-                S.l(i, (t => {
-                    if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            i = t && t.target && t.target.src;
-                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                b.l(o, (t => {
+                    if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                        var i = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
-                    f = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) S.o(a, n) && (S.m[n] = a[n]);
-                    u && u(S)
+                var n, i, [o, a, f] = t,
+                    l = 0;
+                if (o.some((r => 0 !== e[r]))) {
+                    for (n in a) b.o(a, n) && (b.m[n] = a[n]);
+                    f && f(b)
                 }
-                for (r && r(t); f < i.length; f++) o = i[f], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < o.length; l++) i = o[l], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunkipyfilite = self.webpackChunkipyfilite || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), S.nc = void 0;
-    var E = S(229);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = E
+    })(), b.nc = void 0;
+    var y = b(229);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = y
 })();
```

### Comparing `ipyfilite-0.1.2/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.3/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'packages'": '{delete: [2]}'}*

```diff
@@ -7,16 +7,10 @@
             "versionInfo": "3.6.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "1.3.0"
-        },
-        {
-            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2010-2020 Robert Kieffer and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
-            "licenseId": "MIT",
-            "name": "uuid",
-            "versionInfo": "9.0.0"
         }
     ]
 }
```

### Comparing `ipyfilite-0.1.2/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.3/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/src/extension.ts` & `ipyfilite-0.1.3/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/src/plugin.ts` & `ipyfilite-0.1.3/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/src/version.ts` & `ipyfilite-0.1.3/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/src/widget.ts` & `ipyfilite-0.1.3/src/widget.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 // Copyright (c) Juniper Tyree
 // Distributed under the terms of the Modified BSD License.
 
 import {
   DOMWidgetModel,
   DOMWidgetView,
   ISerializers,
+  uuid as uuidv4,
 } from '@jupyter-widgets/base';
-import { v4 as uuidv4 } from 'uuid';
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
 
 // Import the CSS
 import '../css/widget.css';
 
 interface IFileUploaded {
@@ -96,15 +96,15 @@
           type: file.type,
           size: file.size,
           last_modified: file.lastModified,
           path: `/uploads/${uuid}/${file.name}`,
         };
       });
 
-      new BroadcastChannel('ipyfilite').postMessage({
+      Private.getBroadcastChannel().postMessage({
         files: this.fileInput.files,
         uuid,
         session: this.model.get('_session'),
       });
 
       this.model.set({
         value: files,
@@ -165,7 +165,15 @@
     primary: ['mod-primary'],
     success: ['mod-success'],
     info: ['mod-info'],
     warning: ['mod-warning'],
     danger: ['mod-danger'],
   };
 }
+
+namespace Private {
+  const _channel = new BroadcastChannel('ipyfilite');
+
+  export function getBroadcastChannel(): BroadcastChannel {
+    return _channel;
+  }
+}
```

### Comparing `ipyfilite-0.1.2/src/__tests__/index.spec.ts` & `ipyfilite-0.1.3/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/src/__tests__/utils.ts` & `ipyfilite-0.1.3/src/__tests__/utils.ts`

 * *Files 15% similar despite different names*

```diff
@@ -113,7 +113,36 @@
   const modelOptions = {
     widget_manager: widget_manager,
     model_id: id,
   };
 
   return new constructor(attributes, modelOptions);
 }
+
+class BroadcastChannelMock {
+  name: string;
+  constructor(name: string) {
+    this.name = name;
+  }
+  postMessage(data: any) {
+    this.onmessage({ data });
+  }
+  onmessage(event: any) {
+    // no-op
+  }
+  onmessageerror() {
+    // no-op
+  }
+  close() {
+    // no-op
+  }
+  addEventListener() {
+    // no-op
+  }
+  removeEventListener() {
+    // no-op
+  }
+  dispatchEvent(): boolean {
+    return false;
+  }
+}
+window.BroadcastChannel = BroadcastChannelMock;
```

### Comparing `ipyfilite-0.1.2/.gitignore` & `ipyfilite-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/LICENSE.txt` & `ipyfilite-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.2/pyproject.toml` & `ipyfilite-0.1.3/pyproject.toml`

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
-version = "0.1.2"
+version = "0.1.3"
 
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
-current = "0.1.2"
+current = "0.1.3"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.2/PKG-INFO` & `ipyfilite-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.2
+Version: 0.1.3
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -63,18 +63,27 @@
 Provides-Extra: test
 Requires-Dist: nbval; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 
-# ipyfilite
+# ipyfilite &emsp; [![PyPi]][pypi-url] [![NPM]][npm-url] [![License BSD-3-Clause]][bsd-3] [![CI Status]][ci-status]
 
-[![Build Status](https://travis-ci.org/juntyr/ipyfilite.svg?branch=master)](https://travis-ci.org/juntyr/ipyfilite)
-[![codecov](https://codecov.io/gh/juntyr/ipyfilite/branch/master/graph/badge.svg)](https://codecov.io/gh/juntyr/ipyfilite)
+[PyPI]: https://img.shields.io/pypi/v/ipyfilite
+[pypi-url]: https://pypi.org/project/ipyfilite
+
+[NPM]: https://img.shields.io/npm/v/ipyfilite
+[npm-url]: https://www.npmjs.com/package/ipyfilite
+
+[License BSD-3-Clause]: https://img.shields.io/badge/License-BSD_3--Clause-blue.svg
+[bsd-3]: https://opensource.org/licenses/BSD-3-Clause
+
+[CI Status]: https://img.shields.io/github/actions/workflow/status/juntyr/phepy/ci.yml?branch=main&label=CI
+[ci-status]: https://github.com/juntyr/phepy/actions/workflows/ci.yml?query=branch%3Amain
 
 
 File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 
 ## Installation
 
 You can install using `pip`:
```


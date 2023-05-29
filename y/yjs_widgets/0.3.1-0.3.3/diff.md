# Comparing `tmp/yjs_widgets-0.3.1.tar.gz` & `tmp/yjs_widgets-0.3.3.tar.gz`

## Comparing `yjs_widgets-0.3.1.tar` & `yjs_widgets-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.eslintrc.js
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.prettierignore
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.prettierrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.yarnrc.yml
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/install.json
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/tsconfig.json
--rw-r--r--   0        0        0   201745 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/yarn.lock
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/index.ts
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/model.ts
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/types.ts
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/types.ts
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/style/index.js
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/yjs_widgets/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/yjs_widgets/_version.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/LICENSE
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/README.md
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 yjs_widgets-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.eslintrc.js
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.prettierignore
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.yarnrc.yml
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/install.json
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/tsconfig.json
+-rw-r--r--   0        0        0   201745 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yarn.lock
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/index.ts
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/model.ts
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/types.ts
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/types.ts
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/style/index.js
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yjs_widgets/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/yjs_widgets/_version.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/README.md
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 yjs_widgets-0.3.3/PKG-INFO
```

### Comparing `yjs_widgets-0.3.1/.eslintrc.js` & `yjs_widgets-0.3.3/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/CONTRIBUTING.md` & `yjs_widgets-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/package.json` & `yjs_widgets-0.3.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.3'"}*

```diff
@@ -95,9 +95,9 @@
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.3"
 }
```

### Comparing `yjs_widgets-0.3.1/tsconfig.json` & `yjs_widgets-0.3.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/yarn.lock` & `yjs_widgets-0.3.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/model.ts` & `yjs_widgets-0.3.3/src/model.ts`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     }
     this._attrs.unobserve(this._attrsObserver);
     this._disposed.emit();
     Signal.clearData(this);
     this._isDisposed = true;
   }
 
-  getAttr(key: string): string | undefined {
+  getAttr(key: string): any {
     return this._attrs.get(key);
   }
 
   setAttr(key: string, value: any): void {
     this._attrs.set(key, value);
   }
```

### Comparing `yjs_widgets-0.3.1/src/types.ts` & `yjs_widgets-0.3.3/src/types.ts`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,16 @@
   attrsChange?: MapChange;
   stateChange?: StateChange<any>[];
 }
 
 export interface IJupyterYDoc extends IDisposable {
   attrs: JSONObject;
 
-  getAttr(key: string): string | undefined;
-  setAttr(key: string, value: string): void;
+  getAttr(key: string): any;
+  setAttr(key: string, value: any): void;
   removeAttr(key: string): void;
 
   attrsChanged: ISignal<IJupyterYDoc, MapChange>;
   ydoc: Y.Doc;
   commMetadata: {[key: string]: any};
   disposed: ISignal<any, void>;
 }
```

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/index.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/model.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/types.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/types.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/view.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/widgetManager.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/src/notebookrenderer/yCommProvider.ts` & `yjs_widgets-0.3.3/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/.gitignore` & `yjs_widgets-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/LICENSE` & `yjs_widgets-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/README.md` & `yjs_widgets-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/pyproject.toml` & `yjs_widgets-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yjs_widgets-0.3.1/PKG-INFO` & `yjs_widgets-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yjs_widgets
-Version: 0.3.1
+Version: 0.3.3
 Summary: A JupyterLab extension for widgets based on Yjs.
 Project-URL: Homepage, https://github.com/QuantStack/yjs-widgets
 Project-URL: Bug Tracker, https://github.com/QuantStack/yjs-widgets/issues
 Project-URL: Repository, https://github.com/QuantStack/yjs-widgets.git
 Author-email: Trung Le <leductrungxf@gmail.com>
 License: BSD 3-Clause License
```


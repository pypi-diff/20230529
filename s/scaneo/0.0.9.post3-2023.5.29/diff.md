# Comparing `tmp/scaneo-0.0.9.post3.tar.gz` & `tmp/scaneo-2023.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-0.0.9.post3.tar", max compression
+gzip compressed data, was "scaneo-2023.5.29.tar", max compression
```

## Comparing `scaneo-0.0.9.post3.tar` & `scaneo-2023.5.29.tar`

### file list

```diff
@@ -1,76 +1,26 @@
--rw-r--r--   0        0        0     6199 2023-05-24 09:26:01.616553 scaneo-0.0.9.post3/README.md
--rw-r--r--   0        0        0      347 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 09:29:06.132298 scaneo-0.0.9.post3/scaneo/__init__.py
--rw-r--r--   0        0        0     1037 2023-05-24 12:36:44.461343 scaneo-0.0.9.post3/scaneo/api.py
--rw-r--r--   0        0        0      584 2023-05-24 12:31:10.176185 scaneo-0.0.9.post3/scaneo/main.py
--rw-r--r--   0        0        0     7056 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2836 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js
--rw-r--r--   0        0        0      238 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/stores.a2dd7dd6.js
--rw-r--r--   0        0        0     5722 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/app.77ddf75f.js
--rw-r--r--   0        0        0    23876 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/start.8814d3e0.js
--rw-r--r--   0        0        0      719 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/0.663a3db5.js
--rw-r--r--   0        0        0      800 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/1.86013cb7.js
--rw-r--r--   0        0        0     1328 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/2.35154476.js
--rw-r--r--   0        0        0      372 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/3.cb33ee2b.js
--rw-r--r--   0        0        0       27 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/_app/version.json
--rw-r--r--   0        0        0     7056 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2836 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.1df1af67.js
--rw-r--r--   0        0        0     2836 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.2ddc59bf.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.36580b7a.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.4ffcfa45.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.7210d6da.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.76776748.js
--rw-r--r--   0        0        0     2836 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.8ca8a18c.js
--rw-r--r--   0        0        0     2838 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/singletons.a1fc90ce.js
--rw-r--r--   0        0        0      238 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.24647ac6.js
--rw-r--r--   0        0        0      238 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.6a2effc3.js
--rw-r--r--   0        0        0      238 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.6bb331f9.js
--rw-r--r--   0        0        0      238 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.a2dd7dd6.js
--rw-r--r--   0        0        0      238 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.c0d9e12d.js
--rw-r--r--   0        0        0      238 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.dd0e8ee4.js
--rw-r--r--   0        0        0      238 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.ebd8fd52.js
--rw-r--r--   0        0        0      238 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/chunks/stores.ebfb6cb3.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.11edd54e.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.19a98a41.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.450412c1.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.6cae644b.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:14:25.943839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.77ddf75f.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.9fea0e15.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f45b1117.js
--rw-r--r--   0        0        0     5722 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/app.f61a80e5.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.215451c5.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.2fa5423d.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.31eba02c.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.8814d3e0.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.9cce7b47.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.a5a82fbc.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.aca2ebd3.js
--rw-r--r--   0        0        0    23876 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/entry/start.f2579792.js
--rw-r--r--   0        0        0      719 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.663a3db5.js
--rw-r--r--   0        0        0      676 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/0.6e67e459.js
--rw-r--r--   0        0        0      800 2023-05-24 12:34:55.796976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.519d840f.js
--rw-r--r--   0        0        0      800 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.5cf77ad0.js
--rw-r--r--   0        0        0      800 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.7a4b92ca.js
--rw-r--r--   0        0        0      800 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.86013cb7.js
--rw-r--r--   0        0        0      800 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.8a8831ee.js
--rw-r--r--   0        0        0      800 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.917eb664.js
--rw-r--r--   0        0        0      800 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.a0346c75.js
--rw-r--r--   0        0        0      800 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/1.f89a0772.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.0e7d4a8f.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:31:51.180333 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.0f870bcf.js
--rw-r--r--   0        0        0     1328 2023-05-24 12:14:25.951839 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.35154476.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:36:09.517226 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.b937115c.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:17:37.064518 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.cef09f18.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:34:55.800976 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.d76a8d27.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:32:47.980534 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.da635a22.js
--rw-r--r--   0        0        0     1269 2023-05-24 12:14:59.847912 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/2.eb1e05c8.js
--rw-r--r--   0        0        0      372 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/immutable/nodes/3.cb33ee2b.js
--rw-r--r--   0        0        0       27 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/_app/version.json
--rw-r--r--   0        0        0     1571 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/favicon.png
--rw-r--r--   0        0        0     1574 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/index.html
--rw-r--r--   0        0        0     1363 2023-05-24 12:36:49.181358 scaneo-0.0.9.post3/scaneo/ui/build/kk.html
--rw-r--r--   0        0        0     1571 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/favicon.png
--rw-r--r--   0        0        0     1571 2023-05-24 12:34:37.332913 scaneo-0.0.9.post3/scaneo/ui/index.html
--rw-r--r--   0        0        0     1363 2023-05-24 11:13:45.790816 scaneo-0.0.9.post3/scaneo/ui/kk.html
--rw-r--r--   0        0        0     7260 1970-01-01 00:00:00.000000 scaneo-0.0.9.post3/setup.py
--rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 scaneo-0.0.9.post3/PKG-INFO
+-rw-r--r--   0        0        0      624 2023-05-29 12:30:06.392207 scaneo-2023.5.29/README.md
+-rw-r--r--   0        0        0      350 2023-05-29 12:46:28.650827 scaneo-2023.5.29/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/cli/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/cli/hello.py
+-rw-r--r--   0        0        0       57 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/hello.py
+-rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/main.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/settings.py
+-rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/test.py
+-rw-r--r--   0        0        0     7056 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/index.6dba6488.js
+-rw-r--r--   0        0        0     2838 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/singletons.9f3ec903.js
+-rw-r--r--   0        0        0      238 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/stores.57c5405b.js
+-rw-r--r--   0        0        0     5788 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/app.b9b6597a.js
+-rw-r--r--   0        0        0    23876 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/start.4cfa1304.js
+-rw-r--r--   0        0        0      703 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/0.67f61f78.js
+-rw-r--r--   0        0        0      800 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/1.6c933e22.js
+-rw-r--r--   0        0        0     1259 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/2.39aa7785.js
+-rw-r--r--   0        0        0      663 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/3.d433accd.js
+-rw-r--r--   0        0        0       27 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-05-29 12:46:28.646827 scaneo-2023.5.29/scaneo/ui/favicon.png
+-rw-r--r--   0        0        0     1572 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/index.html
+-rw-r--r--   0        0        0     1454 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/kk/index.html
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 scaneo-2023.5.29/setup.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 scaneo-2023.5.29/PKG-INFO
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/index.6dba6488.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/index.6dba6488.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/chunks/singletons.1df1af67.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/singletons.9f3ec903.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -15,35 +15,35 @@
             if (c) {
                 for (let i = 0; i < u.length; i += 2) u[i][0](u[i + 1]);
                 u.length = 0
             }
         }
     }
 
-    function l(s) {
+    function a(s) {
         r(s(e))
     }
 
-    function a(s, c = d) {
+    function l(s, c = d) {
         const i = [s, c];
         return o.add(i), o.size === 1 && (n = t(r) || d), s(e), () => {
             o.delete(i), o.size === 0 && n && (n(), n = null)
         }
     }
     return {
         set: r,
-        update: l,
-        subscribe: a
+        update: a,
+        subscribe: l
     }
 }
 var g;
-const E = ((g = globalThis.__sveltekit_znfcad) == null ? void 0 : g.base) ?? "";
+const E = ((g = globalThis.__sveltekit_1704jlc) == null ? void 0 : g.base) ?? "";
 var k;
-const A = ((k = globalThis.__sveltekit_znfcad) == null ? void 0 : k.assets) ?? E,
-    R = "1684924446031",
+const A = ((k = globalThis.__sveltekit_1704jlc) == null ? void 0 : k.assets) ?? E,
+    R = "1685364387525",
     y = "sveltekit:snapshot",
     I = "sveltekit:scroll",
     x = "sveltekit:index",
     _ = {
         tap: 1,
         hover: 2,
         viewport: 3,
@@ -90,64 +90,64 @@
 function N(e, t) {
     let n;
     try {
         n = new URL(e instanceof SVGAElement ? e.href.baseVal : e.href, document.baseURI)
     } catch {}
     const o = e instanceof SVGAElement ? e.target.baseVal : e.target,
         r = !n || !!o || T(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
-        l = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
+        a = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
     return {
         url: n,
         external: r,
         target: o,
-        download: l
+        download: a
     }
 }
 
-function z(e) {
+function j(e) {
     let t = null,
         n = null,
         o = null,
         r = null,
-        l = null,
         a = null,
+        l = null,
         s = e;
-    for (; s && s !== document.documentElement;) o === null && (o = f(s, "preload-code")), r === null && (r = f(s, "preload-data")), t === null && (t = f(s, "keepfocus")), n === null && (n = f(s, "noscroll")), l === null && (l = f(s, "reload")), a === null && (a = f(s, "replacestate")), s = v(s);
+    for (; s && s !== document.documentElement;) o === null && (o = f(s, "preload-code")), r === null && (r = f(s, "preload-data")), t === null && (t = f(s, "keepfocus")), n === null && (n = f(s, "noscroll")), a === null && (a = f(s, "reload")), l === null && (l = f(s, "replacestate")), s = v(s);
     return {
         preload_code: b[o ?? "off"],
         preload_data: b[r ?? "off"],
         keep_focus: t === "off" ? !1 : t === "" ? !0 : null,
         noscroll: n === "off" ? !1 : n === "" ? !0 : null,
-        reload: l === "off" ? !1 : l === "" ? !0 : null,
-        replace_state: a === "off" ? !1 : a === "" ? !0 : null
+        reload: a === "off" ? !1 : a === "" ? !0 : null,
+        replace_state: l === "off" ? !1 : l === "" ? !0 : null
     }
 }
 
 function h(e) {
     const t = p(e);
     let n = !0;
 
     function o() {
-        n = !0, t.update(a => a)
+        n = !0, t.update(l => l)
     }
 
-    function r(a) {
-        n = !1, t.set(a)
+    function r(l) {
+        n = !1, t.set(l)
     }
 
-    function l(a) {
+    function a(l) {
         let s;
         return t.subscribe(c => {
-            (s === void 0 || n && c !== s) && a(s = c)
+            (s === void 0 || n && c !== s) && l(s = c)
         })
     }
     return {
         notify: o,
         set: r,
-        subscribe: l
+        subscribe: a
     }
 }
 
 function S() {
     const {
         set: e,
         subscribe: t
@@ -159,16 +159,16 @@
             const r = await fetch(`${A}/_app/version.json`, {
                 headers: {
                     pragma: "no-cache",
                     "cache-control": "no-cache"
                 }
             });
             if (!r.ok) return !1;
-            const a = (await r.json()).version !== R;
-            return a && (e(!0), clearTimeout(n)), a
+            const l = (await r.json()).version !== R;
+            return l && (e(!0), clearTimeout(n)), l
         } catch {
             return !1
         }
     }
     return {
         subscribe: t,
         check: o
@@ -185,9 +185,9 @@
 const V = {
     url: h({}),
     page: h({}),
     navigating: p(null),
     updated: S()
 };
 export {
-    x as I, _ as P, I as S, y as a, N as b, z as c, U as d, E as e, L as f, O as g, P as h, T as i, V as s
+    x as I, _ as P, I as S, y as a, N as b, j as c, U as d, E as e, L as f, O as g, P as h, T as i, V as s
 };
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/app.77ddf75f.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/app.b9b6597a.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -352,15 +352,15 @@
             components: 0,
             form: 2,
             data_0: 3,
             data_1: 4
         })
     }
 }
-const re = [() => y(() => import("../nodes/0.663a3db5.js"), ["../nodes/0.663a3db5.js", "../chunks/index.6dba6488.js"], import.meta.url), () => y(() => import("../nodes/1.86013cb7.js"), ["../nodes/1.86013cb7.js", "../chunks/index.6dba6488.js", "../chunks/stores.a2dd7dd6.js", "../chunks/singletons.1df1af67.js"], import.meta.url), () => y(() => import("../nodes/2.35154476.js"), ["../nodes/2.35154476.js", "../chunks/index.6dba6488.js", "../chunks/stores.a2dd7dd6.js", "../chunks/singletons.1df1af67.js"], import.meta.url), () => y(() => import("../nodes/3.cb33ee2b.js"), ["../nodes/3.cb33ee2b.js", "../chunks/index.6dba6488.js"], import.meta.url)],
+const re = [() => y(() => import("../nodes/0.67f61f78.js"), ["../nodes/0.67f61f78.js", "../chunks/index.6dba6488.js"], import.meta.url), () => y(() => import("../nodes/1.6c933e22.js"), ["../nodes/1.6c933e22.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url), () => y(() => import("../nodes/2.39aa7785.js"), ["../nodes/2.39aa7785.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url), () => y(() => import("../nodes/3.d433accd.js"), ["../nodes/3.d433accd.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url)],
     oe = [],
     ae = {
         "/": [2],
         "/kk": [3]
     },
     le = {
         handleError: ({
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/entry/start.8814d3e0.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/start.4cfa1304.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
     c as le,
     s as V,
     i as _e,
     d as Q,
     e as K,
     P as Fe,
     h as We
-} from "../chunks/singletons.1df1af67.js";
+} from "../chunks/singletons.9f3ec903.js";
 
 function Xe(t, o) {
     return t === "/" || o === "ignore" ? t : o === "never" ? t.endsWith("/") ? t.slice(0, -1) : t : o === "always" && !t.endsWith("/") ? t + "/" : t
 }
 
 function Ze(t) {
     return t.split("%25").map(decodeURI).join("%25")
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/1.86013cb7.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/1.6c933e22.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -14,15 +14,15 @@
     G as E,
     u as $,
     H as q,
     I as y
 } from "../chunks/index.6dba6488.js";
 import {
     p as C
-} from "../chunks/stores.a2dd7dd6.js";
+} from "../chunks/stores.57c5405b.js";
 
 function G(l) {
     var f;
     let a, t = l[0].status + "",
         r, o, n, p = ((f = l[0].error) == null ? void 0 : f.message) + "",
         c;
     return {
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/_app/immutable/nodes/2.35154476.js` & `scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/2.39aa7785.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,85 +1,82 @@
 import {
-    S as q,
-    i as w,
-    s as C,
+    S as H,
+    i as N,
+    s as O,
     k,
     q as m,
-    a as A,
+    a as $,
     l as x,
-    m as y,
+    m as E,
     r as u,
-    h as i,
-    c as I,
-    n as $,
-    b as _,
+    h as r,
+    c as q,
+    n as w,
+    b as d,
     G as c,
-    H as P,
-    I as H
+    H as A,
+    I as P
 } from "../chunks/index.6dba6488.js";
 import {
-    p as K
-} from "../chunks/stores.a2dd7dd6.js";
-const L = "";
+    p as V
+} from "../chunks/stores.57c5405b.js";
 
-function U(p) {
-    let o, h, e, a, l, s, f, b, d, n, E;
+function W(p) {
+    let a, h, s, e, l, o, f, y, _, n, b;
     return {
         c() {
-            o = k("h1"), h = m("Welcome to SvelteKit"), e = A(), a = k("p"), l = m("Visit "), s = k("a"), f = m("kit.svelte.dev"), b = m(" to read the documentation"), d = A(), n = k("a"), E = m("hola"), this.h()
+            a = k("h1"), h = m("Welcome to SCANEO"), s = $(), e = k("p"), l = m("Visit "), o = k("a"), f = m("kit.svelte.dev"), y = m(" to read the documentation"), _ = $(), n = k("a"), b = m("hola"), this.h()
         },
         l(t) {
-            o = x(t, "H1", {});
-            var r = y(o);
-            h = u(r, "Welcome to SvelteKit"), r.forEach(i), e = I(t), a = x(t, "P", {});
-            var v = y(a);
-            l = u(v, "Visit "), s = x(v, "A", {
+            a = x(t, "H1", {});
+            var i = E(a);
+            h = u(i, "Welcome to SCANEO"), i.forEach(r), s = q(t), e = x(t, "P", {});
+            var v = E(e);
+            l = u(v, "Visit "), o = x(v, "A", {
                 href: !0
             });
-            var S = y(s);
-            f = u(S, "kit.svelte.dev"), S.forEach(i), b = u(v, " to read the documentation"), v.forEach(i), d = I(t), n = x(t, "A", {
+            var S = E(o);
+            f = u(S, "kit.svelte.dev"), S.forEach(r), y = u(v, " to read the documentation"), v.forEach(r), _ = q(t), n = x(t, "A", {
                 href: !0
             });
-            var g = y(n);
-            E = u(g, "hola"), g.forEach(i), this.h()
+            var C = E(n);
+            b = u(C, "hola"), C.forEach(r), this.h()
         },
         h() {
-            $(s, "href", "https://kit.svelte.dev"), $(n, "href", "/kk")
+            w(o, "href", "https://kit.svelte.dev"), w(n, "href", "/kk")
         },
-        m(t, r) {
-            _(t, o, r), c(o, h), _(t, e, r), _(t, a, r), c(a, l), c(a, s), c(s, f), c(a, b), _(t, d, r), _(t, n, r), c(n, E)
+        m(t, i) {
+            d(t, a, i), c(a, h), d(t, s, i), d(t, e, i), c(e, l), c(e, o), c(o, f), c(e, y), d(t, _, i), d(t, n, i), c(n, b)
         },
-        p: P,
-        i: P,
-        o: P,
+        p: A,
+        i: A,
+        o: A,
         d(t) {
-            t && i(o), t && i(e), t && i(a), t && i(d), t && i(n)
+            t && r(a), t && r(s), t && r(e), t && r(_), t && r(n)
         }
     }
 }
 
-function V(p, o, h) {
-    let e;
-    H(p, K, l => h(0, e = l));
-    const a = async () => {
-        console.log("ei", L, e.url.origin);
-        const l = e.url.origin;
-        console.log(l);
+function G(p, a, h) {
+    let s;
+    P(p, V, l => h(0, s = l));
+    const e = async () => {
+        const l = s.url.origin;
         try {
-            const f = await (await fetch(l + "/api/test")).text();
+            const f = await (await fetch(l + "/test")).text();
             console.log(f)
-        } catch (s) {
-            console.log(s)
+        } catch (o) {
+            console.log(o)
         }
     };
     return p.$$.update = () => {
-        p.$$.dirty & 1 && e.url.origin && a()
-    }, [e]
+        p.$$.dirty & 1 && s.url.origin && e()
+    }, [s]
 }
-class G extends q {
-    constructor(o) {
-        super(), w(this, o, V, U, C, {})
+class j extends H {
+    constructor(a) {
+        super(), N(this, a, G, W, O, {})
     }
 }
 export {
-    G as component
+    j as component
 };
```

### Comparing `scaneo-0.0.9.post3/scaneo/ui/build/favicon.png` & `scaneo-2023.5.29/scaneo/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.9.post3/scaneo/ui/build/index.html` & `scaneo-2023.5.29/scaneo/ui/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
 		<meta charset="utf-8" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.aca2ebd3.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/start.4cfa1304.js">
 		<link rel="modulepreload" href="./_app/immutable/chunks/index.6dba6488.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.2ddc59bf.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.450412c1.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/0.6e67e459.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/2.0e7d4a8f.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.6a2effc3.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.9f3ec903.js">
+		<link rel="modulepreload" href="./_app/immutable/entry/app.b9b6597a.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/0.67f61f78.js">
+		<link rel="modulepreload" href="./_app/immutable/nodes/2.39aa7785.js">
+		<link rel="modulepreload" href="./_app/immutable/chunks/stores.57c5405b.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
-<h1>Welcome to SvelteKit</h1>
+<h1>Welcome to SCANEO</h1>
 <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
 <a href="/kk">hola</a>
 
 
 			
 			<script>
 				{
-					__sveltekit_rgg8pi = {
+					__sveltekit_1704jlc = {
 						base: new URL(".", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.aca2ebd3.js"),
-						import("./_app/immutable/entry/app.450412c1.js")
+						import("./_app/immutable/entry/start.4cfa1304.js"),
+						import("./_app/immutable/entry/app.b9b6597a.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
 							node_ids: [0, 2],
 							data,
 							form: null,
 							error: null
 						});
```

#### html2text {}

```diff
@@ -4,10 +4,10 @@
 
 
 
 
 
 
 
-****** Welcome to SvelteKit ******
+****** Welcome to SCANEO ******
 Visit kit.svelte.dev to read the documentation
 hola
```


# Comparing `tmp/scaneo-2023.5.29.tar.gz` & `tmp/scaneo-2023.5.29.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-2023.5.29.tar", max compression
+gzip compressed data, was "scaneo-2023.5.29.post2.tar", max compression
```

## Comparing `scaneo-2023.5.29.tar` & `scaneo-2023.5.29.post2.tar`

### file list

```diff
@@ -1,26 +1,48 @@
--rw-r--r--   0        0        0      624 2023-05-29 12:30:06.392207 scaneo-2023.5.29/README.md
--rw-r--r--   0        0        0      350 2023-05-29 12:46:28.650827 scaneo-2023.5.29/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/__init__.py
--rw-r--r--   0        0        0      752 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/api.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/cli/__init__.py
--rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/cli/hello.py
--rw-r--r--   0        0        0       57 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/hello.py
--rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/main.py
--rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/__init__.py
--rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/settings.py
--rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.5.29/scaneo/routers/test.py
--rw-r--r--   0        0        0     7056 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2838 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/singletons.9f3ec903.js
--rw-r--r--   0        0        0      238 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/stores.57c5405b.js
--rw-r--r--   0        0        0     5788 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/app.b9b6597a.js
--rw-r--r--   0        0        0    23876 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/start.4cfa1304.js
--rw-r--r--   0        0        0      703 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/0.67f61f78.js
--rw-r--r--   0        0        0      800 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/1.6c933e22.js
--rw-r--r--   0        0        0     1259 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/2.39aa7785.js
--rw-r--r--   0        0        0      663 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/3.d433accd.js
--rw-r--r--   0        0        0       27 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/_app/version.json
--rw-r--r--   0        0        0     1571 2023-05-29 12:46:28.646827 scaneo-2023.5.29/scaneo/ui/favicon.png
--rw-r--r--   0        0        0     1572 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/index.html
--rw-r--r--   0        0        0     1454 2023-05-29 12:46:28.650827 scaneo-2023.5.29/scaneo/ui/kk/index.html
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 scaneo-2023.5.29/setup.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 scaneo-2023.5.29/PKG-INFO
+-rw-r--r--   0        0        0      624 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/README.md
+-rw-r--r--   0        0        0      352 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/api.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/cli/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/cli/hello.py
+-rw-r--r--   0        0        0       57 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/hello.py
+-rw-r--r--   0        0        0     1105 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/main.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/routers/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/routers/settings.py
+-rw-r--r--   0        0        0      307 2023-05-29 12:30:06.392207 scaneo-2023.5.29.post2/scaneo/routers/test.py
+-rw-r--r--   0        0        0    65275 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/0.cdaa43fa.css
+-rw-r--r--   0        0        0    35557 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/2.ec88bf81.css
+-rw-r--r--   0        0        0     1674 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/PaintPolygon.08b3549b.css
+-rw-r--r--   0        0        0    65273 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/_layout.b00db34a.css
+-rw-r--r--   0        0        0    35641 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/_page.8345281d.css
+-rw-r--r--   0        0        0     5551 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/assets/spritesheet.7077bae9.svg
+-rw-r--r--   0        0        0    27736 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/2.cb8e4807.js
+-rw-r--r--   0        0        0    37061 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/PaintPolygon.47895a92.js
+-rw-r--r--   0        0        0      827 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/ToggleToolset.452a7038.js
+-rw-r--r--   0        0        0      236 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/_commonjsHelpers.725317a4.js
+-rw-r--r--   0        0        0    11356 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/index.8c237fac.js
+-rw-r--r--   0        0        0   150001 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/leaflet-src.20dcb89b.js
+-rw-r--r--   0        0        0    67243 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/leaflet.draw.45fd9d9b.js
+-rw-r--r--   0        0        0     1229 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/parse.bee59afc.js
+-rw-r--r--   0        0        0      759 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/preload-helper.41c905a7.js
+-rw-r--r--   0        0        0     2899 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/singletons.d791afcf.js
+-rw-r--r--   0        0        0      238 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/stores.4b841c19.js
+-rw-r--r--   0        0        0     5248 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/entry/app.2b7d5976.js
+-rw-r--r--   0        0        0    22718 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/entry/start.dc4cd066.js
+-rw-r--r--   0        0        0      703 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/0.2bbf402e.js
+-rw-r--r--   0        0        0      800 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/1.ed3af81f.js
+-rw-r--r--   0        0        0       68 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/2.375c4cd1.js
+-rw-r--r--   0        0        0      663 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/3.35180ced.js
+-rw-r--r--   0        0        0       27 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/favicon.png
+-rw-r--r--   0        0        0     1174 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/brush.svg
+-rw-r--r--   0        0        0     2789 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/eraser.svg
+-rw-r--r--   0        0        0     2828 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/poly.svg
+-rw-r--r--   0        0        0      668 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/save.svg
+-rw-r--r--   0        0        0      826 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/size.svg
+-rw-r--r--   0        0        0     2723 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/toolset.svg
+-rw-r--r--   0        0        0      318 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/trash.svg
+-rw-r--r--   0        0        0      895 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/icons/trashcan.svg
+-rw-r--r--   0        0        0     5242 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/index.html
+-rw-r--r--   0        0        0     1713 2023-05-29 13:20:25.780340 scaneo-2023.5.29.post2/scaneo/ui/kk/index.html
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 scaneo-2023.5.29.post2/setup.py
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 scaneo-2023.5.29.post2/PKG-INFO
```

### Comparing `scaneo-2023.5.29/README.md` & `scaneo-2023.5.29.post2/README.md`

 * *Files identical despite different names*

### Comparing `scaneo-2023.5.29/scaneo/api.py` & `scaneo-2023.5.29.post2/scaneo/api.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.5.29/scaneo/main.py` & `scaneo-2023.5.29.post2/scaneo/main.py`

 * *Files identical despite different names*

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/index.6dba6488.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/index.8c237fac.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,433 +1,744 @@
-function $() {}
+function b() {}
+const Z = t => t;
 
-function H(t, n) {
-    for (const e in n) t[e] = n[e];
+function wt(t, e) {
+    for (const n in e) t[n] = e[n];
     return t
 }
 
-function B(t) {
+function tt(t) {
     return t()
 }
 
-function C() {
+function V() {
     return Object.create(null)
 }
 
-function g(t) {
-    t.forEach(B)
+function v(t) {
+    t.forEach(tt)
 }
 
-function O(t) {
+function R(t) {
     return typeof t == "function"
 }
 
-function lt(t, n) {
-    return t != t ? n == n : t !== n || t && typeof t == "object" || typeof t == "function"
+function It(t, e) {
+    return t != t ? e == e : t !== e || t && typeof t == "object" || typeof t == "function"
 }
 
-function I(t) {
+function xt(t) {
     return Object.keys(t).length === 0
 }
 
-function G(t, ...n) {
-    if (t == null) return $;
-    const e = t.subscribe(...n);
-    return e.unsubscribe ? () => e.unsubscribe() : e
+function et(t, ...e) {
+    if (t == null) return b;
+    const n = t.subscribe(...e);
+    return n.unsubscribe ? () => n.unsubscribe() : n
 }
 
-function ut(t, n, e) {
-    t.$$.on_destroy.push(G(n, e))
+function Wt(t) {
+    let e;
+    return et(t, n => e = n)(), e
 }
 
-function ot(t, n, e, i) {
+function Gt(t, e, n) {
+    t.$$.on_destroy.push(et(e, n))
+}
+
+function Jt(t, e, n, i) {
     if (t) {
-        const r = P(t, n, e, i);
+        const r = nt(t, e, n, i);
         return t[0](r)
     }
 }
 
-function P(t, n, e, i) {
-    return t[1] && i ? H(e.ctx.slice(), t[1](i(n))) : e.ctx
+function nt(t, e, n, i) {
+    return t[1] && i ? wt(n.ctx.slice(), t[1](i(e))) : n.ctx
 }
 
-function st(t, n, e, i) {
+function Kt(t, e, n, i) {
     if (t[2] && i) {
-        const r = t[2](i(e));
-        if (n.dirty === void 0) return r;
+        const r = t[2](i(n));
+        if (e.dirty === void 0) return r;
         if (typeof r == "object") {
-            const s = [],
-                c = Math.max(n.dirty.length, r.length);
-            for (let o = 0; o < c; o += 1) s[o] = n.dirty[o] | r[o];
-            return s
+            const l = [],
+                s = Math.max(e.dirty.length, r.length);
+            for (let u = 0; u < s; u += 1) l[u] = e.dirty[u] | r[u];
+            return l
         }
-        return n.dirty | r
+        return e.dirty | r
     }
-    return n.dirty
+    return e.dirty
 }
 
-function ft(t, n, e, i, r, s) {
+function Qt(t, e, n, i, r, l) {
     if (r) {
-        const c = P(n, e, i, s);
-        t.p(c, r)
+        const s = nt(e, n, i, l);
+        t.p(s, r)
     }
 }
 
-function at(t) {
+function Ut(t) {
     if (t.ctx.length > 32) {
-        const n = [],
-            e = t.ctx.length / 32;
-        for (let i = 0; i < e; i++) n[i] = -1;
-        return n
+        const e = [],
+            n = t.ctx.length / 32;
+        for (let i = 0; i < n; i++) e[i] = -1;
+        return e
     }
     return -1
 }
-let w = !1;
 
-function L() {
-    w = !0
+function Vt(t, e, n) {
+    return t.set(n), e
+}
+
+function Xt(t) {
+    return t && R(t.destroy) ? t.destroy : b
+}
+const it = typeof window < "u";
+let rt = it ? () => window.performance.now() : () => Date.now(),
+    K = it ? t => requestAnimationFrame(t) : b;
+const S = new Set;
+
+function st(t) {
+    S.forEach(e => {
+        e.c(t) || (S.delete(e), e.f())
+    }), S.size !== 0 && K(st)
+}
+
+function ot(t) {
+    let e;
+    return S.size === 0 && K(st), {
+        promise: new Promise(n => {
+            S.add(e = {
+                c: t,
+                f: n
+            })
+        }),
+        abort() {
+            S.delete(e)
+        }
+    }
+}
+let H = !1;
+
+function $t() {
+    H = !0
 }
 
-function W() {
-    w = !1
+function bt() {
+    H = !1
 }
 
-function J(t, n, e, i) {
-    for (; t < n;) {
-        const r = t + (n - t >> 1);
-        e(r) <= i ? t = r + 1 : n = r
+function vt(t, e, n, i) {
+    for (; t < e;) {
+        const r = t + (e - t >> 1);
+        n(r) <= i ? t = r + 1 : e = r
     }
     return t
 }
 
-function K(t) {
+function Et(t) {
     if (t.hydrate_init) return;
     t.hydrate_init = !0;
-    let n = t.childNodes;
+    let e = t.childNodes;
     if (t.nodeName === "HEAD") {
-        const l = [];
-        for (let u = 0; u < n.length; u++) {
-            const a = n[u];
-            a.claim_order !== void 0 && l.push(a)
-        }
-        n = l
-    }
-    const e = new Int32Array(n.length + 1),
-        i = new Int32Array(n.length);
-    e[0] = -1;
+        const c = [];
+        for (let o = 0; o < e.length; o++) {
+            const f = e[o];
+            f.claim_order !== void 0 && c.push(f)
+        }
+        e = c
+    }
+    const n = new Int32Array(e.length + 1),
+        i = new Int32Array(e.length);
+    n[0] = -1;
     let r = 0;
-    for (let l = 0; l < n.length; l++) {
-        const u = n[l].claim_order,
-            a = (r > 0 && n[e[r]].claim_order <= u ? r + 1 : J(1, r, x => n[e[x]].claim_order, u)) - 1;
-        i[l] = e[a] + 1;
-        const f = a + 1;
-        e[f] = l, r = Math.max(f, r)
-    }
-    const s = [],
-        c = [];
-    let o = n.length - 1;
-    for (let l = e[r] + 1; l != 0; l = i[l - 1]) {
-        for (s.push(n[l - 1]); o >= l; o--) c.push(n[o]);
-        o--
-    }
-    for (; o >= 0; o--) c.push(n[o]);
-    s.reverse(), c.sort((l, u) => l.claim_order - u.claim_order);
-    for (let l = 0, u = 0; l < c.length; l++) {
-        for (; u < s.length && c[l].claim_order >= s[u].claim_order;) u++;
-        const a = u < s.length ? s[u] : null;
-        t.insertBefore(c[l], a)
+    for (let c = 0; c < e.length; c++) {
+        const o = e[c].claim_order,
+            f = (r > 0 && e[n[r]].claim_order <= o ? r + 1 : vt(1, r, _ => e[n[_]].claim_order, o)) - 1;
+        i[c] = n[f] + 1;
+        const a = f + 1;
+        n[a] = c, r = Math.max(a, r)
+    }
+    const l = [],
+        s = [];
+    let u = e.length - 1;
+    for (let c = n[r] + 1; c != 0; c = i[c - 1]) {
+        for (l.push(e[c - 1]); u >= c; u--) s.push(e[u]);
+        u--
+    }
+    for (; u >= 0; u--) s.push(e[u]);
+    l.reverse(), s.sort((c, o) => c.claim_order - o.claim_order);
+    for (let c = 0, o = 0; c < s.length; c++) {
+        for (; o < l.length && s[c].claim_order >= l[o].claim_order;) o++;
+        const f = o < l.length ? l[o] : null;
+        t.insertBefore(s[c], f)
     }
 }
 
-function Q(t, n) {
-    if (w) {
-        for (K(t), (t.actual_end_child === void 0 || t.actual_end_child !== null && t.actual_end_child.parentNode !== t) && (t.actual_end_child = t.firstChild); t.actual_end_child !== null && t.actual_end_child.claim_order === void 0;) t.actual_end_child = t.actual_end_child.nextSibling;
-        n !== t.actual_end_child ? (n.claim_order !== void 0 || n.parentNode !== t) && t.insertBefore(n, t.actual_end_child) : t.actual_end_child = n.nextSibling
-    } else(n.parentNode !== t || n.nextSibling !== null) && t.appendChild(n)
+function kt(t, e) {
+    t.appendChild(e)
 }
 
-function dt(t, n, e) {
-    w && !e ? Q(t, n) : (n.parentNode !== t || n.nextSibling != e) && t.insertBefore(n, e || null)
+function ct(t) {
+    if (!t) return document;
+    const e = t.getRootNode ? t.getRootNode() : t.ownerDocument;
+    return e && e.host ? e : t.ownerDocument
 }
 
-function R(t) {
+function Nt(t) {
+    const e = ut("style");
+    return St(ct(t), e), e.sheet
+}
+
+function St(t, e) {
+    return kt(t.head || t, e), e.sheet
+}
+
+function Ct(t, e) {
+    if (H) {
+        for (Et(t), (t.actual_end_child === void 0 || t.actual_end_child !== null && t.actual_end_child.parentNode !== t) && (t.actual_end_child = t.firstChild); t.actual_end_child !== null && t.actual_end_child.claim_order === void 0;) t.actual_end_child = t.actual_end_child.nextSibling;
+        e !== t.actual_end_child ? (e.claim_order !== void 0 || e.parentNode !== t) && t.insertBefore(e, t.actual_end_child) : t.actual_end_child = e.nextSibling
+    } else(e.parentNode !== t || e.nextSibling !== null) && t.appendChild(e)
+}
+
+function Yt(t, e, n) {
+    H && !n ? Ct(t, e) : (e.parentNode !== t || e.nextSibling != n) && t.insertBefore(e, n || null)
+}
+
+function lt(t) {
     t.parentNode && t.parentNode.removeChild(t)
 }
 
-function U(t) {
+function Zt(t, e) {
+    for (let n = 0; n < t.length; n += 1) t[n] && t[n].d(e)
+}
+
+function ut(t) {
     return document.createElement(t)
 }
 
-function A(t) {
+function At(t) {
+    return document.createElementNS("http://www.w3.org/2000/svg", t)
+}
+
+function Q(t) {
     return document.createTextNode(t)
 }
 
-function _t() {
-    return A(" ")
+function te() {
+    return Q(" ")
 }
 
-function ht() {
-    return A("")
+function ee() {
+    return Q("")
+}
+
+function ne(t, e, n, i) {
+    return t.addEventListener(e, n, i), () => t.removeEventListener(e, n, i)
 }
 
-function mt(t, n, e) {
-    e == null ? t.removeAttribute(n) : t.getAttribute(n) !== e && t.setAttribute(n, e)
+function ie(t) {
+    return function(e) {
+        return e.stopPropagation(), t.call(this, e)
+    }
+}
+
+function re(t, e, n) {
+    n == null ? t.removeAttribute(e) : t.getAttribute(e) !== n && t.setAttribute(e, n)
 }
 
-function V(t) {
+function Mt(t) {
     return Array.from(t.childNodes)
 }
 
-function X(t) {
+function jt(t) {
     t.claim_info === void 0 && (t.claim_info = {
         last_index: 0,
         total_claimed: 0
     })
 }
 
-function T(t, n, e, i, r = !1) {
-    X(t);
-    const s = (() => {
-        for (let c = t.claim_info.last_index; c < t.length; c++) {
-            const o = t[c];
-            if (n(o)) {
-                const l = e(o);
-                return l === void 0 ? t.splice(c, 1) : t[c] = l, r || (t.claim_info.last_index = c), o
+function at(t, e, n, i, r = !1) {
+    jt(t);
+    const l = (() => {
+        for (let s = t.claim_info.last_index; s < t.length; s++) {
+            const u = t[s];
+            if (e(u)) {
+                const c = n(u);
+                return c === void 0 ? t.splice(s, 1) : t[s] = c, r || (t.claim_info.last_index = s), u
             }
         }
-        for (let c = t.claim_info.last_index - 1; c >= 0; c--) {
-            const o = t[c];
-            if (n(o)) {
-                const l = e(o);
-                return l === void 0 ? t.splice(c, 1) : t[c] = l, r ? l === void 0 && t.claim_info.last_index-- : t.claim_info.last_index = c, o
+        for (let s = t.claim_info.last_index - 1; s >= 0; s--) {
+            const u = t[s];
+            if (e(u)) {
+                const c = n(u);
+                return c === void 0 ? t.splice(s, 1) : t[s] = c, r ? c === void 0 && t.claim_info.last_index-- : t.claim_info.last_index = s, u
             }
         }
         return i()
     })();
-    return s.claim_order = t.claim_info.total_claimed, t.claim_info.total_claimed += 1, s
+    return l.claim_order = t.claim_info.total_claimed, t.claim_info.total_claimed += 1, l
 }
 
-function Y(t, n, e, i) {
-    return T(t, r => r.nodeName === n, r => {
-        const s = [];
-        for (let c = 0; c < r.attributes.length; c++) {
-            const o = r.attributes[c];
-            e[o.name] || s.push(o.name)
+function ft(t, e, n, i) {
+    return at(t, r => r.nodeName === e, r => {
+        const l = [];
+        for (let s = 0; s < r.attributes.length; s++) {
+            const u = r.attributes[s];
+            n[u.name] || l.push(u.name)
         }
-        s.forEach(c => r.removeAttribute(c))
-    }, () => i(n))
+        l.forEach(s => r.removeAttribute(s))
+    }, () => i(e))
+}
+
+function se(t, e, n) {
+    return ft(t, e, n, ut)
+}
+
+function oe(t, e, n) {
+    return ft(t, e, n, At)
+}
+
+function Ot(t, e) {
+    return at(t, n => n.nodeType === 3, n => {
+        const i = "" + e;
+        if (n.data.startsWith(i)) {
+            if (n.data.length !== i.length) return n.splitText(i.length)
+        } else n.data = i
+    }, () => Q(e), !0)
+}
+
+function ce(t) {
+    return Ot(t, " ")
+}
+
+function le(t, e) {
+    e = "" + e, t.data !== e && (t.data = e)
+}
+
+function ue(t, e) {
+    t.value = e ?? ""
+}
+
+function ae(t, e, n, i) {
+    n == null ? t.style.removeProperty(e) : t.style.setProperty(e, n, i ? "important" : "")
+}
+
+function Pt(t, e, {
+    bubbles: n = !1,
+    cancelable: i = !1
+} = {}) {
+    const r = document.createEvent("CustomEvent");
+    return r.initCustomEvent(t, n, i, e), r
+}
+
+function fe(t, e) {
+    return new t(e)
 }
+const T = new Map;
+let q = 0;
 
-function pt(t, n, e) {
-    return Y(t, n, e, U)
+function Dt(t) {
+    let e = 5381,
+        n = t.length;
+    for (; n--;) e = (e << 5) - e ^ t.charCodeAt(n);
+    return e >>> 0
 }
 
-function Z(t, n) {
-    return T(t, e => e.nodeType === 3, e => {
-        const i = "" + n;
-        if (e.data.startsWith(i)) {
-            if (e.data.length !== i.length) return e.splitText(i.length)
-        } else e.data = i
-    }, () => A(n), !0)
+function Rt(t, e) {
+    const n = {
+        stylesheet: Nt(e),
+        rules: {}
+    };
+    return T.set(t, n), n
 }
 
-function yt(t) {
-    return Z(t, " ")
+function _t(t, e, n, i, r, l, s, u = 0) {
+    const c = 16.666 / i;
+    let o = `{
+`;
+    for (let p = 0; p <= 1; p += c) {
+        const y = e + (n - e) * l(p);
+        o += p * 100 + `%{${s(y,1-y)}}
+`
+    }
+    const f = o + `100% {${s(n,1-n)}}
+}`,
+        a = `__svelte_${Dt(f)}_${u}`,
+        _ = ct(t),
+        {
+            stylesheet: h,
+            rules: d
+        } = T.get(_) || Rt(_, t);
+    d[a] || (d[a] = !0, h.insertRule(`@keyframes ${a} ${f}`, h.cssRules.length));
+    const g = t.style.animation || "";
+    return t.style.animation = `${g?`${g}, `:""}${a} ${i}ms linear ${r}ms 1 both`, q += 1, a
+}
+
+function G(t, e) {
+    const n = (t.style.animation || "").split(", "),
+        i = n.filter(e ? l => l.indexOf(e) < 0 : l => l.indexOf("__svelte") === -1),
+        r = n.length - i.length;
+    r && (t.style.animation = i.join(", "), q -= r, q || zt())
+}
+
+function zt() {
+    K(() => {
+        q || (T.forEach(t => {
+            const {
+                ownerNode: e
+            } = t.stylesheet;
+            e && lt(e)
+        }), T.clear())
+    })
 }
+let P;
 
-function gt(t, n) {
-    n = "" + n, t.data !== n && (t.data = n)
+function O(t) {
+    P = t
 }
 
-function xt(t, n, e, i) {
-    e == null ? t.style.removeProperty(n) : t.style.setProperty(n, e, i ? "important" : "")
+function z() {
+    if (!P) throw new Error("Function called outside component initialization");
+    return P
 }
 
-function bt(t, n) {
-    return new t(n)
+function _e(t) {
+    z().$$.on_mount.push(t)
 }
-let y;
 
-function p(t) {
-    y = t
+function de(t) {
+    z().$$.after_update.push(t)
 }
 
-function q() {
-    if (!y) throw new Error("Function called outside component initialization");
-    return y
+function he(t) {
+    z().$$.on_destroy.push(t)
 }
 
-function $t(t) {
-    q().$$.on_mount.push(t)
+function me(t, e) {
+    return z().$$.context.set(t, e), e
 }
 
-function wt(t) {
-    q().$$.after_update.push(t)
+function pe(t) {
+    return z().$$.context.get(t)
 }
-const h = [],
-    k = [];
-let m = [];
-const M = [],
-    z = Promise.resolve();
-let v = !1;
+const N = [],
+    X = [];
+let C = [];
+const Y = [],
+    dt = Promise.resolve();
+let J = !1;
 
-function D() {
-    v || (v = !0, z.then(F))
+function ht() {
+    J || (J = !0, dt.then(mt))
 }
 
-function Et() {
-    return D(), z
+function ye() {
+    return ht(), dt
 }
 
-function N(t) {
-    m.push(t)
+function D(t) {
+    C.push(t)
 }
-const E = new Set;
-let _ = 0;
+const W = new Set;
+let k = 0;
 
-function F() {
-    if (_ !== 0) return;
-    const t = y;
+function mt() {
+    if (k !== 0) return;
+    const t = P;
     do {
         try {
-            for (; _ < h.length;) {
-                const n = h[_];
-                _++, p(n), tt(n.$$)
+            for (; k < N.length;) {
+                const e = N[k];
+                k++, O(e), Bt(e.$$)
             }
-        } catch (n) {
-            throw h.length = 0, _ = 0, n
+        } catch (e) {
+            throw N.length = 0, k = 0, e
+        }
+        for (O(null), N.length = 0, k = 0; X.length;) X.pop()();
+        for (let e = 0; e < C.length; e += 1) {
+            const n = C[e];
+            W.has(n) || (W.add(n), n())
         }
-        for (p(null), h.length = 0, _ = 0; k.length;) k.pop()();
-        for (let n = 0; n < m.length; n += 1) {
-            const e = m[n];
-            E.has(e) || (E.add(e), e())
-        }
-        m.length = 0
-    } while (h.length);
-    for (; M.length;) M.pop()();
-    v = !1, E.clear(), p(t)
+        C.length = 0
+    } while (N.length);
+    for (; Y.length;) Y.pop()();
+    J = !1, W.clear(), O(t)
 }
 
-function tt(t) {
+function Bt(t) {
     if (t.fragment !== null) {
-        t.update(), g(t.before_update);
-        const n = t.dirty;
-        t.dirty = [-1], t.fragment && t.fragment.p(t.ctx, n), t.after_update.forEach(N)
+        t.update(), v(t.before_update);
+        const e = t.dirty;
+        t.dirty = [-1], t.fragment && t.fragment.p(t.ctx, e), t.after_update.forEach(D)
     }
 }
 
-function nt(t) {
-    const n = [],
-        e = [];
-    m.forEach(i => t.indexOf(i) === -1 ? n.push(i) : e.push(i)), e.forEach(i => i()), m = n
+function Lt(t) {
+    const e = [],
+        n = [];
+    C.forEach(i => t.indexOf(i) === -1 ? e.push(i) : n.push(i)), n.forEach(i => i()), C = e
 }
-const b = new Set;
-let d;
+let j;
 
-function vt() {
-    d = {
+function pt() {
+    return j || (j = Promise.resolve(), j.then(() => {
+        j = null
+    })), j
+}
+
+function F(t, e, n) {
+    t.dispatchEvent(Pt(`${e?"intro":"outro"}${n}`))
+}
+const L = new Set;
+let $;
+
+function ge() {
+    $ = {
         r: 0,
         c: [],
-        p: d
+        p: $
     }
 }
 
-function Nt() {
-    d.r || g(d.c), d = d.p
+function we() {
+    $.r || v($.c), $ = $.p
 }
 
-function et(t, n) {
-    t && t.i && (b.delete(t), t.i(n))
+function yt(t, e) {
+    t && t.i && (L.delete(t), t.i(e))
 }
 
-function At(t, n, e, i) {
+function Tt(t, e, n, i) {
     if (t && t.o) {
-        if (b.has(t)) return;
-        b.add(t), d.c.push(() => {
-            b.delete(t), i && (e && t.d(1), i())
-        }), t.o(n)
+        if (L.has(t)) return;
+        L.add(t), $.c.push(() => {
+            L.delete(t), i && (n && t.d(1), i())
+        }), t.o(e)
     } else i && i()
 }
+const gt = {
+    duration: 0
+};
+
+function xe(t, e, n) {
+    const i = {
+        direction: "in"
+    };
+    let r = e(t, n, i),
+        l = !1,
+        s, u, c = 0;
+
+    function o() {
+        s && G(t, s)
+    }
+
+    function f() {
+        const {
+            delay: _ = 0,
+            duration: h = 300,
+            easing: d = Z,
+            tick: g = b,
+            css: p
+        } = r || gt;
+        p && (s = _t(t, 0, 1, h, _, d, p, c++)), g(0, 1);
+        const y = rt() + _,
+            A = y + h;
+        u && u.abort(), l = !0, D(() => F(t, !0, "start")), u = ot(E => {
+            if (l) {
+                if (E >= A) return g(1, 0), F(t, !0, "end"), o(), l = !1;
+                if (E >= y) {
+                    const M = d((E - y) / h);
+                    g(M, 1 - M)
+                }
+            }
+            return l
+        })
+    }
+    let a = !1;
+    return {
+        start() {
+            a || (a = !0, G(t), R(r) ? (r = r(i), pt().then(f)) : f())
+        },
+        invalidate() {
+            a = !1
+        },
+        end() {
+            l && (o(), l = !1)
+        }
+    }
+}
+
+function $e(t, e, n) {
+    const i = {
+        direction: "out"
+    };
+    let r = e(t, n, i),
+        l = !0,
+        s;
+    const u = $;
+    u.r += 1;
+
+    function c() {
+        const {
+            delay: o = 0,
+            duration: f = 300,
+            easing: a = Z,
+            tick: _ = b,
+            css: h
+        } = r || gt;
+        h && (s = _t(t, 1, 0, f, o, a, h));
+        const d = rt() + o,
+            g = d + f;
+        D(() => F(t, !1, "start")), ot(p => {
+            if (l) {
+                if (p >= g) return _(0, 1), F(t, !1, "end"), --u.r || v(u.c), !1;
+                if (p >= d) {
+                    const y = a((p - d) / f);
+                    _(1 - y, y)
+                }
+            }
+            return l
+        })
+    }
+    return R(r) ? pt().then(() => {
+        r = r(i), c()
+    }) : c(), {
+        end(o) {
+            o && r.tick && r.tick(1, 0), l && (s && G(t, s), l = !1)
+        }
+    }
+}
+
+function be(t, e) {
+    t.d(1), e.delete(t.key)
+}
 
-function St(t) {
+function ve(t, e) {
+    Tt(t, 1, 1, () => {
+        e.delete(t.key)
+    })
+}
+
+function Ee(t, e, n, i, r, l, s, u, c, o, f, a) {
+    let _ = t.length,
+        h = l.length,
+        d = _;
+    const g = {};
+    for (; d--;) g[t[d].key] = d;
+    const p = [],
+        y = new Map,
+        A = new Map,
+        E = [];
+    for (d = h; d--;) {
+        const m = a(r, l, d),
+            w = n(m);
+        let x = s.get(w);
+        x ? i && E.push(() => x.p(m, e)) : (x = o(w, m), x.c()), y.set(w, p[d] = x), w in g && A.set(w, Math.abs(d - g[w]))
+    }
+    const M = new Set,
+        U = new Set;
+
+    function I(m) {
+        yt(m, 1), m.m(u, f), s.set(m.key, m), f = m.first, h--
+    }
+    for (; _ && h;) {
+        const m = p[h - 1],
+            w = t[_ - 1],
+            x = m.key,
+            B = w.key;
+        m === w ? (f = m.first, _--, h--) : y.has(B) ? !s.has(x) || M.has(x) ? I(m) : U.has(B) ? _-- : A.get(x) > A.get(B) ? (U.add(x), I(m)) : (M.add(B), _--) : (c(w, s), _--)
+    }
+    for (; _--;) {
+        const m = t[_];
+        y.has(m.key) || c(m, s)
+    }
+    for (; h;) I(p[h - 1]);
+    return v(E), p
+}
+
+function ke(t) {
     t && t.c()
 }
 
-function jt(t, n) {
-    t && t.l(n)
+function Ne(t, e) {
+    t && t.l(e)
 }
 
-function it(t, n, e, i) {
+function qt(t, e, n, i) {
     const {
         fragment: r,
-        after_update: s
+        after_update: l
     } = t.$$;
-    r && r.m(n, e), i || N(() => {
-        const c = t.$$.on_mount.map(B).filter(O);
-        t.$$.on_destroy ? t.$$.on_destroy.push(...c) : g(c), t.$$.on_mount = []
-    }), s.forEach(N)
+    r && r.m(e, n), i || D(() => {
+        const s = t.$$.on_mount.map(tt).filter(R);
+        t.$$.on_destroy ? t.$$.on_destroy.push(...s) : v(s), t.$$.on_mount = []
+    }), l.forEach(D)
 }
 
-function rt(t, n) {
-    const e = t.$$;
-    e.fragment !== null && (nt(e.after_update), g(e.on_destroy), e.fragment && e.fragment.d(n), e.on_destroy = e.fragment = null, e.ctx = [])
+function Ft(t, e) {
+    const n = t.$$;
+    n.fragment !== null && (Lt(n.after_update), v(n.on_destroy), n.fragment && n.fragment.d(e), n.on_destroy = n.fragment = null, n.ctx = [])
 }
 
-function ct(t, n) {
-    t.$$.dirty[0] === -1 && (h.push(t), D(), t.$$.dirty.fill(0)), t.$$.dirty[n / 31 | 0] |= 1 << n % 31
+function Ht(t, e) {
+    t.$$.dirty[0] === -1 && (N.push(t), ht(), t.$$.dirty.fill(0)), t.$$.dirty[e / 31 | 0] |= 1 << e % 31
 }
 
-function Ct(t, n, e, i, r, s, c, o = [-1]) {
-    const l = y;
-    p(t);
-    const u = t.$$ = {
+function Se(t, e, n, i, r, l, s, u = [-1]) {
+    const c = P;
+    O(t);
+    const o = t.$$ = {
         fragment: null,
         ctx: [],
-        props: s,
-        update: $,
+        props: l,
+        update: b,
         not_equal: r,
-        bound: C(),
+        bound: V(),
         on_mount: [],
         on_destroy: [],
         on_disconnect: [],
         before_update: [],
         after_update: [],
-        context: new Map(n.context || (l ? l.$$.context : [])),
-        callbacks: C(),
-        dirty: o,
+        context: new Map(e.context || (c ? c.$$.context : [])),
+        callbacks: V(),
+        dirty: u,
         skip_bound: !1,
-        root: n.target || l.$$.root
+        root: e.target || c.$$.root
     };
-    c && c(u.root);
-    let a = !1;
-    if (u.ctx = e ? e(t, n.props || {}, (f, x, ...S) => {
-            const j = S.length ? S[0] : x;
-            return u.ctx && r(u.ctx[f], u.ctx[f] = j) && (!u.skip_bound && u.bound[f] && u.bound[f](j), a && ct(t, f)), x
-        }) : [], u.update(), a = !0, g(u.before_update), u.fragment = i ? i(u.ctx) : !1, n.target) {
-        if (n.hydrate) {
-            L();
-            const f = V(n.target);
-            u.fragment && u.fragment.l(f), f.forEach(R)
-        } else u.fragment && u.fragment.c();
-        n.intro && et(t.$$.fragment), it(t, n.target, n.anchor, n.customElement), W(), F()
+    s && s(o.root);
+    let f = !1;
+    if (o.ctx = n ? n(t, e.props || {}, (a, _, ...h) => {
+            const d = h.length ? h[0] : _;
+            return o.ctx && r(o.ctx[a], o.ctx[a] = d) && (!o.skip_bound && o.bound[a] && o.bound[a](d), f && Ht(t, a)), _
+        }) : [], o.update(), f = !0, v(o.before_update), o.fragment = i ? i(o.ctx) : !1, e.target) {
+        if (e.hydrate) {
+            $t();
+            const a = Mt(e.target);
+            o.fragment && o.fragment.l(a), a.forEach(lt)
+        } else o.fragment && o.fragment.c();
+        e.intro && yt(t.$$.fragment), qt(t, e.target, e.anchor, e.customElement), bt(), mt()
     }
-    p(l)
+    O(c)
 }
-class kt {
+class Ce {
     $destroy() {
-        rt(this, 1), this.$destroy = $
+        Ft(this, 1), this.$destroy = b
     }
-    $on(n, e) {
-        if (!O(e)) return $;
-        const i = this.$$.callbacks[n] || (this.$$.callbacks[n] = []);
-        return i.push(e), () => {
-            const r = i.indexOf(e);
+    $on(e, n) {
+        if (!R(n)) return b;
+        const i = this.$$.callbacks[e] || (this.$$.callbacks[e] = []);
+        return i.push(n), () => {
+            const r = i.indexOf(n);
             r !== -1 && i.splice(r, 1)
         }
     }
-    $set(n) {
-        this.$$set && !I(n) && (this.$$.skip_bound = !0, this.$$set(n), this.$$.skip_bound = !1)
+    $set(e) {
+        this.$$set && !xt(e) && (this.$$.skip_bound = !0, this.$$set(e), this.$$.skip_bound = !1)
     }
 }
 export {
-    it as A, rt as B, ot as C, ft as D, at as E, st as F, Q as G, $ as H, ut as I, kt as S, _t as a, dt as b, yt as c, At as d, ht as e, Nt as f, et as g, R as h, Ct as i, wt as j, U as k, pt as l, V as m, mt as n, $t as o, xt as p, A as q, Z as r, lt as s, Et as t, gt as u, vt as v, k as w, bt as x, St as y, jt as z
+    xe as $, qt as A, Ft as B, Jt as C, Qt as D, Ut as E, Kt as F, Ct as G, b as H, Gt as I, he as J, me as K, pe as L, Wt as M, At as N, oe as O, Ee as P, ne as Q, be as R, Ce as S, Vt as T, ve as U, ie as V, ue as W, Xt as X, R as Y, v as Z, D as _, te as a, $e as a0, Zt as a1, Yt as b, ce as c, Tt as d, ee as e, we as f, yt as g, lt as h, Se as i, de as j, ut as k, se as l, Mt as m, re as n, _e as o, ae as p, Q as q, Ot as r, It as s, ye as t, le as u, ge as v, X as w, fe as x, ke as y, Ne as z
 };
```

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/chunks/singletons.9f3ec903.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/chunks/singletons.d791afcf.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,193 +1,198 @@
 import {
     H as d,
-    s as m
-} from "./index.6dba6488.js";
+    s as E
+} from "./index.8c237fac.js";
 const u = [];
 
 function p(e, t = d) {
     let n;
     const o = new Set;
 
-    function r(s) {
-        if (m(e, s) && (e = s, n)) {
+    function l(s) {
+        if (E(e, s) && (e = s, n)) {
             const c = !u.length;
             for (const i of o) i[1](), u.push(i, e);
             if (c) {
                 for (let i = 0; i < u.length; i += 2) u[i][0](u[i + 1]);
                 u.length = 0
             }
         }
     }
 
     function a(s) {
-        r(s(e))
+        l(s(e))
     }
 
-    function l(s, c = d) {
+    function r(s, c = d) {
         const i = [s, c];
-        return o.add(i), o.size === 1 && (n = t(r) || d), s(e), () => {
+        return o.add(i), o.size === 1 && (n = t(l) || d), s(e), () => {
             o.delete(i), o.size === 0 && n && (n(), n = null)
         }
     }
     return {
-        set: r,
+        set: l,
         update: a,
-        subscribe: l
+        subscribe: r
     }
 }
 var g;
-const E = ((g = globalThis.__sveltekit_1704jlc) == null ? void 0 : g.base) ?? "";
+const w = ((g = globalThis.__sveltekit_1norjlf) == null ? void 0 : g.base) ?? "";
 var k;
-const A = ((k = globalThis.__sveltekit_1704jlc) == null ? void 0 : k.assets) ?? E,
-    R = "1685364387525",
-    y = "sveltekit:snapshot",
-    I = "sveltekit:scroll",
-    x = "sveltekit:index",
+const A = ((k = globalThis.__sveltekit_1norjlf) == null ? void 0 : k.assets) ?? w,
+    R = "1685366422380",
+    I = "sveltekit:snapshot",
+    x = "sveltekit:scroll",
+    O = "sveltekit:index",
     _ = {
         tap: 1,
         hover: 2,
         viewport: 3,
         eager: 4,
         off: -1
     };
 
-function O(e) {
+function U(e) {
     let t = e.baseURI;
     if (!t) {
         const n = e.getElementsByTagName("base");
         t = n.length ? n[0].href : e.URL
     }
     return t
 }
 
-function U() {
+function j() {
     return {
         x: pageXOffset,
         y: pageYOffset
     }
 }
 
 function f(e, t) {
     return e.getAttribute(`data-sveltekit-${t}`)
 }
 const b = {
     ..._,
     "": _.hover
 };
 
-function v(e) {
+function m(e) {
     let t = e.assignedSlot ?? e.parentNode;
     return (t == null ? void 0 : t.nodeType) === 11 && (t = t.host), t
 }
 
 function L(e, t) {
     for (; e && e !== t;) {
         if (e.nodeName.toUpperCase() === "A" && e.hasAttribute("href")) return e;
-        e = v(e)
+        e = m(e)
     }
 }
 
 function N(e, t) {
     let n;
     try {
         n = new URL(e instanceof SVGAElement ? e.href.baseVal : e.href, document.baseURI)
     } catch {}
     const o = e instanceof SVGAElement ? e.target.baseVal : e.target,
-        r = !n || !!o || T(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
+        l = !n || !!o || T(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
         a = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
     return {
         url: n,
-        external: r,
+        external: l,
         target: o,
         download: a
     }
 }
 
-function j(e) {
+function P(e) {
     let t = null,
         n = null,
         o = null,
-        r = null,
-        a = null,
         l = null,
+        a = null,
+        r = null,
         s = e;
-    for (; s && s !== document.documentElement;) o === null && (o = f(s, "preload-code")), r === null && (r = f(s, "preload-data")), t === null && (t = f(s, "keepfocus")), n === null && (n = f(s, "noscroll")), a === null && (a = f(s, "reload")), l === null && (l = f(s, "replacestate")), s = v(s);
+    for (; s && s !== document.documentElement;) o === null && (o = f(s, "preload-code")), l === null && (l = f(s, "preload-data")), t === null && (t = f(s, "keepfocus")), n === null && (n = f(s, "noscroll")), a === null && (a = f(s, "reload")), r === null && (r = f(s, "replacestate")), s = m(s);
     return {
         preload_code: b[o ?? "off"],
-        preload_data: b[r ?? "off"],
+        preload_data: b[l ?? "off"],
         keep_focus: t === "off" ? !1 : t === "" ? !0 : null,
         noscroll: n === "off" ? !1 : n === "" ? !0 : null,
         reload: a === "off" ? !1 : a === "" ? !0 : null,
-        replace_state: l === "off" ? !1 : l === "" ? !0 : null
+        replace_state: r === "off" ? !1 : r === "" ? !0 : null
     }
 }
 
 function h(e) {
     const t = p(e);
     let n = !0;
 
     function o() {
-        n = !0, t.update(l => l)
+        n = !0, t.update(r => r)
     }
 
-    function r(l) {
-        n = !1, t.set(l)
+    function l(r) {
+        n = !1, t.set(r)
     }
 
-    function a(l) {
+    function a(r) {
         let s;
         return t.subscribe(c => {
-            (s === void 0 || n && c !== s) && l(s = c)
+            (s === void 0 || n && c !== s) && r(s = c)
         })
     }
     return {
         notify: o,
-        set: r,
+        set: l,
         subscribe: a
     }
 }
 
 function S() {
     const {
         set: e,
         subscribe: t
     } = p(!1);
     let n;
     async function o() {
         clearTimeout(n);
         try {
-            const r = await fetch(`${A}/_app/version.json`, {
+            const l = await fetch(`${A}/_app/version.json`, {
                 headers: {
                     pragma: "no-cache",
                     "cache-control": "no-cache"
                 }
             });
-            if (!r.ok) return !1;
-            const l = (await r.json()).version !== R;
-            return l && (e(!0), clearTimeout(n)), l
+            if (!l.ok) return !1;
+            const r = (await l.json()).version !== R;
+            return r && (e(!0), clearTimeout(n)), r
         } catch {
             return !1
         }
     }
     return {
         subscribe: t,
         check: o
     }
 }
 
 function T(e, t) {
     return e.origin !== location.origin || !e.pathname.startsWith(t)
 }
+let v;
 
-function P(e) {
-    e.client
+function V(e) {
+    v = e.client
+}
+
+function Y(e) {
+    return (...t) => v[e](...t)
 }
-const V = {
+const q = {
     url: h({}),
     page: h({}),
     navigating: p(null),
     updated: S()
 };
 export {
-    x as I, _ as P, I as S, y as a, N as b, j as c, U as d, E as e, L as f, O as g, P as h, T as i, V as s
+    O as I, _ as P, x as S, I as a, N as b, P as c, j as d, w as e, L as f, U as g, V as h, T as i, Y as j, q as s, p as w
 };
```

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/app.b9b6597a.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/entry/app.2b7d5976.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,374 +1,353 @@
 import {
-    S as C,
-    i as q,
-    s as U,
-    a as j,
-    e as h,
-    c as z,
+    _ as D
+} from "../chunks/preload-helper.41c905a7.js";
+import {
+    S,
+    i as j,
+    s as z,
+    a as B,
+    e as p,
+    c as C,
     b as w,
-    d as p,
-    f as L,
+    d as h,
+    f as I,
     g as d,
     h as g,
-    j as W,
-    o as F,
-    k as G,
-    l as H,
-    m as J,
-    n as N,
+    j as M,
+    o as U,
+    k as F,
+    l as G,
+    m as H,
+    n as P,
     p as m,
-    q as K,
-    r as M,
+    q as J,
+    r as K,
     u as Q,
-    v as P,
-    w as S,
-    x as b,
+    v as N,
+    w as R,
+    x as k,
     y as v,
-    z as A,
+    z as V,
     A as E,
-    B as R
-} from "../chunks/index.6dba6488.js";
-const X = "modulepreload",
-    Y = function(a, e) {
-        return new URL(a, e).href
-    },
-    D = {},
-    y = function(e, n, i) {
-        if (!n || n.length === 0) return e();
-        const s = document.getElementsByTagName("link");
-        return Promise.all(n.map(f => {
-            if (f = Y(f, i), f in D) return;
-            D[f] = !0;
-            const t = f.endsWith(".css"),
-                r = t ? '[rel="stylesheet"]' : "";
-            if (!!i)
-                for (let l = s.length - 1; l >= 0; l--) {
-                    const u = s[l];
-                    if (u.href === f && (!t || u.rel === "stylesheet")) return
-                } else if (document.querySelector(`link[href="${f}"]${r}`)) return;
-            const o = document.createElement("link");
-            if (o.rel = t ? "stylesheet" : X, t || (o.as = "script", o.crossOrigin = ""), o.href = f, document.head.appendChild(o), t) return new Promise((l, u) => {
-                o.addEventListener("load", l), o.addEventListener("error", () => u(new Error(`Unable to preload CSS for ${f}`)))
-            })
-        })).then(() => e())
-    },
-    ie = {};
+    B as A
+} from "../chunks/index.8c237fac.js";
+const te = {};
 
-function Z(a) {
+function W(r) {
     let e, n, i;
-    var s = a[1][0];
+    var s = r[1][0];
 
-    function f(t) {
+    function _(t) {
         return {
             props: {
                 data: t[3],
                 form: t[2]
             }
         }
     }
-    return s && (e = b(s, f(a)), a[12](e)), {
+    return s && (e = k(s, _(r)), r[12](e)), {
         c() {
-            e && v(e.$$.fragment), n = h()
+            e && v(e.$$.fragment), n = p()
         },
         l(t) {
-            e && A(e.$$.fragment, t), n = h()
+            e && V(e.$$.fragment, t), n = p()
         },
-        m(t, r) {
-            e && E(e, t, r), w(t, n, r), i = !0
+        m(t, o) {
+            e && E(e, t, o), w(t, n, o), i = !0
         },
-        p(t, r) {
-            const _ = {};
-            if (r & 8 && (_.data = t[3]), r & 4 && (_.form = t[2]), r & 2 && s !== (s = t[1][0])) {
+        p(t, o) {
+            const c = {};
+            if (o & 8 && (c.data = t[3]), o & 4 && (c.form = t[2]), o & 2 && s !== (s = t[1][0])) {
                 if (e) {
-                    P();
-                    const o = e;
-                    p(o.$$.fragment, 1, 0, () => {
-                        R(o, 1)
-                    }), L()
+                    N();
+                    const f = e;
+                    h(f.$$.fragment, 1, 0, () => {
+                        A(f, 1)
+                    }), I()
                 }
-                s ? (e = b(s, f(t)), t[12](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
-            } else s && e.$set(_)
+                s ? (e = k(s, _(t)), t[12](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
+            } else s && e.$set(c)
         },
         i(t) {
             i || (e && d(e.$$.fragment, t), i = !0)
         },
         o(t) {
-            e && p(e.$$.fragment, t), i = !1
+            e && h(e.$$.fragment, t), i = !1
         },
         d(t) {
-            a[12](null), t && g(n), e && R(e, t)
+            r[12](null), t && g(n), e && A(e, t)
         }
     }
 }
 
-function $(a) {
+function X(r) {
     let e, n, i;
-    var s = a[1][0];
+    var s = r[1][0];
 
-    function f(t) {
+    function _(t) {
         return {
             props: {
                 data: t[3],
                 $$slots: {
-                    default: [x]
+                    default: [Y]
                 },
                 $$scope: {
                     ctx: t
                 }
             }
         }
     }
-    return s && (e = b(s, f(a)), a[11](e)), {
+    return s && (e = k(s, _(r)), r[11](e)), {
         c() {
-            e && v(e.$$.fragment), n = h()
+            e && v(e.$$.fragment), n = p()
         },
         l(t) {
-            e && A(e.$$.fragment, t), n = h()
+            e && V(e.$$.fragment, t), n = p()
         },
-        m(t, r) {
-            e && E(e, t, r), w(t, n, r), i = !0
+        m(t, o) {
+            e && E(e, t, o), w(t, n, o), i = !0
         },
-        p(t, r) {
-            const _ = {};
-            if (r & 8 && (_.data = t[3]), r & 8215 && (_.$$scope = {
-                    dirty: r,
+        p(t, o) {
+            const c = {};
+            if (o & 8 && (c.data = t[3]), o & 8215 && (c.$$scope = {
+                    dirty: o,
                     ctx: t
-                }), r & 2 && s !== (s = t[1][0])) {
+                }), o & 2 && s !== (s = t[1][0])) {
                 if (e) {
-                    P();
-                    const o = e;
-                    p(o.$$.fragment, 1, 0, () => {
-                        R(o, 1)
-                    }), L()
+                    N();
+                    const f = e;
+                    h(f.$$.fragment, 1, 0, () => {
+                        A(f, 1)
+                    }), I()
                 }
-                s ? (e = b(s, f(t)), t[11](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
-            } else s && e.$set(_)
+                s ? (e = k(s, _(t)), t[11](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
+            } else s && e.$set(c)
         },
         i(t) {
             i || (e && d(e.$$.fragment, t), i = !0)
         },
         o(t) {
-            e && p(e.$$.fragment, t), i = !1
+            e && h(e.$$.fragment, t), i = !1
         },
         d(t) {
-            a[11](null), t && g(n), e && R(e, t)
+            r[11](null), t && g(n), e && A(e, t)
         }
     }
 }
 
-function x(a) {
+function Y(r) {
     let e, n, i;
-    var s = a[1][1];
+    var s = r[1][1];
 
-    function f(t) {
+    function _(t) {
         return {
             props: {
                 data: t[4],
                 form: t[2]
             }
         }
     }
-    return s && (e = b(s, f(a)), a[10](e)), {
+    return s && (e = k(s, _(r)), r[10](e)), {
         c() {
-            e && v(e.$$.fragment), n = h()
+            e && v(e.$$.fragment), n = p()
         },
         l(t) {
-            e && A(e.$$.fragment, t), n = h()
+            e && V(e.$$.fragment, t), n = p()
         },
-        m(t, r) {
-            e && E(e, t, r), w(t, n, r), i = !0
+        m(t, o) {
+            e && E(e, t, o), w(t, n, o), i = !0
         },
-        p(t, r) {
-            const _ = {};
-            if (r & 16 && (_.data = t[4]), r & 4 && (_.form = t[2]), r & 2 && s !== (s = t[1][1])) {
+        p(t, o) {
+            const c = {};
+            if (o & 16 && (c.data = t[4]), o & 4 && (c.form = t[2]), o & 2 && s !== (s = t[1][1])) {
                 if (e) {
-                    P();
-                    const o = e;
-                    p(o.$$.fragment, 1, 0, () => {
-                        R(o, 1)
-                    }), L()
+                    N();
+                    const f = e;
+                    h(f.$$.fragment, 1, 0, () => {
+                        A(f, 1)
+                    }), I()
                 }
-                s ? (e = b(s, f(t)), t[10](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
-            } else s && e.$set(_)
+                s ? (e = k(s, _(t)), t[10](e), v(e.$$.fragment), d(e.$$.fragment, 1), E(e, n.parentNode, n)) : e = null
+            } else s && e.$set(c)
         },
         i(t) {
             i || (e && d(e.$$.fragment, t), i = !0)
         },
         o(t) {
-            e && p(e.$$.fragment, t), i = !1
+            e && h(e.$$.fragment, t), i = !1
         },
         d(t) {
-            a[10](null), t && g(n), e && R(e, t)
+            r[10](null), t && g(n), e && A(e, t)
         }
     }
 }
 
-function I(a) {
-    let e, n = a[6] && O(a);
+function L(r) {
+    let e, n = r[6] && O(r);
     return {
         c() {
-            e = G("div"), n && n.c(), this.h()
+            e = F("div"), n && n.c(), this.h()
         },
         l(i) {
-            e = H(i, "DIV", {
+            e = G(i, "DIV", {
                 id: !0,
                 "aria-live": !0,
                 "aria-atomic": !0,
                 style: !0
             });
-            var s = J(e);
+            var s = H(e);
             n && n.l(s), s.forEach(g), this.h()
         },
         h() {
-            N(e, "id", "svelte-announcer"), N(e, "aria-live", "assertive"), N(e, "aria-atomic", "true"), m(e, "position", "absolute"), m(e, "left", "0"), m(e, "top", "0"), m(e, "clip", "rect(0 0 0 0)"), m(e, "clip-path", "inset(50%)"), m(e, "overflow", "hidden"), m(e, "white-space", "nowrap"), m(e, "width", "1px"), m(e, "height", "1px")
+            P(e, "id", "svelte-announcer"), P(e, "aria-live", "assertive"), P(e, "aria-atomic", "true"), m(e, "position", "absolute"), m(e, "left", "0"), m(e, "top", "0"), m(e, "clip", "rect(0 0 0 0)"), m(e, "clip-path", "inset(50%)"), m(e, "overflow", "hidden"), m(e, "white-space", "nowrap"), m(e, "width", "1px"), m(e, "height", "1px")
         },
         m(i, s) {
             w(i, e, s), n && n.m(e, null)
         },
         p(i, s) {
             i[6] ? n ? n.p(i, s) : (n = O(i), n.c(), n.m(e, null)) : n && (n.d(1), n = null)
         },
         d(i) {
             i && g(e), n && n.d()
         }
     }
 }
 
-function O(a) {
+function O(r) {
     let e;
     return {
         c() {
-            e = K(a[7])
+            e = J(r[7])
         },
         l(n) {
-            e = M(n, a[7])
+            e = K(n, r[7])
         },
         m(n, i) {
             w(n, e, i)
         },
         p(n, i) {
             i & 128 && Q(e, n[7])
         },
         d(n) {
             n && g(e)
         }
     }
 }
 
-function ee(a) {
-    let e, n, i, s, f;
-    const t = [$, Z],
-        r = [];
+function Z(r) {
+    let e, n, i, s, _;
+    const t = [X, W],
+        o = [];
 
-    function _(l, u) {
-        return l[1][1] ? 0 : 1
+    function c(a, u) {
+        return a[1][1] ? 0 : 1
     }
-    e = _(a), n = r[e] = t[e](a);
-    let o = a[5] && I(a);
+    e = c(r), n = o[e] = t[e](r);
+    let f = r[5] && L(r);
     return {
         c() {
-            n.c(), i = j(), o && o.c(), s = h()
+            n.c(), i = B(), f && f.c(), s = p()
         },
-        l(l) {
-            n.l(l), i = z(l), o && o.l(l), s = h()
+        l(a) {
+            n.l(a), i = C(a), f && f.l(a), s = p()
         },
-        m(l, u) {
-            r[e].m(l, u), w(l, i, u), o && o.m(l, u), w(l, s, u), f = !0
+        m(a, u) {
+            o[e].m(a, u), w(a, i, u), f && f.m(a, u), w(a, s, u), _ = !0
         },
-        p(l, [u]) {
-            let k = e;
-            e = _(l), e === k ? r[e].p(l, u) : (P(), p(r[k], 1, 1, () => {
-                r[k] = null
-            }), L(), n = r[e], n ? n.p(l, u) : (n = r[e] = t[e](l), n.c()), d(n, 1), n.m(i.parentNode, i)), l[5] ? o ? o.p(l, u) : (o = I(l), o.c(), o.m(s.parentNode, s)) : o && (o.d(1), o = null)
+        p(a, [u]) {
+            let b = e;
+            e = c(a), e === b ? o[e].p(a, u) : (N(), h(o[b], 1, 1, () => {
+                o[b] = null
+            }), I(), n = o[e], n ? n.p(a, u) : (n = o[e] = t[e](a), n.c()), d(n, 1), n.m(i.parentNode, i)), a[5] ? f ? f.p(a, u) : (f = L(a), f.c(), f.m(s.parentNode, s)) : f && (f.d(1), f = null)
         },
-        i(l) {
-            f || (d(n), f = !0)
+        i(a) {
+            _ || (d(n), _ = !0)
         },
-        o(l) {
-            p(n), f = !1
+        o(a) {
+            h(n), _ = !1
         },
-        d(l) {
-            r[e].d(l), l && g(i), o && o.d(l), l && g(s)
+        d(a) {
+            o[e].d(a), a && g(i), f && f.d(a), a && g(s)
         }
     }
 }
 
-function te(a, e, n) {
+function $(r, e, n) {
     let {
         stores: i
     } = e, {
         page: s
     } = e, {
-        constructors: f
+        constructors: _
     } = e, {
         components: t = []
     } = e, {
-        form: r
+        form: o
     } = e, {
-        data_0: _ = null
+        data_0: c = null
     } = e, {
-        data_1: o = null
+        data_1: f = null
     } = e;
-    W(i.page.notify);
-    let l = !1,
+    M(i.page.notify);
+    let a = !1,
         u = !1,
-        k = null;
-    F(() => {
-        const c = i.page.subscribe(() => {
-            l && (n(6, u = !0), n(7, k = document.title || "untitled page"))
+        b = null;
+    U(() => {
+        const l = i.page.subscribe(() => {
+            a && (n(6, u = !0), n(7, b = document.title || "untitled page"))
         });
-        return n(5, l = !0), c
+        return n(5, a = !0), l
     });
 
-    function T(c) {
-        S[c ? "unshift" : "push"](() => {
-            t[1] = c, n(0, t)
+    function T(l) {
+        R[l ? "unshift" : "push"](() => {
+            t[1] = l, n(0, t)
         })
     }
 
-    function V(c) {
-        S[c ? "unshift" : "push"](() => {
-            t[0] = c, n(0, t)
+    function y(l) {
+        R[l ? "unshift" : "push"](() => {
+            t[0] = l, n(0, t)
         })
     }
 
-    function B(c) {
-        S[c ? "unshift" : "push"](() => {
-            t[0] = c, n(0, t)
+    function q(l) {
+        R[l ? "unshift" : "push"](() => {
+            t[0] = l, n(0, t)
         })
     }
-    return a.$$set = c => {
-        "stores" in c && n(8, i = c.stores), "page" in c && n(9, s = c.page), "constructors" in c && n(1, f = c.constructors), "components" in c && n(0, t = c.components), "form" in c && n(2, r = c.form), "data_0" in c && n(3, _ = c.data_0), "data_1" in c && n(4, o = c.data_1)
-    }, a.$$.update = () => {
-        a.$$.dirty & 768 && i.page.set(s)
-    }, [t, f, r, _, o, l, u, k, i, s, T, V, B]
+    return r.$$set = l => {
+        "stores" in l && n(8, i = l.stores), "page" in l && n(9, s = l.page), "constructors" in l && n(1, _ = l.constructors), "components" in l && n(0, t = l.components), "form" in l && n(2, o = l.form), "data_0" in l && n(3, c = l.data_0), "data_1" in l && n(4, f = l.data_1)
+    }, r.$$.update = () => {
+        r.$$.dirty & 768 && i.page.set(s)
+    }, [t, _, o, c, f, a, u, b, i, s, T, y, q]
 }
-class se extends C {
+class ne extends S {
     constructor(e) {
-        super(), q(this, e, te, ee, U, {
+        super(), j(this, e, $, Z, z, {
             stores: 8,
             page: 9,
             constructors: 1,
             components: 0,
             form: 2,
             data_0: 3,
             data_1: 4
         })
     }
 }
-const re = [() => y(() => import("../nodes/0.67f61f78.js"), ["../nodes/0.67f61f78.js", "../chunks/index.6dba6488.js"], import.meta.url), () => y(() => import("../nodes/1.6c933e22.js"), ["../nodes/1.6c933e22.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url), () => y(() => import("../nodes/2.39aa7785.js"), ["../nodes/2.39aa7785.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url), () => y(() => import("../nodes/3.d433accd.js"), ["../nodes/3.d433accd.js", "../chunks/index.6dba6488.js", "../chunks/stores.57c5405b.js", "../chunks/singletons.9f3ec903.js"], import.meta.url)],
-    oe = [],
-    ae = {
+const ie = [() => D(() => import("../nodes/0.2bbf402e.js"), ["../nodes/0.2bbf402e.js", "../chunks/index.8c237fac.js", "../assets/0.cdaa43fa.css"], import.meta.url), () => D(() => import("../nodes/1.ed3af81f.js"), ["../nodes/1.ed3af81f.js", "../chunks/index.8c237fac.js", "../chunks/stores.4b841c19.js", "../chunks/singletons.d791afcf.js"], import.meta.url), () => D(() => import("../nodes/2.375c4cd1.js"), ["../nodes/2.375c4cd1.js", "../chunks/2.cb8e4807.js", "../chunks/index.8c237fac.js", "../chunks/preload-helper.41c905a7.js", "../chunks/singletons.d791afcf.js", "../chunks/parse.bee59afc.js", "../chunks/stores.4b841c19.js", "../assets/2.ec88bf81.css"], import.meta.url), () => D(() => import("../nodes/3.35180ced.js"), ["../nodes/3.35180ced.js", "../chunks/index.8c237fac.js", "../chunks/stores.4b841c19.js", "../chunks/singletons.d791afcf.js"], import.meta.url)],
+    se = [],
+    oe = {
         "/": [2],
         "/kk": [3]
     },
-    le = {
+    re = {
         handleError: ({
-            error: a
+            error: r
         }) => {
-            console.error(a)
+            console.error(r)
         }
     };
 export {
-    ae as dictionary, le as hooks, ie as matchers, re as nodes, se as root, oe as server_loads
+    oe as dictionary, re as hooks, te as matchers, ie as nodes, ne as root, se as server_loads
 };
```

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/entry/start.4cfa1304.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/entry/start.dc4cd066.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,735 +1,659 @@
 import {
-    o as Ce,
-    t as ye
-} from "../chunks/index.6dba6488.js";
+    o as De,
+    t as _e
+} from "../chunks/index.8c237fac.js";
 import {
-    S as Je,
-    a as Ke,
+    S as Ke,
+    a as Ve,
     I as q,
-    g as De,
+    g as Ne,
     f as qe,
-    b as we,
+    b as ye,
     c as le,
-    s as V,
-    i as _e,
-    d as Q,
-    e as K,
-    P as Fe,
-    h as We
-} from "../chunks/singletons.9f3ec903.js";
+    s as H,
+    i as we,
+    d as Z,
+    e as V,
+    P as Me,
+    h as Ye
+} from "../chunks/singletons.d791afcf.js";
+import {
+    u as Xe
+} from "../chunks/parse.bee59afc.js";
 
-function Xe(t, o) {
-    return t === "/" || o === "ignore" ? t : o === "never" ? t.endsWith("/") ? t.slice(0, -1) : t : o === "always" && !t.endsWith("/") ? t + "/" : t
+function Qe(a, o) {
+    return a === "/" || o === "ignore" ? a : o === "never" ? a.endsWith("/") ? a.slice(0, -1) : a : o === "always" && !a.endsWith("/") ? a + "/" : a
 }
 
-function Ze(t) {
-    return t.split("%25").map(decodeURI).join("%25")
+function Ze(a) {
+    return a.split("%25").map(decodeURI).join("%25")
 }
 
-function Qe(t) {
-    for (const o in t) t[o] = decodeURIComponent(t[o]);
-    return t
+function et(a) {
+    for (const o in a) a[o] = decodeURIComponent(a[o]);
+    return a
 }
-const et = ["href", "pathname", "search", "searchParams", "toString", "toJSON"];
+const tt = ["href", "pathname", "search", "searchParams", "toString", "toJSON"];
 
-function tt(t, o) {
-    const u = new URL(t);
-    for (const i of et) Object.defineProperty(u, i, {
+function nt(a, o) {
+    const l = new URL(a);
+    for (const c of tt) Object.defineProperty(l, c, {
         get() {
-            return o(), t[i]
+            return o(), a[c]
         },
         enumerable: !0,
         configurable: !0
     });
-    return nt(u), u
+    return at(l), l
 }
 
-function nt(t) {
-    Object.defineProperty(t, "hash", {
+function at(a) {
+    Object.defineProperty(a, "hash", {
         get() {
             throw new Error("Cannot access event.url.hash. Consider using `$page.url.hash` inside a component instead")
         }
     })
 }
-const at = "/__data.json";
+const rt = "/__data.json";
 
-function rt(t) {
-    return t.replace(/\/$/, "") + at
+function ot(a) {
+    return a.replace(/\/$/, "") + rt
 }
 
-function ze(t) {
+function ze(a) {
     try {
-        return JSON.parse(sessionStorage[t])
+        return JSON.parse(sessionStorage[a])
     } catch {}
 }
 
-function Me(t, o) {
-    const u = JSON.stringify(o);
+function Fe(a, o) {
+    const l = JSON.stringify(o);
     try {
-        sessionStorage[t] = u
+        sessionStorage[a] = l
     } catch {}
 }
 
-function ot(...t) {
+function it(...a) {
     let o = 5381;
-    for (const u of t)
-        if (typeof u == "string") {
-            let i = u.length;
-            for (; i;) o = o * 33 ^ u.charCodeAt(--i)
-        } else if (ArrayBuffer.isView(u)) {
-        const i = new Uint8Array(u.buffer, u.byteOffset, u.byteLength);
-        let d = i.length;
-        for (; d;) o = o * 33 ^ i[--d]
+    for (const l of a)
+        if (typeof l == "string") {
+            let c = l.length;
+            for (; c;) o = o * 33 ^ l.charCodeAt(--c)
+        } else if (ArrayBuffer.isView(l)) {
+        const c = new Uint8Array(l.buffer, l.byteOffset, l.byteLength);
+        let m = c.length;
+        for (; m;) o = o * 33 ^ c[--m]
     } else throw new TypeError("value must be a string or TypedArray");
     return (o >>> 0).toString(36)
 }
 const fe = window.fetch;
-window.fetch = (t, o) => ((t instanceof Request ? t.method : (o == null ? void 0 : o.method) || "GET") !== "GET" && te.delete(Se(t)), fe(t, o));
+window.fetch = (a, o) => ((a instanceof Request ? a.method : (o == null ? void 0 : o.method) || "GET") !== "GET" && te.delete(Ee(a)), fe(a, o));
 const te = new Map;
 
-function it(t, o) {
-    const u = Se(t, o),
-        i = document.querySelector(u);
-    if (i != null && i.textContent) {
+function st(a, o) {
+    const l = Ee(a, o),
+        c = document.querySelector(l);
+    if (c != null && c.textContent) {
         const {
-            body: d,
-            ...f
-        } = JSON.parse(i.textContent), S = i.getAttribute("data-ttl");
-        return S && te.set(u, {
-            body: d,
-            init: f,
-            ttl: 1e3 * Number(S)
-        }), Promise.resolve(new Response(d, f))
+            body: m,
+            ..._
+        } = JSON.parse(c.textContent), E = c.getAttribute("data-ttl");
+        return E && te.set(l, {
+            body: m,
+            init: _,
+            ttl: 1e3 * Number(E)
+        }), Promise.resolve(new Response(m, _))
     }
-    return fe(t, o)
+    return fe(a, o)
 }
 
-function st(t, o, u) {
+function ct(a, o, l) {
     if (te.size > 0) {
-        const i = Se(t, u),
-            d = te.get(i);
-        if (d) {
-            if (performance.now() < d.ttl && ["default", "force-cache", "only-if-cached", void 0].includes(u == null ? void 0 : u.cache)) return new Response(d.body, d.init);
-            te.delete(i)
+        const c = Ee(a, l),
+            m = te.get(c);
+        if (m) {
+            if (performance.now() < m.ttl && ["default", "force-cache", "only-if-cached", void 0].includes(l == null ? void 0 : l.cache)) return new Response(m.body, m.init);
+            te.delete(c)
         }
     }
-    return fe(o, u)
+    return fe(o, l)
 }
 
-function Se(t, o) {
-    let i = `script[data-sveltekit-fetched][data-url=${JSON.stringify(t instanceof Request?t.url:t)}]`;
+function Ee(a, o) {
+    let c = `script[data-sveltekit-fetched][data-url=${JSON.stringify(a instanceof Request?a.url:a)}]`;
     if (o != null && o.headers || o != null && o.body) {
-        const d = [];
-        o.headers && d.push([...new Headers(o.headers)].join(",")), o.body && (typeof o.body == "string" || ArrayBuffer.isView(o.body)) && d.push(o.body), i += `[data-hash="${ot(...d)}"]`
+        const m = [];
+        o.headers && m.push([...new Headers(o.headers)].join(",")), o.body && (typeof o.body == "string" || ArrayBuffer.isView(o.body)) && m.push(o.body), c += `[data-hash="${it(...m)}"]`
     }
-    return i
+    return c
 }
-const ct = /^(\[)?(\.\.\.)?(\w+)(?:=(\w+))?(\])?$/;
+const lt = /^(\[)?(\.\.\.)?(\w+)(?:=(\w+))?(\])?$/;
 
-function lt(t) {
+function ft(a) {
     const o = [];
     return {
-        pattern: t === "/" ? /^\/$/ : new RegExp(`^${ut(t).map(i=>{const d=/^\[\.\.\.(\w+)(?:=(\w+))?\]$/.exec(i);if(d)return o.push({name:d[1],matcher:d[2],optional:!1,rest:!0,chained:!0}),"(?:/(.*))?";const f=/^\[\[(\w+)(?:=(\w+))?\]\]$/.exec(i);if(f)return o.push({name:f[1],matcher:f[2],optional:!0,rest:!1,chained:!0}),"(?:/([^/]+))?";if(!i)return;const S=i.split(/\[(.+?)\](?!\])/);return"/"+S.map((b,w)=>{if(w%2){if(b.startsWith("x+"))return be(String.fromCharCode(parseInt(b.slice(2),16)));if(b.startsWith("u+"))return be(String.fromCharCode(...b.slice(2).split("-").map(P=>parseInt(P,16))));const p=ct.exec(b);if(!p)throw new Error(`
+        pattern: a === "/" ? /^\/$/ : new RegExp(`^${dt(a).map(c=>{const m=/^\[\.\.\.(\w+)(?:=(\w+))?\]$/.exec(c);if(m)return o.push({name:m[1],matcher:m[2],optional:!1,rest:!0,chained:!0}),"(?:/(.*))?";const _=/^\[\[(\w+)(?:=(\w+))?\]\]$/.exec(c);if(_)return o.push({name:_[1],matcher:_[2],optional:!0,rest:!1,chained:!0}),"(?:/([^/]+))?";if(!c)return;const E=c.split(/\[(.+?)\](?!\])/);return"/"+E.map((b,S)=>{if(S%2){if(b.startsWith("x+"))return ve(String.fromCharCode(parseInt(b.slice(2),16)));if(b.startsWith("u+"))return ve(String.fromCharCode(...b.slice(2).split("-").map(P=>parseInt(P,16))));const g=lt.exec(b);if(!g)throw new Error(`
             Invalid param: $ {
                 b
             }.Params and matcher names can only have underscores and alphanumeric characters.
-            `);const[,C,x,k,N]=p;return o.push({name:k,matcher:N,optional:!!C,rest:!!x,chained:x?w===1&&S[0]==="":!1}),x?"(.*?)":C?"([^/]*)?":"([^/]+?)"}return be(b)}).join("")}).join("")}/?$`),
+            `);const[,N,j,I,O]=g;return o.push({name:I,matcher:O,optional:!!N,rest:!!j,chained:j?S===1&&E[0]==="":!1}),j?"(.*?)":N?"([^/]*)?":"([^/]+?)"}return ve(b)}).join("")}).join("")}/?$`),
         params: o
     }
 }
 
-function ft(t) {
-    return !/^\([^)]+\)$/.test(t)
+function ut(a) {
+    return !/^\([^)]+\)$/.test(a)
 }
 
-function ut(t) {
-    return t.slice(1).split("/").filter(ft)
+function dt(a) {
+    return a.slice(1).split("/").filter(ut)
 }
 
-function dt(t, o, u) {
-    const i = {},
-        d = t.slice(1);
-    let f = 0;
-    for (let S = 0; S < o.length; S += 1) {
-        const l = o[S],
-            b = d[S - f];
-        if (l.chained && l.rest && f) {
-            i[l.name] = d.slice(S - f, S + 1).filter(w => w).join("/"), f = 0;
+function pt(a, o, l) {
+    const c = {},
+        m = a.slice(1);
+    let _ = 0;
+    for (let E = 0; E < o.length; E += 1) {
+        const y = o[E],
+            b = m[E - _];
+        if (y.chained && y.rest && _) {
+            c[y.name] = m.slice(E - _, E + 1).filter(S => S).join("/"), _ = 0;
             continue
         }
         if (b === void 0) {
-            l.rest && (i[l.name] = "");
+            y.rest && (c[y.name] = "");
             continue
         }
-        if (!l.matcher || u[l.matcher](b)) {
-            i[l.name] = b;
-            const w = o[S + 1],
-                p = d[S + 1];
-            w && !w.rest && w.optional && p && (f = 0);
+        if (!y.matcher || l[y.matcher](b)) {
+            c[y.name] = b;
+            const S = o[E + 1],
+                g = m[E + 1];
+            S && !S.rest && S.optional && g && (_ = 0);
             continue
         }
-        if (l.optional && l.chained) {
-            f++;
+        if (y.optional && y.chained) {
+            _++;
             continue
         }
         return
     }
-    if (!f) return i
+    if (!_) return c
 }
 
-function be(t) {
-    return t.normalize().replace(/[[\]]/g, "\\$&").replace(/%/g, "%25").replace(/\//g, "%2[Ff]").replace(/\?/g, "%3[Ff]").replace(/#/g, "%23").replace(/[.*+?^${}()|\\]/g, "\\$&")
+function ve(a) {
+    return a.normalize().replace(/[[\]]/g, "\\$&").replace(/%/g, "%25").replace(/\//g, "%2[Ff]").replace(/\?/g, "%3[Ff]").replace(/#/g, "%23").replace(/[.*+?^${}()|\\]/g, "\\$&")
 }
 
-function pt({
-    nodes: t,
+function ht({
+    nodes: a,
     server_loads: o,
-    dictionary: u,
-    matchers: i
+    dictionary: l,
+    matchers: c
 }) {
-    const d = new Set(o);
-    return Object.entries(u).map(([l, [b, w, p]]) => {
+    const m = new Set(o);
+    return Object.entries(l).map(([y, [b, S, g]]) => {
         const {
-            pattern: C,
-            params: x
-        } = lt(l), k = {
-            id: l,
-            exec: N => {
-                const P = C.exec(N);
-                if (P) return dt(P, x, i)
+            pattern: N,
+            params: j
+        } = ft(y), I = {
+            id: y,
+            exec: O => {
+                const P = N.exec(O);
+                if (P) return pt(P, j, c)
             },
-            errors: [1, ...p || []].map(N => t[N]),
-            layouts: [0, ...w || []].map(S),
-            leaf: f(b)
+            errors: [1, ...g || []].map(O => a[O]),
+            layouts: [0, ...S || []].map(E),
+            leaf: _(b)
         };
-        return k.errors.length = k.layouts.length = Math.max(k.errors.length, k.layouts.length), k
+        return I.errors.length = I.layouts.length = Math.max(I.errors.length, I.layouts.length), I
     });
 
-    function f(l) {
-        const b = l < 0;
-        return b && (l = ~l), [b, t[l]]
+    function _(y) {
+        const b = y < 0;
+        return b && (y = ~y), [b, a[y]]
     }
 
-    function S(l) {
-        return l === void 0 ? l : [d.has(l), t[l]]
+    function E(y) {
+        return y === void 0 ? y : [m.has(y), a[y]]
     }
 }
 let ee = class {
-        constructor(o, u) {
-            this.status = o, typeof u == "string" ? this.body = {
-                message: u
-            } : u ? this.body = u : this.body = {
+        constructor(o, l) {
+            this.status = o, typeof l == "string" ? this.body = {
+                message: l
+            } : l ? this.body = l : this.body = {
                 message: `Error: ${o}`
             }
         }
         toString() {
             return JSON.stringify(this.body)
         }
     },
-    Ve = class {
-        constructor(o, u) {
-            this.status = o, this.location = u
+    He = class {
+        constructor(o, l) {
+            this.status = o, this.location = l
         }
     };
-async function ht(t) {
+async function mt(a) {
     var o;
-    for (const u in t)
-        if (typeof((o = t[u]) == null ? void 0 : o.then) == "function") return Object.fromEntries(await Promise.all(Object.entries(t).map(async ([i, d]) => [i, await d])));
-    return t
-}
-const gt = -1,
-    mt = -2,
-    yt = -3,
-    wt = -4,
-    _t = -5,
-    bt = -6;
-
-function vt(t, o) {
-    if (typeof t == "number") return d(t, !0);
-    if (!Array.isArray(t) || t.length === 0) throw new Error("Invalid input");
-    const u = t,
-        i = Array(u.length);
-
-    function d(f, S = !1) {
-        if (f === gt) return;
-        if (f === yt) return NaN;
-        if (f === wt) return 1 / 0;
-        if (f === _t) return -1 / 0;
-        if (f === bt) return -0;
-        if (S) throw new Error("Invalid input");
-        if (f in i) return i[f];
-        const l = u[f];
-        if (!l || typeof l != "object") i[f] = l;
-        else if (Array.isArray(l))
-            if (typeof l[0] == "string") {
-                const b = l[0],
-                    w = o == null ? void 0 : o[b];
-                if (w) return i[f] = w(d(l[1]));
-                switch (b) {
-                    case "Date":
-                        i[f] = new Date(l[1]);
-                        break;
-                    case "Set":
-                        const p = new Set;
-                        i[f] = p;
-                        for (let k = 1; k < l.length; k += 1) p.add(d(l[k]));
-                        break;
-                    case "Map":
-                        const C = new Map;
-                        i[f] = C;
-                        for (let k = 1; k < l.length; k += 2) C.set(d(l[k]), d(l[k + 1]));
-                        break;
-                    case "RegExp":
-                        i[f] = new RegExp(l[1], l[2]);
-                        break;
-                    case "Object":
-                        i[f] = Object(l[1]);
-                        break;
-                    case "BigInt":
-                        i[f] = BigInt(l[1]);
-                        break;
-                    case "null":
-                        const x = Object.create(null);
-                        i[f] = x;
-                        for (let k = 1; k < l.length; k += 2) x[l[k]] = d(l[k + 1]);
-                        break;
-                    default:
-                        throw new Error(`Unknown type ${b}`)
-                }
-            } else {
-                const b = new Array(l.length);
-                i[f] = b;
-                for (let w = 0; w < l.length; w += 1) {
-                    const p = l[w];
-                    p !== mt && (b[w] = d(p))
-                }
-            }
-        else {
-            const b = {};
-            i[f] = b;
-            for (const w in l) {
-                const p = l[w];
-                b[w] = d(p)
-            }
-        }
-        return i[f]
-    }
-    return d(0)
+    for (const l in a)
+        if (typeof((o = a[l]) == null ? void 0 : o.then) == "function") return Object.fromEntries(await Promise.all(Object.entries(a).map(async ([c, m]) => [c, await m])));
+    return a
 }
 const Be = new Set(["load", "prerender", "csr", "ssr", "trailingSlash", "config"]);
 [...Be];
-const Et = new Set([...Be, "actions"]);
-[...Et];
+const gt = new Set([...Be, "actions"]);
+[...gt];
 
-function St(t) {
-    return t.filter(o => o != null)
+function _t(a) {
+    return a.filter(o => o != null)
 }
-const kt = "x-sveltekit-invalidated",
-    z = ze(Je) ?? {},
-    Z = ze(Ke) ?? {};
-
-function ve(t) {
-    z[t] = Q()
-}
-
-function Rt(t, o) {
-    var $e;
-    const u = pt(t),
-        i = t.nodes[0],
-        d = t.nodes[1];
-    i(), d();
-    const f = document.documentElement,
-        S = [],
-        l = [];
+const yt = "x-sveltekit-invalidated",
+    z = ze(Ke) ?? {},
+    Q = ze(Ve) ?? {};
+
+function be(a) {
+    z[a] = Z()
+}
+
+function wt(a, o) {
+    var Ie;
+    const l = ht(a),
+        c = a.nodes[0],
+        m = a.nodes[1];
+    c(), m();
+    const _ = document.documentElement,
+        E = [],
+        y = [];
     let b = null;
-    const w = {
+    const S = {
         before_navigate: [],
         after_navigate: []
     };
-    let p = {
+    let g = {
             branch: [],
             error: null,
             url: null
         },
-        C = !1,
-        x = !1,
-        k = !0,
         N = !1,
+        j = !1,
+        I = !0,
+        O = !1,
         P = !1,
         B = !1,
-        H = !1,
-        F, j = ($e = history.state) == null ? void 0 : $e[q];
-    j || (j = Date.now(), history.replaceState({
+        J = !1,
+        M, C = (Ie = history.state) == null ? void 0 : Ie[q];
+    C || (C = Date.now(), history.replaceState({
         ...history.state,
-        [q]: j
+        [q]: C
     }, "", location.href));
-    const ue = z[j];
+    const ue = z[C];
     ue && (history.scrollRestoration = "manual", scrollTo(ue.x, ue.y));
-    let M, ne, ae;
-    async function ke() {
+    let F, ne, ae;
+    async function Re() {
         ae = ae || Promise.resolve(), await ae, ae = null;
         const e = new URL(location.href),
-            n = W(e, !0);
+            t = Y(e, !0);
         b = null;
         const r = ne = {},
-            a = n && await he(n);
-        if (r === ne && a) {
-            if (a.type === "redirect") return re(new URL(a.location, e).href, {}, [e.pathname], r);
-            a.props.page !== void 0 && (M = a.props.page), F.$set(a.props)
+            n = t && await he(t);
+        if (r === ne && n) {
+            if (n.type === "redirect") return re(new URL(n.location, e).href, {}, [e.pathname], r);
+            n.props.page !== void 0 && (F = n.props.page), M.$set(n.props)
         }
     }
 
-    function Re(e) {
-        l.some(n => n == null ? void 0 : n.snapshot) && (Z[e] = l.map(n => {
+    function xe(e) {
+        y.some(t => t == null ? void 0 : t.snapshot) && (Q[e] = y.map(t => {
             var r;
-            return (r = n == null ? void 0 : n.snapshot) == null ? void 0 : r.capture()
+            return (r = t == null ? void 0 : t.snapshot) == null ? void 0 : r.capture()
         }))
     }
 
-    function Ae(e) {
-        var n;
-        (n = Z[e]) == null || n.forEach((r, a) => {
-            var s, c;
-            (c = (s = l[a]) == null ? void 0 : s.snapshot) == null || c.restore(r)
+    function ke(e) {
+        var t;
+        (t = Q[e]) == null || t.forEach((r, n) => {
+            var i, s;
+            (s = (i = y[n]) == null ? void 0 : i.snapshot) == null || s.restore(r)
         })
     }
 
     function Le() {
-        ve(j), Me(Je, z), Re(j), Me(Ke, Z)
+        be(C), Fe(Ke, z), xe(C), Fe(Ve, Q)
     }
     async function re(e, {
-        noScroll: n = !1,
+        noScroll: t = !1,
         replaceState: r = !1,
-        keepFocus: a = !1,
-        state: s = {},
-        invalidateAll: c = !1
-    }, g, m) {
-        return typeof e == "string" && (e = new URL(e, De(document))), ce({
+        keepFocus: n = !1,
+        state: i = {},
+        invalidateAll: s = !1
+    }, u, d) {
+        return typeof e == "string" && (e = new URL(e, Ne(document))), ce({
             url: e,
-            scroll: n ? Q() : null,
-            keepfocus: a,
-            redirect_chain: g,
+            scroll: t ? Z() : null,
+            keepfocus: n,
+            redirect_chain: u,
             details: {
-                state: s,
+                state: i,
                 replaceState: r
             },
-            nav_token: m,
+            nav_token: d,
             accepted: () => {
-                c && (H = !0)
+                s && (J = !0)
             },
             blocked: () => {},
             type: "goto"
         })
     }
-    async function Ie(e) {
+    async function Ae(e) {
         return b = {
             id: e.id,
-            promise: he(e).then(n => (n.type === "loaded" && n.state.error && (b = null), n))
+            promise: he(e).then(t => (t.type === "loaded" && t.state.error && (b = null), t))
         }, b.promise
     }
     async function oe(...e) {
-        const r = u.filter(a => e.some(s => a.exec(s))).map(a => Promise.all([...a.layouts, a.leaf].map(s => s == null ? void 0 : s[1]())));
+        const r = l.filter(n => e.some(i => n.exec(i))).map(n => Promise.all([...n.layouts, n.leaf].map(i => i == null ? void 0 : i[1]())));
         await Promise.all(r)
     }
 
-    function Oe(e) {
-        var a;
-        p = e.state;
-        const n = document.querySelector("style[data-sveltekit]");
-        n && n.remove(), M = e.props.page, F = new t.root({
+    function Pe(e) {
+        var n;
+        g = e.state;
+        const t = document.querySelector("style[data-sveltekit]");
+        t && t.remove(), F = e.props.page, M = new a.root({
             target: o,
             props: {
                 ...e.props,
-                stores: V,
-                components: l
+                stores: H,
+                components: y
             },
             hydrate: !0
-        }), Ae(j);
+        }), ke(C);
         const r = {
             from: null,
             to: {
-                params: p.params,
+                params: g.params,
                 route: {
-                    id: ((a = p.route) == null ? void 0 : a.id) ?? null
+                    id: ((n = g.route) == null ? void 0 : n.id) ?? null
                 },
                 url: new URL(location.href)
             },
             willUnload: !1,
             type: "enter"
         };
-        w.after_navigate.forEach(s => s(r)), x = !0
+        S.after_navigate.forEach(i => i(r)), j = !0
     }
-    async function Y({
+    async function W({
         url: e,
-        params: n,
+        params: t,
         branch: r,
-        status: a,
-        error: s,
-        route: c,
-        form: g
+        status: n,
+        error: i,
+        route: s,
+        form: u
     }) {
-        let m = "never";
-        for (const _ of r)(_ == null ? void 0 : _.slash) !== void 0 && (m = _.slash);
-        e.pathname = Xe(e.pathname, m), e.search = e.search;
-        const v = {
+        let d = "never";
+        for (const h of r)(h == null ? void 0 : h.slash) !== void 0 && (d = h.slash);
+        e.pathname = Qe(e.pathname, d), e.search = e.search;
+        const w = {
             type: "loaded",
             state: {
                 url: e,
-                params: n,
+                params: t,
                 branch: r,
-                error: s,
-                route: c
+                error: i,
+                route: s
             },
             props: {
-                constructors: St(r).map(_ => _.node.component)
+                constructors: _t(r).map(h => h.node.component)
             }
         };
-        g !== void 0 && (v.props.form = g);
-        let y = {},
-            R = !M,
-            L = 0;
-        for (let _ = 0; _ < Math.max(r.length, p.branch.length); _ += 1) {
-            const h = r[_],
-                U = p.branch[_];
-            (h == null ? void 0 : h.data) !== (U == null ? void 0 : U.data) && (R = !0), h && (y = {
-                ...y,
-                ...h.data
-            }, R && (v.props[`data_${L}`] = y), L += 1)
-        }
-        return (!p.url || e.href !== p.url.href || p.error !== s || g !== void 0 && g !== M.form || R) && (v.props.page = {
-            error: s,
-            params: n,
+        u !== void 0 && (w.props.form = u);
+        let p = {},
+            R = !F,
+            k = 0;
+        for (let h = 0; h < Math.max(r.length, g.branch.length); h += 1) {
+            const f = r[h],
+                U = g.branch[h];
+            (f == null ? void 0 : f.data) !== (U == null ? void 0 : U.data) && (R = !0), f && (p = {
+                ...p,
+                ...f.data
+            }, R && (w.props[`data_${k}`] = p), k += 1)
+        }
+        return (!g.url || e.href !== g.url.href || g.error !== i || u !== void 0 && u !== F.form || R) && (w.props.page = {
+            error: i,
+            params: t,
             route: {
-                id: (c == null ? void 0 : c.id) ?? null
+                id: (s == null ? void 0 : s.id) ?? null
             },
-            status: a,
+            status: n,
             url: new URL(e),
-            form: g ?? null,
-            data: R ? y : M.data
-        }), v
+            form: u ?? null,
+            data: R ? p : F.data
+        }), w
     }
     async function de({
         loader: e,
-        parent: n,
+        parent: t,
         url: r,
-        params: a,
-        route: s,
-        server_data_node: c
+        params: n,
+        route: i,
+        server_data_node: s
     }) {
-        var y, R, L;
-        let g = null;
-        const m = {
+        var p, R, k;
+        let u = null;
+        const d = {
                 dependencies: new Set,
                 params: new Set,
                 parent: !1,
                 route: !1,
                 url: !1
             },
-            v = await e();
-        if ((y = v.universal) != null && y.load) {
-            let O = function(...h) {
-                for (const U of h) {
+            w = await e();
+        if ((p = w.universal) != null && p.load) {
+            let A = function(...f) {
+                for (const U of f) {
                     const {
                         href: $
                     } = new URL(U, r);
-                    m.dependencies.add($)
+                    d.dependencies.add($)
                 }
             };
-            const _ = {
+            const h = {
                 route: {
                     get id() {
-                        return m.route = !0, s.id
+                        return d.route = !0, i.id
                     }
                 },
-                params: new Proxy(a, {
-                    get: (h, U) => (m.params.add(U), h[U])
+                params: new Proxy(n, {
+                    get: (f, U) => (d.params.add(U), f[U])
                 }),
-                data: (c == null ? void 0 : c.data) ?? null,
-                url: tt(r, () => {
-                    m.url = !0
+                data: (s == null ? void 0 : s.data) ?? null,
+                url: nt(r, () => {
+                    d.url = !0
                 }),
-                async fetch(h, U) {
+                async fetch(f, U) {
                     let $;
-                    h instanceof Request ? ($ = h.url, U = {
-                        body: h.method === "GET" || h.method === "HEAD" ? void 0 : await h.blob(),
-                        cache: h.cache,
-                        credentials: h.credentials,
-                        headers: h.headers,
-                        integrity: h.integrity,
-                        keepalive: h.keepalive,
-                        method: h.method,
-                        mode: h.mode,
-                        redirect: h.redirect,
-                        referrer: h.referrer,
-                        referrerPolicy: h.referrerPolicy,
-                        signal: h.signal,
+                    f instanceof Request ? ($ = f.url, U = {
+                        body: f.method === "GET" || f.method === "HEAD" ? void 0 : await f.blob(),
+                        cache: f.cache,
+                        credentials: f.credentials,
+                        headers: f.headers,
+                        integrity: f.integrity,
+                        keepalive: f.keepalive,
+                        method: f.method,
+                        mode: f.mode,
+                        redirect: f.redirect,
+                        referrer: f.referrer,
+                        referrerPolicy: f.referrerPolicy,
+                        signal: f.signal,
                         ...U
-                    }) : $ = h;
+                    }) : $ = f;
                     const D = new URL($, r);
-                    return O(D.href), D.origin === r.origin && ($ = D.href.slice(r.origin.length)), x ? st($, D.href, U) : it($, U)
+                    return A(D.href), D.origin === r.origin && ($ = D.href.slice(r.origin.length)), j ? ct($, D.href, U) : st($, U)
                 },
                 setHeaders: () => {},
-                depends: O,
+                depends: A,
                 parent() {
-                    return m.parent = !0, n()
+                    return d.parent = !0, t()
                 }
             };
-            g = await v.universal.load.call(null, _) ?? null, g = g ? await ht(g) : null
+            u = await w.universal.load.call(null, h) ?? null, u = u ? await mt(u) : null
         }
         return {
-            node: v,
+            node: w,
             loader: e,
-            server: c,
-            universal: (R = v.universal) != null && R.load ? {
+            server: s,
+            universal: (R = w.universal) != null && R.load ? {
                 type: "data",
-                data: g,
-                uses: m
+                data: u,
+                uses: d
             } : null,
-            data: g ?? (c == null ? void 0 : c.data) ?? null,
-            slash: ((L = v.universal) == null ? void 0 : L.trailingSlash) ?? (c == null ? void 0 : c.slash)
+            data: u ?? (s == null ? void 0 : s.data) ?? null,
+            slash: ((k = w.universal) == null ? void 0 : k.trailingSlash) ?? (s == null ? void 0 : s.slash)
         }
     }
 
-    function Pe(e, n, r, a, s) {
-        if (H) return !0;
-        if (!a) return !1;
-        if (a.parent && e || a.route && n || a.url && r) return !0;
-        for (const c of a.params)
-            if (s[c] !== p.params[c]) return !0;
-        for (const c of a.dependencies)
-            if (S.some(g => g(new URL(c)))) return !0;
+    function Ue(e, t, r, n, i) {
+        if (J) return !0;
+        if (!n) return !1;
+        if (n.parent && e || n.route && t || n.url && r) return !0;
+        for (const s of n.params)
+            if (i[s] !== g.params[s]) return !0;
+        for (const s of n.dependencies)
+            if (E.some(u => u(new URL(s)))) return !0;
         return !1
     }
 
-    function pe(e, n) {
-        return (e == null ? void 0 : e.type) === "data" ? e : (e == null ? void 0 : e.type) === "skip" ? n ?? null : null
+    function pe(e, t) {
+        return (e == null ? void 0 : e.type) === "data" ? e : (e == null ? void 0 : e.type) === "skip" ? t ?? null : null
     }
     async function he({
         id: e,
-        invalidating: n,
+        invalidating: t,
         url: r,
-        params: a,
-        route: s
+        params: n,
+        route: i
     }) {
         if ((b == null ? void 0 : b.id) === e) return b.promise;
         const {
-            errors: c,
-            layouts: g,
-            leaf: m
-        } = s, v = [...g, m];
-        c.forEach(E => E == null ? void 0 : E().catch(() => {})), v.forEach(E => E == null ? void 0 : E[1]().catch(() => {}));
-        let y = null;
-        const R = p.url ? e !== p.url.pathname + p.url.search : !1,
-            L = p.route ? s.id !== p.route.id : !1;
-        let O = !1;
-        const _ = v.map((E, I) => {
-            var J;
-            const A = p.branch[I],
-                T = !!(E != null && E[0]) && ((A == null ? void 0 : A.loader) !== E[1] || Pe(O, L, R, (J = A.server) == null ? void 0 : J.uses, a));
-            return T && (O = !0), T
+            errors: s,
+            layouts: u,
+            leaf: d
+        } = i, w = [...u, d];
+        s.forEach(v => v == null ? void 0 : v().catch(() => {})), w.forEach(v => v == null ? void 0 : v[1]().catch(() => {}));
+        let p = null;
+        const R = g.url ? e !== g.url.pathname + g.url.search : !1,
+            k = g.route ? i.id !== g.route.id : !1;
+        let A = !1;
+        const h = w.map((v, L) => {
+            var K;
+            const x = g.branch[L],
+                T = !!(v != null && v[0]) && ((x == null ? void 0 : x.loader) !== v[1] || Ue(A, k, R, (K = x.server) == null ? void 0 : K.uses, n));
+            return T && (A = !0), T
         });
-        if (_.some(Boolean)) {
+        if (h.some(Boolean)) {
             try {
-                y = await He(r, _)
-            } catch (E) {
+                p = await Je(r, h)
+            } catch (v) {
                 return ie({
-                    status: E instanceof ee ? E.status : 500,
-                    error: await X(E, {
+                    status: v instanceof ee ? v.status : 500,
+                    error: await X(v, {
                         url: r,
-                        params: a,
+                        params: n,
                         route: {
-                            id: s.id
+                            id: i.id
                         }
                     }),
                     url: r,
-                    route: s
+                    route: i
                 })
             }
-            if (y.type === "redirect") return y
+            if (p.type === "redirect") return p
         }
-        const h = y == null ? void 0 : y.nodes;
+        const f = p == null ? void 0 : p.nodes;
         let U = !1;
-        const $ = v.map(async (E, I) => {
-            var ge;
-            if (!E) return;
-            const A = p.branch[I],
-                T = h == null ? void 0 : h[I];
-            if ((!T || T.type === "skip") && E[1] === (A == null ? void 0 : A.loader) && !Pe(U, L, R, (ge = A.universal) == null ? void 0 : ge.uses, a)) return A;
+        const $ = w.map(async (v, L) => {
+            var me;
+            if (!v) return;
+            const x = g.branch[L],
+                T = f == null ? void 0 : f[L];
+            if ((!T || T.type === "skip") && v[1] === (x == null ? void 0 : x.loader) && !Ue(U, k, R, (me = x.universal) == null ? void 0 : me.uses, n)) return x;
             if (U = !0, (T == null ? void 0 : T.type) === "error") throw T;
             return de({
-                loader: E[1],
+                loader: v[1],
                 url: r,
-                params: a,
-                route: s,
+                params: n,
+                route: i,
                 parent: async () => {
-                    var Te;
-                    const je = {};
-                    for (let me = 0; me < I; me += 1) Object.assign(je, (Te = await $[me]) == null ? void 0 : Te.data);
-                    return je
+                    var je;
+                    const Te = {};
+                    for (let ge = 0; ge < L; ge += 1) Object.assign(Te, (je = await $[ge]) == null ? void 0 : je.data);
+                    return Te
                 },
-                server_data_node: pe(T === void 0 && E[0] ? {
+                server_data_node: pe(T === void 0 && v[0] ? {
                     type: "skip"
-                } : T ?? null, E[0] ? A == null ? void 0 : A.server : void 0)
+                } : T ?? null, v[0] ? x == null ? void 0 : x.server : void 0)
             })
         });
-        for (const E of $) E.catch(() => {});
+        for (const v of $) v.catch(() => {});
         const D = [];
-        for (let E = 0; E < v.length; E += 1)
-            if (v[E]) try {
-                D.push(await $[E])
-            } catch (I) {
-                if (I instanceof Ve) return {
+        for (let v = 0; v < w.length; v += 1)
+            if (w[v]) try {
+                D.push(await $[v])
+            } catch (L) {
+                if (L instanceof He) return {
                     type: "redirect",
-                    location: I.location
+                    location: L.location
                 };
-                let A = 500,
+                let x = 500,
                     T;
-                if (h != null && h.includes(I)) A = I.status ?? A, T = I.error;
-                else if (I instanceof ee) A = I.status, T = I.body;
+                if (f != null && f.includes(L)) x = L.status ?? x, T = L.error;
+                else if (L instanceof ee) x = L.status, T = L.body;
                 else {
-                    if (await V.updated.check()) return await G(r);
-                    T = await X(I, {
-                        params: a,
+                    if (await H.updated.check()) return await G(r);
+                    T = await X(L, {
+                        params: n,
                         url: r,
                         route: {
-                            id: s.id
+                            id: i.id
                         }
                     })
                 }
-                const J = await Ue(E, D, c);
-                return J ? await Y({
+                const K = await Oe(v, D, s);
+                return K ? await W({
                     url: r,
-                    params: a,
-                    branch: D.slice(0, J.idx).concat(J.node),
-                    status: A,
+                    params: n,
+                    branch: D.slice(0, K.idx).concat(K.node),
+                    status: x,
                     error: T,
-                    route: s
-                }) : await Ne(r, {
-                    id: s.id
-                }, T, A)
+                    route: i
+                }) : await Ce(r, {
+                    id: i.id
+                }, T, x)
             } else D.push(void 0);
-        return await Y({
+        return await W({
             url: r,
-            params: a,
+            params: n,
             branch: D,
             status: 200,
             error: null,
-            route: s,
-            form: n ? void 0 : null
+            route: i,
+            form: t ? void 0 : null
         })
     }
-    async function Ue(e, n, r) {
+    async function Oe(e, t, r) {
         for (; e--;)
             if (r[e]) {
-                let a = e;
-                for (; !n[a];) a -= 1;
+                let n = e;
+                for (; !t[n];) n -= 1;
                 try {
                     return {
-                        idx: a + 1,
+                        idx: n + 1,
                         node: {
                             node: await r[e](),
                             loader: r[e],
                             data: {},
                             server: null,
                             universal: null
                         }
@@ -737,624 +661,624 @@
                 } catch {
                     continue
                 }
             }
     }
     async function ie({
         status: e,
-        error: n,
+        error: t,
         url: r,
-        route: a
+        route: n
     }) {
-        const s = {};
-        let c = null;
-        if (t.server_loads[0] === 0) try {
-            const y = await He(r, [!0]);
-            if (y.type !== "data" || y.nodes[0] && y.nodes[0].type !== "data") throw 0;
-            c = y.nodes[0] ?? null
+        const i = {};
+        let s = null;
+        if (a.server_loads[0] === 0) try {
+            const p = await Je(r, [!0]);
+            if (p.type !== "data" || p.nodes[0] && p.nodes[0].type !== "data") throw 0;
+            s = p.nodes[0] ?? null
         } catch {
-            (r.origin !== location.origin || r.pathname !== location.pathname || C) && await G(r)
+            (r.origin !== location.origin || r.pathname !== location.pathname || N) && await G(r)
         }
-        const m = await de({
-                loader: i,
+        const d = await de({
+                loader: c,
                 url: r,
-                params: s,
-                route: a,
+                params: i,
+                route: n,
                 parent: () => Promise.resolve({}),
-                server_data_node: pe(c)
+                server_data_node: pe(s)
             }),
-            v = {
-                node: await d(),
-                loader: d,
+            w = {
+                node: await m(),
+                loader: m,
                 universal: null,
                 server: null,
                 data: null
             };
-        return await Y({
+        return await W({
             url: r,
-            params: s,
-            branch: [m, v],
+            params: i,
+            branch: [d, w],
             status: e,
-            error: n,
+            error: t,
             route: null
         })
     }
 
-    function W(e, n) {
-        if (_e(e, K)) return;
+    function Y(e, t) {
+        if (we(e, V)) return;
         const r = se(e);
-        for (const a of u) {
-            const s = a.exec(r);
-            if (s) return {
+        for (const n of l) {
+            const i = n.exec(r);
+            if (i) return {
                 id: e.pathname + e.search,
-                invalidating: n,
-                route: a,
-                params: Qe(s),
+                invalidating: t,
+                route: n,
+                params: et(i),
                 url: e
             }
         }
     }
 
     function se(e) {
-        return Ze(e.pathname.slice(K.length) || "/")
+        return Ze(e.pathname.slice(V.length) || "/")
     }
 
-    function xe({
+    function $e({
         url: e,
-        type: n,
+        type: t,
         intent: r,
-        delta: a
+        delta: n
     }) {
-        var m, v;
-        let s = !1;
-        const c = {
+        var d, w;
+        let i = !1;
+        const s = {
             from: {
-                params: p.params,
+                params: g.params,
                 route: {
-                    id: ((m = p.route) == null ? void 0 : m.id) ?? null
+                    id: ((d = g.route) == null ? void 0 : d.id) ?? null
                 },
-                url: p.url
+                url: g.url
             },
             to: {
                 params: (r == null ? void 0 : r.params) ?? null,
                 route: {
-                    id: ((v = r == null ? void 0 : r.route) == null ? void 0 : v.id) ?? null
+                    id: ((w = r == null ? void 0 : r.route) == null ? void 0 : w.id) ?? null
                 },
                 url: e
             },
             willUnload: !r,
-            type: n
+            type: t
         };
-        a !== void 0 && (c.delta = a);
-        const g = {
-            ...c,
+        n !== void 0 && (s.delta = n);
+        const u = {
+            ...s,
             cancel: () => {
-                s = !0
+                i = !0
             }
         };
-        return P || w.before_navigate.forEach(y => y(g)), s ? null : c
+        return P || S.before_navigate.forEach(p => p(u)), i ? null : s
     }
     async function ce({
         url: e,
-        scroll: n,
+        scroll: t,
         keepfocus: r,
-        redirect_chain: a,
-        details: s,
-        type: c,
-        delta: g,
-        nav_token: m = {},
-        accepted: v,
-        blocked: y
+        redirect_chain: n,
+        details: i,
+        type: s,
+        delta: u,
+        nav_token: d = {},
+        accepted: w,
+        blocked: p
     }) {
-        var $, D, E;
-        const R = W(e, !1),
-            L = xe({
+        var $, D, v;
+        const R = Y(e, !1),
+            k = $e({
                 url: e,
-                type: c,
-                delta: g,
+                type: s,
+                delta: u,
                 intent: R
             });
-        if (!L) {
-            y();
+        if (!k) {
+            p();
             return
         }
-        const O = j;
-        v(), P = !0, x && V.navigating.set(L), ne = m;
-        let _ = R && await he(R);
-        if (!_) {
-            if (_e(e, K)) return await G(e);
-            _ = await Ne(e, {
+        const A = C;
+        w(), P = !0, j && H.navigating.set(k), ne = d;
+        let h = R && await he(R);
+        if (!h) {
+            if (we(e, V)) return await G(e);
+            h = await Ce(e, {
                 id: null
             }, await X(new Error(`Not found: ${e.pathname}`), {
                 url: e,
                 params: {},
                 route: {
                     id: null
                 }
             }), 404)
         }
-        if (e = (R == null ? void 0 : R.url) || e, ne !== m) return !1;
-        if (_.type === "redirect")
-            if (a.length > 10 || a.includes(e.pathname)) _ = await ie({
+        if (e = (R == null ? void 0 : R.url) || e, ne !== d) return !1;
+        if (h.type === "redirect")
+            if (n.length > 10 || n.includes(e.pathname)) h = await ie({
                 status: 500,
                 error: await X(new Error("Redirect loop"), {
                     url: e,
                     params: {},
                     route: {
                         id: null
                     }
                 }),
                 url: e,
                 route: {
                     id: null
                 }
             });
-            else return re(new URL(_.location, e).href, {}, [...a, e.pathname], m), !1;
-        else(($ = _.props.page) == null ? void 0 : $.status) >= 400 && await V.updated.check() && await G(e);
-        if (S.length = 0, H = !1, N = !0, ve(O), Re(O), (D = _.props.page) != null && D.url && _.props.page.url.pathname !== e.pathname && (e.pathname = (E = _.props.page) == null ? void 0 : E.url.pathname), s) {
-            const I = s.replaceState ? 0 : 1;
-            if (s.state[q] = j += I, history[s.replaceState ? "replaceState" : "pushState"](s.state, "", e), !s.replaceState) {
-                let A = j + 1;
-                for (; Z[A] || z[A];) delete Z[A], delete z[A], A += 1
+            else return re(new URL(h.location, e).href, {}, [...n, e.pathname], d), !1;
+        else(($ = h.props.page) == null ? void 0 : $.status) >= 400 && await H.updated.check() && await G(e);
+        if (E.length = 0, J = !1, O = !0, be(A), xe(A), (D = h.props.page) != null && D.url && h.props.page.url.pathname !== e.pathname && (e.pathname = (v = h.props.page) == null ? void 0 : v.url.pathname), i) {
+            const L = i.replaceState ? 0 : 1;
+            if (i.state[q] = C += L, history[i.replaceState ? "replaceState" : "pushState"](i.state, "", e), !i.replaceState) {
+                let x = C + 1;
+                for (; Q[x] || z[x];) delete Q[x], delete z[x], x += 1
             }
         }
-        b = null, x ? (p = _.state, _.props.page && (_.props.page.url = e), F.$set(_.props)) : Oe(_);
+        b = null, j ? (g = h.state, h.props.page && (h.props.page.url = e), M.$set(h.props)) : Pe(h);
         const {
-            activeElement: h
+            activeElement: f
         } = document;
-        if (await ye(), k) {
-            const I = e.hash && document.getElementById(decodeURIComponent(e.hash.slice(1)));
-            n ? scrollTo(n.x, n.y) : I ? I.scrollIntoView() : scrollTo(0, 0)
-        }
-        const U = document.activeElement !== h && document.activeElement !== document.body;
-        !r && !U && Ee(), k = !0, _.props.page && (M = _.props.page), P = !1, c === "popstate" && Ae(j), w.after_navigate.forEach(I => I(L)), V.navigating.set(null), N = !1
-    }
-    async function Ne(e, n, r, a) {
-        return e.origin === location.origin && e.pathname === location.pathname && !C ? await ie({
-            status: a,
+        if (await _e(), I) {
+            const L = e.hash && document.getElementById(decodeURIComponent(e.hash.slice(1)));
+            t ? scrollTo(t.x, t.y) : L ? L.scrollIntoView() : scrollTo(0, 0)
+        }
+        const U = document.activeElement !== f && document.activeElement !== document.body;
+        !r && !U && Se(), I = !0, h.props.page && (F = h.props.page), P = !1, s === "popstate" && ke(C), S.after_navigate.forEach(L => L(k)), H.navigating.set(null), O = !1
+    }
+    async function Ce(e, t, r, n) {
+        return e.origin === location.origin && e.pathname === location.pathname && !N ? await ie({
+            status: n,
             error: r,
             url: e,
-            route: n
+            route: t
         }) : await G(e)
     }
 
     function G(e) {
         return location.href = e.href, new Promise(() => {})
     }
 
-    function Ye() {
+    function We() {
         let e;
-        f.addEventListener("mousemove", c => {
-            const g = c.target;
+        _.addEventListener("mousemove", s => {
+            const u = s.target;
             clearTimeout(e), e = setTimeout(() => {
-                a(g, 2)
+                n(u, 2)
             }, 20)
         });
 
-        function n(c) {
-            a(c.composedPath()[0], 1)
+        function t(s) {
+            n(s.composedPath()[0], 1)
         }
-        f.addEventListener("mousedown", n), f.addEventListener("touchstart", n, {
+        _.addEventListener("mousedown", t), _.addEventListener("touchstart", t, {
             passive: !0
         });
-        const r = new IntersectionObserver(c => {
-            for (const g of c) g.isIntersecting && (oe(se(new URL(g.target.href))), r.unobserve(g.target))
+        const r = new IntersectionObserver(s => {
+            for (const u of s) u.isIntersecting && (oe(se(new URL(u.target.href))), r.unobserve(u.target))
         }, {
             threshold: 0
         });
 
-        function a(c, g) {
-            const m = qe(c, f);
-            if (!m) return;
+        function n(s, u) {
+            const d = qe(s, _);
+            if (!d) return;
             const {
-                url: v,
-                external: y,
+                url: w,
+                external: p,
                 download: R
-            } = we(m, K);
-            if (y || R) return;
-            const L = le(m);
-            if (!L.reload)
-                if (g <= L.preload_data) {
-                    const O = W(v, !1);
-                    O && Ie(O)
-                } else g <= L.preload_code && oe(se(v))
+            } = ye(d, V);
+            if (p || R) return;
+            const k = le(d);
+            if (!k.reload)
+                if (u <= k.preload_data) {
+                    const A = Y(w, !1);
+                    A && Ae(A)
+                } else u <= k.preload_code && oe(se(w))
         }
 
-        function s() {
+        function i() {
             r.disconnect();
-            for (const c of f.querySelectorAll("a")) {
+            for (const s of _.querySelectorAll("a")) {
                 const {
-                    url: g,
-                    external: m,
-                    download: v
-                } = we(c, K);
-                if (m || v) continue;
-                const y = le(c);
-                y.reload || (y.preload_code === Fe.viewport && r.observe(c), y.preload_code === Fe.eager && oe(se(g)))
+                    url: u,
+                    external: d,
+                    download: w
+                } = ye(s, V);
+                if (d || w) continue;
+                const p = le(s);
+                p.reload || (p.preload_code === Me.viewport && r.observe(s), p.preload_code === Me.eager && oe(se(u)))
             }
         }
-        w.after_navigate.push(s), s()
+        S.after_navigate.push(i), i()
     }
 
-    function X(e, n) {
-        return e instanceof ee ? e.body : t.hooks.handleError({
+    function X(e, t) {
+        return e instanceof ee ? e.body : a.hooks.handleError({
             error: e,
-            event: n
+            event: t
         }) ?? {
-            message: n.route.id != null ? "Internal Error" : "Not Found"
+            message: t.route.id != null ? "Internal Error" : "Not Found"
         }
     }
     return {
         after_navigate: e => {
-            Ce(() => (w.after_navigate.push(e), () => {
-                const n = w.after_navigate.indexOf(e);
-                w.after_navigate.splice(n, 1)
+            De(() => (S.after_navigate.push(e), () => {
+                const t = S.after_navigate.indexOf(e);
+                S.after_navigate.splice(t, 1)
             }))
         },
         before_navigate: e => {
-            Ce(() => (w.before_navigate.push(e), () => {
-                const n = w.before_navigate.indexOf(e);
-                w.before_navigate.splice(n, 1)
+            De(() => (S.before_navigate.push(e), () => {
+                const t = S.before_navigate.indexOf(e);
+                S.before_navigate.splice(t, 1)
             }))
         },
         disable_scroll_handling: () => {
-            (N || !x) && (k = !1)
+            (O || !j) && (I = !1)
         },
-        goto: (e, n = {}) => re(e, n, []),
+        goto: (e, t = {}) => re(e, t, []),
         invalidate: e => {
-            if (typeof e == "function") S.push(e);
+            if (typeof e == "function") E.push(e);
             else {
                 const {
-                    href: n
+                    href: t
                 } = new URL(e, location.href);
-                S.push(r => r.href === n)
+                E.push(r => r.href === t)
             }
-            return ke()
+            return Re()
         },
-        invalidate_all: () => (H = !0, ke()),
+        invalidate_all: () => (J = !0, Re()),
         preload_data: async e => {
-            const n = new URL(e, De(document)),
-                r = W(n, !1);
-            if (!r) throw new Error(`Attempted to preload a URL that does not belong to this app: ${n}`);
-            await Ie(r)
+            const t = new URL(e, Ne(document)),
+                r = Y(t, !1);
+            if (!r) throw new Error(`Attempted to preload a URL that does not belong to this app: ${t}`);
+            await Ae(r)
         },
         preload_code: oe,
         apply_action: async e => {
             if (e.type === "error") {
-                const n = new URL(location.href),
+                const t = new URL(location.href),
                     {
                         branch: r,
-                        route: a
-                    } = p;
-                if (!a) return;
-                const s = await Ue(p.branch.length, r, a.errors);
-                if (s) {
-                    const c = await Y({
-                        url: n,
-                        params: p.params,
-                        branch: r.slice(0, s.idx).concat(s.node),
+                        route: n
+                    } = g;
+                if (!n) return;
+                const i = await Oe(g.branch.length, r, n.errors);
+                if (i) {
+                    const s = await W({
+                        url: t,
+                        params: g.params,
+                        branch: r.slice(0, i.idx).concat(i.node),
                         status: e.status ?? 500,
                         error: e.error,
-                        route: a
+                        route: n
                     });
-                    p = c.state, F.$set(c.props), ye().then(Ee)
+                    g = s.state, M.$set(s.props), _e().then(Se)
                 }
             } else e.type === "redirect" ? re(e.location, {
                 invalidateAll: !0
-            }, []) : (F.$set({
+            }, []) : (M.$set({
                 form: null,
                 page: {
-                    ...M,
+                    ...F,
                     form: e.data,
                     status: e.status
                 }
-            }), await ye(), F.$set({
+            }), await _e(), M.$set({
                 form: e.data
-            }), e.type === "success" && Ee())
+            }), e.type === "success" && Se())
         },
         _start_router: () => {
             var e;
-            history.scrollRestoration = "manual", addEventListener("beforeunload", n => {
-                var a;
+            history.scrollRestoration = "manual", addEventListener("beforeunload", t => {
+                var n;
                 let r = !1;
                 if (Le(), !P) {
-                    const s = {
+                    const i = {
                         from: {
-                            params: p.params,
+                            params: g.params,
                             route: {
-                                id: ((a = p.route) == null ? void 0 : a.id) ?? null
+                                id: ((n = g.route) == null ? void 0 : n.id) ?? null
                             },
-                            url: p.url
+                            url: g.url
                         },
                         to: null,
                         willUnload: !0,
                         type: "leave",
                         cancel: () => r = !0
                     };
-                    w.before_navigate.forEach(c => c(s))
+                    S.before_navigate.forEach(s => s(i))
                 }
-                r ? (n.preventDefault(), n.returnValue = "") : history.scrollRestoration = "auto"
+                r ? (t.preventDefault(), t.returnValue = "") : history.scrollRestoration = "auto"
             }), addEventListener("visibilitychange", () => {
                 document.visibilityState === "hidden" && Le()
-            }), (e = navigator.connection) != null && e.saveData || Ye(), f.addEventListener("click", n => {
-                if (n.button || n.which !== 1 || n.metaKey || n.ctrlKey || n.shiftKey || n.altKey || n.defaultPrevented) return;
-                const r = qe(n.composedPath()[0], f);
+            }), (e = navigator.connection) != null && e.saveData || We(), _.addEventListener("click", t => {
+                if (t.button || t.which !== 1 || t.metaKey || t.ctrlKey || t.shiftKey || t.altKey || t.defaultPrevented) return;
+                const r = qe(t.composedPath()[0], _);
                 if (!r) return;
                 const {
-                    url: a,
-                    external: s,
-                    target: c,
-                    download: g
-                } = we(r, K);
-                if (!a) return;
-                if (c === "_parent" || c === "_top") {
+                    url: n,
+                    external: i,
+                    target: s,
+                    download: u
+                } = ye(r, V);
+                if (!n) return;
+                if (s === "_parent" || s === "_top") {
                     if (window.parent !== window) return
-                } else if (c && c !== "_self") return;
-                const m = le(r);
-                if (!(r instanceof SVGAElement) && a.protocol !== location.protocol && !(a.protocol === "https:" || a.protocol === "http:") || g) return;
-                if (s || m.reload) {
-                    xe({
-                        url: a,
+                } else if (s && s !== "_self") return;
+                const d = le(r);
+                if (!(r instanceof SVGAElement) && n.protocol !== location.protocol && !(n.protocol === "https:" || n.protocol === "http:") || u) return;
+                if (i || d.reload) {
+                    $e({
+                        url: n,
                         type: "link"
-                    }) ? P = !0 : n.preventDefault();
+                    }) ? P = !0 : t.preventDefault();
                     return
                 }
-                const [y, R] = a.href.split("#");
-                if (R !== void 0 && y === location.href.split("#")[0]) {
-                    if (B = !0, ve(j), p.url = a, V.page.set({
-                            ...M,
-                            url: a
-                        }), V.page.notify(), !m.replace_state) return;
-                    B = !1, n.preventDefault()
+                const [p, R] = n.href.split("#");
+                if (R !== void 0 && p === location.href.split("#")[0]) {
+                    if (B = !0, be(C), g.url = n, H.page.set({
+                            ...F,
+                            url: n
+                        }), H.page.notify(), !d.replace_state) return;
+                    B = !1, t.preventDefault()
                 }
                 ce({
-                    url: a,
-                    scroll: m.noscroll ? Q() : null,
-                    keepfocus: m.keep_focus ?? !1,
+                    url: n,
+                    scroll: d.noscroll ? Z() : null,
+                    keepfocus: d.keep_focus ?? !1,
                     redirect_chain: [],
                     details: {
                         state: {},
-                        replaceState: m.replace_state ?? a.href === location.href
+                        replaceState: d.replace_state ?? n.href === location.href
                     },
-                    accepted: () => n.preventDefault(),
-                    blocked: () => n.preventDefault(),
+                    accepted: () => t.preventDefault(),
+                    blocked: () => t.preventDefault(),
                     type: "link"
                 })
-            }), f.addEventListener("submit", n => {
-                if (n.defaultPrevented) return;
-                const r = HTMLFormElement.prototype.cloneNode.call(n.target),
-                    a = n.submitter;
-                if (((a == null ? void 0 : a.formMethod) || r.method) !== "get") return;
-                const c = new URL((a == null ? void 0 : a.hasAttribute("formaction")) && (a == null ? void 0 : a.formAction) || r.action);
-                if (_e(c, K)) return;
-                const g = n.target,
+            }), _.addEventListener("submit", t => {
+                if (t.defaultPrevented) return;
+                const r = HTMLFormElement.prototype.cloneNode.call(t.target),
+                    n = t.submitter;
+                if (((n == null ? void 0 : n.formMethod) || r.method) !== "get") return;
+                const s = new URL((n == null ? void 0 : n.hasAttribute("formaction")) && (n == null ? void 0 : n.formAction) || r.action);
+                if (we(s, V)) return;
+                const u = t.target,
                     {
-                        keep_focus: m,
-                        noscroll: v,
-                        reload: y,
+                        keep_focus: d,
+                        noscroll: w,
+                        reload: p,
                         replace_state: R
-                    } = le(g);
-                if (y) return;
-                n.preventDefault(), n.stopPropagation();
-                const L = new FormData(g),
-                    O = a == null ? void 0 : a.getAttribute("name");
-                O && L.append(O, (a == null ? void 0 : a.getAttribute("value")) ?? ""), c.search = new URLSearchParams(L).toString(), ce({
-                    url: c,
-                    scroll: v ? Q() : null,
-                    keepfocus: m ?? !1,
+                    } = le(u);
+                if (p) return;
+                t.preventDefault(), t.stopPropagation();
+                const k = new FormData(u),
+                    A = n == null ? void 0 : n.getAttribute("name");
+                A && k.append(A, (n == null ? void 0 : n.getAttribute("value")) ?? ""), s.search = new URLSearchParams(k).toString(), ce({
+                    url: s,
+                    scroll: w ? Z() : null,
+                    keepfocus: d ?? !1,
                     redirect_chain: [],
                     details: {
                         state: {},
-                        replaceState: R ?? c.href === location.href
+                        replaceState: R ?? s.href === location.href
                     },
                     nav_token: {},
                     accepted: () => {},
                     blocked: () => {},
                     type: "form"
                 })
-            }), addEventListener("popstate", async n => {
+            }), addEventListener("popstate", async t => {
                 var r;
-                if ((r = n.state) != null && r[q]) {
-                    if (n.state[q] === j) return;
-                    const a = z[n.state[q]];
-                    if (p.url.href.split("#")[0] === location.href.split("#")[0]) {
-                        z[j] = Q(), j = n.state[q], scrollTo(a.x, a.y);
+                if ((r = t.state) != null && r[q]) {
+                    if (t.state[q] === C) return;
+                    const n = z[t.state[q]];
+                    if (g.url.href.split("#")[0] === location.href.split("#")[0]) {
+                        z[C] = Z(), C = t.state[q], scrollTo(n.x, n.y);
                         return
                     }
-                    const s = n.state[q] - j;
+                    const i = t.state[q] - C;
                     await ce({
                         url: new URL(location.href),
-                        scroll: a,
+                        scroll: n,
                         keepfocus: !1,
                         redirect_chain: [],
                         details: null,
                         accepted: () => {
-                            j = n.state[q]
+                            C = t.state[q]
                         },
                         blocked: () => {
-                            history.go(-s)
+                            history.go(-i)
                         },
                         type: "popstate",
-                        delta: s
+                        delta: i
                     })
                 }
             }), addEventListener("hashchange", () => {
                 B && (B = !1, history.replaceState({
                     ...history.state,
-                    [q]: ++j
+                    [q]: ++C
                 }, "", location.href))
             });
-            for (const n of document.querySelectorAll("link")) n.rel === "icon" && (n.href = n.href);
-            addEventListener("pageshow", n => {
-                n.persisted && V.navigating.set(null)
+            for (const t of document.querySelectorAll("link")) t.rel === "icon" && (t.href = t.href);
+            addEventListener("pageshow", t => {
+                t.persisted && H.navigating.set(null)
             })
         },
         _hydrate: async ({
             status: e = 200,
-            error: n,
+            error: t,
             node_ids: r,
-            params: a,
-            route: s,
-            data: c,
-            form: g
+            params: n,
+            route: i,
+            data: s,
+            form: u
         }) => {
-            C = !0;
-            const m = new URL(location.href);
+            N = !0;
+            const d = new URL(location.href);
             ({
-                params: a = {},
-                route: s = {
+                params: n = {},
+                route: i = {
                     id: null
                 }
-            } = W(m, !1) || {});
-            let v;
+            } = Y(d, !1) || {});
+            let w;
             try {
-                const y = r.map(async (O, _) => {
-                        const h = c[_];
-                        return h != null && h.uses && (h.uses = Ge(h.uses)), de({
-                            loader: t.nodes[O],
-                            url: m,
-                            params: a,
-                            route: s,
+                const p = r.map(async (A, h) => {
+                        const f = s[h];
+                        return f != null && f.uses && (f.uses = Ge(f.uses)), de({
+                            loader: a.nodes[A],
+                            url: d,
+                            params: n,
+                            route: i,
                             parent: async () => {
                                 const U = {};
-                                for (let $ = 0; $ < _; $ += 1) Object.assign(U, (await y[$]).data);
+                                for (let $ = 0; $ < h; $ += 1) Object.assign(U, (await p[$]).data);
                                 return U
                             },
-                            server_data_node: pe(h)
+                            server_data_node: pe(f)
                         })
                     }),
-                    R = await Promise.all(y),
-                    L = u.find(({
-                        id: O
-                    }) => O === s.id);
-                if (L) {
-                    const O = L.layouts;
-                    for (let _ = 0; _ < O.length; _++) O[_] || R.splice(_, 0, void 0)
+                    R = await Promise.all(p),
+                    k = l.find(({
+                        id: A
+                    }) => A === i.id);
+                if (k) {
+                    const A = k.layouts;
+                    for (let h = 0; h < A.length; h++) A[h] || R.splice(h, 0, void 0)
                 }
-                v = await Y({
-                    url: m,
-                    params: a,
+                w = await W({
+                    url: d,
+                    params: n,
                     branch: R,
                     status: e,
-                    error: n,
-                    form: g,
-                    route: L ?? null
+                    error: t,
+                    form: u,
+                    route: k ?? null
                 })
-            } catch (y) {
-                if (y instanceof Ve) {
-                    await G(new URL(y.location, location.href));
+            } catch (p) {
+                if (p instanceof He) {
+                    await G(new URL(p.location, location.href));
                     return
                 }
-                v = await ie({
-                    status: y instanceof ee ? y.status : 500,
-                    error: await X(y, {
-                        url: m,
-                        params: a,
-                        route: s
+                w = await ie({
+                    status: p instanceof ee ? p.status : 500,
+                    error: await X(p, {
+                        url: d,
+                        params: n,
+                        route: i
                     }),
-                    url: m,
-                    route: s
+                    url: d,
+                    route: i
                 })
             }
-            Oe(v)
+            Pe(w)
         }
     }
 }
-async function He(t, o) {
-    const u = new URL(t);
-    u.pathname = rt(t.pathname), u.searchParams.append(kt, o.map(d => d ? "1" : "0").join(""));
-    const i = await fe(u.href);
-    if (!i.ok) throw new ee(i.status, await i.json());
-    return new Promise(async d => {
-        var p;
-        const f = new Map,
-            S = i.body.getReader(),
-            l = new TextDecoder;
-
-        function b(C) {
-            return vt(C, {
-                Promise: x => new Promise((k, N) => {
-                    f.set(x, {
-                        fulfil: k,
-                        reject: N
+async function Je(a, o) {
+    const l = new URL(a);
+    l.pathname = ot(a.pathname), l.searchParams.append(yt, o.map(m => m ? "1" : "0").join(""));
+    const c = await fe(l.href);
+    if (!c.ok) throw new ee(c.status, await c.json());
+    return new Promise(async m => {
+        var g;
+        const _ = new Map,
+            E = c.body.getReader(),
+            y = new TextDecoder;
+
+        function b(N) {
+            return Xe(N, {
+                Promise: j => new Promise((I, O) => {
+                    _.set(j, {
+                        fulfil: I,
+                        reject: O
                     })
                 })
             })
         }
-        let w = "";
+        let S = "";
         for (;;) {
             const {
-                done: C,
-                value: x
-            } = await S.read();
-            if (C && !w) break;
-            for (w += !x && w ? `
-` : l.decode(x);;) {
-                const k = w.indexOf(`
+                done: N,
+                value: j
+            } = await E.read();
+            if (N && !S) break;
+            for (S += !j && S ? `
+` : y.decode(j);;) {
+                const I = S.indexOf(`
 `);
-                if (k === -1) break;
-                const N = JSON.parse(w.slice(0, k));
-                if (w = w.slice(k + 1), N.type === "redirect") return d(N);
-                if (N.type === "data")(p = N.nodes) == null || p.forEach(P => {
+                if (I === -1) break;
+                const O = JSON.parse(S.slice(0, I));
+                if (S = S.slice(I + 1), O.type === "redirect") return m(O);
+                if (O.type === "data")(g = O.nodes) == null || g.forEach(P => {
                     (P == null ? void 0 : P.type) === "data" && (P.uses = Ge(P.uses), P.data = b(P.data))
-                }), d(N);
-                else if (N.type === "chunk") {
+                }), m(O);
+                else if (O.type === "chunk") {
                     const {
                         id: P,
                         data: B,
-                        error: H
-                    } = N, F = f.get(P);
-                    f.delete(P), H ? F.reject(b(H)) : F.fulfil(b(B))
+                        error: J
+                    } = O, M = _.get(P);
+                    _.delete(P), J ? M.reject(b(J)) : M.fulfil(b(B))
                 }
             }
         }
     })
 }
 
-function Ge(t) {
+function Ge(a) {
     return {
-        dependencies: new Set((t == null ? void 0 : t.dependencies) ?? []),
-        params: new Set((t == null ? void 0 : t.params) ?? []),
-        parent: !!(t != null && t.parent),
-        route: !!(t != null && t.route),
-        url: !!(t != null && t.url)
+        dependencies: new Set((a == null ? void 0 : a.dependencies) ?? []),
+        params: new Set((a == null ? void 0 : a.params) ?? []),
+        parent: !!(a != null && a.parent),
+        route: !!(a != null && a.route),
+        url: !!(a != null && a.url)
     }
 }
 
-function Ee() {
-    const t = document.querySelector("[autofocus]");
-    if (t) t.focus();
+function Se() {
+    const a = document.querySelector("[autofocus]");
+    if (a) a.focus();
     else {
         const o = document.body,
-            u = o.getAttribute("tabindex");
+            l = o.getAttribute("tabindex");
         o.tabIndex = -1, o.focus({
             preventScroll: !0,
             focusVisible: !1
-        }), u !== null ? o.setAttribute("tabindex", u) : o.removeAttribute("tabindex");
-        const i = getSelection();
-        if (i && i.type !== "None") {
-            const d = [];
-            for (let f = 0; f < i.rangeCount; f += 1) d.push(i.getRangeAt(f));
+        }), l !== null ? o.setAttribute("tabindex", l) : o.removeAttribute("tabindex");
+        const c = getSelection();
+        if (c && c.type !== "None") {
+            const m = [];
+            for (let _ = 0; _ < c.rangeCount; _ += 1) m.push(c.getRangeAt(_));
             setTimeout(() => {
-                if (i.rangeCount === d.length) {
-                    for (let f = 0; f < i.rangeCount; f += 1) {
-                        const S = d[f],
-                            l = i.getRangeAt(f);
-                        if (S.commonAncestorContainer !== l.commonAncestorContainer || S.startContainer !== l.startContainer || S.endContainer !== l.endContainer || S.startOffset !== l.startOffset || S.endOffset !== l.endOffset) return
+                if (c.rangeCount === m.length) {
+                    for (let _ = 0; _ < c.rangeCount; _ += 1) {
+                        const E = m[_],
+                            y = c.getRangeAt(_);
+                        if (E.commonAncestorContainer !== y.commonAncestorContainer || E.startContainer !== y.startContainer || E.endContainer !== y.endContainer || E.startOffset !== y.startOffset || E.endOffset !== y.endOffset) return
                     }
-                    i.removeAllRanges()
+                    c.removeAllRanges()
                 }
             })
         }
     }
 }
-async function Pt(t, o, u) {
-    const i = Rt(t, o);
-    We({
-        client: i
-    }), u ? await i._hydrate(u) : i.goto(location.href, {
+async function xt(a, o, l) {
+    const c = wt(a, o);
+    Ye({
+        client: c
+    }), l ? await c._hydrate(l) : c.goto(location.href, {
         replaceState: !0
-    }), i._start_router()
+    }), c._start_router()
 }
 export {
-    Pt as start
+    xt as start
 };
```

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/1.6c933e22.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/1.ed3af81f.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -11,18 +11,18 @@
     h as m,
     c as k,
     b as _,
     G as E,
     u as $,
     H as q,
     I as y
-} from "../chunks/index.6dba6488.js";
+} from "../chunks/index.8c237fac.js";
 import {
     p as C
-} from "../chunks/stores.57c5405b.js";
+} from "../chunks/stores.4b841c19.js";
 
 function G(l) {
     var f;
     let a, t = l[0].status + "",
         r, o, n, p = ((f = l[0].error) == null ? void 0 : f.message) + "",
         c;
     return {
```

### Comparing `scaneo-2023.5.29/scaneo/ui/_app/immutable/nodes/3.d433accd.js` & `scaneo-2023.5.29.post2/scaneo/ui/_app/immutable/nodes/3.35180ced.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -8,18 +8,18 @@
     m as f,
     r as g,
     h as i,
     b as x,
     G as y,
     H as r,
     I as b
-} from "../chunks/index.6dba6488.js";
+} from "../chunks/index.8c237fac.js";
 import {
     p as $
-} from "../chunks/stores.57c5405b.js";
+} from "../chunks/stores.4b841c19.js";
 
 function q(o) {
     let a, s;
     return {
         c() {
             a = u("p"), s = h("hola")
         },
```

### Comparing `scaneo-2023.5.29/scaneo/ui/favicon.png` & `scaneo-2023.5.29.post2/scaneo/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-2023.5.29/scaneo/ui/index.html` & `scaneo-2023.5.29.post2/scaneo/ui/kk/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="en" data-theme="light">
 	<head>
 		<meta charset="utf-8" />
-		<link rel="icon" href="./favicon.png" />
+		<link rel="icon" href="../favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		<meta http-equiv="content-security-policy" content="">
-		<link rel="modulepreload" href="./_app/immutable/entry/start.4cfa1304.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/index.6dba6488.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/singletons.9f3ec903.js">
-		<link rel="modulepreload" href="./_app/immutable/entry/app.b9b6597a.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/0.67f61f78.js">
-		<link rel="modulepreload" href="./_app/immutable/nodes/2.39aa7785.js">
-		<link rel="modulepreload" href="./_app/immutable/chunks/stores.57c5405b.js">
+		<link href="../_app/immutable/assets/0.cdaa43fa.css" rel="stylesheet">
+		<link rel="modulepreload" href="../_app/immutable/entry/start.dc4cd066.js">
+		<link rel="modulepreload" href="../_app/immutable/chunks/index.8c237fac.js">
+		<link rel="modulepreload" href="../_app/immutable/chunks/singletons.d791afcf.js">
+		<link rel="modulepreload" href="../_app/immutable/chunks/parse.bee59afc.js">
+		<link rel="modulepreload" href="../_app/immutable/entry/app.2b7d5976.js">
+		<link rel="modulepreload" href="../_app/immutable/chunks/preload-helper.41c905a7.js">
+		<link rel="modulepreload" href="../_app/immutable/nodes/0.2bbf402e.js">
+		<link rel="modulepreload" href="../_app/immutable/nodes/3.35180ced.js">
+		<link rel="modulepreload" href="../_app/immutable/chunks/stores.4b841c19.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 
 
-<h1>Welcome to SCANEO</h1>
-<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
-<a href="/kk">hola</a>
+<p>hola</p>
 
 
 			
 			<script>
 				{
-					__sveltekit_1704jlc = {
-						base: new URL(".", location).pathname.slice(0, -1),
+					__sveltekit_1norjlf = {
+						base: new URL("..", location).pathname.slice(0, -1),
 						env: {"PUBLIC_API_URL":""}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					const data = [null,null];
 
 					Promise.all([
-						import("./_app/immutable/entry/start.4cfa1304.js"),
-						import("./_app/immutable/entry/app.b9b6597a.js")
+						import("../_app/immutable/entry/start.dc4cd066.js"),
+						import("../_app/immutable/entry/app.2b7d5976.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element, {
-							node_ids: [0, 2],
+							node_ids: [0, 3],
 							data,
 							form: null,
 							error: null
 						});
 					});
 				}
 			</script>
```

#### html2text {}

```diff
@@ -4,10 +4,11 @@
 
 
 
 
 
 
 
-****** Welcome to SCANEO ******
-Visit kit.svelte.dev to read the documentation
+
+
+
 hola
```

### Comparing `scaneo-2023.5.29/setup.py` & `scaneo-2023.5.29.post2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 packages = \
 ['scaneo', 'scaneo.cli', 'scaneo.routers']
 
 package_data = \
 {'': ['*'],
  'scaneo': ['ui/*',
             'ui/_app/*',
+            'ui/_app/immutable/assets/*',
             'ui/_app/immutable/chunks/*',
             'ui/_app/immutable/entry/*',
             'ui/_app/immutable/nodes/*',
+            'ui/icons/*',
             'ui/kk/*']}
 
 entry_points = \
 {'console_scripts': ['scaneo = scaneo.main:app']}
 
 setup_kwargs = {
     'name': 'scaneo',
-    'version': '2023.5.29',
+    'version': '2023.5.29.post2',
     'description': '',
     'long_description': '# scan\n\nThis repo contains the code for SCAN\n\n- scaneo: includes the cli, lib and api\n- ui: includes the web ui\n\nThe CLI runs the API, which in turns servers the static files for the UI.\n\nThe library can be installed with \n\n```\npip install scaneo\n```\t\n\n## Instructions\n\n### Developement\n\nRun the api with the cli\n\n```\ncd scaneo\npython main.py\n```\n\nThen, run the ui\n\n```\ncd ui\nyarn dev\n```\n\n### Production\n\nBuild the ui, copy the build inside scaneo and build the python package\n\n```\nmake build v=<version>\nmake publish\n```\n\n## Notes\n\nDo not add scaneo/ui to gitignore since the build process will fail (missing entry folder)',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scaneo-2023.5.29/PKG-INFO` & `scaneo-2023.5.29.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaneo
-Version: 2023.5.29
+Version: 2023.5.29.post2
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


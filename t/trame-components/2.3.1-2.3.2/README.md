# Comparing `tmp/trame-components-2.3.1.tar.gz` & `tmp/trame-components-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-components-2.3.1.tar", last modified: Wed Apr 17 20:45:11 2024, max compression
+gzip compressed data, was "trame-components-2.3.2.tar", last modified: Tue Apr 23 22:15:27 2024, max compression
```

## Comparing `trame-components-2.3.1.tar` & `trame-components-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.239639 trame-components-2.3.1/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-17 20:44:54.000000 trame-components-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-17 20:44:54.000000 trame-components-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-17 20:45:11.239639 trame-components-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2024-04-17 20:44:54.000000 trame-components-2.3.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-17 20:45:11.239639 trame-components-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:44:54.000000 trame-components-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/modules/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/module/
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components/module/serve/
--rw-r--r--   0 root         (0) root         (0)   227297 2024-04-17 20:45:07.000000 trame-components-2.3.1/trame_components/module/serve/trame-components.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.239639 trame-components-2.3.1/trame_components/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15929 2024-04-17 20:44:54.000000 trame-components-2.3.1/trame_components/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:45:11.235639 trame-components-2.3.1/trame_components.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-17 20:45:11.000000 trame-components-2.3.1/trame_components.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-23 22:15:11.000000 trame-components-2.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-23 22:15:11.000000 trame-components-2.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-23 22:15:27.411965 trame-components-2.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-23 22:15:11.000000 trame-components-2.3.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-23 22:15:27.411965 trame-components-2.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 22:15:11.000000 trame-components-2.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.407965 trame-components-2.3.2/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame/modules/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame_components/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame_components/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame_components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame_components/module/
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame_components/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame_components/module/serve/
+-rw-r--r--   0 root         (0) root         (0)   226858 2024-04-23 22:15:23.000000 trame-components-2.3.2/trame_components/module/serve/trame-components.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame_components/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame_components/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2024-04-23 22:15:11.000000 trame-components-2.3.2/trame_components/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:15:27.411965 trame-components-2.3.2/trame_components.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-23 22:15:27.000000 trame-components-2.3.2/trame_components.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-23 22:15:27.000000 trame-components-2.3.2/trame_components.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 22:15:27.000000 trame-components-2.3.2/trame_components.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-23 22:15:27.000000 trame-components-2.3.2/trame_components.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-23 22:15:27.000000 trame-components-2.3.2/trame_components.egg-info/top_level.txt
```

### Comparing `trame-components-2.3.1/LICENSE` & `trame-components-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.1/PKG-INFO` & `trame-components-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.3.1
+Version: 2.3.2
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.3.1/README.rst` & `trame-components-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.1/setup.cfg` & `trame-components-2.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-components
-version = 2.3.1
+version = 2.3.2
 description = Core components for trame widgets
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-components-2.3.1/trame_components/LICENSE` & `trame-components-2.3.2/trame_components/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.3.1/trame_components/module/serve/trame-components.umd.js` & `trame-components-2.3.2/trame_components/module/serve/trame-components.umd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
-(function(b0, k0) {
-    typeof exports == "object" && typeof module < "u" ? k0(exports) : typeof define == "function" && define.amd ? define(["exports"], k0) : (b0 = typeof globalThis < "u" ? globalThis : b0 || self, k0(b0.trame_components = {}))
-})(this, function(b0) {
+(function(w0, k0) {
+    typeof exports == "object" && typeof module < "u" ? k0(exports) : typeof define == "function" && define.amd ? define(["exports"], k0) : (w0 = typeof globalThis < "u" ? globalThis : w0 || self, k0(w0.trame_components = {}))
+})(this, function(w0) {
     "use strict";
     const {
         watch: k0,
         nextTick: s9
     } = window.Vue, c9 = {
         props: {
             value: {
@@ -290,15 +290,15 @@
     function V1(e, t, r) {
         const n = e.tree[t.id];
         t.x = r, t.y = e.y, e.y += 1, e.nodes.push(t), !n || n.length === 0 ? e.leaves.push(t) : (n.sort(F1), n.forEach((a, o) => {
             V1(e, a, r + n.length - (o + 1))
         }))
     }
 
-    function x9(e, t) {
+    function R9(e, t) {
         const {
             x: r,
             y: n
         } = t, {
             rootId: a,
             map: o,
             branches: c,
@@ -314,15 +314,15 @@
             y: o[i.parent].y,
             toX: i.x,
             toY: i.y,
             color: i.color
         })
     }
 
-    function R9(e, t = []) {
+    function x9(e, t = []) {
         const {
             nodes: r,
             actives: n
         } = e;
         r.forEach(a => {
             t.indexOf(a.id) !== -1 && n.push(a.y)
         })
@@ -337,15 +337,15 @@
             } = n,
             {
                 nodes: s,
                 branches: u,
                 forks: i,
                 actives: f
             } = n;
-        return a[c].forEach(g => V1(n, g, 0)), R9(n, t), o.forEach(g => x9(n, g)), i.sort((g, l) => g.toX > l.toX), {
+        return a[c].forEach(g => V1(n, g, 0)), x9(n, t), o.forEach(g => R9(n, g)), i.sort((g, l) => g.toX > l.toX), {
             nodes: s,
             branches: u,
             forks: i,
             actives: f,
             leaves: o
         }
     }
@@ -454,111 +454,111 @@
                     s = D0([]);
 
                 function u() {
                     const {
                         nodes: h,
                         branches: C,
                         forks: N,
-                        actives: x
+                        actives: R
                     } = O9(e.sources, e.actives, e.rootId);
-                    a.value = h, o.value = C, c.value = N, s.value = x
+                    a.value = h, o.value = C, c.value = N, s.value = R
                 }
 
                 function i(h) {
                     const {
                         actives: C,
                         deltaY: N,
-                        multiselect: x
+                        multiselect: R
                     } = e, B = C.slice();
                     if (h.target.nodeName !== "circle") {
-                        const b = n.value.getClientRects()[0],
-                            S = b.y || b.top,
-                            w = Math.floor((h.clientY - S) / N),
-                            v = C.indexOf(w);
-                        x && (h.metaKey || h.ctrlKey) ? (v === -1 ? B.push(w) : B.splice(v, 1), s.value = B, t("activesChange", s.value.map(d => a.value[d].id))) : (B[0] = w, s.value = B, t("activesChange", s.value.map(d => a.value[d].id)))
+                        const w = n.value.getClientRects()[0],
+                            S = w.y || w.top,
+                            b = Math.floor((h.clientY - S) / N),
+                            v = C.indexOf(b);
+                        R && (h.metaKey || h.ctrlKey) ? (v === -1 ? B.push(b) : B.splice(v, 1), s.value = B, t("activesChange", s.value.map(d => a.value[d].id))) : (B[0] = b, s.value = B, t("activesChange", s.value.map(d => a.value[d].id)))
                     }
                 }
 
                 function f(h) {
                     const C = parseInt(h.currentTarget.dataset.id, 10),
                         N = Object.assign({}, a.value[C]);
-                    N.visible = !N.visible, a.value = a.value.map((x, B) => B === C ? N : x), t("visibilityChange", {
+                    N.visible = !N.visible, a.value = a.value.map((R, B) => B === C ? N : R), t("visibilityChange", {
                         id: N.id,
                         visible: N.visible
                     })
                 }
 
                 function g(h) {
                     const C = parseInt(h.currentTarget.dataset.id, 10),
                         N = h.currentTarget.dataset.name,
                         {
-                            id: x
+                            id: R
                         } = a.value[C];
                     t("action", {
-                        id: x,
+                        id: R,
                         action: N
                     })
                 }
                 U1(() => e.sources, u), U1(() => e.actives, u);
                 const l = t1(() => o.value.map((h, C) => {
                         const N = e.deltaX * h.x + e.offset,
-                            x = e.deltaY * h.y + e.deltaY / 2,
+                            R = e.deltaY * h.y + e.deltaY / 2,
                             B = e.deltaY * h.to + e.deltaY / 2,
-                            b = h.color || e.palette[h.x % e.palette.length];
+                            w = h.color || e.palette[h.x % e.palette.length];
                         return {
                             key: `branch-${C}`,
-                            d: `M${N},${x} L${N},${B}`,
-                            stroke: b
+                            d: `M${N},${R} L${N},${B}`,
+                            stroke: w
                         }
                     })),
                     p = t1(() => c.value.map((h, C) => {
                         const N = e.deltaX * h.x + e.offset,
-                            x = e.deltaY * h.y + e.deltaY / 2 + e.radius,
+                            R = e.deltaY * h.y + e.deltaY / 2 + e.radius,
                             B = e.deltaX * h.toX + e.offset,
-                            b = e.deltaY * h.toY + e.deltaY / 2 + e.radius,
+                            w = e.deltaY * h.toY + e.deltaY / 2 + e.radius,
                             S = h.color || e.palette[h.toX % e.palette.length],
-                            w = `M${N},${x} Q${N},${x+e.deltaY/3},${(N+B)/2},${x+e.deltaY/3} T${B},${x+e.deltaY} L${B},${b}`;
+                            b = `M${N},${R} Q${N},${R+e.deltaY/3},${(N+B)/2},${R+e.deltaY/3} T${B},${R+e.deltaY} L${B},${w}`;
                         return {
                             key: `fork-${C}`,
-                            d: w,
+                            d: b,
                             stroke: S
                         }
                     })),
                     y = t1(() => a.value.map((h, C) => {
                         const N = s.value.includes(C),
-                            x = !!h.visible,
+                            R = !!h.visible,
                             B = h.color || e.palette[h.x % e.palette.length],
-                            b = e.textColor[N ? 1 : 0],
+                            w = e.textColor[N ? 1 : 0],
                             S = e.textWeight[N ? 1 : 0],
-                            w = N ? e.activeCircleStrokeColor : B || B,
-                            v = x ? B : e.notVisibleCircleFillColor || B,
+                            b = N ? e.activeCircleStrokeColor : B || B,
+                            v = R ? B : e.notVisibleCircleFillColor || B,
                             d = e.deltaX * h.x + e.offset,
                             m = e.deltaY * h.y + e.deltaY / 2,
-                            O = d + e.radius * 2,
+                            T = d + e.radius * 2,
                             D = m + (e.radius - 1),
-                            _ = (h.actions || []).map(T9(e.deltaY * h.y, e.width, e.deltaY, e.actionSize, e.actionMap));
+                            P = (h.actions || []).map(T9(e.deltaY * h.y, e.width, e.deltaY, e.actionSize, e.actionMap));
                         return {
                             key: `node-${C}`,
                             id: h.y,
                             circle: {
                                 cx: d,
                                 cy: m,
                                 radius: e.radius,
-                                stroke: w,
+                                stroke: b,
                                 fill: v
                             },
                             text: {
-                                x: O,
+                                x: T,
                                 y: D,
-                                fill: b,
+                                fill: w,
                                 fontWeight: S,
                                 fontSize: e.fontSize,
                                 content: h.name
                             },
-                            actions: _
+                            actions: P
                         }
                     }));
                 return N9(u), r({
                     toggleActive: i,
                     toggleVisibility: f,
                     triggerAction: g
                 }), {
@@ -865,15 +865,15 @@
             >
               ${L9}
             </v-list-item>
         </v-list>
     </v-col>
     `
         };
-    var e0 = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+    var Q = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
     function _9(e) {
         if (e.__esModule) return e;
         var t = e.default;
         if (typeof t == "function") {
             var r = function n() {
                 if (this instanceof n) {
@@ -1029,189 +1029,189 @@
                 if (!u) {
                     u = {};
                     for (var v in a) v > 95 && v < 112 || a.hasOwnProperty(v) && (u[a[v]] = v)
                 }
                 return u
             }
 
-            function x(v, d, m) {
+            function R(v, d, m) {
                 return m || (m = N()[v] ? "keydown" : "keypress"), m == "keypress" && d.length && (m = "keydown"), m
             }
 
             function B(v) {
                 return v === "+" ? ["+"] : (v = v.replace(/\+{2}/g, "+plus"), v.split("+"))
             }
 
-            function b(v, d) {
-                var m, O, D, _ = [];
-                for (m = B(v), D = 0; D < m.length; ++D) O = m[D], s[O] && (O = s[O]), d && d != "keypress" && c[O] && (O = c[O], _.push("shift")), C(O) && _.push(O);
-                return d = x(O, _, d), {
-                    key: O,
-                    modifiers: _,
+            function w(v, d) {
+                var m, T, D, P = [];
+                for (m = B(v), D = 0; D < m.length; ++D) T = m[D], s[T] && (T = s[T]), d && d != "keypress" && c[T] && (T = c[T], P.push("shift")), C(T) && P.push(T);
+                return d = R(T, P, d), {
+                    key: T,
+                    modifiers: P,
                     action: d
                 }
             }
 
             function S(v, d) {
                 return v === null || v === r ? !1 : v === d ? !0 : S(v.parentNode, d)
             }
 
-            function w(v) {
+            function b(v) {
                 var d = this;
-                if (v = v || r, !(d instanceof w)) return new w(v);
+                if (v = v || r, !(d instanceof b)) return new b(v);
                 d.target = v, d._callbacks = {}, d._directMap = {};
                 var m = {},
-                    O, D = !1,
-                    _ = !1,
-                    U = !1;
+                    T, D = !1,
+                    P = !1,
+                    F = !1;
 
-                function F(M) {
+                function _(M) {
                     M = M || {};
                     var E = !1,
-                        A;
-                    for (A in m) {
-                        if (M[A]) {
+                        L;
+                    for (L in m) {
+                        if (M[L]) {
                             E = !0;
                             continue
                         }
-                        m[A] = 0
+                        m[L] = 0
                     }
-                    E || (U = !1)
+                    E || (F = !1)
                 }
 
-                function T(M, E, A, k, $, Z) {
-                    var P, j, Y = [],
-                        X = A.type;
+                function x(M, E, L, k, $, J) {
+                    var A, U, Y = [],
+                        X = L.type;
                     if (!d._callbacks[M]) return [];
-                    for (X == "keyup" && C(M) && (E = [M]), P = 0; P < d._callbacks[M].length; ++P)
-                        if (j = d._callbacks[M][P], !(!k && j.seq && m[j.seq] != j.level) && X == j.action && (X == "keypress" && !A.metaKey && !A.ctrlKey || l(E, j.modifiers))) {
-                            var l0 = !k && j.combo == $,
-                                f0 = k && j.seq == k && j.level == Z;
-                            (l0 || f0) && d._callbacks[M].splice(P, 1), Y.push(j)
+                    for (X == "keyup" && C(M) && (E = [M]), A = 0; A < d._callbacks[M].length; ++A)
+                        if (U = d._callbacks[M][A], !(!k && U.seq && m[U.seq] != U.level) && X == U.action && (X == "keypress" && !L.metaKey && !L.ctrlKey || l(E, U.modifiers))) {
+                            var s0 = !k && U.combo == $,
+                                c0 = k && U.seq == k && U.level == J;
+                            (s0 || c0) && d._callbacks[M].splice(A, 1), Y.push(U)
                         } return Y
                 }
 
-                function L(M, E, A, k) {
-                    d.stopCallback(E, E.target || E.srcElement, A, k) || M(E, A) === !1 && (y(E), h(E))
+                function j(M, E, L, k) {
+                    d.stopCallback(E, E.target || E.srcElement, L, k) || M(E, L) === !1 && (y(E), h(E))
                 }
-                d._handleKey = function(M, E, A) {
-                    var k = T(M, E, A),
-                        $, Z = {},
-                        P = 0,
-                        j = !1;
-                    for ($ = 0; $ < k.length; ++$) k[$].seq && (P = Math.max(P, k[$].level));
+                d._handleKey = function(M, E, L) {
+                    var k = x(M, E, L),
+                        $, J = {},
+                        A = 0,
+                        U = !1;
+                    for ($ = 0; $ < k.length; ++$) k[$].seq && (A = Math.max(A, k[$].level));
                     for ($ = 0; $ < k.length; ++$) {
                         if (k[$].seq) {
-                            if (k[$].level != P) continue;
-                            j = !0, Z[k[$].seq] = 1, L(k[$].callback, A, k[$].combo, k[$].seq);
+                            if (k[$].level != A) continue;
+                            U = !0, J[k[$].seq] = 1, j(k[$].callback, L, k[$].combo, k[$].seq);
                             continue
                         }
-                        j || L(k[$].callback, A, k[$].combo)
+                        U || j(k[$].callback, L, k[$].combo)
                     }
-                    var Y = A.type == "keypress" && _;
-                    A.type == U && !C(M) && !Y && F(Z), _ = j && A.type == "keydown"
+                    var Y = L.type == "keypress" && P;
+                    L.type == F && !C(M) && !Y && _(J), P = U && L.type == "keydown"
                 };
 
                 function V(M) {
                     typeof M.which != "number" && (M.which = M.keyCode);
                     var E = g(M);
                     if (E) {
                         if (M.type == "keyup" && D === E) {
                             D = !1;
                             return
                         }
                         d.handleKey(E, p(M), M)
                     }
                 }
 
-                function Q() {
-                    clearTimeout(O), O = setTimeout(F, 1e3)
+                function e0() {
+                    clearTimeout(T), T = setTimeout(_, 1e3)
                 }
 
-                function K(M, E, A, k) {
+                function E0(M, E, L, k) {
                     m[M] = 0;
 
                     function $(X) {
                         return function() {
-                            U = X, ++m[M], Q()
+                            F = X, ++m[M], e0()
                         }
                     }
 
-                    function Z(X) {
-                        L(A, X, M), k !== "keyup" && (D = g(X)), setTimeout(F, 10)
+                    function J(X) {
+                        j(L, X, M), k !== "keyup" && (D = g(X)), setTimeout(_, 10)
                     }
-                    for (var P = 0; P < E.length; ++P) {
-                        var j = P + 1 === E.length,
-                            Y = j ? Z : $(k || b(E[P + 1]).action);
-                        a0(E[P], Y, k, M, P)
+                    for (var A = 0; A < E.length; ++A) {
+                        var U = A + 1 === E.length,
+                            Y = U ? J : $(k || w(E[A + 1]).action);
+                        C0(E[A], Y, k, M, A)
                     }
                 }
 
-                function a0(M, E, A, k, $) {
-                    d._directMap[M + ":" + A] = E, M = M.replace(/\s+/g, " ");
-                    var Z = M.split(" "),
-                        P;
-                    if (Z.length > 1) {
-                        K(M, Z, E, A);
+                function C0(M, E, L, k, $) {
+                    d._directMap[M + ":" + L] = E, M = M.replace(/\s+/g, " ");
+                    var J = M.split(" "),
+                        A;
+                    if (J.length > 1) {
+                        E0(M, J, E, L);
                         return
                     }
-                    P = b(M, A), d._callbacks[P.key] = d._callbacks[P.key] || [], T(P.key, P.modifiers, {
-                        type: P.action
-                    }, k, M, $), d._callbacks[P.key][k ? "unshift" : "push"]({
+                    A = w(M, L), d._callbacks[A.key] = d._callbacks[A.key] || [], x(A.key, A.modifiers, {
+                        type: A.action
+                    }, k, M, $), d._callbacks[A.key][k ? "unshift" : "push"]({
                         callback: E,
-                        modifiers: P.modifiers,
-                        action: P.action,
+                        modifiers: A.modifiers,
+                        action: A.action,
                         seq: k,
                         level: $,
                         combo: M
                     })
                 }
-                d._bindMultiple = function(M, E, A) {
-                    for (var k = 0; k < M.length; ++k) a0(M[k], E, A)
+                d._bindMultiple = function(M, E, L) {
+                    for (var k = 0; k < M.length; ++k) C0(M[k], E, L)
                 }, f(v, "keypress", V), f(v, "keydown", V), f(v, "keyup", V)
             }
-            w.prototype.bind = function(v, d, m) {
-                var O = this;
-                return v = v instanceof Array ? v : [v], O._bindMultiple.call(O, v, d, m), O
-            }, w.prototype.unbind = function(v, d) {
+            b.prototype.bind = function(v, d, m) {
+                var T = this;
+                return v = v instanceof Array ? v : [v], T._bindMultiple.call(T, v, d, m), T
+            }, b.prototype.unbind = function(v, d) {
                 var m = this;
                 return m.bind.call(m, v, function() {}, d)
-            }, w.prototype.trigger = function(v, d) {
+            }, b.prototype.trigger = function(v, d) {
                 var m = this;
                 return m._directMap[v + ":" + d] && m._directMap[v + ":" + d]({}, v), m
-            }, w.prototype.reset = function() {
+            }, b.prototype.reset = function() {
                 var v = this;
                 return v._callbacks = {}, v._directMap = {}, v
-            }, w.prototype.stopCallback = function(v, d) {
+            }, b.prototype.stopCallback = function(v, d) {
                 var m = this;
                 if ((" " + d.className + " ").indexOf(" mousetrap ") > -1 || S(d, m.target)) return !1;
                 if ("composedPath" in v && typeof v.composedPath == "function") {
-                    var O = v.composedPath()[0];
-                    O !== v.target && (d = O)
+                    var T = v.composedPath()[0];
+                    T !== v.target && (d = T)
                 }
                 return d.tagName == "INPUT" || d.tagName == "SELECT" || d.tagName == "TEXTAREA" || d.isContentEditable
-            }, w.prototype.handleKey = function() {
+            }, b.prototype.handleKey = function() {
                 var v = this;
                 return v._handleKey.apply(v, arguments)
-            }, w.addKeycodes = function(v) {
+            }, b.addKeycodes = function(v) {
                 for (var d in v) v.hasOwnProperty(d) && (a[d] = v[d]);
                 u = null
-            }, w.init = function() {
-                var v = w(r);
-                for (var d in v) d.charAt(0) !== "_" && (w[d] = function(m) {
+            }, b.init = function() {
+                var v = b(r);
+                for (var d in v) d.charAt(0) !== "_" && (b[d] = function(m) {
                     return function() {
                         return v[m].apply(v, arguments)
                     }
                 }(d))
-            }, w.init(), t.Mousetrap = w, e.exports && (e.exports = w), typeof n == "function" && n.amd && n(function() {
-                return w
+            }, b.init(), t.Mousetrap = b, e.exports && (e.exports = b), typeof n == "function" && n.amd && n(function() {
+                return b
             })
         })(typeof window < "u" ? window : null, typeof window < "u" ? document : null)
     })($9);
-    const p0 = n1,
+    const f0 = n1,
         {
             watch: j9,
             onBeforeUnmount: U9
         } = window.Vue,
         F9 = {
             inject: ["trame"],
             props: {
@@ -1222,41 +1222,41 @@
             emits: [],
             setup(e, {
                 emit: t,
                 expose: r
             }) {
                 const n = {
                     bind(...o) {
-                        p0.bind(...o)
+                        f0.bind(...o)
                     },
                     unbind(o) {
-                        p0.unbind(o)
+                        f0.unbind(o)
                     },
                     trigger(o) {
-                        p0.trigger(o)
+                        f0.trigger(o)
                     },
                     addKeycodes(...o) {
-                        p0.trigger(...o)
+                        f0.trigger(...o)
                     }
                 };
 
                 function a() {
-                    e.mapping && (p0.reset(), e.mapping.forEach(({
+                    e.mapping && (f0.reset(), e.mapping.forEach(({
                         keys: o,
                         event: c,
                         stop: s,
                         listen: u
                     }) => {
-                        p0.bind(o, i => {
+                        f0.bind(o, i => {
                             if (t(c, i), s) return !1
                         }, u)
                     }))
                 }
                 return a(), j9(e.mapping, a), U9(() => {
-                    p0.reset()
+                    f0.reset()
                 }), r(n), n
             }
         },
         {
             inject: V9,
             ref: z9,
             onMounted: H9,
@@ -1302,15 +1302,15 @@
                     elem: n,
                     resize: a
                 }
             },
             template: '<div ref="elem" style="overflow: hidden; position: relative; width: 100%; height: 100%; margin: 0; padding: 0;"><slot></slot></div>'
         };
 
-    function v0(e, t, r) {
+    function g0(e, t, r) {
         return t in e ? Object.defineProperty(e, t, {
             value: r,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = r, e
     }
@@ -1357,24 +1357,24 @@
     }
 
     function q9() {
         throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
     }
 
-    function u0(e, t) {
+    function o0(e, t) {
         return Y9(e) || X9(e, t) || W1(e, t) || q9()
     }
 
-    function y0(e) {
-        return y0 = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
+    function p0(e) {
+        return p0 = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
             return typeof t
         } : function(t) {
             return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-        }, y0(e)
+        }, p0(e)
     }
 
     function K9(e) {
         if (Array.isArray(e)) return a1(e)
     }
 
     function J9(e) {
@@ -1488,26 +1488,26 @@
                     }
                 };
             e = function(p) {
                 var y = p !== null && typeof p == "object",
                     h = r.call(p) === "[object Function]",
                     C = n(p),
                     N = y && r.call(p) === "[object String]",
-                    x = [];
+                    R = [];
                 if (!y && !h && !C) throw new TypeError("Object.keys called on a non-object");
                 var B = c && h;
                 if (N && p.length > 0 && !t.call(p, 0))
-                    for (var b = 0; b < p.length; ++b) x.push(String(b));
+                    for (var w = 0; w < p.length; ++w) R.push(String(w));
                 if (C && p.length > 0)
-                    for (var S = 0; S < p.length; ++S) x.push(String(S));
+                    for (var S = 0; S < p.length; ++S) R.push(String(S));
                 else
-                    for (var w in p) !(B && w === "prototype") && t.call(p, w) && x.push(String(w));
+                    for (var b in p) !(B && b === "prototype") && t.call(p, b) && R.push(String(b));
                 if (o)
-                    for (var v = g(p), d = 0; d < s.length; ++d) !(v && s[d] === "constructor") && t.call(p, s[d]) && x.push(s[d]);
-                return x
+                    for (var v = g(p), d = 0; d < s.length; ++d) !(v && s[d] === "constructor") && t.call(p, s[d]) && R.push(s[d]);
+                return R
             }
         }
         return i1 = e, i1
     }
     var t5 = Array.prototype.slice,
         r5 = X1,
         K1 = Object.keys,
@@ -1583,54 +1583,54 @@
             }
             return a
         },
         p5 = g5,
         e2 = Function.prototype.bind || p5,
         v5 = e2,
         y5 = v5.call(Function.call, Object.prototype.hasOwnProperty),
-        G, N0 = SyntaxError,
+        G, b0 = SyntaxError,
         t2 = Function,
-        B0 = TypeError,
+        N0 = TypeError,
         s1 = function(e) {
             try {
                 return t2('"use strict"; return (' + e + ").constructor;")()
             } catch {}
         },
-        d0 = Object.getOwnPropertyDescriptor;
-    if (d0) try {
-        d0({}, "")
+        v0 = Object.getOwnPropertyDescriptor;
+    if (v0) try {
+        v0({}, "")
     } catch {
-        d0 = null
+        v0 = null
     }
     var c1 = function() {
-            throw new B0
+            throw new N0
         },
-        d5 = d0 ? function() {
+        d5 = v0 ? function() {
             try {
                 return arguments.callee, c1
             } catch {
                 try {
-                    return d0(arguments, "callee").get
+                    return v0(arguments, "callee").get
                 } catch {
                     return c1
                 }
             }
         }() : c1,
-        x0 = i5(),
+        B0 = i5(),
         h5 = s5(),
         z = Object.getPrototypeOf || (h5 ? function(e) {
             return e.__proto__
         } : null),
         R0 = {},
         m5 = typeof Uint8Array > "u" || !z ? G : z(Uint8Array),
-        h0 = {
+        y0 = {
             "%AggregateError%": typeof AggregateError > "u" ? G : AggregateError,
             "%Array%": Array,
             "%ArrayBuffer%": typeof ArrayBuffer > "u" ? G : ArrayBuffer,
-            "%ArrayIteratorPrototype%": x0 && z ? z([][Symbol.iterator]()) : G,
+            "%ArrayIteratorPrototype%": B0 && z ? z([][Symbol.iterator]()) : G,
             "%AsyncFromSyncIteratorPrototype%": G,
             "%AsyncFunction%": R0,
             "%AsyncGenerator%": R0,
             "%AsyncGeneratorFunction%": R0,
             "%AsyncIteratorPrototype%": R0,
             "%Atomics%": typeof Atomics > "u" ? G : Atomics,
             "%BigInt%": typeof BigInt > "u" ? G : BigInt,
@@ -1652,67 +1652,67 @@
             "%Function%": t2,
             "%GeneratorFunction%": R0,
             "%Int8Array%": typeof Int8Array > "u" ? G : Int8Array,
             "%Int16Array%": typeof Int16Array > "u" ? G : Int16Array,
             "%Int32Array%": typeof Int32Array > "u" ? G : Int32Array,
             "%isFinite%": isFinite,
             "%isNaN%": isNaN,
-            "%IteratorPrototype%": x0 && z ? z(z([][Symbol.iterator]())) : G,
+            "%IteratorPrototype%": B0 && z ? z(z([][Symbol.iterator]())) : G,
             "%JSON%": typeof JSON == "object" ? JSON : G,
             "%Map%": typeof Map > "u" ? G : Map,
-            "%MapIteratorPrototype%": typeof Map > "u" || !x0 || !z ? G : z(new Map()[Symbol.iterator]()),
+            "%MapIteratorPrototype%": typeof Map > "u" || !B0 || !z ? G : z(new Map()[Symbol.iterator]()),
             "%Math%": Math,
             "%Number%": Number,
             "%Object%": Object,
             "%parseFloat%": parseFloat,
             "%parseInt%": parseInt,
             "%Promise%": typeof Promise > "u" ? G : Promise,
             "%Proxy%": typeof Proxy > "u" ? G : Proxy,
             "%RangeError%": RangeError,
             "%ReferenceError%": ReferenceError,
             "%Reflect%": typeof Reflect > "u" ? G : Reflect,
             "%RegExp%": RegExp,
             "%Set%": typeof Set > "u" ? G : Set,
-            "%SetIteratorPrototype%": typeof Set > "u" || !x0 || !z ? G : z(new Set()[Symbol.iterator]()),
+            "%SetIteratorPrototype%": typeof Set > "u" || !B0 || !z ? G : z(new Set()[Symbol.iterator]()),
             "%SharedArrayBuffer%": typeof SharedArrayBuffer > "u" ? G : SharedArrayBuffer,
             "%String%": String,
-            "%StringIteratorPrototype%": x0 && z ? z("" [Symbol.iterator]()) : G,
-            "%Symbol%": x0 ? Symbol : G,
-            "%SyntaxError%": N0,
+            "%StringIteratorPrototype%": B0 && z ? z("" [Symbol.iterator]()) : G,
+            "%Symbol%": B0 ? Symbol : G,
+            "%SyntaxError%": b0,
             "%ThrowTypeError%": d5,
             "%TypedArray%": m5,
-            "%TypeError%": B0,
+            "%TypeError%": N0,
             "%Uint8Array%": typeof Uint8Array > "u" ? G : Uint8Array,
             "%Uint8ClampedArray%": typeof Uint8ClampedArray > "u" ? G : Uint8ClampedArray,
             "%Uint16Array%": typeof Uint16Array > "u" ? G : Uint16Array,
             "%Uint32Array%": typeof Uint32Array > "u" ? G : Uint32Array,
             "%URIError%": URIError,
             "%WeakMap%": typeof WeakMap > "u" ? G : WeakMap,
             "%WeakRef%": typeof WeakRef > "u" ? G : WeakRef,
             "%WeakSet%": typeof WeakSet > "u" ? G : WeakSet
         };
     if (z) try {
         null.error
     } catch (e) {
         var C5 = z(z(e));
-        h0["%Error.prototype%"] = C5
+        y0["%Error.prototype%"] = C5
     }
     var S5 = function e(t) {
             var r;
             if (t === "%AsyncFunction%") r = s1("async function () {}");
             else if (t === "%GeneratorFunction%") r = s1("function* () {}");
             else if (t === "%AsyncGeneratorFunction%") r = s1("async function* () {}");
             else if (t === "%AsyncGenerator%") {
                 var n = e("%AsyncGeneratorFunction%");
                 n && (r = n.prototype)
             } else if (t === "%AsyncIteratorPrototype%") {
                 var a = e("%AsyncGenerator%");
                 a && z && (r = z(a.prototype))
             }
-            return h0[t] = r, r
+            return y0[t] = r, r
         },
         r2 = {
             "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
             "%ArrayPrototype%": ["Array", "prototype"],
             "%ArrayProto_entries%": ["Array", "prototype", "entries"],
             "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
             "%ArrayProto_keys%": ["Array", "prototype", "keys"],
@@ -1767,67 +1767,67 @@
         F0 = y5,
         w5 = _0.call(Function.call, Array.prototype.concat),
         b5 = _0.call(Function.apply, Array.prototype.splice),
         n2 = _0.call(Function.call, String.prototype.replace),
         V0 = _0.call(Function.call, String.prototype.slice),
         N5 = _0.call(Function.call, RegExp.prototype.exec),
         B5 = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
-        x5 = /\\(\\)?/g,
-        R5 = function(t) {
+        R5 = /\\(\\)?/g,
+        x5 = function(t) {
             var r = V0(t, 0, 1),
                 n = V0(t, -1);
-            if (r === "%" && n !== "%") throw new N0("invalid intrinsic syntax, expected closing `%`");
-            if (n === "%" && r !== "%") throw new N0("invalid intrinsic syntax, expected opening `%`");
+            if (r === "%" && n !== "%") throw new b0("invalid intrinsic syntax, expected closing `%`");
+            if (n === "%" && r !== "%") throw new b0("invalid intrinsic syntax, expected opening `%`");
             var a = [];
             return n2(t, B5, function(o, c, s, u) {
-                a[a.length] = s ? n2(u, x5, "$1") : c || o
+                a[a.length] = s ? n2(u, R5, "$1") : c || o
             }), a
         },
         O5 = function(t, r) {
             var n = t,
                 a;
-            if (F0(r2, n) && (a = r2[n], n = "%" + a[0] + "%"), F0(h0, n)) {
-                var o = h0[n];
-                if (o === R0 && (o = S5(n)), typeof o > "u" && !r) throw new B0("intrinsic " + t + " exists, but is not available. Please file an issue!");
+            if (F0(r2, n) && (a = r2[n], n = "%" + a[0] + "%"), F0(y0, n)) {
+                var o = y0[n];
+                if (o === R0 && (o = S5(n)), typeof o > "u" && !r) throw new N0("intrinsic " + t + " exists, but is not available. Please file an issue!");
                 return {
                     alias: a,
                     name: n,
                     value: o
                 }
             }
-            throw new N0("intrinsic " + t + " does not exist!")
+            throw new b0("intrinsic " + t + " does not exist!")
         },
         T5 = function(t, r) {
-            if (typeof t != "string" || t.length === 0) throw new B0("intrinsic name must be a non-empty string");
-            if (arguments.length > 1 && typeof r != "boolean") throw new B0('"allowMissing" argument must be a boolean');
-            if (N5(/^%?[^%]*%?$/, t) === null) throw new N0("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
-            var n = R5(t),
+            if (typeof t != "string" || t.length === 0) throw new N0("intrinsic name must be a non-empty string");
+            if (arguments.length > 1 && typeof r != "boolean") throw new N0('"allowMissing" argument must be a boolean');
+            if (N5(/^%?[^%]*%?$/, t) === null) throw new b0("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
+            var n = x5(t),
                 a = n.length > 0 ? n[0] : "",
                 o = O5("%" + a + "%", r),
                 c = o.name,
                 s = o.value,
                 u = !1,
                 i = o.alias;
             i && (a = i[0], b5(n, w5([0, 1], i)));
             for (var f = 1, g = !0; f < n.length; f += 1) {
                 var l = n[f],
                     p = V0(l, 0, 1),
                     y = V0(l, -1);
-                if ((p === '"' || p === "'" || p === "`" || y === '"' || y === "'" || y === "`") && p !== y) throw new N0("property names with quotes must have matching quotes");
-                if ((l === "constructor" || !g) && (u = !0), a += "." + l, c = "%" + a + "%", F0(h0, c)) s = h0[c];
+                if ((p === '"' || p === "'" || p === "`" || y === '"' || y === "'" || y === "`") && p !== y) throw new b0("property names with quotes must have matching quotes");
+                if ((l === "constructor" || !g) && (u = !0), a += "." + l, c = "%" + a + "%", F0(y0, c)) s = y0[c];
                 else if (s != null) {
                     if (!(l in s)) {
-                        if (!r) throw new B0("base intrinsic for " + t + " exists, but the property is not available.");
+                        if (!r) throw new N0("base intrinsic for " + t + " exists, but the property is not available.");
                         return
                     }
-                    if (d0 && f + 1 >= n.length) {
-                        var h = d0(s, l);
+                    if (v0 && f + 1 >= n.length) {
+                        var h = v0(s, l);
                         g = !!h, g && "get" in h && !("originalValue" in h.get) ? s = h.get : s = s[l]
                     } else g = F0(s, l), s = s[l];
-                    g && !u && (h0[c] = s)
+                    g && !u && (y0[c] = s)
                 }
             }
             return s
         },
         M5 = T5,
         l1 = M5("%Object.defineProperty%", !0),
         f1 = function() {
@@ -1890,15 +1890,15 @@
             set exports(e) {
                 z0 = e
             }
         };
     typeof self < "u" ? g1.exports = self : typeof window < "u" ? g1.exports = window : g1.exports = Function("return this")();
     var $5 = z0,
         s2 = function() {
-            return typeof e0 != "object" || !e0 || e0.Math !== Math || e0.Array !== Array ? $5 : e0
+            return typeof Q != "object" || !Q || Q.Math !== Math || Q.Array !== Array ? $5 : Q
         },
         j5 = u2,
         U5 = s2,
         F5 = function() {
             var t = U5();
             if (j5.supportsDescriptors) {
                 var r = Object.getOwnPropertyDescriptor(t, "globalThis");
@@ -1937,45 +1937,45 @@
         return r
     }
 
     function Y5(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? f2(Object(r), !0).forEach(function(n) {
-                v0(e, n, r[n])
+                g0(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : f2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var r0 = W5(),
+    var t0 = W5(),
         g2 = {
             vtkObject: function() {
                 return null
             }
         };
 
-    function m0(e) {
+    function d0(e) {
         if (e == null || e.isA) return e;
-        if (!e.vtkClass) return r0.console && r0.console.error && r0.console.error("Invalid VTK object"), null;
+        if (!e.vtkClass) return t0.console && t0.console.error && t0.console.error("Invalid VTK object"), null;
         var t = g2[e.vtkClass];
-        if (!t) return r0.console && r0.console.error && r0.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
+        if (!t) return t0.console && t0.console.error && t0.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
         var r = Y5({}, e);
         Object.keys(r).forEach(function(a) {
-            r[a] && y0(r[a]) === "object" && r[a].vtkClass && (r[a] = m0(r[a]))
+            r[a] && p0(r[a]) === "object" && r[a].vtkClass && (r[a] = d0(r[a]))
         });
         var n = t(r);
         return n && n.modified && n.modified(), n
     }
 
     function X5(e, t) {
         g2[e] = t
     }
-    m0.register = X5;
+    d0.register = X5;
 
     function q5(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
 
     function p2(e, t) {
         for (var r = 0; r < t.length; r++) {
@@ -1986,22 +1986,22 @@
 
     function K5(e, t, r) {
         return t && p2(e.prototype, t), r && p2(e, r), Object.defineProperty(e, "prototype", {
             writable: !1
         }), e
     }
 
-    function C0(e) {
-        return C0 = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
+    function h0(e) {
+        return h0 = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
             return r.__proto__ || Object.getPrototypeOf(r)
-        }, C0(e)
+        }, h0(e)
     }
 
     function J5(e, t) {
-        for (; !Object.prototype.hasOwnProperty.call(e, t) && (e = C0(e), e !== null););
+        for (; !Object.prototype.hasOwnProperty.call(e, t) && (e = h0(e), e !== null););
         return e
     }
 
     function H0() {
         return typeof Reflect < "u" && Reflect.get ? H0 = Reflect.get : H0 = function(t, r, n) {
             var a = J5(t, r);
             if (a) {
@@ -2026,15 +2026,15 @@
 
     function Z5(e) {
         if (e === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
     function e3(e, t) {
-        if (t && (y0(t) === "object" || typeof t == "function")) return t;
+        if (t && (p0(t) === "object" || typeof t == "function")) return t;
         if (t !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
         return Z5(e)
     }
 
     function t3(e) {
         return Function.toString.call(e).indexOf("[native code]") !== -1
     }
@@ -2046,15 +2046,15 @@
             if (typeof n != "function") throw new TypeError("Super expression must either be null or a function");
             if (typeof t < "u") {
                 if (t.has(n)) return t.get(n);
                 t.set(n, a)
             }
 
             function a() {
-                return P0(n, arguments, C0(this).constructor)
+                return P0(n, arguments, h0(this).constructor)
             }
             return a.prototype = Object.create(n.prototype, {
                 constructor: {
                     value: a,
                     enumerable: !1,
                     writable: !0,
                     configurable: !0
@@ -2062,18 +2062,18 @@
             }), A0(a, n)
         }, p1(e)
     }
 
     function r3(e) {
         var t = n3();
         return function() {
-            var n = C0(e),
+            var n = h0(e),
                 a;
             if (t) {
-                var o = C0(this).constructor;
+                var o = h0(this).constructor;
                 a = Reflect.construct(n, arguments, o)
             } else a = n.apply(this, arguments);
             return e3(this, a)
         }
     }
 
     function n3() {
@@ -2095,15 +2095,15 @@
         return K5(r, [{
             key: "push",
             value: function() {
                 for (var a = this, o, c = arguments.length, s = new Array(c), u = 0; u < c; u++) s[u] = arguments[u];
                 var i = s.filter(function(f) {
                     return !a.includes(f)
                 });
-                return (o = H0(C0(r.prototype), "push", this)).call.apply(o, [this].concat(o1(i)))
+                return (o = H0(h0(r.prototype), "push", this)).call.apply(o, [this].concat(o1(i)))
             }
         }]), r
     }(p1(Array));
 
     function v2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
@@ -2115,81 +2115,81 @@
         return r
     }
 
     function y1(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? v2(Object(r), !0).forEach(function(n) {
-                v0(e, n, r[n])
+                g0(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : v2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
     var d1 = 0,
         a3 = Symbol("void");
 
     function o3() {
         return d1
     }
     var y2 = {};
 
-    function S0() {}
+    function m0() {}
     var i3 = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
     i3.forEach(function(e) {
-        y2[e] = S0
-    }), r0.console = console.hasOwnProperty("log") ? console : y2;
-    var J = {
-        debug: S0,
-        error: r0.console.error || S0,
-        info: r0.console.info || S0,
-        log: r0.console.log || S0,
-        warn: r0.console.warn || S0
+        y2[e] = m0
+    }), t0.console = console.hasOwnProperty("log") ? console : y2;
+    var q = {
+        debug: m0,
+        error: t0.console.error || m0,
+        info: t0.console.info || m0,
+        log: t0.console.log || m0,
+        warn: t0.console.warn || m0
     };
 
     function u3(e, t) {
-        J[e] && (J[e] = t || S0)
+        q[e] && (q[e] = t || m0)
     }
 
     function s3() {
-        J.log.apply(J, arguments)
+        q.log.apply(q, arguments)
     }
 
     function c3() {
-        J.info.apply(J, arguments)
+        q.info.apply(q, arguments)
     }
 
     function h1() {
-        J.debug.apply(J, arguments)
+        q.debug.apply(q, arguments)
     }
 
     function H() {
-        J.error.apply(J, arguments)
+        q.error.apply(q, arguments)
     }
 
     function d2() {
-        J.warn.apply(J, arguments)
+        q.warn.apply(q, arguments)
     }
     var h2 = {};
 
     function l3(e) {
-        h2[e] || (J.error(e), h2[e] = !0)
+        h2[e] || (q.error(e), h2[e] = !0)
     }
-    var t0 = Object.create(null);
-    t0.Float32Array = Float32Array, t0.Float64Array = Float64Array, t0.Uint8Array = Uint8Array, t0.Int8Array = Int8Array, t0.Uint16Array = Uint16Array, t0.Int16Array = Int16Array, t0.Uint32Array = Uint32Array, t0.Int32Array = Int32Array, t0.Uint8ClampedArray = Uint8ClampedArray;
+    var Z = Object.create(null);
+    Z.Float32Array = Float32Array, Z.Float64Array = Float64Array, Z.Uint8Array = Uint8Array, Z.Int8Array = Int8Array, Z.Uint16Array = Uint16Array, Z.Int16Array = Int16Array, Z.Uint32Array = Uint32Array, Z.Int32Array = Int32Array, Z.Uint8ClampedArray = Uint8ClampedArray;
 
     function m2(e) {
         for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
-        return P0(t0[e] || Float64Array, r)
+        return P0(Z[e] || Float64Array, r)
     }
 
     function C2(e) {
         for (var t, r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) n[a - 1] = arguments[a];
-        return (t = t0[e] || Float64Array).from.apply(t, n)
+        return (t = Z[e] || Float64Array).from.apply(t, n)
     }
 
     function m1(e) {
         return e.charAt(0).toUpperCase() + e.slice(1)
     }
 
     function I(e) {
@@ -2340,15 +2340,15 @@
         }, e.toJSON = function() {
             return e.getState()
         }, e
     }
 
     function I0(e, t, r) {
         r.forEach(function(n) {
-            y0(n) === "object" ? e["get".concat(I(n.name))] = function() {
+            p0(n) === "object" ? e["get".concat(I(n.name))] = function() {
                 return t[n.name]
             } : e["get".concat(I(n))] = function() {
                 return t[n]
             }
         })
     }
     var h3 = {
@@ -2369,15 +2369,15 @@
                 }
                 throw H("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(a)), new TypeError("Set Enum with invalid argument (String/Number)")
             }
         }
     };
 
     function B2(e) {
-        if (y0(e) === "object") {
+        if (p0(e) === "object") {
             var t = h3[e.type];
             if (t) return function(r, n) {
                 return t(r, n, e)
             };
             throw H("No setter for field ".concat(e)), new TypeError("No setter for field")
         }
         return function(n, a) {
@@ -2385,23 +2385,23 @@
                 return a.deleted ? (H("instance deleted - cannot call any method"), !1) : a[e] !== c ? (a[e] = c, n.modified(), !0) : !1
             }
         }
     }
 
     function C1(e, t, r) {
         r.forEach(function(n) {
-            y0(n) === "object" ? e["set".concat(I(n.name))] = B2(n)(e, t) : e["set".concat(I(n))] = B2(n)(e, t)
+            p0(n) === "object" ? e["set".concat(I(n.name))] = B2(n)(e, t) : e["set".concat(I(n))] = B2(n)(e, t)
         })
     }
 
-    function x2(e, t, r) {
+    function R2(e, t, r) {
         I0(e, t, r), C1(e, t, r)
     }
 
-    function R2(e, t, r) {
+    function x2(e, t, r) {
         r.forEach(function(n) {
             e["get".concat(I(n))] = function() {
                 return t[n] ? [].concat(t[n]) : t[n]
             }, e["get".concat(I(n), "ByReference")] = function() {
                 return t[n]
             }
         })
@@ -2434,26 +2434,26 @@
                 })
             }
         })
     }
 
     function m3(e, t, r, n) {
         var a = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
-        R2(e, t, r), O2(e, t, r, n, a)
+        x2(e, t, r), O2(e, t, r, n, a)
     }
 
     function C3(e, t, r) {
         for (var n = 0; n < r.length; n++) {
             var a = r[n];
             t[a] !== void 0 && (t["_".concat(a)] = t[a], delete t[a])
         }
     }
 
     function S3(e, t, r, n) {
-        t.inputData ? t.inputData = t.inputData.map(m0) : t.inputData = [], t.inputConnection ? t.inputConnection = t.inputConnection.map(m0) : t.inputConnection = [], t.output ? t.output = t.output.map(m0) : t.output = [], t.inputArrayToProcess ? t.inputArrayToProcess = t.inputArrayToProcess.map(m0) : t.inputArrayToProcess = [], t.numberOfInputs = r;
+        t.inputData ? t.inputData = t.inputData.map(d0) : t.inputData = [], t.inputConnection ? t.inputConnection = t.inputConnection.map(d0) : t.inputConnection = [], t.output ? t.output = t.output.map(d0) : t.output = [], t.inputArrayToProcess ? t.inputArrayToProcess = t.inputArrayToProcess.map(d0) : t.inputArrayToProcess = [], t.numberOfInputs = r;
 
         function a(y) {
             var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (t.deleted) {
                 H("instance deleted - cannot call any method");
                 return
             }
@@ -2516,16 +2516,16 @@
             for (var y = e.getMTime(), h = 1 / 0, C = n; C--;) {
                 if (!t.output[C] || t.output[C].isDeleted()) return !0;
                 var N = t.output[C].getMTime();
                 if (N < y) return !0;
                 N < h && (h = N)
             }
             for (C = t.numberOfInputs; C--;) {
-                var x, B;
-                if ((x = t.inputConnection[C]) !== null && x !== void 0 && x.filter.shouldUpdate() || ((B = e.getInputData(C)) === null || B === void 0 ? void 0 : B.getMTime()) > h) return !0
+                var R, B;
+                if ((R = t.inputConnection[C]) !== null && R !== void 0 && R.filter.shouldUpdate() || ((B = e.getInputData(C)) === null || B === void 0 ? void 0 : B.getMTime()) > h) return !0
             }
             return !1
         };
 
         function l() {
             var y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
                 h = function() {
@@ -2564,15 +2564,15 @@
     function w3(e, t, r) {
         var n = [],
             a = e.delete,
             o = 1;
 
         function c(i) {
             for (var f = 0; f < n.length; ++f) {
-                var g = u0(n[f], 1),
+                var g = o0(n[f], 1),
                     l = g[0];
                 if (l === i) {
                     n.splice(f, 1);
                     return
                 }
             }
         }
@@ -2589,21 +2589,21 @@
         function u() {
             var i = arguments;
             if (t.deleted) {
                 H("instance deleted - cannot call any method");
                 return
             }
             for (var f = n.slice(), g = function(h) {
-                    var C = u0(f[h], 3),
+                    var C = o0(f[h], 3),
                         N = C[1],
-                        x = C[2];
+                        R = C[2];
                     if (!N) return "continue";
-                    if (x < 0) setTimeout(function() {
+                    if (R < 0) setTimeout(function() {
                         return N.apply(e, i)
-                    }, 1 - x);
+                    }, 1 - R);
                     else {
                         var B = N.apply(e, i);
                         if (B === T2) return "break"
                     }
                 }, l = 0; l < f.length; ++l) {
                 var p = g(l);
                 if (p !== "continue" && p === "break") break
@@ -2615,29 +2615,29 @@
             if (t.deleted) return H("instance deleted - cannot call any method"), null;
             var g = o++;
             return n.push([g, i, f]), n.sort(function(l, p) {
                 return p[2] - l[2]
             }), s(g)
         }, e.delete = function() {
             a(), n.forEach(function(i) {
-                var f = u0(i, 1),
+                var f = o0(i, 1),
                     g = f[0];
                 return c(g)
             })
         }
     }
 
     function M2(e, t) {
         var r = function() {
             var a = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
                 o = {},
                 c = {};
             return e(c, o, a), Object.freeze(c)
         };
-        return t && m0.register(t, r), r
+        return t && d0.register(t, r), r
     }
 
     function b3() {
         for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
         return function() {
             for (var n = arguments.length, a = new Array(n), o = 0; o < n; o++) a[o] = arguments[o];
             return t.filter(function(c) {
@@ -2718,21 +2718,21 @@
             return delete t.keystore[n]
         }, e.clearKeystore = function() {
             return e.getAllKeys().forEach(function(n) {
                 return delete t.keystore[n]
             })
         }
     }
-    var x3 = 1,
+    var R3 = 1,
         W0 = "__root__";
 
-    function R3(e, t) {
+    function x3(e, t) {
         E2(e, t);
         var r = e.delete;
-        t.proxyId = "".concat(x3++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), I0(e, t, ["proxyId", "proxyGroup", "proxyName"]), x2(e, t, ["proxyManager"]);
+        t.proxyId = "".concat(R3++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), I0(e, t, ["proxyId", "proxyGroup", "proxyName"]), R2(e, t, ["proxyManager"]);
         var n = {},
             a = {};
 
         function o(i, f) {
             a[f] || (a[f] = []);
             for (var g = a[f], l = 0; l < i.length; l++) g.push(i[l].name), n[i[l].name] = i[l], i[l].children && i[l].children.length && o(i[l].children, i[l].name)
         }
@@ -2764,66 +2764,66 @@
             var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
             if (t.propertyLinkMap[i]) return t.propertyLinkMap[i];
             var g = null,
                 l = [],
                 p = 0,
                 y = !1;
 
-            function h(b) {
+            function h(w) {
                 var S = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
                 if (y) return null;
-                var w = [],
+                var b = [],
                     v = null;
                 for (p = l.length; p--;) {
                     var d = l[p];
-                    d.instance === b ? v = d : w.push(d)
+                    d.instance === w ? v = d : b.push(d)
                 }
                 if (!v) return null;
                 var m = v.instance["get".concat(I(v.propertyName))]();
                 if (!v3(m, g) || S) {
-                    for (g = m, y = !0; w.length;) {
-                        var O = w.pop();
-                        O.instance.set(v0({}, O.propertyName, g))
+                    for (g = m, y = !0; b.length;) {
+                        var T = b.pop();
+                        T.instance.set(g0({}, T.propertyName, g))
                     }
                     y = !1
                 }
                 return t.propertyLinkMap[i].persistent && (t.propertyLinkMap[i].value = m), m
             }
 
-            function C(b, S) {
-                var w = [];
+            function C(w, S) {
+                var b = [];
                 for (p = l.length; p--;) {
                     var v = l[p];
-                    v.instance === b && (v.propertyName === S || S === void 0) && (v.subscription.unsubscribe(), w.push(p))
+                    v.instance === w && (v.propertyName === S || S === void 0) && (v.subscription.unsubscribe(), b.push(p))
                 }
-                for (; w.length;) l.splice(w.pop(), 1)
+                for (; b.length;) l.splice(b.pop(), 1)
             }
 
-            function N(b, S) {
-                var w = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
-                    v = b.onModified(h),
+            function N(w, S) {
+                var b = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
+                    v = w.onModified(h),
                     d = l[0];
                 return l.push({
-                    instance: b,
+                    instance: w,
                     propertyName: S,
                     subscription: v
-                }), w && (t.propertyLinkMap[i].persistent && t.propertyLinkMap[i].value !== void 0 ? b.set(v0({}, S, t.propertyLinkMap[i].value)) : d && h(d.instance, !0)), {
+                }), b && (t.propertyLinkMap[i].persistent && t.propertyLinkMap[i].value !== void 0 ? w.set(g0({}, S, t.propertyLinkMap[i].value)) : d && h(d.instance, !0)), {
                     unsubscribe: function() {
-                        return C(b, S)
+                        return C(w, S)
                     }
                 }
             }
 
-            function x() {
+            function R() {
                 for (; l.length;) l.pop().subscription.unsubscribe()
             }
             var B = {
                 bind: N,
                 unbind: C,
-                unsubscribe: x,
+                unsubscribe: R,
                 persistent: f
             };
             return t.propertyLinkMap[i] = B, B
         };
 
         function s() {
             for (var i = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : W0, f = [], g = t.proxyId, l = c(i) || [], p = 0; p < l.length; p++) {
@@ -2831,16 +2831,16 @@
                     h = e["get".concat(I(y))],
                     C = h ? h() : void 0,
                     N = {
                         id: g,
                         name: y,
                         value: C
                     },
-                    x = s(y);
-                x.length && (N.children = x), f.push(N)
+                    R = s(y);
+                R.length && (N.children = R), f.push(N)
             }
             return f
         }
         e.listPropertyNames = function() {
             return s().map(function(i) {
                 return i.name
             })
@@ -2948,39 +2948,39 @@
             debounce: N3,
             enumToString: y3,
             event: w3,
             EVENT_ABORT: T2,
             formatBytesToProperUnit: g3,
             formatNumbersWithThousandSeparator: p3,
             get: I0,
-            getArray: R2,
+            getArray: x2,
             getCurrentGlobalMTime: o3,
             getStateArrayMapFunc: w2,
             isVtkObject: G2,
             keystore: E2,
             measurePromiseExecution: d3,
             moveToProtected: C3,
             newInstance: M2,
             newTypedArray: m2,
             newTypedArrayFrom: C2,
             normalizeWheel: M3,
             obj: N2,
-            proxy: R3,
+            proxy: x3,
             proxyPropertyMapping: O3,
             proxyPropertyState: T3,
             safeArrays: S2,
             set: C1,
             setArray: O2,
-            setGet: x2,
+            setGet: R2,
             setGetArray: m3,
             setImmediate: b2,
             setLoggerFunction: u3,
             throttle: B3,
             traverseInstanceTree: S1,
-            TYPED_ARRAYS: t0,
+            TYPED_ARRAYS: Z,
             uncapitalize: f3,
             VOID: a3,
             vtkDebugMacro: h1,
             vtkErrorMacro: H,
             vtkInfoMacro: c3,
             vtkLogMacro: s3,
             vtkOnceErrorMacro: l3,
@@ -3035,15 +3035,15 @@
                         return (u >>> 0) * 23283064365386963e-26
                     };
                 return i
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.alea = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(G3);
     var b1 = {},
         E3 = {
             get exports() {
                 return b1
             },
             set exports(e) {
@@ -3080,15 +3080,15 @@
                 }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
                     return o(i, {})
                 }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xor128 = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(E3);
     var N1 = {},
         k3 = {
             get exports() {
                 return N1
             },
             set exports(e) {
@@ -3125,15 +3125,15 @@
                 }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
                     return o(i, {})
                 }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xorwow = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(k3);
     var B1 = {},
         D3 = {
             get exports() {
                 return B1
             },
             set exports(e) {
@@ -3182,23 +3182,23 @@
                 }, g.int32 = i.next, g.quick = g, f && (f.x && o(f, i), g.state = function() {
                     return o(i, {})
                 }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xorshift7 = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(D3);
-    var x1 = {},
+    var R1 = {},
         L3 = {
             get exports() {
-                return x1
+                return R1
             },
             set exports(e) {
-                x1 = e
+                R1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
                 var u = this;
                 u.next = function() {
@@ -3207,16 +3207,16 @@
                         l = u.i,
                         p, y;
                     return u.w = f = f + 1640531527 | 0, y = g[l + 34 & 127], p = g[l = l + 1 & 127], y ^= y << 13, p ^= p << 17, y ^= y >>> 15, p ^= p >>> 12, y = g[l] = y ^ p, u.i = l, y + (f ^ f >>> 16) | 0
                 };
 
                 function i(f, g) {
                     var l, p, y, h, C, N = [],
-                        x = 128;
-                    for (g === (g | 0) ? (p = g, g = null) : (g = g + "\0", p = 0, x = Math.max(x, g.length)), y = 0, h = -32; h < x; ++h) g && (p ^= g.charCodeAt((h + 32) % g.length)), h === 0 && (C = p), p ^= p << 10, p ^= p >>> 15, p ^= p << 4, p ^= p >>> 13, h >= 0 && (C = C + 1640531527 | 0, l = N[h & 127] ^= p + C, y = l == 0 ? y + 1 : 0);
+                        R = 128;
+                    for (g === (g | 0) ? (p = g, g = null) : (g = g + "\0", p = 0, R = Math.max(R, g.length)), y = 0, h = -32; h < R; ++h) g && (p ^= g.charCodeAt((h + 32) % g.length)), h === 0 && (C = p), p ^= p << 10, p ^= p >>> 15, p ^= p << 4, p ^= p >>> 13, h >= 0 && (C = C + 1640531527 | 0, l = N[h & 127] ^= p + C, y = l == 0 ? y + 1 : 0);
                     for (y >= 128 && (N[(g && g.length || 0) & 127] = -1), y = 127, h = 4 * 128; h > 0; --h) p = N[y + 34 & 127], l = N[y = y + 1 & 127], p ^= p << 13, l ^= l << 17, p ^= p >>> 15, l ^= l >>> 12, N[y] = p ^ l;
                     f.w = C, f.X = N, f.i = y
                 }
                 i(u, s)
             }
 
             function o(s, u) {
@@ -3238,23 +3238,23 @@
                 }, g.int32 = i.next, g.quick = g, f && (f.X && o(f, i), g.state = function() {
                     return o(i, {})
                 }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xor4096 = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(L3);
-    var R1 = {},
+    var x1 = {},
         A3 = {
             get exports() {
-                return R1
+                return x1
             },
             set exports(e) {
-                R1 = e
+                x1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
                 var u = this,
                     i = "";
@@ -3286,15 +3286,15 @@
                 }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
                     return o(i, {})
                 }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.tychei = c
-        })(e0, e, !1)
+        })(Q, e, !1)
     })(A3);
     var O1 = {},
         P3 = {
             get exports() {
                 return O1
             },
             set exports(e) {
@@ -3315,101 +3315,101 @@
                 s = "random",
                 u = n.pow(a, o),
                 i = n.pow(2, c),
                 f = i * 2,
                 g = a - 1,
                 l;
 
-            function p(b, S, w) {
+            function p(w, S, b) {
                 var v = [];
                 S = S == !0 ? {
                     entropy: !0
                 } : S || {};
-                var d = N(C(S.entropy ? [b, B(r)] : b ?? x(), 3), v),
+                var d = N(C(S.entropy ? [w, B(r)] : w ?? R(), 3), v),
                     m = new y(v),
-                    O = function() {
-                        for (var D = m.g(o), _ = u, U = 0; D < i;) D = (D + U) * a, _ *= a, U = m.g(1);
-                        for (; D >= f;) D /= 2, _ /= 2, U >>>= 1;
-                        return (D + U) / _
+                    T = function() {
+                        for (var D = m.g(o), P = u, F = 0; D < i;) D = (D + F) * a, P *= a, F = m.g(1);
+                        for (; D >= f;) D /= 2, P /= 2, F >>>= 1;
+                        return (D + F) / P
                     };
-                return O.int32 = function() {
+                return T.int32 = function() {
                     return m.g(4) | 0
-                }, O.quick = function() {
+                }, T.quick = function() {
                     return m.g(4) / 4294967296
-                }, O.double = O, N(B(m.S), r), (S.pass || w || function(D, _, U, F) {
-                    return F && (F.S && h(F, m), D.state = function() {
+                }, T.double = T, N(B(m.S), r), (S.pass || b || function(D, P, F, _) {
+                    return _ && (_.S && h(_, m), D.state = function() {
                         return h(m, {})
-                    }), U ? (n[s] = D, _) : D
-                })(O, d, "global" in S ? S.global : this == n, S.state)
+                    }), F ? (n[s] = D, P) : D
+                })(T, d, "global" in S ? S.global : this == n, S.state)
             }
 
-            function y(b) {
-                var S, w = b.length,
+            function y(w) {
+                var S, b = w.length,
                     v = this,
                     d = 0,
                     m = v.i = v.j = 0,
-                    O = v.S = [];
-                for (w || (b = [w++]); d < a;) O[d] = d++;
-                for (d = 0; d < a; d++) O[d] = O[m = g & m + b[d % w] + (S = O[d])], O[m] = S;
+                    T = v.S = [];
+                for (b || (w = [b++]); d < a;) T[d] = d++;
+                for (d = 0; d < a; d++) T[d] = T[m = g & m + w[d % b] + (S = T[d])], T[m] = S;
                 (v.g = function(D) {
-                    for (var _, U = 0, F = v.i, T = v.j, L = v.S; D--;) _ = L[F = g & F + 1], U = U * a + L[g & (L[F] = L[T = g & T + _]) + (L[T] = _)];
-                    return v.i = F, v.j = T, U
+                    for (var P, F = 0, _ = v.i, x = v.j, j = v.S; D--;) P = j[_ = g & _ + 1], F = F * a + j[g & (j[_] = j[x = g & x + P]) + (j[x] = P)];
+                    return v.i = _, v.j = x, F
                 })(a)
             }
 
-            function h(b, S) {
-                return S.i = b.i, S.j = b.j, S.S = b.S.slice(), S
+            function h(w, S) {
+                return S.i = w.i, S.j = w.j, S.S = w.S.slice(), S
             }
 
-            function C(b, S) {
-                var w = [],
-                    v = typeof b,
+            function C(w, S) {
+                var b = [],
+                    v = typeof w,
                     d;
                 if (S && v == "object")
-                    for (d in b) try {
-                        w.push(C(b[d], S - 1))
+                    for (d in w) try {
+                        b.push(C(w[d], S - 1))
                     } catch {}
-                return w.length ? w : v == "string" ? b : b + "\0"
+                return b.length ? b : v == "string" ? w : w + "\0"
             }
 
-            function N(b, S) {
-                for (var w = b + "", v, d = 0; d < w.length;) S[g & d] = g & (v ^= S[g & d] * 19) + w.charCodeAt(d++);
+            function N(w, S) {
+                for (var b = w + "", v, d = 0; d < b.length;) S[g & d] = g & (v ^= S[g & d] * 19) + b.charCodeAt(d++);
                 return B(S)
             }
 
-            function x() {
+            function R() {
                 try {
-                    var b;
-                    return l && (b = l.randomBytes) ? b = b(a) : (b = new Uint8Array(a), (t.crypto || t.msCrypto).getRandomValues(b)), B(b)
+                    var w;
+                    return l && (w = l.randomBytes) ? w = w(a) : (w = new Uint8Array(a), (t.crypto || t.msCrypto).getRandomValues(w)), B(w)
                 } catch {
                     var S = t.navigator,
-                        w = S && S.plugins;
-                    return [+new Date, t, w, t.screen, B(r)]
+                        b = S && S.plugins;
+                    return [+new Date, t, b, t.screen, B(r)]
                 }
             }
 
-            function B(b) {
-                return String.fromCharCode.apply(0, b)
+            function B(w) {
+                return String.fromCharCode.apply(0, w)
             }
             if (N(n.random(), r), e.exports) {
                 e.exports = p;
                 try {
                     l = _3
                 } catch {}
             } else n["seed" + s] = p
-        })(typeof self < "u" ? self : e0, [], Math)
+        })(typeof self < "u" ? self : Q, [], Math)
     })(P3);
     var $3 = w1,
         j3 = b1,
         U3 = N1,
         F3 = B1,
-        V3 = x1,
-        z3 = R1,
-        O0 = O1;
-    O0.alea = $3, O0.xor128 = j3, O0.xorwow = U3, O0.xorshift7 = F3, O0.xor4096 = V3, O0.tychei = z3;
+        V3 = R1,
+        z3 = x1,
+        x0 = O1;
+    x0.alea = $3, x0.xor128 = j3, x0.xorwow = U3, x0.xorshift7 = F3, x0.xor4096 = V3, x0.tychei = z3;
     var H3 = Math.floor;
 
     function I3(e) {
         var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 3;
         switch (t) {
             case 1:
                 return Math.abs(e);
@@ -3421,92 +3421,92 @@
                 for (var r = 0, n = 0; n < t; n++) r += e[n] * e[n];
                 return Math.sqrt(r)
             }
         }
     }
 
     function Y0(e, t) {
-        var r, n, a = u0(e, 3),
+        var r, n, a = o0(e, 3),
             o = a[0],
             c = a[1],
             s = a[2],
             u = 1 / 3,
             i = 1 / 6,
             f = 2 / 3,
             g = o,
             l = o;
         c > g ? g = c : c < l && (l = c), s > g ? g = s : s < l && (l = s);
         var p = g;
         p > 0 ? n = (g - l) / g : n = 0, n > 0 ? (o === g ? r = i * (c - s) / (g - l) : c === g ? r = u + i * (s - o) / (g - l) : r = f + i * (o - c) / (g - l), r < 0 && (r += 1)) : r = 0, t[0] = r, t[1] = n, t[2] = p
     }
 
     function $0(e, t) {
-        var r = u0(e, 3),
+        var r = o0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = 1 / 3,
             s = 1 / 6,
             u = 2 / 3,
             i = 5 / 6,
             f, g, l;
         n > s && n <= c ? (g = 1, f = (c - n) / s, l = 0) : n > c && n <= .5 ? (g = 1, l = (n - c) / s, f = 0) : n > .5 && n <= u ? (l = 1, g = (u - n) / s, f = 0) : n > u && n <= i ? (l = 1, f = (n - u) / s, g = 0) : n > i && n <= 1 ? (f = 1, l = (1 - n) / s, g = 0) : (f = 1, g = n / s, l = 0), f = a * f + (1 - a), g = a * g + (1 - a), l = a * l + (1 - a), f *= o, g *= o, l *= o, t[0] = f, t[1] = g, t[2] = l
     }
 
     function W3(e, t) {
-        var r = u0(e, 3),
+        var r = o0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = (n + 16) / 116,
             s = a / 500 + c,
             u = c - o / 200;
         Math.pow(c, 3) > .008856 ? c = Math.pow(c, 3) : c = (c - 16 / 116) / 7.787, Math.pow(s, 3) > .008856 ? s = Math.pow(s, 3) : s = (s - 16 / 116) / 7.787, Math.pow(u, 3) > .008856 ? u = Math.pow(u, 3) : u = (u - 16 / 116) / 7.787;
         var i = .9505,
             f = 1,
             g = 1.089;
         t[0] = i * s, t[1] = f * c, t[2] = g * u
     }
 
     function Y3(e, t) {
-        var r = u0(e, 3),
+        var r = o0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = .9505,
             s = 1,
             u = 1.089,
             i = n / c,
             f = a / s,
             g = o / u;
         i > .008856 ? i = Math.pow(i, 1 / 3) : i = 7.787 * i + 16 / 116, f > .008856 ? f = Math.pow(f, 1 / 3) : f = 7.787 * f + 16 / 116, g > .008856 ? g = Math.pow(g, 1 / 3) : g = 7.787 * g + 16 / 116, t[0] = 116 * f - 16, t[1] = 500 * (i - f), t[2] = 200 * (f - g)
     }
 
     function X3(e, t) {
-        var r = u0(e, 3),
+        var r = o0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = n * 3.2406 + a * -1.5372 + o * -.4986,
             s = n * -.9689 + a * 1.8758 + o * .0415,
             u = n * .0557 + a * -.204 + o * 1.057;
         c > .0031308 ? c = 1.055 * Math.pow(c, 1 / 2.4) - .055 : c *= 12.92, s > .0031308 ? s = 1.055 * Math.pow(s, 1 / 2.4) - .055 : s *= 12.92, u > .0031308 ? u = 1.055 * Math.pow(u, 1 / 2.4) - .055 : u *= 12.92;
         var i = c;
         i < s && (i = s), i < u && (i = u), i > 1 && (c /= i, s /= i, u /= i), c < 0 && (c = 0), s < 0 && (s = 0), u < 0 && (u = 0), t[0] = c, t[1] = s, t[2] = u
     }
 
     function q3(e, t) {
-        var r = u0(e, 3),
+        var r = o0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2];
         n > .04045 ? n = Math.pow((n + .055) / 1.055, 2.4) : n /= 12.92, a > .04045 ? a = Math.pow((a + .055) / 1.055, 2.4) : a /= 12.92, o > .04045 ? o = Math.pow((o + .055) / 1.055, 2.4) : o /= 12.92, t[0] = n * .4124 + a * .3576 + o * .1805, t[1] = n * .2126 + a * .7152 + o * .0722, t[2] = n * .0193 + a * .1192 + o * .9505
     }
 
-    function T0(e, t) {
+    function O0(e, t) {
         var r = [0, 0, 0];
         q3(e, r), Y3(r, t)
     }
 
     function T1(e, t) {
         var r = [0, 0, 0];
         W3(e, r), X3(r, t)
@@ -3557,15 +3557,15 @@
         return r
     }
 
     function X0(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? $2(Object(r), !0).forEach(function(n) {
-                v0(e, n, r[n])
+                g0(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : $2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
     var e8 = _2.DefaultDataType,
@@ -3793,42 +3793,42 @@
         return r
     }
 
     function p8(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? z2(Object(r), !0).forEach(function(n) {
-                v0(e, n, r[n])
+                g0(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : z2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
     var H2 = E1.ScalarMappingTarget,
-        o0 = E1.VectorMode,
-        M0 = q0.VtkDataTypes,
+        n0 = E1.VectorMode,
+        T0 = q0.VtkDataTypes,
         I2 = g8.ColorMode,
         W2 = W.vtkErrorMacro;
 
     function v8(e) {
         return e
     }
 
     function Y2(e) {
         return Math.floor(e * 255 + .5)
     }
 
     function y8(e, t) {
         t.classHierarchy.push("vtkScalarsToColors"), e.setVectorModeToMagnitude = function() {
-            return e.setVectorMode(o0.MAGNITUDE)
+            return e.setVectorMode(n0.MAGNITUDE)
         }, e.setVectorModeToComponent = function() {
-            return e.setVectorMode(o0.COMPONENT)
+            return e.setVectorMode(n0.COMPONENT)
         }, e.setVectorModeToRGBColors = function() {
-            return e.setVectorMode(o0.RGBCOLORS)
+            return e.setVectorMode(n0.RGBCOLORS)
         }, e.build = function() {}, e.isOpaque = function() {
             return !0
         }, e.setAnnotations = function(r, n) {
             if (!(r && !n || !r && n)) {
                 if (r && n && r.length !== n.length) {
                     W2("Values and annotations do not have the same number of tuples so ignoring");
                     return
@@ -3878,21 +3878,21 @@
             n[0] = 0, n[1] = 0, n[2] = 0, n[3] = 0
         }, e.updateAnnotatedValueMap = function() {
             t.annotatedValueMap = [];
             for (var r = t.annotationArray.length, n = 0; n < r; n++) t.annotatedValueMap[t.annotationArray[n].value] = n
         }, e.mapScalars = function(r, n, a) {
             var o = r.getNumberOfComponents(),
                 c = null;
-            if (n === I2.DEFAULT && r.getDataType() === M0.UNSIGNED_CHAR || n === I2.DIRECT_SCALARS && r) c = e.convertToRGBA(r, o, r.getNumberOfTuples());
+            if (n === I2.DEFAULT && r.getDataType() === T0.UNSIGNED_CHAR || n === I2.DIRECT_SCALARS && r) c = e.convertToRGBA(r, o, r.getNumberOfTuples());
             else {
                 var s = {
                         type: "vtkDataArray",
                         name: "temp",
                         numberOfComponents: 4,
-                        dataType: M0.UNSIGNED_CHAR
+                        dataType: T0.UNSIGNED_CHAR
                     },
                     u = W.newTypedArray(s.dataType, 4 * r.getNumberOfTuples());
                 s.values = u, s.size = u.length, c = q0.newInstance(s);
                 var i = a;
                 i < 0 && o > 1 ? e.mapVectorsThroughTable(r, c, H2.RGBA, -1, -1) : (i < 0 && (i = 0), i >= o && (i = o - 1), e.mapScalarsThroughTable(r, c, H2.RGBA, i))
             }
             return c
@@ -3902,24 +3902,24 @@
                 s[i] = Math.sqrt(f)
             }
         }, e.mapVectorsThroughTable = function(r, n, a, o, c) {
             var s = e.getVectorMode(),
                 u = c,
                 i = o,
                 f = r.getNumberOfComponents();
-            s === o0.COMPONENT ? (i === -1 && (i = e.getVectorComponent()), i < 0 && (i = 0), i >= f && (i = f - 1)) : (u === -1 && (u = e.getVectorSize()), u <= 0 ? (i = 0, u = f) : (i < 0 && (i = 0), i >= f && (i = f - 1), i + u > f && (u = f - i)), s === o0.MAGNITUDE && (f === 1 || u === 1) && (s = o0.COMPONENT));
+            s === n0.COMPONENT ? (i === -1 && (i = e.getVectorComponent()), i < 0 && (i = 0), i >= f && (i = f - 1)) : (u === -1 && (u = e.getVectorSize()), u <= 0 ? (i = 0, u = f) : (i < 0 && (i = 0), i >= f && (i = f - 1), i + u > f && (u = f - i)), s === n0.MAGNITUDE && (f === 1 || u === 1) && (s = n0.COMPONENT));
             var g = 0;
             switch (i > 0 && (g = i), s) {
-                case o0.COMPONENT: {
+                case n0.COMPONENT: {
                     e.mapScalarsThroughTable(r, n, a, g);
                     break
                 }
-                case o0.RGBCOLORS:
+                case n0.RGBCOLORS:
                     break;
-                case o0.MAGNITUDE:
+                case n0.MAGNITUDE:
                 default: {
                     var l = q0.newInstance({
                         numberOfComponents: 1,
                         values: new Float32Array(r.getNumberOfTuples())
                     });
                     e.mapVectorsToMagnitude(r, l, u), e.mapScalarsThroughTable(l, n, a, 0);
                     break
@@ -3937,25 +3937,25 @@
             }
         }, e.rGBToRGBA = function(r, n, a, o) {
             for (var c = Y2(a), s = n.getData(), u = r.getData(), i = s.length, f = 0, g = 3, l = 0, p = f; p < i; p += g) u[l * 4] = o(s[p]), u[l * 4 + 1] = o(s[p + 1]), u[l * 4 + 2] = o(s[p + 2]), u[l * 4 + 3] = c, l++
         }, e.rGBAToRGBA = function(r, n, a, o) {
             for (var c = n.getData(), s = r.getData(), u = c.length, i = 0, f = 4, g = 0, l = i; l < u; l += f) s[g * 4] = o(c[l]), s[g * 4 + 1] = o(c[l + 1]), s[g * 4 + 2] = o(c[l + 2]), s[g * 4 + 3] = o(c[l + 3]) * a, g++
         }, e.convertToRGBA = function(r, n, a) {
             var o = t.alpha;
-            if (n === 4 && o >= 1 && r.getDataType() === M0.UNSIGNED_CHAR) return r;
+            if (n === 4 && o >= 1 && r.getDataType() === T0.UNSIGNED_CHAR) return r;
             var c = q0.newInstance({
                 numberOfComponents: 4,
                 empty: !0,
                 size: 4 * a,
-                dataType: M0.UNSIGNED_CHAR
+                dataType: T0.UNSIGNED_CHAR
             });
             if (a <= 0) return c;
             o = o > 0 ? o : 0, o = o < 1 ? o : 1;
             var s = v8;
-            switch ((r.getDataType() === M0.FLOAT || r.getDataType() === M0.DOUBLE) && (s = Y2), n) {
+            switch ((r.getDataType() === T0.FLOAT || r.getDataType() === T0.DOUBLE) && (s = Y2), n) {
                 case 1:
                     e.luminanceToRGBA(c, r, o, s);
                     break;
                 case 2:
                     e.luminanceAlphaToRGBA(c, r, s);
                     break;
                 case 3:
@@ -3978,15 +3978,15 @@
             return e.getMappingRange()
         }
     }
     var d8 = {
         alpha: 1,
         vectorComponent: 0,
         vectorSize: -1,
-        vectorMode: o0.COMPONENT,
+        vectorMode: n0.COMPONENT,
         mappingRange: null,
         annotationArray: null,
         annotatedValueMap: null,
         indexedLookup: !1
     };
 
     function X2(e, t) {
@@ -4024,26 +4024,26 @@
         return r
     }
 
     function S8(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
             t % 2 ? K2(Object(r), !0).forEach(function(n) {
-                v0(e, n, r[n])
+                g0(e, n, r[n])
             }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : K2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var n0 = k1.ColorSpace,
+    var r0 = k1.ColorSpace,
         J2 = k1.Scale,
         K0 = q2.ScalarMappingTarget,
         w8 = W.vtkDebugMacro,
-        s0 = W.vtkErrorMacro,
+        i0 = W.vtkErrorMacro,
         b8 = W.vtkWarningMacro;
 
     function Q2(e, t) {
         var r = e[0],
             n = e[1],
             a = e[2],
             o = Math.sqrt(r * r + n * n + a * a),
@@ -4070,15 +4070,15 @@
         for (r < 0 && (r = -r); r >= 2 * Math.PI;) r -= 2 * Math.PI;
         return r > Math.PI && (r = 2 * Math.PI - r), r
     }
 
     function e9(e, t, r, n) {
         var a = [],
             o = [];
-        T0(t, a), T0(r, o);
+        O0(t, a), O0(r, o);
         var c = [],
             s = [];
         Q2(a, c), Q2(o, s);
         var u = e;
         if (c[1] > .05 && s[1] > .05 && B8(c[2], s[2]) > .33 * Math.PI) {
             var i = Math.max(c[0], s[0]);
             i = Math.max(88, i), e < .5 ? (s[0] = i, s[1] = 0, s[2] = 0, u *= 2) : (c[0] = i, c[1] = 0, c[2] = 0, u = 2 * u - 1)
@@ -4086,24 +4086,24 @@
         c[1] < .05 && s[1] > .05 ? c[2] = Z2(s, c[0]) : s[1] < .05 && c[1] > .05 && (s[2] = Z2(c, s[0]));
         var f = [];
         f[0] = (1 - u) * c[0] + u * s[0], f[1] = (1 - u) * c[1] + u * s[1], f[2] = (1 - u) * c[2] + u * s[2];
         var g = [];
         N8(f, g), T1(g, n)
     }
 
-    function x8(e, t) {
+    function R8(e, t) {
         t.classHierarchy.push("vtkColorTransferFunction"), e.getSize = function() {
             return t.nodes.length
         }, e.addRGBPoint = function(r, n, a, o) {
             return e.addRGBPointLong(r, n, a, o, .5, 0)
         }, e.addRGBPointLong = function(r, n, a, o) {
             var c = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : .5,
                 s = arguments.length > 5 && arguments[5] !== void 0 ? arguments[5] : 0;
-            if (c < 0 || c > 1) return s0("Midpoint outside range [0.0, 1.0]"), -1;
-            if (s < 0 || s > 1) return s0("Sharpness outside range [0.0, 1.0]"), -1;
+            if (c < 0 || c > 1) return i0("Midpoint outside range [0.0, 1.0]"), -1;
+            if (s < 0 || s > 1) return i0("Sharpness outside range [0.0, 1.0]"), -1;
             t.allowDuplicateScalars || e.removePoint(r);
             var u = {
                 x: r,
                 r: n,
                 g: a,
                 b: o,
                 midpoint: c,
@@ -4205,98 +4205,98 @@
             u !== 0 && (i = t.nodes[u - 1].r, f = t.nodes[u - 1].g, g = t.nodes[u - 1].b);
             var l = 0,
                 p = 0,
                 y = 0,
                 h = [0, 0, 0],
                 C = [0, 0, 0],
                 N = 0,
-                x = 0,
+                R = 0,
                 B = [],
-                b = t.scale === J2.LOG10;
-            b && (b = t.mappingRange[0] > 0);
+                w = t.scale === J2.LOG10;
+            w && (w = t.mappingRange[0] > 0);
             var S = 0,
-                w = 0,
+                b = 0,
                 v = 0;
-            b && (S = Math.log10(r), w = Math.log10(n));
+            w && (S = Math.log10(r), b = Math.log10(n));
             for (var d = 0; d < a; d++) {
                 var m = 3 * d;
-                if (a > 1 ? b ? (v = S + d / (a - 1) * (w - S), l = Math.pow(10, v)) : l = r + d / (a - 1) * (n - r) : b ? (v = .5 * (S + w), l = Math.pow(10, v)) : l = .5 * (r + n), t.discretize) {
-                    var O = t.mappingRange;
-                    if (l >= O[0] && l <= O[1]) {
+                if (a > 1 ? w ? (v = S + d / (a - 1) * (b - S), l = Math.pow(10, v)) : l = r + d / (a - 1) * (n - r) : w ? (v = .5 * (S + b), l = Math.pow(10, v)) : l = .5 * (r + n), t.discretize) {
+                    var T = t.mappingRange;
+                    if (l >= T[0] && l <= T[1]) {
                         var D = t.numberOfValues,
-                            _ = O[1] - O[0];
-                        if (D <= 1) l = O[0] + _ / 2;
+                            P = T[1] - T[0];
+                        if (D <= 1) l = T[0] + P / 2;
                         else {
-                            var U = (l - O[0]) / _,
-                                F = H3(D * U);
-                            l = O[0] + F / (D - 1) * _
+                            var F = (l - T[0]) / P,
+                                _ = H3(D * F);
+                            l = T[0] + _ / (D - 1) * P
                         }
                     }
                 }
-                for (; s < u && l > t.nodes[s].x;) s++, s < u && (p = t.nodes[s - 1].x, y = t.nodes[s].x, b && (p = Math.log10(p), y = Math.log10(y)), h[0] = t.nodes[s - 1].r, C[0] = t.nodes[s].r, h[1] = t.nodes[s - 1].g, C[1] = t.nodes[s].g, h[2] = t.nodes[s - 1].b, C[2] = t.nodes[s].b, N = t.nodes[s - 1].midpoint, x = t.nodes[s - 1].sharpness, N < 1e-5 && (N = 1e-5), N > .99999 && (N = .99999));
+                for (; s < u && l > t.nodes[s].x;) s++, s < u && (p = t.nodes[s - 1].x, y = t.nodes[s].x, w && (p = Math.log10(p), y = Math.log10(y)), h[0] = t.nodes[s - 1].r, C[0] = t.nodes[s].r, h[1] = t.nodes[s - 1].g, C[1] = t.nodes[s].g, h[2] = t.nodes[s - 1].b, C[2] = t.nodes[s].b, N = t.nodes[s - 1].midpoint, R = t.nodes[s - 1].sharpness, N < 1e-5 && (N = 1e-5), N > .99999 && (N = .99999));
                 if (l > t.mappingRange[1]) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseAboveRangeColor() ? (o[m] = t.aboveRangeColor[0], o[m + 1] = t.aboveRangeColor[1], o[m + 2] = t.aboveRangeColor[2]) : (o[m] = i, o[m + 1] = f, o[m + 2] = g));
                 else if (l < t.mappingRange[0] || K3(l) && l < 0) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseBelowRangeColor() ? (o[m] = t.belowRangeColor[0], o[m + 1] = t.belowRangeColor[1], o[m + 2] = t.belowRangeColor[2]) : u > 0 && (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b));
                 else if (s === 0 && (Math.abs(l - r) < 1e-6 || t.discretize)) u > 0 ? (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b) : (o[m] = 0, o[m + 1] = 0, o[m + 2] = 0);
                 else {
-                    var T = 0;
-                    if (b ? T = (v - p) / (y - p) : T = (l - p) / (y - p), T < N ? T = .5 * T / N : T = .5 + .5 * (T - N) / (1 - N), x > .99)
-                        if (T < .5) {
+                    var x = 0;
+                    if (w ? x = (v - p) / (y - p) : x = (l - p) / (y - p), x < N ? x = .5 * x / N : x = .5 + .5 * (x - N) / (1 - N), R > .99)
+                        if (x < .5) {
                             o[m] = h[0], o[m + 1] = h[1], o[m + 2] = h[2];
                             continue
                         } else {
                             o[m] = C[0], o[m + 1] = C[1], o[m + 2] = C[2];
                             continue
-                        } if (x < .01) {
-                        if (t.colorSpace === n0.RGB) o[m] = (1 - T) * h[0] + T * C[0], o[m + 1] = (1 - T) * h[1] + T * C[1], o[m + 2] = (1 - T) * h[2] + T * C[2];
-                        else if (t.colorSpace === n0.HSV) {
-                            var L = [],
+                        } if (R < .01) {
+                        if (t.colorSpace === r0.RGB) o[m] = (1 - x) * h[0] + x * C[0], o[m + 1] = (1 - x) * h[1] + x * C[1], o[m + 2] = (1 - x) * h[2] + x * C[2];
+                        else if (t.colorSpace === r0.HSV) {
+                            var j = [],
                                 V = [];
-                            Y0(h, L), Y0(C, V), t.hSVWrap && (L[0] - V[0] > .5 || V[0] - L[0] > .5) && (L[0] > V[0] ? L[0] -= 1 : V[0] -= 1);
-                            var Q = [];
-                            Q[0] = (1 - T) * L[0] + T * V[0], Q[0] < 0 && (Q[0] += 1), Q[1] = (1 - T) * L[1] + T * V[1], Q[2] = (1 - T) * L[2] + T * V[2], $0(Q, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                        } else if (t.colorSpace === n0.LAB) {
-                            var K = [],
-                                a0 = [];
-                            T0(h, K), T0(C, a0);
+                            Y0(h, j), Y0(C, V), t.hSVWrap && (j[0] - V[0] > .5 || V[0] - j[0] > .5) && (j[0] > V[0] ? j[0] -= 1 : V[0] -= 1);
+                            var e0 = [];
+                            e0[0] = (1 - x) * j[0] + x * V[0], e0[0] < 0 && (e0[0] += 1), e0[1] = (1 - x) * j[1] + x * V[1], e0[2] = (1 - x) * j[2] + x * V[2], $0(e0, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                        } else if (t.colorSpace === r0.LAB) {
+                            var E0 = [],
+                                C0 = [];
+                            O0(h, E0), O0(C, C0);
                             var M = [];
-                            M[0] = (1 - T) * K[0] + T * a0[0], M[1] = (1 - T) * K[1] + T * a0[1], M[2] = (1 - T) * K[2] + T * a0[2], T1(M, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                        } else t.colorSpace === n0.DIVERGING ? (e9(T, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : s0("ColorSpace set to invalid value.", t.colorSpace);
+                            M[0] = (1 - x) * E0[0] + x * C0[0], M[1] = (1 - x) * E0[1] + x * C0[1], M[2] = (1 - x) * E0[2] + x * C0[2], T1(M, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                        } else t.colorSpace === r0.DIVERGING ? (e9(x, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : i0("ColorSpace set to invalid value.", t.colorSpace);
                         continue
                     }
-                    T < .5 ? T = .5 * Math.pow(T * 2, 1 + 10 * x) : T > .5 && (T = 1 - .5 * Math.pow((1 - T) * 2, 1 + 10 * x));
-                    var E = T * T,
-                        A = E * T,
-                        k = 2 * A - 3 * E + 1,
-                        $ = -2 * A + 3 * E,
-                        Z = A - 2 * E + T,
-                        P = A - E,
-                        j = void 0,
+                    x < .5 ? x = .5 * Math.pow(x * 2, 1 + 10 * R) : x > .5 && (x = 1 - .5 * Math.pow((1 - x) * 2, 1 + 10 * R));
+                    var E = x * x,
+                        L = E * x,
+                        k = 2 * L - 3 * E + 1,
+                        $ = -2 * L + 3 * E,
+                        J = L - 2 * E + x,
+                        A = L - E,
+                        U = void 0,
                         Y = void 0;
-                    if (t.colorSpace === n0.RGB)
-                        for (var X = 0; X < 3; X++) j = C[X] - h[X], Y = (1 - x) * j, o[m + X] = k * h[X] + $ * C[X] + Z * Y + P * Y;
-                    else if (t.colorSpace === n0.HSV) {
-                        var l0 = [],
-                            f0 = [];
-                        Y0(h, l0), Y0(C, f0), t.hSVWrap && (l0[0] - f0[0] > .5 || f0[0] - l0[0] > .5) && (l0[0] > f0[0] ? l0[0] -= 1 : f0[0] -= 1);
-                        for (var e1 = [], i0 = 0; i0 < 3; i0++) j = f0[i0] - l0[i0], Y = (1 - x) * j, e1[i0] = k * l0[i0] + $ * f0[i0] + Z * Y + P * Y, i0 === 0 && e1[i0] < 0 && (e1[i0] += 1);
+                    if (t.colorSpace === r0.RGB)
+                        for (var X = 0; X < 3; X++) U = C[X] - h[X], Y = (1 - R) * U, o[m + X] = k * h[X] + $ * C[X] + J * Y + A * Y;
+                    else if (t.colorSpace === r0.HSV) {
+                        var s0 = [],
+                            c0 = [];
+                        Y0(h, s0), Y0(C, c0), t.hSVWrap && (s0[0] - c0[0] > .5 || c0[0] - s0[0] > .5) && (s0[0] > c0[0] ? s0[0] -= 1 : c0[0] -= 1);
+                        for (var e1 = [], a0 = 0; a0 < 3; a0++) U = c0[a0] - s0[a0], Y = (1 - R) * U, e1[a0] = k * s0[a0] + $ * c0[a0] + J * Y + A * Y, a0 === 0 && e1[a0] < 0 && (e1[a0] += 1);
                         $0(e1, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                    } else if (t.colorSpace === n0.LAB) {
+                    } else if (t.colorSpace === r0.LAB) {
                         var P1 = [],
                             _1 = [];
-                        T0(h, P1), T0(C, _1);
-                        for (var u9 = [], w0 = 0; w0 < 3; w0++) j = _1[w0] - P1[w0], Y = (1 - x) * j, u9[w0] = k * P1[w0] + $ * _1[w0] + Z * Y + P * Y;
+                        O0(h, P1), O0(C, _1);
+                        for (var u9 = [], S0 = 0; S0 < 3; S0++) U = _1[S0] - P1[S0], Y = (1 - R) * U, u9[S0] = k * P1[S0] + $ * _1[S0] + J * Y + A * Y;
                         T1(u9, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                    } else t.colorSpace === n0.DIVERGING ? (e9(T, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : s0("ColorSpace set to invalid value.");
-                    for (var g0 = 0; g0 < 3; g0++) o[m + g0] = o[m + g0] < 0 ? 0 : o[m + g0], o[m + g0] = o[m + g0] > 1 ? 1 : o[m + g0]
+                    } else t.colorSpace === r0.DIVERGING ? (e9(x, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : i0("ColorSpace set to invalid value.");
+                    for (var l0 = 0; l0 < 3; l0++) o[m + l0] = o[m + l0] < 0 ? 0 : o[m + l0], o[m + l0] = o[m + l0] > 1 ? 1 : o[m + l0]
                 }
             }
         }, e.getUint8Table = function(r, n, a) {
             var o = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : !1;
             if (e.getMTime() <= t.buildTime && t.tableSize === a && t.tableWithAlpha !== o) return t.table;
-            if (t.nodes.length === 0) return s0("Attempting to lookup a value with no points in the function"), t.table;
+            if (t.nodes.length === 0) return i0("Attempting to lookup a value with no points in the function"), t.table;
             var c = o ? 4 : 3;
             (t.tableSize !== a || t.tableWithAlpha !== o) && (t.table = new Uint8Array(a * c), t.tableSize = a, t.tableWithAlpha = o);
             var s = [];
             e.getTable(r, n, a, s);
             for (var u = 0; u < a; u++) t.table[u * c + 0] = Math.floor(s[u * 3 + 0] * 255 + .5), t.table[u * c + 1] = Math.floor(s[u * 3 + 1] * 255 + .5), t.table[u * c + 2] = Math.floor(s[u * 3 + 2] * 255 + .5), o && (t.table[u * c + 3] = 255);
             return t.buildTime.modified(), t.table
         }, e.buildFunctionFromTable = function(r, n, a, o) {
@@ -4311,17 +4311,17 @@
                     sharpness: 0,
                     midpoint: .5
                 };
                 t.nodes.push(u)
             }
             e.sortAndUpdateRange()
         }, e.getNodeValue = function(r, n) {
-            return r < 0 || r >= t.nodes.length ? (s0("Index out of range!"), -1) : (n[0] = t.nodes[r].x, n[1] = t.nodes[r].r, n[2] = t.nodes[r].g, n[3] = t.nodes[r].b, n[4] = t.nodes[r].midpoint, n[5] = t.nodes[r].sharpness, 1)
+            return r < 0 || r >= t.nodes.length ? (i0("Index out of range!"), -1) : (n[0] = t.nodes[r].x, n[1] = t.nodes[r].r, n[2] = t.nodes[r].g, n[3] = t.nodes[r].b, n[4] = t.nodes[r].midpoint, n[5] = t.nodes[r].sharpness, 1)
         }, e.setNodeValue = function(r, n) {
-            if (r < 0 || r >= t.nodes.length) return s0("Index out of range!"), -1;
+            if (r < 0 || r >= t.nodes.length) return i0("Index out of range!"), -1;
             var a = t.nodes[r].x;
             return t.nodes[r].x = n[0], t.nodes[r].r = n[1], t.nodes[r].g = n[2], t.nodes[r].b = n[3], t.nodes[r].midpoint = n[4], t.nodes[r].sharpness = n[5], a !== n[0] ? e.sortAndUpdateRange() : e.modified(), 1
         }, e.getNumberOfAvailableColors = function() {
             return t.indexedLookup && e.getSize() ? e.getSize() : t.tableSize ? t.tableSize : 16777216
         }, e.getIndexedColor = function(r, n) {
             var a = e.getSize();
             if (a > 0 && r >= 0) {
@@ -4338,15 +4338,15 @@
                 for (var a = 0; a < r; a++) e.addRGBPoint(n[a * 4], n[a * 4 + 1], n[a * 4 + 2], n[a * 4 + 3])
             }
         }, e.setMappingRange = function(r, n) {
             var a = [r, n],
                 o = e.getRange();
             if (!(o[1] === a[1] && o[0] === a[0])) {
                 if (a[1] === a[0]) {
-                    s0("attempt to set zero width color range");
+                    i0("attempt to set zero width color range");
                     return
                 }
                 for (var c = (a[1] - a[0]) / (o[1] - o[0]), s = a[0] - o[0] * c, u = 0; u < t.nodes.length; ++u) t.nodes[u].x = t.nodes[u].x * c + s;
                 t.mappingRange[0] = a[0], t.mappingRange[1] = a[1], e.modified()
             }
         }, e.adjustRange = function(r) {
             var n = e.getRange(),
@@ -4393,20 +4393,20 @@
                 }
             if (a === K0.LUMINANCE)
                 for (var C = 0; C < s; C++) {
                     var N = f[C * u + o];
                     e.getColor(N, g), i[C] = Math.floor(g[0] * 76.5 + g[1] * 150.45 + g[2] * 28.05 + .5)
                 }
             if (a === K0.LUMINANCE_ALPHA)
-                for (var x = 0; x < s; x++) {
-                    var B = f[x * u + o];
-                    e.getColor(B, g), i[x * 2] = Math.floor(g[0] * 76.5 + g[1] * 150.45 + g[2] * 28.05 + .5), i[x * 2 + 1] = c
+                for (var R = 0; R < s; R++) {
+                    var B = f[R * u + o];
+                    e.getColor(B, g), i[R * 2] = Math.floor(g[0] * 76.5 + g[1] * 150.45 + g[2] * 28.05 + .5), i[R * 2 + 1] = c
                 }
         }, e.applyColorMap = function(r) {
-            if (r.ColorSpace && (t.colorSpace = n0[r.ColorSpace.toUpperCase()], t.colorSpace === void 0 && (s0("ColorSpace ".concat(r.ColorSpace, " not supported, using RGB instead")), t.colorSpace = n0.RGB)), r.NanColor)
+            if (r.ColorSpace && (t.colorSpace = r0[r.ColorSpace.toUpperCase()], t.colorSpace === void 0 && (i0("ColorSpace ".concat(r.ColorSpace, " not supported, using RGB instead")), t.colorSpace = r0.RGB)), r.NanColor)
                 for (t.nanColor = [].concat(r.NanColor); t.nanColor.length < 4;) t.nanColor.push(1);
             if (r.RGBPoints) {
                 var n = r.RGBPoints.length;
                 t.nodes = [];
                 for (var a = .5, o = 0, c = 0; c < n; c += 4) t.nodes.push({
                     x: r.RGBPoints[c],
                     r: r.RGBPoints[c + 1],
@@ -4415,17 +4415,17 @@
                     midpoint: a,
                     sharpness: o
                 })
             }
             e.sortAndUpdateRange()
         }
     }
-    var R8 = {
+    var x8 = {
         clamping: !0,
-        colorSpace: n0.RGB,
+        colorSpace: r0.RGB,
         hSVWrap: !0,
         scale: J2.LINEAR,
         nanColor: null,
         belowRangeColor: null,
         aboveRangeColor: null,
         useAboveRangeColor: !1,
         useBelowRangeColor: !1,
@@ -4436,15 +4436,15 @@
         nodes: null,
         discretize: !1,
         numberOfValues: 256
     };
 
     function t9(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, R8, r), q2.extend(e, t, r), t.table = [], t.nodes = [], t.nanColor = [.5, 0, 0, 1], t.belowRangeColor = [0, 0, 0, 1], t.aboveRangeColor = [1, 1, 1, 1], t.buildTime = {}, W.obj(t.buildTime), W.get(e, t, ["buildTime", "mappingRange"]), W.setGet(e, t, ["useAboveRangeColor", "useBelowRangeColor", "colorSpace", "discretize", "numberOfValues"]), W.setArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"], 4), W.getArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"]), x8(e, t)
+        Object.assign(t, x8, r), q2.extend(e, t, r), t.table = [], t.nodes = [], t.nanColor = [.5, 0, 0, 1], t.belowRangeColor = [0, 0, 0, 1], t.aboveRangeColor = [1, 1, 1, 1], t.buildTime = {}, W.obj(t.buildTime), W.get(e, t, ["buildTime", "mappingRange"]), W.setGet(e, t, ["useAboveRangeColor", "useBelowRangeColor", "colorSpace", "discretize", "numberOfValues"]), W.setArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"], 4), W.getArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"]), R8(e, t)
     }
     var O8 = W.newInstance(t9, "vtkColorTransferFunction"),
         T8 = S8({
             newInstance: O8,
             extend: t9
         }, k1),
         M8 = [{
@@ -5252,42 +5252,42 @@
             RGBPoints: [0, .267004, .004874, .329415, .003922, .26851, .009605, .335427, .007843, .269944, .014625, .341379, .011765, .271305, .019942, .347269, .015686, .272594, .025563, .353093, .019608, .273809, .031497, .358853, .023529, .274952, .037752, .364543, .027451, .276022, .044167, .370164, .031373, .277018, .050344, .375715, .035294, .277941, .056324, .381191, .039216, .278791, .062145, .386592, .043137, .279566, .067836, .391917, .047059, .280267, .073417, .397163, .05098, .280894, .078907, .402329, .054902, .281446, .08432, .407414, .058824, .281924, .089666, .412415, .062745, .282327, .094955, .417331, .066667, .282656, .100196, .42216, .070588, .28291, .105393, .426902, .07451, .283091, .110553, .431554, .078431, .283197, .11568, .436115, .082353, .283229, .120777, .440584, .086275, .283187, .125848, .44496, .090196, .283072, .130895, .449241, .094118, .282884, .13592, .453427, .098039, .282623, .140926, .457517, .101961, .28229, .145912, .46151, .105882, .281887, .150881, .465405, .109804, .281412, .155834, .469201, .113725, .280868, .160771, .472899, .117647, .280255, .165693, .476498, .121569, .279574, .170599, .479997, .12549, .278826, .17549, .483397, .129412, .278012, .180367, .486697, .133333, .277134, .185228, .489898, .137255, .276194, .190074, .493001, .141176, .275191, .194905, .496005, .145098, .274128, .199721, .498911, .14902, .273006, .20452, .501721, .152941, .271828, .209303, .504434, .156863, .270595, .214069, .507052, .160784, .269308, .218818, .509577, .164706, .267968, .223549, .512008, .168627, .26658, .228262, .514349, .172549, .265145, .232956, .516599, .176471, .263663, .237631, .518762, .180392, .262138, .242286, .520837, .184314, .260571, .246922, .522828, .188235, .258965, .251537, .524736, .192157, .257322, .25613, .526563, .196078, .255645, .260703, .528312, .2, .253935, .265254, .529983, .203922, .252194, .269783, .531579, .207843, .250425, .27429, .533103, .211765, .248629, .278775, .534556, .215686, .246811, .283237, .535941, .219608, .244972, .287675, .53726, .223529, .243113, .292092, .538516, .227451, .241237, .296485, .539709, .231373, .239346, .300855, .540844, .235294, .237441, .305202, .541921, .239216, .235526, .309527, .542944, .243137, .233603, .313828, .543914, .247059, .231674, .318106, .544834, .25098, .229739, .322361, .545706, .254902, .227802, .326594, .546532, .258824, .225863, .330805, .547314, .262745, .223925, .334994, .548053, .266667, .221989, .339161, .548752, .270588, .220057, .343307, .549413, .27451, .21813, .347432, .550038, .278431, .21621, .351535, .550627, .282353, .214298, .355619, .551184, .286275, .212395, .359683, .55171, .290196, .210503, .363727, .552206, .294118, .208623, .367752, .552675, .298039, .206756, .371758, .553117, .301961, .204903, .375746, .553533, .305882, .203063, .379716, .553925, .309804, .201239, .38367, .554294, .313725, .19943, .387607, .554642, .317647, .197636, .391528, .554969, .321569, .19586, .395433, .555276, .32549, .1941, .399323, .555565, .329412, .192357, .403199, .555836, .333333, .190631, .407061, .556089, .337255, .188923, .41091, .556326, .341176, .187231, .414746, .556547, .345098, .185556, .41857, .556753, .34902, .183898, .422383, .556944, .352941, .182256, .426184, .55712, .356863, .180629, .429975, .557282, .360784, .179019, .433756, .55743, .364706, .177423, .437527, .557565, .368627, .175841, .44129, .557685, .372549, .174274, .445044, .557792, .376471, .172719, .448791, .557885, .380392, .171176, .45253, .557965, .384314, .169646, .456262, .55803, .388235, .168126, .459988, .558082, .392157, .166617, .463708, .558119, .396078, .165117, .467423, .558141, .4, .163625, .471133, .558148, .403922, .162142, .474838, .55814, .407843, .160665, .47854, .558115, .411765, .159194, .482237, .558073, .415686, .157729, .485932, .558013, .419608, .15627, .489624, .557936, .423529, .154815, .493313, .55784, .427451, .153364, .497, .557724, .431373, .151918, .500685, .557587, .435294, .150476, .504369, .55743, .439216, .149039, .508051, .55725, .443137, .147607, .511733, .557049, .447059, .14618, .515413, .556823, .45098, .144759, .519093, .556572, .454902, .143343, .522773, .556295, .458824, .141935, .526453, .555991, .462745, .140536, .530132, .555659, .466667, .139147, .533812, .555298, .470588, .13777, .537492, .554906, .47451, .136408, .541173, .554483, .478431, .135066, .544853, .554029, .482353, .133743, .548535, .553541, .486275, .132444, .552216, .553018, .490196, .131172, .555899, .552459, .494118, .129933, .559582, .551864, .498039, .128729, .563265, .551229, .501961, .127568, .566949, .550556, .505882, .126453, .570633, .549841, .509804, .125394, .574318, .549086, .513725, .124395, .578002, .548287, .517647, .123463, .581687, .547445, .521569, .122606, .585371, .546557, .52549, .121831, .589055, .545623, .529412, .121148, .592739, .544641, .533333, .120565, .596422, .543611, .537255, .120092, .600104, .54253, .541176, .119738, .603785, .5414, .545098, .119512, .607464, .540218, .54902, .119423, .611141, .538982, .552941, .119483, .614817, .537692, .556863, .119699, .61849, .536347, .560784, .120081, .622161, .534946, .564706, .120638, .625828, .533488, .568627, .12138, .629492, .531973, .572549, .122312, .633153, .530398, .576471, .123444, .636809, .528763, .580392, .12478, .640461, .527068, .584314, .126326, .644107, .525311, .588235, .128087, .647749, .523491, .592157, .130067, .651384, .521608, .596078, .132268, .655014, .519661, .6, .134692, .658636, .517649, .603922, .137339, .662252, .515571, .607843, .14021, .665859, .513427, .611765, .143303, .669459, .511215, .615686, .146616, .67305, .508936, .619608, .150148, .676631, .506589, .623529, .153894, .680203, .504172, .627451, .157851, .683765, .501686, .631373, .162016, .687316, .499129, .635294, .166383, .690856, .496502, .639216, .170948, .694384, .493803, .643137, .175707, .6979, .491033, .647059, .180653, .701402, .488189, .65098, .185783, .704891, .485273, .654902, .19109, .708366, .482284, .658824, .196571, .711827, .479221, .662745, .202219, .715272, .476084, .666667, .20803, .718701, .472873, .670588, .214, .722114, .469588, .67451, .220124, .725509, .466226, .678431, .226397, .728888, .462789, .682353, .232815, .732247, .459277, .686275, .239374, .735588, .455688, .690196, .24607, .73891, .452024, .694118, .252899, .742211, .448284, .698039, .259857, .745492, .444467, .701961, .266941, .748751, .440573, .705882, .274149, .751988, .436601, .709804, .281477, .755203, .432552, .713725, .288921, .758394, .428426, .717647, .296479, .761561, .424223, .721569, .304148, .764704, .419943, .72549, .311925, .767822, .415586, .729412, .319809, .770914, .411152, .733333, .327796, .77398, .40664, .737255, .335885, .777018, .402049, .741176, .344074, .780029, .397381, .745098, .35236, .783011, .392636, .74902, .360741, .785964, .387814, .752941, .369214, .788888, .382914, .756863, .377779, .791781, .377939, .760784, .386433, .794644, .372886, .764706, .395174, .797475, .367757, .768627, .404001, .800275, .362552, .772549, .412913, .803041, .357269, .776471, .421908, .805774, .35191, .780392, .430983, .808473, .346476, .784314, .440137, .811138, .340967, .788235, .449368, .813768, .335384, .792157, .458674, .816363, .329727, .796078, .468053, .818921, .323998, .8, .477504, .821444, .318195, .803922, .487026, .823929, .312321, .807843, .496615, .826376, .306377, .811765, .506271, .828786, .300362, .815686, .515992, .831158, .294279, .819608, .525776, .833491, .288127, .823529, .535621, .835785, .281908, .827451, .545524, .838039, .275626, .831373, .555484, .840254, .269281, .835294, .565498, .84243, .262877, .839216, .575563, .844566, .256415, .843137, .585678, .846661, .249897, .847059, .595839, .848717, .243329, .85098, .606045, .850733, .236712, .854902, .616293, .852709, .230052, .858824, .626579, .854645, .223353, .862745, .636902, .856542, .21662, .866667, .647257, .8584, .209861, .870588, .657642, .860219, .203082, .87451, .668054, .861999, .196293, .878431, .678489, .863742, .189503, .882353, .688944, .865448, .182725, .886275, .699415, .867117, .175971, .890196, .709898, .868751, .169257, .894118, .720391, .87035, .162603, .898039, .730889, .871916, .156029, .901961, .741388, .873449, .149561, .905882, .751884, .874951, .143228, .909804, .762373, .876424, .137064, .913725, .772852, .877868, .131109, .917647, .783315, .879285, .125405, .921569, .79376, .880678, .120005, .92549, .804182, .882046, .114965, .929412, .814576, .883393, .110347, .933333, .82494, .88472, .106217, .937255, .83527, .886029, .102646, .941176, .845561, .887322, .099702, .945098, .85581, .888601, .097452, .94902, .866013, .889868, .095953, .952941, .876168, .891125, .09525, .956863, .886271, .892374, .095374, .960784, .89632, .893616, .096335, .964706, .906311, .894855, .098125, .968627, .916242, .896091, .100717, .972549, .926106, .89733, .104071, .976471, .935904, .89857, .108131, .980392, .945636, .899815, .112838, .984314, .9553, .901065, .118128, .988235, .964894, .902323, .123941, .992157, .974417, .90359, .130215, .996078, .983868, .904867, .136897, 1, .993248, .906157, .143936]
         }, {
             ShowIndexedColorActiveValues: 1,
             IndexedColors: [.07, .5, .7, 1, 1, 1, .85, 1, 1, .8, .5, 1, .76, 1, 0, 1, .71, .71, .5, .5, .5, .05, .05, 1, 1, .05, .05, .7, 1, 1, .7, .89, .96, .67, .36, .95, .54, 1, 0, .75, .65, .65, .5, .6, .6, 1, .5, 0, 1, 1, .19, .12, .94, .12, .5, .82, .89, .56, .25, .83, .24, 1, 0, .9, .9, .9, .75, .76, .78, .65, .65, .67, .54, .6, .78, .61, .48, .78, .5, .48, .78, .44, .48, .78, .36, .48, .76, 1, .48, .38, .49, .5, .69, .76, .56, .56, .4, .56, .56, .74, .5, .89, 1, .63, 0, .65, .16, .16, .36, .72, .82, .44, .18, .69, 0, 1, 0, .58, 1, 1, .58, .88, .88, .45, .76, .79, .33, .71, .71, .23, .62, .62, .14, .56, .56, .04, .49, .55, 0, .41, .52, .88, .88, 1, 1, .85, .56, .65, .46, .45, .4, .5, .5, .62, .39, .71, .83, .48, 0, .58, 0, .58, .26, .62, .69, .34, .09, .56, 0, .79, 0, .44, .83, 1, 1, 1, .78, .85, 1, .78, .78, 1, .78, .64, 1, .78, .56, 1, .78, .38, 1, .78, .27, 1, .78, .19, 1, .78, .12, 1, .78, 0, 1, .61, 0, .9, .46, 0, .83, .32, 0, .75, .22, 0, .67, .14, .3, .76, 1, .3, .65, 1, .13, .58, .84, .15, .49, .67, .15, .4, .59, .09, .33, .53, .96, .93, .82, .8, .82, .12, .71, .71, .76, .65, .33, .3, .34, .35, .38, .62, .31, .71, .67, .36, 0, .46, .31, .27, .26, .51, .59, .26, 0, .4, 0, .49, 0, .44, .67, .98, 0, .73, 1, 0, .63, 1, 0, .56, 1, 0, .5, 1, 0, .42, 1, .33, .36, .95, .47, .36, .89, .54, .31, .89, .63, .21, .83, .7, .12, .83, .7, .12, .73, .7, .05, .65, .74, .05, .53, .78, 0, .4, .8, 0, .35, .82, 0, .31, .85, 0, .27, .88, 0, .22, .9, 0, .18, .91, 0, .15, .92, 0, .14, .93, 0, .13, .94, 0, .12, .95, 0, .11, .96, 0, .1, .97, 0, .09, .98, 0, .08, .99, 0, .07, 1, 0, .06],
             Annotations: [0, "Xx", 1, "H", 2, "He", 3, "Li", 4, "Be", 5, "B", 6, "C", 7, "N", 8, "O", 9, "F", 10, "Ne", 11, "Na", 12, "Mg", 13, "Al", 14, "Si", 15, "P", 16, "S", 17, "Cl", 18, "Ar", 19, "K", 20, "Ca", 21, "Sc", 22, "Ti", 23, "V", 24, "Cr", 25, "Mn", 26, "Fe", 27, "Co", 28, "Ni", 29, "Cu", 30, "Zn", 31, "Ga", 32, "Ge", 33, "As", 34, "Se", 35, "Br", 36, "Kr", 37, "Rb", 38, "Sr", 39, "Y", 40, "Zr", 41, "Nb", 42, "Mo", 43, "Tc", 44, "Ru", 45, "Rh", 46, "Pd", 47, "Ag", 48, "Cd", 49, "In", 50, "Sn", 51, "Sb", 52, "Te", 53, "I", 54, "Xe", 55, "Cs", 56, "Ba", 57, "La", 58, "Ce", 59, "Pr", 60, "Nd", 61, "Pm", 62, "Sm", 63, "Eu", 64, "Gd", 65, "Tb", 66, "Dy", 67, "Ho", 68, "Er", 69, "Tm", 70, "Yb", 71, "Lu", 72, "Hf", 73, "Ta", 74, "W", 75, "Re", 76, "Os", 77, "Ir", 78, "Pt", 79, "Au", 80, "Hg", 81, "Tl", 82, "Pb", 83, "Bi", 84, "Po", 85, "At", 86, "Rn", 87, "Fr", 88, "Ra", 89, "Ac", 90, "Th", 91, "Pa", 92, "U", 93, "Np", 94, "Pu", 95, "Am", 96, "Cm", 97, "Bk", 98, "Cf", 99, "Es", 100, "Fm", 101, "Md", 102, "No", 103, "Lr", 104, "Rf", 105, "Db", 106, "Sg", 107, "Bh", 108, "Hs", 109, "Mt", 110, "Ds", 111, "Rg", 112, "Cn", 113, "Uut", 114, "Uuq", 115, "Uup", 116, "Uuh", 117, "Uus", 118, "Uuo"],
             Name: "BlueObeliskElements"
         }],
-        G0 = Object.create(null);
+        M0 = Object.create(null);
     M8.filter(function(e) {
         return e.RGBPoints
     }).filter(function(e) {
         return e.ColorSpace !== "CIELAB"
     }).forEach(function(e) {
-        G0[e.Name] = e
+        M0[e.Name] = e
     });
-    var E0 = Object.keys(G0);
-    E0.sort();
+    var G0 = Object.keys(M0);
+    G0.sort();
 
     function G8(e) {
-        return G0[e]
+        return M0[e]
     }
 
     function E8(e) {
-        !e.RGBPoints || e.ColorSpace === "CIELAB" || (G0[e.Name] || (E0.push(e.Name), E0.sort()), G0[e.Name] = e)
+        !e.RGBPoints || e.ColorSpace === "CIELAB" || (M0[e.Name] || (G0.push(e.Name), G0.sort()), M0[e.Name] = e)
     }
 
     function k8(e) {
-        var t = E0.indexOf(e);
-        t > -1 && E0.splice(t, 1), delete G0[e]
+        var t = G0.indexOf(e);
+        t > -1 && G0.splice(t, 1), delete M0[e]
     }
     var r9 = {
         addPreset: E8,
         removePresetByName: k8,
         getPresetByName: G8,
-        rgbPresetNames: E0
+        rgbPresetNames: G0
     };
     const D1 = document.createElement("canvas");
     D1.width = 100, D1.height = 100;
 
     function D8(e, t, r, n) {
         const o = D1.getContext("2d").createImageData(e, t);
         for (let c = 0; c < t; c++)
@@ -5296,15 +5296,15 @@
                     i = n(r[u]);
                 o.data[u * 4 + 0] = i[0], o.data[u * 4 + 1] = i[1], o.data[u * 4 + 2] = i[2], o.data[u * 4 + 3] = 255
             }
         return o
     }
     const {
         ref: n9,
-        computed: c0,
+        computed: u0,
         onMounted: L8,
         nextTick: A8,
         watch: J0
     } = window.Vue, a9 = {
         props: {
             heatmap: {
                 type: [Array, Float32Array, Float64Array, Uint8Array, Uint16Array, Uint32Array, Int8Array, Int16Array, Int32Array],
@@ -5337,99 +5337,99 @@
                 o = T8.newInstance();
             o.applyColorMap(r9.getPresetByName(e.colorPreset));
             const c = [0, 0, 0, 255];
 
             function s(S) {
                 return o.getColor(S, c), c[0] *= 255, c[1] *= 255, c[2] *= 255, c
             }
-            const u = c0(() => e.shape[0]),
-                i = c0(() => e.shape[1]),
-                f = c0(() => {
+            const u = u0(() => e.shape[0]),
+                i = u0(() => e.shape[1]),
+                f = u0(() => {
                     let S = e.heatmap[0],
-                        w = e.heatmap[0];
+                        b = e.heatmap[0];
                     for (let v = 0; v < e.heatmap.length; v++) {
                         const d = e.heatmap[v];
-                        S > d && (S = d), w < d && (w = d)
+                        S > d && (S = d), b < d && (b = d)
                     }
-                    return t("fullRange", [S, w]), [S, w]
+                    return t("fullRange", [S, b]), [S, b]
                 }),
-                g = c0(() => {
-                    const [S, w] = f.value, v = Math.max(-S, w);
+                g = u0(() => {
+                    const [S, b] = f.value, v = Math.max(-S, b);
                     return [-v, v]
                 }),
-                l = c0(() => {
-                    const [S, w] = f.value, v = Math.min(-S, w);
+                l = u0(() => {
+                    const [S, b] = f.value, v = Math.min(-S, b);
                     return [-v, v]
                 }),
-                p = c0(() => {
+                p = u0(() => {
                     const [, S] = f.value;
                     return S < 0 ? [S, 0] : [0, S]
                 }),
-                y = c0(() => {
+                y = u0(() => {
                     const [S] = f.value;
                     return S > 0 ? [0, S] : [S, 0]
                 }),
-                h = c0(() => ({
+                h = u0(() => ({
                     full: f.value,
                     maxSym: g.value,
                     minSym: l.value,
                     positive: p.value,
                     negative: y.value,
                     custom: e.colorRange.map(Number)
                 })),
-                C = c0(() => h.value[e.colorMode] || f.value);
+                C = u0(() => h.value[e.colorMode] || f.value);
 
             function N() {
-                const [S, w] = C.value;
-                if (!u.value || !i.value || !(w - S) || !e.heatmap || (t("colorRange", [S, w]), o.setMappingRange(S, w), o.updateRange(), !u.value || !i.value)) return;
+                const [S, b] = C.value;
+                if (!u.value || !i.value || !(b - S) || !e.heatmap || (t("colorRange", [S, b]), o.setMappingRange(S, b), o.updateRange(), !u.value || !i.value)) return;
                 const v = D8(u.value, i.value, e.heatmap, s),
                     d = n.value.getContext("2d");
                 d.imageSmoothingEnabled = !1, d.clearRect(0, 0, u.value, i.value), d.putImageData(v, 0, 0)
             }
 
-            function x() {
+            function R() {
                 A8(N)
             }
 
             function B(S) {
                 const {
-                    clientX: w,
+                    clientX: b,
                     clientY: v
                 } = S, {
                     top: d,
                     left: m,
-                    width: O,
+                    width: T,
                     height: D
-                } = a.value, _ = (w - m) / O, U = 1 - (v - d) / D, F = Math.round(_ * (u.value - 1)), T = Math.round(U * (i.value - 1));
+                } = a.value, P = (b - m) / T, F = 1 - (v - d) / D, _ = Math.round(P * (u.value - 1)), x = Math.round(F * (i.value - 1));
                 t("hover", {
-                    i: F,
-                    j: T
+                    i: _,
+                    j: x
                 })
             }
 
-            function b() {
+            function w() {
                 t("enter"), a.value = n.value.getBoundingClientRect()
             }
-            return J0(() => C.value, x), J0(() => e.shape, x), J0(() => e.heatmap, x), J0(() => e.colorPreset, S => {
-                o.applyColorMap(r9.getPresetByName(S)), x()
-            }), L8(x), r({
+            return J0(() => C.value, R), J0(() => e.shape, R), J0(() => e.heatmap, R), J0(() => e.colorPreset, S => {
+                o.applyColorMap(r9.getPresetByName(S)), R()
+            }), L8(R), r({
                 render: N
             }), {
                 canvasElem: n,
                 width: u,
                 height: i,
                 fullRange: f,
                 maxSymRange: g,
                 minSymRange: l,
                 positiveRange: p,
                 negativeRange: y,
                 colorRanges: h,
                 colorRangeToUse: C,
                 onMouseMove: B,
-                onMouseEnter: b,
+                onMouseEnter: w,
                 emit: t
             }
         },
         template: `
     <canvas 
         ref="canvasElem" 
         :width="width" 
@@ -5536,60 +5536,60 @@
                 g = j0({
                     position: "absolute",
                     top: 0,
                     left: 0
                 }),
                 l = Q0(() => {
                     e.areaSelected;
-                    const b = e.areaSelectedOpacity ?? c.value,
+                    const w = e.areaSelectedOpacity ?? c.value,
                         S = e.areaOpacity ?? s.value;
-                    return e.areas.map((w, v) => ({
-                        ...w,
-                        opacity: N(v) ? b : S,
+                    return e.areas.map((b, v) => ({
+                        ...b,
+                        opacity: N(v) ? w : S,
                         color: e.colors[v % e.colors.length]
                     }))
                 }),
                 p = Q0(() => e.heatmaps && e.heatmaps[e.heatmapActive]),
                 y = Q0(() => ({
                     ...g.value,
                     opacity: e.heatmapOpacity
                 })),
                 h = Q0(() => [a.value, o.value]);
 
             function C() {
                 f.height = "auto", f.width = "auto";
-                const b = {
+                const w = {
                     ...g.value
                 };
-                e.maxHeight ? (f.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`, b.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`) : (delete f.maxHeight, delete b.maxHeight), e.maxWidth ? (f.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`, b.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`) : (f.maxWidth = "100%", b.maxWidth = "100%"), e.width ? (i.width = e.width, f.width = e.width, b.width = e.width) : (delete i.width, delete b.width), g.value = b
+                e.maxHeight ? (f.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`, w.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`) : (delete f.maxHeight, delete w.maxHeight), e.maxWidth ? (f.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`, w.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`) : (f.maxWidth = "100%", w.maxWidth = "100%"), e.width ? (i.width = e.width, f.width = e.width, w.width = e.width) : (delete i.width, delete w.width), g.value = w
             }
 
-            function N(b) {
-                const S = e.areas[b][e.areaKey];
-                return e.areaSelected ? !!e.areaSelected.find(w => S == w) : !1
+            function N(w) {
+                const S = e.areas[w][e.areaKey];
+                return e.areaSelected ? !!e.areaSelected.find(b => S == b) : !1
             }
 
-            function x(b, S) {
-                const w = e.areas[b];
-                u[w[e.areaKey]] = S;
+            function R(w, S) {
+                const b = e.areas[w];
+                u[b[e.areaKey]] = S;
                 const v = [];
                 for (let d = 0; d < e.areas.length; d++) {
                     const m = e.areas[d][this.areaKey];
                     u[m] && v.push(m)
                 }
                 t("areaSelectionChange", v)
             }
 
             function B() {
                 a.value = this.width, o.value = this.height
             }
             return n.addEventListener("load", B), _8(() => {
                 n.removeEventListener("load", B)
             }), $8(() => n.src = e.src), o9(() => e.maxWidth, C), o9(() => e.maxHeight, C), r({
-                updateAreaSelection: x
+                updateAreaSelection: R
             }), C(), {
                 ...P8(e),
                 imageWidth: a,
                 imageHeight: o,
                 areaSelectedOpacityValue: c,
                 areaOpacityValue: s,
                 containerStyle: i,
@@ -5631,18 +5631,18 @@
           :opacity="item.opacity"
           fill="none"
           v-bind="areaStyle"
         />
       </svg>
     </div>`
     }, {
-        ref: q,
+        ref: K,
         computed: Z0,
         watch: A1,
-        unref: R,
+        unref: O,
         toRefs: U8,
         onMounted: F8,
         onBeforeUnmount: V8
     } = window.Vue, i9 = {
         TrameClientStateChange: c9,
         TrameClientTriggers: g9,
         TrameCursor: m9,
@@ -5676,126 +5676,126 @@
                     type: Array,
                     default () {
                         return [-1, 1, -1, 1, -1, 1]
                     }
                 },
                 image: {
                     default: null
+                },
+                nbSliders: {
+                    type: Number,
+                    default: 0
                 }
             },
             emit: ["update-seed"],
             setup(e, {
                 emit: t
             }) {
                 let r = 0,
                     n = null,
                     a = null;
-                const o = q(null),
-                    c = q([0, 0]),
-                    s = q(1),
-                    u = q(10),
-                    i = q([0, 0]),
-                    f = q([0, 0]),
-                    g = q(!1),
-                    l = q(e.point1[0]),
-                    p = q(e.point1[1]),
-                    y = q(e.point1[2]),
-                    h = q(e.point2[0]),
-                    C = q(e.point2[1]),
-                    N = q(e.point2[2]),
-                    x = q(!0),
-                    B = q(50),
-                    b = Z0(() => R(x) ? "#2196F3" : "#4CAF50"),
-                    S = Z0(() => (e.bounds[5] - e.bounds[4]) / e.numberOfSteps),
+                const o = K(null),
+                    c = K([0, 0]),
+                    s = K(1),
+                    u = K(10),
+                    i = K([0, 0]),
+                    f = K([0, 0]),
+                    g = K(!1),
+                    l = K(e.point1[0]),
+                    p = K(e.point1[1]),
+                    y = K(e.point1[2]),
+                    h = K(e.point2[0]),
+                    C = K(e.point2[1]),
+                    N = K(e.point2[2]),
+                    R = Z0(() => O(e.nbSliders) == 2 ? "#4CAF50" : "#2196F3"),
+                    B = Z0(() => (e.bounds[5] - e.bounds[4]) / e.numberOfSteps),
                     w = Z0(() => (e.bounds[3] - e.bounds[2]) / 500),
-                    v = Z0(() => (e.bounds[5] - e.bounds[4]) / 500);
+                    S = Z0(() => (e.bounds[5] - e.bounds[4]) / 500);
 
-                function d() {
-                    i.value = [500 - (R(p) - e.bounds[2]) / R(w), 500 - (R(y) - e.bounds[4]) / R(v)], f.value = [500 - (R(C) - e.bounds[2]) / R(w), 500 - (R(N) - e.bounds[4]) / R(v)]
+                function b() {
+                    i.value = [500 - (O(p) - e.bounds[2]) / O(w), 500 - (O(y) - e.bounds[4]) / O(S)], f.value = [500 - (O(C) - e.bounds[2]) / O(w), 500 - (O(N) - e.bounds[4]) / O(S)]
                 }
 
-                function m() {
-                    if (!R(g)) return;
-                    const L = R(x) ? l : h;
+                function v() {
+                    if (!O(g)) return;
+                    const _ = e.nbSliders == 1 ? l : h;
                     t("update-seed", {
-                        p1: [R(l), R(p), R(y)],
-                        p2: [R(L), R(C), R(N)]
+                        p1: [O(l), O(p), O(y)],
+                        p2: [O(_), O(C), O(N)]
                     })
                 }
 
-                function O(L) {
-                    if (R(g) || (g.value = !0), r) {
-                        const V = n.clientX - L.clientX,
-                            Q = n.clientY - L.clientY;
+                function d(_) {
+                    if (O(g) || (g.value = !0), r) {
+                        const x = n.clientX - _.clientX,
+                            j = n.clientY - _.clientY;
                         switch (r) {
                             case 1:
-                                i.value = [a[0] - R(s) * V, a[1] - R(s) * Q], p.value = (500 - R(i)[0]) * R(w) + e.bounds[2], y.value = (500 - R(i)[1]) * R(v) + e.bounds[4];
+                                i.value = [a[0] - O(s) * x, a[1] - O(s) * j], p.value = (500 - O(i)[0]) * O(w) + e.bounds[2], y.value = (500 - O(i)[1]) * O(S) + e.bounds[4];
                                 break;
                             case 2:
-                                f.value = [a[0] - R(s) * V, a[1] - R(s) * Q], C.value = (500 - R(f)[0]) * R(w) + e.bounds[2], N.value = (500 - R(f)[1]) * R(v) + e.bounds[4];
+                                f.value = [a[0] - O(s) * x, a[1] - O(s) * j], C.value = (500 - O(f)[0]) * O(w) + e.bounds[2], N.value = (500 - O(f)[1]) * O(S) + e.bounds[4];
                                 break;
                             case 3:
-                                i.value = [a[0][0] - R(s) * V, a[0][1] - R(s) * Q], p.value = (500 - R(i)[0]) * R(w) + e.bounds[2], y.value = (500 - R(i)[1]) * R(v) + e.bounds[4], f.value = [a[1][0] - R(s) * V, a[1][1] - R(s) * Q], C.value = (500 - R(f)[0]) * R(w) + e.bounds[2], N.value = (500 - R(f)[1]) * R(v) + e.bounds[4];
+                                i.value = [a[0][0] - O(s) * x, a[0][1] - O(s) * j], p.value = (500 - O(i)[0]) * O(w) + e.bounds[2], y.value = (500 - O(i)[1]) * O(S) + e.bounds[4], f.value = [a[1][0] - O(s) * x, a[1][1] - O(s) * j], C.value = (500 - O(f)[0]) * O(w) + e.bounds[2], N.value = (500 - O(f)[1]) * O(S) + e.bounds[4];
                                 break
                         }
-                        const K = [R(i)[0] - R(f)[0], R(i)[1] - R(f)[1]],
-                            a0 = Math.sqrt(K[0] * K[0] + K[1] * K[1]);
-                        a0 > 1e-4 && (K[0] /= a0, K[1] /= a0), c.value = K, m()
+                        const V = [O(i)[0] - O(f)[0], O(i)[1] - O(f)[1]],
+                            e0 = Math.sqrt(V[0] * V[0] + V[1] * V[1]);
+                        e0 > 1e-4 && (V[0] /= e0, V[1] /= e0), c.value = V, v()
                     }
                 }
 
-                function D(L, V) {
-                    switch (r = L, n = V, L) {
+                function m(_, x) {
+                    switch (r = _, n = x, _) {
                         case 1:
-                            a = R(i).slice();
+                            a = O(i).slice();
                             break;
                         case 2:
-                            a = R(f).slice();
+                            a = O(f).slice();
                             break;
                         case 3:
-                            a = [R(i).slice(), R(f).slice()];
+                            a = [O(i).slice(), O(f).slice()];
                             break
                     }
                 }
 
-                function _() {
+                function T() {
                     r = 0
                 }
 
-                function U() {
-                    s.value = 500 / R(o).getBoundingClientRect().width
+                function D() {
+                    s.value = 500 / O(o).getBoundingClientRect().width
                 }
-                const F = new ResizeObserver(U);
+                const P = new ResizeObserver(D);
                 F8(() => {
-                    console.log("svgContainer", R(o)), F.observe(R(o))
-                }), V8(() => F.disconnect()), A1(() => e.point1, L => {
-                    [l.value, p.value, y.value] = L, d()
-                }), A1(() => e.point2, L => {
-                    [h.value, C.value, N.value] = L, d()
-                }), A1(x, m), d();
+                    console.log("svgContainer", O(o)), P.observe(O(o))
+                }), V8(() => P.disconnect()), A1(() => e.point1, _ => {
+                    [l.value, p.value, y.value] = _, b()
+                }), A1(() => e.point2, _ => {
+                    [h.value, C.value, N.value] = _, b()
+                }), A1(() => e.nbSliders, v), b();
                 const {
-                    image: T
+                    image: F
                 } = U8(e);
                 return {
                     svgContainer: o,
-                    onMouseMove: O,
-                    onMousePress: D,
-                    onMouseRelease: _,
+                    onMouseMove: d,
+                    onMousePress: m,
+                    onMouseRelease: T,
                     normalDelta: c,
                     radius: u,
                     p1: i,
                     p2: f,
-                    nbSeeds: B,
-                    sharedDepth: x,
                     x1: l,
                     x2: h,
-                    step: S,
-                    pointColor2: b,
-                    pushLineSeed: m,
-                    image: T
+                    step: B,
+                    pointColor2: R,
+                    pushLineSeed: v,
+                    image: F
                 }
             },
             template: `<v-col class="mt-2">
   <svg viewBox="0 0 500 500"
     ref="svgContainer"
     width="100%"
     @mousemove="onMouseMove"
@@ -5834,53 +5834,31 @@
       stroke-width="8"
       fill="rgba(0,0,0,0)"
       @mousedown="onMousePress(1, $event)"
       style="cursor: pointer;"
     />
   </svg>
   <v-col class="pt-0">
-    <v-row class="align-center">
-      <v-col cols="12" md="11">
-      <v-text-field
-        density="compact"
-        hide-details
-        type="number"
-        min="5"
-        max="1000"
-        step="1"
-        label="Seeds count"
-        v-model="nbSeeds"
-      />
-      </v-col>
-      <v-col cols="12" md="1">
-      <v-switch
-        style="width: 80px" 
-        class="mt-0"
-        density="compact"
-        v-model="sharedDepth"
-        hide-details
-      />
-      </v-col>
-    </v-row>
     <v-row>
         <v-slider 
-            v-show="!sharedDepth" 
+            v-show="nbSliders > 1"
             v-model="x2" 
             track-color="green" 
             color="green" 
             density="compact" 
             hide-details 
             @update:modelValue="pushLineSeed" 
             :min="bounds[0]" 
             :max="bounds[1]" 
             :step="step" 
         />
     </v-row>
     <v-row>
         <v-slider 
+            v-show="nbSliders > 0"
             v-model="x1" 
             track-color="blue" 
             color="blue" 
             density="compact"  
             hide-details 
             @update:modelValue="pushLineSeed"
             :min="bounds[0]" 
@@ -5895,11 +5873,11 @@
     };
 
     function z8(e) {
         Object.keys(i9).forEach(t => {
             e.component(t, i9[t])
         })
     }
-    b0.install = z8, Object.defineProperty(b0, Symbol.toStringTag, {
+    w0.install = z8, Object.defineProperty(w0, Symbol.toStringTag, {
         value: "Module"
     })
 });
```

### Comparing `trame-components-2.3.1/trame_components/widgets/trame.py` & `trame-components-2.3.2/trame_components/widgets/trame.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,14 +488,15 @@
 
 class LineSeed(HtmlElement):
     def __init__(self, children=None, **kwargs):
         super().__init__("trame-line-seed", children, **kwargs)
         self._attr_names += [
             ("point_1", "point1"),
             ("point_2", "point2"),
-            ("number_steps", "numberOfSteps"),
+            ("n_steps", "numberOfSteps"),
+            ("n_sliders", "nbSliders"),
             "bounds",
             "image",
         ]
         self._event_names += [
             ("update_seed", "update-seed"),
         ]
```

### Comparing `trame-components-2.3.1/trame_components.egg-info/PKG-INFO` & `trame-components-2.3.2/trame_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.3.1
+Version: 2.3.2
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.3.1/trame_components.egg-info/SOURCES.txt` & `trame-components-2.3.2/trame_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*


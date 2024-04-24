# Comparing `tmp/gryannote_audio-0.1.4.tar.gz` & `tmp/gryannote_audio-0.1.5.tar.gz`

## Comparing `gryannote_audio-0.1.4.tar` & `gryannote_audio-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/__init__.py
--rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/annotatedaudio.py
--rw-r--r--   0        0        0    77967 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/annotatedaudio.pyi
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/core.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0   400465 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/index.js
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-2c3384e6.js
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-aafe8b06.js
--rw-r--r--   0        0        0   118992 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-d82531d9.js
--rw-r--r--   0        0        0    24021 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/example/index.js
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/backend/gryannote_audio/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/demo/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/demo/app.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/Example.svelte
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/Index.svelte
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/index.ts
--rw-r--r--   0        0        0    48788 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/package-lock.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/package.json
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/interactive/InteractiveAnnotatedAudio.svelte
--rw-r--r--   0        0        0    20179 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/player/AudioPlayerWithAnnotation.svelte
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/recorder/AudioRecorder.svelte
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/AnnotatedAudioData.ts
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/Audio.svelte
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/Caption.svelte
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/VolumeControl.svelte
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/VolumeLevels.svelte
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/WaveformControls.svelte
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/WaveformRecordControls.svelte
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/audioBufferToWav.ts
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/index.ts
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/types.ts
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/utils.ts
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/icons/Gum.svelte
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/icons/Magnifier.svelte
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/shared/icons/Plus.svelte
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/static/StaticAnnotatedAudio.svelte
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/frontend/streaming/StreamAudio.svelte
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/.gitignore
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/README.md
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 gryannote_audio-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/__init__.py
+-rw-r--r--   0        0        0    16841 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.py
+-rw-r--r--   0        0        0    77967 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.pyi
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/core.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0   400469 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/index.js
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-2c3384e6.js
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-aafe8b06.js
+-rw-r--r--   0        0        0   118992 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-d82531d9.js
+-rw-r--r--   0        0        0    24006 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/index.js
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/demo/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/demo/app.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/Example.svelte
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/Index.svelte
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/index.ts
+-rw-r--r--   0        0        0    48788 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/package-lock.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/package.json
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/interactive/InteractiveAnnotatedAudio.svelte
+-rw-r--r--   0        0        0    20347 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/player/AudioPlayerWithAnnotation.svelte
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/recorder/AudioRecorder.svelte
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/AnnotatedAudioData.ts
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/Audio.svelte
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/Caption.svelte
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/VolumeControl.svelte
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/VolumeLevels.svelte
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/WaveformControls.svelte
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/WaveformRecordControls.svelte
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/audioBufferToWav.ts
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/index.ts
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/types.ts
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Gum.svelte
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Magnifier.svelte
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/shared/icons/Plus.svelte
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/static/StaticAnnotatedAudio.svelte
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/frontend/streaming/StreamAudio.svelte
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/.gitignore
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/README.md
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 gryannote_audio-0.1.5/PKG-INFO
```

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/annotatedaudio.py` & `gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.py`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/annotatedaudio.pyi` & `gryannote_audio-0.1.5/backend/gryannote_audio/annotatedaudio.pyi`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/core.py` & `gryannote_audio-0.1.5/backend/gryannote_audio/core.py`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/index.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
     return t = t.split("."), e = e.split("."), Ho(t[0], e[0]) || Ho(t[1], e[1]) || (e[2] = e.slice(2).join("."), n = /[.-]/.test(t[2] = t.slice(2).join(".")), n == /[.-]/.test(e[2]) ? Ho(t[2], e[2]) : n ? -1 : 1);
 }
 
 function Pa(t, e, n) {
     return e.startsWith("http://") || e.startsWith("https://") ? n ? t : e : t + e;
 }
 
-function No(t) {
+function Oo(t) {
     if (t.startsWith("http")) {
         const {
             protocol: e,
             host: n
         } = new URL(t);
         return n.endsWith("hf.space") ? {
             ws_protocol: "wss",
@@ -52,35 +52,35 @@
                 }
             );
             if (o.status !== 200)
                 throw new Error("Space metadata could not be loaded.");
             const r = (await o.json()).host;
             return {
                 space_id: t,
-                ...No(r)
+                ...Oo(r)
             };
         } catch (o) {
             throw new Error("Space metadata could not be loaded." + o.message);
         }
     if (kc.test(i)) {
         const {
             ws_protocol: o,
             http_protocol: r,
             host: s
-        } = No(i);
+        } = Oo(i);
         return {
             space_id: s.replace(".hf.space", ""),
             ws_protocol: o,
             http_protocol: r,
             host: s
         };
     }
     return {
         space_id: !1,
-        ...No(i)
+        ...Oo(i)
     };
 }
 
 function Cc(t) {
     let e = {};
     return t.forEach(({
         api_name: n
@@ -143,36 +143,36 @@
         (r) => r.blob
     );
     return await Promise.all(
         await i(e, o, void 0, n).then(
             async (r) => {
                 if (r.error)
                     throw new Error(r.error);
-                return r.files ? r.files.map((s, a) => new mo({
+                return r.files ? r.files.map((s, a) => new _o({
                     ...t[a],
                     path: s,
                     url: e + "/file=" + s
                 })) : [];
             }
         )
     );
 }
 async function Ba(t, e) {
     return t.map(
-        (n, i) => new mo({
+        (n, i) => new _o({
             path: n.name,
             orig_name: n.name,
             blob: n,
             size: n.size,
             mime_type: n.type,
             is_stream: e
         })
     );
 }
-class mo {
+class _o {
     constructor({
         path: e,
         url: n,
         orig_name: i,
         size: o,
         blob: r,
         is_stream: s,
@@ -240,77 +240,77 @@
                     headers: c
                 });
             } catch {
                 return {
                     error: Vt
                 };
             }
-            const g = await d.json();
-            h.push(...g);
+            const b = await d.json();
+            h.push(...b);
         }
         return {
             files: h
         };
     }
     async function o(s, a = {}) {
         return new Promise(async (l) => {
             const {
                 status_callback: u,
                 hf_token: c
             } = a, f = {
                 predict: X,
-                submit: E,
-                view_api: $,
-                component_server: I
+                submit: C,
+                view_api: K,
+                component_server: U
             };
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
-                const H = await import("./wrapper-6f348d45-19fa94bf.js");
-                Da = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = H.WebSocket;
+                const O = await import("./wrapper-6f348d45-19fa94bf.js");
+                Da = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = O.WebSocket;
             }
             const {
                 ws_protocol: h,
                 http_protocol: d,
                 host: _,
                 space_id: m
-            } = await Ec(s, c), v = Math.random().toString(36).substring(2), g = {};
+            } = await Ec(s, c), v = Math.random().toString(36).substring(2), b = {};
             let S = !1,
                 w = {},
                 k = {},
-                C = null;
+                E = null;
             const y = {},
-                O = /* @__PURE__ */ new Set();
+                H = /* @__PURE__ */ new Set();
             let L, P = {},
                 M = !1;
             c && m && (M = await Bc(m, c));
-            async function x(H) {
-                if (L = H, window.location.protocol === "https:" && (L.root = L.root.replace("http://", "https://")), P = Cc((H == null ? void 0 : H.dependencies) || []), L.auth_required)
+            async function Z(O) {
+                if (L = O, window.location.protocol === "https:" && (L.root = L.root.replace("http://", "https://")), P = Cc((O == null ? void 0 : O.dependencies) || []), L.auth_required)
                     return {
                         config: L,
                         ...f
                     };
                 try {
-                    Z = await $(L);
+                    x = await K(L);
                 } catch (J) {
                     console.error(`Could not get api details: ${J.message}`);
                 }
                 return {
                     config: L,
                     ...f
                 };
             }
-            let Z;
-            async function G(H) {
-                if (u && u(H), H.status === "running")
+            let x;
+            async function j(O) {
+                if (u && u(O), O.status === "running")
                     try {
                         L = await Es(
                             t,
                             `${d}//${_}`,
                             c
                         );
-                        const J = await x(L);
+                        const J = await Z(L);
                         l(J);
                     } catch (J) {
                         console.error(J), u && u({
                             status: "error",
                             message: "Could not load this space.",
                             load_status: "error",
                             detail: "NOT_FOUND"
@@ -319,608 +319,608 @@
             }
             try {
                 L = await Es(
                     t,
                     `${d}//${_}`,
                     c
                 );
-                const H = await x(L);
-                l(H);
-            } catch (H) {
-                console.error(H), m ? Br(
+                const O = await Z(L);
+                l(O);
+            } catch (O) {
+                console.error(O), m ? Rr(
                     m,
                     La.test(m) ? "space_name" : "subdomain",
-                    G
+                    j
                 ) : u && u({
                     status: "error",
                     message: "Could not load this space.",
                     load_status: "error",
                     detail: "NOT_FOUND"
                 });
             }
 
-            function X(H, J, ee) {
+            function X(O, J, le) {
                 let p = !1,
-                    T = !1,
+                    A = !1,
                     q;
-                if (typeof H == "number")
-                    q = L.dependencies[H];
+                if (typeof O == "number")
+                    q = L.dependencies[O];
                 else {
-                    const z = H.replace(/^\//, "");
+                    const z = O.replace(/^\//, "");
                     q = L.dependencies[P[z]];
                 }
                 if (q.types.continuous)
                     throw new Error(
                         "Cannot call predict on this function as it may run forever. Use submit instead"
                     );
-                return new Promise((z, _e) => {
-                    const me = E(H, J, ee);
-                    let U;
-                    me.on("data", (Ce) => {
-                        T && (me.destroy(), z(Ce)), p = !0, U = Ce;
-                    }).on("status", (Ce) => {
-                        Ce.stage === "error" && _e(Ce), Ce.stage === "complete" && (T = !0, p && (me.destroy(), z(U)));
+                return new Promise((z, he) => {
+                    const _e = C(O, J, le);
+                    let F;
+                    _e.on("data", (ve) => {
+                        A && (_e.destroy(), z(ve)), p = !0, F = ve;
+                    }).on("status", (ve) => {
+                        ve.stage === "error" && he(ve), ve.stage === "complete" && (A = !0, p && (_e.destroy(), z(F)));
                     });
                 });
             }
 
-            function E(H, J, ee, p = null) {
-                let T, q;
-                if (typeof H == "number")
-                    T = H, q = Z.unnamed_endpoints[T];
+            function C(O, J, le, p = null) {
+                let A, q;
+                if (typeof O == "number")
+                    A = O, q = x.unnamed_endpoints[A];
                 else {
-                    const b = H.replace(/^\//, "");
-                    T = P[b], q = Z.named_endpoints[H.trim()];
+                    const g = O.replace(/^\//, "");
+                    A = P[g], q = x.named_endpoints[O.trim()];
                 }
-                if (typeof T != "number")
+                if (typeof A != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
-                let z, _e, me = L.protocol ?? "ws";
-                const U = typeof H == "number" ? "/predict" : H;
-                let Ce, B = null,
+                let z, he, _e = L.protocol ?? "ws";
+                const F = typeof O == "number" ? "/predict" : O;
+                let ve, B = null,
                     R = !1;
                 const ce = {};
                 let Se = "";
                 typeof window < "u" && (Se = new URLSearchParams(window.location.search).toString()), r(`${L.root}`, J, q, c).then(
-                    (b) => {
-                        if (Ce = {
-                                data: b || [],
-                                event_data: ee,
-                                fn_index: T,
+                    (g) => {
+                        if (ve = {
+                                data: g || [],
+                                event_data: le,
+                                fn_index: A,
                                 trigger_id: p
-                            }, Mc(T, L))
+                            }, Mc(A, L))
                             Y({
                                 type: "status",
-                                endpoint: U,
+                                endpoint: F,
                                 stage: "pending",
                                 queue: !1,
-                                fn_index: T,
+                                fn_index: A,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
-                                `${L.root}/run${U.startsWith("/") ? U : `/${U}`}${Se ? "?" + Se : ""}`, {
-                                    ...Ce,
+                                `${L.root}/run${F.startsWith("/") ? F : `/${F}`}${Se ? "?" + Se : ""}`, {
+                                    ...ve,
                                     session_hash: v
                                 },
                                 c
-                            ).then(([D, j]) => {
-                                const ne = D.data;
-                                j == 200 ? (Y({
+                            ).then(([D, N]) => {
+                                const te = D.data;
+                                N == 200 ? (Y({
                                     type: "data",
-                                    endpoint: U,
-                                    fn_index: T,
-                                    data: ne,
+                                    endpoint: F,
+                                    fn_index: A,
+                                    data: te,
                                     time: /* @__PURE__ */ new Date()
                                 }), Y({
                                     type: "status",
-                                    endpoint: U,
-                                    fn_index: T,
+                                    endpoint: F,
+                                    fn_index: A,
                                     stage: "complete",
                                     eta: D.average_duration,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 })) : Y({
                                     type: "status",
                                     stage: "error",
-                                    endpoint: U,
-                                    fn_index: T,
+                                    endpoint: F,
+                                    fn_index: A,
                                     message: D.error,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             }).catch((D) => {
                                 Y({
                                     type: "status",
                                     stage: "error",
                                     message: D.message,
-                                    endpoint: U,
-                                    fn_index: T,
+                                    endpoint: F,
+                                    fn_index: A,
                                     queue: !1,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             });
-                        else if (me == "ws") {
+                        else if (_e == "ws") {
                             Y({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: U,
-                                fn_index: T,
+                                endpoint: F,
+                                fn_index: A,
                                 time: /* @__PURE__ */ new Date()
                             });
                             let D = new URL(`${h}://${Pa(
                 _,
                 L.path,
                 !0
               )}
 							/queue/join${Se ? "?" + Se : ""}`);
-                            M && D.searchParams.set("__sign", M), z = new WebSocket(D), z.onclose = (j) => {
-                                j.wasClean || Y({
+                            M && D.searchParams.set("__sign", M), z = new WebSocket(D), z.onclose = (N) => {
+                                N.wasClean || Y({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
                                     message: Vt,
                                     queue: !0,
-                                    endpoint: U,
-                                    fn_index: T,
+                                    endpoint: F,
+                                    fn_index: A,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }, z.onmessage = function(j) {
-                                const ne = JSON.parse(j.data),
+                            }, z.onmessage = function(N) {
+                                const te = JSON.parse(N.data),
                                     {
-                                        type: re,
-                                        status: se,
+                                        type: oe,
+                                        status: re,
                                         data: ae
-                                    } = Io(
-                                        ne,
-                                        g[T]
+                                    } = No(
+                                        te,
+                                        b[A]
                                     );
-                                if (re === "update" && se && !R)
+                                if (oe === "update" && re && !R)
                                     Y({
                                         type: "status",
-                                        endpoint: U,
-                                        fn_index: T,
+                                        endpoint: F,
+                                        fn_index: A,
                                         time: /* @__PURE__ */ new Date(),
-                                        ...se
-                                    }), se.stage === "error" && z.close();
-                                else if (re === "hash") {
+                                        ...re
+                                    }), re.stage === "error" && z.close();
+                                else if (oe === "hash") {
                                     z.send(JSON.stringify({
-                                        fn_index: T,
+                                        fn_index: A,
                                         session_hash: v
                                     }));
                                     return;
                                 } else
-                                    re === "data" ? z.send(JSON.stringify({
-                                        ...Ce,
+                                    oe === "data" ? z.send(JSON.stringify({
+                                        ...ve,
                                         session_hash: v
-                                    })) : re === "complete" ? R = se : re === "log" ? Y({
+                                    })) : oe === "complete" ? R = re : oe === "log" ? Y({
                                         type: "log",
                                         log: ae.log,
                                         level: ae.level,
-                                        endpoint: U,
-                                        fn_index: T
-                                    }) : re === "generating" && Y({
+                                        endpoint: F,
+                                        fn_index: A
+                                    }) : oe === "generating" && Y({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
-                                        ...se,
-                                        stage: se == null ? void 0 : se.stage,
+                                        ...re,
+                                        stage: re == null ? void 0 : re.stage,
                                         queue: !0,
-                                        endpoint: U,
-                                        fn_index: T
+                                        endpoint: F,
+                                        fn_index: A
                                     });
                                 ae && (Y({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
                                     data: ae.data,
-                                    endpoint: U,
-                                    fn_index: T
+                                    endpoint: F,
+                                    fn_index: A
                                 }), R && (Y({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
                                     ...R,
-                                    stage: se == null ? void 0 : se.stage,
+                                    stage: re == null ? void 0 : re.stage,
                                     queue: !0,
-                                    endpoint: U,
-                                    fn_index: T
+                                    endpoint: F,
+                                    fn_index: A
                                 }), z.close()));
                             }, bs(L.version || "2.0.0", "3.6") < 0 && addEventListener(
                                 "open",
                                 () => z.send(JSON.stringify({
                                     hash: v
                                 }))
                             );
-                        } else if (me == "sse") {
+                        } else if (_e == "sse") {
                             Y({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: U,
-                                fn_index: T,
+                                endpoint: F,
+                                fn_index: A,
                                 time: /* @__PURE__ */ new Date()
                             });
-                            var A = new URLSearchParams({
-                                fn_index: T.toString(),
+                            var T = new URLSearchParams({
+                                fn_index: A.toString(),
                                 session_hash: v
                             }).toString();
                             let D = new URL(
-                                `${L.root}/queue/join?${Se ? Se + "&" : ""}${A}`
+                                `${L.root}/queue/join?${Se ? Se + "&" : ""}${T}`
                             );
-                            _e = e(D), _e.onmessage = async function(j) {
-                                const ne = JSON.parse(j.data),
+                            he = e(D), he.onmessage = async function(N) {
+                                const te = JSON.parse(N.data),
                                     {
-                                        type: re,
-                                        status: se,
+                                        type: oe,
+                                        status: re,
                                         data: ae
-                                    } = Io(
-                                        ne,
-                                        g[T]
+                                    } = No(
+                                        te,
+                                        b[A]
                                     );
-                                if (re === "update" && se && !R)
+                                if (oe === "update" && re && !R)
                                     Y({
                                         type: "status",
-                                        endpoint: U,
-                                        fn_index: T,
+                                        endpoint: F,
+                                        fn_index: A,
                                         time: /* @__PURE__ */ new Date(),
-                                        ...se
-                                    }), se.stage === "error" && _e.close();
-                                else if (re === "data") {
-                                    B = ne.event_id;
+                                        ...re
+                                    }), re.stage === "error" && he.close();
+                                else if (oe === "data") {
+                                    B = te.event_id;
                                     let [Wt, yc] = await n(
                                         `${L.root}/queue/data`, {
-                                            ...Ce,
+                                            ...ve,
                                             session_hash: v,
                                             event_id: B
                                         },
                                         c
                                     );
                                     yc !== 200 && (Y({
                                         type: "status",
                                         stage: "error",
                                         message: Vt,
                                         queue: !0,
-                                        endpoint: U,
-                                        fn_index: T,
+                                        endpoint: F,
+                                        fn_index: A,
                                         time: /* @__PURE__ */ new Date()
-                                    }), _e.close());
+                                    }), he.close());
                                 } else
-                                    re === "complete" ? R = se : re === "log" ? Y({
+                                    oe === "complete" ? R = re : oe === "log" ? Y({
                                         type: "log",
                                         log: ae.log,
                                         level: ae.level,
-                                        endpoint: U,
-                                        fn_index: T
-                                    }) : re === "generating" && Y({
+                                        endpoint: F,
+                                        fn_index: A
+                                    }) : oe === "generating" && Y({
                                         type: "status",
                                         time: /* @__PURE__ */ new Date(),
-                                        ...se,
-                                        stage: se == null ? void 0 : se.stage,
+                                        ...re,
+                                        stage: re == null ? void 0 : re.stage,
                                         queue: !0,
-                                        endpoint: U,
-                                        fn_index: T
+                                        endpoint: F,
+                                        fn_index: A
                                     });
                                 ae && (Y({
                                     type: "data",
                                     time: /* @__PURE__ */ new Date(),
                                     data: ae.data,
-                                    endpoint: U,
-                                    fn_index: T
+                                    endpoint: F,
+                                    fn_index: A
                                 }), R && (Y({
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
                                     ...R,
-                                    stage: se == null ? void 0 : se.stage,
+                                    stage: re == null ? void 0 : re.stage,
                                     queue: !0,
-                                    endpoint: U,
-                                    fn_index: T
-                                }), _e.close()));
+                                    endpoint: F,
+                                    fn_index: A
+                                }), he.close()));
                             };
                         } else
-                            (me == "sse_v1" || me == "sse_v2" || me == "sse_v2.1" || me == "sse_v3") && (Y({
+                            (_e == "sse_v1" || _e == "sse_v2" || _e == "sse_v2.1" || _e == "sse_v3") && (Y({
                                 type: "status",
                                 stage: "pending",
                                 queue: !0,
-                                endpoint: U,
-                                fn_index: T,
+                                endpoint: F,
+                                fn_index: A,
                                 time: /* @__PURE__ */ new Date()
                             }), n(
                                 `${L.root}/queue/join?${Se}`, {
-                                    ...Ce,
+                                    ...ve,
                                     session_hash: v
                                 },
                                 c
-                            ).then(([D, j]) => {
-                                if (j === 503)
+                            ).then(([D, N]) => {
+                                if (N === 503)
                                     Y({
                                         type: "status",
                                         stage: "error",
                                         message: Ma,
                                         queue: !0,
-                                        endpoint: U,
-                                        fn_index: T,
+                                        endpoint: F,
+                                        fn_index: A,
                                         time: /* @__PURE__ */ new Date()
                                     });
-                                else if (j !== 200)
+                                else if (N !== 200)
                                     Y({
                                         type: "status",
                                         stage: "error",
                                         message: Vt,
                                         queue: !0,
-                                        endpoint: U,
-                                        fn_index: T,
+                                        endpoint: F,
+                                        fn_index: A,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else {
                                     B = D.event_id;
-                                    let ne = async function(re) {
+                                    let te = async function(oe) {
                                         try {
                                             const {
-                                                type: se,
+                                                type: re,
                                                 status: ae,
                                                 data: Wt
-                                            } = Io(
-                                                re,
-                                                g[T]
+                                            } = No(
+                                                oe,
+                                                b[A]
                                             );
-                                            if (se == "heartbeat")
+                                            if (re == "heartbeat")
                                                 return;
-                                            if (se === "update" && ae && !R)
+                                            if (re === "update" && ae && !R)
                                                 Y({
                                                     type: "status",
-                                                    endpoint: U,
-                                                    fn_index: T,
+                                                    endpoint: F,
+                                                    fn_index: A,
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...ae
                                                 });
-                                            else if (se === "complete")
+                                            else if (re === "complete")
                                                 R = ae;
-                                            else if (se == "unexpected_error")
+                                            else if (re == "unexpected_error")
                                                 console.error("Unexpected error", ae == null ? void 0 : ae.message), Y({
                                                     type: "status",
                                                     stage: "error",
                                                     message: (ae == null ? void 0 : ae.message) || "An Unexpected Error Occurred!",
                                                     queue: !0,
-                                                    endpoint: U,
-                                                    fn_index: T,
+                                                    endpoint: F,
+                                                    fn_index: A,
                                                     time: /* @__PURE__ */ new Date()
                                                 });
-                                            else if (se === "log") {
+                                            else if (re === "log") {
                                                 Y({
                                                     type: "log",
                                                     log: Wt.log,
                                                     level: Wt.level,
-                                                    endpoint: U,
-                                                    fn_index: T
+                                                    endpoint: F,
+                                                    fn_index: A
                                                 });
                                                 return;
                                             } else
-                                                se === "generating" && (Y({
+                                                re === "generating" && (Y({
                                                     type: "status",
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...ae,
                                                     stage: ae == null ? void 0 : ae.stage,
                                                     queue: !0,
-                                                    endpoint: U,
-                                                    fn_index: T
-                                                }), Wt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(me) && wt(B, Wt));
+                                                    endpoint: F,
+                                                    fn_index: A
+                                                }), Wt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(_e) && wt(B, Wt));
                                             Wt && (Y({
                                                 type: "data",
                                                 time: /* @__PURE__ */ new Date(),
                                                 data: Wt.data,
-                                                endpoint: U,
-                                                fn_index: T
+                                                endpoint: F,
+                                                fn_index: A
                                             }), R && Y({
                                                 type: "status",
                                                 time: /* @__PURE__ */ new Date(),
                                                 ...R,
                                                 stage: ae == null ? void 0 : ae.stage,
                                                 queue: !0,
-                                                endpoint: U,
-                                                fn_index: T
+                                                endpoint: F,
+                                                fn_index: A
                                             })), ((ae == null ? void 0 : ae.stage) === "complete" || (ae == null ? void 0 : ae.stage) === "error") && (y[B] && delete y[B], B in k && delete k[B]);
-                                        } catch (se) {
-                                            console.error("Unexpected client exception", se), Y({
+                                        } catch (re) {
+                                            console.error("Unexpected client exception", re), Y({
                                                 type: "status",
                                                 stage: "error",
                                                 message: "An Unexpected Error Occurred!",
                                                 queue: !0,
-                                                endpoint: U,
-                                                fn_index: T,
+                                                endpoint: F,
+                                                fn_index: A,
                                                 time: /* @__PURE__ */ new Date()
-                                            }), ["sse_v2", "sse_v2.1"].includes(me) && N();
+                                            }), ["sse_v2", "sse_v2.1"].includes(_e) && I();
                                         }
                                     };
                                     B in w && (w[B].forEach(
-                                        (re) => ne(re)
-                                    ), delete w[B]), y[B] = ne, O.add(B), S || F();
+                                        (oe) => te(oe)
+                                    ), delete w[B]), y[B] = te, H.add(B), S || G();
                                 }
                             }));
                     }
                 );
 
-                function wt(b, A) {
-                    !k[b] ? (k[b] = [], A.data.forEach((j, ne) => {
-                        k[b][ne] = j;
-                    })) : A.data.forEach((j, ne) => {
-                        let re = Tc(
-                            k[b][ne],
-                            j
+                function wt(g, T) {
+                    !k[g] ? (k[g] = [], T.data.forEach((N, te) => {
+                        k[g][te] = N;
+                    })) : T.data.forEach((N, te) => {
+                        let oe = Tc(
+                            k[g][te],
+                            N
                         );
-                        k[b][ne] = re, A.data[ne] = re;
+                        k[g][te] = oe, T.data[te] = oe;
                     });
                 }
 
-                function Y(b) {
-                    const D = ce[b.type] || [];
-                    D == null || D.forEach((j) => j(b));
+                function Y(g) {
+                    const D = ce[g.type] || [];
+                    D == null || D.forEach((N) => N(g));
                 }
 
-                function yt(b, A) {
+                function yt(g, T) {
                     const D = ce,
-                        j = D[b] || [];
-                    return D[b] = j, j == null || j.push(A), {
+                        N = D[g] || [];
+                    return D[g] = N, N == null || N.push(T), {
                         on: yt,
                         off: wn,
                         cancel: ei,
                         destroy: ti
                     };
                 }
 
-                function wn(b, A) {
+                function wn(g, T) {
                     const D = ce;
-                    let j = D[b] || [];
-                    return j = j == null ? void 0 : j.filter((ne) => ne !== A), D[b] = j, {
+                    let N = D[g] || [];
+                    return N = N == null ? void 0 : N.filter((te) => te !== T), D[g] = N, {
                         on: yt,
                         off: wn,
                         cancel: ei,
                         destroy: ti
                     };
                 }
                 async function ei() {
-                    const b = {
+                    const g = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
                     };
-                    R = b, Y({
-                        ...b,
+                    R = g, Y({
+                        ...g,
                         type: "status",
-                        endpoint: U,
-                        fn_index: T
+                        endpoint: F,
+                        fn_index: A
                     });
-                    let A = {};
-                    me === "ws" ? (z && z.readyState === 0 ? z.addEventListener("open", () => {
+                    let T = {};
+                    _e === "ws" ? (z && z.readyState === 0 ? z.addEventListener("open", () => {
                         z.close();
-                    }) : z.close(), A = {
-                        fn_index: T,
+                    }) : z.close(), T = {
+                        fn_index: A,
                         session_hash: v
-                    }) : (_e.close(), A = {
+                    }) : (he.close(), T = {
                         event_id: B
                     });
                     try {
                         await t(`${L.root}/reset`, {
                             headers: {
                                 "Content-Type": "application/json"
                             },
                             method: "POST",
-                            body: JSON.stringify(A)
+                            body: JSON.stringify(T)
                         });
                     } catch {
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
                 function ti() {
-                    for (const b in ce)
-                        ce[b].forEach((A) => {
-                            wn(b, A);
+                    for (const g in ce)
+                        ce[g].forEach((T) => {
+                            wn(g, T);
                         });
                 }
                 return {
                     on: yt,
                     off: wn,
                     cancel: ei,
                     destroy: ti
                 };
             }
 
-            function F() {
+            function G() {
                 S = !0;
-                let H = new URLSearchParams({
+                let O = new URLSearchParams({
                         session_hash: v
                     }).toString(),
-                    J = new URL(`${L.root}/queue/data?${H}`);
-                C = e(J), C.onmessage = async function(ee) {
-                    let p = JSON.parse(ee.data);
-                    const T = p.event_id;
-                    if (!T)
+                    J = new URL(`${L.root}/queue/data?${O}`);
+                E = e(J), E.onmessage = async function(le) {
+                    let p = JSON.parse(le.data);
+                    const A = p.event_id;
+                    if (!A)
                         await Promise.all(
                             Object.keys(y).map(
                                 (q) => y[q](p)
                             )
                         );
-                    else if (y[T]) {
-                        p.msg === "process_completed" && ["sse", "sse_v1", "sse_v2", "sse_v2.1"].includes(L.protocol) && (O.delete(T), O.size === 0 && N());
-                        let q = y[T];
+                    else if (y[A]) {
+                        p.msg === "process_completed" && ["sse", "sse_v1", "sse_v2", "sse_v2.1"].includes(L.protocol) && (H.delete(A), H.size === 0 && I());
+                        let q = y[A];
                         window.setTimeout(q, 0, p);
                     } else
-                        w[T] || (w[T] = []), w[T].push(p);
-                    p.msg === "close_stream" && N();
-                }, C.onerror = async function(ee) {
+                        w[A] || (w[A] = []), w[A].push(p);
+                    p.msg === "close_stream" && I();
+                }, E.onerror = async function(le) {
                     await Promise.all(
                         Object.keys(y).map(
                             (p) => y[p]({
                                 msg: "unexpected_error",
                                 message: Vt
                             })
                         )
-                    ), N();
+                    ), I();
                 };
             }
 
-            function N() {
-                S = !1, C == null || C.close();
+            function I() {
+                S = !1, E == null || E.close();
             }
-            async function I(H, J, ee) {
+            async function U(O, J, le) {
                 var p;
-                const T = {
+                const A = {
                     "Content-Type": "application/json"
                 };
-                c && (T.Authorization = `Bearer ${c}`);
+                c && (A.Authorization = `Bearer ${c}`);
                 let q, z = L.components.find(
-                    (U) => U.id === H
+                    (F) => F.id === O
                 );
                 (p = z == null ? void 0 : z.props) != null && p.root_url ? q = z.props.root_url : q = L.root;
-                const _e = await t(
+                const he = await t(
                     `${q}/component_server/`, {
                         method: "POST",
                         body: JSON.stringify({
-                            data: ee,
-                            component_id: H,
+                            data: le,
+                            component_id: O,
                             fn_name: J,
                             session_hash: v
                         }),
-                        headers: T
+                        headers: A
                     }
                 );
-                if (!_e.ok)
+                if (!he.ok)
                     throw new Error(
-                        "Could not connect to component server: " + _e.statusText
+                        "Could not connect to component server: " + he.statusText
                     );
-                return await _e.json();
+                return await he.json();
             }
-            async function $(H) {
-                if (Z)
-                    return Z;
+            async function K(O) {
+                if (x)
+                    return x;
                 const J = {
                     "Content-Type": "application/json"
                 };
                 c && (J.Authorization = `Bearer ${c}`);
-                let ee;
-                if (bs(H.version || "2.0.0", "3.30") < 0 ? ee = await t(
+                let le;
+                if (bs(O.version || "2.0.0", "3.30") < 0 ? le = await t(
                         "https://gradio-space-api-fetcher-v2.hf.space/api", {
                             method: "POST",
                             body: JSON.stringify({
                                 serialize: !1,
-                                config: JSON.stringify(H)
+                                config: JSON.stringify(O)
                             }),
                             headers: J
                         }
-                    ) : ee = await t(`${H.root}/info`, {
+                    ) : le = await t(`${O.root}/info`, {
                         headers: J
-                    }), !ee.ok)
+                    }), !le.ok)
                     throw new Error(Vt);
-                let p = await ee.json();
-                return "api" in p && (p = p.api), p.named_endpoints["/predict"] && !p.unnamed_endpoints[0] && (p.unnamed_endpoints[0] = p.named_endpoints["/predict"]), Rc(p, H, P);
+                let p = await le.json();
+                return "api" in p && (p = p.api), p.named_endpoints["/predict"] && !p.unnamed_endpoints[0] && (p.unnamed_endpoints[0] = p.named_endpoints["/predict"]), Rc(p, O, P);
             }
         });
     }
     async function r(s, a, l, u) {
-        const c = await Rr(
+        const c = await Lr(
             a,
             void 0,
             [],
             !0,
             l
         );
         return Promise.all(
@@ -948,28 +948,28 @@
             file_url: d,
             type: _,
             name: m
         }) => {
             if (_ === "Gallery")
                 ks(a, d, h);
             else if (d) {
-                const v = new mo({
+                const v = new _o({
                     path: d,
                     orig_name: m
                 });
                 ks(a, v, h);
             }
         }), a));
     }
 }
 const {
-    post_data: z2,
+    post_data: zv,
     upload_files: Lc,
-    client: G2,
-    handle_blob: W2
+    client: Gv,
+    handle_blob: Wv
 } = Pc(
     fetch,
     (...t) => new EventSource(...t)
 );
 
 function ws(t, e, n, i) {
     switch (t.type) {
@@ -1048,23 +1048,23 @@
 }
 
 function ks(t, e, n) {
     for (; n.length > 1;)
         t = t[n.shift()];
     t[n.shift()] = e;
 }
-async function Rr(t, e = void 0, n = [], i = !1, o = void 0) {
+async function Lr(t, e = void 0, n = [], i = !1, o = void 0) {
     if (Array.isArray(t)) {
         let r = [];
         return await Promise.all(
             t.map(async (s, a) => {
                 var l;
                 let u = n.slice();
                 u.push(a);
-                const c = await Rr(
+                const c = await Lr(
                     t[a],
                     i ? ((l = o == null ? void 0 : o.parameters[a]) == null ? void 0 : l.component) || void 0 : e,
                     u,
                     !1,
                     o
                 );
                 r = r.concat(c);
@@ -1079,15 +1079,15 @@
             }];
         if (typeof t == "object") {
             let r = [];
             for (let s in t)
                 if (t.hasOwnProperty(s)) {
                     let a = n.slice();
                     a.push(s), r = r.concat(
-                        await Rr(
+                        await Lr(
                             t[s],
                             void 0,
                             a,
                             !1,
                             o
                         )
                     );
@@ -1119,15 +1119,15 @@
             const r = await o.json();
             return r.path = r.path ?? "", r.root = e, r;
         }
         throw new Error("Could not get config.");
     }
     throw new Error("No config or app endpoint found");
 }
-async function Br(t, e, n) {
+async function Rr(t, e, n) {
     let i = e === "subdomain" ? `https://huggingface.co/api/spaces/by-subdomain/${t}` : `https://huggingface.co/api/spaces/${t}`,
         o, r;
     try {
         if (o = await fetch(i), r = o.status, r !== 200)
             throw new Error();
         o = await o.json();
     } catch {
@@ -1152,15 +1152,15 @@
         case "SLEEPING":
             n({
                 status: "sleeping",
                 load_status: "pending",
                 message: "Space is asleep. Waking it up...",
                 detail: s
             }), setTimeout(() => {
-                Br(t, e, n);
+                Rr(t, e, n);
             }, 1e3);
             break;
         case "PAUSED":
             n({
                 status: "paused",
                 load_status: "error",
                 message: "This space has been paused by the author. If you would like to try this demo, consider duplicating the space.",
@@ -1180,30 +1180,30 @@
         case "BUILDING":
             n({
                 status: "building",
                 load_status: "pending",
                 message: "Space is building...",
                 detail: s
             }), setTimeout(() => {
-                Br(t, e, n);
+                Rr(t, e, n);
             }, 1e3);
             break;
         default:
             n({
                 status: "space_error",
                 load_status: "error",
                 message: "This space is experiencing an issue.",
                 detail: s,
                 discussions_enabled: await vs(a)
             });
             break;
     }
 }
 
-function Io(t, e) {
+function No(t, e) {
     switch (t.msg) {
         case "send_data":
             return {
                 type: "data"
             };
         case "send_hash":
             return {
@@ -1325,15 +1325,15 @@
         orig_name: i,
         size: o,
         blob: r,
         is_stream: s,
         mime_type: a,
         alt_text: l
     }) {
-        this.file_data = new mo({
+        this.file_data = new _o({
             path: e,
             url: n,
             orig_name: i,
             size: o,
             blob: r,
             is_stream: s,
             mime_type: a,
@@ -1685,34 +1685,34 @@
         [e]: {
             primary: Ss[e][n],
             secondary: Ss[e][i]
         }
     }), {}
 );
 
-function Oc(t) {
+function Hc(t) {
     let e, n = t[0],
         i = 1;
     for (; i < t.length;) {
         const o = t[i],
             r = t[i + 1];
         if (i += 2, (o === "optionalAccess" || o === "optionalCall") && n == null)
             return;
         o === "access" || o === "optionalAccess" ? (e = n, n = r(n)) : (o === "call" || o === "optionalCall") && (n = r((...s) => n.call(e, ...s)), e = void 0);
     }
     return n;
 }
-class Uo extends Error {
+class Io extends Error {
     constructor(e) {
         super(e), this.name = "ShareError";
     }
 }
-async function Hc(t, e) {
+async function Oc(t, e) {
     if (window.__gradio_space__ == null)
-        throw new Uo("Must be on Spaces to share.");
+        throw new Io("Must be on Spaces to share.");
     let n, i, o;
     if (e === "url") {
         const l = await fetch(t);
         n = await l.blob(), i = l.headers.get("content-type") || "", o = l.headers.get("content-disposition") || "";
     } else
         n = Nc(t), i = t.split(";")[0].split(":")[1], o = "file" + i.split("/")[1];
     const r = new File([n], o, {
@@ -1723,19 +1723,19 @@
             body: r,
             headers: {
                 "Content-Type": r.type,
                 "X-Requested-With": "XMLHttpRequest"
             }
         });
     if (!s.ok) {
-        if (Oc([s, "access", (l) => l.headers, "access", (l) => l.get, "call", (l) => l("content-type"), "optionalAccess", (l) => l.includes, "call", (l) => l("application/json")])) {
+        if (Hc([s, "access", (l) => l.headers, "access", (l) => l.get, "call", (l) => l("content-type"), "optionalAccess", (l) => l.includes, "call", (l) => l("application/json")])) {
             const l = await s.json();
-            throw new Uo(`Upload failed: ${l.error}`);
+            throw new Io(`Upload failed: ${l.error}`);
         }
-        throw new Uo("Upload failed.");
+        throw new Io("Upload failed.");
     }
     return await s.text();
 }
 
 function Nc(t) {
     for (var e = t.split(","), n = e[0].match(/:(.*?);/)[1], i = atob(e[1]), o = i.length, r = new Uint8Array(o); o--;)
         r[o] = i.charCodeAt(o);
@@ -1762,16 +1762,16 @@
     get_spread_update: Wc,
     init: Vc,
     insert: Xc,
     safe_not_equal: xc,
     set_dynamic_element_data: As,
     set_style: qe,
     toggle_class: dt,
-    transition_in: Oa,
-    transition_out: Ha,
+    transition_in: Ha,
+    transition_out: Oa,
     update_slot_base: Zc
 } = window.__gradio__svelte__internal;
 
 function Jc(t) {
     let e, n, i;
     const o = (
             /*#slots*/
@@ -1967,18 +1967,18 @@
                     /*scale*/
                     l[12]
                 ), u & /*min_width*/
                 8192 && qe(e, "min-width", `calc(min(${/*min_width*/
       l[13]}px, 100%))`);
         },
         i(l) {
-            i || (Oa(r, l), i = !0);
+            i || (Ha(r, l), i = !0);
         },
         o(l) {
-            Ha(r, l), i = !1;
+            Oa(r, l), i = !1;
         },
         d(l) {
             l && Fc(e), r && r.d(l);
         }
     };
 }
 
@@ -1995,18 +1995,18 @@
             n && n.m(i, o), e = !0;
         },
         p(i, [o]) {
             /*tag*/
             i[14] && n.p(i, o);
         },
         i(i) {
-            e || (Oa(n, i), e = !0);
+            e || (Ha(n, i), e = !0);
         },
         o(i) {
-            Ha(n, i), e = !1;
+            Oa(n, i), e = !1;
         },
         d(i) {
             n && n.d(i);
         }
     };
 }
 
@@ -2035,47 +2035,47 @@
     } = e, {
         explicit_call: _ = !1
     } = e, {
         container: m = !0
     } = e, {
         visible: v = !0
     } = e, {
-        allow_overflow: g = !0
+        allow_overflow: b = !0
     } = e, {
         scale: S = null
     } = e, {
         min_width: w = 0
     } = e, k = h === "fieldset" ? "fieldset" : "div";
-    const C = (y) => {
+    const E = (y) => {
         if (y !== void 0) {
             if (typeof y == "number")
                 return y + "px";
             if (typeof y == "string")
                 return y;
         }
     };
     return t.$$set = (y) => {
-        "height" in y && n(0, r = y.height), "width" in y && n(1, s = y.width), "elem_id" in y && n(2, a = y.elem_id), "elem_classes" in y && n(3, l = y.elem_classes), "variant" in y && n(4, u = y.variant), "border_mode" in y && n(5, c = y.border_mode), "padding" in y && n(6, f = y.padding), "type" in y && n(16, h = y.type), "test_id" in y && n(7, d = y.test_id), "explicit_call" in y && n(8, _ = y.explicit_call), "container" in y && n(9, m = y.container), "visible" in y && n(10, v = y.visible), "allow_overflow" in y && n(11, g = y.allow_overflow), "scale" in y && n(12, S = y.scale), "min_width" in y && n(13, w = y.min_width), "$$scope" in y && n(17, o = y.$$scope);
+        "height" in y && n(0, r = y.height), "width" in y && n(1, s = y.width), "elem_id" in y && n(2, a = y.elem_id), "elem_classes" in y && n(3, l = y.elem_classes), "variant" in y && n(4, u = y.variant), "border_mode" in y && n(5, c = y.border_mode), "padding" in y && n(6, f = y.padding), "type" in y && n(16, h = y.type), "test_id" in y && n(7, d = y.test_id), "explicit_call" in y && n(8, _ = y.explicit_call), "container" in y && n(9, m = y.container), "visible" in y && n(10, v = y.visible), "allow_overflow" in y && n(11, b = y.allow_overflow), "scale" in y && n(12, S = y.scale), "min_width" in y && n(13, w = y.min_width), "$$scope" in y && n(17, o = y.$$scope);
     }, [
         r,
         s,
         a,
         l,
         u,
         c,
         f,
         d,
         _,
         m,
         v,
-        g,
+        b,
         S,
         w,
         k,
-        C,
+        E,
         h,
         o,
         i
     ];
 }
 class Na extends Ic {
     constructor(e) {
@@ -2096,15 +2096,15 @@
             scale: 12,
             min_width: 13
         });
     }
 }
 const {
     SvelteComponent: Kc,
-    append: jo,
+    append: Uo,
     attr: Ii,
     create_component: $c,
     destroy_component: ef,
     detach: tf,
     element: Ts,
     init: nf,
     insert: of,
@@ -2137,15 +2137,15 @@
                 e,
                 "hide-label",
                 /*disable*/
                 t[3]
             );
         },
         m(a, l) {
-            of(a, e, l), jo(e, n), rf(i, n, null), jo(e, o), jo(e, r), s = !0;
+            of(a, e, l), Uo(e, n), rf(i, n, null), Uo(e, o), Uo(e, r), s = !0;
         },
         p(a, [l]) {
             (!s || l & /*label*/
                 1) && lf(
                 r,
                 /*label*/
                 a[0]
@@ -2204,21 +2204,21 @@
             disable: 3,
             float: 4
         });
     }
 }
 const {
     SvelteComponent: _f,
-    append: Mr,
+    append: Br,
     attr: Et,
     bubble: mf,
     create_component: pf,
     destroy_component: gf,
     detach: Ua,
-    element: Dr,
+    element: Mr,
     init: bf,
     insert: ja,
     listen: vf,
     mount_component: wf,
     safe_not_equal: yf,
     set_data: kf,
     set_style: Ui,
@@ -2229,21 +2229,21 @@
     transition_out: Af
 } = window.__gradio__svelte__internal;
 
 function Ps(t) {
     let e, n;
     return {
         c() {
-            e = Dr("span"), n = Cf(
+            e = Mr("span"), n = Cf(
                 /*label*/
                 t[1]
             ), Et(e, "class", "svelte-lpi64a");
         },
         m(i, o) {
-            ja(i, e, o), Mr(e, n);
+            ja(i, e, o), Br(e, n);
         },
         p(i, o) {
             o & /*label*/
                 2 && kf(
                     n,
                     /*label*/
                     i[1]
@@ -2259,15 +2259,15 @@
     let e, n, i, o, r, s, a, l = (
         /*show_label*/
         t[2] && Ps(t)
     );
     return o = new /*Icon*/
     t[0]({}), {
         c() {
-            e = Dr("button"), l && l.c(), n = Ef(), i = Dr("div"), pf(o.$$.fragment), Et(i, "class", "svelte-lpi64a"), Ge(
+            e = Mr("button"), l && l.c(), n = Ef(), i = Mr("div"), pf(o.$$.fragment), Et(i, "class", "svelte-lpi64a"), Ge(
                     i,
                     "small",
                     /*size*/
                     t[4] === "small"
                 ), Ge(
                     i,
                     "large",
@@ -2317,15 +2317,15 @@
                     ) : "var(--block-label-text-color)"), Ui(e, "--bg-color", /*disabled*/
                     t[7] ? "auto" : (
                         /*background*/
                         t[10]
                     ));
         },
         m(u, c) {
-            ja(u, e, c), l && l.m(e, null), Mr(e, n), Mr(e, i), wf(o, i, null), r = !0, s || (a = vf(
+            ja(u, e, c), l && l.m(e, null), Br(e, n), Br(e, i), wf(o, i, null), r = !0, s || (a = vf(
                 e,
                 "click",
                 /*click_handler*/
                 t[13]
             ), s = !0);
         },
         p(u, [c]) {
@@ -2445,19 +2445,19 @@
         {
             transparent: _ = !1
         } = e,
         {
             background: m = "var(--background-fill-primary)"
         } = e;
 
-    function v(g) {
-        mf.call(this, t, g);
+    function v(b) {
+        mf.call(this, t, b);
     }
-    return t.$$set = (g) => {
-        "Icon" in g && n(0, o = g.Icon), "label" in g && n(1, r = g.label), "show_label" in g && n(2, s = g.show_label), "pending" in g && n(3, a = g.pending), "size" in g && n(4, l = g.size), "padded" in g && n(5, u = g.padded), "highlight" in g && n(6, c = g.highlight), "disabled" in g && n(7, f = g.disabled), "hasPopup" in g && n(8, h = g.hasPopup), "color" in g && n(12, d = g.color), "transparent" in g && n(9, _ = g.transparent), "background" in g && n(10, m = g.background);
+    return t.$$set = (b) => {
+        "Icon" in b && n(0, o = b.Icon), "label" in b && n(1, r = b.label), "show_label" in b && n(2, s = b.show_label), "pending" in b && n(3, a = b.pending), "size" in b && n(4, l = b.size), "padded" in b && n(5, u = b.padded), "highlight" in b && n(6, c = b.highlight), "disabled" in b && n(7, f = b.disabled), "hasPopup" in b && n(8, h = b.hasPopup), "color" in b && n(12, d = b.color), "transparent" in b && n(9, _ = b.transparent), "background" in b && n(10, m = b.background);
     }, t.$$.update = () => {
         t.$$.dirty & /*highlight, color*/
             4160 && n(11, i = c ? "var(--color-accent)" : d);
     }, [
         o,
         r,
         s,
@@ -2491,21 +2491,21 @@
             background: 10
         });
     }
 }
 const {
     SvelteComponent: Lf,
     append: Rf,
-    attr: Fo,
+    attr: jo,
     binding_callbacks: Bf,
     create_slot: Mf,
     detach: Df,
     element: Ls,
-    get_all_dirty_from_scope: Of,
-    get_slot_changes: Hf,
+    get_all_dirty_from_scope: Hf,
+    get_slot_changes: Of,
     init: Nf,
     insert: If,
     safe_not_equal: Uf,
     toggle_class: Rt,
     transition_in: jf,
     transition_out: Ff,
     update_slot_base: qf
@@ -2522,15 +2522,15 @@
             t,
             /*$$scope*/
             t[4],
             null
         );
     return {
         c() {
-            e = Ls("div"), n = Ls("div"), r && r.c(), Fo(n, "class", "icon svelte-3w3rth"), Fo(e, "class", "empty svelte-3w3rth"), Fo(e, "aria-label", "Empty value"), Rt(
+            e = Ls("div"), n = Ls("div"), r && r.c(), jo(n, "class", "icon svelte-3w3rth"), jo(e, "class", "empty svelte-3w3rth"), jo(e, "aria-label", "Empty value"), Rt(
                 e,
                 "small",
                 /*size*/
                 t[0] === "small"
             ), Rt(
                 e,
                 "large",
@@ -2555,21 +2555,21 @@
             r && r.p && (!i || a & /*$$scope*/
                 16) && qf(
                 r,
                 o,
                 s,
                 /*$$scope*/
                 s[4],
-                i ? Hf(
+                i ? Of(
                     o,
                     /*$$scope*/
                     s[4],
                     a,
                     null
-                ) : Of(
+                ) : Hf(
                     /*$$scope*/
                     s[4]
                 ),
                 null
             ), (!i || a & /*size*/
                 1) && Rt(
                 e,
@@ -2678,66 +2678,66 @@
 const {
     SvelteComponent: Vf,
     append: Xf,
     attr: We,
     detach: xf,
     init: Zf,
     insert: Jf,
-    noop: qo,
+    noop: Fo,
     safe_not_equal: Yf,
     svg_element: Rs
 } = window.__gradio__svelte__internal;
 
 function Qf(t) {
     let e, n;
     return {
         c() {
             e = Rs("svg"), n = Rs("path"), We(n, "stroke", "currentColor"), We(n, "stroke-width", "1.5"), We(n, "stroke-linecap", "round"), We(n, "stroke-linejoin", "round"), We(n, "d", "M21.044 5.704a.6.6 0 0 1 .956.483v11.626a.6.6 0 0 1-.956.483l-7.889-5.813a.6.6 0 0 1 0-.966l7.89-5.813ZM10.044 5.704a.6.6 0 0 1 .956.483v11.626a.6.6 0 0 1-.956.483l-7.888-5.813a.6.6 0 0 1 0-.966l7.888-5.813Z"), We(e, "xmlns", "http://www.w3.org/2000/svg"), We(e, "width", "24px"), We(e, "height", "24px"), We(e, "fill", "currentColor"), We(e, "stroke-width", "1.5"), We(e, "viewBox", "0 0 24 24"), We(e, "color", "currentColor");
         },
         m(i, o) {
             Jf(i, e, o), Xf(e, n);
         },
-        p: qo,
-        i: qo,
-        o: qo,
+        p: Fo,
+        i: Fo,
+        o: Fo,
         d(i) {
             i && xf(e);
         }
     };
 }
 class Kf extends Vf {
     constructor(e) {
         super(), Zf(this, e, null, Qf, Yf, {});
     }
 }
 const {
     SvelteComponent: $f,
-    append: zo,
+    append: qo,
     attr: et,
     detach: ed,
     init: td,
     insert: nd,
-    noop: Go,
+    noop: zo,
     safe_not_equal: id,
     set_style: ht,
     svg_element: ji
 } = window.__gradio__svelte__internal;
 
 function od(t) {
     let e, n, i, o;
     return {
         c() {
             e = ji("svg"), n = ji("g"), i = ji("path"), o = ji("path"), et(i, "d", "M18,6L6.087,17.913"), ht(i, "fill", "none"), ht(i, "fill-rule", "nonzero"), ht(i, "stroke-width", "2px"), et(n, "transform", "matrix(1.14096,-0.140958,-0.140958,1.14096,-0.0559523,0.0559523)"), et(o, "d", "M4.364,4.364L19.636,19.636"), ht(o, "fill", "none"), ht(o, "fill-rule", "nonzero"), ht(o, "stroke-width", "2px"), et(e, "width", "100%"), et(e, "height", "100%"), et(e, "viewBox", "0 0 24 24"), et(e, "version", "1.1"), et(e, "xmlns", "http://www.w3.org/2000/svg"), et(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), et(e, "xml:space", "preserve"), et(e, "stroke", "currentColor"), ht(e, "fill-rule", "evenodd"), ht(e, "clip-rule", "evenodd"), ht(e, "stroke-linecap", "round"), ht(e, "stroke-linejoin", "round");
         },
         m(r, s) {
-            nd(r, e, s), zo(e, n), zo(n, i), zo(e, o);
+            nd(r, e, s), qo(e, n), qo(n, i), qo(e, o);
         },
-        p: Go,
-        i: Go,
-        o: Go,
+        p: zo,
+        i: zo,
+        o: zo,
         d(r) {
             r && ed(e);
         }
     };
 }
 class rd extends $f {
     constructor(e) {
@@ -2747,31 +2747,31 @@
 const {
     SvelteComponent: sd,
     append: ld,
     attr: yn,
     detach: ad,
     init: ud,
     insert: cd,
-    noop: Wo,
+    noop: Go,
     safe_not_equal: fd,
     svg_element: Bs
 } = window.__gradio__svelte__internal;
 
 function dd(t) {
     let e, n;
     return {
         c() {
             e = Bs("svg"), n = Bs("path"), yn(n, "fill", "currentColor"), yn(n, "d", "M26 24v4H6v-4H4v4a2 2 0 0 0 2 2h20a2 2 0 0 0 2-2v-4zm0-10l-1.41-1.41L17 20.17V2h-2v18.17l-7.59-7.58L6 14l10 10l10-10z"), yn(e, "xmlns", "http://www.w3.org/2000/svg"), yn(e, "width", "100%"), yn(e, "height", "100%"), yn(e, "viewBox", "0 0 32 32");
         },
         m(i, o) {
             cd(i, e, o), ld(e, n);
         },
-        p: Wo,
-        i: Wo,
-        o: Wo,
+        p: Go,
+        i: Go,
+        o: Go,
         d(i) {
             i && ad(e);
         }
     };
 }
 class qa extends sd {
     constructor(e) {
@@ -2781,31 +2781,31 @@
 const {
     SvelteComponent: hd,
     append: _d,
     attr: tt,
     detach: md,
     init: pd,
     insert: gd,
-    noop: Vo,
+    noop: Wo,
     safe_not_equal: bd,
     svg_element: Ms
 } = window.__gradio__svelte__internal;
 
 function vd(t) {
     let e, n;
     return {
         c() {
             e = Ms("svg"), n = Ms("path"), tt(n, "d", "M17 3a2.828 2.828 0 1 1 4 4L7.5 20.5 2 22l1.5-5.5L17 3z"), tt(e, "xmlns", "http://www.w3.org/2000/svg"), tt(e, "width", "100%"), tt(e, "height", "100%"), tt(e, "viewBox", "0 0 24 24"), tt(e, "fill", "none"), tt(e, "stroke", "currentColor"), tt(e, "stroke-width", "1.5"), tt(e, "stroke-linecap", "round"), tt(e, "stroke-linejoin", "round"), tt(e, "class", "feather feather-edit-2");
         },
         m(i, o) {
             gd(i, e, o), _d(e, n);
         },
-        p: Vo,
-        i: Vo,
-        o: Vo,
+        p: Wo,
+        i: Wo,
+        o: Wo,
         d(i) {
             i && md(e);
         }
     };
 }
 class wd extends hd {
     constructor(e) {
@@ -2815,31 +2815,31 @@
 const {
     SvelteComponent: yd,
     append: kd,
     attr: Ve,
     detach: Ed,
     init: Cd,
     insert: Sd,
-    noop: Xo,
+    noop: Vo,
     safe_not_equal: Ad,
     svg_element: Ds
 } = window.__gradio__svelte__internal;
 
 function Td(t) {
     let e, n;
     return {
         c() {
             e = Ds("svg"), n = Ds("path"), Ve(n, "stroke", "currentColor"), Ve(n, "stroke-width", "1.5"), Ve(n, "stroke-linecap", "round"), Ve(n, "stroke-linejoin", "round"), Ve(n, "d", "M2.956 5.704A.6.6 0 0 0 2 6.187v11.626a.6.6 0 0 0 .956.483l7.889-5.813a.6.6 0 0 0 0-.966l-7.89-5.813ZM13.956 5.704a.6.6 0 0 0-.956.483v11.626a.6.6 0 0 0 .956.483l7.889-5.813a.6.6 0 0 0 0-.966l-7.89-5.813Z"), Ve(e, "xmlns", "http://www.w3.org/2000/svg"), Ve(e, "width", "24px"), Ve(e, "height", "24px"), Ve(e, "fill", "currentColor"), Ve(e, "stroke-width", "1.5"), Ve(e, "viewBox", "0 0 24 24"), Ve(e, "color", "currentColor");
         },
         m(i, o) {
             Sd(i, e, o), kd(e, n);
         },
-        p: Xo,
-        i: Xo,
-        o: Xo,
+        p: Vo,
+        i: Vo,
+        o: Vo,
         d(i) {
             i && Ed(e);
         }
     };
 }
 class Pd extends yd {
     constructor(e) {
@@ -2849,133 +2849,133 @@
 const {
     SvelteComponent: Ld,
     append: Rd,
     attr: kn,
     detach: Bd,
     init: Md,
     insert: Dd,
-    noop: xo,
-    safe_not_equal: Od,
-    svg_element: Os
+    noop: Xo,
+    safe_not_equal: Hd,
+    svg_element: Hs
 } = window.__gradio__svelte__internal;
 
-function Hd(t) {
+function Od(t) {
     let e, n;
     return {
         c() {
-            e = Os("svg"), n = Os("path"), kn(n, "fill", "currentColor"), kn(n, "d", "M13.75 2a2.25 2.25 0 0 1 2.236 2.002V4h1.764A2.25 2.25 0 0 1 20 6.25V11h-1.5V6.25a.75.75 0 0 0-.75-.75h-2.129c-.404.603-1.091 1-1.871 1h-3.5c-.78 0-1.467-.397-1.871-1H6.25a.75.75 0 0 0-.75.75v13.5c0 .414.336.75.75.75h4.78a3.99 3.99 0 0 0 .505 1.5H6.25A2.25 2.25 0 0 1 4 19.75V6.25A2.25 2.25 0 0 1 6.25 4h1.764a2.25 2.25 0 0 1 2.236-2h3.5Zm2.245 2.096L16 4.25c0-.052-.002-.103-.005-.154ZM13.75 3.5h-3.5a.75.75 0 0 0 0 1.5h3.5a.75.75 0 0 0 0-1.5ZM15 12a3 3 0 0 0-3 3v5c0 .556.151 1.077.415 1.524l3.494-3.494a2.25 2.25 0 0 1 3.182 0l3.494 3.494c.264-.447.415-.968.415-1.524v-5a3 3 0 0 0-3-3h-5Zm0 11a2.985 2.985 0 0 1-1.524-.415l3.494-3.494a.75.75 0 0 1 1.06 0l3.494 3.494A2.985 2.985 0 0 1 20 23h-5Zm5-7a1 1 0 1 1 0-2a1 1 0 0 1 0 2Z"), kn(e, "xmlns", "http://www.w3.org/2000/svg"), kn(e, "width", "100%"), kn(e, "height", "100%"), kn(e, "viewBox", "0 0 24 24");
+            e = Hs("svg"), n = Hs("path"), kn(n, "fill", "currentColor"), kn(n, "d", "M13.75 2a2.25 2.25 0 0 1 2.236 2.002V4h1.764A2.25 2.25 0 0 1 20 6.25V11h-1.5V6.25a.75.75 0 0 0-.75-.75h-2.129c-.404.603-1.091 1-1.871 1h-3.5c-.78 0-1.467-.397-1.871-1H6.25a.75.75 0 0 0-.75.75v13.5c0 .414.336.75.75.75h4.78a3.99 3.99 0 0 0 .505 1.5H6.25A2.25 2.25 0 0 1 4 19.75V6.25A2.25 2.25 0 0 1 6.25 4h1.764a2.25 2.25 0 0 1 2.236-2h3.5Zm2.245 2.096L16 4.25c0-.052-.002-.103-.005-.154ZM13.75 3.5h-3.5a.75.75 0 0 0 0 1.5h3.5a.75.75 0 0 0 0-1.5ZM15 12a3 3 0 0 0-3 3v5c0 .556.151 1.077.415 1.524l3.494-3.494a2.25 2.25 0 0 1 3.182 0l3.494 3.494c.264-.447.415-.968.415-1.524v-5a3 3 0 0 0-3-3h-5Zm0 11a2.985 2.985 0 0 1-1.524-.415l3.494-3.494a.75.75 0 0 1 1.06 0l3.494 3.494A2.985 2.985 0 0 1 20 23h-5Zm5-7a1 1 0 1 1 0-2a1 1 0 0 1 0 2Z"), kn(e, "xmlns", "http://www.w3.org/2000/svg"), kn(e, "width", "100%"), kn(e, "height", "100%"), kn(e, "viewBox", "0 0 24 24");
         },
         m(i, o) {
             Dd(i, e, o), Rd(e, n);
         },
-        p: xo,
-        i: xo,
-        o: xo,
+        p: Xo,
+        i: Xo,
+        o: Xo,
         d(i) {
             i && Bd(e);
         }
     };
 }
 class za extends Ld {
     constructor(e) {
-        super(), Md(this, e, null, Hd, Od, {});
+        super(), Md(this, e, null, Od, Hd, {});
     }
 }
 const {
     SvelteComponent: Nd,
     append: Fi,
-    attr: pe,
+    attr: me,
     detach: Id,
     init: Ud,
     insert: jd,
-    noop: Zo,
+    noop: xo,
     safe_not_equal: Fd,
     svg_element: ni
 } = window.__gradio__svelte__internal;
 
 function qd(t) {
     let e, n, i, o, r;
     return {
         c() {
-            e = ni("svg"), n = ni("path"), i = ni("path"), o = ni("line"), r = ni("line"), pe(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), pe(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), pe(o, "x1", "12"), pe(o, "y1", "19"), pe(o, "x2", "12"), pe(o, "y2", "23"), pe(r, "x1", "8"), pe(r, "y1", "23"), pe(r, "x2", "16"), pe(r, "y2", "23"), pe(e, "xmlns", "http://www.w3.org/2000/svg"), pe(e, "width", "100%"), pe(e, "height", "100%"), pe(e, "viewBox", "0 0 24 24"), pe(e, "fill", "none"), pe(e, "stroke", "currentColor"), pe(e, "stroke-width", "2"), pe(e, "stroke-linecap", "round"), pe(e, "stroke-linejoin", "round"), pe(e, "class", "feather feather-mic");
+            e = ni("svg"), n = ni("path"), i = ni("path"), o = ni("line"), r = ni("line"), me(n, "d", "M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z"), me(i, "d", "M19 10v2a7 7 0 0 1-14 0v-2"), me(o, "x1", "12"), me(o, "y1", "19"), me(o, "x2", "12"), me(o, "y2", "23"), me(r, "x1", "8"), me(r, "y1", "23"), me(r, "x2", "16"), me(r, "y2", "23"), me(e, "xmlns", "http://www.w3.org/2000/svg"), me(e, "width", "100%"), me(e, "height", "100%"), me(e, "viewBox", "0 0 24 24"), me(e, "fill", "none"), me(e, "stroke", "currentColor"), me(e, "stroke-width", "2"), me(e, "stroke-linecap", "round"), me(e, "stroke-linejoin", "round"), me(e, "class", "feather feather-mic");
         },
         m(s, a) {
             jd(s, e, a), Fi(e, n), Fi(e, i), Fi(e, o), Fi(e, r);
         },
-        p: Zo,
-        i: Zo,
-        o: Zo,
+        p: xo,
+        i: xo,
+        o: xo,
         d(s) {
             s && Id(e);
         }
     };
 }
 class zd extends Nd {
     constructor(e) {
         super(), Ud(this, e, null, qd, Fd, {});
     }
 }
 const {
     SvelteComponent: Gd,
-    append: Jo,
+    append: Zo,
     attr: Pe,
     detach: Wd,
     init: Vd,
     insert: Xd,
-    noop: Yo,
+    noop: Jo,
     safe_not_equal: xd,
     svg_element: qi
 } = window.__gradio__svelte__internal;
 
 function Zd(t) {
     let e, n, i, o;
     return {
         c() {
             e = qi("svg"), n = qi("path"), i = qi("circle"), o = qi("circle"), Pe(n, "d", "M9 18V5l12-2v13"), Pe(i, "cx", "6"), Pe(i, "cy", "18"), Pe(i, "r", "3"), Pe(o, "cx", "18"), Pe(o, "cy", "16"), Pe(o, "r", "3"), Pe(e, "xmlns", "http://www.w3.org/2000/svg"), Pe(e, "width", "100%"), Pe(e, "height", "100%"), Pe(e, "viewBox", "0 0 24 24"), Pe(e, "fill", "none"), Pe(e, "stroke", "currentColor"), Pe(e, "stroke-width", "1.5"), Pe(e, "stroke-linecap", "round"), Pe(e, "stroke-linejoin", "round"), Pe(e, "class", "feather feather-music");
         },
         m(r, s) {
-            Xd(r, e, s), Jo(e, n), Jo(e, i), Jo(e, o);
+            Xd(r, e, s), Zo(e, n), Zo(e, i), Zo(e, o);
         },
-        p: Yo,
-        i: Yo,
-        o: Yo,
+        p: Jo,
+        i: Jo,
+        o: Jo,
         d(r) {
             r && Wd(e);
         }
     };
 }
-class po extends Gd {
+class mo extends Gd {
     constructor(e) {
         super(), Vd(this, e, null, Zd, xd, {});
     }
 }
 const {
     SvelteComponent: Jd,
-    append: Hs,
+    append: Os,
     attr: Le,
     detach: Yd,
     init: Qd,
     insert: Kd,
-    noop: Qo,
+    noop: Yo,
     safe_not_equal: $d,
-    svg_element: Ko
+    svg_element: Qo
 } = window.__gradio__svelte__internal;
 
 function eh(t) {
     let e, n, i;
     return {
         c() {
-            e = Ko("svg"), n = Ko("rect"), i = Ko("rect"), Le(n, "x", "6"), Le(n, "y", "4"), Le(n, "width", "4"), Le(n, "height", "16"), Le(i, "x", "14"), Le(i, "y", "4"), Le(i, "width", "4"), Le(i, "height", "16"), Le(e, "xmlns", "http://www.w3.org/2000/svg"), Le(e, "width", "100%"), Le(e, "height", "100%"), Le(e, "viewBox", "0 0 24 24"), Le(e, "fill", "currentColor"), Le(e, "stroke", "currentColor"), Le(e, "stroke-width", "1.5"), Le(e, "stroke-linecap", "round"), Le(e, "stroke-linejoin", "round");
+            e = Qo("svg"), n = Qo("rect"), i = Qo("rect"), Le(n, "x", "6"), Le(n, "y", "4"), Le(n, "width", "4"), Le(n, "height", "16"), Le(i, "x", "14"), Le(i, "y", "4"), Le(i, "width", "4"), Le(i, "height", "16"), Le(e, "xmlns", "http://www.w3.org/2000/svg"), Le(e, "width", "100%"), Le(e, "height", "100%"), Le(e, "viewBox", "0 0 24 24"), Le(e, "fill", "currentColor"), Le(e, "stroke", "currentColor"), Le(e, "stroke-width", "1.5"), Le(e, "stroke-linecap", "round"), Le(e, "stroke-linejoin", "round");
         },
         m(o, r) {
-            Kd(o, e, r), Hs(e, n), Hs(e, i);
+            Kd(o, e, r), Os(e, n), Os(e, i);
         },
-        p: Qo,
-        i: Qo,
-        o: Qo,
+        p: Yo,
+        i: Yo,
+        o: Yo,
         d(o) {
             o && Yd(e);
         }
     };
 }
 class Ga extends Jd {
     constructor(e) {
@@ -2985,65 +2985,65 @@
 const {
     SvelteComponent: th,
     append: nh,
     attr: _t,
     detach: ih,
     init: oh,
     insert: rh,
-    noop: $o,
+    noop: Ko,
     safe_not_equal: sh,
     svg_element: Ns
 } = window.__gradio__svelte__internal;
 
 function lh(t) {
     let e, n;
     return {
         c() {
             e = Ns("svg"), n = Ns("polygon"), _t(n, "points", "5 3 19 12 5 21 5 3"), _t(e, "xmlns", "http://www.w3.org/2000/svg"), _t(e, "width", "100%"), _t(e, "height", "100%"), _t(e, "viewBox", "0 0 24 24"), _t(e, "fill", "currentColor"), _t(e, "stroke", "currentColor"), _t(e, "stroke-width", "1.5"), _t(e, "stroke-linecap", "round"), _t(e, "stroke-linejoin", "round");
         },
         m(i, o) {
             rh(i, e, o), nh(e, n);
         },
-        p: $o,
-        i: $o,
-        o: $o,
+        p: Ko,
+        i: Ko,
+        o: Ko,
         d(i) {
             i && ih(e);
         }
     };
 }
 class ah extends th {
     constructor(e) {
         super(), oh(this, e, null, lh, sh, {});
     }
 }
 const {
     SvelteComponent: uh,
     append: ii,
-    attr: le,
+    attr: se,
     detach: ch,
     init: fh,
     insert: dh,
-    noop: er,
+    noop: $o,
     safe_not_equal: hh,
     svg_element: En
 } = window.__gradio__svelte__internal;
 
 function _h(t) {
     let e, n, i, o, r, s;
     return {
         c() {
-            e = En("svg"), n = En("circle"), i = En("circle"), o = En("line"), r = En("line"), s = En("line"), le(n, "cx", "6"), le(n, "cy", "6"), le(n, "r", "3"), le(i, "cx", "6"), le(i, "cy", "18"), le(i, "r", "3"), le(o, "x1", "20"), le(o, "y1", "4"), le(o, "x2", "8.12"), le(o, "y2", "15.88"), le(r, "x1", "14.47"), le(r, "y1", "14.48"), le(r, "x2", "20"), le(r, "y2", "20"), le(s, "x1", "8.12"), le(s, "y1", "8.12"), le(s, "x2", "12"), le(s, "y2", "12"), le(e, "xmlns", "http://www.w3.org/2000/svg"), le(e, "width", "100%"), le(e, "height", "100%"), le(e, "viewBox", "0 0 24 24"), le(e, "fill", "none"), le(e, "stroke", "currentColor"), le(e, "stroke-width", "2"), le(e, "stroke-linecap", "round"), le(e, "stroke-linejoin", "round"), le(e, "class", "feather feather-scissors");
+            e = En("svg"), n = En("circle"), i = En("circle"), o = En("line"), r = En("line"), s = En("line"), se(n, "cx", "6"), se(n, "cy", "6"), se(n, "r", "3"), se(i, "cx", "6"), se(i, "cy", "18"), se(i, "r", "3"), se(o, "x1", "20"), se(o, "y1", "4"), se(o, "x2", "8.12"), se(o, "y2", "15.88"), se(r, "x1", "14.47"), se(r, "y1", "14.48"), se(r, "x2", "20"), se(r, "y2", "20"), se(s, "x1", "8.12"), se(s, "y1", "8.12"), se(s, "x2", "12"), se(s, "y2", "12"), se(e, "xmlns", "http://www.w3.org/2000/svg"), se(e, "width", "100%"), se(e, "height", "100%"), se(e, "viewBox", "0 0 24 24"), se(e, "fill", "none"), se(e, "stroke", "currentColor"), se(e, "stroke-width", "2"), se(e, "stroke-linecap", "round"), se(e, "stroke-linejoin", "round"), se(e, "class", "feather feather-scissors");
         },
         m(a, l) {
             dh(a, e, l), ii(e, n), ii(e, i), ii(e, o), ii(e, r), ii(e, s);
         },
-        p: er,
-        i: er,
-        o: er,
+        p: $o,
+        i: $o,
+        o: $o,
         d(a) {
             a && ch(e);
         }
     };
 }
 class mh extends uh {
     constructor(e) {
@@ -3053,65 +3053,65 @@
 const {
     SvelteComponent: ph,
     append: Is,
     attr: Xe,
     detach: gh,
     init: bh,
     insert: vh,
-    noop: tr,
+    noop: er,
     safe_not_equal: wh,
-    svg_element: nr
+    svg_element: tr
 } = window.__gradio__svelte__internal;
 
 function yh(t) {
     let e, n, i;
     return {
         c() {
-            e = nr("svg"), n = nr("polyline"), i = nr("path"), Xe(n, "points", "1 4 1 10 7 10"), Xe(i, "d", "M3.51 15a9 9 0 1 0 2.13-9.36L1 10"), Xe(e, "xmlns", "http://www.w3.org/2000/svg"), Xe(e, "width", "100%"), Xe(e, "height", "100%"), Xe(e, "viewBox", "0 0 24 24"), Xe(e, "fill", "none"), Xe(e, "stroke", "currentColor"), Xe(e, "stroke-width", "2"), Xe(e, "stroke-linecap", "round"), Xe(e, "stroke-linejoin", "round"), Xe(e, "class", "feather feather-rotate-ccw");
+            e = tr("svg"), n = tr("polyline"), i = tr("path"), Xe(n, "points", "1 4 1 10 7 10"), Xe(i, "d", "M3.51 15a9 9 0 1 0 2.13-9.36L1 10"), Xe(e, "xmlns", "http://www.w3.org/2000/svg"), Xe(e, "width", "100%"), Xe(e, "height", "100%"), Xe(e, "viewBox", "0 0 24 24"), Xe(e, "fill", "none"), Xe(e, "stroke", "currentColor"), Xe(e, "stroke-width", "2"), Xe(e, "stroke-linecap", "round"), Xe(e, "stroke-linejoin", "round"), Xe(e, "class", "feather feather-rotate-ccw");
         },
         m(o, r) {
             vh(o, e, r), Is(e, n), Is(e, i);
         },
-        p: tr,
-        i: tr,
-        o: tr,
+        p: er,
+        i: er,
+        o: er,
         d(o) {
             o && gh(e);
         }
     };
 }
 class Wa extends ph {
     constructor(e) {
         super(), bh(this, e, null, yh, wh, {});
     }
 }
 const {
     SvelteComponent: kh,
-    append: ir,
+    append: nr,
     attr: Re,
     detach: Eh,
     init: Ch,
     insert: Sh,
-    noop: or,
+    noop: ir,
     safe_not_equal: Ah,
     svg_element: zi
 } = window.__gradio__svelte__internal;
 
 function Th(t) {
     let e, n, i, o;
     return {
         c() {
             e = zi("svg"), n = zi("path"), i = zi("polyline"), o = zi("line"), Re(n, "d", "M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"), Re(i, "points", "17 8 12 3 7 8"), Re(o, "x1", "12"), Re(o, "y1", "3"), Re(o, "x2", "12"), Re(o, "y2", "15"), Re(e, "xmlns", "http://www.w3.org/2000/svg"), Re(e, "width", "90%"), Re(e, "height", "90%"), Re(e, "viewBox", "0 0 24 24"), Re(e, "fill", "none"), Re(e, "stroke", "currentColor"), Re(e, "stroke-width", "2"), Re(e, "stroke-linecap", "round"), Re(e, "stroke-linejoin", "round"), Re(e, "class", "feather feather-upload");
         },
         m(r, s) {
-            Sh(r, e, s), ir(e, n), ir(e, i), ir(e, o);
+            Sh(r, e, s), nr(e, n), nr(e, i), nr(e, o);
         },
-        p: or,
-        i: or,
-        o: or,
+        p: ir,
+        i: ir,
+        o: ir,
         d(r) {
             r && Eh(e);
         }
     };
 }
 let Va = class extends kh {
     constructor(e) {
@@ -3121,102 +3121,102 @@
 const {
     SvelteComponent: Ph,
     append: Gi,
     attr: Ne,
     detach: Lh,
     init: Rh,
     insert: Bh,
-    noop: rr,
+    noop: or,
     safe_not_equal: Mh,
     svg_element: Wi,
     text: Dh
 } = window.__gradio__svelte__internal;
 
-function Oh(t) {
+function Hh(t) {
     let e, n, i, o, r;
     return {
         c() {
             e = Wi("svg"), n = Wi("title"), i = Dh("Low volume"), o = Wi("path"), r = Wi("path"), Ne(o, "d", "M19.5 7.5C19.5 7.5 21 9 21 11.5C21 14 19.5 15.5 19.5 15.5"), Ne(o, "stroke-width", "1.5"), Ne(o, "stroke-linecap", "round"), Ne(o, "stroke-linejoin", "round"), Ne(r, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), Ne(r, "stroke-width", "1.5"), Ne(e, "width", "100%"), Ne(e, "height", "100%"), Ne(e, "viewBox", "0 0 24 24"), Ne(e, "stroke-width", "1.5"), Ne(e, "fill", "none"), Ne(e, "xmlns", "http://www.w3.org/2000/svg"), Ne(e, "stroke", "currentColor"), Ne(e, "color", "currentColor");
         },
         m(s, a) {
             Bh(s, e, a), Gi(e, n), Gi(n, i), Gi(e, o), Gi(e, r);
         },
-        p: rr,
-        i: rr,
-        o: rr,
+        p: or,
+        i: or,
+        o: or,
         d(s) {
             s && Lh(e);
         }
     };
 }
-class Hh extends Ph {
+class Oh extends Ph {
     constructor(e) {
-        super(), Rh(this, e, null, Oh, Mh, {});
+        super(), Rh(this, e, null, Hh, Mh, {});
     }
 }
 const {
     SvelteComponent: Nh,
     append: oi,
     attr: Ae,
     detach: Ih,
     init: Uh,
     insert: jh,
-    noop: sr,
+    noop: rr,
     safe_not_equal: Fh,
     svg_element: ri,
     text: qh
 } = window.__gradio__svelte__internal;
 
 function zh(t) {
     let e, n, i, o, r, s;
     return {
         c() {
             e = ri("svg"), n = ri("title"), i = qh("High volume"), o = ri("path"), r = ri("path"), s = ri("path"), Ae(o, "d", "M1 13.8571V10.1429C1 9.03829 1.89543 8.14286 3 8.14286H5.9C6.09569 8.14286 6.28708 8.08544 6.45046 7.97772L12.4495 4.02228C13.1144 3.5839 14 4.06075 14 4.85714V19.1429C14 19.9392 13.1144 20.4161 12.4495 19.9777L6.45046 16.0223C6.28708 15.9146 6.09569 15.8571 5.9 15.8571H3C1.89543 15.8571 1 14.9617 1 13.8571Z"), Ae(o, "stroke-width", "1.5"), Ae(r, "d", "M17.5 7.5C17.5 7.5 19 9 19 11.5C19 14 17.5 15.5 17.5 15.5"), Ae(r, "stroke-width", "1.5"), Ae(r, "stroke-linecap", "round"), Ae(r, "stroke-linejoin", "round"), Ae(s, "d", "M20.5 4.5C20.5 4.5 23 7 23 11.5C23 16 20.5 18.5 20.5 18.5"), Ae(s, "stroke-width", "1.5"), Ae(s, "stroke-linecap", "round"), Ae(s, "stroke-linejoin", "round"), Ae(e, "width", "100%"), Ae(e, "height", "100%"), Ae(e, "viewBox", "0 0 24 24"), Ae(e, "stroke-width", "1.5"), Ae(e, "fill", "none"), Ae(e, "stroke", "currentColor"), Ae(e, "xmlns", "http://www.w3.org/2000/svg"), Ae(e, "color", "currentColor");
         },
         m(a, l) {
             jh(a, e, l), oi(e, n), oi(n, i), oi(e, o), oi(e, r), oi(e, s);
         },
-        p: sr,
-        i: sr,
-        o: sr,
+        p: rr,
+        i: rr,
+        o: rr,
         d(a) {
             a && Ih(e);
         }
     };
 }
 class Gh extends Nh {
     constructor(e) {
         super(), Uh(this, e, null, zh, Fh, {});
     }
 }
 const {
     SvelteComponent: Wh,
     append: Bt,
-    attr: ve,
+    attr: we,
     detach: Vh,
     init: Xh,
     insert: xh,
-    noop: lr,
+    noop: sr,
     safe_not_equal: Zh,
     svg_element: Mt,
     text: Jh
 } = window.__gradio__svelte__internal;
 
 function Yh(t) {
     let e, n, i, o, r, s, a, l, u;
     return {
         c() {
-            e = Mt("svg"), n = Mt("title"), i = Jh("Muted volume"), o = Mt("g"), r = Mt("path"), s = Mt("path"), a = Mt("defs"), l = Mt("clipPath"), u = Mt("rect"), ve(r, "d", "M18 14L20.0005 12M22 10L20.0005 12M20.0005 12L18 10M20.0005 12L22 14"), ve(r, "stroke-width", "1.5"), ve(r, "stroke-linecap", "round"), ve(r, "stroke-linejoin", "round"), ve(s, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), ve(s, "stroke-width", "1.5"), ve(o, "clip-path", "url(#clip0_3173_16686)"), ve(u, "width", "24"), ve(u, "height", "24"), ve(u, "fill", "white"), ve(l, "id", "clip0_3173_16686"), ve(e, "width", "100%"), ve(e, "height", "100%"), ve(e, "viewBox", "0 0 24 24"), ve(e, "stroke-width", "1.5"), ve(e, "fill", "none"), ve(e, "xmlns", "http://www.w3.org/2000/svg"), ve(e, "stroke", "currentColor"), ve(e, "color", "currentColor");
+            e = Mt("svg"), n = Mt("title"), i = Jh("Muted volume"), o = Mt("g"), r = Mt("path"), s = Mt("path"), a = Mt("defs"), l = Mt("clipPath"), u = Mt("rect"), we(r, "d", "M18 14L20.0005 12M22 10L20.0005 12M20.0005 12L18 10M20.0005 12L22 14"), we(r, "stroke-width", "1.5"), we(r, "stroke-linecap", "round"), we(r, "stroke-linejoin", "round"), we(s, "d", "M2 13.8571V10.1429C2 9.03829 2.89543 8.14286 4 8.14286H6.9C7.09569 8.14286 7.28708 8.08544 7.45046 7.97772L13.4495 4.02228C14.1144 3.5839 15 4.06075 15 4.85714V19.1429C15 19.9392 14.1144 20.4161 13.4495 19.9777L7.45046 16.0223C7.28708 15.9146 7.09569 15.8571 6.9 15.8571H4C2.89543 15.8571 2 14.9617 2 13.8571Z"), we(s, "stroke-width", "1.5"), we(o, "clip-path", "url(#clip0_3173_16686)"), we(u, "width", "24"), we(u, "height", "24"), we(u, "fill", "white"), we(l, "id", "clip0_3173_16686"), we(e, "width", "100%"), we(e, "height", "100%"), we(e, "viewBox", "0 0 24 24"), we(e, "stroke-width", "1.5"), we(e, "fill", "none"), we(e, "xmlns", "http://www.w3.org/2000/svg"), we(e, "stroke", "currentColor"), we(e, "color", "currentColor");
         },
         m(c, f) {
             xh(c, e, f), Bt(e, n), Bt(n, i), Bt(e, o), Bt(o, r), Bt(o, s), Bt(e, a), Bt(a, l), Bt(l, u);
         },
-        p: lr,
-        i: lr,
-        o: lr,
+        p: sr,
+        i: sr,
+        o: sr,
         d(c) {
             c && Vh(e);
         }
     };
 }
 class Qh extends Wh {
     constructor(e) {
@@ -3226,77 +3226,77 @@
 const {
     SvelteComponent: Kh,
     append: Us,
     attr: Dt,
     detach: $h,
     init: e_,
     insert: t_,
-    noop: ar,
+    noop: lr,
     safe_not_equal: n_,
-    svg_element: ur
+    svg_element: ar
 } = window.__gradio__svelte__internal;
 
 function i_(t) {
     let e, n, i;
     return {
         c() {
-            e = ur("svg"), n = ur("path"), i = ur("path"), Dt(n, "fill", "currentColor"), Dt(n, "d", "M12 2c-4.963 0-9 4.038-9 9c0 3.328 1.82 6.232 4.513 7.79l-2.067 1.378A1 1 0 0 0 6 22h12a1 1 0 0 0 .555-1.832l-2.067-1.378C19.18 17.232 21 14.328 21 11c0-4.962-4.037-9-9-9zm0 16c-3.859 0-7-3.141-7-7c0-3.86 3.141-7 7-7s7 3.14 7 7c0 3.859-3.141 7-7 7z"), Dt(i, "fill", "currentColor"), Dt(i, "d", "M12 6c-2.757 0-5 2.243-5 5s2.243 5 5 5s5-2.243 5-5s-2.243-5-5-5zm0 8c-1.654 0-3-1.346-3-3s1.346-3 3-3s3 1.346 3 3s-1.346 3-3 3z"), Dt(e, "xmlns", "http://www.w3.org/2000/svg"), Dt(e, "width", "100%"), Dt(e, "height", "100%"), Dt(e, "viewBox", "0 0 24 24");
+            e = ar("svg"), n = ar("path"), i = ar("path"), Dt(n, "fill", "currentColor"), Dt(n, "d", "M12 2c-4.963 0-9 4.038-9 9c0 3.328 1.82 6.232 4.513 7.79l-2.067 1.378A1 1 0 0 0 6 22h12a1 1 0 0 0 .555-1.832l-2.067-1.378C19.18 17.232 21 14.328 21 11c0-4.962-4.037-9-9-9zm0 16c-3.859 0-7-3.141-7-7c0-3.86 3.141-7 7-7s7 3.14 7 7c0 3.859-3.141 7-7 7z"), Dt(i, "fill", "currentColor"), Dt(i, "d", "M12 6c-2.757 0-5 2.243-5 5s2.243 5 5 5s5-2.243 5-5s-2.243-5-5-5zm0 8c-1.654 0-3-1.346-3-3s1.346-3 3-3s3 1.346 3 3s-1.346 3-3 3z"), Dt(e, "xmlns", "http://www.w3.org/2000/svg"), Dt(e, "width", "100%"), Dt(e, "height", "100%"), Dt(e, "viewBox", "0 0 24 24");
         },
         m(o, r) {
             t_(o, e, r), Us(e, n), Us(e, i);
         },
-        p: ar,
-        i: ar,
-        o: ar,
+        p: lr,
+        i: lr,
+        o: lr,
         d(o) {
             o && $h(e);
         }
     };
 }
 class o_ extends Kh {
     constructor(e) {
         super(), e_(this, e, null, i_, n_, {});
     }
 }
 const {
     SvelteComponent: r_,
     append: Kt,
-    attr: Or,
+    attr: Dr,
     check_outros: s_,
     create_component: Xa,
     destroy_component: xa,
     detach: Qi,
     element: Hr,
     group_outros: l_,
     init: a_,
     insert: Ki,
     mount_component: Za,
     safe_not_equal: u_,
-    set_data: Nr,
-    space: Ir,
+    set_data: Or,
+    space: Nr,
     text: fi,
     toggle_class: js,
-    transition_in: io,
-    transition_out: oo
+    transition_in: no,
+    transition_out: io
 } = window.__gradio__svelte__internal;
 
 function c_(t) {
     let e, n;
     return e = new Va({}), {
         c() {
             Xa(e.$$.fragment);
         },
         m(i, o) {
             Za(e, i, o), n = !0;
         },
         i(i) {
-            n || (io(e.$$.fragment, i), n = !0);
+            n || (no(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            oo(e.$$.fragment, i), n = !1;
+            io(e.$$.fragment, i), n = !1;
         },
         d(i) {
             xa(e, i);
         }
     };
 }
 
@@ -3306,18 +3306,18 @@
         c() {
             Xa(e.$$.fragment);
         },
         m(i, o) {
             Za(e, i, o), n = !0;
         },
         i(i) {
-            n || (io(e.$$.fragment, i), n = !0);
+            n || (no(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            oo(e.$$.fragment, i), n = !1;
+            io(e.$$.fragment, i), n = !1;
         },
         d(i) {
             xa(e, i);
         }
     };
 }
 
@@ -3330,26 +3330,26 @@
             /*message*/
             (t[2] || /*i18n*/
                 t[1]("upload_text.click_to_upload")) + ""
         ),
         l;
     return {
         c() {
-            e = Hr("span"), n = fi("- "), o = fi(i), r = fi(" -"), s = Ir(), l = fi(a), Or(e, "class", "or svelte-kzcjhc");
+            e = Hr("span"), n = fi("- "), o = fi(i), r = fi(" -"), s = Nr(), l = fi(a), Dr(e, "class", "or svelte-kzcjhc");
         },
         m(u, c) {
             Ki(u, e, c), Kt(e, n), Kt(e, o), Kt(e, r), Ki(u, s, c), Ki(u, l, c);
         },
         p(u, c) {
             c & /*i18n*/
                 2 && i !== (i = /*i18n*/
-                    u[1]("common.or") + "") && Nr(o, i), c & /*message, i18n*/
+                    u[1]("common.or") + "") && Or(o, i), c & /*message, i18n*/
                 6 && a !== (a = /*message*/
                     (u[2] || /*i18n*/
-                        u[1]("upload_text.click_to_upload")) + "") && Nr(l, a);
+                        u[1]("upload_text.click_to_upload")) + "") && Or(l, a);
         },
         d(u) {
             u && (Qi(e), Qi(s), Qi(l));
         }
     };
 }
 
@@ -3378,51 +3378,51 @@
     i = h(t), o = f[i] = c[i](t);
     let d = (
         /*mode*/
         t[3] !== "short" && Fs(t)
     );
     return {
         c() {
-            e = Hr("div"), n = Hr("span"), o.c(), r = Ir(), a = fi(s), l = Ir(), d && d.c(), Or(n, "class", "icon-wrap svelte-kzcjhc"), js(
+            e = Hr("div"), n = Hr("span"), o.c(), r = Nr(), a = fi(s), l = Nr(), d && d.c(), Dr(n, "class", "icon-wrap svelte-kzcjhc"), js(
                 n,
                 "hovered",
                 /*hovered*/
                 t[4]
-            ), Or(e, "class", "wrap svelte-kzcjhc");
+            ), Dr(e, "class", "wrap svelte-kzcjhc");
         },
         m(_, m) {
             Ki(_, e, m), Kt(e, n), f[i].m(n, null), Kt(e, r), Kt(e, a), Kt(e, l), d && d.m(e, null), u = !0;
         },
         p(_, [m]) {
             let v = i;
-            i = h(_), i !== v && (l_(), oo(f[v], 1, 1, () => {
+            i = h(_), i !== v && (l_(), io(f[v], 1, 1, () => {
                     f[v] = null;
-                }), s_(), o = f[i], o || (o = f[i] = c[i](_), o.c()), io(o, 1), o.m(n, null)), (!u || m & /*hovered*/
+                }), s_(), o = f[i], o || (o = f[i] = c[i](_), o.c()), no(o, 1), o.m(n, null)), (!u || m & /*hovered*/
                     16) && js(
                     n,
                     "hovered",
                     /*hovered*/
                     _[4]
                 ), (!u || m & /*i18n, type*/
                     3) && s !== (s = /*i18n*/
                     _[1](
                         /*defs*/
                         _[5][
                             /*type*/
                             _[0]
                         ] || /*defs*/
                         _[5].file
-                    ) + "") && Nr(a, s), /*mode*/
+                    ) + "") && Or(a, s), /*mode*/
                 _[3] !== "short" ? d ? d.p(_, m) : (d = Fs(_), d.c(), d.m(e, null)) : d && (d.d(1), d = null);
         },
         i(_) {
-            u || (io(o), u = !0);
+            u || (no(o), u = !0);
         },
         o(_) {
-            oo(o), u = !1;
+            io(o), u = !1;
         },
         d(_) {
             _ && Qi(e), f[i].d(), d && d.d();
         }
     };
 }
 
@@ -3460,31 +3460,31 @@
             mode: 3,
             hovered: 4
         });
     }
 }
 const {
     SvelteComponent: m_,
-    append: cr,
+    append: ur,
     attr: vt,
     check_outros: di,
-    create_component: go,
-    destroy_component: bo,
+    create_component: po,
+    destroy_component: go,
     detach: Xn,
     element: Ci,
     empty: p_,
     group_outros: hi,
     init: g_,
     insert: xn,
-    listen: vo,
-    mount_component: wo,
+    listen: bo,
+    mount_component: vo,
     safe_not_equal: b_,
-    space: fr,
+    space: cr,
     toggle_class: jt,
-    transition_in: ye,
+    transition_in: ke,
     transition_out: Ue
 } = window.__gradio__svelte__internal;
 
 function qs(t) {
     let e, n = (
             /*sources*/
             t[1].includes("upload")
@@ -3503,68 +3503,68 @@
         ),
         u, c = n && zs(t),
         f = o && Gs(t),
         h = s && Ws(t),
         d = l && Vs(t);
     return {
         c() {
-            e = Ci("span"), c && c.c(), i = fr(), f && f.c(), r = fr(), h && h.c(), a = fr(), d && d.c(), vt(e, "class", "source-selection svelte-1jp3vgd"), vt(e, "data-testid", "source-select");
+            e = Ci("span"), c && c.c(), i = cr(), f && f.c(), r = cr(), h && h.c(), a = cr(), d && d.c(), vt(e, "class", "source-selection svelte-1jp3vgd"), vt(e, "data-testid", "source-select");
         },
         m(_, m) {
-            xn(_, e, m), c && c.m(e, null), cr(e, i), f && f.m(e, null), cr(e, r), h && h.m(e, null), cr(e, a), d && d.m(e, null), u = !0;
+            xn(_, e, m), c && c.m(e, null), ur(e, i), f && f.m(e, null), ur(e, r), h && h.m(e, null), ur(e, a), d && d.m(e, null), u = !0;
         },
         p(_, m) {
             m & /*sources*/
                 2 && (n = /*sources*/
                     _[1].includes("upload")), n ? c ? (c.p(_, m), m & /*sources*/
-                    2 && ye(c, 1)) : (c = zs(_), c.c(), ye(c, 1), c.m(e, i)) : c && (hi(), Ue(c, 1, 1, () => {
+                    2 && ke(c, 1)) : (c = zs(_), c.c(), ke(c, 1), c.m(e, i)) : c && (hi(), Ue(c, 1, 1, () => {
                     c = null;
                 }), di()), m & /*sources*/
                 2 && (o = /*sources*/
                     _[1].includes("microphone")), o ? f ? (f.p(_, m), m & /*sources*/
-                    2 && ye(f, 1)) : (f = Gs(_), f.c(), ye(f, 1), f.m(e, r)) : f && (hi(), Ue(f, 1, 1, () => {
+                    2 && ke(f, 1)) : (f = Gs(_), f.c(), ke(f, 1), f.m(e, r)) : f && (hi(), Ue(f, 1, 1, () => {
                     f = null;
                 }), di()), m & /*sources*/
                 2 && (s = /*sources*/
                     _[1].includes("webcam")), s ? h ? (h.p(_, m), m & /*sources*/
-                    2 && ye(h, 1)) : (h = Ws(_), h.c(), ye(h, 1), h.m(e, a)) : h && (hi(), Ue(h, 1, 1, () => {
+                    2 && ke(h, 1)) : (h = Ws(_), h.c(), ke(h, 1), h.m(e, a)) : h && (hi(), Ue(h, 1, 1, () => {
                     h = null;
                 }), di()), m & /*sources*/
                 2 && (l = /*sources*/
                     _[1].includes("clipboard")), l ? d ? (d.p(_, m), m & /*sources*/
-                    2 && ye(d, 1)) : (d = Vs(_), d.c(), ye(d, 1), d.m(e, null)) : d && (hi(), Ue(d, 1, 1, () => {
+                    2 && ke(d, 1)) : (d = Vs(_), d.c(), ke(d, 1), d.m(e, null)) : d && (hi(), Ue(d, 1, 1, () => {
                     d = null;
                 }), di());
         },
         i(_) {
-            u || (ye(c), ye(f), ye(h), ye(d), u = !0);
+            u || (ke(c), ke(f), ke(h), ke(d), u = !0);
         },
         o(_) {
             Ue(c), Ue(f), Ue(h), Ue(d), u = !1;
         },
         d(_) {
             _ && Xn(e), c && c.d(), f && f.d(), h && h.d(), d && d.d();
         }
     };
 }
 
 function zs(t) {
     let e, n, i, o, r;
     return n = new Va({}), {
         c() {
-            e = Ci("button"), go(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Upload file"), jt(
+            e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Upload file"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "upload" || ! /*active_source*/
                 t[0]
             );
         },
         m(s, a) {
-            xn(s, e, a), wo(n, e, null), i = !0, o || (r = vo(
+            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler*/
                 t[6]
             ), o = !0);
         },
         p(s, a) {
@@ -3574,38 +3574,38 @@
                 "selected",
                 /*active_source*/
                 s[0] === "upload" || ! /*active_source*/
                 s[0]
             );
         },
         i(s) {
-            i || (ye(n.$$.fragment, s), i = !0);
+            i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), bo(n), o = !1, r();
+            s && Xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Gs(t) {
     let e, n, i, o, r;
     return n = new zd({}), {
         c() {
-            e = Ci("button"), go(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Record audio"), jt(
+            e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Record audio"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "microphone"
             );
         },
         m(s, a) {
-            xn(s, e, a), wo(n, e, null), i = !0, o || (r = vo(
+            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_1*/
                 t[7]
             ), o = !0);
         },
         p(s, a) {
@@ -3614,38 +3614,38 @@
                 e,
                 "selected",
                 /*active_source*/
                 s[0] === "microphone"
             );
         },
         i(s) {
-            i || (ye(n.$$.fragment, s), i = !0);
+            i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), bo(n), o = !1, r();
+            s && Xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Ws(t) {
     let e, n, i, o, r;
     return n = new o_({}), {
         c() {
-            e = Ci("button"), go(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Capture from camera"), jt(
+            e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Capture from camera"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "webcam"
             );
         },
         m(s, a) {
-            xn(s, e, a), wo(n, e, null), i = !0, o || (r = vo(
+            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_2*/
                 t[8]
             ), o = !0);
         },
         p(s, a) {
@@ -3654,38 +3654,38 @@
                 e,
                 "selected",
                 /*active_source*/
                 s[0] === "webcam"
             );
         },
         i(s) {
-            i || (ye(n.$$.fragment, s), i = !0);
+            i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), bo(n), o = !1, r();
+            s && Xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function Vs(t) {
     let e, n, i, o, r;
     return n = new za({}), {
         c() {
-            e = Ci("button"), go(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Paste from clipboard"), jt(
+            e = Ci("button"), po(n.$$.fragment), vt(e, "class", "icon svelte-1jp3vgd"), vt(e, "aria-label", "Paste from clipboard"), jt(
                 e,
                 "selected",
                 /*active_source*/
                 t[0] === "clipboard"
             );
         },
         m(s, a) {
-            xn(s, e, a), wo(n, e, null), i = !0, o || (r = vo(
+            xn(s, e, a), vo(n, e, null), i = !0, o || (r = bo(
                 e,
                 "click",
                 /*click_handler_3*/
                 t[9]
             ), o = !0);
         },
         p(s, a) {
@@ -3694,21 +3694,21 @@
                 e,
                 "selected",
                 /*active_source*/
                 s[0] === "clipboard"
             );
         },
         i(s) {
-            i || (ye(n.$$.fragment, s), i = !0);
+            i || (ke(n.$$.fragment, s), i = !0);
         },
         o(s) {
             Ue(n.$$.fragment, s), i = !1;
         },
         d(s) {
-            s && Xn(e), bo(n), o = !1, r();
+            s && Xn(e), go(n), o = !1, r();
         }
     };
 }
 
 function v_(t) {
     let e, n, i = (
         /*unique_sources*/
@@ -3720,20 +3720,20 @@
         },
         m(o, r) {
             i && i.m(o, r), xn(o, e, r), n = !0;
         },
         p(o, [r]) {
             /*unique_sources*/
             o[2].length > 1 ? i ? (i.p(o, r), r & /*unique_sources*/
-                4 && ye(i, 1)) : (i = qs(o), i.c(), ye(i, 1), i.m(e.parentNode, e)) : i && (hi(), Ue(i, 1, 1, () => {
+                4 && ke(i, 1)) : (i = qs(o), i.c(), ke(i, 1), i.m(e.parentNode, e)) : i && (hi(), Ue(i, 1, 1, () => {
                 i = null;
             }), di());
         },
         i(o) {
-            n || (ye(i), n = !0);
+            n || (ke(i), n = !0);
         },
         o(o) {
             Ue(i), n = !1;
         },
         d(o) {
             o && Xn(e), i && i.d(o);
         }
@@ -3791,15 +3791,15 @@
 const {
     SvelteComponent: k_,
     append: si,
     attr: nt,
     detach: E_,
     init: C_,
     insert: S_,
-    noop: dr,
+    noop: fr,
     safe_not_equal: A_,
     svg_element: Cn
 } = window.__gradio__svelte__internal;
 
 function T_(t) {
     let e, n, i, o, r, s;
     return {
@@ -3807,17 +3807,17 @@
             e = Cn("svg"), n = Cn("g"), i = Cn("g"), o = Cn("path"), r = Cn("path"), s = Cn("polygon"), nt(o, "d", `M348.994,102.946L250.04,3.993c-5.323-5.323-13.954-5.324-19.277,0l-153.7,153.701l118.23,118.23l153.701-153.7\r
 			C354.317,116.902,354.317,108.271,348.994,102.946z`), nt(r, "d", `M52.646,182.11l-41.64,41.64c-5.324,5.322-5.324,13.953,0,19.275l98.954,98.957c5.323,5.322,13.954,5.32,19.277,0\r
 			l41.639-41.641L52.646,182.11z`), nt(s, "points", "150.133,360 341.767,360 341.767,331.949 182.806,331.949"), nt(e, "version", "1.1"), nt(e, "id", "Capa_1"), nt(e, "xmlns", "http://www.w3.org/2000/svg"), nt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), nt(e, "width", "100%"), nt(e, "height", "100%"), nt(e, "viewBox", "0 0 360 360"), nt(e, "color", "#9CA3AF");
         },
         m(a, l) {
             S_(a, e, l), si(e, n), si(n, i), si(i, o), si(i, r), si(i, s);
         },
-        p: dr,
-        i: dr,
-        o: dr,
+        p: fr,
+        i: fr,
+        o: fr,
         d(a) {
             a && E_(e);
         }
     };
 }
 class P_ extends k_ {
     constructor(e) {
@@ -3834,15 +3834,15 @@
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
 AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
 INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
 LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
 OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 PERFORMANCE OF THIS SOFTWARE.
 ***************************************************************************** */
-function Ee(t, e, n, i) {
+function Ce(t, e, n, i) {
     return new(n || (n = Promise))(function(o, r) {
         function s(u) {
             try {
                 l(i.next(u));
             } catch (c) {
                 r(c);
             }
@@ -3892,15 +3892,15 @@
     }
     emit(e, ...n) {
         this.listeners[e] && this.listeners[e].forEach((i) => i(...n));
     }
 };
 const Xs = {
     decode: function(t, e) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             const n = new AudioContext({
                 sampleRate: e
             });
             return n.decodeAudioData(t).finally(() => n.close());
         });
     },
     createBuffer: function(t, e) {
@@ -3948,31 +3948,31 @@
 var L_ = Object.freeze({
     __proto__: null,
     createElement: xs,
     default: xs
 });
 const R_ = {
     fetchBlob: function(t, e, n) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             const i = yield fetch(t, n);
             if (i.status >= 400)
                 throw new Error(`Failed to fetch ${t}: ${i.status} (${i.statusText})`);
             return function(o, r) {
-                Ee(this, void 0, void 0, function*() {
+                Ce(this, void 0, void 0, function*() {
                     if (!o.body || !o.headers)
                         return;
                     const s = o.body.getReader(),
                         a = Number(o.headers.get("Content-Length")) || 0;
                     let l = 0;
-                    const u = (f) => Ee(this, void 0, void 0, function*() {
+                    const u = (f) => Ce(this, void 0, void 0, function*() {
                             l += (f == null ? void 0 : f.length) || 0;
                             const h = Math.round(l / a * 100);
                             r(h);
                         }),
-                        c = () => Ee(this, void 0, void 0, function*() {
+                        c = () => Ce(this, void 0, void 0, function*() {
                             let f;
                             try {
                                 f = yield s.read();
                             } catch {
                                 return;
                             }
                             f.done || (u(f.value), yield c());
@@ -4014,15 +4014,15 @@
     destroy() {
         this.media.pause(), this.isExternalMedia || (this.media.remove(), this.revokeSrc(), this.media.src = "", this.media.load());
     }
     setMediaElement(e) {
         this.media = e;
     }
     play() {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             return this.media.play();
         });
     }
     pause() {
         this.media.pause();
     }
     isPlaying() {
@@ -4061,15 +4061,15 @@
     getMediaElement() {
         return this.media;
     }
     setSinkId(e) {
         return this.media.setSinkId(e);
     }
 }
-class yo extends Si {
+class wo extends Si {
     constructor(e, n) {
         super(), this.timeouts = [], this.isScrollable = !1, this.audioData = null, this.resizeObserver = null, this.lastContainerWidth = 0, this.isDragging = !1, this.subscriptions = [], this.subscriptions = [], this.options = e;
         const i = this.parentFromOptionsContainer(e.container);
         this.parent = i;
         const [o, r] = this.initHtml();
         i.appendChild(o), this.container = o, this.scrollContainer = r.querySelector(".scroll"), this.wrapper = r.querySelector(".wrapper"), this.canvasWrapper = r.querySelector(".canvases"), this.progressWrapper = r.querySelector(".progress"), this.cursor = r.querySelector(".cursor"), n && r.appendChild(n), this.initEvents();
     }
@@ -4115,50 +4115,50 @@
                 return () => {};
             let l, u = !1,
                 c = !1,
                 f = 0,
                 h = 0,
                 d = 0;
             const _ = matchMedia("(pointer: coarse)").matches,
-                m = (C) => {
-                    C.button === s && (C.stopPropagation(), u = !0, c = !1, d = Date.now(), l = e.getBoundingClientRect(), f = C.clientX - l.left, h = C.clientY - l.top);
+                m = (E) => {
+                    E.button === s && (E.stopPropagation(), u = !0, c = !1, d = Date.now(), l = e.getBoundingClientRect(), f = E.clientX - l.left, h = E.clientY - l.top);
                 },
-                v = (C) => {
+                v = (E) => {
                     if (u = !1, d = 0, c) {
-                        C.preventDefault(), C.stopPropagation(), setTimeout(() => {
+                        E.preventDefault(), E.stopPropagation(), setTimeout(() => {
                             c = !1;
                         }, 300);
-                        const y = C.clientX - l.left,
-                            O = C.clientY - l.top;
-                        o == null || o(y, O);
+                        const y = E.clientX - l.left,
+                            H = E.clientY - l.top;
+                        o == null || o(y, H);
                     }
                 },
-                g = (C) => {
+                b = (E) => {
                     if (!u || _ && Date.now() - d < a)
                         return;
-                    C.preventDefault(), C.stopPropagation();
-                    const y = C.clientX - l.left,
-                        O = C.clientY - l.top,
+                    E.preventDefault(), E.stopPropagation();
+                    const y = E.clientX - l.left,
+                        H = E.clientY - l.top,
                         L = y - f,
-                        P = O - h;
-                    (c || Math.abs(L) > r || Math.abs(P) > r) && (c || (i == null || i(f, h), c = !0), n(L, P, y, O), f = y, h = O);
+                        P = H - h;
+                    (c || Math.abs(L) > r || Math.abs(P) > r) && (c || (i == null || i(f, h), c = !0), n(L, P, y, H), f = y, h = H);
                 },
-                S = (C) => {
-                    C.relatedTarget && C.relatedTarget !== document.documentElement || v(C);
+                S = (E) => {
+                    E.relatedTarget && E.relatedTarget !== document.documentElement || v(E);
                 },
-                w = (C) => {
-                    c && C.preventDefault();
+                w = (E) => {
+                    c && E.preventDefault();
                 },
-                k = (C) => {
-                    c && (C.stopPropagation(), C.preventDefault());
+                k = (E) => {
+                    c && (E.stopPropagation(), E.preventDefault());
                 };
-            return e.addEventListener("pointerdown", m), e.addEventListener("click", k, !0), document.addEventListener("click", k, !0), document.addEventListener("pointermove", g), document.addEventListener("touchmove", w, {
+            return e.addEventListener("pointerdown", m), e.addEventListener("click", k, !0), document.addEventListener("click", k, !0), document.addEventListener("pointermove", b), document.addEventListener("touchmove", w, {
                 passive: !1
             }), document.addEventListener("pointerup", v), document.addEventListener("pointerleave", S), document.addEventListener("pointercancel", v), () => {
-                e.removeEventListener("pointerdown", m), e.removeEventListener("click", k, !0), document.removeEventListener("click", k, !0), document.removeEventListener("pointermove", g), document.removeEventListener("touchmove", w), document.removeEventListener("pointerup", v), document.removeEventListener("pointerleave", S), document.removeEventListener("pointercancel", v);
+                e.removeEventListener("pointerdown", m), e.removeEventListener("click", k, !0), document.removeEventListener("click", k, !0), document.removeEventListener("pointermove", b), document.removeEventListener("touchmove", w), document.removeEventListener("pointerup", v), document.removeEventListener("pointerleave", S), document.removeEventListener("pointercancel", v);
             };
         }(this.wrapper, (e, n, i) => {
             this.emit("drag", Math.max(0, Math.min(1, i / this.wrapper.getBoundingClientRect().width)));
         }, (e) => {
             this.isDragging = !0, this.emit("dragstart", Math.max(0, Math.min(1, e / this.wrapper.getBoundingClientRect().width)));
         }, (e) => {
             this.isDragging = !1, this.emit("dragend", Math.max(0, Math.min(1, e / this.wrapper.getBoundingClientRect().width)));
@@ -4310,28 +4310,28 @@
             f = window.devicePixelRatio || 1,
             h = n.barWidth ? n.barWidth * f : 1,
             d = n.barGap ? n.barGap * f : n.barWidth ? h / 2 : 0,
             _ = n.barRadius || 0,
             m = l / (h + d) / a,
             v = _ && "roundRect" in i ? "roundRect" : "rect";
         i.beginPath();
-        let g = 0,
+        let b = 0,
             S = 0,
             w = 0;
         for (let k = 0; k <= a; k++) {
-            const C = Math.round(k * m);
-            if (C > g) {
+            const E = Math.round(k * m);
+            if (E > b) {
                 const L = Math.round(S * c * o),
                     P = L + Math.round(w * c * o) || 1;
                 let M = c - L;
-                n.barAlign === "top" ? M = 0 : n.barAlign === "bottom" && (M = u - P), i[v](g * (h + d), M, h, P, _), g = C, S = 0, w = 0;
+                n.barAlign === "top" ? M = 0 : n.barAlign === "bottom" && (M = u - P), i[v](b * (h + d), M, h, P, _), b = E, S = 0, w = 0;
             }
             const y = Math.abs(r[k] || 0),
-                O = Math.abs(s[k] || 0);
-            y > S && (S = y), O > w && (w = O);
+                H = Math.abs(s[k] || 0);
+            y > S && (S = y), H > w && (w = H);
         }
         i.fill(), i.closePath();
     }
     renderLineWaveform(e, n, i, o) {
         const r = (s) => {
             const a = e[s] || e[0],
                 l = a.length,
@@ -4342,16 +4342,16 @@
                 f = i.canvas.width / l;
             i.moveTo(0, c);
             let h = 0,
                 d = 0;
             for (let _ = 0; _ <= l; _++) {
                 const m = Math.round(_ * f);
                 if (m > h) {
-                    const g = c + (Math.round(d * c * o) || 1) * (s === 0 ? -1 : 1);
-                    i.lineTo(h, g), h = m, d = 0;
+                    const b = c + (Math.round(d * c * o) || 1) * (s === 0 ? -1 : 1);
+                    i.lineTo(h, b), h = m, d = 0;
                 }
                 const v = Math.abs(a[_] || 0);
                 v > d && (d = v);
             }
             i.lineTo(h, c);
         };
         i.beginPath(), r(0), r(1), i.fill(), i.closePath();
@@ -4388,57 +4388,57 @@
             if (a != null && typeof Object.getOwnPropertySymbols == "function") {
                 var f = 0;
                 for (c = Object.getOwnPropertySymbols(a); f < c.length; f++)
                     l.indexOf(c[f]) < 0 && Object.prototype.propertyIsEnumerable.call(a, c[f]) && (u[c[f]] = a[c[f]]);
             }
             return u;
         }(n, ["overlay"]);
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             const a = document.createElement("div"),
                 l = this.getHeight(s.height);
             a.style.height = `${l}px`, r && o > 0 && (a.style.marginTop = `-${l}px`), this.canvasWrapper.style.minHeight = `${l}px`, this.canvasWrapper.appendChild(a);
             const u = a.cloneNode();
             this.progressWrapper.appendChild(u);
             const c = e[0].length,
-                f = (k, C) => {
-                    this.renderSingleCanvas(e, s, i, l, Math.max(0, k), Math.min(C, c), a, u);
+                f = (k, E) => {
+                    this.renderSingleCanvas(e, s, i, l, Math.max(0, k), Math.min(E, c), a, u);
                 };
             if (!this.isScrollable)
                 return void f(0, c);
             const {
                 scrollLeft: h,
                 scrollWidth: d,
                 clientWidth: _
             } = this.scrollContainer, m = c / d;
-            let v = Math.min(yo.MAX_CANVAS_WIDTH, _);
+            let v = Math.min(wo.MAX_CANVAS_WIDTH, _);
             if (s.barWidth || s.barGap) {
                 const k = s.barWidth || 0.5,
-                    C = k + (s.barGap || k / 2);
-                v % C != 0 && (v = Math.floor(v / C) * C);
+                    E = k + (s.barGap || k / 2);
+                v % E != 0 && (v = Math.floor(v / E) * E);
             }
-            const g = Math.floor(Math.abs(h) * m),
-                S = Math.floor(g + v * m),
-                w = S - g;
-            w <= 0 || (f(g, S), yield Promise.all([Ee(this, void 0, void 0, function*() {
-                if (g === 0)
+            const b = Math.floor(Math.abs(h) * m),
+                S = Math.floor(b + v * m),
+                w = S - b;
+            w <= 0 || (f(b, S), yield Promise.all([Ce(this, void 0, void 0, function*() {
+                if (b === 0)
                     return;
                 const k = this.createDelay();
-                for (let C = g; C >= 0; C -= w)
-                    yield k(), f(Math.max(0, C - w), C);
-            }), Ee(this, void 0, void 0, function*() {
+                for (let E = b; E >= 0; E -= w)
+                    yield k(), f(Math.max(0, E - w), E);
+            }), Ce(this, void 0, void 0, function*() {
                 if (S === c)
                     return;
                 const k = this.createDelay();
-                for (let C = S; C < c; C += w)
-                    yield k(), f(C, Math.min(c, C + w));
+                for (let E = S; E < c; E += w)
+                    yield k(), f(E, Math.min(c, E + w));
             })]));
         });
     }
     render(e) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             this.timeouts.forEach((a) => a()), this.timeouts = [], this.canvasWrapper.innerHTML = "", this.progressWrapper.innerHTML = "", this.options.width != null && (this.scrollContainer.style.width = typeof this.options.width == "number" ? `${this.options.width}px` : this.options.width);
             const n = window.devicePixelRatio || 1,
                 i = this.scrollContainer.clientWidth,
                 o = Math.ceil(e.duration * (this.options.minPxPerSec || 0));
             this.isScrollable = o > i;
             const r = this.options.fillParent && !this.isScrollable,
                 s = (r ? i : o) * n;
@@ -4503,15 +4503,15 @@
     renderProgress(e, n) {
         if (isNaN(e))
             return;
         const i = 100 * e;
         this.canvasWrapper.style.clipPath = `polygon(${i}% 0, 100% 0, 100% 100%, ${i}% 100%)`, this.progressWrapper.style.width = `${i}%`, this.cursor.style.left = `${i}%`, this.cursor.style.transform = `translateX(-${Math.round(i) === 100 ? this.options.cursorWidth : 0}px)`, this.isScrollable && this.options.autoScroll && this.scrollIntoView(e, n);
     }
     exportImage(e, n, i) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             const o = this.canvasWrapper.querySelectorAll("canvas");
             if (!o.length)
                 throw new Error("No waveform data");
             if (i === "dataURL") {
                 const r = Array.from(o).map((s) => s.toDataURL(e, n));
                 return Promise.resolve(r);
             }
@@ -4519,15 +4519,15 @@
                 r.toBlob((l) => {
                     l ? s(l) : a(new Error("Could not export image"));
                 }, e, n);
             })));
         });
     }
 }
-yo.MAX_CANVAS_WIDTH = 4e3;
+wo.MAX_CANVAS_WIDTH = 4e3;
 class M_ extends Si {
     constructor() {
         super(...arguments), this.unsubscribe = () => {};
     }
     start() {
         this.unsubscribe = this.on("tick", () => {
             requestAnimationFrame(() => {
@@ -4543,15 +4543,15 @@
     }
 }
 class Zs extends Si {
     constructor(e = new AudioContext()) {
         super(), this.bufferNode = null, this.playStartTime = 0, this.playedDuration = 0, this._muted = !1, this._playbackRate = 1, this._duration = void 0, this.buffer = null, this.currentSrc = "", this.paused = !0, this.crossOrigin = null, this.seeking = !1, this.autoplay = !1, this.addEventListener = this.on, this.removeEventListener = this.un, this.audioContext = e, this.gainNode = this.audioContext.createGain(), this.gainNode.connect(this.audioContext.destination);
     }
     load() {
-        return Ee(this, void 0, void 0, function*() {});
+        return Ce(this, void 0, void 0, function*() {});
     }
     get src() {
         return this.currentSrc;
     }
     set src(e) {
         if (this.currentSrc = e, this._duration = void 0, !e)
             return this.buffer = null, void this.emit("emptied");
@@ -4574,15 +4574,15 @@
         };
     }
     _pause() {
         var e;
         this.paused = !0, (e = this.bufferNode) === null || e === void 0 || e.stop(), this.playedDuration += this.audioContext.currentTime - this.playStartTime;
     }
     play() {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             this.paused && (this._play(), this.emit("play"));
         });
     }
     pause() {
         this.paused || (this._pause(), this.emit("pause"));
     }
     stopAt(e) {
@@ -4591,15 +4591,15 @@
         (n = this.bufferNode) === null || n === void 0 || n.stop(this.audioContext.currentTime + o), (i = this.bufferNode) === null || i === void 0 || i.addEventListener("ended", () => {
             this.bufferNode = null, this.pause();
         }, {
             once: !0
         });
     }
     setSinkId(e) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             return this.audioContext.setSinkId(e);
         });
     }
     get playbackRate() {
         return this._playbackRate;
     }
     set playbackRate(e) {
@@ -4668,15 +4668,15 @@
         super({
             media: n,
             mediaControls: e.mediaControls,
             autoplay: e.autoplay,
             playbackRate: e.audioRate
         }), this.plugins = [], this.decodedData = null, this.subscriptions = [], this.mediaSubscriptions = [], this.abortController = null, this.options = Object.assign({}, D_, e), this.timer = new M_();
         const i = n ? void 0 : this.getMediaElement();
-        this.renderer = new yo(this.options, i), this.initPlayerEvents(), this.initRendererEvents(), this.initTimerEvents(), this.initPlugins(), Promise.resolve().then(() => {
+        this.renderer = new wo(this.options, i), this.initPlayerEvents(), this.initRendererEvents(), this.initTimerEvents(), this.initPlugins(), Promise.resolve().then(() => {
             this.emit("init");
             const o = this.options.url || this.getSrc() || "";
             (o || this.options.peaks && this.options.duration) && this.load(o, this.options.peaks, this.options.duration).catch(() => null);
         });
     }
     updateProgress(e = this.getCurrentTime()) {
         return this.renderer.renderProgress(e / this.getDuration(), this.isPlaying()), e;
@@ -4764,15 +4764,15 @@
         this.renderer.setScrollPercentage(n);
     }
     getActivePlugins() {
         return this.plugins;
     }
     loadAudio(e, n, i, o) {
         var r;
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             if (this.emit("load", e), !this.options.media && this.isPlaying() && this.pause(), this.decodedData = null, !n && !i) {
                 const a = this.options.fetchParams || {};
                 window.AbortController && !a.signal && (this.abortController = new AbortController(), a.signal = (r = this.abortController) === null || r === void 0 ? void 0 : r.signal);
                 const l = (u) => this.emit("loading", u);
                 n = yield R_.fetchBlob(e, l, a);
             }
             this.setSrc(e, n);
@@ -4791,24 +4791,24 @@
                 const a = yield n.arrayBuffer();
                 this.decodedData = yield Xs.decode(a, this.options.sampleRate);
             }
             this.decodedData && (this.emit("decode", this.getDuration()), this.renderer.render(this.decodedData)), this.emit("ready", this.getDuration());
         });
     }
     load(e, n, i) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             try {
                 return yield this.loadAudio(e, void 0, n, i);
             } catch (o) {
                 throw this.emit("error", o), o;
             }
         });
     }
     loadBlob(e, n, i) {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             try {
                 return yield this.loadAudio("blob", e, n, i);
             } catch (o) {
                 throw this.emit("error", o), o;
             }
         });
     }
@@ -4857,15 +4857,15 @@
         super.setTime(e), this.updateProgress(e), this.emit("timeupdate", e);
     }
     seekTo(e) {
         const n = this.getDuration() * e;
         this.setTime(n);
     }
     playPause() {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             return this.isPlaying() ? this.pause() : this.play();
         });
     }
     stop() {
         this.pause(), this.setTime(0);
     }
     skip(e) {
@@ -4876,15 +4876,15 @@
             [0]
         ], 1e-3);
     }
     setMediaElement(e) {
         this.unsubscribePlayerEvents(), super.setMediaElement(e), this.initPlayerEvents();
     }
     exportImage(e = "image/png", n = 1, i = "dataURL") {
-        return Ee(this, void 0, void 0, function*() {
+        return Ce(this, void 0, void 0, function*() {
             return this.renderer.exportImage(e, n, i);
         });
     }
     destroy() {
         var e;
         this.emit("destroy"), (e = this.abortController) === null || e === void 0 || e.abort(), this.plugins.forEach((n) => n.destroy()), this.subscriptions.forEach((n) => n()), this.unsubscribePlayerEvents(), this.timer.destroy(), this.renderer.destroy(), super.destroy();
     }
@@ -4926,15 +4926,15 @@
         unAll() {
             this.listeners = {};
         }
         emit(e, ...n) {
             this.listeners[e] && this.listeners[e].forEach((i) => i(...n));
         }
     },
-    O_ = class extends Ya {
+    H_ = class extends Ya {
         constructor(e) {
             super(), this.subscriptions = [], this.options = e;
         }
         onInit() {}
         _init(e) {
             this.wavesurfer = e, this.onInit();
         }
@@ -4956,42 +4956,42 @@
             k.button === r && (k.stopPropagation(), l = !0, u = !1, h = Date.now(), a = t.getBoundingClientRect(), c = k.clientX - a.left, f = k.clientY - a.top);
         },
         m = (k) => {
             if (l = !1, h = 0, u) {
                 k.preventDefault(), k.stopPropagation(), setTimeout(() => {
                     u = !1;
                 }, 300);
-                const C = k.clientX - a.left,
+                const E = k.clientX - a.left,
                     y = k.clientY - a.top;
-                i == null || i(C, y);
+                i == null || i(E, y);
             }
         },
         v = (k) => {
             if (!l || d && Date.now() - h < s)
                 return;
             k.preventDefault(), k.stopPropagation();
-            const C = k.clientX - a.left,
+            const E = k.clientX - a.left,
                 y = k.clientY - a.top,
-                O = C - c,
+                H = E - c,
                 L = y - f;
-            (u || Math.abs(O) > o || Math.abs(L) > o) && (u || (n == null || n(c, f), u = !0), e(O, L, C, y), c = C, f = y);
+            (u || Math.abs(H) > o || Math.abs(L) > o) && (u || (n == null || n(c, f), u = !0), e(H, L, E, y), c = E, f = y);
         },
-        g = (k) => {
+        b = (k) => {
             k.relatedTarget && k.relatedTarget !== document.documentElement || m(k);
         },
         S = (k) => {
             u && k.preventDefault();
         },
         w = (k) => {
             u && (k.stopPropagation(), k.preventDefault());
         };
     return t.addEventListener("pointerdown", _), t.addEventListener("click", w, !0), document.addEventListener("click", w, !0), document.addEventListener("pointermove", v), document.addEventListener("touchmove", S, {
         passive: !1
-    }), document.addEventListener("pointerup", m), document.addEventListener("pointerleave", g), document.addEventListener("pointercancel", m), () => {
-        t.removeEventListener("pointerdown", _), t.removeEventListener("click", w, !0), document.removeEventListener("click", w, !0), document.removeEventListener("pointermove", v), document.removeEventListener("touchmove", S), document.removeEventListener("pointerup", m), document.removeEventListener("pointerleave", g), document.removeEventListener("pointercancel", m);
+    }), document.addEventListener("pointerup", m), document.addEventListener("pointerleave", b), document.addEventListener("pointercancel", m), () => {
+        t.removeEventListener("pointerdown", _), t.removeEventListener("click", w, !0), document.removeEventListener("click", w, !0), document.removeEventListener("pointermove", v), document.removeEventListener("touchmove", S), document.removeEventListener("pointerup", m), document.removeEventListener("pointerleave", b), document.removeEventListener("pointercancel", m);
     };
 }
 
 function Qa(t, e) {
     const n = e.xmlns ? document.createElementNS(e.xmlns, t) : document.createElement(t);
     for (const [i, o] of Object.entries(e))
         if (i === "children")
@@ -5147,15 +5147,15 @@
                 this.resize = e.resize, this.resize && !o ? this.addResizeHandles(this.element) : this.removeResizeHandles(this.element);
             }
         }
         remove() {
             this.emit("remove"), this.subscriptions.forEach((e) => e()), this.element.remove(), this.element = null;
         }
     },
-    H_ = class Ka extends O_ {
+    O_ = class Ka extends H_ {
         constructor(e) {
             super(e), this.regions = [], this.regionsContainer = this.initRegionsContainer();
         }
         static create(e) {
             return new Ka(e);
         }
         onInit() {
@@ -5281,35 +5281,35 @@
         destroy() {
             this.clearRegions(), super.destroy(), this.regionsContainer.remove();
         }
     };
 const {
     SvelteComponent: N_,
     append: I_,
-    attr: Ot,
+    attr: Ht,
     detach: U_,
     init: j_,
     insert: F_,
-    noop: hr,
+    noop: dr,
     safe_not_equal: q_,
     svg_element: Ys
 } = window.__gradio__svelte__internal;
 
 function z_(t) {
     let e, n;
     return {
         c() {
-            e = Ys("svg"), n = Ys("path"), Ot(n, "d", "m17.545 15.467-3.779-3.779a6.15 6.15 0 0 0 .898-3.21c0-3.417-2.961-6.377-6.378-6.377A6.185 6.185 0 0 0 2.1 8.287c0 3.416 2.961 6.377 6.377 6.377a6.15 6.15 0 0 0 3.115-.844l3.799 3.801a.953.953 0 0 0 1.346 0l.943-.943c.371-.371.236-.84-.135-1.211zM4.004 8.287a4.282 4.282 0 0 1 4.282-4.283c2.366 0 4.474 2.107 4.474 4.474a4.284 4.284 0 0 1-4.283 4.283c-2.366-.001-4.473-2.109-4.473-4.474z"), Ot(e, "version", "1.0"), Ot(e, "xmlns", "http://www.w3.org/2000/svg"), Ot(e, "viewBox", "0 0 20 20"), Ot(e, "id", "magnifier"), Ot(e, "width", "100%"), Ot(e, "height", "100%"), Ot(e, "color", "currentColor");
+            e = Ys("svg"), n = Ys("path"), Ht(n, "d", "m17.545 15.467-3.779-3.779a6.15 6.15 0 0 0 .898-3.21c0-3.417-2.961-6.377-6.378-6.377A6.185 6.185 0 0 0 2.1 8.287c0 3.416 2.961 6.377 6.377 6.377a6.15 6.15 0 0 0 3.115-.844l3.799 3.801a.953.953 0 0 0 1.346 0l.943-.943c.371-.371.236-.84-.135-1.211zM4.004 8.287a4.282 4.282 0 0 1 4.282-4.283c2.366 0 4.474 2.107 4.474 4.474a4.284 4.284 0 0 1-4.283 4.283c-2.366-.001-4.473-2.109-4.473-4.474z"), Ht(e, "version", "1.0"), Ht(e, "xmlns", "http://www.w3.org/2000/svg"), Ht(e, "viewBox", "0 0 20 20"), Ht(e, "id", "magnifier"), Ht(e, "width", "100%"), Ht(e, "height", "100%"), Ht(e, "color", "currentColor");
         },
         m(i, o) {
             F_(i, e, o), I_(e, n);
         },
-        p: hr,
-        i: hr,
-        o: hr,
+        p: dr,
+        i: dr,
+        o: dr,
         d(i) {
             i && U_(e);
         }
     };
 }
 class G_ extends N_ {
     constructor(e) {
@@ -5394,15 +5394,15 @@
             is(e, i);
         }
     };
 }
 
 function t0(t) {
     let e, n;
-    return e = new Hh({}), {
+    return e = new Oh({}), {
         c() {
             ns(e.$$.fragment);
         },
         m(i, o) {
             os(e, i, o), n = !0;
         },
         i(i) {
@@ -5595,15 +5595,15 @@
             waveform: 2
         });
     }
 }
 const {
     SvelteComponent: b0,
     add_flush_callback: el,
-    append: we,
+    append: ye,
     attr: ue,
     bind: tl,
     binding_callbacks: nl,
     check_outros: il,
     create_component: $t,
     destroy_component: en,
     detach: $a,
@@ -5680,15 +5680,15 @@
     );
 }
 
 function ul(t) {
     let e, n, i;
     return {
         c() {
-            e = xe("input"), ue(e, "type", "range"), ue(e, "min", Ur), ue(e, "max", jr), ue(e, "class", "svelte-sgfovr");
+            e = xe("input"), ue(e, "type", "range"), ue(e, "min", Ir), ue(e, "max", Ur), ue(e, "class", "svelte-sgfovr");
         },
         m(o, r) {
             eu(o, e, r), rl(
                 e,
                 /*currentZoom*/
                 t[9]
             ), n || (i = [
@@ -5771,81 +5771,81 @@
         d(i) {
             en(e, i);
         }
     };
 }
 
 function A0(t) {
-    let e, n, i, o, r, s, a, l, u, c, f, h, d, _, m, v, g, S, w, k, C, y, O, L, P, M, x, Z, G, X, E, F, N;
+    let e, n, i, o, r, s, a, l, u, c, f, h, d, _, m, v, b, S, w, k, E, y, H, L, P, M, Z, x, j, X, C, G, I;
     o = new r0({
         props: {
             currentVolume: (
                 /*currentVolume*/
                 t[8]
             )
         }
     });
-    let I = (
+    let U = (
         /*show_volume_slider*/
         t[0] && al(t)
     );
     m = new G_({});
-    let $ = (
+    let K = (
         /*showZoomSlider*/
         t[1] && ul(t)
     );
     k = new Kf({});
-    const H = [S0, C0],
+    const O = [S0, C0],
         J = [];
 
-    function ee(p, T) {
+    function le(p, A) {
         return (
             /*playing*/
             p[5] ? 0 : 1
         );
     }
-    return L = ee(t), P = J[L] = H[L](t), G = new Pd({}), {
+    return L = le(t), P = J[L] = O[L](t), j = new Pd({}), {
         c() {
-            e = xe("div"), n = xe("div"), i = xe("button"), $t(o.$$.fragment), r = Xt(), I && I.c(), s = Xt(), a = xe("button"), l = xe("span"), u = sl(
+            e = xe("div"), n = xe("div"), i = xe("button"), $t(o.$$.fragment), r = Xt(), U && U.c(), s = Xt(), a = xe("button"), l = xe("span"), u = sl(
                 /*playbackSpeed*/
                 t[7]
-            ), c = sl("x"), h = Xt(), d = xe("div"), _ = xe("button"), $t(m.$$.fragment), v = Xt(), $ && $.c(), g = Xt(), S = xe("div"), w = xe("button"), $t(k.$$.fragment), y = Xt(), O = xe("button"), P.c(), x = Xt(), Z = xe("button"), $t(G.$$.fragment), ue(i, "class", "action icon volume svelte-sgfovr"), ue(i, "aria-label", "Adjust volume"), ue(l, "class", "svelte-sgfovr"), ue(a, "class", "playback icon svelte-sgfovr"), ue(a, "aria-label", f = `Adjust playback speed to ${/*playbackSpeeds*/
+            ), c = sl("x"), h = Xt(), d = xe("div"), _ = xe("button"), $t(m.$$.fragment), v = Xt(), K && K.c(), b = Xt(), S = xe("div"), w = xe("button"), $t(k.$$.fragment), y = Xt(), H = xe("button"), P.c(), Z = Xt(), x = xe("button"), $t(j.$$.fragment), ue(i, "class", "action icon volume svelte-sgfovr"), ue(i, "aria-label", "Adjust volume"), ue(l, "class", "svelte-sgfovr"), ue(a, "class", "playback icon svelte-sgfovr"), ue(a, "aria-label", f = `Adjust playback speed to ${/*playbackSpeeds*/
       t[10][
         /*playbackSpeeds*/
         (t[10].indexOf(
           /*playbackSpeed*/
           t[7]
         ) + 1) % /*playbackSpeeds*/
         t[10].length
       ]}x`), ll(
                 a,
                 "hidden",
                 /*show_volume_slider*/
                 t[0]
-            ), ue(_, "class", "zoom-button icon svelte-sgfovr"), ue(d, "class", "zoom-wrapper svelte-sgfovr"), ue(n, "class", "control-wrapper svelte-sgfovr"), ue(w, "class", "rewind icon svelte-sgfovr"), ue(w, "aria-label", C = `Skip backwards by ${Ln(
+            ), ue(_, "class", "zoom-button icon svelte-sgfovr"), ue(d, "class", "zoom-wrapper svelte-sgfovr"), ue(n, "class", "control-wrapper svelte-sgfovr"), ue(w, "class", "rewind icon svelte-sgfovr"), ue(w, "aria-label", E = `Skip backwards by ${Ln(
         /*audio_duration*/
         t[3],
         /*waveform_options*/
         t[6].skip_length
-      )} seconds`), ue(O, "class", "play-pause-button icon svelte-sgfovr"), ue(O, "aria-label", M = /*playing*/
+      )} seconds`), ue(H, "class", "play-pause-button icon svelte-sgfovr"), ue(H, "aria-label", M = /*playing*/
                 t[5] ? (
                     /*i18n*/
                     t[4]("audio.pause")
                 ) : (
                     /*i18n*/
                     t[4]("audio.play")
-                )), ue(Z, "class", "skip icon svelte-sgfovr"), ue(Z, "aria-label", X = "Skip forward by " + Ln(
+                )), ue(x, "class", "skip icon svelte-sgfovr"), ue(x, "aria-label", X = "Skip forward by " + Ln(
                 /*audio_duration*/
                 t[3],
                 /*waveform_options*/
                 t[6].skip_length
             ) + " seconds"), ue(S, "class", "play-pause-wrapper svelte-sgfovr"), ue(e, "class", "controls svelte-sgfovr"), ue(e, "data-testid", "waveform-controls");
         },
-        m(p, T) {
-            eu(p, e, T), we(e, n), we(n, i), tn(o, i, null), we(n, r), I && I.m(n, null), we(n, s), we(n, a), we(a, l), we(l, u), we(l, c), we(n, h), we(n, d), we(d, _), tn(m, _, null), we(d, v), $ && $.m(d, null), we(e, g), we(e, S), we(S, w), tn(k, w, null), we(S, y), we(S, O), J[L].m(O, null), we(S, x), we(S, Z), tn(G, Z, null), E = !0, F || (N = [
+        m(p, A) {
+            eu(p, e, A), ye(e, n), ye(n, i), tn(o, i, null), ye(n, r), U && U.m(n, null), ye(n, s), ye(n, a), ye(a, l), ye(l, u), ye(l, c), ye(n, h), ye(n, d), ye(d, _), tn(m, _, null), ye(d, v), K && K.m(d, null), ye(e, b), ye(e, S), ye(S, w), tn(k, w, null), ye(S, y), ye(S, H), J[L].m(H, null), ye(S, Z), ye(S, x), tn(j, x, null), C = !0, G || (I = [
                 pt(
                     i,
                     "click",
                     /*click_handler*/
                     t[12]
                 ),
                 pt(
@@ -5863,95 +5863,95 @@
                 pt(
                     w,
                     "click",
                     /*click_handler_3*/
                     t[20]
                 ),
                 pt(
-                    O,
+                    H,
                     "click",
                     /*click_handler_4*/
                     t[21]
                 ),
                 pt(
-                    Z,
+                    x,
                     "click",
                     /*click_handler_5*/
                     t[22]
                 )
-            ], F = !0);
+            ], G = !0);
         },
-        p(p, [T]) {
+        p(p, [A]) {
             const q = {};
-            T & /*currentVolume*/
+            A & /*currentVolume*/
                 256 && (q.currentVolume = /*currentVolume*/
                     p[8]), o.$set(q), /*show_volume_slider*/
-                p[0] ? I ? (I.p(p, T), T & /*show_volume_slider*/
-                    1 && Je(I, 1)) : (I = al(p), I.c(), Je(I, 1), I.m(n, s)) : I && (ol(), rt(I, 1, 1, () => {
-                    I = null;
-                }), il()), (!E || T & /*playbackSpeed*/
+                p[0] ? U ? (U.p(p, A), A & /*show_volume_slider*/
+                    1 && Je(U, 1)) : (U = al(p), U.c(), Je(U, 1), U.m(n, s)) : U && (ol(), rt(U, 1, 1, () => {
+                    U = null;
+                }), il()), (!C || A & /*playbackSpeed*/
                     128) && y0(
                     u,
                     /*playbackSpeed*/
                     p[7]
-                ), (!E || T & /*playbackSpeed*/
+                ), (!C || A & /*playbackSpeed*/
                     128 && f !== (f = `Adjust playback speed to ${/*playbackSpeeds*/
       p[10][
         /*playbackSpeeds*/
         (p[10].indexOf(
           /*playbackSpeed*/
           p[7]
         ) + 1) % /*playbackSpeeds*/
         p[10].length
-      ]}x`)) && ue(a, "aria-label", f), (!E || T & /*show_volume_slider*/
+      ]}x`)) && ue(a, "aria-label", f), (!C || A & /*show_volume_slider*/
                     1) && ll(
                     a,
                     "hidden",
                     /*show_volume_slider*/
                     p[0]
                 ), /*showZoomSlider*/
-                p[1] ? $ ? $.p(p, T) : ($ = ul(p), $.c(), $.m(d, null)) : $ && ($.d(1), $ = null), (!E || T & /*audio_duration, waveform_options*/
-                    72 && C !== (C = `Skip backwards by ${Ln(
+                p[1] ? K ? K.p(p, A) : (K = ul(p), K.c(), K.m(d, null)) : K && (K.d(1), K = null), (!C || A & /*audio_duration, waveform_options*/
+                    72 && E !== (E = `Skip backwards by ${Ln(
         /*audio_duration*/
         p[3],
         /*waveform_options*/
         p[6].skip_length
-      )} seconds`)) && ue(w, "aria-label", C);
+      )} seconds`)) && ue(w, "aria-label", E);
             let z = L;
-            L = ee(p), L !== z && (ol(), rt(J[z], 1, 1, () => {
+            L = le(p), L !== z && (ol(), rt(J[z], 1, 1, () => {
                 J[z] = null;
-            }), il(), P = J[L], P || (P = J[L] = H[L](p), P.c()), Je(P, 1), P.m(O, null)), (!E || T & /*playing, i18n*/
+            }), il(), P = J[L], P || (P = J[L] = O[L](p), P.c()), Je(P, 1), P.m(H, null)), (!C || A & /*playing, i18n*/
                 48 && M !== (M = /*playing*/
                     p[5] ? (
                         /*i18n*/
                         p[4]("audio.pause")
                     ) : (
                         /*i18n*/
                         p[4]("audio.play")
-                    ))) && ue(O, "aria-label", M), (!E || T & /*audio_duration, waveform_options*/
+                    ))) && ue(H, "aria-label", M), (!C || A & /*audio_duration, waveform_options*/
                 72 && X !== (X = "Skip forward by " + Ln(
                     /*audio_duration*/
                     p[3],
                     /*waveform_options*/
                     p[6].skip_length
-                ) + " seconds")) && ue(Z, "aria-label", X);
+                ) + " seconds")) && ue(x, "aria-label", X);
         },
         i(p) {
-            E || (Je(o.$$.fragment, p), Je(I), Je(m.$$.fragment, p), Je(k.$$.fragment, p), Je(P), Je(G.$$.fragment, p), E = !0);
+            C || (Je(o.$$.fragment, p), Je(U), Je(m.$$.fragment, p), Je(k.$$.fragment, p), Je(P), Je(j.$$.fragment, p), C = !0);
         },
         o(p) {
-            rt(o.$$.fragment, p), rt(I), rt(m.$$.fragment, p), rt(k.$$.fragment, p), rt(P), rt(G.$$.fragment, p), E = !1;
+            rt(o.$$.fragment, p), rt(U), rt(m.$$.fragment, p), rt(k.$$.fragment, p), rt(P), rt(j.$$.fragment, p), C = !1;
         },
         d(p) {
-            p && $a(e), en(o), I && I.d(), en(m), $ && $.d(), en(k), J[L].d(), en(G), F = !1, tu(N);
+            p && $a(e), en(o), U && U.d(), en(m), K && K.d(), en(k), J[L].d(), en(j), G = !1, tu(I);
         }
     };
 }
-let Ur = 10,
-    jr = 1e4,
+let Ir = 10,
+    Ur = 1e4,
     cl = 100;
 
 function T0(t, e, n) {
     let {
         waveform: i
     } = e, {
         audio_duration: o
@@ -5964,15 +5964,15 @@
     } = e, {
         show_volume_slider: l = !1
     } = e, {
         showZoomSlider: u = !1
     } = e, c = [0.5, 1, 1.5, 2], f = c[1], h = 1, d = 10;
 
     function _(M) {
-        n(9, d = M), d < Ur ? n(9, d = Ur) : d > jr && n(9, d = jr), i.zoom(d);
+        n(9, d = M), d < Ir ? n(9, d = Ir) : d > Ur && n(9, d = Ur), i.zoom(d);
     }
     E0(() => {
         window.addEventListener("keydown", (M) => {
             switch (M.key) {
                 case " ":
                     i.playPause(), M.preventDefault();
                     break;
@@ -5987,28 +5987,28 @@
     });
     const m = () => n(0, l = !l);
 
     function v(M) {
         h = M, n(8, h);
     }
 
-    function g(M) {
+    function b(M) {
         l = M, n(0, l);
     }
     const S = () => {
             n(7, f = c[(c.indexOf(f) + 1) % c.length]), i.setPlaybackRate(f);
         },
         w = () => n(1, u = !u);
 
     function k() {
         d = k0(this.value), n(9, d);
     }
-    const C = (M) => _(M.target.value),
+    const E = (M) => _(M.target.value),
         y = () => n(1, u = !1),
-        O = () => i.skip(Ln(o, a.skip_length) * -1),
+        H = () => i.skip(Ln(o, a.skip_length) * -1),
         L = () => i.playPause(),
         P = () => i.skip(Ln(o, a.skip_length));
     return t.$$set = (M) => {
         "waveform" in M && n(2, i = M.waveform), "audio_duration" in M && n(3, o = M.audio_duration), "i18n" in M && n(4, r = M.i18n), "playing" in M && n(5, s = M.playing), "waveform_options" in M && n(6, a = M.waveform_options), "show_volume_slider" in M && n(0, l = M.show_volume_slider), "showZoomSlider" in M && n(1, u = M.showZoomSlider);
     }, [
         l,
         u,
@@ -6020,21 +6020,21 @@
         f,
         h,
         d,
         c,
         _,
         m,
         v,
-        g,
+        b,
         S,
         w,
         k,
-        C,
+        E,
         y,
-        O,
+        H,
         L,
         P
     ];
 }
 class nu extends b0 {
     constructor(e) {
         super(), v0(this, e, T0, A0, w0, {
@@ -6045,15 +6045,15 @@
             waveform_options: 6,
             show_volume_slider: 0,
             showZoomSlider: 1
         });
     }
 }
 const {
-    setContext: Y2,
+    setContext: Yv,
     getContext: P0
 } = window.__gradio__svelte__internal, L0 = "WORKER_PROXY_CONTEXT_KEY";
 
 function iu() {
     return P0(L0);
 }
 
@@ -6094,32 +6094,32 @@
             type: ou(o.headers, "content-type")
         });
         return URL.createObjectURL(r);
     });
 }
 const {
     SvelteComponent: B0,
-    assign: ro,
+    assign: oo,
     check_outros: su,
     compute_rest_props: dl,
     create_slot: rs,
-    detach: ko,
+    detach: yo,
     element: lu,
     empty: au,
     exclude_internal_props: M0,
     get_all_dirty_from_scope: ss,
     get_slot_changes: ls,
     get_spread_update: uu,
     group_outros: cu,
     init: D0,
-    insert: Eo,
+    insert: ko,
     listen: fu,
-    prevent_default: O0,
-    safe_not_equal: H0,
-    set_attributes: so,
+    prevent_default: H0,
+    safe_not_equal: O0,
+    set_attributes: ro,
     transition_in: cn,
     transition_out: fn,
     update_slot_base: as
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: N0
 } = window.__gradio__svelte__internal;
 
@@ -6152,21 +6152,21 @@
                 )
             },
             /*$$restProps*/
             t[6]
         ],
         u = {};
     for (let c = 0; c < l.length; c += 1)
-        u = ro(u, l[c]);
+        u = oo(u, l[c]);
     return {
         c() {
-            e = lu("a"), a && a.c(), so(e, u);
+            e = lu("a"), a && a.c(), ro(e, u);
         },
         m(c, f) {
-            Eo(c, e, f), a && a.m(e, null), i = !0, o || (r = fu(
+            ko(c, e, f), a && a.m(e, null), i = !0, o || (r = fu(
                 e,
                 "click",
                 /*dispatch*/
                 t[3].bind(null, "click")
             ), o = !0);
         },
         p(c, f) {
@@ -6184,15 +6184,15 @@
                     f,
                     null
                 ) : ss(
                     /*$$scope*/
                     c[7]
                 ),
                 null
-            ), so(e, u = uu(l, [
+            ), ro(e, u = uu(l, [
                 (!i || f & /*href*/
                     1) && {
                     href: (
                         /*href*/
                         c[0]
                     )
                 }, {
@@ -6215,15 +6215,15 @@
         i(c) {
             i || (cn(a, c), i = !0);
         },
         o(c) {
             fn(a, c), i = !1;
         },
         d(c) {
-            c && ko(e), a && a.d(c), o = !1, r();
+            c && yo(e), a && a.d(c), o = !1, r();
         }
     };
 }
 
 function U0(t) {
     let e, n, i, o;
     const r = [F0, j0],
@@ -6236,30 +6236,30 @@
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
             n.c(), i = au();
         },
         m(l, u) {
-            s[e].m(l, u), Eo(l, i, u), o = !0;
+            s[e].m(l, u), ko(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
             e = a(l), e === c ? s[e].p(l, u) : (cu(), fn(s[c], 1, 1, () => {
                 s[c] = null;
             }), su(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), cn(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
             o || (cn(n), o = !0);
         },
         o(l) {
             fn(n), o = !1;
         },
         d(l) {
-            l && ko(i), s[e].d(l);
+            l && yo(i), s[e].d(l);
         }
     };
 }
 
 function j0(t) {
     let e, n, i, o;
     const r = (
@@ -6280,21 +6280,21 @@
                     /*href*/
                     t[0]
                 )
             }
         ],
         l = {};
     for (let u = 0; u < a.length; u += 1)
-        l = ro(l, a[u]);
+        l = oo(l, a[u]);
     return {
         c() {
-            e = lu("a"), s && s.c(), so(e, l);
+            e = lu("a"), s && s.c(), ro(e, l);
         },
         m(u, c) {
-            Eo(u, e, c), s && s.m(e, null), n = !0, i || (o = fu(e, "click", O0(
+            ko(u, e, c), s && s.m(e, null), n = !0, i || (o = fu(e, "click", H0(
                 /*wasm_click_handler*/
                 t[5]
             )), i = !0);
         },
         p(u, c) {
             s && s.p && (!n || c & /*$$scope*/
                 128) && as(
@@ -6310,15 +6310,15 @@
                     c,
                     null
                 ) : ss(
                     /*$$scope*/
                     u[7]
                 ),
                 null
-            ), so(e, l = uu(a, [
+            ), ro(e, l = uu(a, [
                 c & /*$$restProps*/
                 64 && /*$$restProps*/
                 u[6],
                 (!n || c & /*href*/
                     1) && {
                     href: (
                         /*href*/
@@ -6330,15 +6330,15 @@
         i(u) {
             n || (cn(s, u), n = !0);
         },
         o(u) {
             fn(s, u), n = !1;
         },
         d(u) {
-            u && ko(e), s && s.d(u), i = !1, o();
+            u && yo(e), s && s.d(u), i = !1, o();
         }
     };
 }
 
 function F0(t) {
     let e;
     const n = (
@@ -6406,30 +6406,30 @@
                 ))), e ? 0 : 1;
     }
     return n = l(t, -1), i = a[n] = s[n](t), {
         c() {
             i.c(), o = au();
         },
         m(u, c) {
-            a[n].m(u, c), Eo(u, o, c), r = !0;
+            a[n].m(u, c), ko(u, o, c), r = !0;
         },
         p(u, [c]) {
             let f = n;
             n = l(u, c), n === f ? a[n].p(u, c) : (cu(), fn(a[f], 1, 1, () => {
                 a[f] = null;
             }), su(), i = a[n], i ? i.p(u, c) : (i = a[n] = s[n](u), i.c()), cn(i, 1), i.m(o.parentNode, o));
         },
         i(u) {
             r || (cn(i), r = !0);
         },
         o(u) {
             fn(i), r = !1;
         },
         d(u) {
-            u && ko(o), a[n].d(u);
+            u && yo(o), a[n].d(u);
         }
     };
 }
 
 function z0(t, e, n) {
     const i = ["href", "download"];
     let o = dl(e, i),
@@ -6463,70 +6463,70 @@
             if (m.status !== 200)
                 throw new Error(`Failed to get file ${_} from the Wasm worker.`);
             const v = new Blob(
                     [m.body], {
                         type: ou(m.headers, "content-type")
                     }
                 ),
-                g = URL.createObjectURL(v),
+                b = URL.createObjectURL(v),
                 S = document.createElement("a");
-            S.href = g, S.download = l, S.click(), URL.revokeObjectURL(g);
+            S.href = b, S.download = l, S.click(), URL.revokeObjectURL(b);
         }).finally(() => {
             n(2, c = !1);
         });
     }
     return t.$$set = (d) => {
-        e = ro(ro({}, e), M0(d)), n(6, o = dl(e, i)), "href" in d && n(0, a = d.href), "download" in d && n(1, l = d.download), "$$scope" in d && n(7, s = d.$$scope);
+        e = oo(oo({}, e), M0(d)), n(6, o = dl(e, i)), "href" in d && n(0, a = d.href), "download" in d && n(1, l = d.download), "$$scope" in d && n(7, s = d.$$scope);
     }, [
         a,
         l,
         c,
         u,
         f,
         h,
         o,
         s,
         r
     ];
 }
 class du extends B0 {
     constructor(e) {
-        super(), D0(this, e, z0, q0, H0, {
+        super(), D0(this, e, z0, q0, O0, {
             href: 0,
             download: 1
         });
     }
 }
 const {
     SvelteComponent: G0,
     append: hl,
     attr: kt,
     detach: W0,
     init: V0,
     insert: X0,
-    noop: _r,
+    noop: hr,
     safe_not_equal: x0,
-    svg_element: mr
+    svg_element: _r
 } = window.__gradio__svelte__internal;
 
 function Z0(t) {
     let e, n, i;
     return {
         c() {
-            e = mr("svg"), n = mr("g"), i = mr("path"), kt(i, "d", `M41.267,18.557H26.832V4.134C26.832,1.851,24.99,0,22.707,0c-2.283,0-4.124,1.851-4.124,4.135v14.432H4.141\r
+            e = _r("svg"), n = _r("g"), i = _r("path"), kt(i, "d", `M41.267,18.557H26.832V4.134C26.832,1.851,24.99,0,22.707,0c-2.283,0-4.124,1.851-4.124,4.135v14.432H4.141\r
 		c-2.283,0-4.139,1.851-4.138,4.135c-0.001,1.141,0.46,2.187,1.207,2.934c0.748,0.749,1.78,1.222,2.92,1.222h14.453V41.27\r
 		c0,1.142,0.453,2.176,1.201,2.922c0.748,0.748,1.777,1.211,2.919,1.211c2.282,0,4.129-1.851,4.129-4.133V26.857h14.435\r
 		c2.283,0,4.134-1.867,4.133-4.15C45.399,20.425,43.548,18.557,41.267,18.557z`), kt(e, "version", "1.1"), kt(e, "id", "Capa_1"), kt(e, "xmlns", "http://www.w3.org/2000/svg"), kt(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), kt(e, "width", "100%"), kt(e, "height", "100%"), kt(e, "viewBox", "0 10 45.402 45.402	"), kt(e, "xml:space", "preserve");
         },
         m(o, r) {
             X0(o, e, r), hl(e, n), hl(n, i);
         },
-        p: _r,
-        i: _r,
-        o: _r,
+        p: hr,
+        i: hr,
+        o: hr,
         d(o) {
             o && W0(e);
         }
     };
 }
 class J0 extends G0 {
     constructor(e) {
@@ -6559,30 +6559,30 @@
 function dm(t) {
     let e, n, i, o, r, s, a, l, u;
     return s = new J0({}), {
         c() {
             e = xi("div"), n = xi("div"), i = lm(), o = xi("div"), r = xi("button"), K0(s.$$.fragment), Xi(n, "class", "caption svelte-43he0g"), Xi(r, "class", "create-label svelte-43he0g"), Xi(o, "class", "action-buttons svelte-43he0g"), Xi(e, "class", "caption-container svelte-43he0g");
         },
         m(c, f) {
-            nm(c, e, f), Vi(e, n), t[4](n), Vi(e, i), Vi(e, o), Vi(o, r), om(s, r, null), a = !0, l || (u = im(
+            nm(c, e, f), Vi(e, n), t[5](n), Vi(e, i), Vi(e, o), Vi(o, r), om(s, r, null), a = !0, l || (u = im(
                 r,
                 "click",
                 /*click_handler*/
-                t[5]
+                t[6]
             ), l = !0);
         },
         p: rm,
         i(c) {
             a || (am(s.$$.fragment, c), a = !0);
         },
         o(c) {
             um(s.$$.fragment, c), a = !1;
         },
         d(c) {
-            c && em(e), t[4](null), $0(s), l = !1, u();
+            c && em(e), t[5](null), $0(s), l = !1, u();
         }
     };
 }
 
 function hm(t, e, n) {
     let {
         value: i = null
@@ -6591,153 +6591,170 @@
             "rgba(255, 215, 0, 0.5)",
             "rgba(0, 0, 255, 0.5)",
             "rgba(255, 0, 0, 0.5)",
             "rgba(0, 255, 0, 0.5)"
         ],
         u = cm();
 
-    function c(m) {
-        const v = document.createElement("button");
-        v.style.backgroundColor = m.color, v.classList.add("captionLabel"), v.id = m.shortcut, v.innerHTML = '<span style="font-weight: bold;">' + m.shortcut + "</span>: " + m.speaker, v.addEventListener("focusin", () => {
-            h(m.shortcut);
-        }), v.addEventListener("focusout", () => {
-            h("Escape");
-        }), o.appendChild(v);
+    function c(v) {
+        const b = document.createElement("button");
+        b.style.backgroundColor = v.color, b.classList.add("captionLabel"), b.id = v.shortcut, b.innerHTML = '<span style="font-weight: bold;">' + v.shortcut + "</span>: " + v.speaker, b.addEventListener("focusin", () => {
+            d(v.shortcut);
+        }), b.addEventListener("focusout", () => {
+            d("Escape");
+        }), o.appendChild(b);
     }
 
-    function f(m, v, g) {
+    function f(v, b, S) {
         if (r.length === 26)
             return;
-        if (m || (m = "SPEAKER_" + a.toString().padStart(2, "0")), v || (v = l[a % l.length]), !g)
-            for (g = "A"; r.some((w) => w.shortcut === g) && g !== "Z";)
-                g = String.fromCharCode(g.charCodeAt(0) + 1);
-        const S = {
-            speaker: m,
-            color: v,
-            shortcut: g
+        if (v || (v = "SPEAKER_" + a.toString().padStart(2, "0")), b || (b = l[a % l.length]), !S)
+            for (S = "A"; r.some((k) => k.shortcut === S) && S !== "Z";)
+                S = String.fromCharCode(S.charCodeAt(0) + 1);
+        const w = {
+            speaker: v,
+            color: b,
+            shortcut: S
         };
-        return r.push(S), c(S), a++, S;
+        return r.push(w), c(w), a++, w;
     }
 
-    function h(m) {
-        if (s && document.getElementById(s.shortcut).classList.remove("active-button"), m !== "Escape") {
-            let v = r.find((g) => g.shortcut === m.toUpperCase());
-            v || (v = f(void 0, void 0, m.toUpperCase())), s = v, document.getElementById(s.shortcut).classList.add("active-button"), u("select", s);
-        }
+    function h(v) {
+        s && document.getElementById(s.shortcut).classList.remove("active-button"), s = v, document.getElementById(s.shortcut).classList.add("active-button"), u("select", s);
+    }
+
+    function d(v) {
+        let b = null;
+        v !== "Escape" && (b = r.find((S) => S.shortcut === v.toUpperCase()), b || (b = f(void 0, void 0, v.toUpperCase()))), h(b);
     }
     fm(() => {
-        window.addEventListener("keydown", (m) => {
-            (m.key.match(/^[a-zA-Z]$/) || m.key === "Escape") && h(m.key);
+        window.addEventListener("keydown", (v) => {
+            (v.key.match(/^[a-zA-Z]$/) || v.key === "Escape") && d(v.key);
         });
     });
 
-    function d(m) {
-        Q0[m ? "unshift" : "push"](() => {
-            o = m, n(0, o);
+    function _(v) {
+        Q0[v ? "unshift" : "push"](() => {
+            o = v, n(1, o);
         });
     }
-    const _ = () => f();
-    return t.$$set = (m) => {
-        "value" in m && n(2, i = m.value);
+    const m = () => {
+        const v = f();
+        h(v);
+    };
+    return t.$$set = (v) => {
+        "value" in v && n(3, i = v.value);
     }, t.$$.update = () => {
         t.$$.dirty & /*container, value, labels*/
-            13 && o && i && (i.forEach((m) => {
-                r.some((v) => v.speaker === m.speaker) || f(m.speaker, m.color);
-            }), n(3, r = r.sort((m, v) => m.shortcut.localeCompare(v.shortcut))));
-    }, [o, f, i, r, d, _];
+            26 && o && i && (i.forEach((v) => {
+                r.some((b) => b.speaker === v.speaker) || f(v.speaker, v.color);
+            }), n(4, r = r.sort((v, b) => v.shortcut.localeCompare(b.shortcut))));
+    }, [
+        f,
+        o,
+        h,
+        i,
+        r,
+        _,
+        m
+    ];
 }
 class _m extends Y0 {
     constructor(e) {
         super(), tm(this, e, hm, dm, sm, {
-            value: 2
+            value: 3,
+            createLabel: 0
         });
     }
+    get createLabel() {
+        return this.$$.ctx[0];
+    }
 }
 const {
     SvelteComponent: mm,
     add_flush_callback: pm,
     append: Ye,
-    attr: oe,
+    attr: ie,
     bind: gm,
-    binding_callbacks: eo,
-    check_outros: lo,
+    binding_callbacks: mi,
+    check_outros: so,
     create_component: dn,
     destroy_component: hn,
     detach: ut,
     element: je,
     empty: hu,
-    group_outros: ao,
+    group_outros: lo,
     init: bm,
     insert: ct,
-    listen: mi,
+    listen: jr,
     mount_component: _n,
     noop: _l,
     run_all: vm,
     safe_not_equal: wm,
     space: sn,
     src_url_equal: ml,
-    transition_in: ke,
+    transition_in: Ee,
     transition_out: Me
 } = window.__gradio__svelte__internal, {
     onMount: ym
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: km
 } = window.__gradio__svelte__internal;
 
 function Em(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h, d = (
         /*waveform*/
         t[9] && pl(t)
     );
     return {
         c() {
-            e = je("div"), n = je("div"), i = je("div"), o = sn(), r = je("div"), s = je("time"), s.textContent = "0:00", a = sn(), l = je("div"), u = je("time"), u.textContent = "0:00", c = sn(), d && d.c(), oe(i, "id", "waveform"), oe(i, "class", "svelte-hdzdnn"), oe(n, "class", "waveform-container svelte-hdzdnn"), oe(s, "id", "time"), oe(s, "class", "svelte-hdzdnn"), oe(u, "id", "duration"), oe(u, "class", "svelte-hdzdnn"), oe(r, "class", "timestamps svelte-hdzdnn"), oe(e, "class", "component-wrapper svelte-hdzdnn"), oe(e, "data-testid", f = /*label*/
+            e = je("div"), n = je("div"), i = je("div"), o = sn(), r = je("div"), s = je("time"), s.textContent = "0:00", a = sn(), l = je("div"), u = je("time"), u.textContent = "0:00", c = sn(), d && d.c(), ie(i, "id", "waveform"), ie(i, "class", "svelte-1w83umt"), ie(n, "class", "waveform-container svelte-1w83umt"), ie(s, "id", "time"), ie(s, "class", "svelte-1w83umt"), ie(u, "id", "duration"), ie(u, "class", "svelte-1w83umt"), ie(r, "class", "timestamps svelte-1w83umt"), ie(e, "class", "component-wrapper svelte-1w83umt"), ie(e, "data-testid", f = /*label*/
                 t[2] ? "waveform-" + /*label*/
                 t[2] : "unlabelled-audio");
         },
         m(_, m) {
             ct(_, e, m), Ye(e, n), Ye(n, i), t[25](i), Ye(e, o), Ye(e, r), Ye(r, s), t[26](s), Ye(r, a), Ye(r, l), Ye(l, u), t[27](u), Ye(e, c), d && d.m(e, null), h = !0;
         },
         p(_, m) {
             /*waveform*/
             _[9] ? d ? (d.p(_, m), m[0] & /*waveform*/
-                512 && ke(d, 1)) : (d = pl(_), d.c(), ke(d, 1), d.m(e, null)) : d && (ao(), Me(d, 1, 1, () => {
+                512 && Ee(d, 1)) : (d = pl(_), d.c(), Ee(d, 1), d.m(e, null)) : d && (lo(), Me(d, 1, 1, () => {
                 d = null;
-            }), lo()), (!h || m[0] & /*label*/
+            }), so()), (!h || m[0] & /*label*/
                 4 && f !== (f = /*label*/
                     _[2] ? "waveform-" + /*label*/
-                    _[2] : "unlabelled-audio")) && oe(e, "data-testid", f);
+                    _[2] : "unlabelled-audio")) && ie(e, "data-testid", f);
         },
         i(_) {
-            h || (ke(d), h = !0);
+            h || (Ee(d), h = !0);
         },
         o(_) {
             Me(d), h = !1;
         },
         d(_) {
             _ && ut(e), t[25](null), t[26](null), t[27](null), d && d.d();
         }
     };
 }
 
 function Cm(t) {
     let e, n, i;
     return {
         c() {
-            e = je("audio"), oe(e, "class", "standard-player svelte-hdzdnn"), ml(e.src, n = /*value*/
-                    t[0].file_data.url) || oe(e, "src", n), e.controls = !0, e.autoplay = i = /*waveform_settings*/
+            e = je("audio"), ie(e, "class", "standard-player svelte-1w83umt"), ml(e.src, n = /*value*/
+                    t[0].file_data.url) || ie(e, "src", n), e.controls = !0, e.autoplay = i = /*waveform_settings*/
                 t[6].autoplay;
         },
         m(o, r) {
             ct(o, e, r);
         },
         p(o, r) {
             r[0] & /*value*/
                 1 && !ml(e.src, n = /*value*/
-                    o[0].file_data.url) && oe(e, "src", n), r[0] & /*waveform_settings*/
+                    o[0].file_data.url) && ie(e, "src", n), r[0] & /*waveform_settings*/
                 64 && i !== (i = /*waveform_settings*/
                     o[6].autoplay) && (e.autoplay = i);
         },
         i: _l,
         o: _l,
         d(o) {
             o && ut(e);
@@ -6769,31 +6786,30 @@
             o[1] & /*$$scope*/
                 16777216 && (r.$$scope = {
                     dirty: o,
                     ctx: i
                 }), e.$set(r);
         },
         i(i) {
-            n || (ke(e.$$.fragment, i), n = !0);
+            n || (Ee(e.$$.fragment, i), n = !0);
         },
         o(i) {
             Me(e.$$.fragment, i), n = !1;
         },
         d(i) {
             hn(e, i);
         }
     };
 }
 
 function pl(t) {
-    var _;
     let e, n, i, o, r, s, a, l, u;
 
-    function c(m) {
-        t[28](m);
+    function c(_) {
+        t[28](_);
     }
     let f = {
         waveform: (
             /*waveform*/
             t[9]
         ),
         playing: (
@@ -6813,215 +6829,202 @@
             t[7]
         )
     };
     /*show_volume_slider*/
     t[14] !== void 0 && (f.show_volume_slider = /*show_volume_slider*/
         t[14]), i = new nu({
         props: f
-    }), eo.push(() => gm(i, "show_volume_slider", c));
+    }), mi.push(() => gm(i, "show_volume_slider", c));
     let h = (
             /*editable*/
             t[5] && /*interactive*/
             t[4] && /*value*/
-            t[0].annotations && gl(t)
+            t[0] && gl(t)
         ),
         d = (
             /*value*/
-            ((_ = t[0]) == null ? void 0 : _.annotations) && bl(t)
+            t[0] && bl(t)
         );
     return {
         c() {
-            e = je("div"), n = je("div"), dn(i.$$.fragment), r = sn(), s = je("div"), h && h.c(), a = sn(), d && d.c(), l = hu(), oe(n, "class", "waveform-controls svelte-hdzdnn"), oe(s, "class", "regions-actions svelte-hdzdnn"), oe(e, "class", "commands svelte-hdzdnn");
+            e = je("div"), n = je("div"), dn(i.$$.fragment), r = sn(), s = je("div"), h && h.c(), a = sn(), d && d.c(), l = hu(), ie(n, "class", "waveform-controls svelte-1w83umt"), ie(s, "class", "regions-actions svelte-1w83umt"), ie(e, "class", "commands svelte-1w83umt");
         },
-        m(m, v) {
-            ct(m, e, v), Ye(e, n), _n(i, n, null), Ye(e, r), Ye(e, s), h && h.m(s, null), ct(m, a, v), d && d.m(m, v), ct(m, l, v), u = !0;
+        m(_, m) {
+            ct(_, e, m), Ye(e, n), _n(i, n, null), Ye(e, r), Ye(e, s), h && h.m(s, null), ct(_, a, m), d && d.m(_, m), ct(_, l, m), u = !0;
         },
-        p(m, v) {
-            var S;
-            const g = {};
-            v[0] & /*waveform*/
-                512 && (g.waveform = /*waveform*/
-                    m[9]), v[0] & /*playing*/
-                8192 && (g.playing = /*playing*/
-                    m[13]), v[0] & /*audio_duration*/
-                4096 && (g.audio_duration = /*audio_duration*/
-                    m[12]), v[0] & /*i18n*/
-                8 && (g.i18n = /*i18n*/
-                    m[3]), v[0] & /*waveform_options*/
-                128 && (g.waveform_options = /*waveform_options*/
-                    m[7]), !o && v[0] & /*show_volume_slider*/
-                16384 && (o = !0, g.show_volume_slider = /*show_volume_slider*/
-                    m[14], pm(() => o = !1)), i.$set(g), /*editable*/
-                m[5] && /*interactive*/
-                m[4] && /*value*/
-                m[0].annotations ? h ? (h.p(m, v), v[0] & /*editable, interactive, value*/
-                    49 && ke(h, 1)) : (h = gl(m), h.c(), ke(h, 1), h.m(s, null)) : h && (ao(), Me(h, 1, 1, () => {
+        p(_, m) {
+            const v = {};
+            m[0] & /*waveform*/
+                512 && (v.waveform = /*waveform*/
+                    _[9]), m[0] & /*playing*/
+                8192 && (v.playing = /*playing*/
+                    _[13]), m[0] & /*audio_duration*/
+                4096 && (v.audio_duration = /*audio_duration*/
+                    _[12]), m[0] & /*i18n*/
+                8 && (v.i18n = /*i18n*/
+                    _[3]), m[0] & /*waveform_options*/
+                128 && (v.waveform_options = /*waveform_options*/
+                    _[7]), !o && m[0] & /*show_volume_slider*/
+                16384 && (o = !0, v.show_volume_slider = /*show_volume_slider*/
+                    _[14], pm(() => o = !1)), i.$set(v), /*editable*/
+                _[5] && /*interactive*/
+                _[4] && /*value*/
+                _[0] ? h ? (h.p(_, m), m[0] & /*editable, interactive, value*/
+                    49 && Ee(h, 1)) : (h = gl(_), h.c(), Ee(h, 1), h.m(s, null)) : h && (lo(), Me(h, 1, 1, () => {
                     h = null;
-                }), lo()), /*value*/
-                (S = m[0]) != null && S.annotations ? d ? (d.p(m, v), v[0] & /*value*/
-                    1 && ke(d, 1)) : (d = bl(m), d.c(), ke(d, 1), d.m(l.parentNode, l)) : d && (ao(), Me(d, 1, 1, () => {
+                }), so()), /*value*/
+                _[0] ? d ? (d.p(_, m), m[0] & /*value*/
+                    1 && Ee(d, 1)) : (d = bl(_), d.c(), Ee(d, 1), d.m(l.parentNode, l)) : d && (lo(), Me(d, 1, 1, () => {
                     d = null;
-                }), lo());
+                }), so());
         },
-        i(m) {
-            u || (ke(i.$$.fragment, m), ke(h), ke(d), u = !0);
+        i(_) {
+            u || (Ee(i.$$.fragment, _), Ee(h), Ee(d), u = !0);
         },
-        o(m) {
-            Me(i.$$.fragment, m), Me(h), Me(d), u = !1;
+        o(_) {
+            Me(i.$$.fragment, _), Me(h), Me(d), u = !1;
         },
-        d(m) {
-            m && (ut(e), ut(a), ut(l)), hn(i), h && h.d(), d && d.d(m);
+        d(_) {
+            _ && (ut(e), ut(a), ut(l)), hn(i), h && h.d(), d && d.d(_);
         }
     };
 }
 
 function gl(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h = (
         /*showRedo*/
-        t[16] && Am(t)
+        t[17] && Am(t)
     );
     return i = new P_({}), a = new mh({}), {
         c() {
-            h && h.c(), e = sn(), n = je("button"), dn(i.$$.fragment), r = sn(), s = je("button"), dn(a.$$.fragment), oe(n, "class", "action icon remove-button svelte-hdzdnn"), oe(n, "aria-label", "Remove an annotation"), oe(n, "title", o = /*i18n*/
-                t[3]("Remove an annotation")), oe(s, "class", "action icon trim-button svelte-hdzdnn"), oe(s, "aria-label", "Split an annotation"), oe(s, "title", l = /*i18n*/
+            h && h.c(), e = sn(), n = je("button"), dn(i.$$.fragment), r = sn(), s = je("button"), dn(a.$$.fragment), ie(n, "class", "action icon remove-button svelte-1w83umt"), ie(n, "aria-label", "Remove an annotation"), ie(n, "title", o = /*i18n*/
+                t[3]("Remove an annotation")), ie(s, "class", "action icon trim-button svelte-1w83umt"), ie(s, "aria-label", "Split an annotation"), ie(s, "title", l = /*i18n*/
                 t[3]("Split an annotation"));
         },
         m(d, _) {
             h && h.m(d, _), ct(d, e, _), ct(d, n, _), _n(i, n, null), ct(d, r, _), ct(d, s, _), _n(a, s, null), u = !0, c || (f = [
-                mi(
+                jr(
                     n,
-                    "focusin",
-                    /*focusin_handler*/
+                    "click",
+                    /*click_handler*/
                     t[29]
                 ),
-                mi(
-                    n,
-                    "focusout",
-                    /*focusout_handler*/
-                    t[30]
-                ),
-                mi(
-                    s,
-                    "focusin",
-                    /*focusin_handler_1*/
-                    t[31]
-                ),
-                mi(
+                jr(
                     s,
-                    "focusout",
-                    /*focusout_handler_1*/
-                    t[32]
+                    "click",
+                    /*click_handler_1*/
+                    t[30]
                 )
             ], c = !0);
         },
         p(d, _) {
             /*showRedo*/
-            d[16] && h.p(d, _), (!u || _[0] & /*i18n*/
+            d[17] && h.p(d, _), (!u || _[0] & /*i18n*/
                 8 && o !== (o = /*i18n*/
-                    d[3]("Remove an annotation"))) && oe(n, "title", o), (!u || _[0] & /*i18n*/
+                    d[3]("Remove an annotation"))) && ie(n, "title", o), (!u || _[0] & /*i18n*/
                 8 && l !== (l = /*i18n*/
-                    d[3]("Split an annotation"))) && oe(s, "title", l);
+                    d[3]("Split an annotation"))) && ie(s, "title", l);
         },
         i(d) {
-            u || (ke(h), ke(i.$$.fragment, d), ke(a.$$.fragment, d), u = !0);
+            u || (Ee(h), Ee(i.$$.fragment, d), Ee(a.$$.fragment, d), u = !0);
         },
         o(d) {
             Me(h), Me(i.$$.fragment, d), Me(a.$$.fragment, d), u = !1;
         },
         d(d) {
             d && (ut(e), ut(n), ut(r), ut(s)), h && h.d(d), hn(i), hn(a), c = !1, vm(f);
         }
     };
 }
 
 function Am(t) {
     let e, n, i, o, r, s;
     return n = new Wa({}), {
         c() {
-            e = je("button"), dn(n.$$.fragment), oe(e, "class", "action icon svelte-hdzdnn"), oe(e, "aria-label", "Reset annotations"), oe(e, "title", i = /*i18n*/
+            e = je("button"), dn(n.$$.fragment), ie(e, "class", "action icon svelte-1w83umt"), ie(e, "aria-label", "Reset annotations"), ie(e, "title", i = /*i18n*/
                 t[3]("Reset annotations"));
         },
         m(a, l) {
-            ct(a, e, l), _n(n, e, null), o = !0, r || (s = mi(
+            ct(a, e, l), _n(n, e, null), o = !0, r || (s = jr(
                 e,
                 "click",
                 /*resetRegions*/
-                t[17]
+                t[18]
             ), r = !0);
         },
         p(a, l) {
             (!o || l[0] & /*i18n*/
                 8 && i !== (i = /*i18n*/
-                    a[3]("Reset annotations"))) && oe(e, "title", i);
+                    a[3]("Reset annotations"))) && ie(e, "title", i);
         },
         i(a) {
-            o || (ke(n.$$.fragment, a), o = !0);
+            o || (Ee(n.$$.fragment, a), o = !0);
         },
         o(a) {
             Me(n.$$.fragment, a), o = !1;
         },
         d(a) {
             a && ut(e), hn(n), r = !1, s();
         }
     };
 }
 
 function bl(t) {
-    let e, n;
+    let e, n, i = {
+        value: (
+            /*value*/
+            t[0].annotations
+        )
+    };
     return e = new _m({
-        props: {
-            value: (
-                /*value*/
-                t[0].annotations
-            )
-        }
-    }), e.$on(
+        props: i
+    }), t[31](e), e.$on(
         "select",
         /*select_handler*/
-        t[33]
+        t[32]
     ), e.$on(
         "select",
         /*select_handler_1*/
-        t[34]
+        t[33]
     ), {
         c() {
             dn(e.$$.fragment);
         },
-        m(i, o) {
-            _n(e, i, o), n = !0;
+        m(o, r) {
+            _n(e, o, r), n = !0;
         },
-        p(i, o) {
-            const r = {};
-            o[0] & /*value*/
-                1 && (r.value = /*value*/
-                    i[0].annotations), e.$set(r);
+        p(o, r) {
+            const s = {};
+            r[0] & /*value*/
+                1 && (s.value = /*value*/
+                    o[0].annotations), e.$set(s);
         },
-        i(i) {
-            n || (ke(e.$$.fragment, i), n = !0);
+        i(o) {
+            n || (Ee(e.$$.fragment, o), n = !0);
         },
-        o(i) {
-            Me(e.$$.fragment, i), n = !1;
+        o(o) {
+            Me(e.$$.fragment, o), n = !1;
         },
-        d(i) {
-            hn(e, i);
+        d(o) {
+            t[31](null), hn(e, o);
         }
     };
 }
 
 function Tm(t) {
     let e, n;
-    return e = new po({}), {
+    return e = new mo({}), {
         c() {
             dn(e.$$.fragment);
         },
         m(i, o) {
             _n(e, i, o), n = !0;
         },
         i(i) {
-            n || (ke(e.$$.fragment, i), n = !0);
+            n || (Ee(e.$$.fragment, i), n = !0);
         },
         o(i) {
             Me(e.$$.fragment, i), n = !1;
         },
         d(i) {
             hn(e, i);
         }
@@ -7047,31 +7050,31 @@
             n.c(), i = hu();
         },
         m(l, u) {
             s[e].m(l, u), ct(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
-            e = a(l), e === c ? s[e].p(l, u) : (ao(), Me(s[c], 1, 1, () => {
+            e = a(l), e === c ? s[e].p(l, u) : (lo(), Me(s[c], 1, 1, () => {
                 s[c] = null;
-            }), lo(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), ke(n, 1), n.m(i.parentNode, i));
+            }), so(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Ee(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
-            o || (ke(n), o = !0);
+            o || (Ee(n), o = !0);
         },
         o(l) {
             Me(n), o = !1;
         },
         d(l) {
             l && ut(i), s[e].d(l);
         }
     };
 }
 
-function he(t) {
+function pe(t) {
     let e, n = t[0],
         i = 1;
     for (; i < t.length;) {
         const o = t[i],
             r = t[i + 1];
         if (i += 2, (o === "optionalAccess" || o === "optionalCall") && n == null)
             return;
@@ -7108,415 +7111,420 @@
         {
             waveform_options: c
         } = e,
         {
             mode: f = ""
         } = e,
         h, d, _, m = null,
-        v, g, S, w, k, C = !1,
+        v, b, S, w, k, E = !1,
         y = !1,
-        O = a,
+        H = a,
         L = null,
         P = /* @__PURE__ */ new Map(),
-        M = null,
+        M, Z = null,
         x = null;
-    const Z = km();
+    const j = km();
 
-    function G() {
+    function X() {
         n(9, d = Ft.create({
             container: h,
             ...u
-        })), fl(he([o, "access", (b) => b.file_data, "optionalAccess", (b) => b.url])).then((b) => {
-            if (b && d)
-                return d.load(b);
+        })), fl(pe([o, "access", (g) => g.file_data, "optionalAccess", (g) => g.url])).then((g) => {
+            if (g && d)
+                return d.load(g);
         }), d.on("dblclick", () => {
-            he([o, "optionalAccess", (b) => b.annotations]) && N(d.getCurrentTime());
+            U(d.getCurrentTime());
         });
     }
 
-    function X() {
-        let b = o.annotations;
-        if (L === null) {
-            if (n(23, L = []), b.length === 0)
-                return;
-            M = {
-                speaker: b[0].speaker,
-                color: b[0].color,
-                shortcut: "A"
-            }, b.forEach((A) => L.push(Object.assign({}, A)));
-        }
-        o.annotations.forEach((A) => {
-            let D = F({
-                    start: A.start,
-                    end: A.end,
-                    color: A.color,
+    function C(g) {
+        if (L || (L = [...g]), g.length === 0)
+            return;
+        Z = {
+            speaker: g[0].speaker,
+            color: g[0].color,
+            shortcut: "A"
+        };
+        const T = Array.from(P.values());
+        g = g.filter((D) => !T.some((N) => D.start === N.start && D.end === N.end && D.speaker === N.speaker)), g.forEach((D) => {
+            let N = I({
+                    start: D.start,
+                    end: D.end,
+                    color: D.color,
                     drag: !0,
                     resize: !0
                 },
-                A.speaker
+                D.speaker
             );
-            D.element.style.top = (A.level * 10).toString() + "%", D.element.style.height = (100 - (A.numLevels + 1) * 10).toString() + "%";
+            N.element.style.top = (D.level * 10).toString() + "%", N.element.style.height = (100 - (D.numLevels + 1) * 10).toString() + "%";
         });
     }
 
-    function E() {
-        n(0, o.annotations = Array.from(P.values()), o), Z("edit", o);
+    function G() {
+        n(0, o.annotations = Array.from(P.values()), o), j("edit", o);
     }
 
-    function F(b, A) {
-        let D = _.addRegion(b);
-        return P.set(D.id, {
+    function I(g, T) {
+        let D = _.addRegion(g);
+        const N = {
             start: D.start,
             end: D.end,
-            speaker: A,
+            speaker: T,
             color: D.color
-        }), E(), D;
+        };
+        return P.set(D.id, N), L || (L = [N]), G(), D;
     }
 
-    function N(b) {
-        let A = x !== null ? x : M;
-        if (A === null)
+    function U(g) {
+        let T = x !== null ? x : Z;
+        if (T === null) {
+            window.alert('First create a label by clicking on "+" or by pressing A-Z');
             return;
-        let D = F({
-                start: b - 1,
-                end: b + 1,
-                color: A.color,
+        }
+        let D = I({
+                start: g - 1,
+                end: g + 1,
+                color: T.color,
                 drag: !0,
                 resize: !0
             },
-            A.speaker
+            T.speaker
         );
-        ee(D);
+        p(D);
     }
 
-    function I(b) {
-        b === m && ee(null), P.delete(b.id), b.remove(), E();
+    function K(g) {
+        g === m && p(null), P.delete(g.id), g.remove(), G();
     }
 
-    function $(b, A) {
+    function O(g, T) {
         if (!m)
             return;
-        let D = _.getRegions().find((j) => j.id === m.id);
-        b === "Delete" || b == "Backspace" && A ? T(!1) : T(!0), I(D);
+        let D = _.getRegions().find((N) => N.id === m.id);
+        g === "Delete" || g == "Backspace" && T ? q(!1) : q(!0), K(D);
     }
 
-    function H() {
-        J(), L.forEach((b) => o.annotations.push(Object.assign({}, b))), X(), Z("edit", o);
+    function J() {
+        le(), L.forEach((g) => o.annotations.push(Object.assign({}, g))), C(o.annotations), j("edit", o);
     }
 
-    function J() {
-        ee(null), he([_, "optionalAccess", (b) => b.clearRegions, "call", (b) => b()]), n(0, o.annotations = [], o), P.clear();
+    function le() {
+        p(null), pe([_, "optionalAccess", (g) => g.clearRegions, "call", (g) => g()]), n(0, o.annotations = [], o), P.clear();
     }
 
-    function ee(b) {
-        if (m !== null && n(20, m.element.style.background = m.color, m), b === null) {
-            n(20, m = b);
+    function p(g) {
+        if (m !== null && n(21, m.element.style.background = m.color, m), g === null) {
+            n(21, m = g);
             return;
         }
-        n(20, m = b), n(20, m.element.style.background = "repeating-linear-gradient(45deg," + b.color + " ," + b.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
+        n(21, m = g), n(21, m.element.style.background = "repeating-linear-gradient(45deg," + g.color + " ," + g.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
     }
 
-    function p(b) {
+    function A(g) {
         if (m !== null) {
             m.setOptions({
                 start: m.start,
                 end: m.end,
-                color: b.color,
+                color: g.color,
                 drag: !0,
                 resize: !0
-            }), n(20, m.element.style.background = "repeating-linear-gradient(45deg," + m.color + " ," + m.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
-            let A = P.get(m.id);
-            A.color = b.color, A.speaker = b.speaker, E();
+            }), n(21, m.element.style.background = "repeating-linear-gradient(45deg," + m.color + " ," + m.color + " 10px, #ffffff 10px ,#ffffff 15px)", m);
+            let T = P.get(m.id);
+            T.color = g.color, T.speaker = g.speaker, G();
         }
     }
 
-    function T(b) {
-        var A = b ? -1 : 1,
-            D = _.getRegions().sort((ne, re) => ne.start > re.start ? 1 : -1);
+    function q(g) {
+        var T = g ? -1 : 1,
+            D = _.getRegions().sort((te, oe) => te.start > oe.start ? 1 : -1);
         if (m === null)
-            ee(D[0]);
+            p(D[0]);
         else {
-            var j = D.indexOf(m);
-            ee(D.at((j + A) % D.length));
+            var N = D.indexOf(m);
+            p(D.at((N + T) % D.length));
         }
     }
 
-    function q(b, A) {
-        if (A < b.start || A > b.end)
+    function z(g, T) {
+        if (T < g.start || T > g.end)
             throw new RangeError("split time out of region bounds");
-        let D = P.get(b.id).speaker;
-        F({
-                start: b.start,
-                end: A,
-                color: b.color,
-                drag: b.drag,
-                resize: b.resize
+        let D = P.get(g.id).speaker;
+        I({
+                start: g.start,
+                end: T,
+                color: g.color,
+                drag: g.drag,
+                resize: g.resize
             },
             D
         );
-        let j = F({
-                start: A,
-                end: b.end,
-                color: b.color,
-                drag: b.drag,
-                resize: b.resize
+        let N = I({
+                start: T,
+                end: g.end,
+                color: g.color,
+                drag: g.drag,
+                resize: g.resize
             },
             D
         );
-        ee(j), I(b);
+        p(N), K(g);
     }
 
-    function z(b) {
-        let A = _.getRegions().find((D) => D.start < b && D.end > b);
-        if (A === void 0) {
+    function he(g) {
+        let T = _.getRegions().find((D) => D.start < g && D.end > g);
+        if (T === void 0) {
             if (m === null)
                 return;
-            A = m, b = A.start + (A.end - A.start) / 2;
+            T = m, g = T.start + (T.end - T.start) / 2;
         }
-        q(A, b);
+        z(T, g);
     }
 
-    function _e(b, A, D) {
-        let j, ne, re = 0.05;
-        A && (re = re * 4), D ? b === "ArrowLeft" ? (j = m.start, ne = m.end - re) : (j = m.start, ne = m.end + re) : b === "ArrowLeft" ? (j = m.start - re, ne = m.end) : (j = m.start + re, ne = m.end), j > m.end && (j = m.end - 0.1), ne < m.start && (ne = m.start + 0.1), m.setOptions({
-            start: j,
-            end: ne
+    function _e(g, T, D) {
+        let N, te, oe = 0.05;
+        T && (oe = oe * 4), D ? g === "ArrowLeft" ? (N = m.start, te = m.end - oe) : (N = m.start, te = m.end + oe) : g === "ArrowLeft" ? (N = m.start - oe, te = m.end) : (N = m.start + oe, te = m.end), N > m.end && (N = m.end - 0.1), te < m.start && (te = m.start + 0.1), m.setOptions({
+            start: N,
+            end: te
         });
     }
 
-    function me(b, A) {
+    function F(g, T) {
         let D = d.getCurrentTime(),
-            j, ne = 0.05;
-        A && (ne = ne * 4), b === "ArrowLeft" ? j = D - ne : j = D + ne, d.setTime(j);
+            N, te = 0.05;
+        T && (te = te * 4), g === "ArrowLeft" ? N = D - te : N = D + te, d.setTime(N);
     }
 
-    function U(b, A, D) {
+    function ve(g, T, D) {
         if (m) {
-            _e(b, A, D);
+            _e(g, T, D);
             return;
         }
-        me(b, A);
+        F(g, T);
     }
-    async function Ce(b) {
-        await fl(b).then((A) => {
-            if (!(!A || he([
+    async function B(g) {
+        await fl(g).then((T) => {
+            if (!(!T || pe([
                     o,
                     "access",
                     (D) => D.file_data,
                     "optionalAccess",
                     (D) => D.is_stream
                 ])))
-                return he([
+                return pe([
                     d,
                     "optionalAccess",
                     (D) => D.load,
                     "call",
-                    (D) => D(A)
+                    (D) => D(T)
                 ]);
         });
     }
     ym(() => {
-        window.addEventListener("keydown", (b) => {
-            switch (b.key) {
+        window.addEventListener("keydown", (g) => {
+            switch (g.key) {
                 case "ArrowLeft":
-                    U("ArrowLeft", b.shiftKey, b.altKey);
+                    ve("ArrowLeft", g.shiftKey, g.altKey);
                     break;
                 case "ArrowRight":
-                    U("ArrowRight", b.shiftKey, b.altKey);
+                    ve("ArrowRight", g.shiftKey, g.altKey);
                     break;
                 case "Escape":
-                    ee(null);
+                    p(null);
                     break;
                 case "Tab":
-                    b.preventDefault(), T(b.shiftKey);
+                    g.preventDefault(), q(g.shiftKey);
                     break;
                 case "Delete":
-                    $("Delete", b.shiftKey);
+                    O("Delete", g.shiftKey);
                     break;
                 case "Backspace":
-                    $("Backspace", b.shiftKey);
+                    O("Backspace", g.shiftKey);
                     break;
                 case "Enter":
-                    b.preventDefault(), b.shiftKey ? z(d.getCurrentTime()) : N(d.getCurrentTime());
+                    g.preventDefault(), g.shiftKey ? he(d.getCurrentTime()) : U(d.getCurrentTime());
                     break;
             }
         });
     });
 
-    function B(b) {
-        eo[b ? "unshift" : "push"](() => {
-            h = b, n(8, h), n(9, d);
+    function R(g) {
+        mi[g ? "unshift" : "push"](() => {
+            h = g, n(8, h), n(9, d);
         });
     }
 
-    function R(b) {
-        eo[b ? "unshift" : "push"](() => {
-            S = b, n(10, S), n(9, d);
+    function ce(g) {
+        mi[g ? "unshift" : "push"](() => {
+            S = g, n(10, S), n(9, d);
         });
     }
 
-    function ce(b) {
-        eo[b ? "unshift" : "push"](() => {
-            w = b, n(11, w), n(9, d);
+    function Se(g) {
+        mi[g ? "unshift" : "push"](() => {
+            w = g, n(11, w), n(9, d);
         });
     }
 
-    function Se(b) {
-        y = b, n(14, y);
+    function wt(g) {
+        y = g, n(14, y);
     }
-    const wt = () => n(1, f = "remove"),
-        Y = () => n(1, f = ""),
-        yt = () => n(1, f = "split"),
-        wn = () => n(1, f = ""),
-        ei = (b) => p(b.detail),
-        ti = (b) => n(15, x = b.detail);
-    return t.$$set = (b) => {
-        "value" in b && n(0, o = b.value), "label" in b && n(2, r = b.label), "i18n" in b && n(3, s = b.i18n), "interactive" in b && n(4, a = b.interactive), "editable" in b && n(5, l = b.editable), "waveform_settings" in b && n(6, u = b.waveform_settings), "waveform_options" in b && n(7, c = b.waveform_options), "mode" in b && n(1, f = b.mode);
+    const Y = () => n(1, f = "remove"),
+        yt = () => n(1, f = "split");
+
+    function wn(g) {
+        mi[g ? "unshift" : "push"](() => {
+            M = g, n(15, M);
+        });
+    }
+    const ei = (g) => A(g.detail),
+        ti = (g) => n(16, x = g.detail);
+    return t.$$set = (g) => {
+        "value" in g && n(0, o = g.value), "label" in g && n(2, r = g.label), "i18n" in g && n(3, s = g.i18n), "interactive" in g && n(4, a = g.interactive), "editable" in g && n(5, l = g.editable), "waveform_settings" in g && n(6, u = g.waveform_settings), "waveform_options" in g && n(7, c = g.waveform_options), "mode" in g && n(1, f = g.mode);
     }, t.$$.update = () => {
         if (t.$$.dirty[0] & /*value*/
-            1 && n(24, i = he([o, "access", (b) => b.file_data, "optionalAccess", (b) => b.url])), t.$$.dirty[0] & /*container, waveform*/
-            768 && h !== void 0 && (d !== void 0 && d.destroy(), n(8, h.innerHTML = "", h), G(), n(13, C = !1)), t.$$.dirty[0] & /*waveform, wsRegions, waveform_settings*/
-            524864 && he([
+            1 && n(24, i = pe([o, "access", (g) => g.file_data, "optionalAccess", (g) => g.url])), t.$$.dirty[0] & /*container, waveform*/
+            768 && h !== void 0 && (d !== void 0 && d.destroy(), n(8, h.innerHTML = "", h), X(), n(13, E = !1)), t.$$.dirty[0] & /*waveform, wsRegions, waveform_settings*/
+            1049152 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("ready", () => {
-                    _ === void 0 && n(19, _ = d.registerPlugin(H_.create())), u.autoplay ? he([d, "optionalAccess", (A) => A.play, "call", (A) => A()]) : he([d, "optionalAccess", (A) => A.stop, "call", (A) => A()]);
+                (g) => g("ready", () => {
+                    _ === void 0 && n(20, _ = d.registerPlugin(O_.create())), u.autoplay ? pe([d, "optionalAccess", (T) => T.play, "call", (T) => T()]) : pe([d, "optionalAccess", (T) => T.stop, "call", (T) => T()]);
                 })
-            ]), t.$$.dirty[0] & /*value, wsRegions, initialAnnotations*/
-            8912897 && he([o, "optionalAccess", (b) => b.annotations]) !== null && _ && L === null && X(), t.$$.dirty[0] & /*waveform, durationRef*/
-            2560 && he([
+            ]), t.$$.dirty[0] & /*value, wsRegions*/
+            1048577 && pe([o, "optionalAccess", (g) => g.annotations]) !== null && _ && C(o.annotations), t.$$.dirty[0] & /*waveform, durationRef*/
+            2560 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("decode", (A) => {
-                    n(12, k = A), w && n(11, w.textContent = vl(A), w);
+                (g) => g("decode", (T) => {
+                    n(12, k = T), w && n(11, w.textContent = vl(T), w);
                 })
             ]), t.$$.dirty[0] & /*waveform, timeRef*/
-            1536 && he([
+            1536 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("timeupdate", (A) => S && n(10, S.textContent = vl(A), S))
+                (g) => g("timeupdate", (T) => S && n(10, S.textContent = vl(T), S))
             ]), t.$$.dirty[0] & /*waveform*/
-            512 && he([
+            512 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("finish", () => {
-                    n(13, C = !1), Z("stop");
+                (g) => g("finish", () => {
+                    n(13, E = !1), j("stop");
                 })
             ]), t.$$.dirty[0] & /*waveform*/
-            512 && he([
+            512 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("pause", () => {
-                    n(13, C = !1), Z("pause");
+                (g) => g("pause", () => {
+                    n(13, E = !1), j("pause");
                 })
             ]), t.$$.dirty[0] & /*waveform*/
-            512 && he([
+            512 && pe([
                 d,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("play", () => {
-                    n(13, C = !0), Z("play");
+                (g) => g("play", () => {
+                    n(13, E = !0), j("play");
                 })
             ]), t.$$.dirty[0] & /*wsRegions*/
-            524288 && he([
+            1048576 && pe([
                 _,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("region-updated", (A) => {
-                    var D = P.get(A.id);
-                    D.start = A.start, D.end = A.end, E();
+                (g) => g("region-updated", (T) => {
+                    var D = P.get(T.id);
+                    D.start = T.start, D.end = T.end, G();
                 })
             ]), t.$$.dirty[0] & /*wsRegions, mode*/
-            524290 && he([
+            1048578 && pe([
                 _,
                 "optionalAccess",
-                (b) => b.on,
+                (g) => g.on,
                 "call",
-                (b) => b("region-clicked", (A, D) => {
+                (g) => g("region-clicked", (T, D) => {
                     switch (f) {
                         case "remove":
-                            I(A);
+                            K(T);
                             break;
                         case "split":
-                            q(A, A.start + (A.end - A.start) / 2);
+                            z(T, T.start + (T.end - T.start) / 2);
                             break;
                         default:
-                            ee(A), A.play();
+                            p(T), T.play();
                     }
+                    n(1, f = "");
                 })
             ]), t.$$.dirty[0] & /*activeRegion, container, leftRegionHandle, rightRegionHandle, wsRegions*/
-            7864576 && m) {
-            const b = h.children[0].shadowRoot;
-            n(22, g = b.querySelector('[data-resize="right"]')), n(21, v = b.querySelector('[data-resize="left"]')), v && g && (v.setAttribute("role", "button"), g.setAttribute("role", "button"), he([
+            15728896 && m) {
+            const g = h.children[0].shadowRoot;
+            n(23, b = g.querySelector('[data-resize="right"]')), n(22, v = g.querySelector('[data-resize="left"]')), v && b && (v.setAttribute("role", "button"), b.setAttribute("role", "button"), pe([
                 v,
                 "optionalAccess",
-                (A) => A.setAttribute,
+                (T) => T.setAttribute,
                 "call",
-                (A) => A("aria-label", "Drag to adjust start time")
-            ]), he([
-                g,
+                (T) => T("aria-label", "Drag to adjust start time")
+            ]), pe([
+                b,
                 "optionalAccess",
-                (A) => A.setAttribute,
+                (T) => T.setAttribute,
                 "call",
-                (A) => A("aria-label", "Drag to adjust end time")
-            ]), he([
+                (T) => T("aria-label", "Drag to adjust end time")
+            ]), pe([
                 v,
                 "optionalAccess",
-                (A) => A.setAttribute,
+                (T) => T.setAttribute,
                 "call",
-                (A) => A("tabindex", "0")
-            ]), he([
-                g,
+                (T) => T("tabindex", "0")
+            ]), pe([
+                b,
                 "optionalAccess",
-                (A) => A.setAttribute,
+                (T) => T.setAttribute,
                 "call",
-                (A) => A("tabindex", "0")
-            ]), v.addEventListener("focus", () => {}), g.addEventListener("focus", () => {}));
+                (T) => T("tabindex", "0")
+            ]), v.addEventListener("focus", () => {}), b.addEventListener("focus", () => {}));
         }
         t.$$.dirty[0] & /*url*/
-            16777216 && i && Ce(i);
+            16777216 && i && B(i);
     }, [
         o,
         f,
         r,
         s,
         a,
         l,
         u,
         c,
         h,
         d,
         S,
         w,
         k,
-        C,
+        E,
         y,
+        M,
         x,
-        O,
         H,
-        p,
+        J,
+        A,
         _,
         m,
         v,
-        g,
-        L,
+        b,
         i,
-        B,
         R,
         ce,
         Se,
         wt,
         Y,
         yt,
         wn,
@@ -7557,20 +7565,20 @@
     detach: vi,
     element: gu,
     empty: Mm,
     group_outros: bu,
     init: Dm,
     insert: wi,
     mount_component: Yn,
-    safe_not_equal: Om,
+    safe_not_equal: Hm,
     space: Fr,
     transition_in: Ke,
     transition_out: ft
 } = window.__gradio__svelte__internal, {
-    createEventDispatcher: Hm
+    createEventDispatcher: Om
 } = window.__gradio__svelte__internal;
 
 function Nm(t) {
     let e, n;
     return e = new Fa({
         props: {
             size: "small",
@@ -7688,15 +7696,15 @@
             l && (vi(e), vi(i)), s && s.d(), Jn(o, l);
         }
     };
 }
 
 function Um(t) {
     let e, n;
-    return e = new po({}), {
+    return e = new mo({}), {
         c() {
             Zn(e.$$.fragment);
         },
         m(i, o) {
             Yn(e, i, o), n = !0;
         },
         i(i) {
@@ -7802,15 +7810,15 @@
     let e, n, i, o, r, s;
     e = new Ia({
         props: {
             show_label: (
                 /*show_label*/
                 t[2]
             ),
-            Icon: po,
+            Icon: mo,
             float: !1,
             label: (
                 /*label*/
                 t[1] || /*i18n*/
                 t[4]("audio.audio")
             )
         }
@@ -7869,38 +7877,38 @@
     } = e, {
         i18n: a
     } = e, {
         waveform_settings: l
     } = e, {
         waveform_options: u
     } = e;
-    const c = Hm(),
-        f = async (g) => g ? `<audio controls src="${await Hc(g.url, "url")}"></audio>` : "";
+    const c = Om(),
+        f = async (b) => b ? `<audio controls src="${await Oc(b.url, "url")}"></audio>` : "";
 
-    function h(g) {
-        li.call(this, t, g);
+    function h(b) {
+        li.call(this, t, b);
     }
 
-    function d(g) {
-        li.call(this, t, g);
+    function d(b) {
+        li.call(this, t, b);
     }
 
-    function _(g) {
-        li.call(this, t, g);
+    function _(b) {
+        li.call(this, t, b);
     }
 
-    function m(g) {
-        li.call(this, t, g);
+    function m(b) {
+        li.call(this, t, b);
     }
 
-    function v(g) {
-        li.call(this, t, g);
+    function v(b) {
+        li.call(this, t, b);
     }
-    return t.$$set = (g) => {
-        "value" in g && n(0, i = g.value), "label" in g && n(1, o = g.label), "show_label" in g && n(2, r = g.show_label), "show_download_button" in g && n(3, s = g.show_download_button), "i18n" in g && n(4, a = g.i18n), "waveform_settings" in g && n(5, l = g.waveform_settings), "waveform_options" in g && n(6, u = g.waveform_options);
+    return t.$$set = (b) => {
+        "value" in b && n(0, i = b.value), "label" in b && n(1, o = b.label), "show_label" in b && n(2, r = b.show_label), "show_download_button" in b && n(3, s = b.show_download_button), "i18n" in b && n(4, a = b.i18n), "waveform_settings" in b && n(5, l = b.waveform_settings), "waveform_options" in b && n(6, u = b.waveform_options);
     }, t.$$.update = () => {
         t.$$.dirty & /*value*/
             1 && i && c("change", i);
     }, [
         i,
         o,
         r,
@@ -7914,15 +7922,15 @@
         _,
         m,
         v
     ];
 }
 class Gm extends Rm {
     constructor(e) {
-        super(), Dm(this, e, zm, Fm, Om, {
+        super(), Dm(this, e, zm, Fm, Hm, {
             value: 0,
             label: 1,
             show_label: 2,
             show_download_button: 3,
             i18n: 4,
             waveform_settings: 5,
             waveform_options: 6
@@ -7956,33 +7964,33 @@
     }
     const n = t.subscribe(...e);
     return n.unsubscribe ? () => n.unsubscribe() : n;
 }
 const vu = typeof window < "u";
 let yl = vu ? () => window.performance.now() : () => Date.now(),
     wu = vu ? (t) => requestAnimationFrame(t) : ln;
-const Hn = /* @__PURE__ */ new Set();
+const On = /* @__PURE__ */ new Set();
 
 function yu(t) {
-    Hn.forEach((e) => {
-        e.c(t) || (Hn.delete(e), e.f());
-    }), Hn.size !== 0 && wu(yu);
+    On.forEach((e) => {
+        e.c(t) || (On.delete(e), e.f());
+    }), On.size !== 0 && wu(yu);
 }
 
 function Jm(t) {
     let e;
-    return Hn.size === 0 && wu(yu), {
+    return On.size === 0 && wu(yu), {
         promise: new Promise((n) => {
-            Hn.add(e = {
+            On.add(e = {
                 c: t,
                 f: n
             });
         }),
         abort() {
-            Hn.delete(e);
+            On.delete(e);
         }
     };
 }
 const An = [];
 
 function Ym(t, e) {
     return {
@@ -8097,38 +8105,38 @@
         } = e;
     let s, a, l, u = t,
         c = t,
         f = 1,
         h = 0,
         d = !1;
 
-    function _(v, g = {}) {
+    function _(v, b = {}) {
         c = v;
         const S = l = {};
-        return t == null || g.hard || m.stiffness >= 1 && m.damping >= 1 ? (d = !0, s = yl(), u = v, n.set(t = c), Promise.resolve()) : (g.soft && (h = 1 / ((g.soft === !0 ? 0.5 : +g.soft) * 60), f = 0), a || (s = yl(), d = !1, a = Jm((w) => {
+        return t == null || b.hard || m.stiffness >= 1 && m.damping >= 1 ? (d = !0, s = yl(), u = v, n.set(t = c), Promise.resolve()) : (b.soft && (h = 1 / ((b.soft === !0 ? 0.5 : +b.soft) * 60), f = 0), a || (s = yl(), d = !1, a = Jm((w) => {
             if (d)
                 return d = !1, a = null, !1;
             f = Math.min(f + h, 1);
             const k = {
                     inv_mass: f,
                     opts: m,
                     settled: !0,
                     dt: (w - s) * 60 / 1e3
                 },
-                C = qr(k, u, t, c);
-            return s = w, u = t, n.set(t = C), k.settled && (a = null), !k.settled;
+                E = qr(k, u, t, c);
+            return s = w, u = t, n.set(t = E), k.settled && (a = null), !k.settled;
         })), new Promise((w) => {
             a.promise.then(() => {
                 S === l && w();
             });
         }));
     }
     const m = {
         set: _,
-        update: (v, g) => _(v(c, t), g),
+        update: (v, b) => _(v(c, t), b),
         subscribe: n.subscribe,
         stiffness: i,
         damping: o,
         precision: r
     };
     return m;
 }
@@ -8232,36 +8240,36 @@
         n.__proto__ = i;
     } || function(n, i) {
         for (var o in i)
             Object.prototype.hasOwnProperty.call(i, o) && (n[o] = i[o]);
     }, zr(t, e);
 };
 
-function Co(t, e) {
+function Eo(t, e) {
     if (typeof e != "function" && e !== null)
         throw new TypeError("Class extends value " + String(e) + " is not a constructor or null");
     zr(t, e);
 
     function n() {
         this.constructor = t;
     }
     t.prototype = e === null ? Object.create(e) : (n.prototype = e.prototype, new n());
 }
-var ie = function() {
-    return ie = Object.assign || function(e) {
+var ne = function() {
+    return ne = Object.assign || function(e) {
         for (var n, i = 1, o = arguments.length; i < o; i++) {
             n = arguments[i];
             for (var r in n)
                 Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r]);
         }
         return e;
-    }, ie.apply(this, arguments);
+    }, ne.apply(this, arguments);
 };
 
-function pr(t, e, n) {
+function mr(t, e, n) {
     if (n || arguments.length === 2)
         for (var i = 0, o = e.length, r; i < o; i++)
             (r || !(i in e)) && (r || (r = Array.prototype.slice.call(e, 0, i)), r[i] = e[i]);
     return t.concat(r || Array.prototype.slice.call(e));
 }
 var Q;
 (function(t) {
@@ -8546,25 +8554,25 @@
                 e.notation = "compact", e.compactDisplay = "short";
                 continue;
             case "compact-long":
             case "KK":
                 e.notation = "compact", e.compactDisplay = "long";
                 continue;
             case "scientific":
-                e = ie(ie(ie({}, e), {
+                e = ne(ne(ne({}, e), {
                     notation: "scientific"
                 }), o.options.reduce(function(l, u) {
-                    return ie(ie({}, l), Pl(u));
+                    return ne(ne({}, l), Pl(u));
                 }, {}));
                 continue;
             case "engineering":
-                e = ie(ie(ie({}, e), {
+                e = ne(ne(ne({}, e), {
                     notation: "engineering"
                 }), o.options.reduce(function(l, u) {
-                    return ie(ie({}, l), Pl(u));
+                    return ne(ne({}, l), Pl(u));
                 }, {}));
                 continue;
             case "notation-simple":
                 e.notation = "standard";
                 continue;
             case "unit-width-narrow":
                 e.currencyDisplay = "narrowSymbol", e.unitDisplay = "narrow";
@@ -8604,27 +8612,27 @@
         if (Al.test(o.stem)) {
             if (o.options.length > 1)
                 throw new RangeError("Fraction-precision stems only accept a single optional option");
             o.stem.replace(Al, function(l, u, c, f, h, d) {
                 return c === "*" ? e.minimumFractionDigits = u.length : f && f[0] === "#" ? e.maximumFractionDigits = f.length : h && d ? (e.minimumFractionDigits = h.length, e.maximumFractionDigits = h.length + d.length) : (e.minimumFractionDigits = u.length, e.maximumFractionDigits = u.length), "";
             });
             var r = o.options[0];
-            r === "w" ? e = ie(ie({}, e), {
+            r === "w" ? e = ne(ne({}, e), {
                 trailingZeroDisplay: "stripIfInteger"
-            }) : r && (e = ie(ie({}, e), Tl(r)));
+            }) : r && (e = ne(ne({}, e), Tl(r)));
             continue;
         }
         if (Bu.test(o.stem)) {
-            e = ie(ie({}, e), Tl(o.stem));
+            e = ne(ne({}, e), Tl(o.stem));
             continue;
         }
         var s = Du(o.stem);
-        s && (e = ie(ie({}, e), s));
+        s && (e = ne(ne({}, e), s));
         var a = yp(o.stem);
-        a && (e = ie(ie({}, e), a));
+        a && (e = ne(ne({}, e), a));
     }
     return e;
 }
 var Zi = {
     AX: [
         "H"
     ],
@@ -10001,37 +10009,37 @@
         }
     var n = t.language,
         i;
     n !== "root" && (i = t.maximize().region);
     var o = Zi[i || ""] || Zi[n || ""] || Zi["".concat(n, "-001")] || Zi["001"];
     return o[0];
 }
-var gr, Sp = new RegExp("^".concat(Ru.source, "*")),
+var pr, Sp = new RegExp("^".concat(Ru.source, "*")),
     Ap = new RegExp("".concat(Ru.source, "*$"));
 
-function K(t, e) {
+function $(t, e) {
     return {
         start: t,
         end: e
     };
 }
 var Tp = !!String.prototype.startsWith,
     Pp = !!String.fromCodePoint,
     Lp = !!Object.fromEntries,
     Rp = !!String.prototype.codePointAt,
     Bp = !!String.prototype.trimStart,
     Mp = !!String.prototype.trimEnd,
     Dp = !!Number.isSafeInteger,
-    Op = Dp ? Number.isSafeInteger : function(t) {
+    Hp = Dp ? Number.isSafeInteger : function(t) {
         return typeof t == "number" && isFinite(t) && Math.floor(t) === t && Math.abs(t) <= 9007199254740991;
     },
     Wr = !0;
 try {
-    var Hp = Hu("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
-    Wr = ((gr = Hp.exec("a")) === null || gr === void 0 ? void 0 : gr[0]) === "a";
+    var Op = Ou("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+    Wr = ((pr = Op.exec("a")) === null || pr === void 0 ? void 0 : pr[0]) === "a";
 } catch {
     Wr = !1;
 }
 var Ll = Tp ? (
         // Native
         function(e, n, i) {
             return e.startsWith(n, i);
@@ -10066,15 +10074,15 @@
                         a = r[1];
                     n[s] = a;
                 }
                 return n;
             }
         )
     ),
-    Ou = Rp ? (
+    Hu = Rp ? (
         // Native
         function(e, n) {
             return e.codePointAt(n);
         }
     ) : (
         // IE 11
         function(e, n) {
@@ -10105,30 +10113,30 @@
     ) : (
         // Ponyfill
         function(e) {
             return e.replace(Ap, "");
         }
     );
 
-function Hu(t, e) {
+function Ou(t, e) {
     return new RegExp(t, e);
 }
 var Xr;
 if (Wr) {
-    var Bl = Hu("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
+    var Bl = Ou("([^\\p{White_Space}\\p{Pattern_Syntax}]*)", "yu");
     Xr = function(e, n) {
         var i;
         Bl.lastIndex = n;
         var o = Bl.exec(e);
         return (i = o[1]) !== null && i !== void 0 ? i : "";
     };
 } else
     Xr = function(e, n) {
         for (var i = [];;) {
-            var o = Ou(e, n);
+            var o = Hu(e, n);
             if (o === void 0 || Nu(o) || qp(o))
                 break;
             i.push(o), n += o >= 65536 ? 2 : 1;
         }
         return Vr.apply(void 0, i);
     };
 var Up = (
@@ -10156,20 +10164,20 @@
                 } else {
                     if (r === 125 && e > 0)
                         break;
                     if (r === 35 && (n === "plural" || n === "selectordinal")) {
                         var a = this.clonePosition();
                         this.bump(), o.push({
                             type: fe.pound,
-                            location: K(a, this.clonePosition())
+                            location: $(a, this.clonePosition())
                         });
                     } else if (r === 60 && !this.ignoreTag && this.peek() === 47) {
                         if (i)
                             break;
-                        return this.error(Q.UNMATCHED_CLOSING_TAG, K(this.clonePosition(), this.clonePosition()));
+                        return this.error(Q.UNMATCHED_CLOSING_TAG, $(this.clonePosition(), this.clonePosition()));
                     } else if (r === 60 && !this.ignoreTag && xr(this.peek() || 0)) {
                         var s = this.parseTag(e, n);
                         if (s.err)
                             return s;
                         o.push(s.val);
                     } else {
                         var s = this.parseLiteral(e, n);
@@ -10188,42 +10196,42 @@
             this.bump();
             var o = this.parseTagName();
             if (this.bumpSpace(), this.bumpIf("/>"))
                 return {
                     val: {
                         type: fe.literal,
                         value: "<".concat(o, "/>"),
-                        location: K(i, this.clonePosition())
+                        location: $(i, this.clonePosition())
                     },
                     err: null
                 };
             if (this.bumpIf(">")) {
                 var r = this.parseMessage(e + 1, n, !0);
                 if (r.err)
                     return r;
                 var s = r.val,
                     a = this.clonePosition();
                 if (this.bumpIf("</")) {
                     if (this.isEOF() || !xr(this.char()))
-                        return this.error(Q.INVALID_TAG, K(a, this.clonePosition()));
+                        return this.error(Q.INVALID_TAG, $(a, this.clonePosition()));
                     var l = this.clonePosition(),
                         u = this.parseTagName();
-                    return o !== u ? this.error(Q.UNMATCHED_CLOSING_TAG, K(l, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
+                    return o !== u ? this.error(Q.UNMATCHED_CLOSING_TAG, $(l, this.clonePosition())) : (this.bumpSpace(), this.bumpIf(">") ? {
                         val: {
                             type: fe.tag,
                             value: o,
                             children: s,
-                            location: K(i, this.clonePosition())
+                            location: $(i, this.clonePosition())
                         },
                         err: null
-                    } : this.error(Q.INVALID_TAG, K(a, this.clonePosition())));
+                    } : this.error(Q.INVALID_TAG, $(a, this.clonePosition())));
                 } else
-                    return this.error(Q.UNCLOSED_TAG, K(i, this.clonePosition()));
+                    return this.error(Q.UNCLOSED_TAG, $(i, this.clonePosition()));
             } else
-                return this.error(Q.INVALID_TAG, K(i, this.clonePosition()));
+                return this.error(Q.INVALID_TAG, $(i, this.clonePosition()));
         }, t.prototype.parseTagName = function() {
             var e = this.offset();
             for (this.bump(); !this.isEOF() && Fp(this.char());)
                 this.bump();
             return this.message.slice(e, this.offset());
         }, t.prototype.parseLiteral = function(e, n) {
             for (var i = this.clonePosition(), o = "";;) {
@@ -10240,15 +10248,15 @@
                 var a = this.tryParseLeftAngleBracket();
                 if (a) {
                     o += a;
                     continue;
                 }
                 break;
             }
-            var l = K(i, this.clonePosition());
+            var l = $(i, this.clonePosition());
             return {
                 val: {
                     type: fe.literal,
                     value: o,
                     location: l
                 },
                 err: null
@@ -10294,81 +10302,81 @@
             if (this.isEOF())
                 return null;
             var i = this.char();
             return i === 60 || i === 123 || i === 35 && (n === "plural" || n === "selectordinal") || i === 125 && e > 0 ? null : (this.bump(), Vr(i));
         }, t.prototype.parseArgument = function(e, n) {
             var i = this.clonePosition();
             if (this.bump(), this.bumpSpace(), this.isEOF())
-                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, K(i, this.clonePosition()));
+                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition()));
             if (this.char() === 125)
-                return this.bump(), this.error(Q.EMPTY_ARGUMENT, K(i, this.clonePosition()));
+                return this.bump(), this.error(Q.EMPTY_ARGUMENT, $(i, this.clonePosition()));
             var o = this.parseIdentifierIfPossible().value;
             if (!o)
-                return this.error(Q.MALFORMED_ARGUMENT, K(i, this.clonePosition()));
+                return this.error(Q.MALFORMED_ARGUMENT, $(i, this.clonePosition()));
             if (this.bumpSpace(), this.isEOF())
-                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, K(i, this.clonePosition()));
+                return this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition()));
             switch (this.char()) {
                 case 125:
                     return this.bump(), {
                         val: {
                             type: fe.argument,
                             // value does not include the opening and closing braces.
                             value: o,
-                            location: K(i, this.clonePosition())
+                            location: $(i, this.clonePosition())
                         },
                         err: null
                     };
                 case 44:
-                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, K(i, this.clonePosition())) : this.parseArgumentOptions(e, n, o, i);
+                    return this.bump(), this.bumpSpace(), this.isEOF() ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(i, this.clonePosition())) : this.parseArgumentOptions(e, n, o, i);
                 default:
-                    return this.error(Q.MALFORMED_ARGUMENT, K(i, this.clonePosition()));
+                    return this.error(Q.MALFORMED_ARGUMENT, $(i, this.clonePosition()));
             }
         }, t.prototype.parseIdentifierIfPossible = function() {
             var e = this.clonePosition(),
                 n = this.offset(),
                 i = Xr(this.message, n),
                 o = n + i.length;
             this.bumpTo(o);
             var r = this.clonePosition(),
-                s = K(e, r);
+                s = $(e, r);
             return {
                 value: i,
                 location: s
             };
         }, t.prototype.parseArgumentOptions = function(e, n, i, o) {
             var r, s = this.clonePosition(),
                 a = this.parseIdentifierIfPossible().value,
                 l = this.clonePosition();
             switch (a) {
                 case "":
-                    return this.error(Q.EXPECT_ARGUMENT_TYPE, K(s, l));
+                    return this.error(Q.EXPECT_ARGUMENT_TYPE, $(s, l));
                 case "number":
                 case "date":
                 case "time": {
                     this.bumpSpace();
                     var u = null;
                     if (this.bumpIf(",")) {
                         this.bumpSpace();
                         var c = this.clonePosition(),
                             f = this.parseSimpleArgStyleIfPossible();
                         if (f.err)
                             return f;
                         var h = Ip(f.val);
                         if (h.length === 0)
-                            return this.error(Q.EXPECT_ARGUMENT_STYLE, K(this.clonePosition(), this.clonePosition()));
-                        var d = K(c, this.clonePosition());
+                            return this.error(Q.EXPECT_ARGUMENT_STYLE, $(this.clonePosition(), this.clonePosition()));
+                        var d = $(c, this.clonePosition());
                         u = {
                             style: h,
                             styleLocation: d
                         };
                     }
                     var _ = this.tryParseArgumentClose(o);
                     if (_.err)
                         return _;
-                    var m = K(o, this.clonePosition());
+                    var m = $(o, this.clonePosition());
                     if (u && Ll(u == null ? void 0 : u.style, "::", 0)) {
                         var v = Np(u.style.slice(2));
                         if (a === "number") {
                             var f = this.parseNumberSkeletonFromString(v, u.styleLocation);
                             return f.err ? f : {
                                 val: {
                                     type: fe.number,
@@ -10377,21 +10385,21 @@
                                     style: f.val
                                 },
                                 err: null
                             };
                         } else {
                             if (v.length === 0)
                                 return this.error(Q.EXPECT_DATE_TIME_SKELETON, m);
-                            var g = v;
-                            this.locale && (g = Ep(v, this.locale));
+                            var b = v;
+                            this.locale && (b = Ep(v, this.locale));
                             var h = {
                                     type: Un.dateTime,
-                                    pattern: g,
+                                    pattern: b,
                                     location: u.styleLocation,
-                                    parsedOptions: this.shouldParseSkeletons ? pp(g) : {}
+                                    parsedOptions: this.shouldParseSkeletons ? pp(b) : {}
                                 },
                                 S = a === "date" ? fe.date : fe.time;
                             return {
                                 val: {
                                     type: S,
                                     value: i,
                                     location: m,
@@ -10412,71 +10420,71 @@
                     };
                 }
                 case "plural":
                 case "selectordinal":
                 case "select": {
                     var w = this.clonePosition();
                     if (this.bumpSpace(), !this.bumpIf(","))
-                        return this.error(Q.EXPECT_SELECT_ARGUMENT_OPTIONS, K(w, ie({}, w)));
+                        return this.error(Q.EXPECT_SELECT_ARGUMENT_OPTIONS, $(w, ne({}, w)));
                     this.bumpSpace();
                     var k = this.parseIdentifierIfPossible(),
-                        C = 0;
+                        E = 0;
                     if (a !== "select" && k.value === "offset") {
                         if (!this.bumpIf(":"))
-                            return this.error(Q.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, K(this.clonePosition(), this.clonePosition()));
+                            return this.error(Q.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, $(this.clonePosition(), this.clonePosition()));
                         this.bumpSpace();
                         var f = this.tryParseDecimalInteger(Q.EXPECT_PLURAL_ARGUMENT_OFFSET_VALUE, Q.INVALID_PLURAL_ARGUMENT_OFFSET_VALUE);
                         if (f.err)
                             return f;
-                        this.bumpSpace(), k = this.parseIdentifierIfPossible(), C = f.val;
+                        this.bumpSpace(), k = this.parseIdentifierIfPossible(), E = f.val;
                     }
                     var y = this.tryParsePluralOrSelectOptions(e, a, n, k);
                     if (y.err)
                         return y;
                     var _ = this.tryParseArgumentClose(o);
                     if (_.err)
                         return _;
-                    var O = K(o, this.clonePosition());
+                    var H = $(o, this.clonePosition());
                     return a === "select" ? {
                         val: {
                             type: fe.select,
                             value: i,
                             options: Rl(y.val),
-                            location: O
+                            location: H
                         },
                         err: null
                     } : {
                         val: {
                             type: fe.plural,
                             value: i,
                             options: Rl(y.val),
-                            offset: C,
+                            offset: E,
                             pluralType: a === "plural" ? "cardinal" : "ordinal",
-                            location: O
+                            location: H
                         },
                         err: null
                     };
                 }
                 default:
-                    return this.error(Q.INVALID_ARGUMENT_TYPE, K(s, l));
+                    return this.error(Q.INVALID_ARGUMENT_TYPE, $(s, l));
             }
         }, t.prototype.tryParseArgumentClose = function(e) {
-            return this.isEOF() || this.char() !== 125 ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, K(e, this.clonePosition())) : (this.bump(), {
+            return this.isEOF() || this.char() !== 125 ? this.error(Q.EXPECT_ARGUMENT_CLOSING_BRACE, $(e, this.clonePosition())) : (this.bump(), {
                 val: !0,
                 err: null
             });
         }, t.prototype.parseSimpleArgStyleIfPossible = function() {
             for (var e = 0, n = this.clonePosition(); !this.isEOF();) {
                 var i = this.char();
                 switch (i) {
                     case 39: {
                         this.bump();
                         var o = this.clonePosition();
                         if (!this.bumpUntil("'"))
-                            return this.error(Q.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, K(o, this.clonePosition()));
+                            return this.error(Q.UNCLOSED_QUOTE_IN_ARGUMENT_STYLE, $(o, this.clonePosition()));
                         this.bump();
                         break;
                     }
                     case 123: {
                         e += 1, this.bump();
                         break;
                     }
@@ -10519,54 +10527,54 @@
             for (var r, s = !1, a = [], l = /* @__PURE__ */ new Set(), u = o.value, c = o.location;;) {
                 if (u.length === 0) {
                     var f = this.clonePosition();
                     if (n !== "select" && this.bumpIf("=")) {
                         var h = this.tryParseDecimalInteger(Q.EXPECT_PLURAL_ARGUMENT_SELECTOR, Q.INVALID_PLURAL_ARGUMENT_SELECTOR);
                         if (h.err)
                             return h;
-                        c = K(f, this.clonePosition()), u = this.message.slice(f.offset, this.offset());
+                        c = $(f, this.clonePosition()), u = this.message.slice(f.offset, this.offset());
                     } else
                         break;
                 }
                 if (l.has(u))
                     return this.error(n === "select" ? Q.DUPLICATE_SELECT_ARGUMENT_SELECTOR : Q.DUPLICATE_PLURAL_ARGUMENT_SELECTOR, c);
                 u === "other" && (s = !0), this.bumpSpace();
                 var d = this.clonePosition();
                 if (!this.bumpIf("{"))
-                    return this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, K(this.clonePosition(), this.clonePosition()));
+                    return this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR_FRAGMENT : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR_FRAGMENT, $(this.clonePosition(), this.clonePosition()));
                 var _ = this.parseMessage(e + 1, n, i);
                 if (_.err)
                     return _;
                 var m = this.tryParseArgumentClose(d);
                 if (m.err)
                     return m;
                 a.push([
                     u, {
                         value: _.val,
-                        location: K(d, this.clonePosition())
+                        location: $(d, this.clonePosition())
                     }
                 ]), l.add(u), this.bumpSpace(), r = this.parseIdentifierIfPossible(), u = r.value, c = r.location;
             }
-            return a.length === 0 ? this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR, K(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !s ? this.error(Q.MISSING_OTHER_CLAUSE, K(this.clonePosition(), this.clonePosition())) : {
+            return a.length === 0 ? this.error(n === "select" ? Q.EXPECT_SELECT_ARGUMENT_SELECTOR : Q.EXPECT_PLURAL_ARGUMENT_SELECTOR, $(this.clonePosition(), this.clonePosition())) : this.requiresOtherClause && !s ? this.error(Q.MISSING_OTHER_CLAUSE, $(this.clonePosition(), this.clonePosition())) : {
                 val: a,
                 err: null
             };
         }, t.prototype.tryParseDecimalInteger = function(e, n) {
             var i = 1,
                 o = this.clonePosition();
             this.bumpIf("+") || this.bumpIf("-") && (i = -1);
             for (var r = !1, s = 0; !this.isEOF();) {
                 var a = this.char();
                 if (a >= 48 && a <= 57)
                     r = !0, s = s * 10 + (a - 48), this.bump();
                 else
                     break;
             }
-            var l = K(o, this.clonePosition());
-            return r ? (s *= i, Op(s) ? {
+            var l = $(o, this.clonePosition());
+            return r ? (s *= i, Hp(s) ? {
                 val: s,
                 err: null
             } : this.error(n, l)) : this.error(e, l);
         }, t.prototype.offset = function() {
             return this.position.offset;
         }, t.prototype.isEOF = function() {
             return this.offset() === this.message.length;
@@ -10576,15 +10584,15 @@
                 line: this.position.line,
                 column: this.position.column
             };
         }, t.prototype.char = function() {
             var e = this.position.offset;
             if (e >= this.message.length)
                 throw Error("out of bound");
-            var n = Ou(this.message, e);
+            var n = Hu(this.message, e);
             if (n === void 0)
                 throw Error("Offset ".concat(e, " is at invalid UTF-16 code unit boundary"));
             return n;
         }, t.prototype.error = function(e, n) {
             return {
                 val: null,
                 err: {
@@ -10662,27 +10670,27 @@
                 delete e.options[n].location, Zr(e.options[n].value);
         else
             Eu(e) && Lu(e.style) || (Cu(e) || Su(e)) && Gr(e.style) ? delete e.style.location : Pu(e) && Zr(e.children);
     });
 }
 
 function zp(t, e) {
-    e === void 0 && (e = {}), e = ie({
+    e === void 0 && (e = {}), e = ne({
         shouldParseSkeletons: !0,
         requiresOtherClause: !0
     }, e);
     var n = new Up(t, e).parse();
     if (n.err) {
         var i = SyntaxError(Q[n.err.kind]);
         throw i.location = n.err.location, i.originalMessage = n.err.message, i;
     }
     return e != null && e.captureLocation || Zr(n.val), n.val;
 }
 
-function br(t, e) {
+function gr(t, e) {
     var n = e && e.cache ? e.cache : Zp,
         i = e && e.serializer ? e.serializer : xp,
         o = e && e.strategy ? e.strategy : Wp;
     return o(t, {
         cache: n,
         serializer: i
     });
@@ -10735,68 +10743,68 @@
     this.cache[t] = e;
 };
 var Zp = {
         create: function() {
             return new cs();
         }
     },
-    vr = {
+    br = {
         variadic: Vp,
         monadic: Xp
     },
     jn;
 (function(t) {
     t.MISSING_VALUE = "MISSING_VALUE", t.INVALID_VALUE = "INVALID_VALUE", t.MISSING_INTL_API = "MISSING_INTL_API";
 })(jn || (jn = {}));
-var So = (
+var Co = (
         /** @class */
         function(t) {
-            Co(e, t);
+            Eo(e, t);
 
             function e(n, i, o) {
                 var r = t.call(this, n) || this;
                 return r.code = i, r.originalMessage = o, r;
             }
             return e.prototype.toString = function() {
                 return "[formatjs Error: ".concat(this.code, "] ").concat(this.message);
             }, e;
         }(Error)
     ),
     Ml = (
         /** @class */
         function(t) {
-            Co(e, t);
+            Eo(e, t);
 
             function e(n, i, o, r) {
                 return t.call(this, 'Invalid values for "'.concat(n, '": "').concat(i, '". Options are "').concat(Object.keys(o).join('", "'), '"'), jn.INVALID_VALUE, r) || this;
             }
             return e;
-        }(So)
+        }(Co)
     ),
     Jp = (
         /** @class */
         function(t) {
-            Co(e, t);
+            Eo(e, t);
 
             function e(n, i, o) {
                 return t.call(this, 'Value for "'.concat(n, '" must be of type ').concat(i), jn.INVALID_VALUE, o) || this;
             }
             return e;
-        }(So)
+        }(Co)
     ),
     Yp = (
         /** @class */
         function(t) {
-            Co(e, t);
+            Eo(e, t);
 
             function e(n, i) {
                 return t.call(this, 'The intl string context variable "'.concat(n, '" was not provided to the string "').concat(i, '"'), jn.MISSING_VALUE, i) || this;
             }
             return e;
-        }(So)
+        }(Co)
     ),
     De;
 (function(t) {
     t[t.literal = 0] = "literal", t[t.object = 1] = "object";
 })(De || (De = {}));
 
 function Qp(t) {
@@ -10806,15 +10814,15 @@
     }, []);
 }
 
 function Kp(t) {
     return typeof t == "function";
 }
 
-function to(t, e, n, i, o, r, s) {
+function eo(t, e, n, i, o, r, s) {
     if (t.length === 1 && Sl(t[0]))
         return [{
             type: De.literal,
             value: t[0].value
         }];
     for (var a = [], l = 0, u = t; l < u.length; l++) {
         var c = u[l];
@@ -10869,66 +10877,66 @@
         }
         if (Pu(c)) {
             var _ = c.children,
                 m = c.value,
                 v = o[m];
             if (!Kp(v))
                 throw new Jp(m, "function", s);
-            var g = to(_, e, n, i, o, r),
-                S = v(g.map(function(C) {
-                    return C.value;
+            var b = eo(_, e, n, i, o, r),
+                S = v(b.map(function(E) {
+                    return E.value;
                 }));
-            Array.isArray(S) || (S = [S]), a.push.apply(a, S.map(function(C) {
+            Array.isArray(S) || (S = [S]), a.push.apply(a, S.map(function(E) {
                 return {
-                    type: typeof C == "string" ? De.literal : De.object,
-                    value: C
+                    type: typeof E == "string" ? De.literal : De.object,
+                    value: E
                 };
             }));
         }
         if (Au(c)) {
             var w = c.options[h] || c.options.other;
             if (!w)
                 throw new Ml(c.value, h, Object.keys(c.options), s);
-            a.push.apply(a, to(w.value, e, n, i, o));
+            a.push.apply(a, eo(w.value, e, n, i, o));
             continue;
         }
         if (Tu(c)) {
             var w = c.options["=".concat(h)];
             if (!w) {
                 if (!Intl.PluralRules)
-                    throw new So(`Intl.PluralRules is not available in this environment.
+                    throw new Co(`Intl.PluralRules is not available in this environment.
 Try polyfilling it using "@formatjs/intl-pluralrules"
 `, jn.MISSING_INTL_API, s);
                 var k = n.getPluralRules(e, {
                     type: c.pluralType
                 }).select(h - (c.offset || 0));
                 w = c.options[k] || c.options.other;
             }
             if (!w)
                 throw new Ml(c.value, h, Object.keys(c.options), s);
-            a.push.apply(a, to(w.value, e, n, i, o, h - (c.offset || 0)));
+            a.push.apply(a, eo(w.value, e, n, i, o, h - (c.offset || 0)));
             continue;
         }
     }
     return Qp(a);
 }
 
 function $p(t, e) {
-    return e ? ie(ie(ie({}, t || {}), e || {}), Object.keys(t).reduce(function(n, i) {
-        return n[i] = ie(ie({}, t[i]), e[i] || {}), n;
+    return e ? ne(ne(ne({}, t || {}), e || {}), Object.keys(t).reduce(function(n, i) {
+        return n[i] = ne(ne({}, t[i]), e[i] || {}), n;
     }, {})) : t;
 }
 
 function e1(t, e) {
     return e ? Object.keys(t).reduce(function(n, i) {
         return n[i] = $p(t[i], e[i]), n;
-    }, ie({}, t)) : t;
+    }, ne({}, t)) : t;
 }
 
-function wr(t) {
+function vr(t) {
     return {
         create: function() {
             return {
                 get: function(e) {
                     return t[e];
                 },
                 set: function(e, n) {
@@ -10941,37 +10949,37 @@
 
 function t1(t) {
     return t === void 0 && (t = {
         number: {},
         dateTime: {},
         pluralRules: {}
     }), {
-        getNumberFormat: br(function() {
+        getNumberFormat: gr(function() {
             for (var e, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((e = Intl.NumberFormat).bind.apply(e, pr([void 0], n, !1)))();
+            return new((e = Intl.NumberFormat).bind.apply(e, mr([void 0], n, !1)))();
         }, {
-            cache: wr(t.number),
-            strategy: vr.variadic
+            cache: vr(t.number),
+            strategy: br.variadic
         }),
-        getDateTimeFormat: br(function() {
+        getDateTimeFormat: gr(function() {
             for (var e, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((e = Intl.DateTimeFormat).bind.apply(e, pr([void 0], n, !1)))();
+            return new((e = Intl.DateTimeFormat).bind.apply(e, mr([void 0], n, !1)))();
         }, {
-            cache: wr(t.dateTime),
-            strategy: vr.variadic
+            cache: vr(t.dateTime),
+            strategy: br.variadic
         }),
-        getPluralRules: br(function() {
+        getPluralRules: gr(function() {
             for (var e, n = [], i = 0; i < arguments.length; i++)
                 n[i] = arguments[i];
-            return new((e = Intl.PluralRules).bind.apply(e, pr([void 0], n, !1)))();
+            return new((e = Intl.PluralRules).bind.apply(e, mr([void 0], n, !1)))();
         }, {
-            cache: wr(t.pluralRules),
-            strategy: vr.variadic
+            cache: vr(t.pluralRules),
+            strategy: br.variadic
         })
     };
 }
 var n1 = (
     /** @class */
     function() {
         function t(e, n, i, o) {
@@ -10985,15 +10993,15 @@
                     if (a.length === 1)
                         return a[0].value;
                     var l = a.reduce(function(u, c) {
                         return !u.length || c.type !== De.literal || typeof u[u.length - 1] != "string" ? u.push(c.value) : u[u.length - 1] += c.value, u;
                     }, []);
                     return l.length <= 1 ? l[0] || "" : l;
                 }, this.formatToParts = function(s) {
-                    return to(r.ast, r.locales, r.formatters, r.formats, s, void 0, r.message);
+                    return eo(r.ast, r.locales, r.formatters, r.formats, s, void 0, r.message);
                 }, this.resolvedOptions = function() {
                     return {
                         locale: r.resolvedLocale.toString()
                     };
                 }, this.getAst = function() {
                     return r.ast;
                 }, this.locales = n, this.resolvedLocale = t.resolveLocale(n), typeof e == "string") {
@@ -11104,15 +11112,15 @@
 const Nt = {},
     o1 = (t, e, n) => n && (e in Nt || (Nt[e] = {}), t in Nt[e] || (Nt[e][t] = n), n),
     ju = (t, e) => {
         if (e == null)
             return;
         if (e in Nt && t in Nt[e])
             return Nt[e][t];
-        const n = Ao(e);
+        const n = So(e);
         for (let i = 0; i < n.length; i++) {
             const o = n[i],
                 r = s1(o, t);
             if (r)
                 return o1(t, e, r);
         }
     };
@@ -11133,15 +11141,15 @@
     const n = r1(t);
     return i1(n, e);
 }
 
 function l1(t) {
     if (t == null)
         return;
-    const e = Ao(t);
+    const e = So(t);
     for (let n = 0; n < e.length; n++) {
         const i = e[n];
         if (Fu(i))
             return i;
     }
 }
 
@@ -11149,33 +11157,33 @@
     delete Nt[t], Ti.update((n) => (n[t] = dp.all([n[t] || {}, ...e]), n));
 }
 Qn(
     [Ti],
     ([t]) => Object.keys(t)
 );
 Ti.subscribe((t) => fs = t);
-const no = {};
+const to = {};
 
 function u1(t, e) {
-    no[t].delete(e), no[t].size === 0 && delete no[t];
+    to[t].delete(e), to[t].size === 0 && delete to[t];
 }
 
 function qu(t) {
-    return no[t];
+    return to[t];
 }
 
 function c1(t) {
-    return Ao(t).map((e) => {
+    return So(t).map((e) => {
         const n = qu(e);
         return [e, n ? [...n] : []];
     }).filter(([, e]) => e.length > 0);
 }
 
 function Jr(t) {
-    return t == null ? !1 : Ao(t).some(
+    return t == null ? !1 : So(t).some(
         (e) => {
             var n;
             return (n = qu(e)) == null ? void 0 : n.size;
         }
     );
 }
 
@@ -11273,143 +11281,143 @@
         ignoreTag: !0
     },
     _1 = h1;
 
 function Fn() {
     return _1;
 }
-const yr = Ai(!1);
+const wr = Ai(!1);
 var m1 = Object.defineProperty,
     p1 = Object.defineProperties,
     g1 = Object.getOwnPropertyDescriptors,
     Dl = Object.getOwnPropertySymbols,
     b1 = Object.prototype.hasOwnProperty,
     v1 = Object.prototype.propertyIsEnumerable,
-    Ol = (t, e, n) => e in t ? m1(t, e, {
+    Hl = (t, e, n) => e in t ? m1(t, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : t[e] = n,
     w1 = (t, e) => {
         for (var n in e || (e = {}))
-            b1.call(e, n) && Ol(t, n, e[n]);
+            b1.call(e, n) && Hl(t, n, e[n]);
         if (Dl)
             for (var n of Dl(e))
-                v1.call(e, n) && Ol(t, n, e[n]);
+                v1.call(e, n) && Hl(t, n, e[n]);
         return t;
     },
     y1 = (t, e) => p1(t, g1(e));
 let Yr;
-const uo = Ai(null);
+const ao = Ai(null);
 
-function Hl(t) {
+function Ol(t) {
     return t.split("-").map((e, n, i) => i.slice(0, n + 1).join("-")).reverse();
 }
 
-function Ao(t, e = Fn().fallbackLocale) {
-    const n = Hl(t);
-    return e ? [... /* @__PURE__ */ new Set([...n, ...Hl(e)])] : n;
+function So(t, e = Fn().fallbackLocale) {
+    const n = Ol(t);
+    return e ? [... /* @__PURE__ */ new Set([...n, ...Ol(e)])] : n;
 }
 
 function vn() {
     return Yr ?? void 0;
 }
-uo.subscribe((t) => {
+ao.subscribe((t) => {
     Yr = t ?? void 0, typeof window < "u" && t != null && document.documentElement.setAttribute("lang", t);
 });
 const k1 = (t) => {
         if (t && l1(t) && Jr(t)) {
             const {
                 loadingDelay: e
             } = Fn();
             let n;
             return typeof window < "u" && vn() != null && e ? n = window.setTimeout(
-                () => yr.set(!0),
+                () => wr.set(!0),
                 e
-            ) : yr.set(!0), zu(t).then(() => {
-                uo.set(t);
+            ) : wr.set(!0), zu(t).then(() => {
+                ao.set(t);
             }).finally(() => {
-                clearTimeout(n), yr.set(!1);
+                clearTimeout(n), wr.set(!1);
             });
         }
-        return uo.set(t);
+        return ao.set(t);
     },
-    Pi = y1(w1({}, uo), {
+    Pi = y1(w1({}, ao), {
         set: k1
     }),
-    To = (t) => {
+    Ao = (t) => {
         const e = /* @__PURE__ */ Object.create(null);
         return (i) => {
             const o = JSON.stringify(i);
             return o in e ? e[o] : e[o] = t(i);
         };
     };
 var E1 = Object.defineProperty,
-    co = Object.getOwnPropertySymbols,
+    uo = Object.getOwnPropertySymbols,
     Gu = Object.prototype.hasOwnProperty,
     Wu = Object.prototype.propertyIsEnumerable,
     Nl = (t, e, n) => e in t ? E1(t, e, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : t[e] = n,
     ds = (t, e) => {
         for (var n in e || (e = {}))
             Gu.call(e, n) && Nl(t, n, e[n]);
-        if (co)
-            for (var n of co(e))
+        if (uo)
+            for (var n of uo(e))
                 Wu.call(e, n) && Nl(t, n, e[n]);
         return t;
     },
     Kn = (t, e) => {
         var n = {};
         for (var i in t)
             Gu.call(t, i) && e.indexOf(i) < 0 && (n[i] = t[i]);
-        if (t != null && co)
-            for (var i of co(t))
+        if (t != null && uo)
+            for (var i of uo(t))
                 e.indexOf(i) < 0 && Wu.call(t, i) && (n[i] = t[i]);
         return n;
     };
 const ki = (t, e) => {
         const {
             formats: n
         } = Fn();
         if (t in n && e in n[t])
             return n[t][e];
         throw new Error(`[svelte-i18n] Unknown "${e}" ${t} format.`);
     },
-    C1 = To(
+    C1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
                 o = Kn(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format numbers');
             return i && (o = ki("number", i)), new Intl.NumberFormat(n, o);
         }
     ),
-    S1 = To(
+    S1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
                 o = Kn(e, ["locale", "format"]);
             if (n == null)
                 throw new Error('[svelte-i18n] A "locale" must be set to format dates');
             return i ? o = ki("date", i) : Object.keys(o).length === 0 && (o = ki("date", "short")), new Intl.DateTimeFormat(n, o);
         }
     ),
-    A1 = To(
+    A1 = Ao(
         (t) => {
             var e = t,
                 {
                     locale: n,
                     format: i
                 } = e,
                 o = Kn(e, ["locale", "format"]);
@@ -11452,15 +11460,15 @@
             i = Kn(e, [
                 "locale"
             ]);
         return A1(ds({
             locale: n
         }, i));
     },
-    R1 = To(
+    R1 = Ao(
         // eslint-disable-next-line @typescript-eslint/no-non-null-assertion
         (t, e = vn()) => new n1(t, e, Fn().formats, {
             ignoreTag: Fn().ignoreTag
         })
     ),
     B1 = (t, e = {}) => {
         var n, i, o, r;
@@ -11497,33 +11505,33 @@
                 h.message
             );
         }
         return f;
     },
     M1 = (t, e) => L1(e).format(t),
     D1 = (t, e) => P1(e).format(t),
-    O1 = (t, e) => T1(e).format(t),
-    H1 = (t, e = vn()) => ju(t, e);
+    H1 = (t, e) => T1(e).format(t),
+    O1 = (t, e = vn()) => ju(t, e);
 Qn([Pi, Ti], () => B1);
 Qn([Pi], () => M1);
 Qn([Pi], () => D1);
-Qn([Pi], () => O1);
-Qn([Pi, Ti], () => H1);
+Qn([Pi], () => H1);
+Qn([Pi, Ti], () => O1);
 const {
     SvelteComponent: N1,
     append: Fe,
     attr: Yt,
     detach: Vu,
     element: Qt,
     init: I1,
     insert: Xu,
     noop: Il,
     safe_not_equal: U1,
-    set_data: fo,
-    set_style: kr,
+    set_data: co,
+    set_style: yr,
     space: Qr,
     text: Rn,
     toggle_class: Ul
 } = window.__gradio__svelte__internal, {
     onMount: j1,
     createEventDispatcher: F1,
     getContext: q1
@@ -11537,34 +11545,34 @@
         s, a, l, u, c = (
             /*file_to_display*/
             t[2].orig_name + ""
         ),
         f;
     return {
         c() {
-            e = Qt("div"), n = Qt("span"), i = Qt("div"), o = Qt("progress"), s = Rn(r), l = Qr(), u = Qt("span"), f = Rn(c), kr(o, "visibility", "hidden"), kr(o, "height", "0"), kr(o, "width", "0"), o.value = a = pi(
+            e = Qt("div"), n = Qt("span"), i = Qt("div"), o = Qt("progress"), s = Rn(r), l = Qr(), u = Qt("span"), f = Rn(c), yr(o, "visibility", "hidden"), yr(o, "height", "0"), yr(o, "width", "0"), o.value = a = pi(
                 /*file_to_display*/
                 t[2]
             ), Yt(o, "max", "100"), Yt(o, "class", "svelte-cr2edf"), Yt(i, "class", "progress-bar svelte-cr2edf"), Yt(u, "class", "file-name svelte-cr2edf"), Yt(e, "class", "file svelte-cr2edf");
         },
         m(h, d) {
             Xu(h, e, d), Fe(e, n), Fe(n, i), Fe(i, o), Fe(o, s), Fe(e, l), Fe(e, u), Fe(u, f);
         },
         p(h, d) {
             d & /*file_to_display*/
                 4 && r !== (r = pi(
                     /*file_to_display*/
                     h[2]
-                ) + "") && fo(s, r), d & /*file_to_display*/
+                ) + "") && co(s, r), d & /*file_to_display*/
                 4 && a !== (a = pi(
                     /*file_to_display*/
                     h[2]
                 )) && (o.value = a), d & /*file_to_display*/
                 4 && c !== (c = /*file_to_display*/
-                    h[2].orig_name + "") && fo(f, c);
+                    h[2].orig_name + "") && co(f, c);
         },
         d(h) {
             h && Vu(e);
         }
     };
 }
 
@@ -11592,17 +11600,17 @@
         },
         m(h, d) {
             Xu(h, e, d), Fe(e, n), Fe(n, i), Fe(n, r), Fe(n, s), Fe(n, l), Fe(n, u), Fe(e, c), f && f.m(e, null);
         },
         p(h, [d]) {
             d & /*files_with_progress*/
                 1 && o !== (o = /*files_with_progress*/
-                    h[0].length + "") && fo(r, o), d & /*files_with_progress*/
+                    h[0].length + "") && co(r, o), d & /*files_with_progress*/
                 1 && a !== (a = /*files_with_progress*/
-                    h[0].length > 1 ? "files" : "file") && fo(l, a), /*file_to_display*/
+                    h[0].length > 1 ? "files" : "file") && co(l, a), /*file_to_display*/
                 h[2] ? f ? f.p(h, d) : (f = jl(h), f.c(), f.m(e, null)) : f && (f.d(1), f = null), d & /*progress*/
                 2 && Ul(
                     e,
                     "progress",
                     /*progress*/
                     h[1]
                 );
@@ -11679,22 +11687,22 @@
     attr: Be,
     binding_callbacks: x1,
     bubble: xt,
     check_outros: xu,
     create_component: Z1,
     create_slot: Zu,
     destroy_component: J1,
-    detach: Po,
+    detach: To,
     element: Kr,
     empty: Ju,
     get_all_dirty_from_scope: Yu,
     get_slot_changes: Qu,
     group_outros: Ku,
     init: Y1,
-    insert: Lo,
+    insert: Po,
     listen: ze,
     mount_component: Q1,
     prevent_default: Zt,
     run_all: K1,
     safe_not_equal: $1,
     set_style: $u,
     space: eg,
@@ -11753,15 +11761,15 @@
                     e,
                     "disable_click",
                     /*disable_click*/
                     t[7]
                 ), $u(e, "height", "100%");
         },
         m(_, m) {
-            Lo(_, e, m), d && d.m(e, null), Fl(e, n), Fl(e, i), t[30](i), u = !0, c || (f = [
+            Po(_, e, m), d && d.m(e, null), Fl(e, n), Fl(e, i), t[30](i), u = !0, c || (f = [
                 ze(
                     i,
                     "change",
                     /*load_files_from_upload*/
                     t[16]
                 ),
                 ze(e, "drag", Jt(Zt(
@@ -11882,28 +11890,28 @@
         i(_) {
             u || (Ut(d, _), u = !0);
         },
         o(_) {
             mn(d, _), u = !1;
         },
         d(_) {
-            _ && Po(e), d && d.d(_), t[30](null), c = !1, K1(f);
+            _ && To(e), d && d.d(_), t[30](null), c = !1, K1(f);
         }
     };
 }
 
 function rg(t) {
     let e, n, i = ! /*hidden*/
         t[9] && ql(t);
     return {
         c() {
             i && i.c(), e = Ju();
         },
         m(o, r) {
-            i && i.m(o, r), Lo(o, e, r), n = !0;
+            i && i.m(o, r), Po(o, e, r), n = !0;
         },
         p(o, r) {
             /*hidden*/
             o[9] ? i && (Ku(), mn(i, 1, 1, () => {
                 i = null;
             }), xu()) : i ? (i.p(o, r), r[0] & /*hidden*/
                 512 && Ut(i, 1)) : (i = ql(o), i.c(), Ut(i, 1), i.m(e.parentNode, e));
@@ -11911,15 +11919,15 @@
         i(o) {
             n || (Ut(i), n = !0);
         },
         o(o) {
             mn(i), n = !1;
         },
         d(o) {
-            o && Po(e), i && i.d(o);
+            o && To(e), i && i.d(o);
         }
     };
 }
 
 function sg(t) {
     let e, n, i, o, r;
     const s = (
@@ -11955,15 +11963,15 @@
                 e,
                 "flex",
                 /*flex*/
                 t[5]
             ), $u(e, "height", "100%");
         },
         m(l, u) {
-            Lo(l, e, u), a && a.m(e, null), i = !0, o || (r = ze(
+            Po(l, e, u), a && a.m(e, null), i = !0, o || (r = ze(
                 e,
                 "click",
                 /*paste_clipboard*/
                 t[10]
             ), o = !0);
         },
         p(l, u) {
@@ -12016,15 +12024,15 @@
         i(l) {
             i || (Ut(a, l), i = !0);
         },
         o(l) {
             mn(a, l), i = !1;
         },
         d(l) {
-            l && Po(e), a && a.d(l), o = !1, r();
+            l && To(e), a && a.d(l), o = !1, r();
         }
     };
 }
 
 function ql(t) {
     let e, n;
     return e = new V1({
@@ -12087,30 +12095,30 @@
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
             n.c(), i = Ju();
         },
         m(l, u) {
-            s[e].m(l, u), Lo(l, i, u), o = !0;
+            s[e].m(l, u), Po(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
             e = a(l), e === c ? s[e].p(l, u) : (Ku(), mn(s[c], 1, 1, () => {
                 s[c] = null;
             }), xu(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Ut(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
             o || (Ut(n), o = !0);
         },
         o(l) {
             mn(n), o = !1;
         },
         d(l) {
-            l && Po(i), s[e].d(l);
+            l && To(i), s[e].d(l);
         }
     };
 }
 
 function zl(t) {
     let e, n = t[0],
         i = 1;
@@ -12164,148 +12172,148 @@
         hidden: d = !1
     } = e, {
         format: _ = "file"
     } = e, {
         uploading: m = !1
     } = e, {
         hidden_upload: v = null
-    } = e, g, S, w;
+    } = e, b, S, w;
     const k = ig("upload_files"),
-        C = tg(),
+        E = tg(),
         y = ["image", "video", "audio", "text", "file"],
-        O = (p) => p.startsWith(".") || p.endsWith("/*") ? p : y.includes(p) ? p + "/*" : "." + p;
+        H = (p) => p.startsWith(".") || p.endsWith("/*") ? p : y.includes(p) ? p + "/*" : "." + p;
 
     function L() {
         n(18, s = !s);
     }
 
     function P() {
         navigator.clipboard.read().then(async (p) => {
-            for (let T = 0; T < p.length; T++) {
-                const q = p[T].types.find((z) => z.startsWith("image/"));
+            for (let A = 0; A < p.length; A++) {
+                const q = p[A].types.find((z) => z.startsWith("image/"));
                 if (q) {
-                    p[T].getType(q).then(async (z) => {
-                        const _e = new File([z], `clipboard.${q.replace("image/", "")}`);
-                        await Z([_e]);
+                    p[A].getType(q).then(async (z) => {
+                        const he = new File([z], `clipboard.${q.replace("image/", "")}`);
+                        await x([he]);
                     });
                     break;
                 }
             }
         });
     }
 
     function M() {
         f || v && (n(2, v.value = "", v), v.click());
     }
-    async function x(p) {
-        await ng(), n(12, g = Math.random().toString(36).substring(2, 15)), n(1, m = !0);
-        const T = await Ra(p, h, g, k);
-        return C("load", c === "single" ? zl([T, "optionalAccess", (q) => q[0]]) : T), n(1, m = !1), T || [];
-    }
     async function Z(p) {
+        await ng(), n(12, b = Math.random().toString(36).substring(2, 15)), n(1, m = !0);
+        const A = await Ra(p, h, b, k);
+        return E("load", c === "single" ? zl([A, "optionalAccess", (q) => q[0]]) : A), n(1, m = !1), A || [];
+    }
+    async function x(p) {
         if (!p.length)
             return;
-        let T = p.map((q) => new File([q], q.name, {
+        let A = p.map((q) => new File([q], q.name, {
             type: q.type
         }));
-        return n(13, S = await Ba(T)), await x(S);
+        return n(13, S = await Ba(A)), await Z(S);
     }
-    async function G(p) {
-        const T = p.target;
-        if (T.files)
+    async function j(p) {
+        const A = p.target;
+        if (A.files)
             if (_ != "blob")
-                await Z(Array.from(T.files));
+                await x(Array.from(A.files));
             else {
                 if (c === "single") {
-                    C("load", T.files[0]);
+                    E("load", A.files[0]);
                     return;
                 }
-                C("load", T.files);
+                E("load", A.files);
             }
     }
     async function X(p) {
         if (n(18, s = !1), !zl([p, "access", (q) => q.dataTransfer, "optionalAccess", (q) => q.files]))
             return;
-        const T = Array.from(p.dataTransfer.files).filter((q) => {
+        const A = Array.from(p.dataTransfer.files).filter((q) => {
             const z = "." + q.name.split(".").pop();
-            return z && ag(w, z, q.type) || (z && Array.isArray(r) ? r.includes(z) : z === r) ? !0 : (C("error", `Invalid file type only ${r} allowed.`), !1);
+            return z && ag(w, z, q.type) || (z && Array.isArray(r) ? r.includes(z) : z === r) ? !0 : (E("error", `Invalid file type only ${r} allowed.`), !1);
         });
-        await Z(T);
+        await x(A);
     }
 
-    function E(p) {
+    function C(p) {
         xt.call(this, t, p);
     }
 
-    function F(p) {
+    function G(p) {
         xt.call(this, t, p);
     }
 
-    function N(p) {
+    function I(p) {
         xt.call(this, t, p);
     }
 
-    function I(p) {
+    function U(p) {
         xt.call(this, t, p);
     }
 
-    function $(p) {
+    function K(p) {
         xt.call(this, t, p);
     }
 
-    function H(p) {
+    function O(p) {
         xt.call(this, t, p);
     }
 
     function J(p) {
         xt.call(this, t, p);
     }
 
-    function ee(p) {
+    function le(p) {
         x1[p ? "unshift" : "push"](() => {
             v = p, n(2, v);
         });
     }
     return t.$$set = (p) => {
         "filetype" in p && n(0, r = p.filetype), "dragging" in p && n(18, s = p.dragging), "boundedheight" in p && n(3, a = p.boundedheight), "center" in p && n(4, l = p.center), "flex" in p && n(5, u = p.flex), "file_count" in p && n(6, c = p.file_count), "disable_click" in p && n(7, f = p.disable_click), "root" in p && n(8, h = p.root), "hidden" in p && n(9, d = p.hidden), "format" in p && n(19, _ = p.format), "uploading" in p && n(1, m = p.uploading), "hidden_upload" in p && n(2, v = p.hidden_upload), "$$scope" in p && n(21, o = p.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*filetype*/
-            1 && (r == null ? n(14, w = null) : typeof r == "string" ? n(14, w = O(r)) : (n(0, r = r.map(O)), n(14, w = r.join(", "))));
+            1 && (r == null ? n(14, w = null) : typeof r == "string" ? n(14, w = H(r)) : (n(0, r = r.map(H)), n(14, w = r.join(", "))));
     }, [
         r,
         m,
         v,
         a,
         l,
         u,
         c,
         f,
         h,
         d,
         P,
         M,
-        g,
+        b,
         S,
         w,
         L,
-        G,
+        j,
         X,
         s,
         _,
-        Z,
+        x,
         o,
         i,
-        E,
-        F,
-        N,
+        C,
+        G,
         I,
-        $,
-        H,
+        U,
+        K,
+        O,
         J,
-        ee
+        le
     ];
 }
 class cg extends X1 {
     constructor(e) {
         super(), Y1(
             this,
             e,
@@ -12340,28 +12348,28 @@
     }
     get load_files() {
         return this.$$.ctx[20];
     }
 }
 const {
     SvelteComponent: fg,
-    append: Er,
+    append: kr,
     attr: dg,
-    check_outros: Cr,
+    check_outros: Er,
     create_component: Li,
     destroy_component: Ri,
     detach: hg,
     element: _g,
-    group_outros: Sr,
+    group_outros: Cr,
     init: mg,
     insert: pg,
     mount_component: Bi,
     safe_not_equal: gg,
     set_style: Gl,
-    space: Ar,
+    space: Sr,
     toggle_class: Wl,
     transition_in: Ie,
     transition_out: lt
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: bg
 } = window.__gradio__svelte__internal;
 
@@ -12546,39 +12554,39 @@
         }
     }), r.$on(
         "click",
         /*click_handler_2*/
         t[8]
     ), {
         c() {
-            e = _g("div"), a && a.c(), n = Ar(), l && l.c(), i = Ar(), u && u.c(), o = Ar(), Li(r.$$.fragment), dg(e, "class", "svelte-1wj0ocy"), Wl(e, "not-absolute", ! /*absolute*/
+            e = _g("div"), a && a.c(), n = Sr(), l && l.c(), i = Sr(), u && u.c(), o = Sr(), Li(r.$$.fragment), dg(e, "class", "svelte-1wj0ocy"), Wl(e, "not-absolute", ! /*absolute*/
                 t[3]), Gl(
                 e,
                 "position",
                 /*absolute*/
                 t[3] ? "absolute" : "static"
             );
         },
         m(c, f) {
-            pg(c, e, f), a && a.m(e, null), Er(e, n), l && l.m(e, null), Er(e, i), u && u.m(e, null), Er(e, o), Bi(r, e, null), s = !0;
+            pg(c, e, f), a && a.m(e, null), kr(e, n), l && l.m(e, null), kr(e, i), u && u.m(e, null), kr(e, o), Bi(r, e, null), s = !0;
         },
         p(c, [f]) {
             /*editable*/
             c[0] ? a ? (a.p(c, f), f & /*editable*/
-                    1 && Ie(a, 1)) : (a = Vl(c), a.c(), Ie(a, 1), a.m(e, n)) : a && (Sr(), lt(a, 1, 1, () => {
+                    1 && Ie(a, 1)) : (a = Vl(c), a.c(), Ie(a, 1), a.m(e, n)) : a && (Cr(), lt(a, 1, 1, () => {
                     a = null;
-                }), Cr()), /*undoable*/
+                }), Er()), /*undoable*/
                 c[1] ? l ? (l.p(c, f), f & /*undoable*/
-                    2 && Ie(l, 1)) : (l = Xl(c), l.c(), Ie(l, 1), l.m(e, i)) : l && (Sr(), lt(l, 1, 1, () => {
+                    2 && Ie(l, 1)) : (l = Xl(c), l.c(), Ie(l, 1), l.m(e, i)) : l && (Cr(), lt(l, 1, 1, () => {
                     l = null;
-                }), Cr()), /*download*/
+                }), Er()), /*download*/
                 c[2] ? u ? (u.p(c, f), f & /*download*/
-                    4 && Ie(u, 1)) : (u = xl(c), u.c(), Ie(u, 1), u.m(e, o)) : u && (Sr(), lt(u, 1, 1, () => {
+                    4 && Ie(u, 1)) : (u = xl(c), u.c(), Ie(u, 1), u.m(e, o)) : u && (Cr(), lt(u, 1, 1, () => {
                     u = null;
-                }), Cr());
+                }), Er());
             const h = {};
             f & /*i18n*/
                 16 && (h.label = /*i18n*/
                     c[4]("common.clear")), r.$set(h), (!s || f & /*absolute*/
                     8) && Wl(e, "not-absolute", ! /*absolute*/
                     c[3]), f & /*absolute*/
                 8 && Gl(
@@ -12653,15 +12661,15 @@
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
 AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
 INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
 LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
 OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 PERFORMANCE OF THIS SOFTWARE.
 ***************************************************************************** */
-function Tr(t, e, n, i) {
+function Ar(t, e, n, i) {
     return new(n || (n = Promise))(function(o, r) {
         function s(u) {
             try {
                 l(i.next(u));
             } catch (c) {
                 r(c);
             }
@@ -12795,15 +12803,15 @@
             },
             onEnd: () => {
                 this.isWaveformPaused = !0, cancelAnimationFrame(a), this.stopMic();
             }
         };
     }
     startMic(e) {
-        return Tr(this, void 0, void 0, function*() {
+        return Ar(this, void 0, void 0, function*() {
             let n;
             try {
                 n = yield navigator.mediaDevices.getUserMedia({
                     audio: !(e != null && e.deviceId) || {
                         deviceId: e.deviceId
                     }
                 });
@@ -12817,15 +12825,15 @@
             return this.subscriptions.push(this.once("destroy", i)), this.subscriptions.push(this.once("record-end", o)), this.stream = n, n;
         });
     }
     stopMic() {
         this.stream && (this.stream.getTracks().forEach((e) => e.stop()), this.stream = null, this.mediaRecorder = null);
     }
     startRecording(e) {
-        return Tr(this, void 0, void 0, function*() {
+        return Ar(this, void 0, void 0, function*() {
             const n = this.stream || (yield this.startMic(e));
             this.dataWindow = null;
             const i = this.mediaRecorder || new MediaRecorder(n, {
                 mimeType: this.options.mimeType || Cg.find((s) => MediaRecorder.isTypeSupported(s)),
                 audioBitsPerSecond: this.options.audioBitsPerSecond
             });
             this.mediaRecorder = i, this.stopRecording();
@@ -12867,15 +12875,15 @@
         this.isRecording() && (this.isWaveformPaused = !0, (e = this.mediaRecorder) === null || e === void 0 || e.requestData(), (n = this.mediaRecorder) === null || n === void 0 || n.pause(), this.timer.stop(), this.lastDuration = this.duration);
     }
     resumeRecording() {
         var e;
         this.isPaused() && (this.isWaveformPaused = !1, (e = this.mediaRecorder) === null || e === void 0 || e.resume(), this.timer.start(), this.lastStartTime = performance.now(), this.emit("record-resume"));
     }
     static getAvailableAudioDevices() {
-        return Tr(this, void 0, void 0, function*() {
+        return Ar(this, void 0, void 0, function*() {
             return navigator.mediaDevices.enumerateDevices().then((e) => e.filter((n) => n.kind === "audioinput"));
         });
     }
     destroy() {
         this.applyOriginalOptionsIfNeeded(), super.destroy(), this.stopRecording(), this.stopMic();
     }
     applyOriginalOptionsIfNeeded() {
@@ -12891,25 +12899,25 @@
     destroy_component: Tg,
     destroy_each: Pg,
     detach: Di,
     element: st,
     empty: Lg,
     ensure_array_like: Zl,
     init: Rg,
-    insert: Oi,
+    insert: Hi,
     listen: ci,
     mount_component: Bg,
     run_all: Mg,
     safe_not_equal: Dg,
     set_data: nn,
     set_input_value: $r,
     space: Tn,
     text: on,
-    transition_in: Og,
-    transition_out: Hg
+    transition_in: Hg,
+    transition_out: Og
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Ng
 } = window.__gradio__svelte__internal;
 
 function Jl(t, e, n) {
     const i = t.slice();
     return i[22] = e[n], i;
@@ -12921,15 +12929,15 @@
         c() {
             e = st("time"), n = on(
                 /*record_time*/
                 t[2]
             ), Ze(e, "class", "duration-button duration svelte-l4xo8n");
         },
         m(i, o) {
-            Oi(i, e, o), be(e, n);
+            Hi(i, e, o), be(e, n);
         },
         p(i, o) {
             o & /*record_time*/
                 4 && nn(
                     n,
                     /*record_time*/
                     i[2]
@@ -12954,15 +12962,15 @@
             for (let o = 0; o < i.length; o += 1)
                 i[o].c();
             e = Lg();
         },
         m(o, r) {
             for (let s = 0; s < i.length; s += 1)
                 i[s] && i[s].m(o, r);
-            Oi(o, e, r);
+            Hi(o, e, r);
         },
         p(o, r) {
             if (r & /*micDevices*/
                 32) {
                 n = Zl(
                     /*micDevices*/
                     o[5]
@@ -12990,15 +12998,15 @@
         ),
         i;
     return {
         c() {
             e = st("option"), i = on(n), e.__value = "", $r(e, e.__value);
         },
         m(o, r) {
-            Oi(o, e, r), be(e, i);
+            Hi(o, e, r), be(e, i);
         },
         p(o, r) {
             r & /*i18n*/
                 2 && n !== (n = /*i18n*/
                     o[1]("audio.no_microphone") + "") && nn(i, n);
         },
         d(o) {
@@ -13015,15 +13023,15 @@
         i, o;
     return {
         c() {
             e = st("option"), i = on(n), e.__value = o = /*micDevice*/
                 t[22].deviceId, $r(e, e.__value);
         },
         m(r, s) {
-            Oi(r, e, s), be(e, i);
+            Hi(r, e, s), be(e, i);
         },
         p(r, s) {
             s & /*micDevices*/
                 32 && n !== (n = /*micDevice*/
                     r[22].label + "") && nn(i, n), s & /*micDevices*/
                 32 && o !== (o = /*micDevice*/
                     r[22].deviceId) && (e.__value = o, $r(e, e.__value));
@@ -13043,42 +13051,42 @@
             /*i18n*/
             t[1]("audio.stop") + ""
         ),
         u, c, f, h, d = (
             /*i18n*/
             t[1]("audio.stop") + ""
         ),
-        _, m, v, g, S, w, k = (
+        _, m, v, b, S, w, k = (
             /*i18n*/
             t[1]("audio.resume") + ""
         ),
-        C, y, O, L, P, M, x, Z;
-    g = new Ga({});
-    let G = (
+        E, y, H, L, P, M, Z, x;
+    b = new Ga({});
+    let j = (
         /*timing*/
         t[4] && ! /*show_recording_waveform*/
         t[3] && Yl(t)
     );
 
-    function X(N, I) {
+    function X(I, U) {
         return (
             /*micDevices*/
-            N[5].length === 0 ? Ug : Ig
+            I[5].length === 0 ? Ug : Ig
         );
     }
-    let E = X(t),
-        F = E(t);
+    let C = X(t),
+        G = C(t);
     return {
         c() {
-            e = st("div"), n = st("div"), i = st("button"), r = on(o), s = Tn(), a = st("button"), u = on(l), f = Tn(), h = st("button"), _ = on(d), m = Tn(), v = st("button"), Ag(g.$$.fragment), S = Tn(), w = st("button"), C = on(k), y = Tn(), G && G.c(), O = Tn(), L = st("select"), F.c(), Ze(i, "class", "record record-button svelte-l4xo8n"), Ze(a, "class", c = "stop-button " + /*record*/
+            e = st("div"), n = st("div"), i = st("button"), r = on(o), s = Tn(), a = st("button"), u = on(l), f = Tn(), h = st("button"), _ = on(d), m = Tn(), v = st("button"), Ag(b.$$.fragment), S = Tn(), w = st("button"), E = on(k), y = Tn(), j && j.c(), H = Tn(), L = st("select"), G.c(), Ze(i, "class", "record record-button svelte-l4xo8n"), Ze(a, "class", c = "stop-button " + /*record*/
                     (t[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n"), Ze(h, "id", "stop-paused"), Ze(h, "class", "stop-button-paused svelte-l4xo8n"), Ze(v, "class", "pause-button svelte-l4xo8n"), Ze(w, "class", "resume-button svelte-l4xo8n"), Ze(n, "class", "wrapper svelte-l4xo8n"), Ze(L, "class", "mic-select svelte-l4xo8n"), Ze(L, "aria-label", "Select input device"), L.disabled = P = /*micDevices*/
                 t[5].length === 0, Ze(e, "class", "controls svelte-l4xo8n");
         },
-        m(N, I) {
-            Oi(N, e, I), be(e, n), be(n, i), be(i, r), t[11](i), be(n, s), be(n, a), be(a, u), t[13](a), be(n, f), be(n, h), be(h, _), t[15](h), be(n, m), be(n, v), Bg(g, v, null), t[17](v), be(n, S), be(n, w), be(w, C), t[19](w), be(n, y), G && G.m(n, null), be(e, O), be(e, L), F.m(L, null), M = !0, x || (Z = [
+        m(I, U) {
+            Hi(I, e, U), be(e, n), be(n, i), be(i, r), t[11](i), be(n, s), be(n, a), be(a, u), t[13](a), be(n, f), be(n, h), be(h, _), t[15](h), be(n, m), be(n, v), Bg(b, v, null), t[17](v), be(n, S), be(n, w), be(w, E), t[19](w), be(n, y), j && j.m(n, null), be(e, H), be(e, L), G.m(L, null), M = !0, Z || (x = [
                 ci(
                     i,
                     "click",
                     /*click_handler*/
                     t[12]
                 ),
                 ci(
@@ -13101,41 +13109,41 @@
                 ),
                 ci(
                     w,
                     "click",
                     /*click_handler_4*/
                     t[20]
                 )
-            ], x = !0);
+            ], Z = !0);
         },
-        p(N, [I]) {
-            (!M || I & /*i18n*/
+        p(I, [U]) {
+            (!M || U & /*i18n*/
                 2) && o !== (o = /*i18n*/
-                    N[1]("audio.record") + "") && nn(r, o), (!M || I & /*i18n*/
+                    I[1]("audio.record") + "") && nn(r, o), (!M || U & /*i18n*/
                     2) && l !== (l = /*i18n*/
-                    N[1]("audio.stop") + "") && nn(u, l), (!M || I & /*record*/
+                    I[1]("audio.stop") + "") && nn(u, l), (!M || U & /*record*/
                     1 && c !== (c = "stop-button " + /*record*/
-                        (N[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n")) && Ze(a, "class", c), (!M || I & /*i18n*/
+                        (I[0].isPaused() ? "stop-button-paused" : "") + " svelte-l4xo8n")) && Ze(a, "class", c), (!M || U & /*i18n*/
                     2) && d !== (d = /*i18n*/
-                    N[1]("audio.stop") + "") && nn(_, d), (!M || I & /*i18n*/
+                    I[1]("audio.stop") + "") && nn(_, d), (!M || U & /*i18n*/
                     2) && k !== (k = /*i18n*/
-                    N[1]("audio.resume") + "") && nn(C, k), /*timing*/
-                N[4] && ! /*show_recording_waveform*/
-                N[3] ? G ? G.p(N, I) : (G = Yl(N), G.c(), G.m(n, null)) : G && (G.d(1), G = null), E === (E = X(N)) && F ? F.p(N, I) : (F.d(1), F = E(N), F && (F.c(), F.m(L, null))), (!M || I & /*micDevices*/
+                    I[1]("audio.resume") + "") && nn(E, k), /*timing*/
+                I[4] && ! /*show_recording_waveform*/
+                I[3] ? j ? j.p(I, U) : (j = Yl(I), j.c(), j.m(n, null)) : j && (j.d(1), j = null), C === (C = X(I)) && G ? G.p(I, U) : (G.d(1), G = C(I), G && (G.c(), G.m(L, null))), (!M || U & /*micDevices*/
                     32 && P !== (P = /*micDevices*/
-                        N[5].length === 0)) && (L.disabled = P);
+                        I[5].length === 0)) && (L.disabled = P);
         },
-        i(N) {
-            M || (Og(g.$$.fragment, N), M = !0);
+        i(I) {
+            M || (Hg(b.$$.fragment, I), M = !0);
         },
-        o(N) {
-            Hg(g.$$.fragment, N), M = !1;
+        o(I) {
+            Og(b.$$.fragment, I), M = !1;
         },
-        d(N) {
-            N && Di(e), t[11](null), t[13](null), t[15](null), Tg(g), t[17](null), t[19](null), G && G.d(), F.d(), x = !1, Mg(Z);
+        d(I) {
+            I && Di(e), t[11](null), t[13](null), t[15](null), Tg(b), t[17](null), t[19](null), j && j.d(), G.d(), Z = !1, Mg(x);
         }
     };
 }
 
 function Fg(t, e, n) {
     let {
         record: i
@@ -13153,15 +13161,15 @@
     function m(P) {
         ui[P ? "unshift" : "push"](() => {
             s = P, n(6, s), n(0, i);
         });
     }
     const v = () => i.startRecording();
 
-    function g(P) {
+    function b(P) {
         ui[P ? "unshift" : "push"](() => {
             u = P, n(9, u), n(0, i);
         });
     }
     const S = () => {
         i.isPaused() && (i.resumeRecording(), i.stopRecording()), i.stopRecording();
     };
@@ -13171,37 +13179,37 @@
             c = P, n(10, c), n(0, i);
         });
     }
     const k = () => {
         i.isPaused() && (i.resumeRecording(), i.stopRecording()), i.stopRecording();
     };
 
-    function C(P) {
+    function E(P) {
         ui[P ? "unshift" : "push"](() => {
             a = P, n(7, a), n(0, i);
         });
     }
     const y = () => i.pauseRecording();
 
-    function O(P) {
+    function H(P) {
         ui[P ? "unshift" : "push"](() => {
             l = P, n(8, l), n(0, i);
         });
     }
     const L = () => i.resumeRecording();
     return t.$$set = (P) => {
         "record" in P && n(0, i = P.record), "i18n" in P && n(1, o = P.i18n), "record_time" in P && n(2, f = P.record_time), "show_recording_waveform" in P && n(3, h = P.show_recording_waveform), "timing" in P && n(4, d = P.timing);
     }, t.$$.update = () => {
         if (t.$$.dirty & /*i18n*/
             2)
             try {
                 let P = [];
                 Mi.getAvailableAudioDevices().then((M) => {
-                    n(5, r = M), M.forEach((x) => {
-                        x.deviceId && P.push(x);
+                    n(5, r = M), M.forEach((Z) => {
+                        Z.deviceId && P.push(Z);
                     }), n(5, r = P);
                 });
             } catch (P) {
                 throw P instanceof DOMException && P.name == "NotAllowedError" && _("error", o("audio.allow_recording_access")), P;
             }
         t.$$.dirty & /*record*/
             1 && i.on("record-start", () => {
@@ -13226,21 +13234,21 @@
         s,
         a,
         l,
         u,
         c,
         m,
         v,
-        g,
+        b,
         S,
         w,
         k,
-        C,
+        E,
         y,
-        O,
+        H,
         L
     ];
 }
 class qg extends Sg {
     constructor(e) {
         super(), Rg(this, e, Fg, jg, Dg, {
             record: 0,
@@ -13257,26 +13265,26 @@
     append: at,
     attr: Ct,
     bind: oc,
     binding_callbacks: Bn,
     check_outros: Kl,
     create_component: rc,
     destroy_component: sc,
-    detach: Hi,
+    detach: Oi,
     element: At,
     group_outros: $l,
     init: Gg,
     insert: Ni,
     mount_component: lc,
     noop: ac,
     safe_not_equal: Wg,
     set_data: Vg,
     space: Mn,
     text: Xg,
-    transition_in: Ht,
+    transition_in: Ot,
     transition_out: Dn
 } = window.__gradio__svelte__internal, {
     onMount: xg
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: Zg
 } = window.__gradio__svelte__internal;
 
@@ -13302,15 +13310,15 @@
             Ni(c, e, f), at(e, n), t[19](n), at(e, i), at(e, o), s && s.m(o, null), at(o, r), u.m(o, null);
         },
         p(c, f) {
             /*mode*/
             c[0] === "edit" && es > 0 ? s ? s.p(c, f) : (s = ta(), s.c(), s.m(o, r)) : s && (s.d(1), s = null), l === (l = a(c)) && u ? u.p(c, f) : (u.d(1), u = l(c), u && (u.c(), u.m(o, null)));
         },
         d(c) {
-            c && Hi(e), t[19](null), s && s.d(), u.d();
+            c && Oi(e), t[19](null), s && s.d(), u.d();
         }
     };
 }
 
 function ta(t) {
     let e;
     return {
@@ -13318,15 +13326,15 @@
             e = At("time"), e.textContent = `${un(es)}`, Ct(e, "class", "trim-duration svelte-1z0uz8p");
         },
         m(n, i) {
             Ni(n, e, i);
         },
         p: ac,
         d(n) {
-            n && Hi(e);
+            n && Oi(e);
         }
     };
 }
 
 function Jg(t) {
     let e;
     return {
@@ -13334,15 +13342,15 @@
             e = At("time"), e.textContent = "0:00", Ct(e, "class", "duration svelte-1z0uz8p");
         },
         m(n, i) {
             Ni(n, e, i), t[20](e);
         },
         p: ac,
         d(n) {
-            n && Hi(e), t[20](null);
+            n && Oi(e), t[20](null);
         }
     };
 }
 
 function Yg(t) {
     let e, n = un(
             /*seconds*/
@@ -13360,15 +13368,15 @@
             r & /*seconds*/
                 4096 && n !== (n = un(
                     /*seconds*/
                     o[12]
                 ) + "") && Vg(i, n);
         },
         d(o) {
-            o && Hi(e);
+            o && Oi(e);
         }
     };
 }
 
 function na(t) {
     let e, n, i;
 
@@ -13418,15 +13426,15 @@
                         /*seconds*/
                         s[12]
                     )), !n && a & /*record*/
                     64 && (n = !0, l.record = /*record*/
                         s[6], ic(() => n = !1)), e.$set(l);
             },
             i(s) {
-                i || (Ht(e.$$.fragment, s), i = !0);
+                i || (Ot(e.$$.fragment, s), i = !0);
             },
             o(s) {
                 Dn(e.$$.fragment, s), i = !1;
             },
             d(s) {
                 sc(e, s);
             }
@@ -13481,15 +13489,15 @@
                         s[1]), a & /*waveform_options*/
                     4 && (l.waveform_options = /*waveform_options*/
                         s[2]), !n && a & /*recordingWaveform*/
                     8 && (n = !0, l.waveform = /*recordingWaveform*/
                         s[3], ic(() => n = !1)), e.$set(l);
             },
             i(s) {
-                i || (Ht(e.$$.fragment, s), i = !0);
+                i || (Ot(e.$$.fragment, s), i = !0);
             },
             o(s) {
                 Dn(e.$$.fragment, s), i = !1;
             },
             d(s) {
                 sc(e, s);
             }
@@ -13524,31 +13532,31 @@
         p(h, [d]) {
             /*timing*/
             (h[13] || /*recordedAudio*/
                 h[7]) && /*waveform_options*/
             h[2].show_recording_waveform ? u ? u.p(h, d) : (u = ea(h), u.c(), u.m(e, s)) : u && (u.d(1), u = null), /*microphoneContainer*/
                 h[5] && ! /*recordedAudio*/
                 h[7] ? c ? (c.p(h, d), d & /*microphoneContainer, recordedAudio*/
-                    160 && Ht(c, 1)) : (c = na(h), c.c(), Ht(c, 1), c.m(e, a)) : c && ($l(), Dn(c, 1, 1, () => {
+                    160 && Ot(c, 1)) : (c = na(h), c.c(), Ot(c, 1), c.m(e, a)) : c && ($l(), Dn(c, 1, 1, () => {
                     c = null;
                 }), Kl()), /*recordingWaveform*/
                 h[3] && /*recordedAudio*/
                 h[7] ? f ? (f.p(h, d), d & /*recordingWaveform, recordedAudio*/
-                    136 && Ht(f, 1)) : (f = ia(h), f.c(), Ht(f, 1), f.m(e, null)) : f && ($l(), Dn(f, 1, 1, () => {
+                    136 && Ot(f, 1)) : (f = ia(h), f.c(), Ot(f, 1), f.m(e, null)) : f && ($l(), Dn(f, 1, 1, () => {
                     f = null;
                 }), Kl());
         },
         i(h) {
-            l || (Ht(c), Ht(f), l = !0);
+            l || (Ot(c), Ot(f), l = !0);
         },
         o(h) {
             Dn(c), Dn(f), l = !1;
         },
         d(h) {
-            h && Hi(e), t[17](null), t[18](null), u && u.d(), c && c.d(), f && f.d();
+            h && Oi(e), t[17](null), t[18](null), u && u.d(), c && c.d(), f && f.d();
         }
     };
 }
 let es = 0;
 
 function mt(t) {
     let e, n = t[0],
@@ -13572,208 +13580,208 @@
         dispatch_blob: r
     } = e, {
         waveform_settings: s
     } = e, {
         waveform_options: a = {
             show_recording_waveform: !0
         }
-    } = e, l, u, c = !1, f, h, d, _ = null, m, v, g, S = 0, w, k = !1;
-    const C = () => {
+    } = e, l, u, c = !1, f, h, d, _ = null, m, v, b, S = 0, w, k = !1;
+    const E = () => {
             clearInterval(w), n(16, w = setInterval(
                 () => {
                     n(12, S++, S);
                 },
                 1e3
             ));
         },
         y = Zg(),
-        O = () => {
+        H = () => {
             h && n(5, h.innerHTML = "", h), l !== void 0 && l.destroy(), h && (l = Ft.create({
                 ...s,
                 normalize: !1,
                 container: h
             }), n(6, d = l.registerPlugin(Mi.create())), d.startMic());
         },
         L = () => {
-            let E = f;
-            !_ || !E || n(3, u = Ft.create({
-                container: E,
+            let C = f;
+            !_ || !C || n(3, u = Ft.create({
+                container: C,
                 url: _,
                 ...s
             }));
         };
     xg(() => {
-        O(), window.addEventListener("keydown", (E) => {
-            E.key === "ArrowRight" ? Qs(u, 0.1) : E.key === "ArrowLeft" && Qs(u, -0.1);
+        H(), window.addEventListener("keydown", (C) => {
+            C.key === "ArrowRight" ? Qs(u, 0.1) : C.key === "ArrowLeft" && Qs(u, -0.1);
         });
     });
 
-    function P(E) {
-        Bn[E ? "unshift" : "push"](() => {
-            h = E, n(5, h);
+    function P(C) {
+        Bn[C ? "unshift" : "push"](() => {
+            h = C, n(5, h);
         });
     }
 
-    function M(E) {
-        Bn[E ? "unshift" : "push"](() => {
-            f = E, n(4, f);
+    function M(C) {
+        Bn[C ? "unshift" : "push"](() => {
+            f = C, n(4, f);
         });
     }
 
-    function x(E) {
-        Bn[E ? "unshift" : "push"](() => {
-            m = E, n(8, m), n(3, u);
+    function Z(C) {
+        Bn[C ? "unshift" : "push"](() => {
+            m = C, n(8, m), n(3, u);
         });
     }
 
-    function Z(E) {
-        Bn[E ? "unshift" : "push"](() => {
-            v = E, n(9, v), n(3, u);
+    function x(C) {
+        Bn[C ? "unshift" : "push"](() => {
+            v = C, n(9, v), n(3, u);
         });
     }
 
-    function G(E) {
-        d = E, n(6, d);
+    function j(C) {
+        d = C, n(6, d);
     }
 
-    function X(E) {
-        u = E, n(3, u);
+    function X(C) {
+        u = C, n(3, u);
     }
-    return t.$$set = (E) => {
-        "mode" in E && n(0, i = E.mode), "i18n" in E && n(1, o = E.i18n), "dispatch_blob" in E && n(14, r = E.dispatch_blob), "waveform_settings" in E && n(15, s = E.waveform_settings), "waveform_options" in E && n(2, a = E.waveform_options);
+    return t.$$set = (C) => {
+        "mode" in C && n(0, i = C.mode), "i18n" in C && n(1, o = C.i18n), "dispatch_blob" in C && n(14, r = C.dispatch_blob), "waveform_settings" in C && n(15, s = C.waveform_settings), "waveform_options" in C && n(2, a = C.waveform_options);
     }, t.$$.update = () => {
         t.$$.dirty & /*record, waveform_options, microphoneContainer*/
             100 && mt([
                 d,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("record-start", () => {
-                    if (C(), n(13, k = !0), y("start_recording"), a.show_recording_waveform) {
-                        let F = h;
-                        F && (F.style.display = "block");
+                (C) => C("record-start", () => {
+                    if (E(), n(13, k = !0), y("start_recording"), a.show_recording_waveform) {
+                        let G = h;
+                        G && (G.style.display = "block");
                     }
                 })
             ]), t.$$.dirty & /*record, interval, waveform_settings, dispatch_blob*/
             114752 && mt([
                 d,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("record-end", async (F) => {
+                (C) => C("record-end", async (G) => {
                     n(12, S = 0), n(13, k = !1), clearInterval(w);
                     try {
-                        const N = await F.arrayBuffer(),
-                            $ = await new AudioContext({
+                        const I = await G.arrayBuffer(),
+                            K = await new AudioContext({
                                 sampleRate: s.sampleRate
-                            }).decodeAudioData(N);
-                        console.log($), $ && await V_($).then(async (H) => {
-                            await r([H], "change"), await r([H], "stop_recording");
+                            }).decodeAudioData(I);
+                        console.log(K), K && await V_(K).then(async (O) => {
+                            await r([O], "change"), await r([O], "stop_recording");
                         });
-                    } catch (N) {
-                        console.error(N);
+                    } catch (I) {
+                        console.error(I);
                     }
                 })
             ]), t.$$.dirty & /*record, interval*/
             65600 && mt([
                 d,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("record-pause", () => {
+                (C) => C("record-pause", () => {
                     y("pause_recording"), clearInterval(w);
                 })
             ]), t.$$.dirty & /*record*/
             64 && mt([
                 d,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("record-resume", () => {
-                    C();
+                (C) => C("record-resume", () => {
+                    E();
                 })
             ]), t.$$.dirty & /*recordingWaveform, durationRef*/
             520 && mt([
                 u,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("decode", (F) => {
-                    n(11, g = F), v && n(9, v.textContent = un(F), v);
+                (C) => C("decode", (G) => {
+                    n(11, b = G), v && n(9, v.textContent = un(G), v);
                 })
             ]), t.$$.dirty & /*recordingWaveform, timeRef*/
             264 && mt([
                 u,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("timeupdate", (F) => m && n(8, m.textContent = un(F), m))
+                (C) => C("timeupdate", (G) => m && n(8, m.textContent = un(G), m))
             ]), t.$$.dirty & /*recordingWaveform*/
             8 && mt([
                 u,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("pause", () => {
+                (C) => C("pause", () => {
                     y("pause"), n(10, c = !1);
                 })
             ]), t.$$.dirty & /*recordingWaveform*/
             8 && mt([
                 u,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("play", () => {
+                (C) => C("play", () => {
                     y("play"), n(10, c = !0);
                 })
             ]), t.$$.dirty & /*recordingWaveform*/
             8 && mt([
                 u,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("finish", () => {
+                (C) => C("finish", () => {
                     y("stop"), n(10, c = !1);
                 })
             ]), t.$$.dirty & /*record, microphoneContainer, recordingContainer, recordedAudio*/
             240 && mt([
                 d,
                 "optionalAccess",
-                (E) => E.on,
+                (C) => C.on,
                 "call",
-                (E) => E("record-end", (F) => {
-                    n(7, _ = URL.createObjectURL(F));
-                    const N = h,
-                        I = f;
-                    N && (N.style.display = "none"), I && _ && (I.innerHTML = "", L());
+                (C) => C("record-end", (G) => {
+                    n(7, _ = URL.createObjectURL(G));
+                    const I = h,
+                        U = f;
+                    I && (I.style.display = "none"), U && _ && (U.innerHTML = "", L());
                 })
             ]);
     }, [
         i,
         o,
         a,
         u,
         f,
         h,
         d,
         _,
         m,
         v,
         c,
-        g,
+        b,
         S,
         k,
         r,
         s,
         w,
         P,
         M,
-        x,
         Z,
-        G,
+        x,
+        j,
         X
     ];
 }
 class $g extends zg {
     constructor(e) {
         super(), Gg(this, e, Kg, Qg, Wg, {
             mode: 0,
@@ -13785,18 +13793,18 @@
     }
 }
 const {
     SvelteComponent: eb,
     append: an,
     attr: Nn,
     binding_callbacks: tb,
-    detach: Ro,
+    detach: Lo,
     element: qn,
     init: nb,
-    insert: Bo,
+    insert: Ro,
     listen: uc,
     noop: oa,
     null_to_empty: ra,
     safe_not_equal: ib,
     set_data: cc,
     set_style: sa,
     space: hs,
@@ -13813,27 +13821,27 @@
                 e,
                 "display",
                 /*recording*/
                 t[0] ? "block" : "none"
             );
         },
         m(n, i) {
-            Bo(n, e, i), t[9](e);
+            Ro(n, e, i), t[9](e);
         },
         p(n, i) {
             i & /*recording*/
                 1 && sa(
                     e,
                     "display",
                     /*recording*/
                     n[0] ? "block" : "none"
                 );
         },
         d(n) {
-            n && Ro(e), t[9](null);
+            n && Lo(e), t[9](null);
         }
     };
 }
 
 function rb(t) {
     let e, n, i, o = (
             /*i18n*/
@@ -13841,28 +13849,28 @@
         ),
         r, s, a;
     return {
         c() {
             e = qn("button"), n = qn("span"), n.innerHTML = '<span class="dot"></span>', i = hs(), r = fc(o), Nn(n, "class", "record-icon"), Nn(e, "class", "record-button svelte-4ycsjo");
         },
         m(l, u) {
-            Bo(l, e, u), an(e, n), an(e, i), an(e, r), s || (a = uc(
+            Ro(l, e, u), an(e, n), an(e, i), an(e, r), s || (a = uc(
                 e,
                 "click",
                 /*click_handler_1*/
                 t[11]
             ), s = !0);
         },
         p(l, u) {
             u & /*i18n*/
                 16 && o !== (o = /*i18n*/
                     l[4]("audio.record") + "") && cc(r, o);
         },
         d(l) {
-            l && Ro(e), s = !1, a();
+            l && Lo(e), s = !1, a();
         }
     };
 }
 
 function sb(t) {
     let e, n, i, o = (
             /*paused_recording*/
@@ -13879,15 +13887,15 @@
         c() {
             e = qn("button"), n = qn("span"), n.innerHTML = '<span class="pinger"></span> <span class="dot"></span>', i = hs(), r = fc(o), Nn(n, "class", "record-icon"), Nn(e, "class", s = ra(
                 /*paused_recording*/
                 t[1] ? "stop-button-paused" : "stop-button"
             ) + " svelte-4ycsjo");
         },
         m(u, c) {
-            Bo(u, e, c), an(e, n), an(e, i), an(e, r), a || (l = uc(
+            Ro(u, e, c), an(e, n), an(e, i), an(e, r), a || (l = uc(
                 e,
                 "click",
                 /*click_handler*/
                 t[10]
             ), a = !0);
         },
         p(u, c) {
@@ -13902,15 +13910,15 @@
                     )) + "") && cc(r, o), c & /*paused_recording*/
                 2 && s !== (s = ra(
                     /*paused_recording*/
                     u[1] ? "stop-button-paused" : "stop-button"
                 ) + " svelte-4ycsjo") && Nn(e, "class", s);
         },
         d(u) {
-            u && Ro(e), a = !1, l();
+            u && Lo(e), a = !1, l();
         }
     };
 }
 
 function lb(t) {
     let e, n, i = (
         /*waveform_options*/
@@ -13926,24 +13934,24 @@
     let r = o(t),
         s = r(t);
     return {
         c() {
             e = qn("div"), i && i.c(), n = hs(), s.c(), Nn(e, "class", "mic-wrap svelte-4ycsjo");
         },
         m(a, l) {
-            Bo(a, e, l), i && i.m(e, null), an(e, n), s.m(e, null);
+            Ro(a, e, l), i && i.m(e, null), an(e, n), s.m(e, null);
         },
         p(a, [l]) {
             /*waveform_options*/
             a[5].show_recording_waveform ? i ? i.p(a, l) : (i = la(a), i.c(), i.m(e, n)) : i && (i.d(1), i = null), r === (r = o(a)) && s ? s.p(a, l) : (s.d(1), s = r(a), s && (s.c(), s.m(e, null)));
         },
         i: oa,
         o: oa,
         d(a) {
-            a && Ro(e), i && i.d(), s.d();
+            a && Lo(e), i && i.d(), s.d();
         }
     };
 }
 
 function ab(t, e, n) {
     let {
         recording: i = !1
@@ -13969,27 +13977,27 @@
         c !== void 0 && c.destroy(), h && (c = Ft.create({
             ...l,
             height: 100,
             container: h
         }), n(6, f = c.registerPlugin(Mi.create())));
     };
 
-    function _(g) {
-        tb[g ? "unshift" : "push"](() => {
-            h = g, n(7, h);
+    function _(b) {
+        tb[b ? "unshift" : "push"](() => {
+            h = b, n(7, h);
         });
     }
     const m = () => {
             f == null || f.stopMic(), r();
         },
         v = () => {
             f == null || f.startMic(), s();
         };
-    return t.$$set = (g) => {
-        "recording" in g && n(0, i = g.recording), "paused_recording" in g && n(1, o = g.paused_recording), "stop" in g && n(2, r = g.stop), "record" in g && n(3, s = g.record), "i18n" in g && n(4, a = g.i18n), "waveform_settings" in g && n(8, l = g.waveform_settings), "waveform_options" in g && n(5, u = g.waveform_options);
+    return t.$$set = (b) => {
+        "recording" in b && n(0, i = b.recording), "paused_recording" in b && n(1, o = b.paused_recording), "stop" in b && n(2, r = b.stop), "record" in b && n(3, s = b.record), "i18n" in b && n(4, a = b.i18n), "waveform_settings" in b && n(8, l = b.waveform_settings), "waveform_options" in b && n(5, u = b.waveform_options);
     }, [
         i,
         o,
         r,
         s,
         a,
         u,
@@ -14012,34 +14020,34 @@
             waveform_settings: 8,
             waveform_options: 5
         });
     }
 }
 const {
     SvelteComponent: cb,
-    add_flush_callback: Mo,
-    bind: Do,
-    binding_callbacks: Oo,
-    bubble: Pr,
+    add_flush_callback: Bo,
+    bind: Mo,
+    binding_callbacks: Do,
+    bubble: Tr,
     check_outros: _s,
     create_component: qt,
     create_slot: fb,
     destroy_component: zt,
     detach: zn,
     empty: dc,
     get_all_dirty_from_scope: db,
     get_slot_changes: hb,
     group_outros: ms,
     init: _b,
     insert: Gn,
     mount_component: Gt,
     safe_not_equal: mb,
-    space: ho,
-    transition_in: Oe,
-    transition_out: He,
+    space: fo,
+    transition_in: He,
+    transition_out: Oe,
     update_slot_base: pb
 } = window.__gradio__svelte__internal, {
     getContext: gb,
     onDestroy: bb,
     createEventDispatcher: vb
 } = window.__gradio__svelte__internal;
 
@@ -14101,15 +14109,15 @@
         interactive: !0
     };
     return (
         /*mode*/
         t[14] !== void 0 && (a.mode = /*mode*/
             t[14]), i = new _u({
             props: a
-        }), Oo.push(() => Do(i, "mode", s)), i.$on(
+        }), Do.push(() => Mo(i, "mode", s)), i.$on(
             "stop",
             /*stop_handler*/
             t[31]
         ), i.$on(
             "play",
             /*play_handler*/
             t[32]
@@ -14119,15 +14127,15 @@
             t[33]
         ), i.$on(
             "edit",
             /*edit_handler_1*/
             t[34]
         ), {
             c() {
-                qt(e.$$.fragment), n = ho(), qt(i.$$.fragment);
+                qt(e.$$.fragment), n = fo(), qt(i.$$.fragment);
             },
             m(l, u) {
                 Gt(e, l, u), Gn(l, n, u), Gt(i, l, u), r = !0;
             },
             p(l, u) {
                 const c = {};
                 u[0] & /*i18n*/
@@ -14149,21 +14157,21 @@
                     1024 && (f.waveform_settings = /*waveform_settings*/
                         l[10]), u[0] & /*waveform_options*/
                     2048 && (f.waveform_options = /*waveform_options*/
                         l[11]), u[0] & /*editable*/
                     4096 && (f.editable = /*editable*/
                         l[12]), !o && u[0] & /*mode*/
                     16384 && (o = !0, f.mode = /*mode*/
-                        l[14], Mo(() => o = !1)), i.$set(f);
+                        l[14], Bo(() => o = !1)), i.$set(f);
             },
             i(l) {
-                r || (Oe(e.$$.fragment, l), Oe(i.$$.fragment, l), r = !0);
+                r || (He(e.$$.fragment, l), He(i.$$.fragment, l), r = !0);
             },
             o(l) {
-                He(e.$$.fragment, l), He(i.$$.fragment, l), r = !1;
+                Oe(e.$$.fragment, l), Oe(i.$$.fragment, l), r = !1;
             },
             d(l) {
                 l && zn(n), zt(e, l), zt(i, l);
             }
         }
     );
 }
@@ -14187,23 +14195,23 @@
             n && n.c(), i = dc();
         },
         m(l, u) {
             ~e && s[e].m(l, u), Gn(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
-            e = a(l), e === c ? ~e && s[e].p(l, u) : (n && (ms(), He(s[c], 1, 1, () => {
+            e = a(l), e === c ? ~e && s[e].p(l, u) : (n && (ms(), Oe(s[c], 1, 1, () => {
                 s[c] = null;
-            }), _s()), ~e ? (n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Oe(n, 1), n.m(i.parentNode, i)) : n = null);
+            }), _s()), ~e ? (n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), He(n, 1), n.m(i.parentNode, i)) : n = null);
         },
         i(l) {
-            o || (Oe(n), o = !0);
+            o || (He(n), o = !0);
         },
         o(l) {
-            He(n), o = !1;
+            Oe(n), o = !1;
         },
         d(l) {
             l && zn(i), ~e && s[e].d(l);
         }
     };
 }
 
@@ -14227,15 +14235,15 @@
         }
     };
     return (
         /*dragging*/
         t[0] !== void 0 && (r.dragging = /*dragging*/
             t[0]), e = new cg({
             props: r
-        }), Oo.push(() => Do(e, "dragging", o)), e.$on(
+        }), Do.push(() => Mo(e, "dragging", o)), e.$on(
             "load",
             /*handle_load*/
             t[19]
         ), e.$on(
             "error",
             /*error_handler*/
             t[28]
@@ -14252,21 +14260,21 @@
                     16 && (l.root = /*root*/
                         s[4]), a[1] & /*$$scope*/
                     32 && (l.$$scope = {
                         dirty: a,
                         ctx: s
                     }), !n && a[0] & /*dragging*/
                     1 && (n = !0, l.dragging = /*dragging*/
-                        s[0], Mo(() => n = !1)), e.$set(l);
+                        s[0], Bo(() => n = !1)), e.$set(l);
             },
             i(s) {
-                i || (Oe(e.$$.fragment, s), i = !0);
+                i || (He(e.$$.fragment, s), i = !0);
             },
             o(s) {
-                He(e.$$.fragment, s), i = !1;
+                Oe(e.$$.fragment, s), i = !1;
             },
             d(s) {
                 zt(e, s);
             }
         }
     );
 }
@@ -14293,34 +14301,34 @@
         return (
             /*streaming*/
             c[8] ? 0 : 1
         );
     }
     return i = u(t), o = l[i] = a[i](t), {
         c() {
-            qt(e.$$.fragment), n = ho(), o.c(), r = dc();
+            qt(e.$$.fragment), n = fo(), o.c(), r = dc();
         },
         m(c, f) {
             Gt(e, c, f), Gn(c, n, f), l[i].m(c, f), Gn(c, r, f), s = !0;
         },
         p(c, f) {
             const h = {};
             f[0] & /*i18n*/
                 512 && (h.i18n = /*i18n*/
                     c[9]), e.$set(h);
             let d = i;
-            i = u(c), i === d ? l[i].p(c, f) : (ms(), He(l[d], 1, 1, () => {
+            i = u(c), i === d ? l[i].p(c, f) : (ms(), Oe(l[d], 1, 1, () => {
                 l[d] = null;
-            }), _s(), o = l[i], o ? o.p(c, f) : (o = l[i] = a[i](c), o.c()), Oe(o, 1), o.m(r.parentNode, r));
+            }), _s(), o = l[i], o ? o.p(c, f) : (o = l[i] = a[i](c), o.c()), He(o, 1), o.m(r.parentNode, r));
         },
         i(c) {
-            s || (Oe(e.$$.fragment, c), Oe(o), s = !0);
+            s || (He(e.$$.fragment, c), He(o), s = !0);
         },
         o(c) {
-            He(e.$$.fragment, c), He(o), s = !1;
+            Oe(e.$$.fragment, c), Oe(o), s = !1;
         },
         d(c) {
             c && (zn(n), zn(r)), zt(e, c), l[i].d(c);
         }
     };
 }
 
@@ -14362,18 +14370,18 @@
                     /*$$scope*/
                     o[36]
                 ),
                 null
             );
         },
         i(o) {
-            e || (Oe(i, o), e = !0);
+            e || (He(i, o), e = !0);
         },
         o(o) {
-            He(i, o), e = !1;
+            Oe(i, o), e = !1;
         },
         d(o) {
             i && i.d(o);
         }
     };
 }
 
@@ -14402,15 +14410,15 @@
         )
     };
     return (
         /*mode*/
         t[14] !== void 0 && (r.mode = /*mode*/
             t[14]), e = new $g({
             props: r
-        }), Oo.push(() => Do(e, "mode", o)), {
+        }), Do.push(() => Mo(e, "mode", o)), {
             c() {
                 qt(e.$$.fragment);
             },
             m(s, a) {
                 Gt(e, s, a), i = !0;
             },
             p(s, a) {
@@ -14419,21 +14427,21 @@
                     512 && (l.i18n = /*i18n*/
                         s[9]), a[0] & /*waveform_settings*/
                     1024 && (l.waveform_settings = /*waveform_settings*/
                         s[10]), a[0] & /*waveform_options*/
                     2048 && (l.waveform_options = /*waveform_options*/
                         s[11]), !n && a[0] & /*mode*/
                     16384 && (n = !0, l.mode = /*mode*/
-                        s[14], Mo(() => n = !1)), e.$set(l);
+                        s[14], Bo(() => n = !1)), e.$set(l);
             },
             i(s) {
-                i || (Oe(e.$$.fragment, s), i = !0);
+                i || (He(e.$$.fragment, s), i = !0);
             },
             o(s) {
-                He(e.$$.fragment, s), i = !1;
+                Oe(e.$$.fragment, s), i = !1;
             },
             d(s) {
                 zt(e, s);
             }
         }
     );
 }
@@ -14483,18 +14491,18 @@
                     i[9]), o[0] & /*waveform_settings*/
                 1024 && (r.waveform_settings = /*waveform_settings*/
                     i[10]), o[0] & /*waveform_options*/
                 2048 && (r.waveform_options = /*waveform_options*/
                     i[11]), e.$set(r);
         },
         i(i) {
-            n || (Oe(e.$$.fragment, i), n = !0);
+            n || (He(e.$$.fragment, i), n = !0);
         },
         o(i) {
-            He(e.$$.fragment, i), n = !1;
+            Oe(e.$$.fragment, i), n = !1;
         },
         d(i) {
             zt(e, i);
         }
     };
 }
 
@@ -14502,15 +14510,15 @@
     let e, n, i, o, r, s, a, l;
     e = new Ia({
         props: {
             show_label: (
                 /*show_label*/
                 t[5]
             ),
-            Icon: po,
+            Icon: mo,
             float: (
                 /*active_source*/
                 t[2] === "upload" && /*value*/
                 t[1] === null
             ),
             label: (
                 /*label*/
@@ -14545,17 +14553,17 @@
         )
     };
     return (
         /*active_source*/
         t[2] !== void 0 && (d.active_source = /*active_source*/
             t[2]), s = new y_({
             props: d
-        }), Oo.push(() => Do(s, "active_source", h)), {
+        }), Do.push(() => Mo(s, "active_source", h)), {
             c() {
-                qt(e.$$.fragment), n = ho(), o.c(), r = ho(), qt(s.$$.fragment);
+                qt(e.$$.fragment), n = fo(), o.c(), r = fo(), qt(s.$$.fragment);
             },
             m(_, m) {
                 Gt(e, _, m), Gn(_, n, m), c[i].m(_, m), Gn(_, r, m), Gt(s, _, m), l = !0;
             },
             p(_, m) {
                 const v = {};
                 m[0] & /*show_label*/
@@ -14563,30 +14571,30 @@
                         _[5]), m[0] & /*active_source, value*/
                     6 && (v.float = /*active_source*/
                         _[2] === "upload" && /*value*/
                         _[1] === null), m[0] & /*label, i18n*/
                     520 && (v.label = /*label*/
                         _[3] || /*i18n*/
                         _[9]("audio.audio")), e.$set(v);
-                let g = i;
-                i = f(_), i === g ? c[i].p(_, m) : (ms(), He(c[g], 1, 1, () => {
-                    c[g] = null;
-                }), _s(), o = c[i], o ? o.p(_, m) : (o = c[i] = u[i](_), o.c()), Oe(o, 1), o.m(r.parentNode, r));
+                let b = i;
+                i = f(_), i === b ? c[i].p(_, m) : (ms(), Oe(c[b], 1, 1, () => {
+                    c[b] = null;
+                }), _s(), o = c[i], o ? o.p(_, m) : (o = c[i] = u[i](_), o.c()), He(o, 1), o.m(r.parentNode, r));
                 const S = {};
                 m[0] & /*sources*/
                     128 && (S.sources = /*sources*/
                         _[7]), !a && m[0] & /*active_source*/
                     4 && (a = !0, S.active_source = /*active_source*/
-                        _[2], Mo(() => a = !1)), s.$set(S);
+                        _[2], Bo(() => a = !1)), s.$set(S);
             },
             i(_) {
-                l || (Oe(e.$$.fragment, _), Oe(o), Oe(s.$$.fragment, _), l = !0);
+                l || (He(e.$$.fragment, _), He(o), He(s.$$.fragment, _), l = !0);
             },
             o(_) {
-                He(e.$$.fragment, _), He(o), He(s.$$.fragment, _), l = !1;
+                Oe(e.$$.fragment, _), Oe(o), Oe(s.$$.fragment, _), l = !1;
             },
             d(_) {
                 _ && (zn(n), zn(r)), zt(e, _), c[i].d(_), zt(s, _);
             }
         }
     );
 }
@@ -14630,51 +14638,51 @@
     } = e, {
         waveform_settings: _
     } = e, {
         waveform_options: m = {}
     } = e, {
         dragging: v
     } = e, {
-        active_source: g
+        active_source: b
     } = e, {
         editable: S = !0
     } = e;
     const w = gb("upload_files");
     let k = !1,
-        C, y = "",
-        O, L = [],
+        E, y = "",
+        H, L = [],
         P = !1,
         M = !1,
-        x = [],
-        Z;
+        Z = [],
+        x;
 
-    function G() {
-        Z = [
+    function j() {
+        x = [
             import("./module-d82531d9.js"),
             import("./module-aafe8b06.js")
         ];
     }
-    h && G();
+    h && j();
     const X = vb(),
-        E = async (R, ce) => {
+        C = async (R, ce) => {
             let Se = new File(R, "audio.wav");
             const wt = await Ba([Se], ce === "stream");
             let Y = (await Lb([
                 await Ra(wt, a, void 0, w),
                 "optionalAccess",
                 async (yt) => yt.filter,
                     "call",
                     async (yt) => yt(Boolean)
             ]))[0];
             r === null ? n(1, r = new Cs(Y)) : n(1, r.file_data = Y, r), X(ce, r);
         };
     bb(() => {
-        h && C && C.state !== "inactive" && C.stop();
+        h && E && E.state !== "inactive" && E.stop();
     });
-    async function F() {
+    async function G() {
         let R;
         try {
             R = await navigator.mediaDevices.getUserMedia({
                 audio: !0
             });
         } catch (ce) {
             if (!navigator.mediaDevices) {
@@ -14690,132 +14698,132 @@
         if (R != null) {
             if (h) {
                 const [{
                     MediaRecorder: ce,
                     register: Se
                 }, {
                     connect: wt
-                }] = await Promise.all(Z);
-                await Se(await wt()), C = new ce(R, {
+                }] = await Promise.all(x);
+                await Se(await wt()), E = new ce(R, {
                     mimeType: "audio/wav"
-                }), C.addEventListener("dataavailable", N);
+                }), E.addEventListener("dataavailable", I);
             } else
-                C = new MediaRecorder(R), C.addEventListener("dataavailable", (ce) => {
-                    x.push(ce.data);
-                }), C.addEventListener("stop", async () => {
-                    n(13, k = !1), await E(x, "change"), await E(x, "stop_recording"), x = [];
+                E = new MediaRecorder(R), E.addEventListener("dataavailable", (ce) => {
+                    Z.push(ce.data);
+                }), E.addEventListener("stop", async () => {
+                    n(13, k = !1), await C(Z, "change"), await C(Z, "stop_recording"), Z = [];
                 });
             M = !0;
         }
     }
-    async function N(R) {
+    async function I(R) {
         let ce = await R.data.arrayBuffer(),
             Se = new Uint8Array(ce);
-        if (O || (n(22, O = new Uint8Array(ce.slice(0, aa))), Se = new Uint8Array(ce.slice(aa))), f)
+        if (H || (n(22, H = new Uint8Array(ce.slice(0, aa))), Se = new Uint8Array(ce.slice(aa))), f)
             L.push(Se);
         else {
-            let wt = [O].concat(L, [Se]);
-            E(wt, "stream"), n(23, L = []);
+            let wt = [H].concat(L, [Se]);
+            C(wt, "stream"), n(23, L = []);
         }
     }
-    async function I() {
-        n(13, k = !0), X("start_recording"), M || await F(), n(22, O = void 0), h && C.start(Pb);
+    async function U() {
+        n(13, k = !0), X("start_recording"), M || await G(), n(22, H = void 0), h && E.start(Pb);
     }
 
-    function $() {
+    function K() {
         X("change", null), X("clear"), n(14, y = ""), n(1, r = null);
     }
 
-    function H({
+    function O({
         detail: R
     }) {
         n(1, r = new Cs(R)), X("change", r), X("upload", R);
     }
 
     function J() {
-        n(13, k = !1), h && (X("stop_recording"), C.stop(), f && n(24, P = !0), E(x, "stop_recording"), X("clear"), n(14, y = ""));
+        n(13, k = !1), h && (X("stop_recording"), E.stop(), f && n(24, P = !0), C(Z, "stop_recording"), X("clear"), n(14, y = ""));
     }
 
-    function ee(R) {
+    function le(R) {
         y = R, n(14, y);
     }
 
     function p(R) {
         v = R, n(0, v);
     }
-    const T = ({
+    const A = ({
             detail: R
         }) => X("error", R),
         q = () => n(14, y = "edit");
 
     function z(R) {
         y = R, n(14, y);
     }
 
-    function _e(R) {
-        Pr.call(this, t, R);
+    function he(R) {
+        Tr.call(this, t, R);
     }
 
-    function me(R) {
-        Pr.call(this, t, R);
+    function _e(R) {
+        Tr.call(this, t, R);
     }
 
-    function U(R) {
-        Pr.call(this, t, R);
+    function F(R) {
+        Tr.call(this, t, R);
     }
-    const Ce = (R) => X("edit", R.detail);
+    const ve = (R) => X("edit", R.detail);
 
     function B(R) {
-        g = R, n(2, g);
+        b = R, n(2, b);
     }
     return t.$$set = (R) => {
-        "value" in R && n(1, r = R.value), "label" in R && n(3, s = R.label), "root" in R && n(4, a = R.root), "show_label" in R && n(5, l = R.show_label), "show_download_button" in R && n(6, u = R.show_download_button), "sources" in R && n(7, c = R.sources), "pending" in R && n(21, f = R.pending), "streaming" in R && n(8, h = R.streaming), "i18n" in R && n(9, d = R.i18n), "waveform_settings" in R && n(10, _ = R.waveform_settings), "waveform_options" in R && n(11, m = R.waveform_options), "dragging" in R && n(0, v = R.dragging), "active_source" in R && n(2, g = R.active_source), "editable" in R && n(12, S = R.editable), "$$scope" in R && n(36, o = R.$$scope);
+        "value" in R && n(1, r = R.value), "label" in R && n(3, s = R.label), "root" in R && n(4, a = R.root), "show_label" in R && n(5, l = R.show_label), "show_download_button" in R && n(6, u = R.show_download_button), "sources" in R && n(7, c = R.sources), "pending" in R && n(21, f = R.pending), "streaming" in R && n(8, h = R.streaming), "i18n" in R && n(9, d = R.i18n), "waveform_settings" in R && n(10, _ = R.waveform_settings), "waveform_options" in R && n(11, m = R.waveform_options), "dragging" in R && n(0, v = R.dragging), "active_source" in R && n(2, b = R.active_source), "editable" in R && n(12, S = R.editable), "$$scope" in R && n(36, o = R.$$scope);
     }, t.$$.update = () => {
         if (t.$$.dirty[0] & /*dragging*/
             1 && X("drag", v), t.$$.dirty[0] & /*submit_pending_stream_on_pending_end, pending, header, pending_stream*/
-            31457280 && P && f === !1 && (n(24, P = !1), O && L)) {
-            let R = [O].concat(L);
-            n(23, L = []), E(R, "stream");
+            31457280 && P && f === !1 && (n(24, P = !1), H && L)) {
+            let R = [H].concat(L);
+            n(23, L = []), C(R, "stream");
         }
     }, [
         v,
         r,
-        g,
+        b,
         s,
         a,
         l,
         u,
         c,
         h,
         d,
         _,
         m,
         S,
         k,
         y,
         X,
-        E,
-        I,
-        $,
-        H,
+        C,
+        U,
+        K,
+        O,
         J,
         f,
-        O,
+        H,
         L,
         P,
         i,
-        ee,
+        le,
         p,
-        T,
+        A,
         q,
         z,
+        he,
         _e,
-        me,
-        U,
-        Ce,
+        F,
+        ve,
         B,
         o
     ];
 }
 class Bb extends cb {
     constructor(e) {
         super(), _b(
@@ -14841,49 +14849,49 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 
-function On(t) {
+function Hn(t) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         n = 0;
     for (; t > 1e3 && n < e.length - 1;)
         t /= 1e3, n++;
     let i = e[n];
     return (Number.isInteger(t) ? t : t.toFixed(1)) + i;
 }
 const {
     SvelteComponent: Mb,
     append: it,
-    attr: te,
+    attr: ee,
     component_subscribe: ua,
     detach: Db,
-    element: Ob,
-    init: Hb,
+    element: Hb,
+    init: Ob,
     insert: Nb,
     noop: ca,
     safe_not_equal: Ib,
     set_style: Ji,
     svg_element: ot,
     toggle_class: fa
 } = window.__gradio__svelte__internal, {
     onMount: Ub
 } = window.__gradio__svelte__internal;
 
 function jb(t) {
     let e, n, i, o, r, s, a, l, u, c, f, h;
     return {
         c() {
-            e = Ob("div"), n = ot("svg"), i = ot("g"), o = ot("path"), r = ot("path"), s = ot("path"), a = ot("path"), l = ot("g"), u = ot("path"), c = ot("path"), f = ot("path"), h = ot("path"), te(o, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), te(o, "fill", "#FF7C00"), te(o, "fill-opacity", "0.4"), te(o, "class", "svelte-43sxxs"), te(r, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), te(r, "fill", "#FF7C00"), te(r, "class", "svelte-43sxxs"), te(s, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), te(s, "fill", "#FF7C00"), te(s, "fill-opacity", "0.4"), te(s, "class", "svelte-43sxxs"), te(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), te(a, "fill", "#FF7C00"), te(a, "class", "svelte-43sxxs"), Ji(i, "transform", "translate(" + /*$top*/
+            e = Hb("div"), n = ot("svg"), i = ot("g"), o = ot("path"), r = ot("path"), s = ot("path"), a = ot("path"), l = ot("g"), u = ot("path"), c = ot("path"), f = ot("path"), h = ot("path"), ee(o, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), ee(o, "fill", "#FF7C00"), ee(o, "fill-opacity", "0.4"), ee(o, "class", "svelte-43sxxs"), ee(r, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), ee(r, "fill", "#FF7C00"), ee(r, "class", "svelte-43sxxs"), ee(s, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), ee(s, "fill", "#FF7C00"), ee(s, "fill-opacity", "0.4"), ee(s, "class", "svelte-43sxxs"), ee(a, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), ee(a, "fill", "#FF7C00"), ee(a, "class", "svelte-43sxxs"), Ji(i, "transform", "translate(" + /*$top*/
                 t[1][0] + "px, " + /*$top*/
-                t[1][1] + "px)"), te(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), te(u, "fill", "#FF7C00"), te(u, "fill-opacity", "0.4"), te(u, "class", "svelte-43sxxs"), te(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), te(c, "fill", "#FF7C00"), te(c, "class", "svelte-43sxxs"), te(f, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), te(f, "fill", "#FF7C00"), te(f, "fill-opacity", "0.4"), te(f, "class", "svelte-43sxxs"), te(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), te(h, "fill", "#FF7C00"), te(h, "class", "svelte-43sxxs"), Ji(l, "transform", "translate(" + /*$bottom*/
+                t[1][1] + "px)"), ee(u, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), ee(u, "fill", "#FF7C00"), ee(u, "fill-opacity", "0.4"), ee(u, "class", "svelte-43sxxs"), ee(c, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), ee(c, "fill", "#FF7C00"), ee(c, "class", "svelte-43sxxs"), ee(f, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), ee(f, "fill", "#FF7C00"), ee(f, "fill-opacity", "0.4"), ee(f, "class", "svelte-43sxxs"), ee(h, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), ee(h, "fill", "#FF7C00"), ee(h, "class", "svelte-43sxxs"), Ji(l, "transform", "translate(" + /*$bottom*/
                 t[2][0] + "px, " + /*$bottom*/
-                t[2][1] + "px)"), te(n, "viewBox", "-1200 -1200 3000 3000"), te(n, "fill", "none"), te(n, "xmlns", "http://www.w3.org/2000/svg"), te(n, "class", "svelte-43sxxs"), te(e, "class", "svelte-43sxxs"), fa(
+                t[2][1] + "px)"), ee(n, "viewBox", "-1200 -1200 3000 3000"), ee(n, "fill", "none"), ee(n, "xmlns", "http://www.w3.org/2000/svg"), ee(n, "class", "svelte-43sxxs"), ee(e, "class", "svelte-43sxxs"), fa(
                 e,
                 "margin",
                 /*margin*/
                 t[0]
             );
         },
         m(d, _) {
@@ -14932,15 +14940,15 @@
     }
     return Ub(() => (f(), () => l = !0)), t.$$set = (h) => {
         "margin" in h && n(0, r = h.margin);
     }, [r, i, o, s, a];
 }
 class qb extends Mb {
     constructor(e) {
-        super(), Hb(this, e, Fb, jb, Ib, {
+        super(), Ob(this, e, Fb, jb, Ib, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: zb,
     append: rn,
@@ -14950,15 +14958,15 @@
     create_component: Gb,
     create_slot: Wb,
     destroy_component: Vb,
     destroy_each: _c,
     detach: W,
     element: St,
     empty: $n,
-    ensure_array_like: _o,
+    ensure_array_like: ho,
     get_all_dirty_from_scope: Xb,
     get_slot_changes: xb,
     group_outros: mc,
     init: Zb,
     insert: V,
     mount_component: Jb,
     noop: ts,
@@ -14971,27 +14979,27 @@
     transition_in: Wn,
     transition_out: Vn,
     update_slot_base: Qb
 } = window.__gradio__svelte__internal, {
     tick: Kb
 } = window.__gradio__svelte__internal, {
     onDestroy: $b
-} = window.__gradio__svelte__internal, e2 = (t) => ({}), ha = (t) => ({});
+} = window.__gradio__svelte__internal, ev = (t) => ({}), ha = (t) => ({});
 
 function _a(t, e, n) {
     const i = t.slice();
     return i[38] = e[n], i[40] = n, i;
 }
 
 function ma(t, e, n) {
     const i = t.slice();
     return i[38] = e[n], i;
 }
 
-function t2(t) {
+function tv(t) {
     let e, n = (
             /*i18n*/
             t[1]("common.error") + ""
         ),
         i, o, r;
     const s = (
             /*#slots*/
@@ -15022,15 +15030,15 @@
                 /*$$scope*/
                 l[28],
                 r ? xb(
                     s,
                     /*$$scope*/
                     l[28],
                     u,
-                    e2
+                    ev
                 ) : Xb(
                     /*$$scope*/
                     l[28]
                 ),
                 ha
             );
         },
@@ -15042,60 +15050,60 @@
         },
         d(l) {
             l && (W(e), W(o)), a && a.d(l);
         }
     };
 }
 
-function n2(t) {
+function nv(t) {
     let e, n, i, o, r, s, a, l, u, c = (
         /*variant*/
         t[8] === "default" && /*show_eta_bar*/
         t[18] && /*show_progress*/
         t[6] === "full" && pa(t)
     );
 
     function f(w, k) {
         if (
             /*progress*/
             w[7]
         )
-            return r2;
+            return rv;
         if (
             /*queue_position*/
             w[2] !== null && /*queue_size*/
             w[3] !== void 0 && /*queue_position*/
             w[2] >= 0
         )
-            return o2;
+            return ov;
         if (
             /*queue_position*/
             w[2] === 0
         )
-            return i2;
+            return iv;
     }
     let h = f(t),
         d = h && h(t),
         _ = (
             /*timer*/
             t[5] && va(t)
         );
-    const m = [u2, a2],
+    const m = [uv, av],
         v = [];
 
-    function g(w, k) {
+    function b(w, k) {
         return (
             /*last_progress_level*/
             w[15] != null ? 0 : (
                 /*show_progress*/
                 w[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(r = g(t)) && (s = v[r] = m[r](t));
+    ~(r = b(t)) && (s = v[r] = m[r](t));
     let S = ! /*timer*/
         t[5] && Aa(t);
     return {
         c() {
             c && c.c(), e = bt(), n = St("div"), d && d.c(), i = bt(), _ && _.c(), o = bt(), s && s.c(), a = bt(), S && S.c(), l = $n(), gt(n, "class", "progress-text svelte-1yserjw"), Qe(
                 n,
                 "meta-text-center",
@@ -15125,17 +15133,17 @@
                 ), (!u || k[0] & /*variant*/
                     256) && Qe(
                     n,
                     "meta-text",
                     /*variant*/
                     w[8] === "default"
                 );
-            let C = r;
-            r = g(w), r === C ? ~r && v[r].p(w, k) : (s && (mc(), Vn(v[C], 1, 1, () => {
-                    v[C] = null;
+            let E = r;
+            r = b(w), r === E ? ~r && v[r].p(w, k) : (s && (mc(), Vn(v[E], 1, 1, () => {
+                    v[E] = null;
                 }), hc()), ~r ? (s = v[r], s ? s.p(w, k) : (s = v[r] = m[r](w), s.c()), Wn(s, 1), s.m(a.parentNode, a)) : s = null), /*timer*/
                 w[5] ? S && (S.d(1), S = null) : S ? S.p(w, k) : (S = Aa(w), S.c(), S.m(l.parentNode, l));
         },
         i(w) {
             u || (Wn(s), u = !0);
         },
         o(w) {
@@ -15164,15 +15172,15 @@
         },
         d(i) {
             i && W(e);
         }
     };
 }
 
-function i2(t) {
+function iv(t) {
     let e;
     return {
         c() {
             e = de("processing |");
         },
         m(n, i) {
             V(n, e, i);
@@ -15180,15 +15188,15 @@
         p: ts,
         d(n) {
             n && W(e);
         }
     };
 }
 
-function o2(t) {
+function ov(t) {
     let e, n = (
             /*queue_position*/
             t[2] + 1 + ""
         ),
         i, o, r, s;
     return {
         c() {
@@ -15212,16 +15220,16 @@
         },
         d(a) {
             a && (W(e), W(i), W(o), W(r), W(s));
         }
     };
 }
 
-function r2(t) {
-    let e, n = _o(
+function rv(t) {
+    let e, n = ho(
             /*progress*/
             t[7]
         ),
         i = [];
     for (let o = 0; o < n.length; o += 1)
         i[o] = ba(ma(t, n, o));
     return {
@@ -15234,15 +15242,15 @@
             for (let s = 0; s < i.length; s += 1)
                 i[s] && i[s].m(o, r);
             V(o, e, r);
         },
         p(o, r) {
             if (r[0] & /*progress*/
                 128) {
-                n = _o(
+                n = ho(
                     /*progress*/
                     o[7]
                 );
                 let s;
                 for (s = 0; s < n.length; s += 1) {
                     const a = ma(o, n, s);
                     i[s] ? i[s].p(a, r) : (i[s] = ba(a), i[s].c(), i[s].m(e.parentNode, e));
@@ -15265,15 +15273,15 @@
         ),
         i, o, r = " ",
         s;
 
     function a(c, f) {
         return (
             /*p*/
-            c[38].length != null ? l2 : s2
+            c[38].length != null ? lv : sv
         );
     }
     let l = a(t),
         u = l(t);
     return {
         c() {
             u.c(), e = bt(), i = de(n), o = de(" | "), s = de(r);
@@ -15288,64 +15296,64 @@
         },
         d(c) {
             c && (W(e), W(i), W(o), W(s)), u.d(c);
         }
     };
 }
 
-function s2(t) {
-    let e = On(
+function sv(t) {
+    let e = Hn(
             /*p*/
             t[38].index || 0
         ) + "",
         n;
     return {
         c() {
             n = de(e);
         },
         m(i, o) {
             V(i, n, o);
         },
         p(i, o) {
             o[0] & /*progress*/
-                128 && e !== (e = On(
+                128 && e !== (e = Hn(
                     /*p*/
                     i[38].index || 0
                 ) + "") && $e(n, e);
         },
         d(i) {
             i && W(n);
         }
     };
 }
 
-function l2(t) {
-    let e = On(
+function lv(t) {
+    let e = Hn(
             /*p*/
             t[38].index || 0
         ) + "",
-        n, i, o = On(
+        n, i, o = Hn(
             /*p*/
             t[38].length
         ) + "",
         r;
     return {
         c() {
             n = de(e), i = de("/"), r = de(o);
         },
         m(s, a) {
             V(s, n, a), V(s, i, a), V(s, r, a);
         },
         p(s, a) {
             a[0] & /*progress*/
-                128 && e !== (e = On(
+                128 && e !== (e = Hn(
                     /*p*/
                     s[38].index || 0
                 ) + "") && $e(n, e), a[0] & /*progress*/
-                128 && o !== (o = On(
+                128 && o !== (o = Hn(
                     /*p*/
                     s[38].length
                 ) + "") && $e(r, o);
         },
         d(s) {
             s && (W(n), W(i), W(r));
         }
@@ -15404,15 +15412,15 @@
         },
         d(r) {
             r && (W(e), W(i), W(o));
         }
     };
 }
 
-function a2(t) {
+function av(t) {
     let e, n;
     return e = new qb({
         props: {
             margin: (
                 /*variant*/
                 t[8] === "default"
             )
@@ -15438,15 +15446,15 @@
         },
         d(i) {
             Vb(e, i);
         }
     };
 }
 
-function u2(t) {
+function uv(t) {
     let e, n, i, o, r, s = `${/*last_progress_level*/
   t[15] * 100}%`,
         a = (
             /*progress*/
             t[7] != null && wa(t)
         );
     return {
@@ -15467,15 +15475,15 @@
         d(l) {
             l && W(e), a && a.d(), t[30](null);
         }
     };
 }
 
 function wa(t) {
-    let e, n = _o(
+    let e, n = ho(
             /*progress*/
             t[7]
         ),
         i = [];
     for (let o = 0; o < n.length; o += 1)
         i[o] = Sa(_a(t, n, o));
     return {
@@ -15488,15 +15496,15 @@
             for (let s = 0; s < i.length; s += 1)
                 i[s] && i[s].m(o, r);
             V(o, e, r);
         },
         p(o, r) {
             if (r[0] & /*progress_level, progress*/
                 16512) {
-                n = _o(
+                n = ho(
                     /*progress*/
                     o[7]
                 );
                 let s;
                 for (s = 0; s < n.length; s += 1) {
                     const a = _a(o, n, s);
                     i[s] ? i[s].p(a, r) : (i[s] = Sa(a), i[s].c(), i[s].m(e.parentNode, e));
@@ -15511,15 +15519,15 @@
         }
     };
 }
 
 function ya(t) {
     let e, n, i, o, r = (
             /*i*/
-            t[40] !== 0 && c2()
+            t[40] !== 0 && cv()
         ),
         s = (
             /*p*/
             t[38].desc != null && ka(t)
         ),
         a = (
             /*p*/
@@ -15554,15 +15562,15 @@
         },
         d(u) {
             u && (W(e), W(n), W(i), W(o)), r && r.d(u), s && s.d(u), a && a.d(u), l && l.d(u);
         }
     };
 }
 
-function c2(t) {
+function cv(t) {
     let e;
     return {
         c() {
             e = de(" /");
         },
         m(n, i) {
             V(n, e, i);
@@ -15694,17 +15702,17 @@
         },
         d(i) {
             i && W(e);
         }
     };
 }
 
-function f2(t) {
+function fv(t) {
     let e, n, i, o, r;
-    const s = [n2, t2],
+    const s = [nv, tv],
         a = [];
 
     function l(u, c) {
         return (
             /*status*/
             u[4] === "pending" ? 0 : (
                 /*status*/
@@ -15808,36 +15816,36 @@
         },
         d(u) {
             u && W(e), ~n && a[n].d(), t[31](null);
         }
     };
 }
 let Yi = [],
-    Lr = !1;
-async function d2(t, e = !0) {
+    Pr = !1;
+async function dv(t, e = !0) {
     if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && e !== !0)) {
-        if (Yi.push(t), !Lr)
-            Lr = !0;
+        if (Yi.push(t), !Pr)
+            Pr = !0;
         else
             return;
         await Kb(), requestAnimationFrame(() => {
             let n = [0, 0];
             for (let i = 0; i < Yi.length; i++) {
                 const r = Yi[i].getBoundingClientRect();
                 (i === 0 || r.top + window.scrollY <= n[0]) && (n[0] = r.top + window.scrollY, n[1] = i);
             }
             window.scrollTo({
                 top: n[0] - 20,
                 behavior: "smooth"
-            }), Lr = !1, Yi = [];
+            }), Pr = !1, Yi = [];
         });
     }
 }
 
-function h2(t, e, n) {
+function hv(t, e, n) {
     let i, {
             $$slots: o = {},
             $$scope: r
         } = e,
         {
             i18n: s
         } = e,
@@ -15868,125 +15876,125 @@
         {
             progress: m = null
         } = e,
         {
             variant: v = "default"
         } = e,
         {
-            loading_text: g = "Loading..."
+            loading_text: b = "Loading..."
         } = e,
         {
             absolute: S = !0
         } = e,
         {
             translucent: w = !1
         } = e,
         {
             border: k = !1
         } = e,
         {
-            autoscroll: C
+            autoscroll: E
         } = e,
-        y, O = !1,
+        y, H = !1,
         L = 0,
         P = 0,
         M = null,
-        x = null,
-        Z = 0,
-        G = null,
-        X, E = null,
-        F = !0;
-    const N = () => {
-        n(0, a = n(26, M = n(19, H = null))), n(24, L = performance.now()), n(25, P = 0), O = !0, I();
+        Z = null,
+        x = 0,
+        j = null,
+        X, C = null,
+        G = !0;
+    const I = () => {
+        n(0, a = n(26, M = n(19, O = null))), n(24, L = performance.now()), n(25, P = 0), H = !0, U();
     };
 
-    function I() {
+    function U() {
         requestAnimationFrame(() => {
-            n(25, P = (performance.now() - L) / 1e3), O && I();
+            n(25, P = (performance.now() - L) / 1e3), H && U();
         });
     }
 
-    function $() {
-        n(25, P = 0), n(0, a = n(26, M = n(19, H = null))), O && (O = !1);
+    function K() {
+        n(25, P = 0), n(0, a = n(26, M = n(19, O = null))), H && (H = !1);
     }
     $b(() => {
-        O && $();
+        H && K();
     });
-    let H = null;
+    let O = null;
 
     function J(p) {
         da[p ? "unshift" : "push"](() => {
-            E = p, n(16, E), n(7, m), n(14, G), n(15, X);
+            C = p, n(16, C), n(7, m), n(14, j), n(15, X);
         });
     }
 
-    function ee(p) {
+    function le(p) {
         da[p ? "unshift" : "push"](() => {
             y = p, n(13, y);
         });
     }
     return t.$$set = (p) => {
-        "i18n" in p && n(1, s = p.i18n), "eta" in p && n(0, a = p.eta), "queue_position" in p && n(2, l = p.queue_position), "queue_size" in p && n(3, u = p.queue_size), "status" in p && n(4, c = p.status), "scroll_to_output" in p && n(21, f = p.scroll_to_output), "timer" in p && n(5, h = p.timer), "show_progress" in p && n(6, d = p.show_progress), "message" in p && n(22, _ = p.message), "progress" in p && n(7, m = p.progress), "variant" in p && n(8, v = p.variant), "loading_text" in p && n(9, g = p.loading_text), "absolute" in p && n(10, S = p.absolute), "translucent" in p && n(11, w = p.translucent), "border" in p && n(12, k = p.border), "autoscroll" in p && n(23, C = p.autoscroll), "$$scope" in p && n(28, r = p.$$scope);
+        "i18n" in p && n(1, s = p.i18n), "eta" in p && n(0, a = p.eta), "queue_position" in p && n(2, l = p.queue_position), "queue_size" in p && n(3, u = p.queue_size), "status" in p && n(4, c = p.status), "scroll_to_output" in p && n(21, f = p.scroll_to_output), "timer" in p && n(5, h = p.timer), "show_progress" in p && n(6, d = p.show_progress), "message" in p && n(22, _ = p.message), "progress" in p && n(7, m = p.progress), "variant" in p && n(8, v = p.variant), "loading_text" in p && n(9, b = p.loading_text), "absolute" in p && n(10, S = p.absolute), "translucent" in p && n(11, w = p.translucent), "border" in p && n(12, k = p.border), "autoscroll" in p && n(23, E = p.autoscroll), "$$scope" in p && n(28, r = p.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            218103809 && (a === null && n(0, a = M), a != null && M !== a && (n(27, x = (performance.now() - L) / 1e3 + a), n(19, H = x.toFixed(1)), n(26, M = a))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            167772160 && n(17, Z = x === null || x <= 0 || !P ? null : Math.min(P / x, 1)), t.$$.dirty[0] & /*progress*/
-            128 && m != null && n(18, F = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (m != null ? n(14, G = m.map((p) => {
+            218103809 && (a === null && n(0, a = M), a != null && M !== a && (n(27, Z = (performance.now() - L) / 1e3 + a), n(19, O = Z.toFixed(1)), n(26, M = a))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            167772160 && n(17, x = Z === null || Z <= 0 || !P ? null : Math.min(P / Z, 1)), t.$$.dirty[0] & /*progress*/
+            128 && m != null && n(18, G = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (m != null ? n(14, j = m.map((p) => {
                 if (p.index != null && p.length != null)
                     return p.index / p.length;
                 if (p.progress != null)
                     return p.progress;
-            })) : n(14, G = null), G ? (n(15, X = G[G.length - 1]), E && (X === 0 ? n(16, E.style.transition = "0", E) : n(16, E.style.transition = "150ms", E))) : n(15, X = void 0)), t.$$.dirty[0] & /*status*/
-            16 && (c === "pending" ? N() : $()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            10493968 && y && f && (c === "pending" || c === "complete") && d2(y, C), t.$$.dirty[0] & /*status, message*/
+            })) : n(14, j = null), j ? (n(15, X = j[j.length - 1]), C && (X === 0 ? n(16, C.style.transition = "0", C) : n(16, C.style.transition = "150ms", C))) : n(15, X = void 0)), t.$$.dirty[0] & /*status*/
+            16 && (c === "pending" ? I() : K()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            10493968 && y && f && (c === "pending" || c === "complete") && dv(y, E), t.$$.dirty[0] & /*status, message*/
             4194320, t.$$.dirty[0] & /*timer_diff*/
             33554432 && n(20, i = P.toFixed(1));
     }, [
         a,
         s,
         l,
         u,
         c,
         h,
         d,
         m,
         v,
-        g,
+        b,
         S,
         w,
         k,
         y,
-        G,
+        j,
         X,
-        E,
-        Z,
-        F,
-        H,
+        C,
+        x,
+        G,
+        O,
         i,
         f,
         _,
-        C,
+        E,
         L,
         P,
         M,
-        x,
+        Z,
         r,
         o,
         J,
-        ee
+        le
     ];
 }
 class pc extends zb {
     constructor(e) {
         super(), Zb(
             this,
             e,
-            h2,
-            f2,
+            hv,
+            fv,
             Yb, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 21,
@@ -16003,38 +16011,38 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: _2,
-    add_flush_callback: m2,
+    SvelteComponent: _v,
+    add_flush_callback: mv,
     assign: gc,
-    bind: p2,
-    binding_callbacks: g2,
-    check_outros: b2,
+    bind: pv,
+    binding_callbacks: gv,
+    check_outros: bv,
     create_component: pn,
     destroy_component: gn,
     detach: ps,
-    empty: v2,
+    empty: vv,
     flush: ge,
     get_spread_object: bc,
     get_spread_update: vc,
-    group_outros: w2,
-    init: y2,
+    group_outros: wv,
+    init: yv,
     insert: gs,
     mount_component: bn,
-    safe_not_equal: k2,
+    safe_not_equal: kv,
     space: wc,
     transition_in: Tt,
     transition_out: Pt
 } = window.__gradio__svelte__internal;
 
-function E2(t) {
+function Ev(t) {
     let e, n;
     return e = new Na({
         props: {
             variant: (
                 /*value*/
                 t[0] === null && /*active_source*/
                 t[19] === "upload" ? "dashed" : "solid"
@@ -16065,15 +16073,15 @@
                 t[12]
             ),
             min_width: (
                 /*min_width*/
                 t[13]
             ),
             $$slots: {
-                default: [A2]
+                default: [Av]
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
@@ -16116,15 +16124,15 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function C2(t) {
+function Cv(t) {
     let e, n;
     return e = new Na({
         props: {
             variant: "solid",
             border_mode: (
                 /*dragging*/
                 t[20] ? "focus" : "base"
@@ -16151,15 +16159,15 @@
                 t[12]
             ),
             min_width: (
                 /*min_width*/
                 t[13]
             ),
             $$slots: {
-                default: [T2]
+                default: [Tv]
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
@@ -16199,15 +16207,15 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function S2(t) {
+function Sv(t) {
     let e, n;
     return e = new __({
         props: {
             i18n: (
                 /*gradio*/
                 t[18].i18n
             ),
@@ -16234,15 +16242,15 @@
         },
         d(i) {
             gn(e, i);
         }
     };
 }
 
-function A2(t) {
+function Av(t) {
     let e, n, i, o, r;
     const s = [{
             autoscroll: (
                 /*gradio*/
                 t[18].autoscroll
             )
         }, {
@@ -16314,26 +16322,26 @@
             t[21]
         ),
         waveform_options: (
             /*waveform_options*/
             t[15]
         ),
         $$slots: {
-            default: [S2]
+            default: [Sv]
         },
         $$scope: {
             ctx: t
         }
     };
     return (
         /*dragging*/
         t[20] !== void 0 && (u.dragging = /*dragging*/
             t[20]), i = new Bb({
             props: u
-        }), g2.push(() => p2(i, "dragging", l)), i.$on(
+        }), gv.push(() => pv(i, "dragging", l)), i.$on(
             "change",
             /*change_handler*/
             t[32]
         ), i.$on(
             "stream",
             /*stream_handler*/
             t[33]
@@ -16442,30 +16450,30 @@
                         c[15]), f[0] & /*gradio*/
                     262144 | f[1] & /*$$scope*/
                     16384 && (d.$$scope = {
                         dirty: f,
                         ctx: c
                     }), !o && f[0] & /*dragging*/
                     1048576 && (o = !0, d.dragging = /*dragging*/
-                        c[20], m2(() => o = !1)), i.$set(d);
+                        c[20], mv(() => o = !1)), i.$set(d);
             },
             i(c) {
                 r || (Tt(e.$$.fragment, c), Tt(i.$$.fragment, c), r = !0);
             },
             o(c) {
                 Pt(e.$$.fragment, c), Pt(i.$$.fragment, c), r = !1;
             },
             d(c) {
                 c && ps(n), gn(e, c), gn(i, c);
             }
         }
     );
 }
 
-function T2(t) {
+function Tv(t) {
     let e, n, i, o;
     const r = [{
             autoscroll: (
                 /*gradio*/
                 t[18].autoscroll
             )
         }, {
@@ -16589,51 +16597,51 @@
         },
         d(a) {
             a && ps(n), gn(e, a), gn(i, a);
         }
     };
 }
 
-function P2(t) {
+function Pv(t) {
     let e, n, i, o;
-    const r = [C2, E2],
+    const r = [Cv, Ev],
         s = [];
 
     function a(l, u) {
         return (
             /*interactive*/
             l[5] ? 1 : 0
         );
     }
     return e = a(t), n = s[e] = r[e](t), {
         c() {
-            n.c(), i = v2();
+            n.c(), i = vv();
         },
         m(l, u) {
             s[e].m(l, u), gs(l, i, u), o = !0;
         },
         p(l, u) {
             let c = e;
-            e = a(l), e === c ? s[e].p(l, u) : (w2(), Pt(s[c], 1, 1, () => {
+            e = a(l), e === c ? s[e].p(l, u) : (wv(), Pt(s[c], 1, 1, () => {
                 s[c] = null;
-            }), b2(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Tt(n, 1), n.m(i.parentNode, i));
+            }), bv(), n = s[e], n ? n.p(l, u) : (n = s[e] = r[e](l), n.c()), Tt(n, 1), n.m(i.parentNode, i));
         },
         i(l) {
             o || (Tt(n), o = !0);
         },
         o(l) {
             Pt(n), o = !1;
         },
         d(l) {
             l && ps(i), s[e].d(l);
         }
     };
 }
 
-function L2(t, e, n) {
+function Lv(t, e, n) {
     let {
         elem_id: i = ""
     } = e, {
         elem_classes: o = []
     } = e, {
         visible: r = !0
     } = e, {
@@ -16655,78 +16663,78 @@
     } = e, {
         scale: _ = null
     } = e, {
         min_width: m = void 0
     } = e, {
         loading_status: v
     } = e, {
-        autoplay: g = !1
+        autoplay: b = !1
     } = e, {
         editable: S = !0
     } = e, {
         waveform_options: w = {}
     } = e, {
         pending: k
     } = e, {
-        streaming: C
+        streaming: E
     } = e, {
         gradio: y
-    } = e, O = null, L, P = a, M, x;
+    } = e, H = null, L, P = a, M, Z;
 
-    function Z({
+    function x({
         detail: B
     }) {
         const [R, ce] = B.includes("Invalid file type") ? ["warning", "complete"] : ["error", "error"];
         n(1, v = v || {}), n(1, v.status = ce, v), n(1, v.message = B, v), y.dispatch(R, B);
     }
-    const G = (B) => y.dispatch("share", B.detail),
+    const j = (B) => y.dispatch("share", B.detail),
         X = (B) => y.dispatch("error", B.detail),
-        E = () => y.dispatch("play"),
-        F = () => y.dispatch("pause"),
-        N = () => y.dispatch("stop");
+        C = () => y.dispatch("play"),
+        G = () => y.dispatch("pause"),
+        I = () => y.dispatch("stop");
 
-    function I(B) {
+    function U(B) {
         M = B, n(20, M);
     }
-    const $ = ({
+    const K = ({
             detail: B
         }) => n(0, a = B),
-        H = ({
+        O = ({
             detail: B
         }) => {
             n(0, a = B), y.dispatch("stream", a);
         },
         J = ({
             detail: B
         }) => n(20, M = B),
-        ee = (B) => y.dispatch("edit", B.detail),
+        le = (B) => y.dispatch("edit", B.detail),
         p = () => y.dispatch("play"),
-        T = () => y.dispatch("pause"),
+        A = () => y.dispatch("pause"),
         q = () => y.dispatch("stop"),
         z = () => y.dispatch("start_recording"),
-        _e = () => y.dispatch("pause_recording"),
-        me = (B) => y.dispatch("stop_recording", B.detail),
-        U = () => y.dispatch("upload"),
-        Ce = () => y.dispatch("clear");
+        he = () => y.dispatch("pause_recording"),
+        _e = (B) => y.dispatch("stop_recording", B.detail),
+        F = () => y.dispatch("upload"),
+        ve = () => y.dispatch("clear");
     return t.$$set = (B) => {
-        "elem_id" in B && n(2, i = B.elem_id), "elem_classes" in B && n(3, o = B.elem_classes), "visible" in B && n(4, r = B.visible), "interactive" in B && n(5, s = B.interactive), "value" in B && n(0, a = B.value), "sources" in B && n(6, l = B.sources), "label" in B && n(7, u = B.label), "root" in B && n(8, c = B.root), "show_label" in B && n(9, f = B.show_label), "show_download_button" in B && n(10, h = B.show_download_button), "container" in B && n(11, d = B.container), "scale" in B && n(12, _ = B.scale), "min_width" in B && n(13, m = B.min_width), "loading_status" in B && n(1, v = B.loading_status), "autoplay" in B && n(23, g = B.autoplay), "editable" in B && n(14, S = B.editable), "waveform_options" in B && n(15, w = B.waveform_options), "pending" in B && n(16, k = B.pending), "streaming" in B && n(17, C = B.streaming), "gradio" in B && n(18, y = B.gradio);
+        "elem_id" in B && n(2, i = B.elem_id), "elem_classes" in B && n(3, o = B.elem_classes), "visible" in B && n(4, r = B.visible), "interactive" in B && n(5, s = B.interactive), "value" in B && n(0, a = B.value), "sources" in B && n(6, l = B.sources), "label" in B && n(7, u = B.label), "root" in B && n(8, c = B.root), "show_label" in B && n(9, f = B.show_label), "show_download_button" in B && n(10, h = B.show_download_button), "container" in B && n(11, d = B.container), "scale" in B && n(12, _ = B.scale), "min_width" in B && n(13, m = B.min_width), "loading_status" in B && n(1, v = B.loading_status), "autoplay" in B && n(23, b = B.autoplay), "editable" in B && n(14, S = B.editable), "waveform_options" in B && n(15, w = B.waveform_options), "pending" in B && n(16, k = B.pending), "streaming" in B && n(17, E = B.streaming), "gradio" in B && n(18, y = B.gradio);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*value, initial_value*/
             33554433 && a && P === null && n(25, P = a), t.$$.dirty[0] & /*value, old_value, gradio*/
-            17039361 && JSON.stringify(a) !== JSON.stringify(O) && (n(24, O = a), y.dispatch("change")), t.$$.dirty[0] & /*active_source, sources*/
+            17039361 && JSON.stringify(a) !== JSON.stringify(H) && (n(24, H = a), y.dispatch("change")), t.$$.dirty[0] & /*active_source, sources*/
             524352 && !L && l && n(19, L = l[0]), t.$$.dirty[0] & /*waveform_options, autoplay*/
-            8421376 && n(21, x = {
+            8421376 && n(21, Z = {
                 height: 50,
                 waveColor: w.waveform_color || "#9ca3af",
                 progressColor: w.waveform_progress_color || "#f97316",
                 barWidth: 2,
                 barGap: 3,
                 cursorWidth: 2,
                 cursorColor: "#ddd5e9",
-                autoplay: g,
+                autoplay: b,
                 barRadius: 10,
                 dragToSeek: !0,
                 normalize: !0,
                 minPxPerSec: 20,
                 mediaControls: w.show_controls
             });
     }, [
@@ -16743,51 +16751,51 @@
         h,
         d,
         _,
         m,
         S,
         w,
         k,
-        C,
+        E,
         y,
         L,
         M,
-        x,
         Z,
-        g,
-        O,
+        x,
+        b,
+        H,
         P,
-        G,
+        j,
         X,
-        E,
-        F,
-        N,
+        C,
+        G,
         I,
-        $,
-        H,
+        U,
+        K,
+        O,
         J,
-        ee,
+        le,
         p,
-        T,
+        A,
         q,
         z,
+        he,
         _e,
-        me,
-        U,
-        Ce
+        F,
+        ve
     ];
 }
-class Q2 extends _2 {
+class Qv extends _v {
     constructor(e) {
-        super(), y2(
+        super(), yv(
             this,
             e,
-            L2,
-            P2,
-            k2, {
+            Lv,
+            Pv,
+            kv, {
                 elem_id: 2,
                 elem_classes: 3,
                 visible: 4,
                 interactive: 5,
                 value: 0,
                 sources: 6,
                 label: 7,
@@ -16967,36 +16975,36 @@
     set gradio(e) {
         this.$$set({
             gradio: e
         }), ge();
     }
 }
 const {
-    SvelteComponent: R2,
-    append: B2,
-    attr: M2,
-    detach: D2,
-    element: O2,
-    init: H2,
-    insert: N2,
+    SvelteComponent: Rv,
+    append: Bv,
+    attr: Mv,
+    detach: Dv,
+    element: Hv,
+    init: Ov,
+    insert: Nv,
     noop: Ta,
-    safe_not_equal: I2,
-    set_data: U2,
-    text: j2,
+    safe_not_equal: Iv,
+    set_data: Uv,
+    text: jv,
     toggle_class: Pn
 } = window.__gradio__svelte__internal;
 
-function F2(t) {
+function Fv(t) {
     let e, n;
     return {
         c() {
-            e = O2("div"), n = j2(
+            e = Hv("div"), n = jv(
                 /*value*/
                 t[0]
-            ), M2(e, "class", "svelte-1gecy8w"), Pn(
+            ), Mv(e, "class", "svelte-1gecy8w"), Pn(
                 e,
                 "table",
                 /*type*/
                 t[1] === "table"
             ), Pn(
                 e,
                 "gallery",
@@ -17006,19 +17014,19 @@
                 e,
                 "selected",
                 /*selected*/
                 t[2]
             );
         },
         m(i, o) {
-            N2(i, e, o), B2(e, n);
+            Nv(i, e, o), Bv(e, n);
         },
         p(i, [o]) {
             o & /*value*/
-                1 && U2(
+                1 && Uv(
                     n,
                     /*value*/
                     i[0]
                 ), o & /*type*/
                 2 && Pn(
                     e,
                     "table",
@@ -17037,41 +17045,41 @@
                     /*selected*/
                     i[2]
                 );
         },
         i: Ta,
         o: Ta,
         d(i) {
-            i && D2(e);
+            i && Dv(e);
         }
     };
 }
 
-function q2(t, e, n) {
+function qv(t, e, n) {
     let {
         value: i
     } = e, {
         type: o
     } = e, {
         selected: r = !1
     } = e;
     return t.$$set = (s) => {
         "value" in s && n(0, i = s.value), "type" in s && n(1, o = s.type), "selected" in s && n(2, r = s.selected);
     }, [i, o, r];
 }
-class K2 extends R2 {
+class Kv extends Rv {
     constructor(e) {
-        super(), H2(this, e, q2, F2, I2, {
+        super(), Ov(this, e, qv, Fv, Iv, {
             value: 0,
             type: 1,
             selected: 2
         });
     }
 }
 export {
-    K2 as BaseExample,
+    Kv as BaseExample,
     Bb as BaseInteractiveAudio,
     _u as BasePlayer,
     Gm as BaseStaticAudio,
-    Q2 as
+    Qv as
     default
 };
```

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-2c3384e6.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-2c3384e6.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-aafe8b06.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-aafe8b06.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/module-d82531d9.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/module-d82531d9.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/style.css` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}.volume-slider.svelte-1xy0951{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:var(--size-20);accent-color:var(--color-accent);height:4px;cursor:pointer;outline:none;border-radius:15px;background-color:var(--neutral-400)}input[type=range].svelte-1xy0951::-webkit-slider-thumb{-webkit-appearance:none;-moz-appearance:none;appearance:none;height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}input[type=range].svelte-1xy0951::-moz-range-thumb{height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}.controls.svelte-sgfovr.svelte-sgfovr{display:grid;grid-template-columns:1fr 1fr 1fr;margin-top:5px;align-items:center;position:relative}.hidden.svelte-sgfovr.svelte-sgfovr{display:none}.control-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:self-start;align-items:center;justify-content:space-between}@media (max-width: 375px){.controls.svelte-sgfovr.svelte-sgfovr{display:flex;flex-wrap:wrap}.controls.svelte-sgfovr .svelte-sgfovr{margin:var(--spacing-sm)}}.action.svelte-sgfovr.svelte-sgfovr{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.icon.svelte-sgfovr.svelte-sgfovr:hover{color:var(--color-accent);fill:var(--color-accent)}.play-pause-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:right}.playback.svelte-sgfovr.svelte-sgfovr{border:1px solid var(--neutral-400);border-radius:var(--radius-sm);width:5.5ch;font-weight:300;font-size:var(--size-3);text-align:center;color:var(--neutral-400);height:var(--size-5);font-weight:700}.playback.svelte-sgfovr.svelte-sgfovr:hover,.playback.svelte-sgfovr.svelte-sgfovr:focus{color:var(--color-accent);border-color:var(--color-accent)}.rewind.svelte-sgfovr.svelte-sgfovr,.skip.svelte-sgfovr.svelte-sgfovr{margin:0 10px;color:var(--neutral-400)}.play-pause-button.svelte-sgfovr.svelte-sgfovr{width:var(--size-8);display:flex;align-items:center;justify-content:center;color:var(--neutral-400);fill:var(--neutral-400)}.volume.svelte-sgfovr.svelte-sgfovr{position:relative;display:flex;justify-content:center;margin-right:var(--spacing-xl)}.zoom-button.svelte-sgfovr.svelte-sgfovr{width:1.75em;fill:var(--neutral-400)}.caption-container.svelte-43he0g{display:flex;justify-content:center;margin-top:1em}div.svelte-43he0g.caption-container button{display:inline-block;padding:0 .5em;margin:.2em .5em}div.svelte-43he0g.caption-container button:hover{border-color:var(--color-accent)}button.active-button{border-width:2px;border-color:var(--color-accent)}.create-label.svelte-43he0g{width:2.25em;height:2.25em;fill:var(--neutral-400)}.create-label.svelte-43he0g:hover{fill:var(--color-accent)}.action.svelte-hdzdnn{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.regions-actions.svelte-hdzdnn{display:flex;justify-self:self-end;align-items:center}.commands.svelte-hdzdnn{display:flex;justify-content:space-between}.component-wrapper.svelte-hdzdnn{padding:4em}.icon.svelte-hdzdnn:hover{color:var(--color-accent)}.remove-button.svelte-hdzdnn,.trim-button.svelte-hdzdnn{fill:#9ca3af}.remove-button.svelte-hdzdnn:hover,.remove-button.svelte-hdzdnn:focus{fill:var(--color-accent)}.trim-button.svelte-hdzdnn:hover,.trim-button.svelte-hdzdnn:focus{fill:var(--color-accent)}::part(wrapper){margin-bottom:var(--size-2)}.timestamps.svelte-hdzdnn{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0}#time.svelte-hdzdnn,#duration.svelte-hdzdnn{color:var(--neutral-400)}.waveform-container.svelte-hdzdnn{display:flex;align-items:center;justify-content:center;width:var(--size-full)}.waveform-controls.svelte-hdzdnn{width:80em}#waveform.svelte-hdzdnn{width:100%;height:100%;position:relative}.standard-player.svelte-hdzdnn{width:100%;padding:var(--size-2)}.icon-buttons.svelte-1mrvp2o{display:flex;position:absolute;top:6px;right:6px;gap:var(--size-1)}.wrap.svelte-cr2edf.svelte-cr2edf{overflow-y:auto;transition:opacity .5s ease-in-out;background:var(--block-background-fill);position:relative;display:flex;flex-direction:column;align-items:center;justify-content:center;min-height:var(--size-40);width:var(--size-full)}.wrap.svelte-cr2edf.svelte-cr2edf:after{content:"";position:absolute;top:0;left:0;width:var(--upload-progress-width);height:100%;transition:all .5s ease-in-out;z-index:1}.uploading.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-lg);font-family:var(--font);z-index:2}.file-name.svelte-cr2edf.svelte-cr2edf{margin:var(--spacing-md);font-size:var(--text-lg);color:var(--body-text-color-subdued)}.file.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-md);z-index:2;display:flex;align-items:center}.file.svelte-cr2edf progress.svelte-cr2edf{display:inline;height:var(--size-1);width:100%;transition:all .5s ease-in-out;color:var(--color-accent);border:none}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-value{background-color:var(--color-accent);border-radius:20px}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-bar{background-color:var(--border-color-accent);border-radius:20px}.progress-bar.svelte-cr2edf.svelte-cr2edf{width:14px;height:14px;border-radius:50%;background:radial-gradient(closest-side,var(--block-background-fill) 64%,transparent 53% 100%),conic-gradient(var(--color-accent) var(--upload-progress-width),var(--border-color-accent) 0);transition:all .5s ease-in-out}button.svelte-1s26xmt{cursor:pointer;width:var(--size-full)}.hidden.svelte-1s26xmt{display:none;height:0!important;position:absolute;width:0;flex-grow:0}.center.svelte-1s26xmt{display:flex;justify-content:center}.flex.svelte-1s26xmt{display:flex;flex-direction:column;justify-content:center;align-items:center}.disable_click.svelte-1s26xmt{cursor:default}input.svelte-1s26xmt{display:none}div.svelte-1wj0ocy{display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.not-absolute.svelte-1wj0ocy{margin:var(--size-1)}.mic-select.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);background:var(--block-background-fill);padding:0px var(--spacing-xxl);border-radius:var(--radius-full);font-size:var(--text-md);border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.controls.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;overflow:hidden}.controls.svelte-l4xo8n select.svelte-l4xo8n{text-overflow:ellipsis;max-width:var(--size-40)}@media (max-width: 375px){.controls.svelte-l4xo8n select.svelte-l4xo8n{width:100%}}.wrapper.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;flex-wrap:wrap}.record.svelte-l4xo8n.svelte-l4xo8n{margin-right:var(--spacing-md)}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-l4xo8n-scaling 1.8s infinite}.stop-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin:var(--size-1) var(--size-1) 0 0}.record-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed}.record-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed;opacity:.5}@keyframes svelte-l4xo8n-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}.pause-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);margin:var(--size-1) var(--size-1) 0 0}.resume-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-xl);line-height:1px;font-size:var(--text-md);margin:var(--size-1) var(--size-1) 0 0}.duration.svelte-l4xo8n.svelte-l4xo8n{display:flex;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);align-items:center;justify-content:center;margin:var(--size-1) var(--size-1) 0 0}::part(region){border-radius:var(--radius-md);height:98%!important;border:1px solid var(--color-accent);border-width:0px 0px}::part(region-handle){width:5px!important;border:none}.microphone.svelte-1z0uz8p{width:100%;display:none}.component-wrapper.svelte-1z0uz8p{padding:var(--size-3);width:100%}.timestamps.svelte-1z0uz8p{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0;margin:var(--spacing-md) 0}.time.svelte-1z0uz8p,.duration.svelte-1z0uz8p{color:var(--neutral-400)}.trim-duration.svelte-1z0uz8p{color:var(--color-accent);margin-right:var(--spacing-sm)}.mic-wrap.svelte-4ycsjo{display:block;align-items:center;margin:var(--spacing-xl)}.stop-button-paused.svelte-4ycsjo{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin-right:5px}.stop-button-paused.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-4ycsjo-scaling 1.8s infinite}.stop-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin-right:5px;display:flex}.record-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}@keyframes svelte-4ycsjo-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1yserjw.svelte-1yserjw{top:0;right:0;left:0}.wrap.default.svelte-1yserjw.svelte-1yserjw{top:0;right:0;bottom:0;left:0}.hide.svelte-1yserjw.svelte-1yserjw{opacity:0;pointer-events:none}.generating.svelte-1yserjw.svelte-1yserjw{animation:svelte-1yserjw-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1)}.translucent.svelte-1yserjw.svelte-1yserjw{background:none}@keyframes svelte-1yserjw-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1yserjw.svelte-1yserjw{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1yserjw.svelte-1yserjw{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1yserjw.svelte-1yserjw{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1yserjw.svelte-1yserjw{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1yserjw.svelte-1yserjw{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1yserjw .progress-text.svelte-1yserjw{background:var(--block-background-fill)}.border.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-1gecy8w{padding:var(--size-1) var(--size-2)}
+.block.svelte-nl1om8{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-nl1om8{border-color:var(--color-accent)}.block.border_contrast.svelte-nl1om8{border-color:var(--body-text-color)}.padded.svelte-nl1om8{padding:var(--block-padding)}.hidden.svelte-nl1om8{display:none}.hide-container.svelte-nl1om8{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.dropdown-arrow.svelte-145leq6{fill:currentColor}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}.volume-slider.svelte-1xy0951{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:var(--size-20);accent-color:var(--color-accent);height:4px;cursor:pointer;outline:none;border-radius:15px;background-color:var(--neutral-400)}input[type=range].svelte-1xy0951::-webkit-slider-thumb{-webkit-appearance:none;-moz-appearance:none;appearance:none;height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}input[type=range].svelte-1xy0951::-moz-range-thumb{height:15px;width:15px;background-color:var(--color-accent);border-radius:50%;border:none;transition:.2s ease-in-out}.controls.svelte-sgfovr.svelte-sgfovr{display:grid;grid-template-columns:1fr 1fr 1fr;margin-top:5px;align-items:center;position:relative}.hidden.svelte-sgfovr.svelte-sgfovr{display:none}.control-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:self-start;align-items:center;justify-content:space-between}@media (max-width: 375px){.controls.svelte-sgfovr.svelte-sgfovr{display:flex;flex-wrap:wrap}.controls.svelte-sgfovr .svelte-sgfovr{margin:var(--spacing-sm)}}.action.svelte-sgfovr.svelte-sgfovr{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.icon.svelte-sgfovr.svelte-sgfovr:hover{color:var(--color-accent);fill:var(--color-accent)}.play-pause-wrapper.svelte-sgfovr.svelte-sgfovr{display:flex;justify-self:right}.playback.svelte-sgfovr.svelte-sgfovr{border:1px solid var(--neutral-400);border-radius:var(--radius-sm);width:5.5ch;font-weight:300;font-size:var(--size-3);text-align:center;color:var(--neutral-400);height:var(--size-5);font-weight:700}.playback.svelte-sgfovr.svelte-sgfovr:hover,.playback.svelte-sgfovr.svelte-sgfovr:focus{color:var(--color-accent);border-color:var(--color-accent)}.rewind.svelte-sgfovr.svelte-sgfovr,.skip.svelte-sgfovr.svelte-sgfovr{margin:0 10px;color:var(--neutral-400)}.play-pause-button.svelte-sgfovr.svelte-sgfovr{width:var(--size-8);display:flex;align-items:center;justify-content:center;color:var(--neutral-400);fill:var(--neutral-400)}.volume.svelte-sgfovr.svelte-sgfovr{position:relative;display:flex;justify-content:center;margin-right:var(--spacing-xl)}.zoom-button.svelte-sgfovr.svelte-sgfovr{width:1.75em;fill:var(--neutral-400)}.caption-container.svelte-43he0g{display:flex;justify-content:center;margin-top:1em}div.svelte-43he0g.caption-container button{display:inline-block;padding:0 .5em;margin:.2em .5em}div.svelte-43he0g.caption-container button:hover{border-color:var(--color-accent)}button.active-button{border-width:2px;border-color:var(--color-accent)}.create-label.svelte-43he0g{width:2.25em;height:2.25em;fill:var(--neutral-400)}.create-label.svelte-43he0g:hover{fill:var(--color-accent)}.action.svelte-1w83umt{width:var(--size-5);color:var(--neutral-400);margin-left:var(--spacing-md)}.regions-actions.svelte-1w83umt{display:flex;justify-self:self-end;align-items:center}.commands.svelte-1w83umt{display:flex;justify-content:space-between}.component-wrapper.svelte-1w83umt{padding:4em}.icon.svelte-1w83umt:hover{color:var(--color-accent)}.remove-button.svelte-1w83umt,.trim-button.svelte-1w83umt{fill:var(--neutral-400)}.remove-button.svelte-1w83umt:hover,.remove-button.svelte-1w83umt:focus{fill:var(--color-accent)}.trim-button.svelte-1w83umt:hover,.trim-button.svelte-1w83umt:focus{fill:var(--color-accent)}.timestamps.svelte-1w83umt{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0}#time.svelte-1w83umt,#duration.svelte-1w83umt{color:var(--neutral-400)}.waveform-container.svelte-1w83umt{display:flex;align-items:center;justify-content:center;width:var(--size-full)}.waveform-controls.svelte-1w83umt{width:80em}#waveform.svelte-1w83umt{width:100%;height:100%;position:relative}.standard-player.svelte-1w83umt{width:100%;padding:var(--size-2)}.icon-buttons.svelte-1mrvp2o{display:flex;position:absolute;top:6px;right:6px;gap:var(--size-1)}.wrap.svelte-cr2edf.svelte-cr2edf{overflow-y:auto;transition:opacity .5s ease-in-out;background:var(--block-background-fill);position:relative;display:flex;flex-direction:column;align-items:center;justify-content:center;min-height:var(--size-40);width:var(--size-full)}.wrap.svelte-cr2edf.svelte-cr2edf:after{content:"";position:absolute;top:0;left:0;width:var(--upload-progress-width);height:100%;transition:all .5s ease-in-out;z-index:1}.uploading.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-lg);font-family:var(--font);z-index:2}.file-name.svelte-cr2edf.svelte-cr2edf{margin:var(--spacing-md);font-size:var(--text-lg);color:var(--body-text-color-subdued)}.file.svelte-cr2edf.svelte-cr2edf{font-size:var(--text-md);z-index:2;display:flex;align-items:center}.file.svelte-cr2edf progress.svelte-cr2edf{display:inline;height:var(--size-1);width:100%;transition:all .5s ease-in-out;color:var(--color-accent);border:none}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-value{background-color:var(--color-accent);border-radius:20px}.file.svelte-cr2edf progress[value].svelte-cr2edf::-webkit-progress-bar{background-color:var(--border-color-accent);border-radius:20px}.progress-bar.svelte-cr2edf.svelte-cr2edf{width:14px;height:14px;border-radius:50%;background:radial-gradient(closest-side,var(--block-background-fill) 64%,transparent 53% 100%),conic-gradient(var(--color-accent) var(--upload-progress-width),var(--border-color-accent) 0);transition:all .5s ease-in-out}button.svelte-1s26xmt{cursor:pointer;width:var(--size-full)}.hidden.svelte-1s26xmt{display:none;height:0!important;position:absolute;width:0;flex-grow:0}.center.svelte-1s26xmt{display:flex;justify-content:center}.flex.svelte-1s26xmt{display:flex;flex-direction:column;justify-content:center;align-items:center}.disable_click.svelte-1s26xmt{cursor:default}input.svelte-1s26xmt{display:none}div.svelte-1wj0ocy{display:flex;top:var(--size-2);right:var(--size-2);justify-content:flex-end;gap:var(--spacing-sm);z-index:var(--layer-1)}.not-absolute.svelte-1wj0ocy{margin:var(--size-1)}.mic-select.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);background:var(--block-background-fill);padding:0px var(--spacing-xxl);border-radius:var(--radius-full);font-size:var(--text-md);border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.controls.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;overflow:hidden}.controls.svelte-l4xo8n select.svelte-l4xo8n{text-overflow:ellipsis;max-width:var(--size-40)}@media (max-width: 375px){.controls.svelte-l4xo8n select.svelte-l4xo8n{width:100%}}.wrapper.svelte-l4xo8n.svelte-l4xo8n{display:flex;align-items:center;flex-wrap:wrap}.record.svelte-l4xo8n.svelte-l4xo8n{margin-right:var(--spacing-md)}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin:var(--size-1) var(--size-1) 0 0}.stop-button-paused.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-l4xo8n-scaling 1.8s infinite}.stop-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin:var(--size-1) var(--size-1) 0 0}.record-button.svelte-l4xo8n.svelte-l4xo8n:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-l4xo8n.svelte-l4xo8n{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}.stop-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed}.record-button.svelte-l4xo8n.svelte-l4xo8n:disabled{cursor:not-allowed;opacity:.5}@keyframes svelte-l4xo8n-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}.pause-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);margin:var(--size-1) var(--size-1) 0 0}.resume-button.svelte-l4xo8n.svelte-l4xo8n{display:none;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-xl);line-height:1px;font-size:var(--text-md);margin:var(--size-1) var(--size-1) 0 0}.duration.svelte-l4xo8n.svelte-l4xo8n{display:flex;height:var(--size-8);width:var(--size-20);border:1px solid var(--neutral-400);border-radius:var(--radius-3xl);padding:var(--spacing-md);align-items:center;justify-content:center;margin:var(--size-1) var(--size-1) 0 0}::part(region){border-radius:var(--radius-md);height:98%!important;border:1px solid var(--color-accent);border-width:0px 0px}::part(region-handle){width:5px!important;border:none}.microphone.svelte-1z0uz8p{width:100%;display:none}.component-wrapper.svelte-1z0uz8p{padding:var(--size-3);width:100%}.timestamps.svelte-1z0uz8p{display:flex;justify-content:space-between;align-items:center;width:100%;padding:var(--size-1) 0;margin:var(--spacing-md) 0}.time.svelte-1z0uz8p,.duration.svelte-1z0uz8p{color:var(--neutral-400)}.trim-duration.svelte-1z0uz8p{color:var(--color-accent);margin-right:var(--spacing-sm)}.mic-wrap.svelte-4ycsjo{display:block;align-items:center;margin:var(--spacing-xl)}.stop-button-paused.svelte-4ycsjo{display:none;height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--neutral-400);margin-right:5px}.stop-button-paused.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.stop-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl);animation:svelte-4ycsjo-scaling 1.8s infinite}.stop-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-20);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);align-items:center;border:1px solid var(--primary-600);margin-right:5px;display:flex}.record-button.svelte-4ycsjo:before{content:"";height:var(--size-4);width:var(--size-4);border-radius:var(--radius-full);background:var(--primary-600);margin:0 var(--spacing-xl)}.record-button.svelte-4ycsjo{height:var(--size-8);width:var(--size-24);background-color:var(--block-background-fill);border-radius:var(--radius-3xl);display:flex;align-items:center;border:1px solid var(--neutral-400)}@keyframes svelte-4ycsjo-scaling{0%{background-color:var(--primary-600);scale:1}50%{background-color:var(--primary-600);scale:1.2}to{background-color:var(--primary-600);scale:1}}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1yserjw.svelte-1yserjw{top:0;right:0;left:0}.wrap.default.svelte-1yserjw.svelte-1yserjw{top:0;right:0;bottom:0;left:0}.hide.svelte-1yserjw.svelte-1yserjw{opacity:0;pointer-events:none}.generating.svelte-1yserjw.svelte-1yserjw{animation:svelte-1yserjw-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent;z-index:var(--layer-1)}.translucent.svelte-1yserjw.svelte-1yserjw{background:none}@keyframes svelte-1yserjw-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1yserjw.svelte-1yserjw{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1yserjw.svelte-1yserjw{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1yserjw.svelte-1yserjw{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1yserjw.svelte-1yserjw{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1yserjw.svelte-1yserjw{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1yserjw.svelte-1yserjw{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1yserjw.svelte-1yserjw{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1yserjw .progress-text.svelte-1yserjw{background:var(--block-background-fill)}.border.svelte-1yserjw.svelte-1yserjw{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}.gallery.svelte-1gecy8w{padding:var(--size-1) var(--size-2)}
```

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/backend/gryannote_audio/templates/example/index.js` & `gryannote_audio-0.1.5/backend/gryannote_audio/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/Index.svelte` & `gryannote_audio-0.1.5/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/package-lock.json` & `gryannote_audio-0.1.5/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/package.json` & `gryannote_audio-0.1.5/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/interactive/InteractiveAnnotatedAudio.svelte` & `gryannote_audio-0.1.5/frontend/interactive/InteractiveAnnotatedAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/player/AudioPlayerWithAnnotation.svelte` & `gryannote_audio-0.1.5/frontend/player/AudioPlayerWithAnnotation.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 		type RegionParams,
 	} from "wavesurfer.js/dist/plugins/regions.js";
 	import WaveformControls from "../shared/WaveformControls.svelte";
 	import { Empty } from "@gradio/atoms";
 	import { resolve_wasm_src } from "@gradio/wasm/svelte";
 	import AnnotatedAudioData from "../shared/AnnotatedAudioData";
 	import { createEventDispatcher } from "svelte";
-	import Caption from "../shared/Caption.svelte"
+	import Caption  from "../shared/Caption.svelte"
 
 	export let value: null | AnnotatedAudioData = null;
 	$: url = value.file_data?.url;
 	export let label: string;
 	export let i18n: I18nFormatter;
 	export let interactive = true;
 	export let editable = true;
@@ -38,19 +38,20 @@
 	let timeRef: HTMLTimeElement;
 	let durationRef: HTMLTimeElement;
 	let audio_duration: number;
 	let playing = false;
 
 	let show_volume_slider = false;
 	let showRedo = interactive;
-
+	// keep initial annotations in memory
 	let initialAnnotations: Annotation[] | null = null;
 	// correspondence between a Region and an Annotation
 	let regionsMap: Map<string, Annotation> = new Map();
 
+	let caption: Caption;
 	let defaultLabel: CaptionLabel | null = null;
 	let activeLabel: CaptionLabel | null = null;
 
 	const dispatch = createEventDispatcher<{
 		stop: undefined;
 		play: undefined;
 		pause: undefined;
@@ -73,46 +74,43 @@
 		resolve_wasm_src(value.file_data?.url).then((resolved_src) => {
 			if (resolved_src && waveform) {
 				return waveform.load(resolved_src);
 			}
 		});
 
 		waveform.on("dblclick", () => {
-			// allow the user to add a region only after the pipeline has been applied
-			if(value?.annotations){
-				handleRegionAdd(waveform.getCurrentTime());
-			}
+			handleRegionAdd(waveform.getCurrentTime());
 		});
 	};
 
 	/**
 	 * Print regions on waveform given annotation data provided by the pipeline.
 	 * A region can be view as a visual representation of an annotation.
 	 */
-	function initRegions(): void {
+	function createRegions(annotations: Annotation[]): void {
 
-		let annotations = value.annotations;
-
-		// keep initial annotations in memory, for future retrieval
-		if (initialAnnotations === null){
-			initialAnnotations = []
-
-			// defines a label that will be activated by default if the user selects none
-			// this label is set to the first annotation's speaker, if there is at least one
-			// annotation, or none otherwise.
-			if(annotations.length === 0){
-				return;
-			}
-			defaultLabel = {speaker: annotations[0].speaker, color: annotations[0].color, shortcut: "A"};
-			annotations.forEach(
-				annotation => initialAnnotations.push(Object.assign({}, annotation))
-			);
+		if (!initialAnnotations){
+			initialAnnotations = [...annotations];
+		}
+		if(annotations.length === 0){
+			return;
 		}
+		// defines a label that will be activated by default if the user selects none
+		// this label is set to the first annotation's speaker, if there is at least one
+		// annotation, or none otherwise.
+		defaultLabel = {speaker: annotations[0].speaker, color: annotations[0].color, shortcut: "A"};
+
+		const currentAnnotations = Array.from(regionsMap.values());
+		annotations = annotations.filter(annotation => !currentAnnotations.some(currentAnnotation =>
+			annotation.start === currentAnnotation.start &&
+			annotation.end === currentAnnotation.end &&
+			annotation.speaker === currentAnnotation.speaker
+		))
 
-		value.annotations.forEach(annotation => {
+		annotations.forEach(annotation => {
 			let region = addRegion({
 				start: annotation.start,
 				end: annotation.end,
 				color: annotation.color,
 				drag: true,
 				resize: true,
 			}, annotation.speaker);
@@ -136,42 +134,44 @@
 	 * @param options region's params (start, end, color)
 	 * @param speaker region's label
 	 *
 	 * @returns the added region
 	 */
 	function addRegion(options: RegionParams, speaker: string): Region {
 		let region = wsRegions.addRegion(options);
-		regionsMap.set(region.id, {
-			start: region.start,
-			end: region.end,
-			speaker: speaker,
-			color: region.color,
-		});
+		const annotation = {start: region.start, end: region.end, speaker: speaker, color: region.color};
+		regionsMap.set(region.id, annotation);
+
+		// if this is the first region added on the waveform
+		if(!initialAnnotations){
+			initialAnnotations = [annotation];
+		}
 		updateAnnotations();
 
 		return region;
 	}
 
 	/**
 	 * Handle add region event. The new added region become the active region.
 	 * @param relativeY mouse y-coordinate relative to waveform start
 	 */
 	function handleRegionAdd(relativeY: number): void{
-		let regionLabel = (activeLabel !== null ? activeLabel : defaultLabel);
+		let label = (activeLabel !== null ? activeLabel : defaultLabel);
 		// if annotations were not initialized, do nothing
-		if (regionLabel === null){
+		if (label === null){
+			window.alert("First create a label by clicking on \"+\" or by pressing A-Z");
 			return;
 		}
 		let region = addRegion({
 			start: relativeY - 1.0,
 			end: relativeY + 1.0,
-			color: regionLabel.color,
+			color: label.color,
 			drag: true,
 			resize: true,
-		}, regionLabel.speaker);
+		}, label.speaker);
 
 		// set region as active one
 		setActiveRegion(region);
 	}
 
 	/**
 	 * Remove specified region from waveform as well as
@@ -219,15 +219,15 @@
 	 * data provided by pipeline
 	 */
 	function resetRegions(): void {
 		clearRegions();
 		initialAnnotations.forEach(
 				annotation => value.annotations.push(Object.assign({}, annotation))
 		);
-		initRegions();
+		createRegions(value.annotations);
 		dispatch("edit", value);
 	}
 
 	/**
 	 * Clear all the regions from waveform, as well as
 	 * annotation data given by pipeline
 	 */
@@ -467,16 +467,16 @@
 	$: if (container !== undefined) {
 		if (waveform !== undefined) waveform.destroy();
 		container.innerHTML = "";
 		create_waveform();
 		playing = false;
 	}
 
-	$: if(value?.annotations !== null && wsRegions && initialAnnotations === null){
-		initRegions();
+	$: if(value?.annotations !== null && wsRegions){
+		createRegions(value.annotations);
 	}
 
 	$: waveform?.on("decode", (duration: any) => {
 		audio_duration = duration;
 		durationRef && (durationRef.textContent = formatTime(duration));
 	});
 
@@ -521,14 +521,15 @@
 
 	$: wsRegions?.on("region-clicked", (region, e) => {
 		switch(mode){
 			case "remove": removeRegion(region); break;
 			case "split": splitRegion(region, region.start + (region.end - region.start) / 2); break;
 			default: setActiveRegion(region); region.play();
 		}
+		mode = "";
 	});
 
 	$: if (activeRegion) {
 		const shadowRoot = container.children[0]!.shadowRoot!;
 
 		rightRegionHandle = shadowRoot.querySelector('[data-resize="right"]');
 		leftRegionHandle = shadowRoot.querySelector('[data-resize="left"]');
@@ -619,49 +620,48 @@
 						{audio_duration}
 						{i18n}
 						bind:show_volume_slider
 						{waveform_options}
 					/>
 				</div>
 				<div class="regions-actions">
-					{#if editable && interactive && value.annotations}
+					{#if editable && interactive && value}
 					{#if showRedo}
 						<button
 							class="action icon"
 							aria-label="Reset annotations"
 							title={i18n("Reset annotations")}
 							on:click={resetRegions}
 						>
 							<Undo/>
 						</button>
 					{/if}
 					<button
 						class="action icon remove-button"
 						aria-label="Remove an annotation"
 						title={i18n("Remove an annotation")}
-						on:focusin={() => mode = "remove"}
-						on:focusout={() => mode = ""}
+						on:click={() => mode = "remove"}
 					>
 						<Gum/>
 					</button>
 					<button
 						class="action icon trim-button"
 						aria-label="Split an annotation"
 						title={i18n("Split an annotation")}
-						on:focusin={() => mode = "split"}
-						on:focusout={() => mode = ""}
+						on:click={() => mode = "split"}
 					>
 						<Trim/>
 					</button>
 				{/if}
 				</div>
 			</div>
-			{#if value?.annotations}
+			{#if value}
 				<Caption
 					value={value.annotations}
+					bind:this={caption}
 					on:select={(e) => setRegionSpeaker(e.detail)}
 					on:select={(e) => activeLabel = e.detail}
 				/>
 			{/if}
 		{/if}
 	</div>
 {/if}
@@ -690,29 +690,25 @@
 	}
 
 	.icon:hover {
 		color: var(--color-accent);
 	}
 
 	.remove-button, .trim-button {
-		fill: #9ca3af;
+		fill: var(--neutral-400);
 	}
 
 	.remove-button:hover, .remove-button:focus {
 		fill: var(--color-accent);
 	}
 
 	.trim-button:hover, .trim-button:focus {
 		fill: var(--color-accent);
 	}
 
-	:global(::part(wrapper)) {
-		margin-bottom: var(--size-2);
-	}
-
 	.timestamps {
 		display: flex;
 		justify-content: space-between;
 		align-items: center;
 		width: 100%;
 		padding: var(--size-1) 0;
 	}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {#if value === null} {:else if value.file_data.is_stream} {:else}
 "waveform-" + label : "unlabelled-audio"} >
 0:00
 0:00
 {#if waveform}
 waveform} {playing} {audio_duration} {i18n} bind:show_volume_slider
 {waveform_options} />
-{#if editable && interactive && value.annotations} {#if showRedo} {/if}
-> mode = "remove"} on:focusout={() => mode = ""} >
-> mode = "split"} on:focusout={() => mode = ""} > {/if}
-{#if value?.annotations}
+{#if editable && interactive && value} {#if showRedo} {/if}
+> mode = "remove"} >
+> mode = "split"} > {/if}
+{#if value}
 > setRegionSpeaker(e.detail)} on:select={(e) => activeLabel = e.detail} /> {/
 if} {/if}
 {/if}
```

### Comparing `gryannote_audio-0.1.4/frontend/recorder/AudioRecorder.svelte` & `gryannote_audio-0.1.5/frontend/recorder/AudioRecorder.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/AnnotatedAudioData.ts` & `gryannote_audio-0.1.5/frontend/shared/AnnotatedAudioData.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/Audio.svelte` & `gryannote_audio-0.1.5/frontend/shared/Audio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/Caption.svelte` & `gryannote_audio-0.1.5/frontend/shared/Caption.svelte`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
     function createLabelElement(label: CaptionLabel): void {
         const labelButton = document.createElement("button");
         labelButton.style.backgroundColor = label.color;
         labelButton.classList.add("captionLabel");
         labelButton.id = label.shortcut;
         labelButton.innerHTML = "<span style=\"font-weight: bold;\">" +  label.shortcut + "</span>: " + label.speaker;
-        labelButton.addEventListener("focusin", () => {selectActiveLabel(label.shortcut)});
-        labelButton.addEventListener("focusout", () => {selectActiveLabel("Escape")});
+        labelButton.addEventListener("focusin", () => {handleKeyboardSelection(label.shortcut)});
+        labelButton.addEventListener("focusout", () => {handleKeyboardSelection("Escape")});
 
         container.appendChild(labelButton);
     }
 
 
-    function createLabel(speaker?: string, color?: string, shortcut?: string): CaptionLabel {
+    export function createLabel(speaker?: string, color?: string, shortcut?: string): CaptionLabel {
         // if maximum number of labels has been reached, do nothing
         if(labels.length === 26){
             return;
         }
         if(!speaker){
             speaker = "SPEAKER_" + speakerIdx.toString().padStart(2, "0");
         }
@@ -59,31 +59,37 @@
         createLabelElement(label);
 
         speakerIdx++;
 
         return label;
     }
 
-    function selectActiveLabel(key: string): void {
+    function setActiveLabel(label: CaptionLabel): void {
         // reset active label
         if(activeLabel){
             document.getElementById(activeLabel.shortcut).classList.remove("active-button");
         }
 
+        // update active label
+        activeLabel = label;
+        document.getElementById(activeLabel.shortcut).classList.add("active-button");
+        dispatch("select", activeLabel);
+    }
+
+    function handleKeyboardSelection(key: string): void {
+        let label = null
+
         if(key !== "Escape"){
-            let label = labels.find((_label) => _label.shortcut === key.toUpperCase());
+            label = labels.find((_label) => _label.shortcut === key.toUpperCase());
             // if current key does not correspond to any label, create a new one
             if(!label){
                 label = createLabel(undefined, undefined , key.toUpperCase());
             }
-            // update active label
-            activeLabel = label;
-            document.getElementById(activeLabel.shortcut).classList.add("active-button");
-            dispatch("select", activeLabel);
         }
+        setActiveLabel(label);
     }
 
     $:{
         if(container && value){
             // retrieve speaker list and corresponding annotation color
             value.forEach(annotation => {
                 // if annotation has a label that does not already exist in the caption,
@@ -95,24 +101,27 @@
             labels = labels.sort((i1, i2) => i1.shortcut.localeCompare(i2.shortcut));
         }
     }
 
     onMount(() => {
         window.addEventListener("keydown", (e): void => {
             if(e.key.match(/^[a-zA-Z]$/) || e.key === "Escape"){
-                selectActiveLabel(e.key);
+                handleKeyboardSelection(e.key);
             }
         });
     });
 </script>
 
 <div class="caption-container">
     <div class="caption" bind:this={container}></div>
     <div class="action-buttons">
-        <button class="create-label" on:click={() => createLabel()}>
+        <button class="create-label" on:click={() => {
+                const label = createLabel();
+                setActiveLabel(label);
+            }}>
              <Plus/>
         </button>
     </div>
 </div>
 
 <style>
```

#### html2text {}

```diff
@@ -1 +1 @@
-> createLabel()}>
+> { const label = createLabel(); setActiveLabel(label); }}>
```

### Comparing `gryannote_audio-0.1.4/frontend/shared/VolumeControl.svelte` & `gryannote_audio-0.1.5/frontend/shared/VolumeControl.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/WaveformControls.svelte` & `gryannote_audio-0.1.5/frontend/shared/WaveformControls.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/WaveformRecordControls.svelte` & `gryannote_audio-0.1.5/frontend/shared/WaveformRecordControls.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/audioBufferToWav.ts` & `gryannote_audio-0.1.5/frontend/shared/audioBufferToWav.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/utils.ts` & `gryannote_audio-0.1.5/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/icons/Gum.svelte` & `gryannote_audio-0.1.5/frontend/shared/icons/Gum.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/icons/Magnifier.svelte` & `gryannote_audio-0.1.5/frontend/shared/icons/Magnifier.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/shared/icons/Plus.svelte` & `gryannote_audio-0.1.5/frontend/shared/icons/Plus.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/static/StaticAnnotatedAudio.svelte` & `gryannote_audio-0.1.5/frontend/static/StaticAnnotatedAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/frontend/streaming/StreamAudio.svelte` & `gryannote_audio-0.1.5/frontend/streaming/StreamAudio.svelte`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/README.md` & `gryannote_audio-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gryannote_audio-0.1.4/pyproject.toml` & `gryannote_audio-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gryannote_audio"
-version = "0.1.4"
+version = "0.1.5"
 description = "audio component with speaker annotations"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Clément Pagés", email = "clement.pages@irit.fr" }]
 keywords = ["gradio-custom-component", "gradio-template-Audio", "pyannote.audio", "speaker diarization"]
 # Add dependencies here
```

### Comparing `gryannote_audio-0.1.4/PKG-INFO` & `gryannote_audio-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gryannote_audio
-Version: 0.1.4
+Version: 0.1.5
 Summary: audio component with speaker annotations
 Author-email: Clément Pagés <clement.pages@irit.fr>
 License-Expression: MIT
 Keywords: gradio-custom-component,gradio-template-Audio,pyannote.audio,speaker diarization
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```


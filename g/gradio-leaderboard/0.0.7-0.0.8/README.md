# Comparing `tmp/gradio_leaderboard-0.0.7.tar.gz` & `tmp/gradio_leaderboard-0.0.8.tar.gz`

## Comparing `gradio_leaderboard-0.0.7.tar` & `gradio_leaderboard-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/__init__.py
--rw-r--r--   0        0        0    18498 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/leaderboard.py
--rw-r--r--   0        0        0    33817 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/leaderboard.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0  1006135 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/index.js
--rw-r--r--   0        0        0  1498407 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/example/index.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/app.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/config.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/css.css
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/docs.md
--rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/leaderboard_data.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/demo/space.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/Example.svelte
--rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/Index.svelte
--rw-r--r--   0        0        0    50149 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/package-lock.json
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/package.json
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/Checkboxgroup.svelte
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/EditableCell.svelte
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/Example.svelte
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/RangeSlider.svelte
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/SimpleTextbox.svelte
--rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/Table.svelte
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/VirtualTable.svelte
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/frontend/shared/utils.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/.gitignore
--rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/README.md
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/__init__.py
+-rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.py
+-rw-r--r--   0        0        0    34570 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0  1006163 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/index.js
+-rw-r--r--   0        0        0  1498407 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/index.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/__init__.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/app.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/config.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/css.css
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/docs.md
+-rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/leaderboard_data.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/space.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/Example.svelte
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/Index.svelte
+-rw-r--r--   0        0        0    50149 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/package-lock.json
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/package.json
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Checkboxgroup.svelte
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/EditableCell.svelte
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Example.svelte
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/RangeSlider.svelte
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/SimpleTextbox.svelte
+-rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Table.svelte
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/VirtualTable.svelte
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/.gitignore
+-rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/README.md
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/PKG-INFO
```

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/leaderboard.py` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         self.wrap = wrap
         self.headers = [str(s) for s in value.columns]
         self.datatype = datatype
         self.search_columns = self._get_search_columns(search_columns)
         self.bool_checkboxgroup_label = bool_checkboxgroup_label
         self.select_columns_config = self._get_select_columns(select_columns, value)
         self.filter_columns = self._get_column_filter_configs(filter_columns, value)
+        self.raise_error_if_incorrect_config()
+
         self.hide_columns = hide_columns or []
         self.col_count = (len(self.headers), "fixed")
         self.row_count = (value.shape[0], "fixed")
 
         if latex_delimiters is None:
             latex_delimiters = [{"left": "$$", "right": "$$", "display": True}]
         self.latex_delimiters = latex_delimiters
@@ -152,14 +154,25 @@
             interactive=interactive,
             visible=visible,
             elem_id=elem_id,
             elem_classes=elem_classes,
             render=render,
             value=value,
         )
+    
+    def raise_error_if_incorrect_config(self):
+        for col in [self.search_columns.primary_column, *self.search_columns.secondary_columns]:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
+        for col in self.select_columns_config.default_selection + self.select_columns_config.cant_deselect:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
+        for col in [col.column for col in self.filter_columns]:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
 
     @staticmethod
     def _get_best_filter_type(
         column: str, value: pd.DataFrame
     ) -> Literal["slider", "checkboxgroup", "dropdown", "checkbox"]:
         if is_bool_dtype(value[column]):
             return "checkbox"
```

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/leaderboard.pyi` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,16 @@
         self.wrap = wrap
         self.headers = [str(s) for s in value.columns]
         self.datatype = datatype
         self.search_columns = self._get_search_columns(search_columns)
         self.bool_checkboxgroup_label = bool_checkboxgroup_label
         self.select_columns_config = self._get_select_columns(select_columns, value)
         self.filter_columns = self._get_column_filter_configs(filter_columns, value)
+        self.raise_error_if_incorrect_config()
+
         self.hide_columns = hide_columns or []
         self.col_count = (len(self.headers), "fixed")
         self.row_count = (value.shape[0], "fixed")
 
         if latex_delimiters is None:
             latex_delimiters = [{"left": "$$", "right": "$$", "display": True}]
         self.latex_delimiters = latex_delimiters
@@ -149,14 +151,25 @@
             interactive=interactive,
             visible=visible,
             elem_id=elem_id,
             elem_classes=elem_classes,
             render=render,
             value=value,
         )
+    
+    def raise_error_if_incorrect_config(self):
+        for col in [self.search_columns.primary_column, *self.search_columns.secondary_columns]:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
+        for col in self.select_columns_config.default_selection + self.select_columns_config.cant_deselect:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
+        for col in [col.column for col in self.filter_columns]:
+            if col not in self.headers:
+                raise ValueError(f"Column '{col}' not found in the DataFrame headers.")
 
     @staticmethod
     def _get_best_filter_type(
         column: str, value: pd.DataFrame
     ) -> Literal["slider", "checkboxgroup", "dropdown", "checkbox"]:
         if is_bool_dtype(value[column]):
             return "checkbox"
```

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/index.js` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1179,33 +1179,33 @@
         formatRows: h,
         formatRow: p,
         formatValue: _
     };
 }
 var zu = Object.prototype.hasOwnProperty;
 
-function Fn(t, e) {
+function Cn(t, e) {
     var n, r;
     if (t === e)
         return !0;
     if (t && e && (n = t.constructor) === e.constructor) {
         if (n === Date)
             return t.getTime() === e.getTime();
         if (n === RegExp)
             return t.toString() === e.toString();
         if (n === Array) {
             if ((r = t.length) === e.length)
-                for (; r-- && Fn(t[r], e[r]);)
+                for (; r-- && Cn(t[r], e[r]);)
             ;
             return r === -1;
         }
         if (!n || typeof t == "object") {
             r = 0;
             for (n in t)
-                if (zu.call(t, n) && ++r && !zu.call(e, n) || !(n in e) || !Fn(t[n], e[n]))
+                if (zu.call(t, n) && ++r && !zu.call(e, n) || !(n in e) || !Cn(t[n], e[n]))
                     return !1;
             return Object.keys(e).length === r;
         }
     }
     return t !== t && e !== e;
 }
 var Ol = new Intl.Collator(0, {
@@ -1391,15 +1391,15 @@
     }) {
         this.meta = {
             _type: "gradio.FileData"
         }, this.path = e, this.url = n, this.orig_name = r, this.size = l, this.blob = n ? void 0 : o, this.is_stream = c, this.mime_type = u, this.alt_text = h;
     }
 }
 const Df = "This application is too busy. Keep trying!",
-    G0 = "Connection errored out.";
+    j0 = "Connection errored out.";
 let Af;
 
 function Tm(t, e) {
     return {
         post_data: n,
         upload_files: r,
         client: l,
@@ -1414,15 +1414,15 @@
             var _ = await t(c, {
                 method: "POST",
                 body: JSON.stringify(u),
                 headers: p
             });
         } catch {
             return [{
-                error: G0
+                error: j0
             }, 500];
         }
         let v, k;
         try {
             v = await _.json(), k = _.status;
         } catch (T) {
             v = {
@@ -1447,15 +1447,15 @@
                 var T = await t(N, {
                     method: "POST",
                     body: U,
                     headers: _
                 });
             } catch {
                 return {
-                    error: G0
+                    error: j0
                 };
             }
             const M = await T.json();
             k.push(...M);
         }
         return {
             files: k
@@ -1466,15 +1466,15 @@
             const {
                 status_callback: p,
                 hf_token: _
             } = u, v = {
                 predict: Ne,
                 submit: ke,
                 view_api: Be,
-                component_server: ae
+                component_server: le
             };
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
                 const oe = await import("./wrapper-6f348d45-19fa94bf.js");
                 Af = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = oe.WebSocket;
             }
             const {
                 ws_protocol: k,
@@ -1667,15 +1667,15 @@
               )}
 							/queue/join${zt ? "?" + zt : ""}`);
                             ne && Ee.searchParams.set("__sign", ne), ve = new WebSocket(Ee), ve.onclose = (me) => {
                                 me.wasClean || Re({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
-                                    message: G0,
+                                    message: j0,
                                     queue: !0,
                                     endpoint: Se,
                                     fn_index: ee,
                                     time: /* @__PURE__ */ new Date()
                                 });
                             }, ve.onmessage = function(me) {
                                 const Oe = JSON.parse(me.data),
@@ -1784,15 +1784,15 @@
                                             event_id: Ie
                                         },
                                         _
                                     );
                                     Rt !== 200 && (Re({
                                         type: "status",
                                         stage: "error",
-                                        message: G0,
+                                        message: j0,
                                         queue: !0,
                                         endpoint: Se,
                                         fn_index: ee,
                                         time: /* @__PURE__ */ new Date()
                                     }), $.close());
                                 } else
                                     et === "complete" ? Xe = Ce : et === "log" ? Re({
@@ -1851,15 +1851,15 @@
                                         fn_index: ee,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else if (me !== 200)
                                     Re({
                                         type: "status",
                                         stage: "error",
-                                        message: G0,
+                                        message: j0,
                                         queue: !0,
                                         endpoint: Se,
                                         fn_index: ee,
                                         time: /* @__PURE__ */ new Date()
                                     });
                                 else {
                                     Ie = Ee.event_id;
@@ -1909,15 +1909,15 @@
                                                     type: "status",
                                                     time: /* @__PURE__ */ new Date(),
                                                     ...Le,
                                                     stage: Le == null ? void 0 : Le.stage,
                                                     queue: !0,
                                                     endpoint: Se,
                                                     fn_index: ee
-                                                }), tt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(xe) && Bn(Ie, tt));
+                                                }), tt && ["sse_v2", "sse_v2.1", "sse_v3"].includes(xe) && Nn(Ie, tt));
                                             tt && (Re({
                                                 type: "data",
                                                 time: /* @__PURE__ */ new Date(),
                                                 data: tt.data,
                                                 endpoint: Se,
                                                 fn_index: ee
                                             }), Xe && Re({
@@ -1945,15 +1945,15 @@
                                         (et) => Oe(et)
                                     ), delete D[Ie]), R[Ie] = Oe, I.add(Ie), N || ce();
                                 }
                             }));
                     }
                 );
 
-                function Bn(ye, Fe) {
+                function Nn(ye, Fe) {
                     !E[ye] ? (E[ye] = [], Fe.data.forEach((me, Oe) => {
                         E[ye][Oe] = me;
                     })) : Fe.data.forEach((me, Oe) => {
                         let et = Sm(
                             E[ye][Oe],
                             me
                         );
@@ -2063,25 +2063,25 @@
                     } else
                         D[ee] || (D[ee] = []), D[ee].push(V);
                 }, C.onerror = async function(de) {
                     await Promise.all(
                         Object.keys(R).map(
                             (V) => R[V]({
                                 msg: "unexpected_error",
-                                message: G0
+                                message: j0
                             })
                         )
                     ), he();
                 };
             }
 
             function he() {
                 N = !1, C == null || C.close();
             }
-            async function ae(oe, Q, de) {
+            async function le(oe, Q, de) {
                 var V;
                 const ee = {
                     "Content-Type": "application/json"
                 };
                 _ && (ee.Authorization = `Bearer ${_}`);
                 let we, ve = z.components.find(
                     (Se) => Se.id === oe
@@ -2121,15 +2121,15 @@
                                 config: JSON.stringify(oe)
                             }),
                             headers: Q
                         }
                     ) : de = await t(`${oe.root}/info`, {
                         headers: Q
                     }), !de.ok)
-                    throw new Error(G0);
+                    throw new Error(j0);
                 let V = await de.json();
                 return "api" in V && (V = V.api), V.named_endpoints["/predict"] && !V.unnamed_endpoints[0] && (V.unnamed_endpoints[0] = V.named_endpoints["/predict"]), Cm(V, oe, Y);
             }
         });
     }
     async function o(c, u, h, p) {
         const _ = await aa(
@@ -2531,15 +2531,15 @@
         status: {
             stage: "error",
             queue: !0
         }
     };
 }
 
-function K0() {}
+function $0() {}
 
 function Nm(t) {
     return t();
 }
 
 function zm(t) {
     t.forEach(Nm);
@@ -2553,15 +2553,15 @@
     return t != t ? e == e : t !== e || t && typeof t == "object" || typeof t == "function";
 }
 
 function Im(t, ...e) {
     if (t == null) {
         for (const r of e)
             r(void 0);
-        return K0;
+        return $0;
     }
     const n = t.subscribe(...e);
     return n.unsubscribe ? () => n.unsubscribe() : n;
 }
 
 function qu(t) {
     const e = typeof t == "string" && t.match(/^\s*(-?[\d.]+)([^\s]*)\s*$/);
@@ -2569,15 +2569,15 @@
         /** @type {number} */
         t,
         "px"
     ];
 }
 const Sf = typeof window < "u";
 let Uu = Sf ? () => window.performance.now() : () => Date.now(),
-    Ef = Sf ? (t) => requestAnimationFrame(t) : K0;
+    Ef = Sf ? (t) => requestAnimationFrame(t) : $0;
 const Er = /* @__PURE__ */ new Set();
 
 function xf(t) {
     Er.forEach((e) => {
         e.c(t) || (Er.delete(e), e.f());
     }), Er.size !== 0 && Ef(xf);
 }
@@ -2629,15 +2629,15 @@
 
 function Pm(t, e) {
     return {
         subscribe: ys(t, e).subscribe
     };
 }
 
-function ys(t, e = K0) {
+function ys(t, e = $0) {
     let n;
     const r = /* @__PURE__ */ new Set();
 
     function l(u) {
         if (Om(t, u) && (t = u, n)) {
             const h = !hr.length;
             for (const p of r)
@@ -2650,17 +2650,17 @@
         }
     }
 
     function o(u) {
         l(u(t));
     }
 
-    function c(u, h = K0) {
+    function c(u, h = $0) {
         const p = [u, h];
-        return r.add(p), r.size === 1 && (n = e(l, o) || K0), u(t), () => {
+        return r.add(p), r.size === 1 && (n = e(l, o) || $0), u(t), () => {
             r.delete(p), r.size === 0 && n && (n(), n = null);
         };
     }
     return {
         set: l,
         update: o,
         subscribe: c
@@ -2673,21 +2673,21 @@
     if (!l.every(Boolean))
         throw new Error("derived() expects stores as input, got a falsy value");
     const o = e.length < 2;
     return Pm(n, (c, u) => {
         let h = !1;
         const p = [];
         let _ = 0,
-            v = K0;
+            v = $0;
         const k = () => {
                 if (_)
                     return;
                 v();
                 const O = e(r ? p[0] : p, c, u);
-                o ? c(O) : v = Rm(O) ? O : K0;
+                o ? c(O) : v = Rm(O) ? O : $0;
             },
             T = l.map(
                 (O, P) => Im(
                     O,
                     (U) => {
                         p[P] = U, _ &= ~(1 << P), h && k();
                     },
@@ -5741,21 +5741,21 @@
                 }
             }
             r = r[n[l]];
         } else
             r = void 0;
     return r;
 }
-const E0 = {},
-    X2 = (t, e, n) => n && (e in E0 || (E0[e] = {}), t in E0[e] || (E0[e][t] = n), n),
+const x0 = {},
+    X2 = (t, e, n) => n && (e in x0 || (x0[e] = {}), t in x0[e] || (x0[e][t] = n), n),
     Vf = (t, e) => {
         if (e == null)
             return;
-        if (e in E0 && t in E0[e])
-            return E0[e][t];
+        if (e in x0 && t in x0[e])
+            return x0[e][t];
         const n = Vi(e);
         for (let r = 0; r < n.length; r++) {
             const l = n[r],
                 o = Z2(l, t);
             if (o)
                 return X2(t, e, o);
         }
@@ -5786,15 +5786,15 @@
         const r = e[n];
         if (Wf(r))
             return r;
     }
 }
 
 function Q2(t, ...e) {
-    delete E0[t], vs.update((n) => (n[t] = t2.all([n[t] || {}, ...e]), n));
+    delete x0[t], vs.update((n) => (n[t] = t2.all([n[t] || {}, ...e]), n));
 }
 zr(
     [vs],
     ([t]) => Object.keys(t)
 );
 vs.subscribe((t) => Ya = t);
 const mi = {};
@@ -5951,27 +5951,27 @@
 }
 
 function Vi(t, e = Cr().fallbackLocale) {
     const n = rc(t);
     return e ? [... /* @__PURE__ */ new Set([...n, ...rc(e)])] : n;
 }
 
-function tr() {
+function nr() {
     return ba ?? void 0;
 }
 Di.subscribe((t) => {
     ba = t ?? void 0, typeof window < "u" && t != null && document.documentElement.setAttribute("lang", t);
 });
 const f3 = (t) => {
         if (t && J2(t) && _a(t)) {
             const {
                 loadingDelay: e
             } = Cr();
             let n;
-            return typeof window < "u" && tr() != null && e ? n = window.setTimeout(
+            return typeof window < "u" && nr() != null && e ? n = window.setTimeout(
                 () => jl.set(!0),
                 e
             ) : jl.set(!0), Yf(t).then(() => {
                 Di.set(t);
             }).finally(() => {
                 clearTimeout(n), jl.set(!1);
             });
@@ -6063,60 +6063,60 @@
                 );
             return r ? l = fs("time", r) : Object.keys(l).length === 0 && (l = fs("time", "short")), new Intl.DateTimeFormat(n, l);
         }
     ),
     g3 = (t = {}) => {
         var e = t,
             {
-                locale: n = tr()
+                locale: n = nr()
             } = e,
             r = Rr(e, [
                 "locale"
             ]);
         return d3(Za({
             locale: n
         }, r));
     },
     _3 = (t = {}) => {
         var e = t,
             {
-                locale: n = tr()
+                locale: n = nr()
             } = e,
             r = Rr(e, [
                 "locale"
             ]);
         return m3(Za({
             locale: n
         }, r));
     },
     b3 = (t = {}) => {
         var e = t,
             {
-                locale: n = tr()
+                locale: n = nr()
             } = e,
             r = Rr(e, [
                 "locale"
             ]);
         return p3(Za({
             locale: n
         }, r));
     },
     w3 = Wi(
         // eslint-disable-next-line @typescript-eslint/no-non-null-assertion
-        (t, e = tr()) => new V2(t, e, Cr().formats, {
+        (t, e = nr()) => new V2(t, e, Cr().formats, {
             ignoreTag: Cr().ignoreTag
         })
     ),
     y3 = (t, e = {}) => {
         var n, r, l, o;
         let c = e;
         typeof t == "object" && (c = t, t = c.id);
         const {
             values: u,
-            locale: h = tr(),
+            locale: h = nr(),
             default: p
         } = c;
         if (h == null)
             throw new Error(
                 "[svelte-i18n] Cannot format a message without first setting the initial locale."
             );
         let _ = Vf(t, h);
@@ -6142,26 +6142,26 @@
             );
         }
         return v;
     },
     v3 = (t, e) => b3(e).format(t),
     k3 = (t, e) => _3(e).format(t),
     D3 = (t, e) => g3(e).format(t),
-    A3 = (t, e = tr()) => Vf(t, e);
+    A3 = (t, e = nr()) => Vf(t, e);
 zr([ks, vs], () => y3);
 zr([ks], () => v3);
 zr([ks], () => k3);
 zr([ks], () => D3);
 zr([ks, vs], () => A3);
 const {
     SvelteComponent: S3,
     append: fn,
-    attr: Y0,
+    attr: Z0,
     detach: Qf,
-    element: Z0,
+    element: J0,
     init: E3,
     insert: Kf,
     noop: ic,
     safe_not_equal: x3,
     set_data: Si,
     set_style: Vl,
     space: wa,
@@ -6181,18 +6181,18 @@
         c, u, h, p, _ = (
             /*file_to_display*/
             t[2].orig_name + ""
         ),
         v;
     return {
         c() {
-            e = Z0("div"), n = Z0("span"), r = Z0("div"), l = Z0("progress"), c = wr(o), h = wa(), p = Z0("span"), v = wr(_), Vl(l, "visibility", "hidden"), Vl(l, "height", "0"), Vl(l, "width", "0"), l.value = u = es(
+            e = J0("div"), n = J0("span"), r = J0("div"), l = J0("progress"), c = wr(o), h = wa(), p = J0("span"), v = wr(_), Vl(l, "visibility", "hidden"), Vl(l, "height", "0"), Vl(l, "width", "0"), l.value = u = es(
                 /*file_to_display*/
                 t[2]
-            ), Y0(l, "max", "100"), Y0(l, "class", "svelte-cr2edf"), Y0(r, "class", "progress-bar svelte-cr2edf"), Y0(p, "class", "file-name svelte-cr2edf"), Y0(e, "class", "file svelte-cr2edf");
+            ), Z0(l, "max", "100"), Z0(l, "class", "svelte-cr2edf"), Z0(r, "class", "progress-bar svelte-cr2edf"), Z0(p, "class", "file-name svelte-cr2edf"), Z0(e, "class", "file svelte-cr2edf");
         },
         m(k, T) {
             Kf(k, e, T), fn(e, n), fn(n, r), fn(r, l), fn(l, c), fn(e, h), fn(e, p), fn(p, v);
         },
         p(k, T) {
             T & /*file_to_display*/
                 4 && o !== (o = es(
@@ -6223,15 +6223,15 @@
         ),
         h, p, _, v = (
             /*file_to_display*/
             t[2] && ac(t)
         );
     return {
         c() {
-            e = Z0("div"), n = Z0("span"), r = wr("Uploading "), o = wr(l), c = wa(), h = wr(u), p = wr("..."), _ = wa(), v && v.c(), Y0(n, "class", "uploading svelte-cr2edf"), Y0(e, "class", "wrap svelte-cr2edf"), lc(
+            e = J0("div"), n = J0("span"), r = wr("Uploading "), o = wr(l), c = wa(), h = wr(u), p = wr("..."), _ = wa(), v && v.c(), Z0(n, "class", "uploading svelte-cr2edf"), Z0(e, "class", "wrap svelte-cr2edf"), lc(
                 e,
                 "progress",
                 /*progress*/
                 t[1]
             );
         },
         m(k, T) {
@@ -6318,38 +6318,38 @@
     }
 }
 const {
     SvelteComponent: R3,
     append: oc,
     attr: Kt,
     binding_callbacks: O3,
-    bubble: j0,
+    bubble: V0,
     check_outros: $f,
     create_component: I3,
     create_slot: eh,
     destroy_component: L3,
     detach: Xi,
     element: ya,
     empty: th,
     get_all_dirty_from_scope: nh,
     get_slot_changes: rh,
     group_outros: sh,
     init: H3,
     insert: Yi,
     listen: _n,
     mount_component: P3,
-    prevent_default: V0,
+    prevent_default: W0,
     run_all: q3,
     safe_not_equal: U3,
     set_style: ih,
     space: G3,
-    stop_propagation: W0,
-    toggle_class: Ut,
-    transition_in: C0,
-    transition_out: $0,
+    stop_propagation: X0,
+    toggle_class: Gt,
+    transition_in: M0,
+    transition_out: er,
     update_slot_base: lh
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: j3,
     tick: V3,
     getContext: W3
 } = window.__gradio__svelte__internal;
 
@@ -6369,74 +6369,74 @@
     return {
         c() {
             e = ya("button"), T && T.c(), n = G3(), r = ya("input"), Kt(r, "aria-label", "file upload"), Kt(r, "data-testid", "file-upload"), Kt(r, "type", "file"), Kt(r, "accept", l = /*accept_file_types*/
                     t[14] || void 0), r.multiple = o = /*file_count*/
                 t[6] === "multiple" || void 0, Kt(r, "webkitdirectory", c = /*file_count*/
                     t[6] === "directory" || void 0), Kt(r, "mozdirectory", u = /*file_count*/
                     t[6] === "directory" || void 0), Kt(r, "class", "svelte-1s26xmt"), Kt(e, "tabindex", h = /*hidden*/
-                    t[9] ? -1 : 0), Kt(e, "class", "svelte-1s26xmt"), Ut(
+                    t[9] ? -1 : 0), Kt(e, "class", "svelte-1s26xmt"), Gt(
                     e,
                     "hidden",
                     /*hidden*/
                     t[9]
-                ), Ut(
+                ), Gt(
                     e,
                     "center",
                     /*center*/
                     t[4]
-                ), Ut(
+                ), Gt(
                     e,
                     "boundedheight",
                     /*boundedheight*/
                     t[3]
-                ), Ut(
+                ), Gt(
                     e,
                     "flex",
                     /*flex*/
                     t[5]
-                ), Ut(
+                ), Gt(
                     e,
                     "disable_click",
                     /*disable_click*/
                     t[7]
                 ), ih(e, "height", "100%");
         },
         m(O, P) {
             Yi(O, e, P), T && T.m(e, null), oc(e, n), oc(e, r), t[30](r), p = !0, _ || (v = [
                 _n(
                     r,
                     "change",
                     /*load_files_from_upload*/
                     t[16]
                 ),
-                _n(e, "drag", W0(V0(
+                _n(e, "drag", X0(W0(
                     /*drag_handler*/
                     t[23]
                 ))),
-                _n(e, "dragstart", W0(V0(
+                _n(e, "dragstart", X0(W0(
                     /*dragstart_handler*/
                     t[24]
                 ))),
-                _n(e, "dragend", W0(V0(
+                _n(e, "dragend", X0(W0(
                     /*dragend_handler*/
                     t[25]
                 ))),
-                _n(e, "dragover", W0(V0(
+                _n(e, "dragover", X0(W0(
                     /*dragover_handler*/
                     t[26]
                 ))),
-                _n(e, "dragenter", W0(V0(
+                _n(e, "dragenter", X0(W0(
                     /*dragenter_handler*/
                     t[27]
                 ))),
-                _n(e, "dragleave", W0(V0(
+                _n(e, "dragleave", X0(W0(
                     /*dragleave_handler*/
                     t[28]
                 ))),
-                _n(e, "drop", W0(V0(
+                _n(e, "drop", X0(W0(
                     /*drop_handler*/
                     t[29]
                 ))),
                 _n(
                     e,
                     "click",
                     /*open_file_upload*/
@@ -6488,50 +6488,50 @@
                     O[6] === "multiple" || void 0)) && (r.multiple = o), (!p || P[0] & /*file_count*/
                 64 && c !== (c = /*file_count*/
                     O[6] === "directory" || void 0)) && Kt(r, "webkitdirectory", c), (!p || P[0] & /*file_count*/
                 64 && u !== (u = /*file_count*/
                     O[6] === "directory" || void 0)) && Kt(r, "mozdirectory", u), (!p || P[0] & /*hidden*/
                 512 && h !== (h = /*hidden*/
                     O[9] ? -1 : 0)) && Kt(e, "tabindex", h), (!p || P[0] & /*hidden*/
-                512) && Ut(
+                512) && Gt(
                 e,
                 "hidden",
                 /*hidden*/
                 O[9]
             ), (!p || P[0] & /*center*/
-                16) && Ut(
+                16) && Gt(
                 e,
                 "center",
                 /*center*/
                 O[4]
             ), (!p || P[0] & /*boundedheight*/
-                8) && Ut(
+                8) && Gt(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 O[3]
             ), (!p || P[0] & /*flex*/
-                32) && Ut(
+                32) && Gt(
                 e,
                 "flex",
                 /*flex*/
                 O[5]
             ), (!p || P[0] & /*disable_click*/
-                128) && Ut(
+                128) && Gt(
                 e,
                 "disable_click",
                 /*disable_click*/
                 O[7]
             );
         },
         i(O) {
-            p || (C0(T, O), p = !0);
+            p || (M0(T, O), p = !0);
         },
         o(O) {
-            $0(T, O), p = !1;
+            er(T, O), p = !1;
         },
         d(O) {
             O && Xi(e), T && T.d(O), t[30](null), _ = !1, q3(v);
         }
     };
 }
 
@@ -6543,24 +6543,24 @@
             r && r.c(), e = th();
         },
         m(l, o) {
             r && r.m(l, o), Yi(l, e, o), n = !0;
         },
         p(l, o) {
             /*hidden*/
-            l[9] ? r && (sh(), $0(r, 1, 1, () => {
+            l[9] ? r && (sh(), er(r, 1, 1, () => {
                 r = null;
             }), $f()) : r ? (r.p(l, o), o[0] & /*hidden*/
-                512 && C0(r, 1)) : (r = uc(l), r.c(), C0(r, 1), r.m(e.parentNode, e));
+                512 && M0(r, 1)) : (r = uc(l), r.c(), M0(r, 1), r.m(e.parentNode, e));
         },
         i(l) {
-            n || (C0(r), n = !0);
+            n || (M0(r), n = !0);
         },
         o(l) {
-            $0(r), n = !1;
+            er(r), n = !1;
         },
         d(l) {
             l && Xi(e), r && r.d(l);
         }
     };
 }
 
@@ -6576,30 +6576,30 @@
             /*$$scope*/
             t[21],
             null
         );
     return {
         c() {
             e = ya("button"), u && u.c(), Kt(e, "tabindex", n = /*hidden*/
-                t[9] ? -1 : 0), Kt(e, "class", "svelte-1s26xmt"), Ut(
+                t[9] ? -1 : 0), Kt(e, "class", "svelte-1s26xmt"), Gt(
                 e,
                 "hidden",
                 /*hidden*/
                 t[9]
-            ), Ut(
+            ), Gt(
                 e,
                 "center",
                 /*center*/
                 t[4]
-            ), Ut(
+            ), Gt(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 t[3]
-            ), Ut(
+            ), Gt(
                 e,
                 "flex",
                 /*flex*/
                 t[5]
             ), ih(e, "height", "100%");
         },
         m(h, p) {
@@ -6628,44 +6628,44 @@
                     /*$$scope*/
                     h[21]
                 ),
                 null
             ), (!r || p[0] & /*hidden*/
                 512 && n !== (n = /*hidden*/
                     h[9] ? -1 : 0)) && Kt(e, "tabindex", n), (!r || p[0] & /*hidden*/
-                512) && Ut(
+                512) && Gt(
                 e,
                 "hidden",
                 /*hidden*/
                 h[9]
             ), (!r || p[0] & /*center*/
-                16) && Ut(
+                16) && Gt(
                 e,
                 "center",
                 /*center*/
                 h[4]
             ), (!r || p[0] & /*boundedheight*/
-                8) && Ut(
+                8) && Gt(
                 e,
                 "boundedheight",
                 /*boundedheight*/
                 h[3]
             ), (!r || p[0] & /*flex*/
-                32) && Ut(
+                32) && Gt(
                 e,
                 "flex",
                 /*flex*/
                 h[5]
             );
         },
         i(h) {
-            r || (C0(u, h), r = !0);
+            r || (M0(u, h), r = !0);
         },
         o(h) {
-            $0(u, h), r = !1;
+            er(u, h), r = !1;
         },
         d(h) {
             h && Xi(e), u && u.d(h), l = !1, o();
         }
     };
 }
 
@@ -6700,18 +6700,18 @@
                     r[8]), l[0] & /*upload_id*/
                 4096 && (o.upload_id = /*upload_id*/
                     r[12]), l[0] & /*file_data*/
                 8192 && (o.files = /*file_data*/
                     r[13]), e.$set(o);
         },
         i(r) {
-            n || (C0(e.$$.fragment, r), n = !0);
+            n || (M0(e.$$.fragment, r), n = !0);
         },
         o(r) {
-            $0(e.$$.fragment, r), n = !1;
+            er(e.$$.fragment, r), n = !1;
         },
         d(r) {
             L3(e, r);
         }
     };
 }
 
@@ -6735,23 +6735,23 @@
             n.c(), r = th();
         },
         m(h, p) {
             c[e].m(h, p), Yi(h, r, p), l = !0;
         },
         p(h, p) {
             let _ = e;
-            e = u(h), e === _ ? c[e].p(h, p) : (sh(), $0(c[_], 1, 1, () => {
+            e = u(h), e === _ ? c[e].p(h, p) : (sh(), er(c[_], 1, 1, () => {
                 c[_] = null;
-            }), $f(), n = c[e], n ? n.p(h, p) : (n = c[e] = o[e](h), n.c()), C0(n, 1), n.m(r.parentNode, r));
+            }), $f(), n = c[e], n ? n.p(h, p) : (n = c[e] = o[e](h), n.c()), M0(n, 1), n.m(r.parentNode, r));
         },
         i(h) {
-            l || (C0(n), l = !0);
+            l || (M0(n), l = !0);
         },
         o(h) {
-            $0(n), l = !1;
+            er(n), l = !1;
         },
         d(h) {
             h && Xi(r), c[e].d(h);
         }
     };
 }
 
@@ -6873,39 +6873,39 @@
             const ve = "." + we.name.split(".").pop();
             return ve && Q3(D, ve, we.type) || (ve && Array.isArray(o) ? o.includes(ve) : ve === o) ? !0 : (C("error", `Invalid file type only ${o} allowed.`), !1);
         });
         await pe(ee);
     }
 
     function ke(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
     function ce(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
     function he(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
-    function ae(V) {
-        j0.call(this, t, V);
+    function le(V) {
+        V0.call(this, t, V);
     }
 
     function Be(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
     function oe(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
     function Q(V) {
-        j0.call(this, t, V);
+        V0.call(this, t, V);
     }
 
     function de(V) {
         O3[V ? "unshift" : "push"](() => {
             U = V, n(2, U);
         });
     }
@@ -6937,15 +6937,15 @@
         O,
         pe,
         l,
         r,
         ke,
         ce,
         he,
-        ae,
+        le,
         Be,
         oe,
         Q,
         de
     ];
 }
 class $3 extends R3 {
@@ -7428,24 +7428,24 @@
     setPrototypeOf: dc,
     isFrozen: hp,
     getPrototypeOf: dp,
     getOwnPropertyDescriptor: mp
 } = Object;
 let {
     freeze: rn,
-    seal: Cn,
+    seal: Mn,
     create: ph
 } = Object, {
     apply: va,
     construct: ka
 } = typeof Reflect < "u" && Reflect;
 rn || (rn = function(e) {
     return e;
 });
-Cn || (Cn = function(e) {
+Mn || (Mn = function(e) {
     return e;
 });
 va || (va = function(e, n, r) {
     return e.apply(n, r);
 });
 ka || (ka = function(e, n) {
     return new e(...n);
@@ -7496,18 +7496,18 @@
 
 function bp(t) {
     for (let e = 0; e < t.length; e++)
         Ln(t, e) || (t[e] = null);
     return t;
 }
 
-function X0(t) {
+function Y0(t) {
     const e = ph(null);
     for (const [n, r] of mh(t))
-        Ln(t, n) && (Array.isArray(r) ? e[n] = bp(r) : r && typeof r == "object" && r.constructor === Object ? e[n] = X0(r) : e[n] = r);
+        Ln(t, n) && (Array.isArray(r) ? e[n] = bp(r) : r && typeof r == "object" && r.constructor === Object ? e[n] = Y0(r) : e[n] = r);
     return e;
 }
 
 function Xs(t, e) {
     for (; t !== null;) {
         const r = mp(t, e);
         if (r) {
@@ -7531,30 +7531,30 @@
     Zl = rn(["math", "menclose", "merror", "mfenced", "mfrac", "mglyph", "mi", "mlabeledtr", "mmultiscripts", "mn", "mo", "mover", "mpadded", "mphantom", "mroot", "mrow", "ms", "mspace", "msqrt", "mstyle", "msub", "msup", "msubsup", "mtable", "mtd", "mtext", "mtr", "munder", "munderover", "mprescripts"]),
     yp = rn(["maction", "maligngroup", "malignmark", "mlongdiv", "mscarries", "mscarry", "msgroup", "mstack", "msline", "msrow", "semantics", "annotation", "annotation-xml", "mprescripts", "none"]),
     _c = rn(["#text"]),
     bc = rn(["accept", "action", "align", "alt", "autocapitalize", "autocomplete", "autopictureinpicture", "autoplay", "background", "bgcolor", "border", "capture", "cellpadding", "cellspacing", "checked", "cite", "class", "clear", "color", "cols", "colspan", "controls", "controlslist", "coords", "crossorigin", "datetime", "decoding", "default", "dir", "disabled", "disablepictureinpicture", "disableremoteplayback", "download", "draggable", "enctype", "enterkeyhint", "face", "for", "headers", "height", "hidden", "high", "href", "hreflang", "id", "inputmode", "integrity", "ismap", "kind", "label", "lang", "list", "loading", "loop", "low", "max", "maxlength", "media", "method", "min", "minlength", "multiple", "muted", "name", "nonce", "noshade", "novalidate", "nowrap", "open", "optimum", "pattern", "placeholder", "playsinline", "poster", "preload", "pubdate", "radiogroup", "readonly", "rel", "required", "rev", "reversed", "role", "rows", "rowspan", "spellcheck", "scope", "selected", "shape", "size", "sizes", "span", "srclang", "start", "src", "srcset", "step", "style", "summary", "tabindex", "title", "translate", "type", "usemap", "valign", "value", "width", "wrap", "xmlns", "slot"]),
     Jl = rn(["accent-height", "accumulate", "additive", "alignment-baseline", "ascent", "attributename", "attributetype", "azimuth", "basefrequency", "baseline-shift", "begin", "bias", "by", "class", "clip", "clippathunits", "clip-path", "clip-rule", "color", "color-interpolation", "color-interpolation-filters", "color-profile", "color-rendering", "cx", "cy", "d", "dx", "dy", "diffuseconstant", "direction", "display", "divisor", "dur", "edgemode", "elevation", "end", "fill", "fill-opacity", "fill-rule", "filter", "filterunits", "flood-color", "flood-opacity", "font-family", "font-size", "font-size-adjust", "font-stretch", "font-style", "font-variant", "font-weight", "fx", "fy", "g1", "g2", "glyph-name", "glyphref", "gradientunits", "gradienttransform", "height", "href", "id", "image-rendering", "in", "in2", "k", "k1", "k2", "k3", "k4", "kerning", "keypoints", "keysplines", "keytimes", "lang", "lengthadjust", "letter-spacing", "kernelmatrix", "kernelunitlength", "lighting-color", "local", "marker-end", "marker-mid", "marker-start", "markerheight", "markerunits", "markerwidth", "maskcontentunits", "maskunits", "max", "mask", "media", "method", "mode", "min", "name", "numoctaves", "offset", "operator", "opacity", "order", "orient", "orientation", "origin", "overflow", "paint-order", "path", "pathlength", "patterncontentunits", "patterntransform", "patternunits", "points", "preservealpha", "preserveaspectratio", "primitiveunits", "r", "rx", "ry", "radius", "refx", "refy", "repeatcount", "repeatdur", "restart", "result", "rotate", "scale", "seed", "shape-rendering", "specularconstant", "specularexponent", "spreadmethod", "startoffset", "stddeviation", "stitchtiles", "stop-color", "stop-opacity", "stroke-dasharray", "stroke-dashoffset", "stroke-linecap", "stroke-linejoin", "stroke-miterlimit", "stroke-opacity", "stroke", "stroke-width", "style", "surfacescale", "systemlanguage", "tabindex", "targetx", "targety", "transform", "transform-origin", "text-anchor", "text-decoration", "text-rendering", "textlength", "type", "u1", "u2", "unicode", "values", "viewbox", "visibility", "version", "vert-adv-y", "vert-origin-x", "vert-origin-y", "width", "word-spacing", "wrap", "writing-mode", "xchannelselector", "ychannelselector", "x", "x1", "x2", "xmlns", "y", "y1", "y2", "z", "zoomandpan"]),
     wc = rn(["accent", "accentunder", "align", "bevelled", "close", "columnsalign", "columnlines", "columnspan", "denomalign", "depth", "dir", "display", "displaystyle", "encoding", "fence", "frame", "height", "href", "id", "largeop", "length", "linethickness", "lspace", "lquote", "mathbackground", "mathcolor", "mathsize", "mathvariant", "maxsize", "minsize", "movablelimits", "notation", "numalign", "open", "rowalign", "rowlines", "rowspacing", "rowspan", "rspace", "rquote", "scriptlevel", "scriptminsize", "scriptsizemultiplier", "selection", "separator", "separators", "stretchy", "subscriptshift", "supscriptshift", "symmetric", "voffset", "width", "xmlns"]),
     Ys = rn(["xlink:href", "xml:id", "xlink:title", "xml:space", "xmlns:xlink"]),
-    vp = Cn(/\{\{[\w\W]*|[\w\W]*\}\}/gm),
-    kp = Cn(/<%[\w\W]*|[\w\W]*%>/gm),
-    Dp = Cn(/\${[\w\W]*}/gm),
-    Ap = Cn(/^data-[\-\w.\u00B7-\uFFFF]/),
-    Sp = Cn(/^aria-[\-\w]+$/),
-    gh = Cn(
+    vp = Mn(/\{\{[\w\W]*|[\w\W]*\}\}/gm),
+    kp = Mn(/<%[\w\W]*|[\w\W]*%>/gm),
+    Dp = Mn(/\${[\w\W]*}/gm),
+    Ap = Mn(/^data-[\-\w.\u00B7-\uFFFF]/),
+    Sp = Mn(/^aria-[\-\w]+$/),
+    gh = Mn(
         /^(?:(?:(?:f|ht)tps?|mailto|tel|callto|sms|cid|xmpp):|[^a-z]|[a-z+.\-]+(?:[^a-z+.\-:]|$))/i
         // eslint-disable-line no-useless-escape
     ),
-    Ep = Cn(/^(?:\w+script|data):/i),
-    xp = Cn(
+    Ep = Mn(/^(?:\w+script|data):/i),
+    xp = Mn(
         /[\u0000-\u0020\u00A0\u1680\u180E\u2000-\u2029\u205F\u3000]/g
         // eslint-disable-line no-control-regex
     ),
-    _h = Cn(/^html$/i),
-    Tp = Cn(/^[a-z][.\w]*(-[.\w]+)+$/i);
+    _h = Mn(/^html$/i),
+    Tp = Mn(/^[a-z][.\w]*(-[.\w]+)+$/i);
 var yc = /* @__PURE__ */ Object.freeze({
     __proto__: null,
     MUSTACHE_EXPR: vp,
     ERB_EXPR: kp,
     TMPLIT_EXPR: Dp,
     DATA_ATTR: Ap,
     ARIA_ATTR: Sp,
@@ -7633,15 +7633,15 @@
         MUSTACHE_EXPR: re,
         ERB_EXPR: pe,
         TMPLIT_EXPR: Me,
         DATA_ATTR: Ne,
         ARIA_ATTR: ke,
         IS_SCRIPT_OR_DATA: ce,
         ATTR_WHITESPACE: he,
-        CUSTOM_ELEMENT: ae
+        CUSTOM_ELEMENT: le
     } = yc;
     let {
         IS_ALLOWED_URI: Be
     } = yc, oe = null;
     const Q = Ve({}, [...gc, ...Xl, ...Yl, ...Zl, ..._c]);
     let de = null;
     const V = Ve({}, [...bc, ...Jl, ...wc, ...Ys]);
@@ -7671,15 +7671,15 @@
         xe = !0,
         Se = !1,
         We = !0,
         Ie = !1,
         Xe = !0,
         Ue = !1,
         zt = !1,
-        Bn = !1,
+        Nn = !1,
         Re = !1,
         $t = !1,
         Ot = !1,
         Ct = !0,
         K = !1;
     const ye = "user-content-";
     let Fe = !0,
@@ -7688,128 +7688,128 @@
         Oe = null;
     const et = Ve({}, ["annotation-xml", "audio", "colgroup", "desc", "foreignobject", "head", "iframe", "math", "mi", "mn", "mo", "ms", "mtext", "noembed", "noframes", "noscript", "plaintext", "script", "style", "svg", "template", "thead", "title", "video", "xmp"]);
     let Ce = null;
     const Le = Ve({}, ["audio", "video", "img", "source", "image", "track"]);
     let tt = null;
     const Rt = Ve({}, ["alt", "class", "for", "id", "label", "name", "pattern", "placeholder", "role", "summary", "title", "value", "style", "xmlns"]),
         Jt = "http://www.w3.org/1998/Math/MathML",
-        Nn = "http://www.w3.org/2000/svg",
+        kn = "http://www.w3.org/2000/svg",
         It = "http://www.w3.org/1999/xhtml";
     let Ze = It,
-        ie = !1,
-        Gt = null;
-    const rr = Ve({}, [Jt, Nn, It], Wl);
+        ae = !1,
+        Ut = null;
+    const s0 = Ve({}, [Jt, kn, It], Wl);
     let Pn = null;
     const sr = ["application/xhtml+xml", "text/html"],
-        s0 = "text/html";
+        i0 = "text/html";
     let wt = null,
         qn = null;
     const Ir = n.createElement("form"),
         jt = function(G) {
             return G instanceof RegExp || G instanceof Function;
         },
         en = function() {
             let G = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
             if (!(qn && qn === G)) {
-                if ((!G || typeof G != "object") && (G = {}), G = X0(G), Pn = // eslint-disable-next-line unicorn/prefer-includes
-                    sr.indexOf(G.PARSER_MEDIA_TYPE) === -1 ? s0 : G.PARSER_MEDIA_TYPE, wt = Pn === "application/xhtml+xml" ? Wl : pi, oe = Ln(G, "ALLOWED_TAGS") ? Ve({}, G.ALLOWED_TAGS, wt) : Q, de = Ln(G, "ALLOWED_ATTR") ? Ve({}, G.ALLOWED_ATTR, wt) : V, Gt = Ln(G, "ALLOWED_NAMESPACES") ? Ve({}, G.ALLOWED_NAMESPACES, Wl) : rr, tt = Ln(G, "ADD_URI_SAFE_ATTR") ? Ve(
-                        X0(Rt),
+                if ((!G || typeof G != "object") && (G = {}), G = Y0(G), Pn = // eslint-disable-next-line unicorn/prefer-includes
+                    sr.indexOf(G.PARSER_MEDIA_TYPE) === -1 ? i0 : G.PARSER_MEDIA_TYPE, wt = Pn === "application/xhtml+xml" ? Wl : pi, oe = Ln(G, "ALLOWED_TAGS") ? Ve({}, G.ALLOWED_TAGS, wt) : Q, de = Ln(G, "ALLOWED_ATTR") ? Ve({}, G.ALLOWED_ATTR, wt) : V, Ut = Ln(G, "ALLOWED_NAMESPACES") ? Ve({}, G.ALLOWED_NAMESPACES, Wl) : s0, tt = Ln(G, "ADD_URI_SAFE_ATTR") ? Ve(
+                        Y0(Rt),
                         // eslint-disable-line indent
                         G.ADD_URI_SAFE_ATTR,
                         // eslint-disable-line indent
                         wt
                         // eslint-disable-line indent
                     ) : Rt, Ce = Ln(G, "ADD_DATA_URI_TAGS") ? Ve(
-                        X0(Le),
+                        Y0(Le),
                         // eslint-disable-line indent
                         G.ADD_DATA_URI_TAGS,
                         // eslint-disable-line indent
                         wt
                         // eslint-disable-line indent
-                    ) : Le, Oe = Ln(G, "FORBID_CONTENTS") ? Ve({}, G.FORBID_CONTENTS, wt) : et, we = Ln(G, "FORBID_TAGS") ? Ve({}, G.FORBID_TAGS, wt) : {}, ve = Ln(G, "FORBID_ATTR") ? Ve({}, G.FORBID_ATTR, wt) : {}, me = Ln(G, "USE_PROFILES") ? G.USE_PROFILES : !1, $ = G.ALLOW_ARIA_ATTR !== !1, xe = G.ALLOW_DATA_ATTR !== !1, Se = G.ALLOW_UNKNOWN_PROTOCOLS || !1, We = G.ALLOW_SELF_CLOSE_IN_ATTR !== !1, Ie = G.SAFE_FOR_TEMPLATES || !1, Xe = G.SAFE_FOR_XML !== !1, Ue = G.WHOLE_DOCUMENT || !1, Re = G.RETURN_DOM || !1, $t = G.RETURN_DOM_FRAGMENT || !1, Ot = G.RETURN_TRUSTED_TYPE || !1, Bn = G.FORCE_BODY || !1, Ct = G.SANITIZE_DOM !== !1, K = G.SANITIZE_NAMED_PROPS || !1, Fe = G.KEEP_CONTENT !== !1, Ee = G.IN_PLACE || !1, Be = G.ALLOWED_URI_REGEXP || gh, Ze = G.NAMESPACE || It, ee = G.CUSTOM_ELEMENT_HANDLING || {}, G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (ee.tagNameCheck = G.CUSTOM_ELEMENT_HANDLING.tagNameCheck), G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (ee.attributeNameCheck = G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), G.CUSTOM_ELEMENT_HANDLING && typeof G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (ee.allowCustomizedBuiltInElements = G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), Ie && (xe = !1), $t && (Re = !0), me && (oe = Ve({}, _c), de = [], me.html === !0 && (Ve(oe, gc), Ve(de, bc)), me.svg === !0 && (Ve(oe, Xl), Ve(de, Jl), Ve(de, Ys)), me.svgFilters === !0 && (Ve(oe, Yl), Ve(de, Jl), Ve(de, Ys)), me.mathMl === !0 && (Ve(oe, Zl), Ve(de, wc), Ve(de, Ys))), G.ADD_TAGS && (oe === Q && (oe = X0(oe)), Ve(oe, G.ADD_TAGS, wt)), G.ADD_ATTR && (de === V && (de = X0(de)), Ve(de, G.ADD_ATTR, wt)), G.ADD_URI_SAFE_ATTR && Ve(tt, G.ADD_URI_SAFE_ATTR, wt), G.FORBID_CONTENTS && (Oe === et && (Oe = X0(Oe)), Ve(Oe, G.FORBID_CONTENTS, wt)), Fe && (oe["#text"] = !0), Ue && Ve(oe, ["html", "head", "body"]), oe.table && (Ve(oe, ["tbody"]), delete we.tbody), G.TRUSTED_TYPES_POLICY) {
+                    ) : Le, Oe = Ln(G, "FORBID_CONTENTS") ? Ve({}, G.FORBID_CONTENTS, wt) : et, we = Ln(G, "FORBID_TAGS") ? Ve({}, G.FORBID_TAGS, wt) : {}, ve = Ln(G, "FORBID_ATTR") ? Ve({}, G.FORBID_ATTR, wt) : {}, me = Ln(G, "USE_PROFILES") ? G.USE_PROFILES : !1, $ = G.ALLOW_ARIA_ATTR !== !1, xe = G.ALLOW_DATA_ATTR !== !1, Se = G.ALLOW_UNKNOWN_PROTOCOLS || !1, We = G.ALLOW_SELF_CLOSE_IN_ATTR !== !1, Ie = G.SAFE_FOR_TEMPLATES || !1, Xe = G.SAFE_FOR_XML !== !1, Ue = G.WHOLE_DOCUMENT || !1, Re = G.RETURN_DOM || !1, $t = G.RETURN_DOM_FRAGMENT || !1, Ot = G.RETURN_TRUSTED_TYPE || !1, Nn = G.FORCE_BODY || !1, Ct = G.SANITIZE_DOM !== !1, K = G.SANITIZE_NAMED_PROPS || !1, Fe = G.KEEP_CONTENT !== !1, Ee = G.IN_PLACE || !1, Be = G.ALLOWED_URI_REGEXP || gh, Ze = G.NAMESPACE || It, ee = G.CUSTOM_ELEMENT_HANDLING || {}, G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (ee.tagNameCheck = G.CUSTOM_ELEMENT_HANDLING.tagNameCheck), G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (ee.attributeNameCheck = G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), G.CUSTOM_ELEMENT_HANDLING && typeof G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (ee.allowCustomizedBuiltInElements = G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), Ie && (xe = !1), $t && (Re = !0), me && (oe = Ve({}, _c), de = [], me.html === !0 && (Ve(oe, gc), Ve(de, bc)), me.svg === !0 && (Ve(oe, Xl), Ve(de, Jl), Ve(de, Ys)), me.svgFilters === !0 && (Ve(oe, Yl), Ve(de, Jl), Ve(de, Ys)), me.mathMl === !0 && (Ve(oe, Zl), Ve(de, wc), Ve(de, Ys))), G.ADD_TAGS && (oe === Q && (oe = Y0(oe)), Ve(oe, G.ADD_TAGS, wt)), G.ADD_ATTR && (de === V && (de = Y0(de)), Ve(de, G.ADD_ATTR, wt)), G.ADD_URI_SAFE_ATTR && Ve(tt, G.ADD_URI_SAFE_ATTR, wt), G.FORBID_CONTENTS && (Oe === et && (Oe = Y0(Oe)), Ve(Oe, G.FORBID_CONTENTS, wt)), Fe && (oe["#text"] = !0), Ue && Ve(oe, ["html", "head", "body"]), oe.table && (Ve(oe, ["tbody"]), delete we.tbody), G.TRUSTED_TYPES_POLICY) {
                     if (typeof G.TRUSTED_TYPES_POLICY.createHTML != "function")
                         throw Yr('TRUSTED_TYPES_POLICY configuration option must provide a "createHTML" hook.');
                     if (typeof G.TRUSTED_TYPES_POLICY.createScriptURL != "function")
                         throw Yr('TRUSTED_TYPES_POLICY configuration option must provide a "createScriptURL" hook.');
                     D = G.TRUSTED_TYPES_POLICY, E = D.createHTML("");
                 } else
                     D === void 0 && (D = Cp(T, l)), D !== null && typeof E == "string" && (E = D.createHTML(""));
                 rn && rn(G), qn = G;
             }
         },
         dn = Ve({}, ["mi", "mo", "mn", "ms", "mtext"]),
-        p0 = Ve({}, ["foreignobject", "desc", "title", "annotation-xml"]),
+        g0 = Ve({}, ["foreignobject", "desc", "title", "annotation-xml"]),
         ir = Ve({}, ["title", "style", "font", "a", "script"]),
         lr = Ve({}, [...Xl, ...Yl, ...wp]),
         ar = Ve({}, [...Zl, ...yp]),
         Lr = function(G) {
-            let le = N(G);
-            (!le || !le.tagName) && (le = {
+            let ie = N(G);
+            (!ie || !ie.tagName) && (ie = {
                 namespaceURI: Ze,
                 tagName: "template"
             });
             const x = pi(G.tagName),
-                Ye = pi(le.tagName);
-            return Gt[G.namespaceURI] ? G.namespaceURI === Nn ? le.namespaceURI === It ? x === "svg" : le.namespaceURI === Jt ? x === "svg" && (Ye === "annotation-xml" || dn[Ye]) : !!lr[x] : G.namespaceURI === Jt ? le.namespaceURI === It ? x === "math" : le.namespaceURI === Nn ? x === "math" && p0[Ye] : !!ar[x] : G.namespaceURI === It ? le.namespaceURI === Nn && !p0[Ye] || le.namespaceURI === Jt && !dn[Ye] ? !1 : !ar[x] && (ir[x] || !lr[x]) : !!(Pn === "application/xhtml+xml" && Gt[G.namespaceURI]) : !1;
+                Ye = pi(ie.tagName);
+            return Ut[G.namespaceURI] ? G.namespaceURI === kn ? ie.namespaceURI === It ? x === "svg" : ie.namespaceURI === Jt ? x === "svg" && (Ye === "annotation-xml" || dn[Ye]) : !!lr[x] : G.namespaceURI === Jt ? ie.namespaceURI === It ? x === "math" : ie.namespaceURI === kn ? x === "math" && g0[Ye] : !!ar[x] : G.namespaceURI === It ? ie.namespaceURI === kn && !g0[Ye] || ie.namespaceURI === Jt && !dn[Ye] ? !1 : !ar[x] && (ir[x] || !lr[x]) : !!(Pn === "application/xhtml+xml" && Ut[G.namespaceURI]) : !1;
         },
         Qt = function(G) {
             Wr(e.removed, {
                 element: G
             });
             try {
                 G.parentNode.removeChild(G);
             } catch {
                 G.remove();
             }
         },
-        q = function(G, le) {
+        q = function(G, ie) {
             try {
                 Wr(e.removed, {
-                    attribute: le.getAttributeNode(G),
-                    from: le
+                    attribute: ie.getAttributeNode(G),
+                    from: ie
                 });
             } catch {
                 Wr(e.removed, {
                     attribute: null,
-                    from: le
+                    from: ie
                 });
             }
-            if (le.removeAttribute(G), G === "is" && !de[G])
+            if (ie.removeAttribute(G), G === "is" && !de[G])
                 if (Re || $t)
                     try {
-                        Qt(le);
+                        Qt(ie);
                     } catch {}
             else
                 try {
-                    le.setAttribute(G, "");
+                    ie.setAttribute(G, "");
                 } catch {}
         },
         d = function(G) {
-            let le = null,
+            let ie = null,
                 x = null;
-            if (Bn)
+            if (Nn)
                 G = "<remove></remove>" + G;
             else {
                 const Lt = pc(G, /^[\r\n\t ]+/);
                 x = Lt && Lt[0];
             }
             Pn === "application/xhtml+xml" && Ze === It && (G = '<html xmlns="http://www.w3.org/1999/xhtml"><head></head><body>' + G + "</body></html>");
             const Ye = D ? D.createHTML(G) : G;
             if (Ze === It)
                 try {
-                    le = new k().parseFromString(Ye, Pn);
+                    ie = new k().parseFromString(Ye, Pn);
                 } catch {}
-            if (!le || !le.documentElement) {
-                le = C.createDocument(Ze, "template", null);
+            if (!ie || !ie.documentElement) {
+                ie = C.createDocument(Ze, "template", null);
                 try {
-                    le.documentElement.innerHTML = ie ? E : Ye;
+                    ie.documentElement.innerHTML = ae ? E : Ye;
                 } catch {}
             }
-            const H = le.body || le.documentElement;
-            return G && x && H.insertBefore(n.createTextNode(x), H.childNodes[0] || null), Ze === It ? z.call(le, Ue ? "html" : "body")[0] : Ue ? le.documentElement : H;
+            const H = ie.body || ie.documentElement;
+            return G && x && H.insertBefore(n.createTextNode(x), H.childNodes[0] || null), Ze === It ? z.call(ie, Ue ? "html" : "body")[0] : Ue ? ie.documentElement : H;
         },
         g = function(G) {
             return R.call(
                 G.ownerDocument || G,
                 G,
                 // eslint-disable-next-line no-bitwise
                 p.SHOW_ELEMENT | p.SHOW_COMMENT | p.SHOW_TEXT | p.SHOW_PROCESSING_INSTRUCTION | p.SHOW_CDATA_SECTION,
@@ -7818,21 +7818,21 @@
         },
         Z = function(G) {
             return G instanceof v && (typeof G.nodeName != "string" || typeof G.textContent != "string" || typeof G.removeChild != "function" || !(G.attributes instanceof _) || typeof G.removeAttribute != "function" || typeof G.setAttribute != "function" || typeof G.namespaceURI != "string" || typeof G.insertBefore != "function" || typeof G.hasChildNodes != "function");
         },
         y = function(G) {
             return typeof u == "function" && G instanceof u;
         },
-        B = function(G, le, x) {
+        B = function(G, ie, x) {
             ne[G] && Ws(ne[G], (Ye) => {
-                Ye.call(e, le, x, qn);
+                Ye.call(e, ie, x, qn);
             });
         },
         ze = function(G) {
-            let le = null;
+            let ie = null;
             if (B("beforeSanitizeElements", G, null), Z(G))
                 return Qt(G), !0;
             const x = wt(G.nodeName);
             if (B("uponSanitizeElement", G, {
                     tagName: x,
                     allowedTags: oe
                 }), G.hasChildNodes() && !y(G.firstElementChild) && an(/<[/\w]/g, G.innerHTML) && an(/<[/\w]/g, G.textContent) || G.nodeType === 7 || Xe && G.nodeType === 8 && an(/<[/\w]/g, G.data))
@@ -7847,83 +7847,83 @@
                         const Lt = H.length;
                         for (let Vt = Lt - 1; Vt >= 0; --Vt)
                             Ye.insertBefore(P(H[Vt], !0), U(G));
                     }
                 }
                 return Qt(G), !0;
             }
-            return G instanceof h && !Lr(G) || (x === "noscript" || x === "noembed" || x === "noframes") && an(/<\/no(script|embed|frames)/i, G.innerHTML) ? (Qt(G), !0) : (Ie && G.nodeType === 3 && (le = G.textContent, Ws([re, pe, Me], (Ye) => {
-                le = Xr(le, Ye, " ");
-            }), G.textContent !== le && (Wr(e.removed, {
+            return G instanceof h && !Lr(G) || (x === "noscript" || x === "noembed" || x === "noframes") && an(/<\/no(script|embed|frames)/i, G.innerHTML) ? (Qt(G), !0) : (Ie && G.nodeType === 3 && (ie = G.textContent, Ws([re, pe, Me], (Ye) => {
+                ie = Xr(ie, Ye, " ");
+            }), G.textContent !== ie && (Wr(e.removed, {
                 element: G.cloneNode()
-            }), G.textContent = le)), B("afterSanitizeElements", G, null), !1);
+            }), G.textContent = ie)), B("afterSanitizeElements", G, null), !1);
         },
-        fe = function(G, le, x) {
-            if (Ct && (le === "id" || le === "name") && (x in n || x in Ir))
+        fe = function(G, ie, x) {
+            if (Ct && (ie === "id" || ie === "name") && (x in n || x in Ir))
                 return !1;
-            if (!(xe && !ve[le] && an(Ne, le))) {
-                if (!($ && an(ke, le))) {
-                    if (!de[le] || ve[le]) {
+            if (!(xe && !ve[ie] && an(Ne, ie))) {
+                if (!($ && an(ke, ie))) {
+                    if (!de[ie] || ve[ie]) {
                         if (
                             // First condition does a very basic check if a) it's basically a valid custom element tagname AND
                             // b) if the tagName passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
                             // and c) if the attribute name passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.attributeNameCheck
-                            !(pt(G) && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, G) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(G)) && (ee.attributeNameCheck instanceof RegExp && an(ee.attributeNameCheck, le) || ee.attributeNameCheck instanceof Function && ee.attributeNameCheck(le)) || // Alternative, second condition checks if it's an `is`-attribute, AND
+                            !(pt(G) && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, G) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(G)) && (ee.attributeNameCheck instanceof RegExp && an(ee.attributeNameCheck, ie) || ee.attributeNameCheck instanceof Function && ee.attributeNameCheck(ie)) || // Alternative, second condition checks if it's an `is`-attribute, AND
                                 // the value passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
-                                le === "is" && ee.allowCustomizedBuiltInElements && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, x) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(x)))
+                                ie === "is" && ee.allowCustomizedBuiltInElements && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, x) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(x)))
                         )
                             return !1;
-                    } else if (!tt[le]) {
+                    } else if (!tt[ie]) {
                         if (!an(Be, Xr(x, he, ""))) {
-                            if (!((le === "src" || le === "xlink:href" || le === "href") && G !== "script" && pp(x, "data:") === 0 && Ce[G])) {
+                            if (!((ie === "src" || ie === "xlink:href" || ie === "href") && G !== "script" && pp(x, "data:") === 0 && Ce[G])) {
                                 if (!(Se && !an(ce, Xr(x, he, "")))) {
                                     if (x)
                                         return !1;
                                 }
                             }
                         }
                     }
                 }
             }
             return !0;
         },
         pt = function(G) {
-            return G !== "annotation-xml" && pc(G, ae);
+            return G !== "annotation-xml" && pc(G, le);
         },
-        kn = function(G) {
+        Dn = function(G) {
             B("beforeSanitizeAttributes", G, null);
             const {
-                attributes: le
+                attributes: ie
             } = G;
-            if (!le)
+            if (!ie)
                 return;
             const x = {
                 attrName: "",
                 attrValue: "",
                 keepAttr: !0,
                 allowedAttributes: de
             };
-            let Ye = le.length;
+            let Ye = ie.length;
             for (; Ye--;) {
-                const H = le[Ye],
+                const H = ie[Ye],
                     {
                         name: Lt,
                         namespaceURI: Vt,
                         value: Un
                     } = H,
                     Gn = wt(Lt);
                 let Ae = Lt === "value" ? Un : gp(Un);
                 if (x.attrName = Gn, x.attrValue = Ae, x.keepAttr = !0, x.forceKeepAttr = void 0, B("uponSanitizeAttribute", G, x), Ae = x.attrValue, x.forceKeepAttr || (q(Lt, G), !x.keepAttr))
                     continue;
                 if (!We && an(/\/>/i, Ae)) {
                     q(Lt, G);
                     continue;
                 }
-                Ie && Ws([re, pe, Me], (P0) => {
-                    Ae = Xr(Ae, P0, " ");
+                Ie && Ws([re, pe, Me], (q0) => {
+                    Ae = Xr(Ae, q0, " ");
                 });
                 const or = wt(G.nodeName);
                 if (fe(or, Gn, Ae)) {
                     if (K && (Gn === "id" || Gn === "name") && (q(Lt, G), Ae = ye + Ae), D && typeof T == "object" && typeof T.getAttributeType == "function" && !Vt)
                         switch (T.getAttributeType(or, Gn)) {
                             case "TrustedHTML": {
                                 Ae = D.createHTML(Ae);
@@ -7938,78 +7938,78 @@
                         Vt ? G.setAttributeNS(Vt, Lt, Ae) : G.setAttribute(Lt, Ae), mc(e.removed);
                     } catch {}
                 }
             }
             B("afterSanitizeAttributes", G, null);
         },
         De = function ue(G) {
-            let le = null;
+            let ie = null;
             const x = g(G);
-            for (B("beforeSanitizeShadowDOM", G, null); le = x.nextNode();)
-                B("uponSanitizeShadowNode", le, null), !ze(le) && (le.content instanceof o && ue(le.content), kn(le));
+            for (B("beforeSanitizeShadowDOM", G, null); ie = x.nextNode();)
+                B("uponSanitizeShadowNode", ie, null), !ze(ie) && (ie.content instanceof o && ue(ie.content), Dn(ie));
             B("afterSanitizeShadowDOM", G, null);
         };
     return e.sanitize = function(ue) {
         let G = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
-            le = null,
+            ie = null,
             x = null,
             Ye = null,
             H = null;
-        if (ie = !ue, ie && (ue = "<!-->"), typeof ue != "string" && !y(ue))
+        if (ae = !ue, ae && (ue = "<!-->"), typeof ue != "string" && !y(ue))
             if (typeof ue.toString == "function") {
                 if (ue = ue.toString(), typeof ue != "string")
                     throw Yr("dirty is not a string, aborting");
             } else
                 throw Yr("toString is not a function");
         if (!e.isSupported)
             return ue;
         if (zt || en(G), e.removed = [], typeof ue == "string" && (Ee = !1), Ee) {
             if (ue.nodeName) {
                 const Un = wt(ue.nodeName);
                 if (!oe[Un] || we[Un])
                     throw Yr("root node is forbidden and cannot be sanitized in-place");
             }
         } else if (ue instanceof u)
-            le = d("<!---->"), x = le.ownerDocument.importNode(ue, !0), x.nodeType === 1 && x.nodeName === "BODY" || x.nodeName === "HTML" ? le = x : le.appendChild(x);
+            ie = d("<!---->"), x = ie.ownerDocument.importNode(ue, !0), x.nodeType === 1 && x.nodeName === "BODY" || x.nodeName === "HTML" ? ie = x : ie.appendChild(x);
         else {
             if (!Re && !Ie && !Ue && // eslint-disable-next-line unicorn/prefer-includes
                 ue.indexOf("<") === -1)
                 return D && Ot ? D.createHTML(ue) : ue;
-            if (le = d(ue), !le)
+            if (ie = d(ue), !ie)
                 return Re ? null : Ot ? E : "";
         }
-        le && Bn && Qt(le.firstChild);
-        const Lt = g(Ee ? ue : le);
+        ie && Nn && Qt(ie.firstChild);
+        const Lt = g(Ee ? ue : ie);
         for (; Ye = Lt.nextNode();)
-            ze(Ye) || (Ye.content instanceof o && De(Ye.content), kn(Ye));
+            ze(Ye) || (Ye.content instanceof o && De(Ye.content), Dn(Ye));
         if (Ee)
             return ue;
         if (Re) {
             if ($t)
-                for (H = I.call(le.ownerDocument); le.firstChild;)
-                    H.appendChild(le.firstChild);
+                for (H = I.call(ie.ownerDocument); ie.firstChild;)
+                    H.appendChild(ie.firstChild);
             else
-                H = le;
+                H = ie;
             return (de.shadowroot || de.shadowrootmode) && (H = Y.call(r, H, !0)), H;
         }
-        let Vt = Ue ? le.outerHTML : le.innerHTML;
-        return Ue && oe["!doctype"] && le.ownerDocument && le.ownerDocument.doctype && le.ownerDocument.doctype.name && an(_h, le.ownerDocument.doctype.name) && (Vt = "<!DOCTYPE " + le.ownerDocument.doctype.name + `>
+        let Vt = Ue ? ie.outerHTML : ie.innerHTML;
+        return Ue && oe["!doctype"] && ie.ownerDocument && ie.ownerDocument.doctype && ie.ownerDocument.doctype.name && an(_h, ie.ownerDocument.doctype.name) && (Vt = "<!DOCTYPE " + ie.ownerDocument.doctype.name + `>
 ` + Vt), Ie && Ws([re, pe, Me], (Un) => {
             Vt = Xr(Vt, Un, " ");
         }), D && Ot ? D.createHTML(Vt) : Vt;
     }, e.setConfig = function() {
         let ue = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
         en(ue), zt = !0;
     }, e.clearConfig = function() {
         qn = null, zt = !1;
-    }, e.isValidAttribute = function(ue, G, le) {
+    }, e.isValidAttribute = function(ue, G, ie) {
         qn || en({});
         const x = wt(ue),
             Ye = wt(G);
-        return fe(x, Ye, le);
+        return fe(x, Ye, ie);
     }, e.addHook = function(ue, G) {
         typeof G == "function" && (ne[ue] = ne[ue] || [], Wr(ne[ue], G));
     }, e.removeHook = function(ue) {
         if (ne[ue])
             return mc(ne[ue]);
     }, e.removeHooks = function(ue) {
         ne[ue] && (ne[ue] = []);
@@ -8315,15 +8315,15 @@
                             return Ne[he[this.id]];
                         }
                         /**
                          * Get the style of a fraction denominator given the fraction in the current
                          * style.
                          */
                         fracDen() {
-                            return Ne[ae[this.id]];
+                            return Ne[le[this.id]];
                         }
                         /**
                          * Get the cramped version of a style (in particular, cramping a cramped style
                          * doesn't change the style).
                          */
                         cramp() {
                             return Ne[Be[this.id]];
@@ -8349,15 +8349,15 @@
                         re = 5,
                         pe = 6,
                         Me = 7,
                         Ne = [new C(R, 0, !1), new C(I, 0, !0), new C(z, 1, !1), new C(Y, 1, !0), new C(ne, 2, !1), new C(re, 2, !0), new C(pe, 3, !1), new C(Me, 3, !0)],
                         ke = [ne, re, ne, re, pe, Me, pe, Me],
                         ce = [re, re, re, re, Me, Me, Me, Me],
                         he = [z, Y, ne, re, pe, Me, pe, Me],
-                        ae = [Y, Y, re, re, Me, Me, Me, Me],
+                        le = [Y, Y, re, re, Me, Me, Me, Me],
                         Be = [I, I, Y, Y, re, re, Me, Me],
                         oe = [R, I, z, Y, z, Y, z, Y];
                     var Q = {
                         DISPLAY: Ne[R],
                         TEXT: Ne[z],
                         SCRIPT: Ne[ne],
                         SCRIPTSCRIPT: Ne[pe]
@@ -8547,15 +8547,15 @@
                                     f = Ie(s, ve);
                                     break;
                                 case "sqrtTall":
                                     f = Ue(s, ve, a);
                             }
                             return f;
                         },
-                        Bn = function(i, s) {
+                        Nn = function(i, s) {
                             switch (i) {
                                 case "⎜":
                                     return "M291 0 H417 V" + s + " H291z M291 0 H417 V" + s + " H291z";
                                 case "∣":
                                     return "M145 0 H188 V" + s + " H145z M145 0 H188 V" + s + " H145z";
                                 case "∥":
                                     return "M145 0 H188 V" + s + " H145z M145 0 H188 V" + s + " H145z" + ("M367 0 H410 V" + s + " H367z M367 0 H410 V" + s + " H367z");
@@ -11424,21 +11424,21 @@
                             // new cicero (12 new didot)
                             sp: 1 / 65536,
                             // scaled point (TeX's internal smallest unit)
                             // https://tex.stackexchange.com/a/41371
                             px: 803 / 800
                             // \pdfpxdimen defaults to 1 bp in pdfTeX and LuaTeX
                         },
-                        Nn = {
+                        kn = {
                             ex: !0,
                             em: !0,
                             mu: !0
                         },
                         It = function(i) {
-                            return typeof i != "string" && (i = i.unit), i in Jt || i in Nn || i === "ex";
+                            return typeof i != "string" && (i = i.unit), i in Jt || i in kn || i === "ex";
                         },
                         Ze = function(i, s) {
                             let a;
                             if (i.unit in Jt)
                                 a = Jt[i.unit] / s.fontMetrics().ptPerEm / s.sizeMultiplier;
                             else if (i.unit === "mu")
                                 a = s.fontMetrics().cssEmPerMu;
@@ -11450,55 +11450,55 @@
                                     a = f.fontMetrics().quad;
                                 else
                                     throw new o("Invalid unit: '" + i.unit + "'");
                                 f !== s && (a *= f.sizeMultiplier / s.sizeMultiplier);
                             }
                             return Math.min(i.number * a, s.maxSize);
                         },
-                        ie = function(i) {
+                        ae = function(i) {
                             return +i.toFixed(4) + "em";
                         },
-                        Gt = function(i) {
+                        Ut = function(i) {
                             return i.filter((s) => s).join(" ");
                         },
-                        rr = function(i, s, a) {
+                        s0 = function(i, s, a) {
                             if (this.classes = i || [], this.attributes = {}, this.height = 0, this.depth = 0, this.maxFontSize = 0, this.style = a || {}, s) {
                                 s.style.isTight() && this.classes.push("mtight");
                                 const f = s.getColor();
                                 f && (this.style.color = f);
                             }
                         },
                         Pn = function(i) {
                             const s = document.createElement(i);
-                            s.className = Gt(this.classes);
+                            s.className = Ut(this.classes);
                             for (const a in this.style)
                                 this.style.hasOwnProperty(a) && (s.style[a] = this.style[a]);
                             for (const a in this.attributes)
                                 this.attributes.hasOwnProperty(a) && s.setAttribute(a, this.attributes[a]);
                             for (let a = 0; a < this.children.length; a++)
                                 s.appendChild(this.children[a].toNode());
                             return s;
                         },
                         sr = function(i) {
                             let s = "<" + i;
-                            this.classes.length && (s += ' class="' + M.escape(Gt(this.classes)) + '"');
+                            this.classes.length && (s += ' class="' + M.escape(Ut(this.classes)) + '"');
                             let a = "";
                             for (const f in this.style)
                                 this.style.hasOwnProperty(f) && (a += M.hyphenate(f) + ":" + this.style[f] + ";");
                             a && (s += ' style="' + M.escape(a) + '"');
                             for (const f in this.attributes)
                                 this.attributes.hasOwnProperty(f) && (s += " " + f + '="' + M.escape(this.attributes[f]) + '"');
                             s += ">";
                             for (let f = 0; f < this.children.length; f++)
                                 s += this.children[f].toMarkup();
                             return s += "</" + i + ">", s;
                         };
-                    class s0 {
+                    class i0 {
                         constructor(s, a, f, m) {
-                            this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, rr.call(this, s, f, m), this.children = a || [];
+                            this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, s0.call(this, s, f, m), this.children = a || [];
                         }
                         /**
                          * Sets an arbitrary attribute on the span. Warning: use this wisely. Not
                          * all browsers support attributes the same, and having too many custom
                          * attributes is probably bad.
                          */
                         setAttribute(s, a) {
@@ -11512,15 +11512,15 @@
                         }
                         toMarkup() {
                             return sr.call(this, "span");
                         }
                     }
                     class wt {
                         constructor(s, a, f, m) {
-                            this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, rr.call(this, a, m), this.children = f || [], this.setAttribute("href", s);
+                            this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, s0.call(this, a, m), this.children = f || [], this.setAttribute("href", s);
                         }
                         setAttribute(s, a) {
                             this.attributes[s] = a;
                         }
                         hasClass(s) {
                             return M.contains(this.classes, s);
                         }
@@ -11572,26 +11572,26 @@
                         /**
                          * Creates a text node or span from a symbol node. Note that a span is only
                          * created if it is needed.
                          */
                         toNode() {
                             const s = document.createTextNode(this.text);
                             let a = null;
-                            this.italic > 0 && (a = document.createElement("span"), a.style.marginRight = ie(this.italic)), this.classes.length > 0 && (a = a || document.createElement("span"), a.className = Gt(this.classes));
+                            this.italic > 0 && (a = document.createElement("span"), a.style.marginRight = ae(this.italic)), this.classes.length > 0 && (a = a || document.createElement("span"), a.className = Ut(this.classes));
                             for (const f in this.style)
                                 this.style.hasOwnProperty(f) && (a = a || document.createElement("span"), a.style[f] = this.style[f]);
                             return a ? (a.appendChild(s), a) : s;
                         }
                         /**
                          * Creates markup for a symbol node.
                          */
                         toMarkup() {
                             let s = !1,
                                 a = "<span";
-                            this.classes.length && (s = !0, a += ' class="', a += M.escape(Gt(this.classes)), a += '"');
+                            this.classes.length && (s = !0, a += ' class="', a += M.escape(Ut(this.classes)), a += '"');
                             let f = "";
                             this.italic > 0 && (f += "margin-right:" + this.italic + "em;");
                             for (const b in this.style)
                                 this.style.hasOwnProperty(b) && (f += M.hyphenate(b) + ":" + this.style[b] + ";");
                             f && (s = !0, a += ' style="' + M.escape(f) + '"');
                             const m = M.escape(this.text);
                             return s ? (a += ">", a += m, a += "</span>", a) : m;
@@ -11627,15 +11627,15 @@
                             const a = document.createElementNS("http://www.w3.org/2000/svg", "path");
                             return this.alternate ? a.setAttribute("d", this.alternate) : a.setAttribute("d", Re[this.pathName]), a;
                         }
                         toMarkup() {
                             return this.alternate ? '<path d="' + M.escape(this.alternate) + '"/>' : '<path d="' + M.escape(Re[this.pathName]) + '"/>';
                         }
                     }
-                    class p0 {
+                    class g0 {
                         constructor(s) {
                             this.attributes = void 0, this.attributes = s || {};
                         }
                         toNode() {
                             const a = document.createElementNS("http://www.w3.org/2000/svg", "line");
                             for (const f in this.attributes)
                                 Object.prototype.hasOwnProperty.call(this.attributes, f) && a.setAttribute(f, this.attributes[f]);
@@ -11652,15 +11652,15 @@
                     function ir(i) {
                         if (i instanceof jt)
                             return i;
                         throw new Error("Expected symbolNode but got " + String(i) + ".");
                     }
 
                     function lr(i) {
-                        if (i instanceof s0)
+                        if (i instanceof i0)
                             return i;
                         throw new Error("Expected span<HtmlDomNode> but got " + String(i) + ".");
                     }
                     const ar = {
                             bin: 1,
                             close: 1,
                             inner: 1,
@@ -11691,23 +11691,23 @@
                     const g = "math",
                         Z = "text",
                         y = "main",
                         B = "ams",
                         ze = "accent-token",
                         fe = "bin",
                         pt = "close",
-                        kn = "inner",
+                        Dn = "inner",
                         De = "mathord",
                         ue = "op-token",
                         G = "open",
-                        le = "punct",
+                        ie = "punct",
                         x = "rel",
                         Ye = "spacing",
                         H = "textord";
-                    d(g, y, x, "≡", "\\equiv", !0), d(g, y, x, "≺", "\\prec", !0), d(g, y, x, "≻", "\\succ", !0), d(g, y, x, "∼", "\\sim", !0), d(g, y, x, "⊥", "\\perp"), d(g, y, x, "⪯", "\\preceq", !0), d(g, y, x, "⪰", "\\succeq", !0), d(g, y, x, "≃", "\\simeq", !0), d(g, y, x, "∣", "\\mid", !0), d(g, y, x, "≪", "\\ll", !0), d(g, y, x, "≫", "\\gg", !0), d(g, y, x, "≍", "\\asymp", !0), d(g, y, x, "∥", "\\parallel"), d(g, y, x, "⋈", "\\bowtie", !0), d(g, y, x, "⌣", "\\smile", !0), d(g, y, x, "⊑", "\\sqsubseteq", !0), d(g, y, x, "⊒", "\\sqsupseteq", !0), d(g, y, x, "≐", "\\doteq", !0), d(g, y, x, "⌢", "\\frown", !0), d(g, y, x, "∋", "\\ni", !0), d(g, y, x, "∝", "\\propto", !0), d(g, y, x, "⊢", "\\vdash", !0), d(g, y, x, "⊣", "\\dashv", !0), d(g, y, x, "∋", "\\owns"), d(g, y, le, ".", "\\ldotp"), d(g, y, le, "⋅", "\\cdotp"), d(g, y, H, "#", "\\#"), d(Z, y, H, "#", "\\#"), d(g, y, H, "&", "\\&"), d(Z, y, H, "&", "\\&"), d(g, y, H, "ℵ", "\\aleph", !0), d(g, y, H, "∀", "\\forall", !0), d(g, y, H, "ℏ", "\\hbar", !0), d(g, y, H, "∃", "\\exists", !0), d(g, y, H, "∇", "\\nabla", !0), d(g, y, H, "♭", "\\flat", !0), d(g, y, H, "ℓ", "\\ell", !0), d(g, y, H, "♮", "\\natural", !0), d(g, y, H, "♣", "\\clubsuit", !0), d(g, y, H, "℘", "\\wp", !0), d(g, y, H, "♯", "\\sharp", !0), d(g, y, H, "♢", "\\diamondsuit", !0), d(g, y, H, "ℜ", "\\Re", !0), d(g, y, H, "♡", "\\heartsuit", !0), d(g, y, H, "ℑ", "\\Im", !0), d(g, y, H, "♠", "\\spadesuit", !0), d(g, y, H, "§", "\\S", !0), d(Z, y, H, "§", "\\S"), d(g, y, H, "¶", "\\P", !0), d(Z, y, H, "¶", "\\P"), d(g, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\textdagger"), d(g, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\textdaggerdbl"), d(g, y, pt, "⎱", "\\rmoustache", !0), d(g, y, G, "⎰", "\\lmoustache", !0), d(g, y, pt, "⟯", "\\rgroup", !0), d(g, y, G, "⟮", "\\lgroup", !0), d(g, y, fe, "∓", "\\mp", !0), d(g, y, fe, "⊖", "\\ominus", !0), d(g, y, fe, "⊎", "\\uplus", !0), d(g, y, fe, "⊓", "\\sqcap", !0), d(g, y, fe, "∗", "\\ast"), d(g, y, fe, "⊔", "\\sqcup", !0), d(g, y, fe, "◯", "\\bigcirc", !0), d(g, y, fe, "∙", "\\bullet", !0), d(g, y, fe, "‡", "\\ddagger"), d(g, y, fe, "≀", "\\wr", !0), d(g, y, fe, "⨿", "\\amalg"), d(g, y, fe, "&", "\\And"), d(g, y, x, "⟵", "\\longleftarrow", !0), d(g, y, x, "⇐", "\\Leftarrow", !0), d(g, y, x, "⟸", "\\Longleftarrow", !0), d(g, y, x, "⟶", "\\longrightarrow", !0), d(g, y, x, "⇒", "\\Rightarrow", !0), d(g, y, x, "⟹", "\\Longrightarrow", !0), d(g, y, x, "↔", "\\leftrightarrow", !0), d(g, y, x, "⟷", "\\longleftrightarrow", !0), d(g, y, x, "⇔", "\\Leftrightarrow", !0), d(g, y, x, "⟺", "\\Longleftrightarrow", !0), d(g, y, x, "↦", "\\mapsto", !0), d(g, y, x, "⟼", "\\longmapsto", !0), d(g, y, x, "↗", "\\nearrow", !0), d(g, y, x, "↩", "\\hookleftarrow", !0), d(g, y, x, "↪", "\\hookrightarrow", !0), d(g, y, x, "↘", "\\searrow", !0), d(g, y, x, "↼", "\\leftharpoonup", !0), d(g, y, x, "⇀", "\\rightharpoonup", !0), d(g, y, x, "↙", "\\swarrow", !0), d(g, y, x, "↽", "\\leftharpoondown", !0), d(g, y, x, "⇁", "\\rightharpoondown", !0), d(g, y, x, "↖", "\\nwarrow", !0), d(g, y, x, "⇌", "\\rightleftharpoons", !0), d(g, B, x, "≮", "\\nless", !0), d(g, B, x, "", "\\@nleqslant"), d(g, B, x, "", "\\@nleqq"), d(g, B, x, "⪇", "\\lneq", !0), d(g, B, x, "≨", "\\lneqq", !0), d(g, B, x, "", "\\@lvertneqq"), d(g, B, x, "⋦", "\\lnsim", !0), d(g, B, x, "⪉", "\\lnapprox", !0), d(g, B, x, "⊀", "\\nprec", !0), d(g, B, x, "⋠", "\\npreceq", !0), d(g, B, x, "⋨", "\\precnsim", !0), d(g, B, x, "⪹", "\\precnapprox", !0), d(g, B, x, "≁", "\\nsim", !0), d(g, B, x, "", "\\@nshortmid"), d(g, B, x, "∤", "\\nmid", !0), d(g, B, x, "⊬", "\\nvdash", !0), d(g, B, x, "⊭", "\\nvDash", !0), d(g, B, x, "⋪", "\\ntriangleleft"), d(g, B, x, "⋬", "\\ntrianglelefteq", !0), d(g, B, x, "⊊", "\\subsetneq", !0), d(g, B, x, "", "\\@varsubsetneq"), d(g, B, x, "⫋", "\\subsetneqq", !0), d(g, B, x, "", "\\@varsubsetneqq"), d(g, B, x, "≯", "\\ngtr", !0), d(g, B, x, "", "\\@ngeqslant"), d(g, B, x, "", "\\@ngeqq"), d(g, B, x, "⪈", "\\gneq", !0), d(g, B, x, "≩", "\\gneqq", !0), d(g, B, x, "", "\\@gvertneqq"), d(g, B, x, "⋧", "\\gnsim", !0), d(g, B, x, "⪊", "\\gnapprox", !0), d(g, B, x, "⊁", "\\nsucc", !0), d(g, B, x, "⋡", "\\nsucceq", !0), d(g, B, x, "⋩", "\\succnsim", !0), d(g, B, x, "⪺", "\\succnapprox", !0), d(g, B, x, "≆", "\\ncong", !0), d(g, B, x, "", "\\@nshortparallel"), d(g, B, x, "∦", "\\nparallel", !0), d(g, B, x, "⊯", "\\nVDash", !0), d(g, B, x, "⋫", "\\ntriangleright"), d(g, B, x, "⋭", "\\ntrianglerighteq", !0), d(g, B, x, "", "\\@nsupseteqq"), d(g, B, x, "⊋", "\\supsetneq", !0), d(g, B, x, "", "\\@varsupsetneq"), d(g, B, x, "⫌", "\\supsetneqq", !0), d(g, B, x, "", "\\@varsupsetneqq"), d(g, B, x, "⊮", "\\nVdash", !0), d(g, B, x, "⪵", "\\precneqq", !0), d(g, B, x, "⪶", "\\succneqq", !0), d(g, B, x, "", "\\@nsubseteqq"), d(g, B, fe, "⊴", "\\unlhd"), d(g, B, fe, "⊵", "\\unrhd"), d(g, B, x, "↚", "\\nleftarrow", !0), d(g, B, x, "↛", "\\nrightarrow", !0), d(g, B, x, "⇍", "\\nLeftarrow", !0), d(g, B, x, "⇏", "\\nRightarrow", !0), d(g, B, x, "↮", "\\nleftrightarrow", !0), d(g, B, x, "⇎", "\\nLeftrightarrow", !0), d(g, B, x, "△", "\\vartriangle"), d(g, B, H, "ℏ", "\\hslash"), d(g, B, H, "▽", "\\triangledown"), d(g, B, H, "◊", "\\lozenge"), d(g, B, H, "Ⓢ", "\\circledS"), d(g, B, H, "®", "\\circledR"), d(Z, B, H, "®", "\\circledR"), d(g, B, H, "∡", "\\measuredangle", !0), d(g, B, H, "∄", "\\nexists"), d(g, B, H, "℧", "\\mho"), d(g, B, H, "Ⅎ", "\\Finv", !0), d(g, B, H, "⅁", "\\Game", !0), d(g, B, H, "‵", "\\backprime"), d(g, B, H, "▲", "\\blacktriangle"), d(g, B, H, "▼", "\\blacktriangledown"), d(g, B, H, "■", "\\blacksquare"), d(g, B, H, "⧫", "\\blacklozenge"), d(g, B, H, "★", "\\bigstar"), d(g, B, H, "∢", "\\sphericalangle", !0), d(g, B, H, "∁", "\\complement", !0), d(g, B, H, "ð", "\\eth", !0), d(Z, y, H, "ð", "ð"), d(g, B, H, "╱", "\\diagup"), d(g, B, H, "╲", "\\diagdown"), d(g, B, H, "□", "\\square"), d(g, B, H, "□", "\\Box"), d(g, B, H, "◊", "\\Diamond"), d(g, B, H, "¥", "\\yen", !0), d(Z, B, H, "¥", "\\yen", !0), d(g, B, H, "✓", "\\checkmark", !0), d(Z, B, H, "✓", "\\checkmark"), d(g, B, H, "ℶ", "\\beth", !0), d(g, B, H, "ℸ", "\\daleth", !0), d(g, B, H, "ℷ", "\\gimel", !0), d(g, B, H, "ϝ", "\\digamma", !0), d(g, B, H, "ϰ", "\\varkappa"), d(g, B, G, "┌", "\\@ulcorner", !0), d(g, B, pt, "┐", "\\@urcorner", !0), d(g, B, G, "└", "\\@llcorner", !0), d(g, B, pt, "┘", "\\@lrcorner", !0), d(g, B, x, "≦", "\\leqq", !0), d(g, B, x, "⩽", "\\leqslant", !0), d(g, B, x, "⪕", "\\eqslantless", !0), d(g, B, x, "≲", "\\lesssim", !0), d(g, B, x, "⪅", "\\lessapprox", !0), d(g, B, x, "≊", "\\approxeq", !0), d(g, B, fe, "⋖", "\\lessdot"), d(g, B, x, "⋘", "\\lll", !0), d(g, B, x, "≶", "\\lessgtr", !0), d(g, B, x, "⋚", "\\lesseqgtr", !0), d(g, B, x, "⪋", "\\lesseqqgtr", !0), d(g, B, x, "≑", "\\doteqdot"), d(g, B, x, "≓", "\\risingdotseq", !0), d(g, B, x, "≒", "\\fallingdotseq", !0), d(g, B, x, "∽", "\\backsim", !0), d(g, B, x, "⋍", "\\backsimeq", !0), d(g, B, x, "⫅", "\\subseteqq", !0), d(g, B, x, "⋐", "\\Subset", !0), d(g, B, x, "⊏", "\\sqsubset", !0), d(g, B, x, "≼", "\\preccurlyeq", !0), d(g, B, x, "⋞", "\\curlyeqprec", !0), d(g, B, x, "≾", "\\precsim", !0), d(g, B, x, "⪷", "\\precapprox", !0), d(g, B, x, "⊲", "\\vartriangleleft"), d(g, B, x, "⊴", "\\trianglelefteq"), d(g, B, x, "⊨", "\\vDash", !0), d(g, B, x, "⊪", "\\Vvdash", !0), d(g, B, x, "⌣", "\\smallsmile"), d(g, B, x, "⌢", "\\smallfrown"), d(g, B, x, "≏", "\\bumpeq", !0), d(g, B, x, "≎", "\\Bumpeq", !0), d(g, B, x, "≧", "\\geqq", !0), d(g, B, x, "⩾", "\\geqslant", !0), d(g, B, x, "⪖", "\\eqslantgtr", !0), d(g, B, x, "≳", "\\gtrsim", !0), d(g, B, x, "⪆", "\\gtrapprox", !0), d(g, B, fe, "⋗", "\\gtrdot"), d(g, B, x, "⋙", "\\ggg", !0), d(g, B, x, "≷", "\\gtrless", !0), d(g, B, x, "⋛", "\\gtreqless", !0), d(g, B, x, "⪌", "\\gtreqqless", !0), d(g, B, x, "≖", "\\eqcirc", !0), d(g, B, x, "≗", "\\circeq", !0), d(g, B, x, "≜", "\\triangleq", !0), d(g, B, x, "∼", "\\thicksim"), d(g, B, x, "≈", "\\thickapprox"), d(g, B, x, "⫆", "\\supseteqq", !0), d(g, B, x, "⋑", "\\Supset", !0), d(g, B, x, "⊐", "\\sqsupset", !0), d(g, B, x, "≽", "\\succcurlyeq", !0), d(g, B, x, "⋟", "\\curlyeqsucc", !0), d(g, B, x, "≿", "\\succsim", !0), d(g, B, x, "⪸", "\\succapprox", !0), d(g, B, x, "⊳", "\\vartriangleright"), d(g, B, x, "⊵", "\\trianglerighteq"), d(g, B, x, "⊩", "\\Vdash", !0), d(g, B, x, "∣", "\\shortmid"), d(g, B, x, "∥", "\\shortparallel"), d(g, B, x, "≬", "\\between", !0), d(g, B, x, "⋔", "\\pitchfork", !0), d(g, B, x, "∝", "\\varpropto"), d(g, B, x, "◀", "\\blacktriangleleft"), d(g, B, x, "∴", "\\therefore", !0), d(g, B, x, "∍", "\\backepsilon"), d(g, B, x, "▶", "\\blacktriangleright"), d(g, B, x, "∵", "\\because", !0), d(g, B, x, "⋘", "\\llless"), d(g, B, x, "⋙", "\\gggtr"), d(g, B, fe, "⊲", "\\lhd"), d(g, B, fe, "⊳", "\\rhd"), d(g, B, x, "≂", "\\eqsim", !0), d(g, y, x, "⋈", "\\Join"), d(g, B, x, "≑", "\\Doteq", !0), d(g, B, fe, "∔", "\\dotplus", !0), d(g, B, fe, "∖", "\\smallsetminus"), d(g, B, fe, "⋒", "\\Cap", !0), d(g, B, fe, "⋓", "\\Cup", !0), d(g, B, fe, "⩞", "\\doublebarwedge", !0), d(g, B, fe, "⊟", "\\boxminus", !0), d(g, B, fe, "⊞", "\\boxplus", !0), d(g, B, fe, "⋇", "\\divideontimes", !0), d(g, B, fe, "⋉", "\\ltimes", !0), d(g, B, fe, "⋊", "\\rtimes", !0), d(g, B, fe, "⋋", "\\leftthreetimes", !0), d(g, B, fe, "⋌", "\\rightthreetimes", !0), d(g, B, fe, "⋏", "\\curlywedge", !0), d(g, B, fe, "⋎", "\\curlyvee", !0), d(g, B, fe, "⊝", "\\circleddash", !0), d(g, B, fe, "⊛", "\\circledast", !0), d(g, B, fe, "⋅", "\\centerdot"), d(g, B, fe, "⊺", "\\intercal", !0), d(g, B, fe, "⋒", "\\doublecap"), d(g, B, fe, "⋓", "\\doublecup"), d(g, B, fe, "⊠", "\\boxtimes", !0), d(g, B, x, "⇢", "\\dashrightarrow", !0), d(g, B, x, "⇠", "\\dashleftarrow", !0), d(g, B, x, "⇇", "\\leftleftarrows", !0), d(g, B, x, "⇆", "\\leftrightarrows", !0), d(g, B, x, "⇚", "\\Lleftarrow", !0), d(g, B, x, "↞", "\\twoheadleftarrow", !0), d(g, B, x, "↢", "\\leftarrowtail", !0), d(g, B, x, "↫", "\\looparrowleft", !0), d(g, B, x, "⇋", "\\leftrightharpoons", !0), d(g, B, x, "↶", "\\curvearrowleft", !0), d(g, B, x, "↺", "\\circlearrowleft", !0), d(g, B, x, "↰", "\\Lsh", !0), d(g, B, x, "⇈", "\\upuparrows", !0), d(g, B, x, "↿", "\\upharpoonleft", !0), d(g, B, x, "⇃", "\\downharpoonleft", !0), d(g, y, x, "⊶", "\\origof", !0), d(g, y, x, "⊷", "\\imageof", !0), d(g, B, x, "⊸", "\\multimap", !0), d(g, B, x, "↭", "\\leftrightsquigarrow", !0), d(g, B, x, "⇉", "\\rightrightarrows", !0), d(g, B, x, "⇄", "\\rightleftarrows", !0), d(g, B, x, "↠", "\\twoheadrightarrow", !0), d(g, B, x, "↣", "\\rightarrowtail", !0), d(g, B, x, "↬", "\\looparrowright", !0), d(g, B, x, "↷", "\\curvearrowright", !0), d(g, B, x, "↻", "\\circlearrowright", !0), d(g, B, x, "↱", "\\Rsh", !0), d(g, B, x, "⇊", "\\downdownarrows", !0), d(g, B, x, "↾", "\\upharpoonright", !0), d(g, B, x, "⇂", "\\downharpoonright", !0), d(g, B, x, "⇝", "\\rightsquigarrow", !0), d(g, B, x, "⇝", "\\leadsto"), d(g, B, x, "⇛", "\\Rrightarrow", !0), d(g, B, x, "↾", "\\restriction"), d(g, y, H, "‘", "`"), d(g, y, H, "$", "\\$"), d(Z, y, H, "$", "\\$"), d(Z, y, H, "$", "\\textdollar"), d(g, y, H, "%", "\\%"), d(Z, y, H, "%", "\\%"), d(g, y, H, "_", "\\_"), d(Z, y, H, "_", "\\_"), d(Z, y, H, "_", "\\textunderscore"), d(g, y, H, "∠", "\\angle", !0), d(g, y, H, "∞", "\\infty", !0), d(g, y, H, "′", "\\prime"), d(g, y, H, "△", "\\triangle"), d(g, y, H, "Γ", "\\Gamma", !0), d(g, y, H, "Δ", "\\Delta", !0), d(g, y, H, "Θ", "\\Theta", !0), d(g, y, H, "Λ", "\\Lambda", !0), d(g, y, H, "Ξ", "\\Xi", !0), d(g, y, H, "Π", "\\Pi", !0), d(g, y, H, "Σ", "\\Sigma", !0), d(g, y, H, "Υ", "\\Upsilon", !0), d(g, y, H, "Φ", "\\Phi", !0), d(g, y, H, "Ψ", "\\Psi", !0), d(g, y, H, "Ω", "\\Omega", !0), d(g, y, H, "A", "Α"), d(g, y, H, "B", "Β"), d(g, y, H, "E", "Ε"), d(g, y, H, "Z", "Ζ"), d(g, y, H, "H", "Η"), d(g, y, H, "I", "Ι"), d(g, y, H, "K", "Κ"), d(g, y, H, "M", "Μ"), d(g, y, H, "N", "Ν"), d(g, y, H, "O", "Ο"), d(g, y, H, "P", "Ρ"), d(g, y, H, "T", "Τ"), d(g, y, H, "X", "Χ"), d(g, y, H, "¬", "\\neg", !0), d(g, y, H, "¬", "\\lnot"), d(g, y, H, "⊤", "\\top"), d(g, y, H, "⊥", "\\bot"), d(g, y, H, "∅", "\\emptyset"), d(g, B, H, "∅", "\\varnothing"), d(g, y, De, "α", "\\alpha", !0), d(g, y, De, "β", "\\beta", !0), d(g, y, De, "γ", "\\gamma", !0), d(g, y, De, "δ", "\\delta", !0), d(g, y, De, "ϵ", "\\epsilon", !0), d(g, y, De, "ζ", "\\zeta", !0), d(g, y, De, "η", "\\eta", !0), d(g, y, De, "θ", "\\theta", !0), d(g, y, De, "ι", "\\iota", !0), d(g, y, De, "κ", "\\kappa", !0), d(g, y, De, "λ", "\\lambda", !0), d(g, y, De, "μ", "\\mu", !0), d(g, y, De, "ν", "\\nu", !0), d(g, y, De, "ξ", "\\xi", !0), d(g, y, De, "ο", "\\omicron", !0), d(g, y, De, "π", "\\pi", !0), d(g, y, De, "ρ", "\\rho", !0), d(g, y, De, "σ", "\\sigma", !0), d(g, y, De, "τ", "\\tau", !0), d(g, y, De, "υ", "\\upsilon", !0), d(g, y, De, "ϕ", "\\phi", !0), d(g, y, De, "χ", "\\chi", !0), d(g, y, De, "ψ", "\\psi", !0), d(g, y, De, "ω", "\\omega", !0), d(g, y, De, "ε", "\\varepsilon", !0), d(g, y, De, "ϑ", "\\vartheta", !0), d(g, y, De, "ϖ", "\\varpi", !0), d(g, y, De, "ϱ", "\\varrho", !0), d(g, y, De, "ς", "\\varsigma", !0), d(g, y, De, "φ", "\\varphi", !0), d(g, y, fe, "∗", "*", !0), d(g, y, fe, "+", "+"), d(g, y, fe, "−", "-", !0), d(g, y, fe, "⋅", "\\cdot", !0), d(g, y, fe, "∘", "\\circ", !0), d(g, y, fe, "÷", "\\div", !0), d(g, y, fe, "±", "\\pm", !0), d(g, y, fe, "×", "\\times", !0), d(g, y, fe, "∩", "\\cap", !0), d(g, y, fe, "∪", "\\cup", !0), d(g, y, fe, "∖", "\\setminus", !0), d(g, y, fe, "∧", "\\land"), d(g, y, fe, "∨", "\\lor"), d(g, y, fe, "∧", "\\wedge", !0), d(g, y, fe, "∨", "\\vee", !0), d(g, y, H, "√", "\\surd"), d(g, y, G, "⟨", "\\langle", !0), d(g, y, G, "∣", "\\lvert"), d(g, y, G, "∥", "\\lVert"), d(g, y, pt, "?", "?"), d(g, y, pt, "!", "!"), d(g, y, pt, "⟩", "\\rangle", !0), d(g, y, pt, "∣", "\\rvert"), d(g, y, pt, "∥", "\\rVert"), d(g, y, x, "=", "="), d(g, y, x, ":", ":"), d(g, y, x, "≈", "\\approx", !0), d(g, y, x, "≅", "\\cong", !0), d(g, y, x, "≥", "\\ge"), d(g, y, x, "≥", "\\geq", !0), d(g, y, x, "←", "\\gets"), d(g, y, x, ">", "\\gt", !0), d(g, y, x, "∈", "\\in", !0), d(g, y, x, "", "\\@not"), d(g, y, x, "⊂", "\\subset", !0), d(g, y, x, "⊃", "\\supset", !0), d(g, y, x, "⊆", "\\subseteq", !0), d(g, y, x, "⊇", "\\supseteq", !0), d(g, B, x, "⊈", "\\nsubseteq", !0), d(g, B, x, "⊉", "\\nsupseteq", !0), d(g, y, x, "⊨", "\\models"), d(g, y, x, "←", "\\leftarrow", !0), d(g, y, x, "≤", "\\le"), d(g, y, x, "≤", "\\leq", !0), d(g, y, x, "<", "\\lt", !0), d(g, y, x, "→", "\\rightarrow", !0), d(g, y, x, "→", "\\to"), d(g, B, x, "≱", "\\ngeq", !0), d(g, B, x, "≰", "\\nleq", !0), d(g, y, Ye, " ", "\\ "), d(g, y, Ye, " ", "\\space"), d(g, y, Ye, " ", "\\nobreakspace"), d(Z, y, Ye, " ", "\\ "), d(Z, y, Ye, " ", " "), d(Z, y, Ye, " ", "\\space"), d(Z, y, Ye, " ", "\\nobreakspace"), d(g, y, Ye, null, "\\nobreak"), d(g, y, Ye, null, "\\allowbreak"), d(g, y, le, ",", ","), d(g, y, le, ";", ";"), d(g, B, fe, "⊼", "\\barwedge", !0), d(g, B, fe, "⊻", "\\veebar", !0), d(g, y, fe, "⊙", "\\odot", !0), d(g, y, fe, "⊕", "\\oplus", !0), d(g, y, fe, "⊗", "\\otimes", !0), d(g, y, H, "∂", "\\partial", !0), d(g, y, fe, "⊘", "\\oslash", !0), d(g, B, fe, "⊚", "\\circledcirc", !0), d(g, B, fe, "⊡", "\\boxdot", !0), d(g, y, fe, "△", "\\bigtriangleup"), d(g, y, fe, "▽", "\\bigtriangledown"), d(g, y, fe, "†", "\\dagger"), d(g, y, fe, "⋄", "\\diamond"), d(g, y, fe, "⋆", "\\star"), d(g, y, fe, "◃", "\\triangleleft"), d(g, y, fe, "▹", "\\triangleright"), d(g, y, G, "{", "\\{"), d(Z, y, H, "{", "\\{"), d(Z, y, H, "{", "\\textbraceleft"), d(g, y, pt, "}", "\\}"), d(Z, y, H, "}", "\\}"), d(Z, y, H, "}", "\\textbraceright"), d(g, y, G, "{", "\\lbrace"), d(g, y, pt, "}", "\\rbrace"), d(g, y, G, "[", "\\lbrack", !0), d(Z, y, H, "[", "\\lbrack", !0), d(g, y, pt, "]", "\\rbrack", !0), d(Z, y, H, "]", "\\rbrack", !0), d(g, y, G, "(", "\\lparen", !0), d(g, y, pt, ")", "\\rparen", !0), d(Z, y, H, "<", "\\textless", !0), d(Z, y, H, ">", "\\textgreater", !0), d(g, y, G, "⌊", "\\lfloor", !0), d(g, y, pt, "⌋", "\\rfloor", !0), d(g, y, G, "⌈", "\\lceil", !0), d(g, y, pt, "⌉", "\\rceil", !0), d(g, y, H, "\\", "\\backslash"), d(g, y, H, "∣", "|"), d(g, y, H, "∣", "\\vert"), d(Z, y, H, "|", "\\textbar", !0), d(g, y, H, "∥", "\\|"), d(g, y, H, "∥", "\\Vert"), d(Z, y, H, "∥", "\\textbardbl"), d(Z, y, H, "~", "\\textasciitilde"), d(Z, y, H, "\\", "\\textbackslash"), d(Z, y, H, "^", "\\textasciicircum"), d(g, y, x, "↑", "\\uparrow", !0), d(g, y, x, "⇑", "\\Uparrow", !0), d(g, y, x, "↓", "\\downarrow", !0), d(g, y, x, "⇓", "\\Downarrow", !0), d(g, y, x, "↕", "\\updownarrow", !0), d(g, y, x, "⇕", "\\Updownarrow", !0), d(g, y, ue, "∐", "\\coprod"), d(g, y, ue, "⋁", "\\bigvee"), d(g, y, ue, "⋀", "\\bigwedge"), d(g, y, ue, "⨄", "\\biguplus"), d(g, y, ue, "⋂", "\\bigcap"), d(g, y, ue, "⋃", "\\bigcup"), d(g, y, ue, "∫", "\\int"), d(g, y, ue, "∫", "\\intop"), d(g, y, ue, "∬", "\\iint"), d(g, y, ue, "∭", "\\iiint"), d(g, y, ue, "∏", "\\prod"), d(g, y, ue, "∑", "\\sum"), d(g, y, ue, "⨂", "\\bigotimes"), d(g, y, ue, "⨁", "\\bigoplus"), d(g, y, ue, "⨀", "\\bigodot"), d(g, y, ue, "∮", "\\oint"), d(g, y, ue, "∯", "\\oiint"), d(g, y, ue, "∰", "\\oiiint"), d(g, y, ue, "⨆", "\\bigsqcup"), d(g, y, ue, "∫", "\\smallint"), d(Z, y, kn, "…", "\\textellipsis"), d(g, y, kn, "…", "\\mathellipsis"), d(Z, y, kn, "…", "\\ldots", !0), d(g, y, kn, "…", "\\ldots", !0), d(g, y, kn, "⋯", "\\@cdots", !0), d(g, y, kn, "⋱", "\\ddots", !0), d(g, y, H, "⋮", "\\varvdots"), d(g, y, ze, "ˊ", "\\acute"), d(g, y, ze, "ˋ", "\\grave"), d(g, y, ze, "¨", "\\ddot"), d(g, y, ze, "~", "\\tilde"), d(g, y, ze, "ˉ", "\\bar"), d(g, y, ze, "˘", "\\breve"), d(g, y, ze, "ˇ", "\\check"), d(g, y, ze, "^", "\\hat"), d(g, y, ze, "⃗", "\\vec"), d(g, y, ze, "˙", "\\dot"), d(g, y, ze, "˚", "\\mathring"), d(g, y, De, "", "\\@imath"), d(g, y, De, "", "\\@jmath"), d(g, y, H, "ı", "ı"), d(g, y, H, "ȷ", "ȷ"), d(Z, y, H, "ı", "\\i", !0), d(Z, y, H, "ȷ", "\\j", !0), d(Z, y, H, "ß", "\\ss", !0), d(Z, y, H, "æ", "\\ae", !0), d(Z, y, H, "œ", "\\oe", !0), d(Z, y, H, "ø", "\\o", !0), d(Z, y, H, "Æ", "\\AE", !0), d(Z, y, H, "Œ", "\\OE", !0), d(Z, y, H, "Ø", "\\O", !0), d(Z, y, ze, "ˊ", "\\'"), d(Z, y, ze, "ˋ", "\\`"), d(Z, y, ze, "ˆ", "\\^"), d(Z, y, ze, "˜", "\\~"), d(Z, y, ze, "ˉ", "\\="), d(Z, y, ze, "˘", "\\u"), d(Z, y, ze, "˙", "\\."), d(Z, y, ze, "¸", "\\c"), d(Z, y, ze, "˚", "\\r"), d(Z, y, ze, "ˇ", "\\v"), d(Z, y, ze, "¨", '\\"'), d(Z, y, ze, "˝", "\\H"), d(Z, y, ze, "◯", "\\textcircled");
+                    d(g, y, x, "≡", "\\equiv", !0), d(g, y, x, "≺", "\\prec", !0), d(g, y, x, "≻", "\\succ", !0), d(g, y, x, "∼", "\\sim", !0), d(g, y, x, "⊥", "\\perp"), d(g, y, x, "⪯", "\\preceq", !0), d(g, y, x, "⪰", "\\succeq", !0), d(g, y, x, "≃", "\\simeq", !0), d(g, y, x, "∣", "\\mid", !0), d(g, y, x, "≪", "\\ll", !0), d(g, y, x, "≫", "\\gg", !0), d(g, y, x, "≍", "\\asymp", !0), d(g, y, x, "∥", "\\parallel"), d(g, y, x, "⋈", "\\bowtie", !0), d(g, y, x, "⌣", "\\smile", !0), d(g, y, x, "⊑", "\\sqsubseteq", !0), d(g, y, x, "⊒", "\\sqsupseteq", !0), d(g, y, x, "≐", "\\doteq", !0), d(g, y, x, "⌢", "\\frown", !0), d(g, y, x, "∋", "\\ni", !0), d(g, y, x, "∝", "\\propto", !0), d(g, y, x, "⊢", "\\vdash", !0), d(g, y, x, "⊣", "\\dashv", !0), d(g, y, x, "∋", "\\owns"), d(g, y, ie, ".", "\\ldotp"), d(g, y, ie, "⋅", "\\cdotp"), d(g, y, H, "#", "\\#"), d(Z, y, H, "#", "\\#"), d(g, y, H, "&", "\\&"), d(Z, y, H, "&", "\\&"), d(g, y, H, "ℵ", "\\aleph", !0), d(g, y, H, "∀", "\\forall", !0), d(g, y, H, "ℏ", "\\hbar", !0), d(g, y, H, "∃", "\\exists", !0), d(g, y, H, "∇", "\\nabla", !0), d(g, y, H, "♭", "\\flat", !0), d(g, y, H, "ℓ", "\\ell", !0), d(g, y, H, "♮", "\\natural", !0), d(g, y, H, "♣", "\\clubsuit", !0), d(g, y, H, "℘", "\\wp", !0), d(g, y, H, "♯", "\\sharp", !0), d(g, y, H, "♢", "\\diamondsuit", !0), d(g, y, H, "ℜ", "\\Re", !0), d(g, y, H, "♡", "\\heartsuit", !0), d(g, y, H, "ℑ", "\\Im", !0), d(g, y, H, "♠", "\\spadesuit", !0), d(g, y, H, "§", "\\S", !0), d(Z, y, H, "§", "\\S"), d(g, y, H, "¶", "\\P", !0), d(Z, y, H, "¶", "\\P"), d(g, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\textdagger"), d(g, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\textdaggerdbl"), d(g, y, pt, "⎱", "\\rmoustache", !0), d(g, y, G, "⎰", "\\lmoustache", !0), d(g, y, pt, "⟯", "\\rgroup", !0), d(g, y, G, "⟮", "\\lgroup", !0), d(g, y, fe, "∓", "\\mp", !0), d(g, y, fe, "⊖", "\\ominus", !0), d(g, y, fe, "⊎", "\\uplus", !0), d(g, y, fe, "⊓", "\\sqcap", !0), d(g, y, fe, "∗", "\\ast"), d(g, y, fe, "⊔", "\\sqcup", !0), d(g, y, fe, "◯", "\\bigcirc", !0), d(g, y, fe, "∙", "\\bullet", !0), d(g, y, fe, "‡", "\\ddagger"), d(g, y, fe, "≀", "\\wr", !0), d(g, y, fe, "⨿", "\\amalg"), d(g, y, fe, "&", "\\And"), d(g, y, x, "⟵", "\\longleftarrow", !0), d(g, y, x, "⇐", "\\Leftarrow", !0), d(g, y, x, "⟸", "\\Longleftarrow", !0), d(g, y, x, "⟶", "\\longrightarrow", !0), d(g, y, x, "⇒", "\\Rightarrow", !0), d(g, y, x, "⟹", "\\Longrightarrow", !0), d(g, y, x, "↔", "\\leftrightarrow", !0), d(g, y, x, "⟷", "\\longleftrightarrow", !0), d(g, y, x, "⇔", "\\Leftrightarrow", !0), d(g, y, x, "⟺", "\\Longleftrightarrow", !0), d(g, y, x, "↦", "\\mapsto", !0), d(g, y, x, "⟼", "\\longmapsto", !0), d(g, y, x, "↗", "\\nearrow", !0), d(g, y, x, "↩", "\\hookleftarrow", !0), d(g, y, x, "↪", "\\hookrightarrow", !0), d(g, y, x, "↘", "\\searrow", !0), d(g, y, x, "↼", "\\leftharpoonup", !0), d(g, y, x, "⇀", "\\rightharpoonup", !0), d(g, y, x, "↙", "\\swarrow", !0), d(g, y, x, "↽", "\\leftharpoondown", !0), d(g, y, x, "⇁", "\\rightharpoondown", !0), d(g, y, x, "↖", "\\nwarrow", !0), d(g, y, x, "⇌", "\\rightleftharpoons", !0), d(g, B, x, "≮", "\\nless", !0), d(g, B, x, "", "\\@nleqslant"), d(g, B, x, "", "\\@nleqq"), d(g, B, x, "⪇", "\\lneq", !0), d(g, B, x, "≨", "\\lneqq", !0), d(g, B, x, "", "\\@lvertneqq"), d(g, B, x, "⋦", "\\lnsim", !0), d(g, B, x, "⪉", "\\lnapprox", !0), d(g, B, x, "⊀", "\\nprec", !0), d(g, B, x, "⋠", "\\npreceq", !0), d(g, B, x, "⋨", "\\precnsim", !0), d(g, B, x, "⪹", "\\precnapprox", !0), d(g, B, x, "≁", "\\nsim", !0), d(g, B, x, "", "\\@nshortmid"), d(g, B, x, "∤", "\\nmid", !0), d(g, B, x, "⊬", "\\nvdash", !0), d(g, B, x, "⊭", "\\nvDash", !0), d(g, B, x, "⋪", "\\ntriangleleft"), d(g, B, x, "⋬", "\\ntrianglelefteq", !0), d(g, B, x, "⊊", "\\subsetneq", !0), d(g, B, x, "", "\\@varsubsetneq"), d(g, B, x, "⫋", "\\subsetneqq", !0), d(g, B, x, "", "\\@varsubsetneqq"), d(g, B, x, "≯", "\\ngtr", !0), d(g, B, x, "", "\\@ngeqslant"), d(g, B, x, "", "\\@ngeqq"), d(g, B, x, "⪈", "\\gneq", !0), d(g, B, x, "≩", "\\gneqq", !0), d(g, B, x, "", "\\@gvertneqq"), d(g, B, x, "⋧", "\\gnsim", !0), d(g, B, x, "⪊", "\\gnapprox", !0), d(g, B, x, "⊁", "\\nsucc", !0), d(g, B, x, "⋡", "\\nsucceq", !0), d(g, B, x, "⋩", "\\succnsim", !0), d(g, B, x, "⪺", "\\succnapprox", !0), d(g, B, x, "≆", "\\ncong", !0), d(g, B, x, "", "\\@nshortparallel"), d(g, B, x, "∦", "\\nparallel", !0), d(g, B, x, "⊯", "\\nVDash", !0), d(g, B, x, "⋫", "\\ntriangleright"), d(g, B, x, "⋭", "\\ntrianglerighteq", !0), d(g, B, x, "", "\\@nsupseteqq"), d(g, B, x, "⊋", "\\supsetneq", !0), d(g, B, x, "", "\\@varsupsetneq"), d(g, B, x, "⫌", "\\supsetneqq", !0), d(g, B, x, "", "\\@varsupsetneqq"), d(g, B, x, "⊮", "\\nVdash", !0), d(g, B, x, "⪵", "\\precneqq", !0), d(g, B, x, "⪶", "\\succneqq", !0), d(g, B, x, "", "\\@nsubseteqq"), d(g, B, fe, "⊴", "\\unlhd"), d(g, B, fe, "⊵", "\\unrhd"), d(g, B, x, "↚", "\\nleftarrow", !0), d(g, B, x, "↛", "\\nrightarrow", !0), d(g, B, x, "⇍", "\\nLeftarrow", !0), d(g, B, x, "⇏", "\\nRightarrow", !0), d(g, B, x, "↮", "\\nleftrightarrow", !0), d(g, B, x, "⇎", "\\nLeftrightarrow", !0), d(g, B, x, "△", "\\vartriangle"), d(g, B, H, "ℏ", "\\hslash"), d(g, B, H, "▽", "\\triangledown"), d(g, B, H, "◊", "\\lozenge"), d(g, B, H, "Ⓢ", "\\circledS"), d(g, B, H, "®", "\\circledR"), d(Z, B, H, "®", "\\circledR"), d(g, B, H, "∡", "\\measuredangle", !0), d(g, B, H, "∄", "\\nexists"), d(g, B, H, "℧", "\\mho"), d(g, B, H, "Ⅎ", "\\Finv", !0), d(g, B, H, "⅁", "\\Game", !0), d(g, B, H, "‵", "\\backprime"), d(g, B, H, "▲", "\\blacktriangle"), d(g, B, H, "▼", "\\blacktriangledown"), d(g, B, H, "■", "\\blacksquare"), d(g, B, H, "⧫", "\\blacklozenge"), d(g, B, H, "★", "\\bigstar"), d(g, B, H, "∢", "\\sphericalangle", !0), d(g, B, H, "∁", "\\complement", !0), d(g, B, H, "ð", "\\eth", !0), d(Z, y, H, "ð", "ð"), d(g, B, H, "╱", "\\diagup"), d(g, B, H, "╲", "\\diagdown"), d(g, B, H, "□", "\\square"), d(g, B, H, "□", "\\Box"), d(g, B, H, "◊", "\\Diamond"), d(g, B, H, "¥", "\\yen", !0), d(Z, B, H, "¥", "\\yen", !0), d(g, B, H, "✓", "\\checkmark", !0), d(Z, B, H, "✓", "\\checkmark"), d(g, B, H, "ℶ", "\\beth", !0), d(g, B, H, "ℸ", "\\daleth", !0), d(g, B, H, "ℷ", "\\gimel", !0), d(g, B, H, "ϝ", "\\digamma", !0), d(g, B, H, "ϰ", "\\varkappa"), d(g, B, G, "┌", "\\@ulcorner", !0), d(g, B, pt, "┐", "\\@urcorner", !0), d(g, B, G, "└", "\\@llcorner", !0), d(g, B, pt, "┘", "\\@lrcorner", !0), d(g, B, x, "≦", "\\leqq", !0), d(g, B, x, "⩽", "\\leqslant", !0), d(g, B, x, "⪕", "\\eqslantless", !0), d(g, B, x, "≲", "\\lesssim", !0), d(g, B, x, "⪅", "\\lessapprox", !0), d(g, B, x, "≊", "\\approxeq", !0), d(g, B, fe, "⋖", "\\lessdot"), d(g, B, x, "⋘", "\\lll", !0), d(g, B, x, "≶", "\\lessgtr", !0), d(g, B, x, "⋚", "\\lesseqgtr", !0), d(g, B, x, "⪋", "\\lesseqqgtr", !0), d(g, B, x, "≑", "\\doteqdot"), d(g, B, x, "≓", "\\risingdotseq", !0), d(g, B, x, "≒", "\\fallingdotseq", !0), d(g, B, x, "∽", "\\backsim", !0), d(g, B, x, "⋍", "\\backsimeq", !0), d(g, B, x, "⫅", "\\subseteqq", !0), d(g, B, x, "⋐", "\\Subset", !0), d(g, B, x, "⊏", "\\sqsubset", !0), d(g, B, x, "≼", "\\preccurlyeq", !0), d(g, B, x, "⋞", "\\curlyeqprec", !0), d(g, B, x, "≾", "\\precsim", !0), d(g, B, x, "⪷", "\\precapprox", !0), d(g, B, x, "⊲", "\\vartriangleleft"), d(g, B, x, "⊴", "\\trianglelefteq"), d(g, B, x, "⊨", "\\vDash", !0), d(g, B, x, "⊪", "\\Vvdash", !0), d(g, B, x, "⌣", "\\smallsmile"), d(g, B, x, "⌢", "\\smallfrown"), d(g, B, x, "≏", "\\bumpeq", !0), d(g, B, x, "≎", "\\Bumpeq", !0), d(g, B, x, "≧", "\\geqq", !0), d(g, B, x, "⩾", "\\geqslant", !0), d(g, B, x, "⪖", "\\eqslantgtr", !0), d(g, B, x, "≳", "\\gtrsim", !0), d(g, B, x, "⪆", "\\gtrapprox", !0), d(g, B, fe, "⋗", "\\gtrdot"), d(g, B, x, "⋙", "\\ggg", !0), d(g, B, x, "≷", "\\gtrless", !0), d(g, B, x, "⋛", "\\gtreqless", !0), d(g, B, x, "⪌", "\\gtreqqless", !0), d(g, B, x, "≖", "\\eqcirc", !0), d(g, B, x, "≗", "\\circeq", !0), d(g, B, x, "≜", "\\triangleq", !0), d(g, B, x, "∼", "\\thicksim"), d(g, B, x, "≈", "\\thickapprox"), d(g, B, x, "⫆", "\\supseteqq", !0), d(g, B, x, "⋑", "\\Supset", !0), d(g, B, x, "⊐", "\\sqsupset", !0), d(g, B, x, "≽", "\\succcurlyeq", !0), d(g, B, x, "⋟", "\\curlyeqsucc", !0), d(g, B, x, "≿", "\\succsim", !0), d(g, B, x, "⪸", "\\succapprox", !0), d(g, B, x, "⊳", "\\vartriangleright"), d(g, B, x, "⊵", "\\trianglerighteq"), d(g, B, x, "⊩", "\\Vdash", !0), d(g, B, x, "∣", "\\shortmid"), d(g, B, x, "∥", "\\shortparallel"), d(g, B, x, "≬", "\\between", !0), d(g, B, x, "⋔", "\\pitchfork", !0), d(g, B, x, "∝", "\\varpropto"), d(g, B, x, "◀", "\\blacktriangleleft"), d(g, B, x, "∴", "\\therefore", !0), d(g, B, x, "∍", "\\backepsilon"), d(g, B, x, "▶", "\\blacktriangleright"), d(g, B, x, "∵", "\\because", !0), d(g, B, x, "⋘", "\\llless"), d(g, B, x, "⋙", "\\gggtr"), d(g, B, fe, "⊲", "\\lhd"), d(g, B, fe, "⊳", "\\rhd"), d(g, B, x, "≂", "\\eqsim", !0), d(g, y, x, "⋈", "\\Join"), d(g, B, x, "≑", "\\Doteq", !0), d(g, B, fe, "∔", "\\dotplus", !0), d(g, B, fe, "∖", "\\smallsetminus"), d(g, B, fe, "⋒", "\\Cap", !0), d(g, B, fe, "⋓", "\\Cup", !0), d(g, B, fe, "⩞", "\\doublebarwedge", !0), d(g, B, fe, "⊟", "\\boxminus", !0), d(g, B, fe, "⊞", "\\boxplus", !0), d(g, B, fe, "⋇", "\\divideontimes", !0), d(g, B, fe, "⋉", "\\ltimes", !0), d(g, B, fe, "⋊", "\\rtimes", !0), d(g, B, fe, "⋋", "\\leftthreetimes", !0), d(g, B, fe, "⋌", "\\rightthreetimes", !0), d(g, B, fe, "⋏", "\\curlywedge", !0), d(g, B, fe, "⋎", "\\curlyvee", !0), d(g, B, fe, "⊝", "\\circleddash", !0), d(g, B, fe, "⊛", "\\circledast", !0), d(g, B, fe, "⋅", "\\centerdot"), d(g, B, fe, "⊺", "\\intercal", !0), d(g, B, fe, "⋒", "\\doublecap"), d(g, B, fe, "⋓", "\\doublecup"), d(g, B, fe, "⊠", "\\boxtimes", !0), d(g, B, x, "⇢", "\\dashrightarrow", !0), d(g, B, x, "⇠", "\\dashleftarrow", !0), d(g, B, x, "⇇", "\\leftleftarrows", !0), d(g, B, x, "⇆", "\\leftrightarrows", !0), d(g, B, x, "⇚", "\\Lleftarrow", !0), d(g, B, x, "↞", "\\twoheadleftarrow", !0), d(g, B, x, "↢", "\\leftarrowtail", !0), d(g, B, x, "↫", "\\looparrowleft", !0), d(g, B, x, "⇋", "\\leftrightharpoons", !0), d(g, B, x, "↶", "\\curvearrowleft", !0), d(g, B, x, "↺", "\\circlearrowleft", !0), d(g, B, x, "↰", "\\Lsh", !0), d(g, B, x, "⇈", "\\upuparrows", !0), d(g, B, x, "↿", "\\upharpoonleft", !0), d(g, B, x, "⇃", "\\downharpoonleft", !0), d(g, y, x, "⊶", "\\origof", !0), d(g, y, x, "⊷", "\\imageof", !0), d(g, B, x, "⊸", "\\multimap", !0), d(g, B, x, "↭", "\\leftrightsquigarrow", !0), d(g, B, x, "⇉", "\\rightrightarrows", !0), d(g, B, x, "⇄", "\\rightleftarrows", !0), d(g, B, x, "↠", "\\twoheadrightarrow", !0), d(g, B, x, "↣", "\\rightarrowtail", !0), d(g, B, x, "↬", "\\looparrowright", !0), d(g, B, x, "↷", "\\curvearrowright", !0), d(g, B, x, "↻", "\\circlearrowright", !0), d(g, B, x, "↱", "\\Rsh", !0), d(g, B, x, "⇊", "\\downdownarrows", !0), d(g, B, x, "↾", "\\upharpoonright", !0), d(g, B, x, "⇂", "\\downharpoonright", !0), d(g, B, x, "⇝", "\\rightsquigarrow", !0), d(g, B, x, "⇝", "\\leadsto"), d(g, B, x, "⇛", "\\Rrightarrow", !0), d(g, B, x, "↾", "\\restriction"), d(g, y, H, "‘", "`"), d(g, y, H, "$", "\\$"), d(Z, y, H, "$", "\\$"), d(Z, y, H, "$", "\\textdollar"), d(g, y, H, "%", "\\%"), d(Z, y, H, "%", "\\%"), d(g, y, H, "_", "\\_"), d(Z, y, H, "_", "\\_"), d(Z, y, H, "_", "\\textunderscore"), d(g, y, H, "∠", "\\angle", !0), d(g, y, H, "∞", "\\infty", !0), d(g, y, H, "′", "\\prime"), d(g, y, H, "△", "\\triangle"), d(g, y, H, "Γ", "\\Gamma", !0), d(g, y, H, "Δ", "\\Delta", !0), d(g, y, H, "Θ", "\\Theta", !0), d(g, y, H, "Λ", "\\Lambda", !0), d(g, y, H, "Ξ", "\\Xi", !0), d(g, y, H, "Π", "\\Pi", !0), d(g, y, H, "Σ", "\\Sigma", !0), d(g, y, H, "Υ", "\\Upsilon", !0), d(g, y, H, "Φ", "\\Phi", !0), d(g, y, H, "Ψ", "\\Psi", !0), d(g, y, H, "Ω", "\\Omega", !0), d(g, y, H, "A", "Α"), d(g, y, H, "B", "Β"), d(g, y, H, "E", "Ε"), d(g, y, H, "Z", "Ζ"), d(g, y, H, "H", "Η"), d(g, y, H, "I", "Ι"), d(g, y, H, "K", "Κ"), d(g, y, H, "M", "Μ"), d(g, y, H, "N", "Ν"), d(g, y, H, "O", "Ο"), d(g, y, H, "P", "Ρ"), d(g, y, H, "T", "Τ"), d(g, y, H, "X", "Χ"), d(g, y, H, "¬", "\\neg", !0), d(g, y, H, "¬", "\\lnot"), d(g, y, H, "⊤", "\\top"), d(g, y, H, "⊥", "\\bot"), d(g, y, H, "∅", "\\emptyset"), d(g, B, H, "∅", "\\varnothing"), d(g, y, De, "α", "\\alpha", !0), d(g, y, De, "β", "\\beta", !0), d(g, y, De, "γ", "\\gamma", !0), d(g, y, De, "δ", "\\delta", !0), d(g, y, De, "ϵ", "\\epsilon", !0), d(g, y, De, "ζ", "\\zeta", !0), d(g, y, De, "η", "\\eta", !0), d(g, y, De, "θ", "\\theta", !0), d(g, y, De, "ι", "\\iota", !0), d(g, y, De, "κ", "\\kappa", !0), d(g, y, De, "λ", "\\lambda", !0), d(g, y, De, "μ", "\\mu", !0), d(g, y, De, "ν", "\\nu", !0), d(g, y, De, "ξ", "\\xi", !0), d(g, y, De, "ο", "\\omicron", !0), d(g, y, De, "π", "\\pi", !0), d(g, y, De, "ρ", "\\rho", !0), d(g, y, De, "σ", "\\sigma", !0), d(g, y, De, "τ", "\\tau", !0), d(g, y, De, "υ", "\\upsilon", !0), d(g, y, De, "ϕ", "\\phi", !0), d(g, y, De, "χ", "\\chi", !0), d(g, y, De, "ψ", "\\psi", !0), d(g, y, De, "ω", "\\omega", !0), d(g, y, De, "ε", "\\varepsilon", !0), d(g, y, De, "ϑ", "\\vartheta", !0), d(g, y, De, "ϖ", "\\varpi", !0), d(g, y, De, "ϱ", "\\varrho", !0), d(g, y, De, "ς", "\\varsigma", !0), d(g, y, De, "φ", "\\varphi", !0), d(g, y, fe, "∗", "*", !0), d(g, y, fe, "+", "+"), d(g, y, fe, "−", "-", !0), d(g, y, fe, "⋅", "\\cdot", !0), d(g, y, fe, "∘", "\\circ", !0), d(g, y, fe, "÷", "\\div", !0), d(g, y, fe, "±", "\\pm", !0), d(g, y, fe, "×", "\\times", !0), d(g, y, fe, "∩", "\\cap", !0), d(g, y, fe, "∪", "\\cup", !0), d(g, y, fe, "∖", "\\setminus", !0), d(g, y, fe, "∧", "\\land"), d(g, y, fe, "∨", "\\lor"), d(g, y, fe, "∧", "\\wedge", !0), d(g, y, fe, "∨", "\\vee", !0), d(g, y, H, "√", "\\surd"), d(g, y, G, "⟨", "\\langle", !0), d(g, y, G, "∣", "\\lvert"), d(g, y, G, "∥", "\\lVert"), d(g, y, pt, "?", "?"), d(g, y, pt, "!", "!"), d(g, y, pt, "⟩", "\\rangle", !0), d(g, y, pt, "∣", "\\rvert"), d(g, y, pt, "∥", "\\rVert"), d(g, y, x, "=", "="), d(g, y, x, ":", ":"), d(g, y, x, "≈", "\\approx", !0), d(g, y, x, "≅", "\\cong", !0), d(g, y, x, "≥", "\\ge"), d(g, y, x, "≥", "\\geq", !0), d(g, y, x, "←", "\\gets"), d(g, y, x, ">", "\\gt", !0), d(g, y, x, "∈", "\\in", !0), d(g, y, x, "", "\\@not"), d(g, y, x, "⊂", "\\subset", !0), d(g, y, x, "⊃", "\\supset", !0), d(g, y, x, "⊆", "\\subseteq", !0), d(g, y, x, "⊇", "\\supseteq", !0), d(g, B, x, "⊈", "\\nsubseteq", !0), d(g, B, x, "⊉", "\\nsupseteq", !0), d(g, y, x, "⊨", "\\models"), d(g, y, x, "←", "\\leftarrow", !0), d(g, y, x, "≤", "\\le"), d(g, y, x, "≤", "\\leq", !0), d(g, y, x, "<", "\\lt", !0), d(g, y, x, "→", "\\rightarrow", !0), d(g, y, x, "→", "\\to"), d(g, B, x, "≱", "\\ngeq", !0), d(g, B, x, "≰", "\\nleq", !0), d(g, y, Ye, " ", "\\ "), d(g, y, Ye, " ", "\\space"), d(g, y, Ye, " ", "\\nobreakspace"), d(Z, y, Ye, " ", "\\ "), d(Z, y, Ye, " ", " "), d(Z, y, Ye, " ", "\\space"), d(Z, y, Ye, " ", "\\nobreakspace"), d(g, y, Ye, null, "\\nobreak"), d(g, y, Ye, null, "\\allowbreak"), d(g, y, ie, ",", ","), d(g, y, ie, ";", ";"), d(g, B, fe, "⊼", "\\barwedge", !0), d(g, B, fe, "⊻", "\\veebar", !0), d(g, y, fe, "⊙", "\\odot", !0), d(g, y, fe, "⊕", "\\oplus", !0), d(g, y, fe, "⊗", "\\otimes", !0), d(g, y, H, "∂", "\\partial", !0), d(g, y, fe, "⊘", "\\oslash", !0), d(g, B, fe, "⊚", "\\circledcirc", !0), d(g, B, fe, "⊡", "\\boxdot", !0), d(g, y, fe, "△", "\\bigtriangleup"), d(g, y, fe, "▽", "\\bigtriangledown"), d(g, y, fe, "†", "\\dagger"), d(g, y, fe, "⋄", "\\diamond"), d(g, y, fe, "⋆", "\\star"), d(g, y, fe, "◃", "\\triangleleft"), d(g, y, fe, "▹", "\\triangleright"), d(g, y, G, "{", "\\{"), d(Z, y, H, "{", "\\{"), d(Z, y, H, "{", "\\textbraceleft"), d(g, y, pt, "}", "\\}"), d(Z, y, H, "}", "\\}"), d(Z, y, H, "}", "\\textbraceright"), d(g, y, G, "{", "\\lbrace"), d(g, y, pt, "}", "\\rbrace"), d(g, y, G, "[", "\\lbrack", !0), d(Z, y, H, "[", "\\lbrack", !0), d(g, y, pt, "]", "\\rbrack", !0), d(Z, y, H, "]", "\\rbrack", !0), d(g, y, G, "(", "\\lparen", !0), d(g, y, pt, ")", "\\rparen", !0), d(Z, y, H, "<", "\\textless", !0), d(Z, y, H, ">", "\\textgreater", !0), d(g, y, G, "⌊", "\\lfloor", !0), d(g, y, pt, "⌋", "\\rfloor", !0), d(g, y, G, "⌈", "\\lceil", !0), d(g, y, pt, "⌉", "\\rceil", !0), d(g, y, H, "\\", "\\backslash"), d(g, y, H, "∣", "|"), d(g, y, H, "∣", "\\vert"), d(Z, y, H, "|", "\\textbar", !0), d(g, y, H, "∥", "\\|"), d(g, y, H, "∥", "\\Vert"), d(Z, y, H, "∥", "\\textbardbl"), d(Z, y, H, "~", "\\textasciitilde"), d(Z, y, H, "\\", "\\textbackslash"), d(Z, y, H, "^", "\\textasciicircum"), d(g, y, x, "↑", "\\uparrow", !0), d(g, y, x, "⇑", "\\Uparrow", !0), d(g, y, x, "↓", "\\downarrow", !0), d(g, y, x, "⇓", "\\Downarrow", !0), d(g, y, x, "↕", "\\updownarrow", !0), d(g, y, x, "⇕", "\\Updownarrow", !0), d(g, y, ue, "∐", "\\coprod"), d(g, y, ue, "⋁", "\\bigvee"), d(g, y, ue, "⋀", "\\bigwedge"), d(g, y, ue, "⨄", "\\biguplus"), d(g, y, ue, "⋂", "\\bigcap"), d(g, y, ue, "⋃", "\\bigcup"), d(g, y, ue, "∫", "\\int"), d(g, y, ue, "∫", "\\intop"), d(g, y, ue, "∬", "\\iint"), d(g, y, ue, "∭", "\\iiint"), d(g, y, ue, "∏", "\\prod"), d(g, y, ue, "∑", "\\sum"), d(g, y, ue, "⨂", "\\bigotimes"), d(g, y, ue, "⨁", "\\bigoplus"), d(g, y, ue, "⨀", "\\bigodot"), d(g, y, ue, "∮", "\\oint"), d(g, y, ue, "∯", "\\oiint"), d(g, y, ue, "∰", "\\oiiint"), d(g, y, ue, "⨆", "\\bigsqcup"), d(g, y, ue, "∫", "\\smallint"), d(Z, y, Dn, "…", "\\textellipsis"), d(g, y, Dn, "…", "\\mathellipsis"), d(Z, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "⋯", "\\@cdots", !0), d(g, y, Dn, "⋱", "\\ddots", !0), d(g, y, H, "⋮", "\\varvdots"), d(g, y, ze, "ˊ", "\\acute"), d(g, y, ze, "ˋ", "\\grave"), d(g, y, ze, "¨", "\\ddot"), d(g, y, ze, "~", "\\tilde"), d(g, y, ze, "ˉ", "\\bar"), d(g, y, ze, "˘", "\\breve"), d(g, y, ze, "ˇ", "\\check"), d(g, y, ze, "^", "\\hat"), d(g, y, ze, "⃗", "\\vec"), d(g, y, ze, "˙", "\\dot"), d(g, y, ze, "˚", "\\mathring"), d(g, y, De, "", "\\@imath"), d(g, y, De, "", "\\@jmath"), d(g, y, H, "ı", "ı"), d(g, y, H, "ȷ", "ȷ"), d(Z, y, H, "ı", "\\i", !0), d(Z, y, H, "ȷ", "\\j", !0), d(Z, y, H, "ß", "\\ss", !0), d(Z, y, H, "æ", "\\ae", !0), d(Z, y, H, "œ", "\\oe", !0), d(Z, y, H, "ø", "\\o", !0), d(Z, y, H, "Æ", "\\AE", !0), d(Z, y, H, "Œ", "\\OE", !0), d(Z, y, H, "Ø", "\\O", !0), d(Z, y, ze, "ˊ", "\\'"), d(Z, y, ze, "ˋ", "\\`"), d(Z, y, ze, "ˆ", "\\^"), d(Z, y, ze, "˜", "\\~"), d(Z, y, ze, "ˉ", "\\="), d(Z, y, ze, "˘", "\\u"), d(Z, y, ze, "˙", "\\."), d(Z, y, ze, "¸", "\\c"), d(Z, y, ze, "˚", "\\r"), d(Z, y, ze, "ˇ", "\\v"), d(Z, y, ze, "¨", '\\"'), d(Z, y, ze, "˝", "\\H"), d(Z, y, ze, "◯", "\\textcircled");
                     const Lt = {
                         "--": !0,
                         "---": !0,
                         "``": !0,
                         "''": !0
                     };
                     d(Z, y, H, "–", "--", !0), d(Z, y, H, "–", "\\textendash"), d(Z, y, H, "—", "---", !0), d(Z, y, H, "—", "\\textemdash"), d(Z, y, H, "‘", "`", !0), d(Z, y, H, "‘", "\\textquoteleft"), d(Z, y, H, "’", "'", !0), d(Z, y, H, "’", "\\textquoteright"), d(Z, y, H, "“", "``", !0), d(Z, y, H, "“", "\\textquotedblleft"), d(Z, y, H, "”", "''", !0), d(Z, y, H, "”", "\\textquotedblright"), d(g, y, H, "°", "\\degree", !0), d(Z, y, H, "°", "\\degree"), d(Z, y, H, "°", "\\textdegree", !0), d(g, y, H, "£", "\\pounds"), d(g, y, H, "£", "\\mathsterling", !0), d(Z, y, H, "£", "\\pounds"), d(Z, y, H, "£", "\\textsterling", !0), d(g, B, H, "✠", "\\maltese"), d(Z, B, H, "✠", "\\maltese");
@@ -11738,15 +11738,15 @@
                         Ae = String.fromCharCode(55349, 57294 + i), d(g, y, De, s, Ae), d(Z, y, H, s, Ae), Ae = String.fromCharCode(55349, 57314 + i), d(g, y, De, s, Ae), d(Z, y, H, s, Ae), Ae = String.fromCharCode(55349, 57324 + i), d(g, y, De, s, Ae), d(Z, y, H, s, Ae), Ae = String.fromCharCode(55349, 57334 + i), d(g, y, De, s, Ae), d(Z, y, H, s, Ae);
                     }
                     const or = "ÐÞþ";
                     for (let i = 0; i < or.length; i++) {
                         const s = or.charAt(i);
                         d(g, y, De, s, s), d(Z, y, H, s, s);
                     }
-                    const P0 = [
+                    const q0 = [
                             ["mathbf", "textbf", "Main-Bold"],
                             // A-Z bold upright
                             ["mathbf", "textbf", "Main-Bold"],
                             // a-z bold upright
                             ["mathnormal", "textit", "Math-Italic"],
                             // A-Z italic
                             ["mathnormal", "textit", "Math-Italic"],
@@ -11814,21 +11814,21 @@
                         rd = function(i, s) {
                             const a = i.charCodeAt(0),
                                 f = i.charCodeAt(1),
                                 m = (a - 55296) * 1024 + (f - 56320) + 65536,
                                 b = s === "math" ? 0 : 1;
                             if (119808 <= m && m < 120484) {
                                 const w = Math.floor((m - 119808) / 26);
-                                return [P0[w][2], P0[w][b]];
+                                return [q0[w][2], q0[w][b]];
                             } else if (120782 <= m && m <= 120831) {
                                 const w = Math.floor((m - 120782) / 10);
                                 return [mo[w][2], mo[w][b]];
                             } else {
                                 if (m === 120485 || m === 120486)
-                                    return [P0[0][2], P0[0][b]];
+                                    return [q0[0][2], q0[0][b]];
                                 if (120486 < m && m < 120782)
                                     return ["", ""];
                                 throw new o("Unsupported character: " + i);
                             }
                         },
                         Fs = function(i, s, a) {
                             return q[a][i] && q[a][i].replace && (i = q[a][i].replace), {
@@ -11905,15 +11905,15 @@
                                     const W = Cs(j, s.fontWeight, s.fontShape);
                                     return zn(m, W, f, s, b.concat(W, s.fontWeight, s.fontShape));
                                 }
                             } else
                                 throw new Error("unexpected type: " + a + " in makeOrd");
                         },
                         ad = (i, s) => {
-                            if (Gt(i.classes) !== Gt(s.classes) || i.skew !== s.skew || i.maxFontSize !== s.maxFontSize)
+                            if (Ut(i.classes) !== Ut(s.classes) || i.skew !== s.skew || i.maxFontSize !== s.maxFontSize)
                                 return !1;
                             if (i.classes.length === 1) {
                                 const a = i.classes[0];
                                 if (a === "mbin" || a === "mord")
                                     return !1;
                             }
                             for (const a in i.style)
@@ -11939,21 +11939,21 @@
                             for (let m = 0; m < i.children.length; m++) {
                                 const b = i.children[m];
                                 b.height > s && (s = b.height), b.depth > a && (a = b.depth), b.maxFontSize > f && (f = b.maxFontSize);
                             }
                             i.height = s, i.depth = a, i.maxFontSize = f;
                         },
                         sn = function(i, s, a, f) {
-                            const m = new s0(i, s, a, f);
+                            const m = new i0(i, s, a, f);
                             return el(m), m;
                         },
-                        po = (i, s, a, f) => new s0(i, s, a, f),
+                        po = (i, s, a, f) => new i0(i, s, a, f),
                         ud = function(i, s, a) {
                             const f = sn([i], [], s);
-                            return f.height = Math.max(a || s.fontMetrics().defaultRuleThickness, s.minRuleThickness), f.style.borderBottomWidth = ie(f.height), f.maxFontSize = 1, f;
+                            return f.height = Math.max(a || s.fontMetrics().defaultRuleThickness, s.minRuleThickness), f.style.borderBottomWidth = ae(f.height), f.maxFontSize = 1, f;
                         },
                         cd = function(i, s, a, f) {
                             const m = new wt(i, s, a, f);
                             return el(m), m;
                         },
                         go = function(i) {
                             const s = new Ot(i);
@@ -12018,50 +12018,50 @@
                                 if (be.type === "elem") {
                                     const Te = be.elem;
                                     m = Math.max(m, Te.maxFontSize, Te.height);
                                 }
                             }
                             m += 2;
                             const b = sn(["pstrut"], []);
-                            b.style.height = ie(m);
+                            b.style.height = ae(m);
                             const w = [];
                             let A = f,
                                 F = f,
                                 L = f;
                             for (let te = 0; te < a.length; te++) {
                                 const be = a[te];
                                 if (be.type === "kern")
                                     L += be.size;
                                 else {
                                     const Te = be.elem,
                                         Je = be.wrapperClasses || [],
                                         Ge = be.wrapperStyle || {},
                                         Ke = sn(Je, [b, Te], void 0, Ge);
-                                    Ke.style.top = ie(-m - L - Te.depth), be.marginLeft && (Ke.style.marginLeft = be.marginLeft), be.marginRight && (Ke.style.marginRight = be.marginRight), w.push(Ke), L += Te.height + Te.depth;
+                                    Ke.style.top = ae(-m - L - Te.depth), be.marginLeft && (Ke.style.marginLeft = be.marginLeft), be.marginRight && (Ke.style.marginRight = be.marginRight), w.push(Ke), L += Te.height + Te.depth;
                                 }
                                 A = Math.min(A, L), F = Math.max(F, L);
                             }
                             const j = sn(["vlist"], w);
-                            j.style.height = ie(F);
+                            j.style.height = ae(F);
                             let W;
                             if (A < 0) {
                                 const te = sn([], []),
                                     be = sn(["vlist"], [te]);
-                                be.style.height = ie(-A);
+                                be.style.height = ae(-A);
                                 const Te = sn(["vlist-s"], [new jt("​")]);
                                 W = [sn(["vlist-r"], [j, Te]), sn(["vlist-r"], [be])];
                             } else
                                 W = [sn(["vlist-r"], [j])];
                             const J = sn(["vlist-t"], W);
                             return W.length === 2 && J.classes.push("vlist-t2"), J.height = F, J.depth = -A, J;
                         },
                         md = (i, s) => {
                             const a = sn(["mspace"], [], s),
                                 f = Ze(i, s);
-                            return a.style.marginRight = ie(f), a;
+                            return a.style.marginRight = ae(f), a;
                         },
                         Cs = function(i, s, a) {
                             let f = "";
                             switch (i) {
                                 case "amsrm":
                                     f = "AMS";
                                     break;
@@ -12152,84 +12152,84 @@
                         makeFragment: go,
                         wrapFragment: fd,
                         makeVList: dd,
                         makeOrd: ld,
                         makeGlue: md,
                         staticSvg: function(i, s) {
                             const [a, f, m] = bo[i], b = new dn(a), w = new en([b], {
-                                width: ie(f),
-                                height: ie(m),
+                                width: ae(f),
+                                height: ae(m),
                                 // Override CSS rule `.katex svg { width: 100% }`
-                                style: "width:" + ie(f),
+                                style: "width:" + ae(f),
                                 viewBox: "0 0 " + 1e3 * f + " " + 1e3 * m,
                                 preserveAspectRatio: "xMinYMin"
                             }), A = po(["overlay"], [w], s);
-                            return A.height = m, A.style.height = ie(m), A.style.width = ie(f), A;
+                            return A.height = m, A.style.height = ae(m), A.style.width = ae(f), A;
                         },
                         svgData: bo,
                         tryCombineChars: od
                     };
                     const Et = {
                             number: 3,
                             unit: "mu"
                         },
-                        q0 = {
+                        U0 = {
                             number: 4,
                             unit: "mu"
                         },
-                        i0 = {
+                        l0 = {
                             number: 5,
                             unit: "mu"
                         },
                         pd = {
                             mord: {
                                 mop: Et,
-                                mbin: q0,
-                                mrel: i0,
+                                mbin: U0,
+                                mrel: l0,
                                 minner: Et
                             },
                             mop: {
                                 mord: Et,
                                 mop: Et,
-                                mrel: i0,
+                                mrel: l0,
                                 minner: Et
                             },
                             mbin: {
-                                mord: q0,
-                                mop: q0,
-                                mopen: q0,
-                                minner: q0
+                                mord: U0,
+                                mop: U0,
+                                mopen: U0,
+                                minner: U0
                             },
                             mrel: {
-                                mord: i0,
-                                mop: i0,
-                                mopen: i0,
-                                minner: i0
+                                mord: l0,
+                                mop: l0,
+                                mopen: l0,
+                                minner: l0
                             },
                             mopen: {},
                             mclose: {
                                 mop: Et,
-                                mbin: q0,
-                                mrel: i0,
+                                mbin: U0,
+                                mrel: l0,
                                 minner: Et
                             },
                             mpunct: {
                                 mord: Et,
                                 mop: Et,
-                                mrel: i0,
+                                mrel: l0,
                                 mopen: Et,
                                 mclose: Et,
                                 mpunct: Et,
                                 minner: Et
                             },
                             minner: {
                                 mord: Et,
                                 mop: Et,
-                                mbin: q0,
-                                mrel: i0,
+                                mbin: U0,
+                                mrel: l0,
                                 mopen: Et,
                                 mpunct: Et,
                                 minner: Et
                             }
                         },
                         gd = {
                             mord: {
@@ -12276,15 +12276,15 @@
                             handler: m
                         };
                         for (let F = 0; F < a.length; ++F)
                             wo[a[F]] = A;
                         s && (b && (Ms[s] = b), w && (Bs[s] = w));
                     }
 
-                    function U0(i) {
+                    function G0(i) {
                         let {
                             type: s,
                             htmlBuilder: a,
                             mathmlBuilder: f
                         } = i;
                         _e({
                             type: s,
@@ -12301,15 +12301,15 @@
                     }
                     const Ns = function(i) {
                             return i.type === "ordgroup" && i.body.length === 1 ? i.body[0] : i;
                         },
                         Nt = function(i) {
                             return i.type === "ordgroup" ? i.body : [i];
                         },
-                        l0 = X.makeSpan,
+                        a0 = X.makeSpan,
                         _d = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
                         bd = ["rightmost", "mrel", "mclose", "mpunct"],
                         wd = {
                             display: Q.DISPLAY,
                             text: Q.TEXT,
                             script: Q.SCRIPT,
                             scriptscript: Q.SCRIPTSCRIPT
@@ -12338,16 +12338,16 @@
                             if (X.tryCombineChars(m), !a)
                                 return m;
                             let b = s;
                             if (i.length === 1) {
                                 const L = i[0];
                                 L.type === "sizing" ? b = s.havingSize(L.size) : L.type === "styling" && (b = s.havingStyle(wd[L.style]));
                             }
-                            const w = l0([f[0] || "leftmost"], [], s),
-                                A = l0([f[1] || "rightmost"], [], s),
+                            const w = a0([f[0] || "leftmost"], [], s),
+                                A = a0([f[1] || "rightmost"], [], s),
                                 F = a === "root";
                             return tl(m, (L, j) => {
                                 const W = j.classes[0],
                                     J = L.classes[0];
                                 W === "mbin" && M.contains(bd, J) ? j.classes[0] = "mord" : J === "mbin" && M.contains(_d, W) && (L.classes[0] = "mord");
                             }, {
                                 node: w
@@ -12372,22 +12372,22 @@
                                     continue;
                                 }
                                 const F = !w.hasClass("mspace");
                                 if (F) {
                                     const L = s(w, a.node);
                                     L && (a.insertAfter ? a.insertAfter(L) : (i.unshift(L), b++));
                                 }
-                                F ? a.node = w : m && w.hasClass("newline") && (a.node = l0(["leftmost"])), a.insertAfter = /* @__PURE__ */ ((L) => (j) => {
+                                F ? a.node = w : m && w.hasClass("newline") && (a.node = a0(["leftmost"])), a.insertAfter = /* @__PURE__ */ ((L) => (j) => {
                                     i.splice(L + 1, 0, j), b++;
                                 })(b);
                             }
                             f && i.pop();
                         },
                         yo = function(i) {
-                            return i instanceof Ot || i instanceof wt || i instanceof s0 && i.hasClass("enclosing") ? i : null;
+                            return i instanceof Ot || i instanceof wt || i instanceof i0 && i.hasClass("enclosing") ? i : null;
                         },
                         nl = function(i, s) {
                             const a = yo(i);
                             if (a) {
                                 const f = a.children;
                                 if (f.length) {
                                     if (s === "right")
@@ -12399,35 +12399,35 @@
                             return i;
                         },
                         rl = function(i, s) {
                             return i ? (s && (i = nl(i, s)), yd[i.classes[0]] || null) : null;
                         },
                         Hr = function(i, s) {
                             const a = ["nulldelimiter"].concat(i.baseSizingClasses());
-                            return l0(s.concat(a));
+                            return a0(s.concat(a));
                         },
                         nt = function(i, s, a) {
                             if (!i)
-                                return l0();
+                                return a0();
                             if (Ms[i.type]) {
                                 let f = Ms[i.type](i, s);
                                 if (a && s.size !== a.size) {
-                                    f = l0(s.sizingClasses(a), [f], s);
+                                    f = a0(s.sizingClasses(a), [f], s);
                                     const m = s.sizeMultiplier / a.sizeMultiplier;
                                     f.height *= m, f.depth *= m;
                                 }
                                 return f;
                             } else
                                 throw new o("Got group of unknown type: '" + i.type + "'");
                         };
 
                     function zs(i, s) {
-                        const a = l0(["base"], i, s),
-                            f = l0(["strut"]);
-                        return f.style.height = ie(a.height + a.depth), a.depth && (f.style.verticalAlign = ie(-a.depth)), a.children.unshift(f), a;
+                        const a = a0(["base"], i, s),
+                            f = a0(["strut"]);
+                        return f.style.height = ae(a.height + a.depth), a.depth && (f.style.verticalAlign = ae(-a.depth)), a.children.unshift(f), a;
                     }
 
                     function sl(i, s) {
                         let a = null;
                         i.length === 1 && i[0].type === "tag" && (a = i[0].tag, i = i[0].body);
                         const f = Ht(i, s, "root");
                         let m;
@@ -12441,26 +12441,26 @@
                                     L++, w.push(f[L]), f[L].hasClass("nobreak") && (j = !0);
                                 j || (b.push(zs(w, s)), w = []);
                             } else
                                 f[L].hasClass("newline") && (w.pop(), w.length > 0 && (b.push(zs(w, s)), w = []), b.push(f[L]));
                         w.length > 0 && b.push(zs(w, s));
                         let A;
                         a ? (A = zs(Ht(a, s, !0)), A.classes = ["tag"], b.push(A)) : m && b.push(m);
-                        const F = l0(["katex-html"], b);
+                        const F = a0(["katex-html"], b);
                         if (F.setAttribute("aria-hidden", "true"), A) {
                             const L = A.children[0];
-                            L.style.height = ie(F.height + F.depth), F.depth && (L.style.verticalAlign = ie(-F.depth));
+                            L.style.height = ae(F.height + F.depth), F.depth && (L.style.verticalAlign = ae(-F.depth));
                         }
                         return F;
                     }
 
                     function vo(i) {
                         return new Ot(i);
                     }
-                    class Dn {
+                    class An {
                         constructor(s, a, f) {
                             this.type = void 0, this.attributes = void 0, this.children = void 0, this.classes = void 0, this.type = s, this.attributes = {}, this.children = a || [], this.classes = f || [];
                         }
                         /**
                          * Sets an attribute on a MathML node. MathML depends on attributes to convey a
                          * semantic content, so this is used heavily.
                          */
@@ -12476,27 +12476,27 @@
                         /**
                          * Converts the math node into a MathML-namespaced DOM element.
                          */
                         toNode() {
                             const s = document.createElementNS("http://www.w3.org/1998/Math/MathML", this.type);
                             for (const a in this.attributes)
                                 Object.prototype.hasOwnProperty.call(this.attributes, a) && s.setAttribute(a, this.attributes[a]);
-                            this.classes.length > 0 && (s.className = Gt(this.classes));
+                            this.classes.length > 0 && (s.className = Ut(this.classes));
                             for (let a = 0; a < this.children.length; a++)
                                 s.appendChild(this.children[a].toNode());
                             return s;
                         }
                         /**
                          * Converts the math node into an HTML markup string.
                          */
                         toMarkup() {
                             let s = "<" + this.type;
                             for (const a in this.attributes)
                                 Object.prototype.hasOwnProperty.call(this.attributes, a) && (s += " " + a + '="', s += M.escape(this.attributes[a]), s += '"');
-                            this.classes.length > 0 && (s += ' class ="' + M.escape(Gt(this.classes)) + '"'), s += ">";
+                            this.classes.length > 0 && (s += ' class ="' + M.escape(Ut(this.classes)) + '"'), s += ">";
                             for (let a = 0; a < this.children.length; a++)
                                 s += this.children[a].toMarkup();
                             return s += "</" + this.type + ">", s;
                         }
                         /**
                          * Converts the math node into a string, similar to innerText, but escaped.
                          */
@@ -12540,37 +12540,37 @@
                          * Converts the math node into a MathML-namespaced DOM element.
                          */
                         toNode() {
                             if (this.character)
                                 return document.createTextNode(this.character);
                             {
                                 const s = document.createElementNS("http://www.w3.org/1998/Math/MathML", "mspace");
-                                return s.setAttribute("width", ie(this.width)), s;
+                                return s.setAttribute("width", ae(this.width)), s;
                             }
                         }
                         /**
                          * Converts the math node into an HTML markup string.
                          */
                         toMarkup() {
-                            return this.character ? "<mtext>" + this.character + "</mtext>" : '<mspace width="' + ie(this.width) + '"/>';
+                            return this.character ? "<mtext>" + this.character + "</mtext>" : '<mspace width="' + ae(this.width) + '"/>';
                         }
                         /**
                          * Converts the math node into a string, similar to innerText.
                          */
                         toText() {
                             return this.character ? this.character : " ";
                         }
                     }
                     var se = {
-                        MathNode: Dn,
+                        MathNode: An,
                         TextNode: Pr,
                         SpaceNode: vd,
                         newDocumentFragment: vo
                     };
-                    const An = function(i, s, a) {
+                    const Sn = function(i, s, a) {
                             return q[s][i] && q[s][i].replace && i.charCodeAt(0) !== 55349 && !(Lt.hasOwnProperty(i) && a && (a.fontFamily && a.fontFamily.slice(4, 6) === "tt" || a.font && a.font.slice(4, 6) === "tt")) && (i = q[s][i].replace), new se.TextNode(i);
                         },
                         il = function(i) {
                             return i.length === 1 ? i[0] : new se.MathNode("mrow", i);
                         },
                         ll = function(i, s) {
                             if (s.fontFamily === "texttt")
@@ -12609,21 +12609,21 @@
                             q[f][m] && q[f][m].replace && (m = q[f][m].replace);
                             const b = X.fontMap[a].fontName;
                             return Ee(m, b, f) ? X.fontMap[a].variant : null;
                         },
                         ln = function(i, s, a) {
                             if (i.length === 1) {
                                 const b = ft(i[0], s);
-                                return a && b instanceof Dn && b.type === "mo" && (b.setAttribute("lspace", "0em"), b.setAttribute("rspace", "0em")), [b];
+                                return a && b instanceof An && b.type === "mo" && (b.setAttribute("lspace", "0em"), b.setAttribute("rspace", "0em")), [b];
                             }
                             const f = [];
                             let m;
                             for (let b = 0; b < i.length; b++) {
                                 const w = ft(i[b], s);
-                                if (w instanceof Dn && m instanceof Dn) {
+                                if (w instanceof An && m instanceof An) {
                                     if (w.type === "mtext" && m.type === "mtext" && w.getAttribute("mathvariant") === m.getAttribute("mathvariant")) {
                                         m.children.push(...w.children);
                                         continue;
                                     } else if (w.type === "mn" && m.type === "mn") {
                                         m.children.push(...w.children);
                                         continue;
                                     } else if (w.type === "mi" && w.children.length === 1 && m.type === "mn") {
@@ -12640,29 +12640,29 @@
                                         }
                                     }
                                 }
                                 f.push(w), m = w;
                             }
                             return f;
                         },
-                        g0 = function(i, s, a) {
+                        _0 = function(i, s, a) {
                             return il(ln(i, s, a));
                         },
                         ft = function(i, s) {
                             if (!i)
                                 return new se.MathNode("mrow");
                             if (Bs[i.type])
                                 return Bs[i.type](i, s);
                             throw new o("Got group of unknown type: '" + i.type + "'");
                         };
 
                     function ko(i, s, a, f, m) {
                         const b = ln(i, a);
                         let w;
-                        b.length === 1 && b[0] instanceof Dn && M.contains(["mrow", "mtable"], b[0].type) ? w = b[0] : w = new se.MathNode("mrow", b);
+                        b.length === 1 && b[0] instanceof An && M.contains(["mrow", "mtable"], b[0].type) ? w = b[0] : w = new se.MathNode("mrow", b);
                         const A = new se.MathNode("annotation", [new se.TextNode(s)]);
                         A.setAttribute("encoding", "application/x-tex");
                         const F = new se.MathNode("semantics", [w, A]),
                             L = new se.MathNode("math", [F]);
                         L.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), f && L.setAttribute("display", "block");
                         const j = m ? "katex" : "katex-mathml";
                         return X.makeSpan([j], [L]);
@@ -12879,45 +12879,45 @@
                             xleftequilibrium: [
                                 ["shortbaraboveleftharpoon", "shortrightharpoonabovebar"], 1.75, 716
                             ]
                         },
                         xd = function(i) {
                             return i.type === "ordgroup" ? i.body.length : 1;
                         };
-                    var a0 = {
+                    var o0 = {
                         encloseSpan: function(i, s, a, f, m) {
                             let b;
                             const w = i.height + i.depth + a + f;
                             if (/fbox|color|angl/.test(s)) {
                                 if (b = X.makeSpan(["stretchy", s], [], m), s === "fbox") {
                                     const A = m.color && m.getColor();
                                     A && (b.style.borderColor = A);
                                 }
                             } else {
                                 const A = [];
-                                /^[bx]cancel$/.test(s) && A.push(new p0({
+                                /^[bx]cancel$/.test(s) && A.push(new g0({
                                     x1: "0",
                                     y1: "0",
                                     x2: "100%",
                                     y2: "100%",
                                     "stroke-width": "0.046em"
-                                })), /^x?cancel$/.test(s) && A.push(new p0({
+                                })), /^x?cancel$/.test(s) && A.push(new g0({
                                     x1: "0",
                                     y1: "100%",
                                     x2: "100%",
                                     y2: "0",
                                     "stroke-width": "0.046em"
                                 }));
                                 const F = new en(A, {
                                     width: "100%",
-                                    height: ie(w)
+                                    height: ae(w)
                                 });
                                 b = X.makeSvgSpan([], [F], m);
                             }
-                            return b.height = w, b.style.height = ie(w), b;
+                            return b.height = w, b.style.height = ae(w), b;
                         },
                         mathMLnode: Sd,
                         svgSpan: function(i, s) {
                             function a() {
                                 let w = 4e5;
                                 const A = i.label.slice(1);
                                 if (M.contains(["widehat", "widecheck", "widetilde", "utilde"], A)) {
@@ -12928,15 +12928,15 @@
                                     else {
                                         const Te = [1, 1, 2, 2, 3, 3][L];
                                         A === "widehat" || A === "widecheck" ? (w = [0, 1062, 2364, 2364, 2364][Te], j = [0, 239, 300, 360, 420][Te], J = [0, 0.24, 0.3, 0.3, 0.36, 0.42][Te], W = A + Te) : (w = [0, 600, 1033, 2339, 2340][Te], j = [0, 260, 286, 306, 312][Te], J = [0, 0.26, 0.286, 0.3, 0.306, 0.34][Te], W = "tilde" + Te);
                                     }
                                     const te = new dn(W),
                                         be = new en([te], {
                                             width: "100%",
-                                            height: ie(J),
+                                            height: ae(J),
                                             viewBox: "0 0 " + w + " " + j,
                                             preserveAspectRatio: "none"
                                         });
                                     return {
                                         span: X.makeSvgSpan([], [be], s),
                                         minWidth: 0,
                                         height: J
@@ -12958,40 +12958,40 @@
                                     else
                                         throw new Error(`Correct katexImagesData or update code here to support
                     ` + be + " children.");
                                     for (let Ge = 0; Ge < be; Ge++) {
                                         const Ke = new dn(j[Ge]),
                                             lt = new en([Ke], {
                                                 width: "400em",
-                                                height: ie(te),
+                                                height: ae(te),
                                                 viewBox: "0 0 " + w + " " + J,
                                                 preserveAspectRatio: Je[Ge] + " slice"
                                             }),
                                             mt = X.makeSvgSpan([Te[Ge]], [lt], s);
                                         if (be === 1)
                                             return {
                                                 span: mt,
                                                 minWidth: W,
                                                 height: te
                                             };
-                                        mt.style.height = ie(te), F.push(mt);
+                                        mt.style.height = ae(te), F.push(mt);
                                     }
                                     return {
                                         span: X.makeSpan(["stretchy"], F, s),
                                         minWidth: W,
                                         height: te
                                     };
                                 }
                             }
                             const {
                                 span: f,
                                 minWidth: m,
                                 height: b
                             } = a();
-                            return f.height = b, f.style.height = ie(b), m > 0 && (f.style.minWidth = ie(m)), f;
+                            return f.height = b, f.style.height = ae(b), m > 0 && (f.style.minWidth = ae(m)), f;
                         }
                     };
 
                     function He(i, s) {
                         if (!i || i.type !== s)
                             throw new Error("Expected node of type " + s + ", but got " + (i ? "node of type " + i.type : String(i)));
                         return i;
@@ -13018,39 +13018,39 @@
                                     te = nt(J, s.havingCrampedStyle());
                                 A = ir(te).skew;
                             }
                             const F = f.label === "\\c";
                             let L = F ? b.height + b.depth : Math.min(b.height, s.fontMetrics().xHeight),
                                 j;
                             if (f.isStretchy)
-                                j = a0.svgSpan(f, s), j = X.makeVList({
+                                j = o0.svgSpan(f, s), j = X.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: b
                                     }, {
                                         type: "elem",
                                         elem: j,
                                         wrapperClasses: ["svg-align"],
                                         wrapperStyle: A > 0 ? {
-                                            width: "calc(100% - " + ie(2 * A) + ")",
-                                            marginLeft: ie(2 * A)
+                                            width: "calc(100% - " + ae(2 * A) + ")",
+                                            marginLeft: ae(2 * A)
                                         } : void 0
                                     }]
                                 }, s);
                             else {
                                 let J, te;
                                 f.label === "\\vec" ? (J = X.staticSvg("vec", s), te = X.svgData.vec[1]) : (J = X.makeOrd({
                                     mode: f.mode,
                                     text: f.label
                                 }, s, "textord"), J = ir(J), J.italic = 0, te = J.width, F && (L += J.depth)), j = X.makeSpan(["accent-body"], [J]);
                                 const be = f.label === "\\textcircled";
                                 be && (j.classes.push("accent-full"), L = b.height);
                                 let Te = A;
-                                be || (Te -= te / 2), j.style.left = ie(Te), f.label === "\\textcircled" && (j.style.top = ".2em"), j = X.makeVList({
+                                be || (Te -= te / 2), j.style.left = ae(Te), f.label === "\\textcircled" && (j.style.top = ".2em"), j = X.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: b
                                     }, {
                                         type: "kern",
                                         size: -L
@@ -13060,15 +13060,15 @@
                                     }]
                                 }, s);
                             }
                             const W = X.makeSpan(["mord", "accent"], [j], s);
                             return m ? (m.children[0] = W, m.height = Math.max(W.height, m.height), m.classes[0] = "mord", m) : W;
                         },
                         So = (i, s) => {
-                            const a = i.isStretchy ? a0.mathMLnode(i.label) : new se.MathNode("mo", [An(i.label, i.mode)]),
+                            const a = i.isStretchy ? o0.mathMLnode(i.label) : new se.MathNode("mo", [Sn(i.label, i.mode)]),
                                 f = new se.MathNode("mover", [ft(i.base, s), a]);
                             return f.setAttribute("accent", "true"), f;
                         },
                         Td = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map((i) => "\\" + i).join("|"));
                     _e({
                         type: "accent",
                         names: ["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring", "\\widecheck", "\\widehat", "\\widetilde", "\\overrightarrow", "\\overleftarrow", "\\Overrightarrow", "\\overleftrightarrow", "\\overgroup", "\\overlinesegment", "\\overleftharpoon", "\\overrightharpoon"],
@@ -13131,15 +13131,15 @@
                                 mode: a.mode,
                                 label: f,
                                 base: m
                             };
                         },
                         htmlBuilder: (i, s) => {
                             const a = nt(i.base, s),
-                                f = a0.svgSpan(i, s),
+                                f = o0.svgSpan(i, s),
                                 m = i.label === "\\utilde" ? 0.12 : 0,
                                 b = X.makeVList({
                                     positionType: "top",
                                     positionData: a.height,
                                     children: [{
                                         type: "elem",
                                         elem: f,
@@ -13151,15 +13151,15 @@
                                         type: "elem",
                                         elem: a
                                     }]
                                 }, s);
                             return X.makeSpan(["mord", "accentunder"], [b], s);
                         },
                         mathmlBuilder: (i, s) => {
-                            const a = a0.mathMLnode(i.label),
+                            const a = o0.mathMLnode(i.label),
                                 f = new se.MathNode("munder", [ft(i.base, s), a]);
                             return f.setAttribute("accentunder", "true"), f;
                         }
                     });
                     const Os = (i) => {
                         const s = new se.MathNode("mpadded", i ? [i] : []);
                         return s.setAttribute("width", "+0.6em"), s.setAttribute("lspace", "0.3em"), s;
@@ -13219,15 +13219,15 @@
                             const a = s.style;
                             let f = s.havingStyle(a.sup());
                             const m = X.wrapFragment(nt(i.body, f, s), s),
                                 b = i.label.slice(0, 2) === "\\x" ? "x" : "cd";
                             m.classes.push(b + "-arrow-pad");
                             let w;
                             i.below && (f = s.havingStyle(a.sub()), w = X.wrapFragment(nt(i.below, f, s), s), w.classes.push(b + "-arrow-pad"));
-                            const A = a0.svgSpan(i, s),
+                            const A = o0.svgSpan(i, s),
                                 F = -s.fontMetrics().axisHeight + 0.5 * A.height;
                             let L = -s.fontMetrics().axisHeight - 0.5 * A.height - 0.111;
                             (m.depth > 0.25 || i.label === "\\xleftequilibrium") && (L -= m.depth);
                             let j;
                             if (w) {
                                 const W = -s.fontMetrics().axisHeight + w.height + 0.5 * A.height + 0.111;
                                 j = X.makeVList({
@@ -13258,15 +13258,15 @@
                                         elem: A,
                                         shift: F
                                     }]
                                 }, s);
                             return j.children[0].children[0].children[1].classes.push("svg-align"), X.makeSpan(["mrel", "x-arrow"], [j], s);
                         },
                         mathmlBuilder(i, s) {
-                            const a = a0.mathMLnode(i.label);
+                            const a = o0.mathMLnode(i.label);
                             a.setAttribute("minsize", i.label.charAt(0) === "x" ? "1.75em" : "3.0em");
                             let f;
                             if (i.body) {
                                 const m = Os(ft(i.body, s));
                                 if (i.below) {
                                     const b = Os(ft(i.below, s));
                                     f = new se.MathNode("munderover", [a, b, m]);
@@ -13571,15 +13571,15 @@
                                 side: f.slice(4),
                                 label: s[0]
                             };
                         },
                         htmlBuilder(i, s) {
                             const a = s.havingStyle(s.style.sup()),
                                 f = X.wrapFragment(nt(i.label, a, s), s);
-                            return f.classes.push("cd-label-" + i.side), f.style.bottom = ie(0.8 - f.depth), f.height = 0, f.depth = 0, f;
+                            return f.classes.push("cd-label-" + i.side), f.style.bottom = ae(0.8 - f.depth), f.height = 0, f.depth = 0, f;
                         },
                         mathmlBuilder(i, s) {
                             let a = new se.MathNode("mrow", [ft(i.label, s)]);
                             return a = new se.MathNode("mpadded", [a]), a.setAttribute("width", "0"), i.side === "left" && a.setAttribute("lspace", "-1width"), a.setAttribute("voffset", "0.7em"), a = new se.MathNode("mstyle", [a]), a.setAttribute("displaystyle", "false"), a.setAttribute("scriptlevel", "1"), a;
                         }
                     }), _e({
                         type: "cdlabelparent",
@@ -13712,19 +13712,19 @@
                                 size: m && He(m, "size").value
                             };
                         },
                         // The following builders are called only at the top level,
                         // not within tabular/array environments.
                         htmlBuilder(i, s) {
                             const a = X.makeSpan(["mspace"], [], s);
-                            return i.newLine && (a.classes.push("newline"), i.size && (a.style.marginTop = ie(Ze(i.size, s)))), a;
+                            return i.newLine && (a.classes.push("newline"), i.size && (a.style.marginTop = ae(Ze(i.size, s)))), a;
                         },
                         mathmlBuilder(i, s) {
                             const a = new se.MathNode("mspace");
-                            return i.newLine && (a.setAttribute("linebreak", "newline"), i.size && a.setAttribute("height", ie(Ze(i.size, s)))), a;
+                            return i.newLine && (a.setAttribute("linebreak", "newline"), i.size && a.setAttribute("height", ae(Ze(i.size, s)))), a;
                         }
                     });
                     const ul = {
                             "\\global": "\\global",
                             "\\long": "\\\\globallong",
                             "\\\\globallong": "\\\\globallong",
                             "\\def": "\\gdef",
@@ -13888,15 +13888,15 @@
                                 b = X.makeSpan(f.concat(m.sizingClasses(a)), [i], a),
                                 w = m.sizeMultiplier / a.sizeMultiplier;
                             return b.height *= w, b.depth *= w, b.maxFontSize = m.sizeMultiplier, b;
                         },
                         zo = function(i, s, a) {
                             const f = s.havingBaseStyle(a),
                                 m = (1 - s.sizeMultiplier / f.sizeMultiplier) * s.fontMetrics().axisHeight;
-                            i.classes.push("delimcenter"), i.style.top = ie(m), i.height -= m, i.depth += m;
+                            i.classes.push("delimcenter"), i.style.top = ae(m), i.height -= m, i.depth += m;
                         },
                         Rd = function(i, s, a, f, m, b) {
                             const w = X.makeSymbol(i, "Main-Regular", m, f),
                                 A = cl(w, s, f, b);
                             return a && zo(A, f, s), A;
                         },
                         Od = function(i, s, a, f) {
@@ -13912,25 +13912,25 @@
                             return s === "Size1-Regular" ? f = "delim-size1" : f = "delim-size4", {
                                 type: "elem",
                                 elem: X.makeSpan(["delimsizinginner", f], [X.makeSpan([], [X.makeSymbol(i, s, a)])])
                             };
                         },
                         hl = function(i, s, a) {
                             const f = Ct["Size4-Regular"][i.charCodeAt(0)] ? Ct["Size4-Regular"][i.charCodeAt(0)][4] : Ct["Size1-Regular"][i.charCodeAt(0)][4],
-                                m = new dn("inner", Bn(i, Math.round(1e3 * s))),
+                                m = new dn("inner", Nn(i, Math.round(1e3 * s))),
                                 b = new en([m], {
-                                    width: ie(f),
-                                    height: ie(s),
+                                    width: ae(f),
+                                    height: ae(s),
                                     // Override CSS rule `.katex svg { width: 100% }`
-                                    style: "width:" + ie(f),
+                                    style: "width:" + ae(f),
                                     viewBox: "0 0 " + 1e3 * f + " " + Math.round(1e3 * s),
                                     preserveAspectRatio: "xMinYMin"
                                 }),
                                 w = X.makeSvgSpan([], [b], a);
-                            return w.height = s, w.style.height = ie(s), w.style.width = ie(f), {
+                            return w.height = s, w.style.height = ae(s), w.style.width = ae(f), {
                                 type: "elem",
                                 elem: w
                             };
                         },
                         dl = 8e-3,
                         Ls = {
                             type: "kern",
@@ -13954,42 +13954,42 @@
                                 mt = 1;
                             if (A !== null) {
                                 const Mt = qr(A, J, m);
                                 lt = Mt.height + Mt.depth, mt = 2;
                             }
                             const tn = be + Ke + lt,
                                 Pt = Math.max(0, Math.ceil((s - tn) / (mt * Je))),
-                                En = tn + Pt * mt * Je;
+                                xn = tn + Pt * mt * Je;
                             let cr = f.fontMetrics().axisHeight;
                             a && (cr *= f.sizeMultiplier);
-                            const rt = En / 2 - cr,
+                            const rt = xn / 2 - cr,
                                 ot = [];
                             if (j.length > 0) {
-                                const Mt = En - be - Ke,
-                                    xt = Math.round(En * 1e3),
-                                    xn = $t(j, Math.round(Mt * 1e3)),
-                                    c4 = new dn(j, xn),
+                                const Mt = xn - be - Ke,
+                                    xt = Math.round(xn * 1e3),
+                                    Tn = $t(j, Math.round(Mt * 1e3)),
+                                    c4 = new dn(j, Tn),
                                     Eu = (W / 1e3).toFixed(3) + "em",
                                     xu = (xt / 1e3).toFixed(3) + "em",
                                     f4 = new en([c4], {
                                         width: Eu,
                                         height: xu,
                                         viewBox: "0 0 " + W + " " + xt
                                     }),
                                     Gs = X.makeSvgSpan([], [f4], f);
                                 Gs.height = xt / 1e3, Gs.style.width = Eu, Gs.style.height = xu, ot.push({
                                     type: "elem",
                                     elem: Gs
                                 });
                             } else {
                                 if (ot.push(fl(L, J, m)), ot.push(Ls), A === null) {
-                                    const Mt = En - be - Ke + 2 * dl;
+                                    const Mt = xn - be - Ke + 2 * dl;
                                     ot.push(hl(F, Mt, f));
                                 } else {
-                                    const Mt = (En - be - Ke - lt) / 2 + 2 * dl;
+                                    const Mt = (xn - be - Ke - lt) / 2 + 2 * dl;
                                     ot.push(hl(F, Mt, f)), ot.push(Ls), ot.push(fl(A, J, m)), ot.push(Ls), ot.push(hl(F, Mt, f));
                                 }
                                 ot.push(Ls), ot.push(fl(w, J, m));
                             }
                             const gt = f.havingBaseStyle(Q.TEXT),
                                 yt = X.makeVList({
                                     positionType: "bottom",
@@ -14002,30 +14002,30 @@
                         pl = 0.08,
                         gl = function(i, s, a, f, m) {
                             const b = zt(i, f, a),
                                 w = new dn(i, b),
                                 A = new en([w], {
                                     // Note: 1000:1 ratio of viewBox to document em width.
                                     width: "400em",
-                                    height: ie(s),
+                                    height: ae(s),
                                     viewBox: "0 0 400000 " + a,
                                     preserveAspectRatio: "xMinYMin slice"
                                 });
                             return X.makeSvgSpan(["hide-tail"], [A], m);
                         },
                         Hd = function(i, s) {
                             const a = s.havingBaseSizing(),
                                 f = Po("\\surd", i * a.sizeMultiplier, Ho, a);
                             let m = a.sizeMultiplier;
                             const b = Math.max(0, s.minRuleThickness - s.fontMetrics().sqrtRuleThickness);
                             let w, A = 0,
                                 F = 0,
                                 L = 0,
                                 j;
-                            return f.type === "small" ? (L = 1e3 + 1e3 * b + ml, i < 1 ? m = 1 : i < 1.4 && (m = 0.7), A = (1 + b + pl) / m, F = (1 + b) / m, w = gl("sqrtMain", A, L, b, s), w.style.minWidth = "0.853em", j = 0.833 / m) : f.type === "large" ? (L = (1e3 + ml) * Ur[f.size], F = (Ur[f.size] + b) / m, A = (Ur[f.size] + b + pl) / m, w = gl("sqrtSize" + f.size, A, L, b, s), w.style.minWidth = "1.02em", j = 1 / m) : (A = i + b + pl, F = i + b, L = Math.floor(1e3 * i + b) + ml, w = gl("sqrtTall", A, L, b, s), w.style.minWidth = "0.742em", j = 1.056), w.height = F, w.style.height = ie(A), {
+                            return f.type === "small" ? (L = 1e3 + 1e3 * b + ml, i < 1 ? m = 1 : i < 1.4 && (m = 0.7), A = (1 + b + pl) / m, F = (1 + b) / m, w = gl("sqrtMain", A, L, b, s), w.style.minWidth = "0.853em", j = 0.833 / m) : f.type === "large" ? (L = (1e3 + ml) * Ur[f.size], F = (Ur[f.size] + b) / m, A = (Ur[f.size] + b + pl) / m, w = gl("sqrtSize" + f.size, A, L, b, s), w.style.minWidth = "1.02em", j = 1 / m) : (A = i + b + pl, F = i + b, L = Math.floor(1e3 * i + b) + ml, w = gl("sqrtTall", A, L, b, s), w.style.minWidth = "0.742em", j = 1.056), w.height = F, w.style.height = ae(A), {
                                 span: w,
                                 advanceWidth: j,
                                 // Calculate the actual line width.
                                 // This actually should depend on the chosen font -- e.g. \boldmath
                                 // should use the thicker surd symbols from e.g. KaTeX_Main-Bold, and
                                 // have thicker rules.
                                 ruleWidth: (s.fontMetrics().sqrtRuleThickness + b) * m
@@ -14126,15 +14126,15 @@
                         qo = function(i, s, a, f, m, b) {
                             i === "<" || i === "\\lt" || i === "⟨" ? i = "\\langle" : (i === ">" || i === "\\gt" || i === "⟩") && (i = "\\rangle");
                             let w;
                             M.contains(Lo, i) ? w = Ud : M.contains(Io, i) ? w = Ho : w = Gd;
                             const A = Po(i, s, w, f);
                             return A.type === "small" ? Rd(i, A.style, a, f, m, b) : A.type === "large" ? Ro(i, A.size, a, f, m, b) : Oo(i, s, a, f, m, b);
                         };
-                    var o0 = {
+                    var u0 = {
                         sqrtImage: Hd,
                         sizedDelim: qd,
                         sizeToMaxHeight: Ur,
                         customSizedDelim: qo,
                         leftRightDelim: function(i, s, a, f, m, b) {
                             const w = f.fontMetrics().axisHeight * f.sizeMultiplier,
                                 A = 901,
@@ -14243,21 +14243,21 @@
                                 type: "delimsizing",
                                 mode: i.parser.mode,
                                 size: Uo[i.funcName].size,
                                 mclass: Uo[i.funcName].mclass,
                                 delim: a.text
                             };
                         },
-                        htmlBuilder: (i, s) => i.delim === "." ? X.makeSpan([i.mclass]) : o0.sizedDelim(i.delim, i.size, s, i.mode, [i.mclass]),
+                        htmlBuilder: (i, s) => i.delim === "." ? X.makeSpan([i.mclass]) : u0.sizedDelim(i.delim, i.size, s, i.mode, [i.mclass]),
                         mathmlBuilder: (i) => {
                             const s = [];
-                            i.delim !== "." && s.push(An(i.delim, i.mode));
+                            i.delim !== "." && s.push(Sn(i.delim, i.mode));
                             const a = new se.MathNode("mo", s);
                             i.mclass === "mopen" || i.mclass === "mclose" ? a.setAttribute("fence", "true") : a.setAttribute("fence", "false"), a.setAttribute("stretchy", "true");
-                            const f = ie(o0.sizeToMaxHeight[i.size]);
+                            const f = ae(u0.sizeToMaxHeight[i.size]);
                             return a.setAttribute("minsize", f), a.setAttribute("maxsize", f), a;
                         }
                     });
 
                     function Go(i) {
                         if (!i.body)
                             throw new Error("Bug: The leftright ParseNode wasn't fully parsed.");
@@ -14310,37 +14310,37 @@
                             let f = 0,
                                 m = 0,
                                 b = !1;
                             for (let F = 0; F < a.length; F++)
                                 a[F].isMiddle ? b = !0 : (f = Math.max(a[F].height, f), m = Math.max(a[F].depth, m));
                             f *= s.sizeMultiplier, m *= s.sizeMultiplier;
                             let w;
-                            if (i.left === "." ? w = Hr(s, ["mopen"]) : w = o0.leftRightDelim(i.left, f, m, s, i.mode, ["mopen"]), a.unshift(w), b)
+                            if (i.left === "." ? w = Hr(s, ["mopen"]) : w = u0.leftRightDelim(i.left, f, m, s, i.mode, ["mopen"]), a.unshift(w), b)
                                 for (let F = 1; F < a.length; F++) {
                                     const j = a[F].isMiddle;
-                                    j && (a[F] = o0.leftRightDelim(j.delim, f, m, j.options, i.mode, []));
+                                    j && (a[F] = u0.leftRightDelim(j.delim, f, m, j.options, i.mode, []));
                                 }
                             let A;
                             if (i.right === ".")
                                 A = Hr(s, ["mclose"]);
                             else {
                                 const F = i.rightColor ? s.withColor(i.rightColor) : s;
-                                A = o0.leftRightDelim(i.right, f, m, F, i.mode, ["mclose"]);
+                                A = u0.leftRightDelim(i.right, f, m, F, i.mode, ["mclose"]);
                             }
                             return a.push(A), X.makeSpan(["minner"], a, s);
                         },
                         mathmlBuilder: (i, s) => {
                             Go(i);
                             const a = ln(i.body, s);
                             if (i.left !== ".") {
-                                const f = new se.MathNode("mo", [An(i.left, i.mode)]);
+                                const f = new se.MathNode("mo", [Sn(i.left, i.mode)]);
                                 f.setAttribute("fence", "true"), a.unshift(f);
                             }
                             if (i.right !== ".") {
-                                const f = new se.MathNode("mo", [An(i.right, i.mode)]);
+                                const f = new se.MathNode("mo", [Sn(i.right, i.mode)]);
                                 f.setAttribute("fence", "true"), i.rightColor && f.setAttribute("mathcolor", i.rightColor), a.push(f);
                             }
                             return il(a);
                         }
                     }), _e({
                         type: "middle",
                         names: ["\\middle"],
@@ -14359,25 +14359,25 @@
                             };
                         },
                         htmlBuilder: (i, s) => {
                             let a;
                             if (i.delim === ".")
                                 a = Hr(s, []);
                             else {
-                                a = o0.sizedDelim(i.delim, 1, s, i.mode, []);
+                                a = u0.sizedDelim(i.delim, 1, s, i.mode, []);
                                 const f = {
                                     delim: i.delim,
                                     options: s
                                 };
                                 a.isMiddle = f;
                             }
                             return a;
                         },
                         mathmlBuilder: (i, s) => {
-                            const a = i.delim === "\\vert" || i.delim === "|" ? An("|", "text") : An(i.delim, i.mode),
+                            const a = i.delim === "\\vert" || i.delim === "|" ? Sn("|", "text") : Sn(i.delim, i.mode),
                                 f = new se.MathNode("mo", [a]);
                             return f.setAttribute("fence", "true"), f.setAttribute("lspace", "0.05em"), f.setAttribute("rspace", "0.05em"), f;
                         }
                     });
                     const _l = (i, s) => {
                             const a = X.wrapFragment(nt(i.body, s), s),
                                 f = i.label.slice(1);
@@ -14394,35 +14394,35 @@
                                     j = Ze({
                                         number: 0.35,
                                         unit: "ex"
                                     }, s),
                                     W = s.havingBaseSizing();
                                 m = m / W.sizeMultiplier;
                                 const J = a.height + a.depth + L + j;
-                                a.style.paddingLeft = ie(J / 2 + L);
+                                a.style.paddingLeft = ae(J / 2 + L);
                                 const te = Math.floor(1e3 * J * m),
                                     be = Xe(te),
                                     Te = new en([new dn("phase", be)], {
                                         width: "400em",
-                                        height: ie(te / 1e3),
+                                        height: ae(te / 1e3),
                                         viewBox: "0 0 400000 " + te,
                                         preserveAspectRatio: "xMinYMin slice"
                                     });
-                                b = X.makeSvgSpan(["hide-tail"], [Te], s), b.style.height = ie(J), w = a.depth + L + j;
+                                b = X.makeSvgSpan(["hide-tail"], [Te], s), b.style.height = ae(J), w = a.depth + L + j;
                             } else {
                                 /cancel/.test(f) ? A || a.classes.push("cancel-pad") : f === "angl" ? a.classes.push("anglpad") : a.classes.push("boxpad");
                                 let L = 0,
                                     j = 0,
                                     W = 0;
                                 /box/.test(f) ? (W = Math.max(
                                     s.fontMetrics().fboxrule,
                                     // default
                                     s.minRuleThickness
                                     // User override.
-                                ), L = s.fontMetrics().fboxsep + (f === "colorbox" ? 0 : W), j = L) : f === "angl" ? (W = Math.max(s.fontMetrics().defaultRuleThickness, s.minRuleThickness), L = 4 * W, j = Math.max(0, 0.25 - a.depth)) : (L = A ? 0.2 : 0, j = L), b = a0.encloseSpan(a, f, L, j, s), /fbox|boxed|fcolorbox/.test(f) ? (b.style.borderStyle = "solid", b.style.borderWidth = ie(W)) : f === "angl" && W !== 0.049 && (b.style.borderTopWidth = ie(W), b.style.borderRightWidth = ie(W)), w = a.depth + j, i.backgroundColor && (b.style.backgroundColor = i.backgroundColor, i.borderColor && (b.style.borderColor = i.borderColor));
+                                ), L = s.fontMetrics().fboxsep + (f === "colorbox" ? 0 : W), j = L) : f === "angl" ? (W = Math.max(s.fontMetrics().defaultRuleThickness, s.minRuleThickness), L = 4 * W, j = Math.max(0, 0.25 - a.depth)) : (L = A ? 0.2 : 0, j = L), b = o0.encloseSpan(a, f, L, j, s), /fbox|boxed|fcolorbox/.test(f) ? (b.style.borderStyle = "solid", b.style.borderWidth = ae(W)) : f === "angl" && W !== 0.049 && (b.style.borderTopWidth = ae(W), b.style.borderRightWidth = ae(W)), w = a.depth + j, i.backgroundColor && (b.style.backgroundColor = i.backgroundColor, i.borderColor && (b.style.borderColor = i.borderColor));
                             }
                             let F;
                             if (i.backgroundColor)
                                 F = X.makeVList({
                                     positionType: "individualShift",
                                     children: [
                                         // Put the color background behind inner;
@@ -14653,26 +14653,26 @@
                          *   and their lexers match.
                          * - Otherwise, returns null.
                          */
                         static range(s, a) {
                             return a ? !s || !s.loc || !a.loc || s.loc.lexer !== a.loc.lexer ? null : new mn(s.loc.lexer, s.loc.start, a.loc.end) : s && s.loc;
                         }
                     }
-                    class Sn {
+                    class En {
                         // don't expand the token
                         // used in \noexpand
                         constructor(s, a) {
                             this.text = void 0, this.loc = void 0, this.noexpand = void 0, this.treatAsRelax = void 0, this.text = s, this.loc = a;
                         }
                         /**
                          * Given a pair of tokens (this and endToken), compute a `Token` encompassing
                          * the whole input range enclosed by these two.
                          */
                         range(s, a) {
-                            return new Sn(a, mn.range(this, s));
+                            return new En(a, mn.range(this, s));
                         }
                     }
 
                     function Wo(i) {
                         const s = [];
                         i.consumeSpaces();
                         let a = i.fetch().text;
@@ -14686,15 +14686,15 @@
                     };
 
                     function wl(i) {
                         if (i.indexOf("ed") === -1)
                             return i.indexOf("*") === -1;
                     }
 
-                    function _0(i, s, a) {
+                    function b0(i, s, a) {
                         let {
                             hskipBeforeAndAfter: f,
                             addJot: m,
                             cols: b,
                             arraystretch: w,
                             colSeparationType: A,
                             autoTag: F,
@@ -14718,15 +14718,15 @@
                             Ge = F != null ? [] : void 0;
 
                         function Ke() {
                             F && i.gullet.macros.set("\\@eqnsw", "1", !0);
                         }
 
                         function lt() {
-                            Ge && (i.gullet.macros.get("\\df@tag") ? (Ge.push(i.subparse([new Sn("\\df@tag")])), i.gullet.macros.set("\\df@tag", void 0, !0)) : Ge.push(!!F && i.gullet.macros.get("\\@eqnsw") === "1"));
+                            Ge && (i.gullet.macros.get("\\df@tag") ? (Ge.push(i.subparse([new En("\\df@tag")])), i.gullet.macros.set("\\df@tag", void 0, !0)) : Ge.push(!!F && i.gullet.macros.get("\\@eqnsw") === "1"));
                         }
                         for (Ke(), Je.push(Wo(i));;) {
                             let mt = i.parseExpression(!1, L ? "\\end" : "\\\\");
                             i.gullet.endGroup(), i.gullet.beginGroup(), mt = {
                                 type: "ordgroup",
                                 mode: i.mode,
                                 body: mt
@@ -14809,79 +14809,79 @@
                             for (Ke(b[0]), a = 0; a < i.body.length; ++a) {
                                 const rt = i.body[a];
                                 let ot = Te,
                                     gt = Je;
                                 w < rt.length && (w = rt.length);
                                 const yt = new Array(rt.length);
                                 for (f = 0; f < rt.length; ++f) {
-                                    const xn = nt(rt[f], s);
-                                    gt < xn.depth && (gt = xn.depth), ot < xn.height && (ot = xn.height), yt[f] = xn;
+                                    const Tn = nt(rt[f], s);
+                                    gt < Tn.depth && (gt = Tn.depth), ot < Tn.height && (ot = Tn.height), yt[f] = Tn;
                                 }
                                 const Mt = i.rowGaps[a];
                                 let xt = 0;
                                 Mt && (xt = Ze(Mt, s), xt > 0 && (xt += Je, gt < xt && (gt = xt), xt = 0)), i.addJot && (gt += te), yt.height = ot, yt.depth = gt, Ge += ot, yt.pos = Ge, Ge += gt + xt, A[a] = yt, Ke(b[a + 1]);
                             }
                             const lt = Ge / 2 + s.fontMetrics().axisHeight,
                                 mt = i.cols || [],
                                 tn = [];
-                            let Pt, En;
+                            let Pt, xn;
                             const cr = [];
                             if (i.tags && i.tags.some((rt) => rt))
                                 for (a = 0; a < m; ++a) {
                                     const rt = A[a],
                                         ot = rt.pos - lt,
                                         gt = i.tags[a];
                                     let yt;
                                     gt === !0 ? yt = X.makeSpan(["eqn-num"], [], s) : gt === !1 ? yt = X.makeSpan([], [], s) : yt = X.makeSpan([], Ht(gt, s, !0), s), yt.depth = rt.depth, yt.height = rt.height, cr.push({
                                         type: "elem",
                                         elem: yt,
                                         shift: ot
                                     });
                                 }
                             for (
-                                f = 0, En = 0;
+                                f = 0, xn = 0;
                                 // Continue while either there are more columns or more column
                                 // descriptions, so trailing separators don't get lost.
-                                f < w || En < mt.length;
-                                ++f, ++En
+                                f < w || xn < mt.length;
+                                ++f, ++xn
                             ) {
-                                let rt = mt[En] || {},
+                                let rt = mt[xn] || {},
                                     ot = !0;
                                 for (; rt.type === "separator";) {
-                                    if (ot || (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ie(s.fontMetrics().doubleRuleSep), tn.push(Pt)), rt.separator === "|" || rt.separator === ":") {
+                                    if (ot || (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ae(s.fontMetrics().doubleRuleSep), tn.push(Pt)), rt.separator === "|" || rt.separator === ":") {
                                         const Mt = rt.separator === "|" ? "solid" : "dashed",
                                             xt = X.makeSpan(["vertical-separator"], [], s);
-                                        xt.style.height = ie(Ge), xt.style.borderRightWidth = ie(L), xt.style.borderRightStyle = Mt, xt.style.margin = "0 " + ie(-L / 2);
-                                        const xn = Ge - lt;
-                                        xn && (xt.style.verticalAlign = ie(-xn)), tn.push(xt);
+                                        xt.style.height = ae(Ge), xt.style.borderRightWidth = ae(L), xt.style.borderRightStyle = Mt, xt.style.margin = "0 " + ae(-L / 2);
+                                        const Tn = Ge - lt;
+                                        Tn && (xt.style.verticalAlign = ae(-Tn)), tn.push(xt);
                                     } else
                                         throw new o("Invalid separator type: " + rt.separator);
-                                    En++, rt = mt[En] || {}, ot = !1;
+                                    xn++, rt = mt[xn] || {}, ot = !1;
                                 }
                                 if (f >= w)
                                     continue;
                                 let gt;
-                                (f > 0 || i.hskipBeforeAndAfter) && (gt = M.deflt(rt.pregap, W), gt !== 0 && (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ie(gt), tn.push(Pt)));
+                                (f > 0 || i.hskipBeforeAndAfter) && (gt = M.deflt(rt.pregap, W), gt !== 0 && (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ae(gt), tn.push(Pt)));
                                 let yt = [];
                                 for (a = 0; a < m; ++a) {
                                     const Mt = A[a],
                                         xt = Mt[f];
                                     if (!xt)
                                         continue;
-                                    const xn = Mt.pos - lt;
+                                    const Tn = Mt.pos - lt;
                                     xt.depth = Mt.depth, xt.height = Mt.height, yt.push({
                                         type: "elem",
                                         elem: xt,
-                                        shift: xn
+                                        shift: Tn
                                     });
                                 }
                                 yt = X.makeVList({
                                     positionType: "individualShift",
                                     children: yt
-                                }, s), yt = X.makeSpan(["col-align-" + (rt.align || "c")], [yt]), tn.push(yt), (f < w - 1 || i.hskipBeforeAndAfter) && (gt = M.deflt(rt.postgap, W), gt !== 0 && (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ie(gt), tn.push(Pt)));
+                                }, s), yt = X.makeSpan(["col-align-" + (rt.align || "c")], [yt]), tn.push(yt), (f < w - 1 || i.hskipBeforeAndAfter) && (gt = M.deflt(rt.postgap, W), gt !== 0 && (Pt = X.makeSpan(["arraycolsep"], []), Pt.style.width = ae(gt), tn.push(Pt)));
                             }
                             if (A = X.makeSpan(["mtable"], tn), F.length > 0) {
                                 const rt = X.makeLineSpan("hline", s, L),
                                     ot = X.makeLineSpan("hdashline", s, L),
                                     gt = [{
                                         type: "elem",
                                         elem: A,
@@ -14929,15 +14929,15 @@
                                     te = [];
                                 for (let be = 0; be < J.length; be++)
                                     te.push(new se.MathNode("mtd", [ft(J[be], s)]));
                                 i.tags && i.tags[W] && (te.unshift(f), te.push(f), i.leqno ? te.unshift(m) : te.push(m)), a.push(new se.MathNode("mtr", te));
                             }
                             let b = new se.MathNode("mtable", a);
                             const w = i.arraystretch === 0.5 ? 0.1 : 0.16 + i.arraystretch - 1 + (i.addJot ? 0.09 : 0);
-                            b.setAttribute("rowspacing", ie(w));
+                            b.setAttribute("rowspacing", ae(w));
                             let A = "",
                                 F = "";
                             if (i.cols && i.cols.length > 0) {
                                 const W = i.cols;
                                 let J = "",
                                     te = !1,
                                     be = 0,
@@ -14963,15 +14963,15 @@
                             return /[sd]/.test(L) && b.setAttribute("rowlines", L.trim()), A !== "" && (b = new se.MathNode("menclose", [b]), b.setAttribute("notation", A.trim())), i.arraystretch && i.arraystretch < 1 && (b = new se.MathNode("mstyle", [b]), b.setAttribute("scriptlevel", "1")), b;
                         },
                         Xo = function(i, s) {
                             i.envName.indexOf("ed") === -1 && Ps(i);
                             const a = [],
                                 f = i.envName.indexOf("at") > -1 ? "alignat" : "align",
                                 m = i.envName === "split",
-                                b = _0(i.parser, {
+                                b = b0(i.parser, {
                                     cols: a,
                                     addJot: !0,
                                     autoTag: m ? void 0 : wl(i.envName),
                                     emptySingleRow: !0,
                                     colSeparationType: f,
                                     maxNumCols: m ? 2 : void 0,
                                     leqno: i.parser.settings.leqno
@@ -15044,15 +15044,15 @@
                                 }),
                                 b = {
                                     cols: m,
                                     hskipBeforeAndAfter: !0,
                                     // \@preamble in lttab.dtx
                                     maxNumCols: m.length
                                 };
-                            return _0(i.parser, b, yl(i.envName));
+                            return b0(i.parser, b, yl(i.envName));
                         },
                         htmlBuilder: Vn,
                         mathmlBuilder: Wn
                     }), jn({
                         type: "array",
                         names: ["matrix", "pmatrix", "bmatrix", "Bmatrix", "vmatrix", "Vmatrix", "matrix*", "pmatrix*", "bmatrix*", "Bmatrix*", "vmatrix*", "Vmatrix*"],
                         props: {
@@ -15082,15 +15082,15 @@
                                         throw new o("Expected l or c or r", w.nextToken);
                                     w.consume(), w.consumeSpaces(), w.expect("]"), w.consume(), f.cols = [{
                                         type: "align",
                                         align: a
                                     }];
                                 }
                             }
-                            const m = _0(i.parser, f, yl(i.envName)),
+                            const m = b0(i.parser, f, yl(i.envName)),
                                 b = Math.max(0, ...m.body.map((w) => w.length));
                             return m.cols = new Array(b).fill({
                                 type: "align",
                                 align: a
                             }), s ? {
                                 type: "leftright",
                                 mode: i.mode,
@@ -15109,15 +15109,15 @@
                         props: {
                             numArgs: 0
                         },
                         handler(i) {
                             const s = {
                                     arraystretch: 0.5
                                 },
-                                a = _0(i.parser, s, "script");
+                                a = b0(i.parser, s, "script");
                             return a.colSeparationType = "small", a;
                         },
                         htmlBuilder: Vn,
                         mathmlBuilder: Wn
                     }), jn({
                         type: "array",
                         names: ["subarray"],
@@ -15137,15 +15137,15 @@
                             if (m.length > 1)
                                 throw new o("{subarray} can contain only one column");
                             let b = {
                                 cols: m,
                                 hskipBeforeAndAfter: !1,
                                 arraystretch: 0.5
                             };
-                            if (b = _0(i.parser, b, "script"), b.body.length > 0 && b.body[0].length > 1)
+                            if (b = b0(i.parser, b, "script"), b.body.length > 0 && b.body[0].length > 1)
                                 throw new o("{subarray} can contain only one column");
                             return b;
                         },
                         htmlBuilder: Vn,
                         mathmlBuilder: Wn
                     }), jn({
                         type: "array",
@@ -15169,15 +15169,15 @@
                                     }, {
                                         type: "align",
                                         align: "l",
                                         pregap: 0,
                                         postgap: 0
                                     }]
                                 },
-                                a = _0(i.parser, s, yl(i.envName));
+                                a = b0(i.parser, s, yl(i.envName));
                             return {
                                 type: "leftright",
                                 mode: i.mode,
                                 body: [a],
                                 left: i.envName.indexOf("r") > -1 ? "." : "\\{",
                                 right: i.envName.indexOf("r") > -1 ? "\\}" : ".",
                                 rightColor: void 0
@@ -15209,15 +15209,15 @@
                                 }],
                                 addJot: !0,
                                 colSeparationType: "gather",
                                 autoTag: wl(i.envName),
                                 emptySingleRow: !0,
                                 leqno: i.parser.settings.leqno
                             };
-                            return _0(i.parser, s, "display");
+                            return b0(i.parser, s, "display");
                         },
                         htmlBuilder: Vn,
                         mathmlBuilder: Wn
                     }), jn({
                         type: "array",
                         names: ["alignat", "alignat*", "alignedat"],
                         props: {
@@ -15237,15 +15237,15 @@
                             const s = {
                                 autoTag: wl(i.envName),
                                 emptySingleRow: !0,
                                 singleRow: !0,
                                 maxNumCols: 1,
                                 leqno: i.parser.settings.leqno
                             };
-                            return _0(i.parser, s, "display");
+                            return b0(i.parser, s, "display");
                         },
                         htmlBuilder: Vn,
                         mathmlBuilder: Wn
                     }), jn({
                         type: "array",
                         names: ["CD"],
                         props: {
@@ -15486,23 +15486,23 @@
                                     }]
                                 }, s);
                             }
                             b = s.havingStyle(a), be.height *= b.sizeMultiplier / s.sizeMultiplier, be.depth *= b.sizeMultiplier / s.sizeMultiplier;
                             let Te;
                             a.size === Q.DISPLAY.size ? Te = s.fontMetrics().delim1 : a.size === Q.SCRIPTSCRIPT.size ? Te = s.havingStyle(Q.SCRIPT).fontMetrics().delim2 : Te = s.fontMetrics().delim2;
                             let Je, Ge;
-                            return i.leftDelim == null ? Je = Hr(s, ["mopen"]) : Je = o0.customSizedDelim(i.leftDelim, Te, !0, s.havingStyle(a), i.mode, ["mopen"]), i.continued ? Ge = X.makeSpan([]) : i.rightDelim == null ? Ge = Hr(s, ["mclose"]) : Ge = o0.customSizedDelim(i.rightDelim, Te, !0, s.havingStyle(a), i.mode, ["mclose"]), X.makeSpan(["mord"].concat(b.sizingClasses(s)), [Je, X.makeSpan(["mfrac"], [be]), Ge], s);
+                            return i.leftDelim == null ? Je = Hr(s, ["mopen"]) : Je = u0.customSizedDelim(i.leftDelim, Te, !0, s.havingStyle(a), i.mode, ["mopen"]), i.continued ? Ge = X.makeSpan([]) : i.rightDelim == null ? Ge = Hr(s, ["mclose"]) : Ge = u0.customSizedDelim(i.rightDelim, Te, !0, s.havingStyle(a), i.mode, ["mclose"]), X.makeSpan(["mord"].concat(b.sizingClasses(s)), [Je, X.makeSpan(["mfrac"], [be]), Ge], s);
                         },
                         kl = (i, s) => {
                             let a = new se.MathNode("mfrac", [ft(i.numer, s), ft(i.denom, s)]);
                             if (!i.hasBarLine)
                                 a.setAttribute("linethickness", "0px");
                             else if (i.barSize) {
                                 const m = Ze(i.barSize, s);
-                                a.setAttribute("linethickness", ie(m));
+                                a.setAttribute("linethickness", ae(m));
                             }
                             const f = Ko(i.size, s.style);
                             if (f.size !== s.style.size) {
                                 a = new se.MathNode("mstyle", [a]);
                                 const m = f.size === Q.DISPLAY.size ? "true" : "false";
                                 a.setAttribute("displaystyle", m), a.setAttribute("scriptlevel", "0");
                             }
@@ -15768,15 +15768,15 @@
                         mathmlBuilder: kl
                     });
                     const tu = (i, s) => {
                         const a = s.style;
                         let f, m;
                         i.type === "supsub" ? (f = i.sup ? nt(i.sup, s.havingStyle(a.sup()), s) : nt(i.sub, s.havingStyle(a.sub()), s), m = He(i.base, "horizBrace")) : m = He(i, "horizBrace");
                         const b = nt(m.base, s.havingBaseStyle(Q.DISPLAY)),
-                            w = a0.svgSpan(m, s);
+                            w = o0.svgSpan(m, s);
                         let A;
                         if (m.isOver ? (A = X.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: b
                                 }, {
@@ -15847,15 +15847,15 @@
                                 label: f,
                                 isOver: /^\\over/.test(f),
                                 base: s[0]
                             };
                         },
                         htmlBuilder: tu,
                         mathmlBuilder: (i, s) => {
-                            const a = a0.mathMLnode(i.label);
+                            const a = o0.mathMLnode(i.label);
                             return new se.MathNode(i.isOver ? "mover" : "munder", [ft(i.base, s), a]);
                         }
                     }), _e({
                         type: "href",
                         names: ["\\href"],
                         props: {
                             numArgs: 2,
@@ -15879,16 +15879,16 @@
                             } : a.formatUnsupportedCmd("\\href");
                         },
                         htmlBuilder: (i, s) => {
                             const a = Ht(i.body, s, !1);
                             return X.makeAnchor(i.href, [], a, s);
                         },
                         mathmlBuilder: (i, s) => {
-                            let a = g0(i.body, s);
-                            return a instanceof Dn || (a = new Dn("mrow", [a])), a.setAttribute("href", i.href), a;
+                            let a = _0(i.body, s);
+                            return a instanceof An || (a = new An("mrow", [a])), a.setAttribute("href", i.href), a;
                         }
                     }), _e({
                         type: "href",
                         names: ["\\url"],
                         props: {
                             numArgs: 1,
                             argTypes: ["url"],
@@ -16019,15 +16019,15 @@
                                 f = ["enclosing"];
                             i.attributes.class && f.push(...i.attributes.class.trim().split(/\s+/));
                             const m = X.makeSpan(f, a, s);
                             for (const b in i.attributes)
                                 b !== "class" && i.attributes.hasOwnProperty(b) && m.setAttribute(b, i.attributes[b]);
                             return m;
                         },
-                        mathmlBuilder: (i, s) => g0(i.body, s)
+                        mathmlBuilder: (i, s) => _0(i.body, s)
                     }), _e({
                         type: "htmlmathml",
                         names: ["\\html@mathml"],
                         props: {
                             numArgs: 2,
                             allowedInText: !0
                         },
@@ -16042,15 +16042,15 @@
                                 mathml: Nt(s[1])
                             };
                         },
                         htmlBuilder: (i, s) => {
                             const a = Ht(i.html, s, !1);
                             return X.makeFragment(a);
                         },
-                        mathmlBuilder: (i, s) => g0(i.mathml, s)
+                        mathmlBuilder: (i, s) => _0(i.mathml, s)
                     });
                     const Dl = function(i) {
                         if (/^[-+]? *(\d+(\.\d*)?|\.\d+)$/.test(i))
                             return {
                                 number: +i,
                                 unit: "bp"
                             };
@@ -16132,28 +16132,28 @@
                         htmlBuilder: (i, s) => {
                             const a = Ze(i.height, s);
                             let f = 0;
                             i.totalheight.number > 0 && (f = Ze(i.totalheight, s) - a);
                             let m = 0;
                             i.width.number > 0 && (m = Ze(i.width, s));
                             const b = {
-                                height: ie(a + f)
+                                height: ae(a + f)
                             };
-                            m > 0 && (b.width = ie(m)), f > 0 && (b.verticalAlign = ie(-f));
+                            m > 0 && (b.width = ae(m)), f > 0 && (b.verticalAlign = ae(-f));
                             const w = new qn(i.src, i.alt, b);
                             return w.height = a, w.depth = f, w;
                         },
                         mathmlBuilder: (i, s) => {
                             const a = new se.MathNode("mglyph", []);
                             a.setAttribute("alt", i.alt);
                             const f = Ze(i.height, s);
                             let m = 0;
-                            if (i.totalheight.number > 0 && (m = Ze(i.totalheight, s) - f, a.setAttribute("valign", ie(-m))), a.setAttribute("height", ie(f + m)), i.width.number > 0) {
+                            if (i.totalheight.number > 0 && (m = Ze(i.totalheight, s) - f, a.setAttribute("valign", ae(-m))), a.setAttribute("height", ae(f + m)), i.width.number > 0) {
                                 const b = Ze(i.width, s);
-                                a.setAttribute("width", ie(b));
+                                a.setAttribute("width", ae(b));
                             }
                             return a.setAttribute("src", i.src), a;
                         }
                     }), _e({
                         type: "kern",
                         names: ["\\kern", "\\mkern", "\\hskip", "\\mskip"],
                         props: {
@@ -16208,15 +16208,15 @@
                         },
                         htmlBuilder: (i, s) => {
                             let a;
                             i.alignment === "clap" ? (a = X.makeSpan([], [nt(i.body, s)]), a = X.makeSpan(["inner"], [a], s)) : a = X.makeSpan(["inner"], [nt(i.body, s)]);
                             const f = X.makeSpan(["fix"], []);
                             let m = X.makeSpan([i.alignment], [a, f], s);
                             const b = X.makeSpan(["strut"]);
-                            return b.style.height = ie(m.height + m.depth), m.depth && (b.style.verticalAlign = ie(-m.depth)), m.children.unshift(b), m = X.makeSpan(["thinbox"], [m], s), X.makeSpan(["mord", "vbox"], [m], s);
+                            return b.style.height = ae(m.height + m.depth), m.depth && (b.style.verticalAlign = ae(-m.depth)), m.children.unshift(b), m = X.makeSpan(["thinbox"], [m], s), X.makeSpan(["mord", "vbox"], [m], s);
                         },
                         mathmlBuilder: (i, s) => {
                             const a = new se.MathNode("mpadded", [ft(i.body, s)]);
                             if (i.alignment !== "rlap") {
                                 const f = i.alignment === "llap" ? "-1" : "-0.5";
                                 a.setAttribute("lspace", f + "width");
                             }
@@ -16296,15 +16296,15 @@
                         htmlBuilder: (i, s) => {
                             const a = nu(i, s),
                                 f = Ht(a, s, !1);
                             return X.makeFragment(f);
                         },
                         mathmlBuilder: (i, s) => {
                             const a = nu(i, s);
-                            return g0(a, s);
+                            return _0(a, s);
                         }
                     });
                     const ru = (i, s, a, f, m, b, w) => {
                             i = X.makeSpan([], [i]);
                             const A = a && M.isCharacterBox(a);
                             let F, L;
                             if (s) {
@@ -16329,28 +16329,28 @@
                                     positionData: J,
                                     children: [{
                                         type: "kern",
                                         size: f.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
                                         elem: F.elem,
-                                        marginLeft: ie(-b)
+                                        marginLeft: ae(-b)
                                     }, {
                                         type: "kern",
                                         size: F.kern
                                     }, {
                                         type: "elem",
                                         elem: i
                                     }, {
                                         type: "kern",
                                         size: L.kern
                                     }, {
                                         type: "elem",
                                         elem: L.elem,
-                                        marginLeft: ie(b)
+                                        marginLeft: ae(b)
                                     }, {
                                         type: "kern",
                                         size: f.fontMetrics().bigOpSpacing5
                                     }]
                                 }, f);
                             } else if (F) {
                                 const J = i.height - w;
@@ -16359,15 +16359,15 @@
                                     positionData: J,
                                     children: [{
                                         type: "kern",
                                         size: f.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
                                         elem: F.elem,
-                                        marginLeft: ie(-b)
+                                        marginLeft: ae(-b)
                                     }, {
                                         type: "kern",
                                         size: F.kern
                                     }, {
                                         type: "elem",
                                         elem: i
                                     }]
@@ -16382,26 +16382,26 @@
                                         elem: i
                                     }, {
                                         type: "kern",
                                         size: L.kern
                                     }, {
                                         type: "elem",
                                         elem: L.elem,
-                                        marginLeft: ie(b)
+                                        marginLeft: ae(b)
                                     }, {
                                         type: "kern",
                                         size: f.fontMetrics().bigOpSpacing5
                                     }]
                                 }, f);
                             } else
                                 return i;
                             const W = [j];
                             if (F && b !== 0 && !A) {
                                 const J = X.makeSpan(["mspace"], [], f);
-                                J.style.marginRight = ie(b), W.unshift(J);
+                                J.style.marginRight = ae(b), W.unshift(J);
                             }
                             return X.makeSpan(["mop", "op-limits"], W, f);
                         },
                         su = ["\\smallint"],
                         ur = (i, s) => {
                             let a, f, m = !1,
                                 b;
@@ -16436,26 +16436,26 @@
                                 const W = [];
                                 for (let J = 1; J < b.name.length; J++)
                                     W.push(X.mathsym(b.name[J], b.mode, s));
                                 F = X.makeSpan(["mop"], W, s);
                             }
                             let L = 0,
                                 j = 0;
-                            return (F instanceof jt || b.name === "\\oiint" || b.name === "\\oiiint") && !b.suppressBaseShift && (L = (F.height - F.depth) / 2 - s.fontMetrics().axisHeight, j = F.italic), m ? ru(F, a, f, s, w, j, L) : (L && (F.style.position = "relative", F.style.top = ie(L)), F);
+                            return (F instanceof jt || b.name === "\\oiint" || b.name === "\\oiiint") && !b.suppressBaseShift && (L = (F.height - F.depth) / 2 - s.fontMetrics().axisHeight, j = F.italic), m ? ru(F, a, f, s, w, j, L) : (L && (F.style.position = "relative", F.style.top = ae(L)), F);
                         },
                         Gr = (i, s) => {
                             let a;
                             if (i.symbol)
-                                a = new Dn("mo", [An(i.name, i.mode)]), M.contains(su, i.name) && a.setAttribute("largeop", "false");
+                                a = new An("mo", [Sn(i.name, i.mode)]), M.contains(su, i.name) && a.setAttribute("largeop", "false");
                             else if (i.body)
-                                a = new Dn("mo", ln(i.body, s));
+                                a = new An("mo", ln(i.body, s));
                             else {
-                                a = new Dn("mi", [new Pr(i.name.slice(1))]);
-                                const f = new Dn("mo", [An("⁡", "text")]);
-                                i.parentIsSupSub ? a = new Dn("mrow", [a, f]) : a = vo([a, f]);
+                                a = new An("mi", [new Pr(i.name.slice(1))]);
+                                const f = new An("mo", [Sn("⁡", "text")]);
+                                i.parentIsSupSub ? a = new An("mrow", [a, f]) : a = vo([a, f]);
                             }
                             return a;
                         },
                         Xd = {
                             "∏": "\\prod",
                             "∐": "\\coprod",
                             "∑": "\\sum",
@@ -16663,24 +16663,24 @@
                             }
                             if (f) {
                                 const w = a.map((A) => A.toText()).join("");
                                 a = [new se.TextNode(w)];
                             }
                             const m = new se.MathNode("mi", a);
                             m.setAttribute("mathvariant", "normal");
-                            const b = new se.MathNode("mo", [An("⁡", "text")]);
+                            const b = new se.MathNode("mo", [Sn("⁡", "text")]);
                             return i.parentIsSupSub ? new se.MathNode("mrow", [m, b]) : se.newDocumentFragment([m, b]);
                         }
-                    }), S("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), U0({
+                    }), S("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), G0({
                         type: "ordgroup",
                         htmlBuilder(i, s) {
                             return i.semisimple ? X.makeFragment(Ht(i.body, s, !1)) : X.makeSpan(["mord"], Ht(i.body, s, !0), s);
                         },
                         mathmlBuilder(i, s) {
-                            return g0(i.body, s, !0);
+                            return _0(i.body, s, !0);
                         }
                     }), _e({
                         type: "overline",
                         names: ["\\overline"],
                         props: {
                             numArgs: 1
                         },
@@ -16893,25 +16893,25 @@
                             };
                         },
                         htmlBuilder(i, s) {
                             const a = X.makeSpan(["mord", "rule"], [], s),
                                 f = Ze(i.width, s),
                                 m = Ze(i.height, s),
                                 b = i.shift ? Ze(i.shift, s) : 0;
-                            return a.style.borderRightWidth = ie(f), a.style.borderTopWidth = ie(m), a.style.bottom = ie(b), a.width = f, a.height = m + b, a.depth = -b, a.maxFontSize = m * 1.125 * s.sizeMultiplier, a;
+                            return a.style.borderRightWidth = ae(f), a.style.borderTopWidth = ae(m), a.style.bottom = ae(b), a.width = f, a.height = m + b, a.depth = -b, a.maxFontSize = m * 1.125 * s.sizeMultiplier, a;
                         },
                         mathmlBuilder(i, s) {
                             const a = Ze(i.width, s),
                                 f = Ze(i.height, s),
                                 m = i.shift ? Ze(i.shift, s) : 0,
                                 b = s.color && s.getColor() || "black",
                                 w = new se.MathNode("mspace");
-                            w.setAttribute("mathbackground", b), w.setAttribute("width", ie(a)), w.setAttribute("height", ie(f));
+                            w.setAttribute("mathbackground", b), w.setAttribute("width", ae(a)), w.setAttribute("height", ae(f));
                             const A = new se.MathNode("mpadded", [w]);
-                            return m >= 0 ? A.setAttribute("height", ie(m)) : (A.setAttribute("height", ie(m)), A.setAttribute("depth", ie(-m))), A.setAttribute("voffset", ie(m)), A;
+                            return m >= 0 ? A.setAttribute("height", ae(m)) : (A.setAttribute("height", ae(m)), A.setAttribute("depth", ae(-m))), A.setAttribute("voffset", ae(m)), A;
                         }
                     });
 
                     function lu(i, s, a) {
                         const f = Ht(i, s, !1),
                             m = s.sizeMultiplier / a.sizeMultiplier;
                         for (let b = 0; b < f.length; b++) {
@@ -16947,15 +16947,15 @@
                             const a = s.havingSize(i.size);
                             return lu(i.body, a, s);
                         },
                         mathmlBuilder: (i, s) => {
                             const a = s.havingSize(i.size),
                                 f = ln(i.body, a),
                                 m = new se.MathNode("mstyle", f);
-                            return m.setAttribute("mathsize", ie(a.sizeMultiplier)), m;
+                            return m.setAttribute("mathsize", ae(a.sizeMultiplier)), m;
                         }
                     }), _e({
                         type: "smash",
                         names: ["\\smash"],
                         props: {
                             numArgs: 1,
                             numOptionalArgs: 1,
@@ -17039,19 +17039,19 @@
                             s.style.id < Q.TEXT.id && (b = s.fontMetrics().xHeight);
                             let w = m + b / 4;
                             const A = a.height + a.depth + w + m,
                                 {
                                     span: F,
                                     ruleWidth: L,
                                     advanceWidth: j
-                                } = o0.sqrtImage(A, s),
+                                } = u0.sqrtImage(A, s),
                                 W = F.height - L;
                             W > a.height + a.depth + w && (w = (w + W - a.height - a.depth) / 2);
                             const J = F.height - a.height - w - L;
-                            a.style.paddingLeft = ie(j);
+                            a.style.paddingLeft = ae(j);
                             const te = X.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: a,
                                     wrapperClasses: ["svg-align"]
                                 }, {
@@ -17140,15 +17140,15 @@
                             return b.setAttribute("scriptlevel", A[0]), b.setAttribute("displaystyle", A[1]), b;
                         }
                     });
                     const Zd = function(i, s) {
                         const a = i.base;
                         return a ? a.type === "op" ? a.limits && (s.style.size === Q.DISPLAY.size || a.alwaysHandleSupSub) ? ur : null : a.type === "operatorname" ? a.alwaysHandleSupSub && (s.style.size === Q.DISPLAY.size || a.limits) ? iu : null : a.type === "accent" ? M.isCharacterBox(a.base) ? ol : null : a.type === "horizBrace" && !i.sub === a.isOver ? tu : null : null;
                     };
-                    U0({
+                    G0({
                         type: "supsub",
                         htmlBuilder(i, s) {
                             const a = Zd(i, s);
                             if (a)
                                 return a(i, s);
                             const {
                                 base: f,
@@ -17167,19 +17167,19 @@
                             if (b) {
                                 const lt = s.havingStyle(s.style.sub());
                                 F = nt(b, lt, s), J || (W = w.depth + lt.fontMetrics().subDrop * lt.sizeMultiplier / s.sizeMultiplier);
                             }
                             let te;
                             s.style === Q.DISPLAY ? te = L.sup1 : s.style.cramped ? te = L.sup3 : te = L.sup2;
                             const be = s.sizeMultiplier,
-                                Te = ie(0.5 / L.ptPerEm / be);
+                                Te = ae(0.5 / L.ptPerEm / be);
                             let Je = null;
                             if (F) {
                                 const lt = i.base && i.base.type === "op" && i.base.name && (i.base.name === "\\oiint" || i.base.name === "\\oiiint");
-                                (w instanceof jt || lt) && (Je = ie(-w.italic));
+                                (w instanceof jt || lt) && (Je = ae(-w.italic));
                             }
                             let Ge;
                             if (A && F) {
                                 j = Math.max(j, te, A.depth + 0.25 * L.xHeight), W = Math.max(W, L.sub2);
                                 const mt = 4 * L.defaultRuleThickness;
                                 if (j - A.depth - (F.height - W) < mt) {
                                     W = mt - (j - A.depth) + F.height;
@@ -17249,51 +17249,51 @@
                                 }
                             else {
                                 const A = i.base;
                                 A && A.type === "op" && A.limits && (s.style === Q.DISPLAY || A.alwaysHandleSupSub) || A && A.type === "operatorname" && A.alwaysHandleSupSub && (A.limits || s.style === Q.DISPLAY) ? w = "mover" : w = "msup";
                             }
                             return new se.MathNode(w, b);
                         }
-                    }), U0({
+                    }), G0({
                         type: "atom",
                         htmlBuilder(i, s) {
                             return X.mathsym(i.text, i.mode, s, ["m" + i.family]);
                         },
                         mathmlBuilder(i, s) {
-                            const a = new se.MathNode("mo", [An(i.text, i.mode)]);
+                            const a = new se.MathNode("mo", [Sn(i.text, i.mode)]);
                             if (i.family === "bin") {
                                 const f = ll(i, s);
                                 f === "bold-italic" && a.setAttribute("mathvariant", f);
                             } else
                                 i.family === "punct" ? a.setAttribute("separator", "true") : (i.family === "open" || i.family === "close") && a.setAttribute("stretchy", "false");
                             return a;
                         }
                     });
                     const uu = {
                         mi: "italic",
                         mn: "normal",
                         mtext: "normal"
                     };
-                    U0({
+                    G0({
                         type: "mathord",
                         htmlBuilder(i, s) {
                             return X.makeOrd(i, s, "mathord");
                         },
                         mathmlBuilder(i, s) {
-                            const a = new se.MathNode("mi", [An(i.text, i.mode, s)]),
+                            const a = new se.MathNode("mi", [Sn(i.text, i.mode, s)]),
                                 f = ll(i, s) || "italic";
                             return f !== uu[a.type] && a.setAttribute("mathvariant", f), a;
                         }
-                    }), U0({
+                    }), G0({
                         type: "textord",
                         htmlBuilder(i, s) {
                             return X.makeOrd(i, s, "textord");
                         },
                         mathmlBuilder(i, s) {
-                            const a = An(i.text, i.mode, s),
+                            const a = Sn(i.text, i.mode, s),
                                 f = ll(i, s) || "normal";
                             let m;
                             return i.mode === "text" ? m = new se.MathNode("mtext", [a]) : /[0-9]/.test(i.text) ? m = new se.MathNode("mn", [a]) : i.text === "\\prime" ? m = new se.MathNode("mo", [a]) : m = new se.MathNode("mi", [a]), f !== uu[m.type] && m.setAttribute("mathvariant", f), m;
                         }
                     });
                     const Al = {
                             "\\nobreak": "nobreak",
@@ -17306,15 +17306,15 @@
                                 className: "nobreak"
                             },
                             "\\space": {},
                             "\\nobreakspace": {
                                 className: "nobreak"
                             }
                         };
-                    U0({
+                    G0({
                         type: "spacing",
                         htmlBuilder(i, s) {
                             if (Sl.hasOwnProperty(i.text)) {
                                 const a = Sl[i.text].className || "";
                                 if (i.mode === "text") {
                                     const f = X.makeOrd(i, s, "textord");
                                     return f.classes.push(a), f;
@@ -17338,18 +17338,18 @@
                             return a;
                         }
                     });
                     const cu = () => {
                         const i = new se.MathNode("mtd", []);
                         return i.setAttribute("width", "50%"), i;
                     };
-                    U0({
+                    G0({
                         type: "tag",
                         mathmlBuilder(i, s) {
-                            const a = new se.MathNode("mtable", [new se.MathNode("mtr", [cu(), new se.MathNode("mtd", [g0(i.body, s)]), cu(), new se.MathNode("mtd", [g0(i.tag, s)])])]);
+                            const a = new se.MathNode("mtable", [new se.MathNode("mtr", [cu(), new se.MathNode("mtd", [_0(i.body, s)]), cu(), new se.MathNode("mtd", [_0(i.tag, s)])])]);
                             return a.setAttribute("width", "100%"), a;
                         }
                     });
                     const fu = {
                             "\\text": void 0,
                             "\\textrm": "textrm",
                             "\\textsf": "textsf",
@@ -17406,15 +17406,15 @@
                         htmlBuilder(i, s) {
                             const a = du(i, s),
                                 f = Ht(i.body, a, !0);
                             return X.makeSpan(["mord", "text"], f, a);
                         },
                         mathmlBuilder(i, s) {
                             const a = du(i, s);
-                            return g0(i.body, a);
+                            return _0(i.body, a);
                         }
                     }), _e({
                         type: "underline",
                         names: ["\\underline"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
@@ -17516,15 +17516,15 @@
                         mathmlBuilder(i, s) {
                             const a = new se.TextNode(mu(i)),
                                 f = new se.MathNode("mtext", [a]);
                             return f.setAttribute("mathvariant", "monospace"), f;
                         }
                     });
                     const mu = (i) => i.body.replace(/ /g, i.star ? "␣" : " ");
-                    var b0 = wo;
+                    var w0 = wo;
                     const pu = `[ \r
 	]`,
                         Qd = "\\\\[a-zA-Z@]+",
                         Kd = "\\\\[^\uD800-\uDFFF]",
                         $d = "(" + Qd + ")" + pu + "*",
                         e4 = `\\\\(
 |[ \r	]+
@@ -17557,25 +17557,25 @@
                         /**
                          * This function lexes a single token.
                          */
                         lex() {
                             const s = this.input,
                                 a = this.tokenRegex.lastIndex;
                             if (a === s.length)
-                                return new Sn("EOF", new mn(this, a, a));
+                                return new En("EOF", new mn(this, a, a));
                             const f = this.tokenRegex.exec(s);
                             if (f === null || f.index !== a)
-                                throw new o("Unexpected character: '" + s[a] + "'", new Sn(s[a], new mn(this, a, a + 1)));
+                                throw new o("Unexpected character: '" + s[a] + "'", new En(s[a], new mn(this, a, a + 1)));
                             const m = f[6] || f[3] || (f[2] ? "\\ " : " ");
                             if (this.catcodes[m] === 14) {
                                 const b = s.indexOf(`
 `, this.tokenRegex.lastIndex);
                                 return b === -1 ? (this.tokenRegex.lastIndex = s.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = b + 1, this.lex();
                             }
-                            return new Sn(m, new mn(this, a, this.tokenRegex.lastIndex));
+                            return new En(m, new mn(this, a, this.tokenRegex.lastIndex));
                         }
                     }
                     class r4 {
                         /**
                          * Both arguments are optional.  The first argument is an object of
                          * built-in mappings which never change.  The second argument is an object
                          * of initial (global-level) mappings, which will constantly change
@@ -17770,15 +17770,15 @@
                         return console.log(s.reverse().map((a) => a.text).join("")), "";
                     }), S("\\errmessage", (i) => {
                         const s = i.consumeArgs(1)[0];
                         return console.error(s.reverse().map((a) => a.text).join("")), "";
                     }), S("\\show", (i) => {
                         const s = i.popToken(),
                             a = s.text;
-                        return console.log(s, i.macros.get(a), b0[a], q.math[a], q.text[a]), "";
+                        return console.log(s, i.macros.get(a), w0[a], q.math[a], q.text[a]), "";
                     }), S("\\bgroup", "{"), S("\\egroup", "}"), S("~", "\\nobreakspace"), S("\\lq", "`"), S("\\rq", "'"), S("\\aa", "\\r a"), S("\\AA", "\\r A"), S("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`©}"), S("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), S("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`®}"), S("ℬ", "\\mathscr{B}"), S("ℰ", "\\mathscr{E}"), S("ℱ", "\\mathscr{F}"), S("ℋ", "\\mathscr{H}"), S("ℐ", "\\mathscr{I}"), S("ℒ", "\\mathscr{L}"), S("ℳ", "\\mathscr{M}"), S("ℛ", "\\mathscr{R}"), S("ℭ", "\\mathfrak{C}"), S("ℌ", "\\mathfrak{H}"), S("ℨ", "\\mathfrak{Z}"), S("\\Bbbk", "\\Bbb{k}"), S("·", "\\cdotp"), S("\\llap", "\\mathllap{\\textrm{#1}}"), S("\\rlap", "\\mathrlap{\\textrm{#1}}"), S("\\clap", "\\mathclap{\\textrm{#1}}"), S("\\mathstrut", "\\vphantom{(}"), S("\\underbar", "\\underline{\\text{#1}}"), S("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), S("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`≠}}"), S("\\ne", "\\neq"), S("≠", "\\neq"), S("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`∉}}"), S("∉", "\\notin"), S("≘", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`≘}}"), S("≙", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`≘}}"), S("≚", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`≚}}"), S("≛", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`≛}}"), S("≝", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`≝}}"), S("≞", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`≞}}"), S("≟", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`≟}}"), S("⟂", "\\perp"), S("‼", "\\mathclose{!\\mkern-0.8mu!}"), S("∌", "\\notni"), S("⌜", "\\ulcorner"), S("⌝", "\\urcorner"), S("⌞", "\\llcorner"), S("⌟", "\\lrcorner"), S("©", "\\copyright"), S("®", "\\textregistered"), S("️", "\\textregistered"), S("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), S("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), S("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), S("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), S("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), S("⋮", "\\vdots"), S("\\varGamma", "\\mathit{\\Gamma}"), S("\\varDelta", "\\mathit{\\Delta}"), S("\\varTheta", "\\mathit{\\Theta}"), S("\\varLambda", "\\mathit{\\Lambda}"), S("\\varXi", "\\mathit{\\Xi}"), S("\\varPi", "\\mathit{\\Pi}"), S("\\varSigma", "\\mathit{\\Sigma}"), S("\\varUpsilon", "\\mathit{\\Upsilon}"), S("\\varPhi", "\\mathit{\\Phi}"), S("\\varPsi", "\\mathit{\\Psi}"), S("\\varOmega", "\\mathit{\\Omega}"), S("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), S("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), S("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), S("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), S("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), S("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
                     const bu = {
                         ",": "\\dotsc",
                         "\\not": "\\dotsb",
                         // \keybin@ checks for the following:
                         "+": "\\dotsb",
                         "=": "\\dotsb",
@@ -17868,15 +17868,15 @@
                     }), S("\\cdots", function(i) {
                         return i.future().text in Tl ? "\\@cdots\\," : "\\@cdots";
                     }), S("\\dotsb", "\\cdots"), S("\\dotsm", "\\cdots"), S("\\dotsi", "\\!\\cdots"), S("\\dotsx", "\\ldots\\,"), S("\\DOTSI", "\\relax"), S("\\DOTSB", "\\relax"), S("\\DOTSX", "\\relax"), S("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), S("\\,", "\\tmspace+{3mu}{.1667em}"), S("\\thinspace", "\\,"), S("\\>", "\\mskip{4mu}"), S("\\:", "\\tmspace+{4mu}{.2222em}"), S("\\medspace", "\\:"), S("\\;", "\\tmspace+{5mu}{.2777em}"), S("\\thickspace", "\\;"), S("\\!", "\\tmspace-{3mu}{.1667em}"), S("\\negthinspace", "\\!"), S("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), S("\\negthickspace", "\\tmspace-{5mu}{.277em}"), S("\\enspace", "\\kern.5em "), S("\\enskip", "\\hskip.5em\\relax"), S("\\quad", "\\hskip1em\\relax"), S("\\qquad", "\\hskip2em\\relax"), S("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), S("\\tag@paren", "\\tag@literal{({#1})}"), S("\\tag@literal", (i) => {
                         if (i.macros.get("\\df@tag"))
                             throw new o("Multiple \\tag");
                         return "\\gdef\\df@tag{\\text{#1}}";
                     }), S("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), S("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), S("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), S("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), S("\\newline", "\\\\\\relax"), S("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-                    const wu = ie(Ct["Main-Regular"][84][1] - 0.7 * Ct["Main-Regular"][65][1]);
+                    const wu = ae(Ct["Main-Regular"][84][1] - 0.7 * Ct["Main-Regular"][65][1]);
                     S("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + wu + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), S("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + wu + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), S("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), S("\\@hspace", "\\hskip #1\\relax"), S("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), S("\\ordinarycolon", ":"), S("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), S("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), S("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), S("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), S("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), S("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), S("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), S("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), S("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), S("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), S("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), S("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), S("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), S("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), S("∷", "\\dblcolon"), S("∹", "\\eqcolon"), S("≔", "\\coloneqq"), S("≕", "\\eqqcolon"), S("⩴", "\\Coloneqq"), S("\\ratio", "\\vcentcolon"), S("\\coloncolon", "\\dblcolon"), S("\\colonequals", "\\coloneqq"), S("\\coloncolonequals", "\\Coloneqq"), S("\\equalscolon", "\\eqqcolon"), S("\\equalscoloncolon", "\\Eqqcolon"), S("\\colonminus", "\\coloneq"), S("\\coloncolonminus", "\\Coloneq"), S("\\minuscolon", "\\eqcolon"), S("\\minuscoloncolon", "\\Eqcolon"), S("\\coloncolonapprox", "\\Colonapprox"), S("\\coloncolonsim", "\\Colonsim"), S("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), S("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), S("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), S("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), S("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`∌}}"), S("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), S("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), S("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), S("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), S("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), S("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), S("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), S("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), S("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{≩}"), S("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{≨}"), S("\\ngeqq", "\\html@mathml{\\@ngeqq}{≱}"), S("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{≱}"), S("\\nleqq", "\\html@mathml{\\@nleqq}{≰}"), S("\\nleqslant", "\\html@mathml{\\@nleqslant}{≰}"), S("\\nshortmid", "\\html@mathml{\\@nshortmid}{∤}"), S("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{∦}"), S("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{⊈}"), S("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{⊉}"), S("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{⊊}"), S("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{⫋}"), S("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{⊋}"), S("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{⫌}"), S("\\imath", "\\html@mathml{\\@imath}{ı}"), S("\\jmath", "\\html@mathml{\\@jmath}{ȷ}"), S("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`⟦}}"), S("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`⟧}}"), S("⟦", "\\llbracket"), S("⟧", "\\rrbracket"), S("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`⦃}}"), S("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`⦄}}"), S("⦃", "\\lBrace"), S("⦄", "\\rBrace"), S("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`⦵}}"), S("⦵", "\\minuso"), S("\\darr", "\\downarrow"), S("\\dArr", "\\Downarrow"), S("\\Darr", "\\Downarrow"), S("\\lang", "\\langle"), S("\\rang", "\\rangle"), S("\\uarr", "\\uparrow"), S("\\uArr", "\\Uparrow"), S("\\Uarr", "\\Uparrow"), S("\\N", "\\mathbb{N}"), S("\\R", "\\mathbb{R}"), S("\\Z", "\\mathbb{Z}"), S("\\alef", "\\aleph"), S("\\alefsym", "\\aleph"), S("\\Alpha", "\\mathrm{A}"), S("\\Beta", "\\mathrm{B}"), S("\\bull", "\\bullet"), S("\\Chi", "\\mathrm{X}"), S("\\clubs", "\\clubsuit"), S("\\cnums", "\\mathbb{C}"), S("\\Complex", "\\mathbb{C}"), S("\\Dagger", "\\ddagger"), S("\\diamonds", "\\diamondsuit"), S("\\empty", "\\emptyset"), S("\\Epsilon", "\\mathrm{E}"), S("\\Eta", "\\mathrm{H}"), S("\\exist", "\\exists"), S("\\harr", "\\leftrightarrow"), S("\\hArr", "\\Leftrightarrow"), S("\\Harr", "\\Leftrightarrow"), S("\\hearts", "\\heartsuit"), S("\\image", "\\Im"), S("\\infin", "\\infty"), S("\\Iota", "\\mathrm{I}"), S("\\isin", "\\in"), S("\\Kappa", "\\mathrm{K}"), S("\\larr", "\\leftarrow"), S("\\lArr", "\\Leftarrow"), S("\\Larr", "\\Leftarrow"), S("\\lrarr", "\\leftrightarrow"), S("\\lrArr", "\\Leftrightarrow"), S("\\Lrarr", "\\Leftrightarrow"), S("\\Mu", "\\mathrm{M}"), S("\\natnums", "\\mathbb{N}"), S("\\Nu", "\\mathrm{N}"), S("\\Omicron", "\\mathrm{O}"), S("\\plusmn", "\\pm"), S("\\rarr", "\\rightarrow"), S("\\rArr", "\\Rightarrow"), S("\\Rarr", "\\Rightarrow"), S("\\real", "\\Re"), S("\\reals", "\\mathbb{R}"), S("\\Reals", "\\mathbb{R}"), S("\\Rho", "\\mathrm{P}"), S("\\sdot", "\\cdot"), S("\\sect", "\\S"), S("\\spades", "\\spadesuit"), S("\\sub", "\\subset"), S("\\sube", "\\subseteq"), S("\\supe", "\\supseteq"), S("\\Tau", "\\mathrm{T}"), S("\\thetasym", "\\vartheta"), S("\\weierp", "\\wp"), S("\\Zeta", "\\mathrm{Z}"), S("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), S("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), S("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), S("\\bra", "\\mathinner{\\langle{#1}|}"), S("\\ket", "\\mathinner{|{#1}\\rangle}"), S("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), S("\\Bra", "\\left\\langle#1\\right|"), S("\\Ket", "\\left|#1\\right\\rangle");
                     const yu = (i) => (s) => {
                         const a = s.consumeArg().tokens,
                             f = s.consumeArg().tokens,
                             m = s.consumeArg().tokens,
                             b = s.consumeArg().tokens,
                             w = s.macros.get("|"),
@@ -17991,15 +17991,15 @@
                                 } = this.consumeArg(["]"]);
                             } else
                                 ({
                                     tokens: m,
                                     start: a,
                                     end: f
                                 } = this.consumeArg());
-                            return this.pushToken(new Sn("EOF", f.loc)), this.pushTokens(m), a.range(f, "");
+                            return this.pushToken(new En("EOF", f.loc)), this.pushTokens(m), a.range(f, "");
                         }
                         /**
                          * Consume all following space tokens, without expansion.
                          */
                         consumeSpaces() {
                             for (; this.future().text === " ";)
                                 this.stack.pop();
@@ -18136,15 +18136,15 @@
                             throw new Error();
                         }
                         /**
                          * Fully expand the given macro name and return the resulting list of
                          * tokens, or return `undefined` if no such macro is defined.
                          */
                         expandMacro(s) {
-                            return this.macros.has(s) ? this.expandTokens([new Sn(s)]) : void 0;
+                            return this.macros.has(s) ? this.expandTokens([new En(s)]) : void 0;
                         }
                         /**
                          * Fully expand the given token stream and return the resulting list of
                          * tokens.  Note that the input tokens are in reverse order, but the
                          * output tokens are in forward order.
                          */
                         expandTokens(s) {
@@ -18201,22 +18201,22 @@
                         /**
                          * Determine whether a command is currently "defined" (has some
                          * functionality), meaning that it's a macro (in the current group),
                          * a function, a symbol, or one of the special commands listed in
                          * `implicitCommands`.
                          */
                         isDefined(s) {
-                            return this.macros.has(s) || b0.hasOwnProperty(s) || q.math.hasOwnProperty(s) || q.text.hasOwnProperty(s) || vu.hasOwnProperty(s);
+                            return this.macros.has(s) || w0.hasOwnProperty(s) || q.math.hasOwnProperty(s) || q.text.hasOwnProperty(s) || vu.hasOwnProperty(s);
                         }
                         /**
                          * Determine whether a command is expandable.
                          */
                         isExpandable(s) {
                             const a = this.macros.get(s);
-                            return a != null ? typeof a == "string" || typeof a == "function" || !a.unexpandable : b0.hasOwnProperty(s) && !b0[s].primitive;
+                            return a != null ? typeof a == "string" || typeof a == "function" || !a.unexpandable : w0.hasOwnProperty(s) && !w0[s].primitive;
                         }
                     }
                     const ku = /^[₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ]/,
                         qs = Object.freeze({
                             "₊": "+",
                             "₋": "-",
                             "₌": "=",
@@ -18761,15 +18761,15 @@
                         }
                         /**
                          * Fully parse a separate sequence of tokens as a separate job.
                          * Tokens should be specified in reverse order, as in a MacroDefinition.
                          */
                         subparse(s) {
                             const a = this.nextToken;
-                            this.consume(), this.gullet.pushToken(new Sn("}")), this.gullet.pushTokens(s);
+                            this.consume(), this.gullet.pushToken(new En("}")), this.gullet.pushTokens(s);
                             const f = this.parseExpression(!1);
                             return this.expect("}"), this.nextToken = a, f;
                         }
                         /**
                          * Parses an "expression", which is a list of atoms.
                          *
                          * `breakOnInfix`: Should the parsing stop when we hit infix nodes? This
@@ -18781,15 +18781,15 @@
                          *                     expression.
                          */
                         parseExpression(s, a) {
                             const f = [];
                             for (;;) {
                                 this.mode === "math" && this.consumeSpaces();
                                 const m = this.fetch();
-                                if (Us.endOfExpression.indexOf(m.text) !== -1 || a && m.text === a || s && b0[m.text] && b0[m.text].infix)
+                                if (Us.endOfExpression.indexOf(m.text) !== -1 || a && m.text === a || s && w0[m.text] && w0[m.text].infix)
                                     break;
                                 const b = this.parseAtom(a);
                                 if (b) {
                                     if (b.type === "internal")
                                         continue;
                                 } else
                                     break;
@@ -18910,19 +18910,19 @@
                                         type: "ordgroup",
                                         mode: this.mode,
                                         body: A
                                     };
                                 } else if (qs[b.text]) {
                                     const w = ku.test(b.text),
                                         A = [];
-                                    for (A.push(new Sn(qs[b.text])), this.consume();;) {
+                                    for (A.push(new En(qs[b.text])), this.consume();;) {
                                         const L = this.fetch().text;
                                         if (!qs[L] || ku.test(L) !== w)
                                             break;
-                                        A.unshift(new Sn(qs[L])), this.consume();
+                                        A.unshift(new En(qs[L])), this.consume();
                                     }
                                     const F = this.subparse(A);
                                     w ? m = {
                                         type: "ordgroup",
                                         mode: "math",
                                         body: F
                                     } : f = {
@@ -18943,15 +18943,15 @@
                         }
                         /**
                          * Parses an entire function, including its base and all of its arguments.
                          */
                         parseFunction(s, a) {
                             const f = this.fetch(),
                                 m = f.text,
-                                b = b0[m];
+                                b = w0[m];
                             if (!b)
                                 return null;
                             if (this.consume(), a && a !== "atom" && !b.allowedInArgument)
                                 throw new o("Got function '" + m + "' with no arguments" + (a ? " as " + a : ""), f);
                             if (this.mode === "text" && !b.allowedInText)
                                 throw new o("Can't use function '" + m + "' in text mode", f);
                             if (this.mode === "math" && b.allowedInMath === !1)
@@ -18968,15 +18968,15 @@
                         callFunction(s, a, f, m, b) {
                             const w = {
                                     funcName: s,
                                     parser: this,
                                     token: m,
                                     breakOnTokenText: b
                                 },
-                                A = b0[s];
+                                A = w0[s];
                             if (A && A.handler)
                                 return A.handler(w, a, f);
                             throw new o("No function handler for " + s);
                         }
                         /**
                          * Parses the arguments of a function or environment
                          */
@@ -19324,15 +19324,15 @@
                         if (delete a.gullet.macros.current["\\current@color"], delete a.gullet.macros.current["\\color"], a.gullet.macros.get("\\df@tag")) {
                             if (!s.displayMode)
                                 throw new o("\\tag works only in display equations");
                             f = [{
                                 type: "tag",
                                 mode: "text",
                                 body: f,
-                                tag: a.subparse([new Sn("\\df@tag")])
+                                tag: a.subparse([new En("\\df@tag")])
                             }];
                         }
                         return f;
                     };
                     let Au = function(i, s, a) {
                         s.textContent = "";
                         const f = Ml(i, a).toNode();
@@ -19444,20 +19444,20 @@
                              * Expose the dom tree node types, which can be useful for type checking nodes.
                              *
                              * NOTE: This method is not currently recommended for public use.
                              * The internal tree representation is unstable and is very likely
                              * to change. Use at your own risk.
                              */
                             __domTree: {
-                                Span: s0,
+                                Span: i0,
                                 Anchor: wt,
                                 SymbolNode: jt,
                                 SvgNode: en,
                                 PathNode: dn,
-                                LineNode: p0
+                                LineNode: g0
                             }
                         },
                         u4 = o4;
                     return r = r.default, r;
                 }()
             );
         });
@@ -19693,18 +19693,18 @@
         pedantic: !1,
         renderer: null,
         silent: !1,
         tokenizer: null,
         walkTokens: null
     };
 }
-let nr = Ja();
+let rr = Ja();
 
 function yh(t) {
-    nr = t;
+    rr = t;
 }
 const vh = /[&<>"']/,
     zp = new RegExp(vh.source, "g"),
     kh = /[<>"']|&(?!(#\d{1,7}|#[Xx][a-fA-F0-9]{1,6}|\w+);)/,
     Rp = new RegExp(kh.source, "g"),
     Op = {
         "&": "&amp;",
@@ -19850,15 +19850,15 @@
 class Fi {
     // set by the lexer
     constructor(e) {
         _t(this, "options");
         _t(this, "rules");
         // set by the lexer
         _t(this, "lexer");
-        this.options = e || nr;
+        this.options = e || rr;
     }
     space(e) {
         const n = this.rules.block.newline.exec(e);
         if (n && n[0].length > 0)
             return {
                 type: "space",
                 raw: n[0]
@@ -20421,15 +20421,15 @@
 class e0 {
     constructor(e) {
         _t(this, "tokens");
         _t(this, "options");
         _t(this, "state");
         _t(this, "tokenizer");
         _t(this, "inlineQueue");
-        this.tokens = [], this.tokens.links = /* @__PURE__ */ Object.create(null), this.options = e || nr, this.options.tokenizer = this.options.tokenizer || new Fi(), this.tokenizer = this.options.tokenizer, this.tokenizer.options = this.options, this.tokenizer.lexer = this, this.inlineQueue = [], this.state = {
+        this.tokens = [], this.tokens.links = /* @__PURE__ */ Object.create(null), this.options = e || rr, this.options.tokenizer = this.options.tokenizer || new Fi(), this.tokenizer = this.options.tokenizer, this.tokenizer.options = this.options, this.tokenizer.lexer = this, this.inlineQueue = [], this.state = {
             inLink: !1,
             inRawBlock: !1,
             top: !0
         };
         const n = {
             block: Js.normal,
             inline: Zr.normal
@@ -20655,15 +20655,15 @@
             }
         return n;
     }
 }
 class Mi {
     constructor(e) {
         _t(this, "options");
-        this.options = e || nr;
+        this.options = e || rr;
     }
     code(e, n, r) {
         var o;
         const l = (o = (n || "").match(/^\S*/)) == null ? void 0 : o[0];
         return e = e.replace(/\n$/, "") + `
 `, l ? '<pre><code class="language-' + wn(l) + '">' + (r ? e : wn(e, !0)) + `</code></pre>
 ` : "<pre><code>" + (r ? e : wn(e, !0)) + `</code></pre>
@@ -20789,15 +20789,15 @@
     }
 }
 class t0 {
     constructor(e) {
         _t(this, "options");
         _t(this, "renderer");
         _t(this, "textRenderer");
-        this.options = e || nr, this.options.renderer = this.options.renderer || new Mi(), this.renderer = this.options.renderer, this.renderer.options = this.options, this.textRenderer = new no();
+        this.options = e || rr, this.options.renderer = this.options.renderer || new Mi(), this.renderer = this.options.renderer, this.renderer.options = this.options, this.textRenderer = new no();
     }
     /**
      * Static Parse Method
      */
     static parse(e, n) {
         return new t0(n).parse(e);
     }
@@ -21000,15 +21000,15 @@
         }
         return r;
     }
 }
 class rs {
     constructor(e) {
         _t(this, "options");
-        this.options = e || nr;
+        this.options = e || rr;
     }
     /**
      * Process markdown before marked
      */
     preprocess(e) {
         return e;
     }
@@ -21223,31 +21223,31 @@
             return n ? Promise.resolve(l) : l;
         }
         if (n)
             return Promise.reject(r);
         throw r;
     };
 };
-const er = new Ch();
+const tr = new Ch();
 
 function ut(t, e) {
-    return er.parse(t, e);
+    return tr.parse(t, e);
 }
 ut.options = ut.setOptions = function(t) {
-    return er.setOptions(t), ut.defaults = er.defaults, yh(ut.defaults), ut;
+    return tr.setOptions(t), ut.defaults = tr.defaults, yh(ut.defaults), ut;
 };
 ut.getDefaults = Ja;
-ut.defaults = nr;
+ut.defaults = rr;
 ut.use = function(...t) {
-    return er.use(...t), ut.defaults = er.defaults, yh(ut.defaults), ut;
+    return tr.use(...t), ut.defaults = tr.defaults, yh(ut.defaults), ut;
 };
 ut.walkTokens = function(t, e) {
-    return er.walkTokens(t, e);
+    return tr.walkTokens(t, e);
 };
-ut.parseInline = er.parseInline;
+ut.parseInline = tr.parseInline;
 ut.Parser = t0;
 ut.parser = t0.parse;
 ut.Renderer = Mi;
 ut.TextRenderer = no;
 ut.Lexer = e0;
 ut.lexer = e0.lex;
 ut.Tokenizer = Fi;
@@ -22036,51 +22036,51 @@
                             Me = !!re.lookbehind,
                             Ne = !!re.greedy,
                             ke = re.alias;
                         if (Ne && !re.pattern.global) {
                             var ce = re.pattern.toString().match(/[imsuy]*$/)[0];
                             re.pattern = RegExp(re.pattern.source, ce + "g");
                         }
-                        for (var he = re.pattern || re, ae = C.next, Be = R; ae !== D.tail && !(I && Be >= I.reach); Be += ae.value.length, ae = ae.next) {
-                            var oe = ae.value;
+                        for (var he = re.pattern || re, le = C.next, Be = R; le !== D.tail && !(I && Be >= I.reach); Be += le.value.length, le = le.next) {
+                            var oe = le.value;
                             if (D.length > N.length)
                                 return;
                             if (!(oe instanceof h)) {
                                 var Q = 1,
                                     de;
                                 if (Ne) {
                                     if (de = p(he, Be, N, Me), !de || de.index >= N.length)
                                         break;
                                     var ve = de.index,
                                         V = de.index + de[0].length,
                                         ee = Be;
-                                    for (ee += ae.value.length; ve >= ee;)
-                                        ae = ae.next, ee += ae.value.length;
-                                    if (ee -= ae.value.length, Be = ee, ae.value instanceof h)
+                                    for (ee += le.value.length; ve >= ee;)
+                                        le = le.next, ee += le.value.length;
+                                    if (ee -= le.value.length, Be = ee, le.value instanceof h)
                                         continue;
-                                    for (var we = ae; we !== D.tail && (ee < V || typeof we.value == "string"); we = we.next)
+                                    for (var we = le; we !== D.tail && (ee < V || typeof we.value == "string"); we = we.next)
                                         Q++, ee += we.value.length;
                                     Q--, oe = N.slice(Be, ee), de.index -= Be;
                                 } else if (de = p(he, 0, oe, Me), !de)
                                     continue;
                                 var ve = de.index,
                                     $ = de[0],
                                     xe = oe.slice(0, ve),
                                     Se = oe.slice(ve + $.length),
                                     We = Be + oe.length;
                                 I && We > I.reach && (I.reach = We);
-                                var Ie = ae.prev;
+                                var Ie = le.prev;
                                 xe && (Ie = k(D, Ie, xe), Be += xe.length), T(D, Ie, Q);
                                 var Xe = new h(z, pe ? u.tokenize($, pe) : $, ke, $);
-                                if (ae = k(D, Ie, Xe), Se && k(D, ae, Se), Q > 1) {
+                                if (le = k(D, Ie, Xe), Se && k(D, le, Se), Q > 1) {
                                     var Ue = {
                                         cause: z + "," + ne,
                                         reach: We
                                     };
-                                    _(N, D, E, ae.prev, Be, Ue), I && Ue.reach > I.reach && (I.reach = Ue.reach);
+                                    _(N, D, E, le.prev, Be, Ue), I && Ue.reach > I.reach && (I.reach = Ue.reach);
                                 }
                             }
                         }
                     }
                 }
         }
 
@@ -23336,39 +23336,39 @@
         super(), K5(this, e, r6, n6, e6, {
             margin: 0
         });
     }
 }
 const {
     SvelteComponent: i6,
-    append: Q0,
+    append: K0,
     attr: n0,
     binding_callbacks: qc,
     check_outros: Lh,
     create_component: l6,
     create_slot: a6,
     destroy_component: o6,
     destroy_each: Hh,
     detach: Pe,
-    element: c0,
+    element: f0,
     empty: Or,
     ensure_array_like: Bi,
     get_all_dirty_from_scope: u6,
     get_slot_changes: c6,
     group_outros: Ph,
     init: f6,
     insert: qe,
     mount_component: h6,
     noop: Sa,
     safe_not_equal: d6,
-    set_data: Mn,
-    set_style: x0,
+    set_data: Bn,
+    set_style: T0,
     space: r0,
     text: Ft,
-    toggle_class: Tn,
+    toggle_class: Fn,
     transition_in: Mr,
     transition_out: Br,
     update_slot_base: m6
 } = window.__gradio__svelte__internal, {
     tick: p6
 } = window.__gradio__svelte__internal, {
     onDestroy: g6
@@ -23399,23 +23399,23 @@
             t,
             /*$$scope*/
             t[28],
             Uc
         );
     return {
         c() {
-            e = c0("span"), r = Ft(n), l = r0(), u && u.c(), n0(e, "class", "error svelte-1yserjw");
+            e = f0("span"), r = Ft(n), l = r0(), u && u.c(), n0(e, "class", "error svelte-1yserjw");
         },
         m(h, p) {
-            qe(h, e, p), Q0(e, r), qe(h, l, p), u && u.m(h, p), o = !0;
+            qe(h, e, p), K0(e, r), qe(h, l, p), u && u.m(h, p), o = !0;
         },
         p(h, p) {
             (!o || p[0] & /*i18n*/
                 2) && n !== (n = /*i18n*/
-                h[1]("common.error") + "") && Mn(r, n), u && u.p && (!o || p[0] & /*$$scope*/
+                h[1]("common.error") + "") && Bn(r, n), u && u.p && (!o || p[0] & /*$$scope*/
                 268435456) && m6(
                 u,
                 c,
                 h,
                 /*$$scope*/
                 h[28],
                 o ? c6(
@@ -23489,42 +23489,42 @@
         );
     }
     ~(o = M(t)) && (c = U[o] = P[o](t));
     let N = ! /*timer*/
         t[5] && t1(t);
     return {
         c() {
-            _ && _.c(), e = r0(), n = c0("div"), T && T.c(), r = r0(), O && O.c(), l = r0(), c && c.c(), u = r0(), N && N.c(), h = Or(), n0(n, "class", "progress-text svelte-1yserjw"), Tn(
+            _ && _.c(), e = r0(), n = f0("div"), T && T.c(), r = r0(), O && O.c(), l = r0(), c && c.c(), u = r0(), N && N.c(), h = Or(), n0(n, "class", "progress-text svelte-1yserjw"), Fn(
                 n,
                 "meta-text-center",
                 /*variant*/
                 t[8] === "center"
-            ), Tn(
+            ), Fn(
                 n,
                 "meta-text",
                 /*variant*/
                 t[8] === "default"
             );
         },
         m(D, E) {
-            _ && _.m(D, E), qe(D, e, E), qe(D, n, E), T && T.m(n, null), Q0(n, r), O && O.m(n, null), qe(D, l, E), ~o && U[o].m(D, E), qe(D, u, E), N && N.m(D, E), qe(D, h, E), p = !0;
+            _ && _.m(D, E), qe(D, e, E), qe(D, n, E), T && T.m(n, null), K0(n, r), O && O.m(n, null), qe(D, l, E), ~o && U[o].m(D, E), qe(D, u, E), N && N.m(D, E), qe(D, h, E), p = !0;
         },
         p(D, E) {
             /*variant*/
             D[8] === "default" && /*show_eta_bar*/
                 D[18] && /*show_progress*/
                 D[6] === "full" ? _ ? _.p(D, E) : (_ = Vc(D), _.c(), _.m(e.parentNode, e)) : _ && (_.d(1), _ = null), k === (k = v(D)) && T ? T.p(D, E) : (T && T.d(1), T = k && k(D), T && (T.c(), T.m(n, r))), /*timer*/
                 D[5] ? O ? O.p(D, E) : (O = Yc(D), O.c(), O.m(n, null)) : O && (O.d(1), O = null), (!p || E[0] & /*variant*/
-                    256) && Tn(
+                    256) && Fn(
                     n,
                     "meta-text-center",
                     /*variant*/
                     D[8] === "center"
                 ), (!p || E[0] & /*variant*/
-                    256) && Tn(
+                    256) && Fn(
                     n,
                     "meta-text",
                     /*variant*/
                     D[8] === "default"
                 );
             let C = o;
             o = M(D), o === C ? ~o && U[o].p(D, E) : (c && (Ph(), Br(U[C], 1, 1, () => {
@@ -23545,23 +23545,23 @@
 }
 
 function Vc(t) {
     let e, n = `translateX(${/*eta_level*/
   (t[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            e = c0("div"), n0(e, "class", "eta-bar svelte-1yserjw"), x0(e, "transform", n);
+            e = f0("div"), n0(e, "class", "eta-bar svelte-1yserjw"), T0(e, "transform", n);
         },
         m(r, l) {
             qe(r, e, l);
         },
         p(r, l) {
             l[0] & /*eta_level*/
                 131072 && n !== (n = `translateX(${/*eta_level*/
-      (r[17] || 0) * 100 - 100}%)`) && x0(e, "transform", n);
+      (r[17] || 0) * 100 - 100}%)`) && T0(e, "transform", n);
         },
         d(r) {
             r && Pe(e);
         }
     };
 }
 
@@ -23596,16 +23596,16 @@
         },
         m(u, h) {
             qe(u, e, h), qe(u, r, h), qe(u, l, h), qe(u, o, h), qe(u, c, h);
         },
         p(u, h) {
             h[0] & /*queue_position*/
                 4 && n !== (n = /*queue_position*/
-                    u[2] + 1 + "") && Mn(r, n), h[0] & /*queue_size*/
-                8 && Mn(
+                    u[2] + 1 + "") && Bn(r, n), h[0] & /*queue_size*/
+                8 && Bn(
                     o,
                     /*queue_size*/
                     u[3]
                 );
         },
         d(u) {
             u && (Pe(e), Pe(r), Pe(l), Pe(o), Pe(c));
@@ -23677,15 +23677,15 @@
         },
         m(_, v) {
             p.m(_, v), qe(_, e, v), qe(_, r, v), qe(_, l, v), qe(_, c, v);
         },
         p(_, v) {
             h === (h = u(_)) && p ? p.p(_, v) : (p.d(1), p = h(_), p && (p.c(), p.m(e.parentNode, e))), v[0] & /*progress*/
                 128 && n !== (n = /*p*/
-                    _[38].unit + "") && Mn(r, n);
+                    _[38].unit + "") && Bn(r, n);
         },
         d(_) {
             _ && (Pe(e), Pe(r), Pe(l), Pe(c)), p.d(_);
         }
     };
 }
 
@@ -23703,15 +23703,15 @@
             qe(r, n, l);
         },
         p(r, l) {
             l[0] & /*progress*/
                 128 && e !== (e = vr(
                     /*p*/
                     r[38].index || 0
-                ) + "") && Mn(n, e);
+                ) + "") && Bn(n, e);
         },
         d(r) {
             r && Pe(n);
         }
     };
 }
 
@@ -23733,19 +23733,19 @@
             qe(c, n, u), qe(c, r, u), qe(c, o, u);
         },
         p(c, u) {
             u[0] & /*progress*/
                 128 && e !== (e = vr(
                     /*p*/
                     c[38].index || 0
-                ) + "") && Mn(n, e), u[0] & /*progress*/
+                ) + "") && Bn(n, e), u[0] & /*progress*/
                 128 && l !== (l = vr(
                     /*p*/
                     c[38].length
-                ) + "") && Mn(o, l);
+                ) + "") && Bn(o, l);
         },
         d(c) {
             c && (Pe(n), Pe(r), Pe(o));
         }
     };
 }
 
@@ -23786,22 +23786,22 @@
             ), r = Ft(n), l = Ft("s");
         },
         m(o, c) {
             qe(o, e, c), qe(o, r, c), qe(o, l, c);
         },
         p(o, c) {
             c[0] & /*formatted_timer*/
-                1048576 && Mn(
+                1048576 && Bn(
                     e,
                     /*formatted_timer*/
                     o[20]
                 ), c[0] & /*eta, formatted_eta*/
                 524289 && n !== (n = /*eta*/
                     o[0] ? `/${/*formatted_eta*/
-      o[19]}` : "") && Mn(r, n);
+      o[19]}` : "") && Bn(r, n);
         },
         d(o) {
             o && (Pe(e), Pe(r), Pe(l));
         }
     };
 }
 
@@ -23844,24 +23844,24 @@
   t[15] * 100}%`,
         u = (
             /*progress*/
             t[7] != null && Zc(t)
         );
     return {
         c() {
-            e = c0("div"), n = c0("div"), u && u.c(), r = r0(), l = c0("div"), o = c0("div"), n0(n, "class", "progress-level-inner svelte-1yserjw"), n0(o, "class", "progress-bar svelte-1yserjw"), x0(o, "width", c), n0(l, "class", "progress-bar-wrap svelte-1yserjw"), n0(e, "class", "progress-level svelte-1yserjw");
+            e = f0("div"), n = f0("div"), u && u.c(), r = r0(), l = f0("div"), o = f0("div"), n0(n, "class", "progress-level-inner svelte-1yserjw"), n0(o, "class", "progress-bar svelte-1yserjw"), T0(o, "width", c), n0(l, "class", "progress-bar-wrap svelte-1yserjw"), n0(e, "class", "progress-level svelte-1yserjw");
         },
         m(h, p) {
-            qe(h, e, p), Q0(e, n), u && u.m(n, null), Q0(e, r), Q0(e, l), Q0(l, o), t[30](o);
+            qe(h, e, p), K0(e, n), u && u.m(n, null), K0(e, r), K0(e, l), K0(l, o), t[30](o);
         },
         p(h, p) {
             /*progress*/
             h[7] != null ? u ? u.p(h, p) : (u = Zc(h), u.c(), u.m(n, null)) : u && (u.d(1), u = null), p[0] & /*last_progress_level*/
                 32768 && c !== (c = `${/*last_progress_level*/
-      h[15] * 100}%`) && x0(o, "width", c);
+      h[15] * 100}%`) && T0(o, "width", c);
         },
         i: Sa,
         o: Sa,
         d(h) {
             h && Pe(e), u && u.d(), t[30](null);
         }
     };
@@ -23982,15 +23982,15 @@
         },
         m(r, l) {
             qe(r, n, l);
         },
         p(r, l) {
             l[0] & /*progress*/
                 128 && e !== (e = /*p*/
-                    r[38].desc + "") && Mn(n, e);
+                    r[38].desc + "") && Bn(n, e);
         },
         d(r) {
             r && Pe(n);
         }
     };
 }
 
@@ -24025,15 +24025,15 @@
         },
         p(l, o) {
             o[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (l[14][
                         /*i*/
                         l[40]
-                    ] || 0)).toFixed(1) + "") && Mn(n, e);
+                    ] || 0)).toFixed(1) + "") && Bn(n, e);
         },
         d(l) {
             l && (Pe(n), Pe(r));
         }
     };
 }
 
@@ -24069,25 +24069,25 @@
     };
 }
 
 function t1(t) {
     let e, n;
     return {
         c() {
-            e = c0("p"), n = Ft(
+            e = f0("p"), n = Ft(
                 /*loading_text*/
                 t[9]
             ), n0(e, "class", "loading svelte-1yserjw");
         },
         m(r, l) {
-            qe(r, e, l), Q0(e, n);
+            qe(r, e, l), K0(e, n);
         },
         p(r, l) {
             l[0] & /*loading_text*/
-                512 && Mn(
+                512 && Bn(
                     n,
                     /*loading_text*/
                     r[9]
                 );
         },
         d(r) {
             r && Pe(e);
@@ -24107,44 +24107,44 @@
                 /*status*/
                 p[4] === "error" ? 1 : -1
             )
         );
     }
     return ~(n = h(t)) && (r = u[n] = c[n](t)), {
         c() {
-            e = c0("div"), r && r.c(), n0(e, "class", l = "wrap " + /*variant*/
+            e = f0("div"), r && r.c(), n0(e, "class", l = "wrap " + /*variant*/
                 t[8] + " " + /*show_progress*/
-                t[6] + " svelte-1yserjw"), Tn(e, "hide", ! /*status*/
+                t[6] + " svelte-1yserjw"), Fn(e, "hide", ! /*status*/
                 t[4] || /*status*/
                 t[4] === "complete" || /*show_progress*/
-                t[6] === "hidden"), Tn(
+                t[6] === "hidden"), Fn(
                 e,
                 "translucent",
                 /*variant*/
                 t[8] === "center" && /*status*/
                 (t[4] === "pending" || /*status*/
                     t[4] === "error") || /*translucent*/
                 t[11] || /*show_progress*/
                 t[6] === "minimal"
-            ), Tn(
+            ), Fn(
                 e,
                 "generating",
                 /*status*/
                 t[4] === "generating"
-            ), Tn(
+            ), Fn(
                 e,
                 "border",
                 /*border*/
                 t[12]
-            ), x0(
+            ), T0(
                 e,
                 "position",
                 /*absolute*/
                 t[10] ? "absolute" : "static"
-            ), x0(
+            ), T0(
                 e,
                 "padding",
                 /*absolute*/
                 t[10] ? "0" : "var(--size-8) 0"
             );
         },
         m(p, _) {
@@ -24154,47 +24154,47 @@
             let v = n;
             n = h(p), n === v ? ~n && u[n].p(p, _) : (r && (Ph(), Br(u[v], 1, 1, () => {
                     u[v] = null;
                 }), Lh()), ~n ? (r = u[n], r ? r.p(p, _) : (r = u[n] = c[n](p), r.c()), Mr(r, 1), r.m(e, null)) : r = null), (!o || _[0] & /*variant, show_progress*/
                     320 && l !== (l = "wrap " + /*variant*/
                         p[8] + " " + /*show_progress*/
                         p[6] + " svelte-1yserjw")) && n0(e, "class", l), (!o || _[0] & /*variant, show_progress, status, show_progress*/
-                    336) && Tn(e, "hide", ! /*status*/
+                    336) && Fn(e, "hide", ! /*status*/
                     p[4] || /*status*/
                     p[4] === "complete" || /*show_progress*/
                     p[6] === "hidden"), (!o || _[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && Tn(
+                    2384) && Fn(
                     e,
                     "translucent",
                     /*variant*/
                     p[8] === "center" && /*status*/
                     (p[4] === "pending" || /*status*/
                         p[4] === "error") || /*translucent*/
                     p[11] || /*show_progress*/
                     p[6] === "minimal"
                 ), (!o || _[0] & /*variant, show_progress, status*/
-                    336) && Tn(
+                    336) && Fn(
                     e,
                     "generating",
                     /*status*/
                     p[4] === "generating"
                 ), (!o || _[0] & /*variant, show_progress, border*/
-                    4416) && Tn(
+                    4416) && Fn(
                     e,
                     "border",
                     /*border*/
                     p[12]
                 ), _[0] & /*absolute*/
-                1024 && x0(
+                1024 && T0(
                     e,
                     "position",
                     /*absolute*/
                     p[10] ? "absolute" : "static"
                 ), _[0] & /*absolute*/
-                1024 && x0(
+                1024 && T0(
                     e,
                     "padding",
                     /*absolute*/
                     p[10] ? "0" : "var(--size-8) 0"
                 );
         },
         i(p) {
@@ -24289,20 +24289,20 @@
         ne = null,
         re = null,
         pe = 0,
         Me = null,
         Ne, ke = null,
         ce = !0;
     const he = () => {
-        n(0, u = n(26, ne = n(19, oe = null))), n(24, z = performance.now()), n(25, Y = 0), I = !0, ae();
+        n(0, u = n(26, ne = n(19, oe = null))), n(24, z = performance.now()), n(25, Y = 0), I = !0, le();
     };
 
-    function ae() {
+    function le() {
         requestAnimationFrame(() => {
-            n(25, Y = (performance.now() - z) / 1e3), I && ae();
+            n(25, Y = (performance.now() - z) / 1e3), I && le();
         });
     }
 
     function Be() {
         n(25, Y = 0), n(0, u = n(26, ne = n(19, oe = null))), I && (I = !1);
     }
     g6(() => {
@@ -24403,15 +24403,15 @@
         );
     }
 }
 const {
     HtmlTag: M6,
     SvelteComponent: B6,
     action_destroyer: N6,
-    attr: S0,
+    attr: E0,
     binding_callbacks: z6,
     bubble: ta,
     check_outros: R6,
     create_component: O6,
     destroy_component: I6,
     detach: hs,
     element: qh,
@@ -24436,15 +24436,15 @@
     createEventDispatcher: X6
 } = window.__gradio__svelte__internal;
 
 function r1(t) {
     let e, n, r;
     return {
         c() {
-            e = qh("input"), S0(e, "role", "textbox"), S0(e, "tabindex", "-1"), S0(e, "class", "svelte-1q554zi"), zi(
+            e = qh("input"), E0(e, "role", "textbox"), E0(e, "tabindex", "-1"), E0(e, "class", "svelte-1q554zi"), zi(
                 e,
                 "header",
                 /*header*/
                 t[5]
             );
         },
         m(l, o) {
@@ -24629,20 +24629,20 @@
                 /*datatype*/
                 k[6] === "markdown" ? 1 : 2
             )
         );
     }
     return r = v(t), l = _[r] = p[r](t), {
         c() {
-            h && h.c(), e = V6(), n = qh("span"), l.c(), S0(n, "tabindex", "-1"), S0(n, "role", "button"), S0(
+            h && h.c(), e = V6(), n = qh("span"), l.c(), E0(n, "tabindex", "-1"), E0(n, "role", "button"), E0(
                 n,
                 "style",
                 /*styling*/
                 t[4]
-            ), S0(n, "class", "svelte-1q554zi"), zi(
+            ), E0(n, "class", "svelte-1q554zi"), zi(
                 n,
                 "edit",
                 /*edit*/
                 t[2]
             );
         },
         m(k, T) {
@@ -24662,15 +24662,15 @@
         p(k, [T]) {
             /*edit*/
             k[2] ? h ? h.p(k, T) : (h = r1(k), h.c(), h.m(e.parentNode, e)) : h && (h.d(1), h = null);
             let O = r;
             r = v(k), r === O ? _[r].p(k, T) : (H6(), xa(_[O], 1, 1, () => {
                 _[O] = null;
             }), R6(), l = _[r], l ? l.p(k, T) : (l = _[r] = p[r](k), l.c()), Ea(l, 1), l.m(n, null)), (!o || T & /*styling*/
-                16) && S0(
+                16) && E0(
                 n,
                 "style",
                 /*styling*/
                 k[4]
             ), (!o || T & /*edit*/
                 4) && zi(
                 n,
@@ -24829,15 +24829,15 @@
     listen: n7,
     outro_and_destroy_block: r7,
     resize_observer_content_box: s7,
     safe_not_equal: i7,
     set_style: In,
     space: o1,
     text: l7,
-    transition_in: J0,
+    transition_in: Q0,
     transition_out: kr,
     update_keyed_each: a7,
     update_slot_base: Ma
 } = window.__gradio__svelte__internal, {
     onMount: o7,
     tick: ti
 } = window.__gradio__svelte__internal, u7 = (t) => ({}), u1 = (t) => ({});
@@ -24898,15 +24898,15 @@
                     /*visible*/
                     u[8]
                 ), Vh(), e = a7(e, h, c, 1, u, o, n, r.parentNode, r7, m1, r, c1), Gh());
         },
         i(u) {
             if (!l) {
                 for (let h = 0; h < o.length; h += 1)
-                    J0(e[h]);
+                    Q0(e[h]);
                 l = !0;
             }
         },
         o(u) {
             for (let h = 0; h < e.length; h += 1)
                 kr(e[h]);
             l = !1;
@@ -24976,15 +24976,15 @@
                     /*$$scope*/
                     e[20]
                 ),
                 f1
             );
         },
         i(u) {
-            r || (J0(c, u), r = !0);
+            r || (Q0(c, u), r = !0);
         },
         o(u) {
             kr(c, u), r = !1;
         },
         d(u) {
             u && Ki(n), c && c.d(u);
         }
@@ -25093,15 +25093,15 @@
                         /*$$scope*/
                         D[20]
                     ),
                     h1
                 ), /*visible*/
                 D[8].length && /*visible*/
                 D[8][0].data.length ? U ? (U.p(D, E), E[0] & /*visible*/
-                    256 && J0(U, 1)) : (U = d1(D), U.c(), J0(U, 1), U.m(c, null)) : U && (Vh(), kr(U, 1, 1, () => {
+                    256 && Q0(U, 1)) : (U = d1(D), U.c(), Q0(U, 1), U.m(c, null)) : U && (Vh(), kr(U, 1, 1, () => {
                     U = null;
                 }), Gh()), N && N.p && (!v || E[0] & /*$$scope*/
                     1048576) && Ma(
                     N,
                     M,
                     D,
                     /*$$scope*/
@@ -25146,15 +25146,15 @@
                     n,
                     "--bw-svt-avg-row-height",
                     /*average_height*/
                     D[1] + "px"
                 );
         },
         i(D) {
-            v || (J0(P, D), J0(U), J0(N, D), v = !0);
+            v || (Q0(P, D), Q0(U), Q0(N, D), v = !0);
         },
         o(D) {
             kr(P, D), kr(U), kr(N, D), v = !1;
         },
         d(D) {
             D && Ki(e), P && P.d(D), l(), U && U.d(), t[23](null), N && N.d(D), p(), t[25](null), _(), k = !1, T();
         }
@@ -25334,15 +25334,15 @@
 
     function he(Q) {
         l1[Q ? "unshift" : "push"](() => {
             P = Q, n(3, P);
         });
     }
 
-    function ae() {
+    function le() {
         M = this.offsetHeight, n(5, M);
     }
 
     function Be(Q) {
         l1[Q ? "unshift" : "push"](() => {
             R = Q, n(7, R);
         });
@@ -25385,15 +25385,15 @@
         ke,
         D,
         r,
         o,
         l,
         ce,
         he,
-        ae,
+        le,
         Be,
         oe
     ];
 }
 class _7 extends e7 {
     constructor(e) {
         super(), t7(
@@ -25419,39 +25419,39 @@
         return this.$$.ctx[17];
     }
 }
 const {
     ResizeObserverSingleton: b7,
     SvelteComponent: w7,
     action_destroyer: y7,
-    add_flush_callback: M0,
+    add_flush_callback: B0,
     append: it,
     attr: ge,
-    bind: B0,
+    bind: N0,
     binding_callbacks: Hn,
-    check_outros: f0,
-    create_component: I0,
-    destroy_component: L0,
+    check_outros: h0,
+    create_component: L0,
+    destroy_component: H0,
     detach: At,
     element: bt,
     empty: ms,
-    ensure_array_like: T0,
-    group_outros: h0,
+    ensure_array_like: F0,
+    group_outros: d0,
     init: v7,
     insert: St,
-    listen: F0,
-    mount_component: H0,
+    listen: C0,
+    mount_component: P0,
     outro_and_destroy_block: Ri,
     resize_observer_content_box: k7,
     run_all: Wh,
     safe_not_equal: D7,
     set_data: xs,
-    set_style: N0,
+    set_style: z0,
     space: hn,
-    svg_element: z0,
+    svg_element: R0,
     text: Ts,
     toggle_class: kt,
     transition_in: ht,
     transition_out: Bt,
     update_keyed_each: Oi
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: A7,
@@ -25551,15 +25551,15 @@
             edit: !1,
             el: null
         }
     }), {
         key: t,
         first: null,
         c() {
-            n = bt("th"), r = bt("div"), I0(l.$$.fragment), o = hn(), c = bt("div"), u = z0("svg"), h = z0("path"), _ = hn(), ge(h, "d", "M4.49999 0L8.3971 6.75H0.602875L4.49999 0Z"), ge(u, "width", "1em"), ge(u, "height", "1em"), ge(u, "viewBox", "0 0 9 7"), ge(u, "fill", "none"), ge(u, "xmlns", "http://www.w3.org/2000/svg"), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", p = "sort-button " + /*sort_direction*/
+            n = bt("th"), r = bt("div"), L0(l.$$.fragment), o = hn(), c = bt("div"), u = R0("svg"), h = R0("path"), _ = hn(), ge(h, "d", "M4.49999 0L8.3971 6.75H0.602875L4.49999 0Z"), ge(u, "width", "1em"), ge(u, "height", "1em"), ge(u, "viewBox", "0 0 9 7"), ge(u, "fill", "none"), ge(u, "xmlns", "http://www.w3.org/2000/svg"), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", p = "sort-button " + /*sort_direction*/
                 e[18] + " svelte-13e3mz4"), kt(
                 c,
                 "sorted",
                 /*sort_by*/
                 e[19] === /*i*/
                 e[94]
             ), kt(
@@ -25579,29 +25579,29 @@
                     e[18]
                 )), ge(n, "class", "svelte-13e3mz4"), kt(
                 n,
                 "editing",
                 /*header_edit*/
                 e[26] === /*i*/
                 e[94]
-            ), N0(
+            ), z0(
                 n,
                 "width",
                 /*column_widths*/
                 e[12].length ? (
                     /*column_widths*/
                     e[12][
                         /*i*/
                         e[94]
                     ]
                 ) : void 0
             ), this.first = n;
         },
         m(T, O) {
-            St(T, n, O), it(n, r), H0(l, r, null), it(r, o), it(r, c), it(c, u), it(u, h), it(n, _), k = !0;
+            St(T, n, O), it(n, r), P0(l, r, null), it(r, o), it(r, c), it(c, u), it(u, h), it(n, _), k = !0;
         },
         p(T, O) {
             e = T;
             const P = {};
             O[0] & /*_headers*/
                 16777216 && (P.value = /*value*/
                     e[89]), O[0] & /*latex_delimiters*/
@@ -25638,15 +25638,15 @@
                     83886080) && kt(
                     n,
                     "editing",
                     /*header_edit*/
                     e[26] === /*i*/
                     e[94]
                 ), O[0] & /*column_widths, _headers*/
-                16781312 && N0(
+                16781312 && z0(
                     n,
                     "width",
                     /*column_widths*/
                     e[12].length ? (
                         /*column_widths*/
                         e[12][
                             /*i*/
@@ -25658,15 +25658,15 @@
         i(T) {
             k || (ht(l.$$.fragment, T), k = !0);
         },
         o(T) {
             Bt(l.$$.fragment, T), k = !1;
         },
         d(T) {
-            T && At(n), L0(l);
+            T && At(n), H0(l);
         }
     };
 }
 
 function D1(t, e) {
     let n, r, l, o, c = (
             /*j*/
@@ -25712,18 +25712,18 @@
             /*td_binding*/
             e[53](null, c)
         );
     return {
         key: t,
         first: null,
         c() {
-            n = bt("td"), r = bt("div"), I0(l.$$.fragment), o = hn(), ge(r, "class", "cell-wrap svelte-13e3mz4"), ge(n, "tabindex", "-1"), ge(n, "class", "svelte-13e3mz4"), this.first = n;
+            n = bt("td"), r = bt("div"), L0(l.$$.fragment), o = hn(), ge(r, "class", "cell-wrap svelte-13e3mz4"), ge(n, "tabindex", "-1"), ge(n, "class", "svelte-13e3mz4"), this.first = n;
         },
         m(_, v) {
-            St(_, n, v), it(n, r), H0(l, r, null), it(n, o), h(), u = !0;
+            St(_, n, v), it(n, r), P0(l, r, null), it(n, o), h(), u = !0;
         },
         p(_, v) {
             e = _;
             const k = {};
             v[1] & /*max*/
                 16 && (k.value = /*value*/
                     e[89]), v[0] & /*latex_delimiters*/
@@ -25751,15 +25751,15 @@
         i(_) {
             u || (ht(l.$$.fragment, _), u = !0);
         },
         o(_) {
             Bt(l.$$.fragment, _), u = !1;
         },
         d(_) {
-            _ && At(n), L0(l), p();
+            _ && At(n), H0(l), p();
         }
     };
 }
 
 function A1(t) {
     let e, n;
     return {
@@ -25872,15 +25872,15 @@
             t[90]
         ].input !== void 0 && (D.el = /*els*/
             t[23][
                 /*id*/
                 t[90]
             ].input), r = new Qi({
             props: D
-        }), Hn.push(() => B0(r, "value", U)), Hn.push(() => B0(r, "el", M)), r.$on(
+        }), Hn.push(() => N0(r, "value", U)), Hn.push(() => N0(r, "el", M)), r.$on(
             "keydown",
             /*end_header_edit*/
             t[42]
         ), r.$on("dblclick", N);
 
     function E() {
         return (
@@ -25889,15 +25889,15 @@
                 /*i*/
                 t[94]
             )
         );
     }
     return {
         c() {
-            e = bt("th"), n = bt("div"), I0(r.$$.fragment), c = hn(), u = bt("div"), h = z0("svg"), p = z0("path"), v = hn(), ge(p, "d", "M4.49999 0L8.3971 6.75H0.602875L4.49999 0Z"), ge(h, "width", "1em"), ge(h, "height", "1em"), ge(h, "viewBox", "0 0 9 7"), ge(h, "fill", "none"), ge(h, "xmlns", "http://www.w3.org/2000/svg"), ge(h, "class", "svelte-13e3mz4"), ge(u, "class", _ = "sort-button " + /*sort_direction*/
+            e = bt("th"), n = bt("div"), L0(r.$$.fragment), c = hn(), u = bt("div"), h = R0("svg"), p = R0("path"), v = hn(), ge(p, "d", "M4.49999 0L8.3971 6.75H0.602875L4.49999 0Z"), ge(h, "width", "1em"), ge(h, "height", "1em"), ge(h, "viewBox", "0 0 9 7"), ge(h, "fill", "none"), ge(h, "xmlns", "http://www.w3.org/2000/svg"), ge(h, "class", "svelte-13e3mz4"), ge(u, "class", _ = "sort-button " + /*sort_direction*/
                 t[18] + " svelte-13e3mz4"), kt(
                 u,
                 "sorted",
                 /*sort_by*/
                 t[19] === /*i*/
                 t[94]
             ), kt(
@@ -25911,27 +25911,27 @@
                 t[36](
                     /*value*/
                     t[89],
                     /*sort_by*/
                     t[19],
                     /*sort_direction*/
                     t[18]
-                )), N0(e, "width", "var(--cell-width-" + /*i*/
+                )), z0(e, "width", "var(--cell-width-" + /*i*/
                 t[94] + ")"), ge(e, "class", "svelte-13e3mz4"), kt(
                 e,
                 "focus",
                 /*header_edit*/
                 t[26] === /*i*/
                 t[94] || /*selected_header*/
                 t[28] === /*i*/
                 t[94]
             );
         },
         m(C, R) {
-            St(C, e, R), it(e, n), H0(r, n, null), it(n, c), it(n, u), it(u, h), it(h, p), it(e, v), T = !0, O || (P = F0(u, "click", E), O = !0);
+            St(C, e, R), it(e, n), P0(r, n, null), it(n, c), it(n, u), it(u, h), it(h, p), it(e, v), T = !0, O || (P = C0(u, "click", E), O = !0);
         },
         p(C, R) {
             t = C;
             const I = {};
             R[0] & /*latex_delimiters*/
                 32 && (I.latex_delimiters = /*latex_delimiters*/
                     t[5]), R[0] & /*line_breaks*/
@@ -25942,20 +25942,20 @@
                     t[94]), R[0] & /*select_on_focus*/
                 134217728 && (I.select_on_focus = /*select_on_focus*/
                     t[27]), !l && R[0] & /*_headers*/
                 16777216 && (l = !0, I.value = /*_headers*/
                     t[24][
                         /*i*/
                         t[94]
-                    ].value, M0(() => l = !1)), !o && R[0] & /*els, _headers*/
+                    ].value, B0(() => l = !1)), !o && R[0] & /*els, _headers*/
                 25165824 && (o = !0, I.el = /*els*/
                     t[23][
                         /*id*/
                         t[90]
-                    ].input, M0(() => o = !1)), r.$set(I), (!T || R[0] & /*sort_direction*/
+                    ].input, B0(() => o = !1)), r.$set(I), (!T || R[0] & /*sort_direction*/
                     262144 && _ !== (_ = "sort-button " + /*sort_direction*/
                         t[18] + " svelte-13e3mz4")) && ge(u, "class", _), (!T || R[0] & /*sort_direction, sort_by, _headers*/
                     17563648) && kt(
                     u,
                     "sorted",
                     /*sort_by*/
                     t[19] === /*i*/
@@ -25974,15 +25974,15 @@
                             /*value*/
                             t[89],
                             /*sort_by*/
                             t[19],
                             /*sort_direction*/
                             t[18]
                         ))) && ge(e, "aria-sort", k), (!T || R[0] & /*_headers*/
-                    16777216) && N0(e, "width", "var(--cell-width-" + /*i*/
+                    16777216) && z0(e, "width", "var(--cell-width-" + /*i*/
                     t[94] + ")"), (!T || R[0] & /*header_edit, _headers, selected_header*/
                     352321536) && kt(
                     e,
                     "focus",
                     /*header_edit*/
                     t[26] === /*i*/
                     t[94] || /*selected_header*/
@@ -25993,15 +25993,15 @@
         i(C) {
             T || (ht(r.$$.fragment, C), T = !0);
         },
         o(C) {
             Bt(r.$$.fragment, C), T = !1;
         },
         d(C) {
-            C && At(e), L0(r), O = !1, P();
+            C && At(e), H0(r), O = !1, P();
         }
     };
 }
 
 function E1(t, e) {
     let n, r = ! /*hide_columns*/
         e[13].includes(
@@ -26021,17 +26021,17 @@
         p(u, h) {
             e = u, h[0] & /*hide_columns, _headers*/
                 16785408 && (r = ! /*hide_columns*/
                     e[13].includes(
                         /*value*/
                         e[89]
                     )), r ? c ? (c.p(e, h), h[0] & /*hide_columns, _headers*/
-                    16785408 && ht(c, 1)) : (c = S1(e), c.c(), ht(c, 1), c.m(l.parentNode, l)) : c && (h0(), Bt(c, 1, 1, () => {
+                    16785408 && ht(c, 1)) : (c = S1(e), c.c(), ht(c, 1), c.m(l.parentNode, l)) : c && (d0(), Bt(c, 1, 1, () => {
                     c = null;
-                }), f0());
+                }), h0());
         },
         i(u) {
             o || (ht(c), o = !0);
         },
         o(u) {
             Bt(c), o = !1;
         },
@@ -26040,15 +26040,15 @@
         }
     };
 }
 
 function x7(t) {
     let e, n = [],
         r = /* @__PURE__ */ new Map(),
-        l, o = T0(
+        l, o = F0(
             /*_headers*/
             t[24]
         );
     const c = (u) => (
         /*id*/
         u[90]
     );
@@ -26069,18 +26069,18 @@
             for (let p = 0; p < n.length; p += 1)
                 n[p] && n[p].m(e, null);
             l = !0;
         },
         p(u, h) {
             h[0] & /*_headers, sort_by, sort_direction, header_edit, selected_header, latex_delimiters, line_breaks, select_on_focus, els, hide_columns*/
                 495724576 | h[1] & /*get_sort_status, handle_sort, end_header_edit, edit_header*/
-                3616 && (o = T0(
+                3616 && (o = F0(
                     /*_headers*/
                     u[24]
-                ), h0(), n = Oi(n, h, c, 1, u, o, r, e, Ri, E1, null, g1), f0());
+                ), d0(), n = Oi(n, h, c, 1, u, o, r, e, Ri, E1, null, g1), h0());
         },
         i(u) {
             if (!l) {
                 for (let h = 0; h < o.length; h += 1)
                     ht(n[h]);
                 l = !0;
             }
@@ -26140,15 +26140,15 @@
             /*line_breaks*/
             t[11]
         ),
         editable: (
             /*editable*/
             t[6]
         ),
-        edit: Fn(
+        edit: Cn(
             /*editing*/
             t[22],
             [
                 /*index*/
                 t[87],
                 /*j*/
                 t[92]
@@ -26192,15 +26192,15 @@
             t[90]
         ].input !== void 0 && (O.el = /*els*/
             t[23][
                 /*id*/
                 t[90]
             ].input), r = new Qi({
             props: O
-        }), Hn.push(() => B0(r, "value", k)), Hn.push(() => B0(r, "el", T)), r.$on(
+        }), Hn.push(() => N0(r, "value", k)), Hn.push(() => N0(r, "el", T)), r.$on(
             "blur",
             /*blur_handler*/
             t[58]
         );
 
     function P() {
         return (
@@ -26236,39 +26236,39 @@
                 t[92]
             )
         );
     }
     return {
         c() {
             var E, C;
-            e = bt("td"), n = bt("div"), I0(r.$$.fragment), c = hn(), ge(n, "class", "cell-wrap svelte-13e3mz4"), ge(e, "tabindex", "0"), ge(e, "style", u = /*styling*/
+            e = bt("td"), n = bt("div"), L0(r.$$.fragment), c = hn(), ge(n, "class", "cell-wrap svelte-13e3mz4"), ge(e, "tabindex", "0"), ge(e, "style", u = /*styling*/
                 ((C = (E = t[15]) == null ? void 0 : E[
                     /*index*/
                     t[87]
                 ]) == null ? void 0 : C[
                     /*j*/
                     t[92]
-                ]) || ""), ge(e, "class", "svelte-13e3mz4"), kt(e, "focus", Fn(
+                ]) || ""), ge(e, "class", "svelte-13e3mz4"), kt(e, "focus", Cn(
                 /*selected*/
                 t[16],
                 [
                     /*index*/
                     t[87],
                     /*j*/
                     t[92]
                 ]
-            )), N0(e, "width", h);
+            )), z0(e, "width", h);
         },
         m(E, C) {
-            St(E, e, C), it(e, n), H0(r, n, null), it(e, c), p = !0, _ || (v = [
-                F0(e, "touchstart", P, {
+            St(E, e, C), it(e, n), P0(r, n, null), it(e, c), p = !0, _ || (v = [
+                C0(e, "touchstart", P, {
                     passive: !0
                 }),
-                F0(e, "click", U),
-                F0(e, "dblclick", M)
+                C0(e, "click", U),
+                C0(e, "dblclick", M)
             ], _ = !0);
         },
         p(E, C) {
             var z, Y, ne, re;
             t = E;
             const R = {};
             C[0] & /*display_value*/
@@ -26284,15 +26284,15 @@
                 32 && (R.latex_delimiters = /*latex_delimiters*/
                     t[5]), C[0] & /*line_breaks*/
                 2048 && (R.line_breaks = /*line_breaks*/
                     t[11]), C[0] & /*editable*/
                 64 && (R.editable = /*editable*/
                     t[6]), C[0] & /*editing*/
                 4194304 | C[2] & /*index, item*/
-                100663296 && (R.edit = Fn(
+                100663296 && (R.edit = Cn(
                     /*editing*/
                     t[22],
                     [
                         /*index*/
                         t[87],
                         /*j*/
                         t[92]
@@ -26318,32 +26318,32 @@
                 100663296 && (l = !0, R.value = /*data*/
                     t[17][
                         /*index*/
                         t[87]
                     ][
                         /*j*/
                         t[92]
-                    ].value, M0(() => l = !1)), !o && C[0] & /*els*/
+                    ].value, B0(() => l = !1)), !o && C[0] & /*els*/
                 8388608 | C[2] & /*item*/
                 67108864 && (o = !0, R.el = /*els*/
                     t[23][
                         /*id*/
                         t[90]
-                    ].input, M0(() => o = !1)), r.$set(R), (!p || C[0] & /*styling*/
+                    ].input, B0(() => o = !1)), r.$set(R), (!p || C[0] & /*styling*/
                     32768 | C[2] & /*index, item*/
                     100663296 && u !== (u = /*styling*/
                         ((re = (ne = t[15]) == null ? void 0 : ne[
                             /*index*/
                             t[87]
                         ]) == null ? void 0 : re[
                             /*j*/
                             t[92]
                         ]) || "")) && ge(e, "style", u), (!p || C[0] & /*selected*/
                     65536 | C[2] & /*index, item*/
-                    100663296) && kt(e, "focus", Fn(
+                    100663296) && kt(e, "focus", Cn(
                     /*selected*/
                     t[16],
                     [
                         /*index*/
                         t[87],
                         /*j*/
                         t[92]
@@ -26351,24 +26351,24 @@
                 ));
             const I = C[0] & /*styling*/
                 32768 | C[2] & /*index, item*/
                 100663296;
             (C[0] & /*styling*/
                 32768 | C[2] & /*item, index*/
                 100663296 && h !== (h = `var(--cell-width-${/*j*/
-      t[92]})`) || I) && N0(e, "width", h);
+      t[92]})`) || I) && z0(e, "width", h);
         },
         i(E) {
             p || (ht(r.$$.fragment, E), p = !0);
         },
         o(E) {
             Bt(r.$$.fragment, E), p = !1;
         },
         d(E) {
-            E && At(e), L0(r), _ = !1, Wh(v);
+            E && At(e), H0(r), _ = !1, Wh(v);
         }
     };
 }
 
 function T1(t, e) {
     let n, r = ! /*hide_columns*/
         e[13].includes(
@@ -26396,17 +26396,17 @@
                         /*_headers*/
                         e[24][
                             /*j*/
                             e[92]
                         ].value
                     )), r ? c ? (c.p(e, h), h[0] & /*hide_columns, _headers*/
                     16785408 | h[2] & /*item*/
-                    67108864 && ht(c, 1)) : (c = x1(e), c.c(), ht(c, 1), c.m(l.parentNode, l)) : c && (h0(), Bt(c, 1, 1, () => {
+                    67108864 && ht(c, 1)) : (c = x1(e), c.c(), ht(c, 1), c.m(l.parentNode, l)) : c && (d0(), Bt(c, 1, 1, () => {
                     c = null;
-                }), f0());
+                }), h0());
         },
         i(u) {
             o || (ht(c), o = !0);
         },
         o(u) {
             Bt(c), o = !1;
         },
@@ -26415,15 +26415,15 @@
         }
     };
 }
 
 function T7(t) {
     let e, n = [],
         r = /* @__PURE__ */ new Map(),
-        l, o = T0(
+        l, o = F0(
             /*item*/
             t[88]
         );
     const c = (u) => (
         /*id*/
         u[90]
     );
@@ -26450,18 +26450,18 @@
                 n[p] && n[p].m(e, null);
             l = !0;
         },
         p(u, h) {
             h[0] & /*styling, selected, display_value, latex_delimiters, line_breaks, editable, editing, datatype, clear_on_focus, data, els, parent, hide_columns, _headers*/
                 1136912481 | h[1] & /*start_edit, handle_cell_click*/
                 320 | h[2] & /*index, item*/
-                100663296 && (o = T0(
+                100663296 && (o = F0(
                     /*item*/
                     u[88]
-                ), h0(), n = Oi(n, h, c, 1, u, o, r, e, Ri, T1, null, _1), f0()), (!l || h[2] & /*index*/
+                ), d0(), n = Oi(n, h, c, 1, u, o, r, e, Ri, T1, null, _1), h0()), (!l || h[2] & /*index*/
                     33554432) && kt(
                     e,
                     "row_odd",
                     /*index*/
                     u[87] % 2 === 0
                 );
         },
@@ -26535,20 +26535,20 @@
         t[17] !== void 0 && (p.items = /*data*/
             t[17]), /*table_height*/
         t[32] !== void 0 && (p.actual_height = /*table_height*/
             t[32]), /*scrollbar_width*/
         t[33] !== void 0 && (p.table_scrollbar_width = /*scrollbar_width*/
             t[33]), e = new _7({
             props: p
-        }), Hn.push(() => B0(e, "items", c)), Hn.push(() => B0(e, "actual_height", u)), Hn.push(() => B0(e, "table_scrollbar_width", h)), {
+        }), Hn.push(() => N0(e, "items", c)), Hn.push(() => N0(e, "actual_height", u)), Hn.push(() => N0(e, "table_scrollbar_width", h)), {
             c() {
-                I0(e.$$.fragment);
+                L0(e.$$.fragment);
             },
             m(_, v) {
-                H0(e, _, v), o = !0;
+                P0(e, _, v), o = !0;
             },
             p(_, v) {
                 const k = {};
                 v[0] & /*height*/
                     1024 && (k.max_height = /*height*/
                         _[10]), v[1] & /*selected_index*/
                     8 && (k.selected = /*selected_index*/
@@ -26556,28 +26556,28 @@
                     1607460963 | v[2] & /*index, item*/
                     100663296 | v[3] & /*$$scope*/
                     16 && (k.$$scope = {
                         dirty: v,
                         ctx: _
                     }), !n && v[0] & /*data*/
                     131072 && (n = !0, k.items = /*data*/
-                        _[17], M0(() => n = !1)), !r && v[1] & /*table_height*/
+                        _[17], B0(() => n = !1)), !r && v[1] & /*table_height*/
                     2 && (r = !0, k.actual_height = /*table_height*/
-                        _[32], M0(() => r = !1)), !l && v[1] & /*scrollbar_width*/
+                        _[32], B0(() => r = !1)), !l && v[1] & /*scrollbar_width*/
                     4 && (l = !0, k.table_scrollbar_width = /*scrollbar_width*/
-                        _[33], M0(() => l = !1)), e.$set(k);
+                        _[33], B0(() => l = !1)), e.$set(k);
             },
             i(_) {
                 o || (ht(e.$$.fragment, _), o = !0);
             },
             o(_) {
                 Bt(e.$$.fragment, _), o = !1;
             },
             d(_) {
-                L0(e, _);
+                H0(e, _);
             }
         }
     );
 }
 
 function F1(t) {
     let e, n, r, l = (
@@ -26594,21 +26594,21 @@
         },
         m(c, u) {
             St(c, e, u), l && l.m(e, null), it(e, n), o && o.m(e, null), r = !0;
         },
         p(c, u) {
             /*row_count*/
             c[4][1] === "dynamic" ? l ? (l.p(c, u), u[0] & /*row_count*/
-                    16 && ht(l, 1)) : (l = C1(c), l.c(), ht(l, 1), l.m(e, n)) : l && (h0(), Bt(l, 1, 1, () => {
+                    16 && ht(l, 1)) : (l = C1(c), l.c(), ht(l, 1), l.m(e, n)) : l && (d0(), Bt(l, 1, 1, () => {
                     l = null;
-                }), f0()), /*col_count*/
+                }), h0()), /*col_count*/
                 c[3][1] === "dynamic" ? o ? (o.p(c, u), u[0] & /*col_count*/
-                    8 && ht(o, 1)) : (o = M1(c), o.c(), ht(o, 1), o.m(e, null)) : o && (h0(), Bt(o, 1, 1, () => {
+                    8 && ht(o, 1)) : (o = M1(c), o.c(), ht(o, 1), o.m(e, null)) : o && (d0(), Bt(o, 1, 1, () => {
                     o = null;
-                }), f0());
+                }), h0());
         },
         i(c) {
             r || (ht(l), ht(o), r = !0);
         },
         o(c) {
             Bt(l), Bt(o), r = !1;
         },
@@ -26633,18 +26633,18 @@
         }
     }), n.$on(
         "click",
         /*click_handler_2*/
         t[73]
     ), {
         c() {
-            e = bt("span"), I0(n.$$.fragment), ge(e, "class", "button-wrap svelte-13e3mz4");
+            e = bt("span"), L0(n.$$.fragment), ge(e, "class", "button-wrap svelte-13e3mz4");
         },
         m(l, o) {
-            St(l, e, o), H0(n, e, null), r = !0;
+            St(l, e, o), P0(n, e, null), r = !0;
         },
         p(l, o) {
             const c = {};
             o[0] & /*i18n*/
                 512 | o[3] & /*$$scope*/
                 16 && (c.$$scope = {
                     dirty: o,
@@ -26654,28 +26654,28 @@
         i(l) {
             r || (ht(n.$$.fragment, l), r = !0);
         },
         o(l) {
             Bt(n.$$.fragment, l), r = !1;
         },
         d(l) {
-            l && At(e), L0(n);
+            l && At(e), H0(n);
         }
     };
 }
 
 function C7(t) {
     let e, n, r, l = (
             /*i18n*/
             t[9]("dataframe.new_row") + ""
         ),
         o;
     return {
         c() {
-            e = z0("svg"), n = z0("path"), r = hn(), o = Ts(l), ge(n, "fill", "currentColor"), ge(n, "d", "M24.59 16.59L17 24.17V4h-2v20.17l-7.59-7.58L6 18l10 10l10-10l-1.41-1.41z"), ge(e, "xmlns", "http://www.w3.org/2000/svg"), ge(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), ge(e, "aria-hidden", "true"), ge(e, "role", "img"), ge(e, "width", "1em"), ge(e, "height", "1em"), ge(e, "preserveAspectRatio", "xMidYMid meet"), ge(e, "viewBox", "0 0 32 32"), ge(e, "class", "svelte-13e3mz4");
+            e = R0("svg"), n = R0("path"), r = hn(), o = Ts(l), ge(n, "fill", "currentColor"), ge(n, "d", "M24.59 16.59L17 24.17V4h-2v20.17l-7.59-7.58L6 18l10 10l10-10l-1.41-1.41z"), ge(e, "xmlns", "http://www.w3.org/2000/svg"), ge(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), ge(e, "aria-hidden", "true"), ge(e, "role", "img"), ge(e, "width", "1em"), ge(e, "height", "1em"), ge(e, "preserveAspectRatio", "xMidYMid meet"), ge(e, "viewBox", "0 0 32 32"), ge(e, "class", "svelte-13e3mz4");
         },
         m(c, u) {
             St(c, e, u), it(e, n), St(c, r, u), St(c, o, u);
         },
         p(c, u) {
             u[0] & /*i18n*/
                 512 && l !== (l = /*i18n*/
@@ -26702,18 +26702,18 @@
         }
     }), n.$on(
         "click",
         /*click_handler_3*/
         t[74]
     ), {
         c() {
-            e = bt("span"), I0(n.$$.fragment), ge(e, "class", "button-wrap svelte-13e3mz4");
+            e = bt("span"), L0(n.$$.fragment), ge(e, "class", "button-wrap svelte-13e3mz4");
         },
         m(l, o) {
-            St(l, e, o), H0(n, e, null), r = !0;
+            St(l, e, o), P0(n, e, null), r = !0;
         },
         p(l, o) {
             const c = {};
             o[0] & /*i18n*/
                 512 | o[3] & /*$$scope*/
                 16 && (c.$$scope = {
                     dirty: o,
@@ -26723,28 +26723,28 @@
         i(l) {
             r || (ht(n.$$.fragment, l), r = !0);
         },
         o(l) {
             Bt(n.$$.fragment, l), r = !1;
         },
         d(l) {
-            l && At(e), L0(n);
+            l && At(e), H0(n);
         }
     };
 }
 
 function M7(t) {
     let e, n, r, l = (
             /*i18n*/
             t[9]("dataframe.new_column") + ""
         ),
         o;
     return {
         c() {
-            e = z0("svg"), n = z0("path"), r = hn(), o = Ts(l), ge(n, "fill", "currentColor"), ge(n, "d", "m18 6l-1.43 1.393L24.15 15H4v2h20.15l-7.58 7.573L18 26l10-10L18 6z"), ge(e, "xmlns", "http://www.w3.org/2000/svg"), ge(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), ge(e, "aria-hidden", "true"), ge(e, "role", "img"), ge(e, "width", "1em"), ge(e, "height", "1em"), ge(e, "preserveAspectRatio", "xMidYMid meet"), ge(e, "viewBox", "0 0 32 32"), ge(e, "class", "svelte-13e3mz4");
+            e = R0("svg"), n = R0("path"), r = hn(), o = Ts(l), ge(n, "fill", "currentColor"), ge(n, "d", "m18 6l-1.43 1.393L24.15 15H4v2h20.15l-7.58 7.573L18 26l10-10L18 6z"), ge(e, "xmlns", "http://www.w3.org/2000/svg"), ge(e, "xmlns:xlink", "http://www.w3.org/1999/xlink"), ge(e, "aria-hidden", "true"), ge(e, "role", "img"), ge(e, "width", "1em"), ge(e, "height", "1em"), ge(e, "preserveAspectRatio", "xMidYMid meet"), ge(e, "viewBox", "0 0 32 32"), ge(e, "class", "svelte-13e3mz4");
         },
         m(c, u) {
             St(c, e, u), it(e, n), St(c, r, u), St(c, o, u);
         },
         p(c, u) {
             u[0] & /*i18n*/
                 512 && l !== (l = /*i18n*/
@@ -26768,39 +26768,39 @@
             t[2] && y1(t)
         ),
         z = (
             /*label*/
             t[1] && /*label*/
             t[1].length !== 0 && v1(t)
         ),
-        Y = T0(
+        Y = F0(
             /*_headers*/
             t[24]
         );
     const ne = (ce) => (
         /*id*/
         ce[90]
     );
     for (let ce = 0; ce < Y.length; ce += 1) {
         let he = w1(t, Y, ce),
-            ae = ne(he);
-        p.set(ae, h[ce] = k1(ae, he));
+            le = ne(he);
+        p.set(le, h[ce] = k1(le, he));
     }
-    let re = T0(
+    let re = F0(
         /*max*/
         t[35]
     );
     const pe = (ce) => (
         /*id*/
         ce[90]
     );
     for (let ce = 0; ce < re.length; ce += 1) {
         let he = b1(t, re, ce),
-            ae = pe(he);
-        O.set(ae, T[ce] = D1(ae, he));
+            le = pe(he);
+        O.set(le, T[ce] = D1(le, he));
     }
 
     function Me(ce) {
         t[69](ce);
     }
     let Ne = {
         flex: !1,
@@ -26818,15 +26818,15 @@
             ctx: t
         }
     };
     /*dragging*/
     t[29] !== void 0 && (Ne.dragging = /*dragging*/
         t[29]), M = new $3({
         props: Ne
-    }), Hn.push(() => B0(M, "dragging", Me)), M.$on(
+    }), Hn.push(() => N0(M, "dragging", Me)), M.$on(
         "load",
         /*load_handler*/
         t[70]
     );
     let ke = (
         /*editable*/
         t[6] && F1(t)
@@ -26835,20 +26835,20 @@
         c() {
             e = bt("div"), I && I.c(), n = hn(), r = bt("div"), l = bt("table"), z && z.c(), o = hn(), c = bt("thead"), u = bt("tr");
             for (let ce = 0; ce < h.length; ce += 1)
                 h[ce].c();
             _ = hn(), v = bt("tbody"), k = bt("tr");
             for (let ce = 0; ce < T.length; ce += 1)
                 T[ce].c();
-            U = hn(), I0(M.$$.fragment), D = hn(), ke && ke.c(), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", "svelte-13e3mz4"), ge(k, "class", "svelte-13e3mz4"), ge(l, "class", "svelte-13e3mz4"), kt(
+            U = hn(), L0(M.$$.fragment), D = hn(), ke && ke.c(), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", "svelte-13e3mz4"), ge(k, "class", "svelte-13e3mz4"), ge(l, "class", "svelte-13e3mz4"), kt(
                 l,
                 "fixed-layout",
                 /*column_widths*/
                 t[12].length != 0
-            ), ge(r, "class", "table-wrap svelte-13e3mz4"), N0(
+            ), ge(r, "class", "table-wrap svelte-13e3mz4"), z0(
                 r,
                 "height",
                 /*table_height*/
                 t[32] + "px"
             ), ge(r, "role", "grid"), ge(r, "tabindex", "0"), kt(
                 r,
                 "dragging",
@@ -26861,43 +26861,43 @@
                 /*label*/
                 t[1] && /*label*/
                 t[1].length !== 0
             );
         },
         m(ce, he) {
             St(ce, e, he), I && I.m(e, null), it(e, n), it(e, r), it(r, l), z && z.m(l, null), it(l, o), it(l, c), it(c, u);
-            for (let ae = 0; ae < h.length; ae += 1)
-                h[ae] && h[ae].m(u, null);
+            for (let le = 0; le < h.length; le += 1)
+                h[le] && h[le].m(u, null);
             it(l, _), it(l, v), it(v, k);
-            for (let ae = 0; ae < T.length; ae += 1)
-                T[ae] && T[ae].m(k, null);
+            for (let le = 0; le < T.length; le += 1)
+                T[le] && T[le].m(k, null);
             P = k7.observe(
                 l,
                 /*table_1_elementresizecontentbox_handler*/
                 t[54].bind(l)
-            ), t[55](l), it(r, U), H0(M, r, null), t[71](r), it(e, D), ke && ke.m(e, null), E = !0, C || (R = [
-                F0(
+            ), t[55](l), it(r, U), P0(M, r, null), t[71](r), it(e, D), ke && ke.m(e, null), E = !0, C || (R = [
+                C0(
                     window,
                     "click",
                     /*handle_click_outside*/
                     t[45]
                 ),
-                F0(
+                C0(
                     window,
                     "touchstart",
                     /*handle_click_outside*/
                     t[45]
                 ),
-                F0(
+                C0(
                     window,
                     "resize",
                     /*resize_handler*/
                     t[52]
                 ),
-                F0(
+                C0(
                     r,
                     "keydown",
                     /*keydown_handler*/
                     t[72]
                 ),
                 y7(mm.call(null, e))
             ], C = !0);
@@ -26906,59 +26906,59 @@
             /*label*/
             ce[1] && /*label*/
                 ce[1].length !== 0 && /*show_label*/
                 ce[2] ? I ? I.p(ce, he) : (I = y1(ce), I.c(), I.m(e, n)) : I && (I.d(1), I = null), /*label*/
                 ce[1] && /*label*/
                 ce[1].length !== 0 ? z ? z.p(ce, he) : (z = v1(ce), z.c(), z.m(l, o)) : z && (z.d(1), z = null), he[0] & /*_headers, sort_by, sort_direction, header_edit, column_widths, latex_delimiters, line_breaks*/
                 84678688 | he[1] & /*get_sort_status*/
-                32 && (Y = T0(
+                32 && (Y = F0(
                     /*_headers*/
                     ce[24]
-                ), h0(), h = Oi(h, he, ne, 1, ce, Y, p, u, Ri, k1, null, w1), f0()), he[0] & /*cells, latex_delimiters, line_breaks, datatype*/
+                ), d0(), h = Oi(h, he, ne, 1, ce, Y, p, u, Ri, k1, null, w1), h0()), he[0] & /*cells, latex_delimiters, line_breaks, datatype*/
                 1050657 | he[1] & /*max*/
-                16 && (re = T0(
+                16 && (re = F0(
                     /*max*/
                     ce[35]
-                ), h0(), T = Oi(T, he, pe, 1, ce, re, O, k, Ri, D1, null, b1), f0()), (!E || he[0] & /*column_widths*/
+                ), d0(), T = Oi(T, he, pe, 1, ce, re, O, k, Ri, D1, null, b1), h0()), (!E || he[0] & /*column_widths*/
                     4096) && kt(
                     l,
                     "fixed-layout",
                     /*column_widths*/
                     ce[12].length != 0
                 );
-            const ae = {};
+            const le = {};
             he[0] & /*root*/
-                256 && (ae.root = /*root*/
+                256 && (le.root = /*root*/
                     ce[8]), he[0] & /*height, data, styling, selected, display_value, latex_delimiters, line_breaks, editable, editing, datatype, clear_on_focus, els, parent, hide_columns, _headers, sort_by, sort_direction, header_edit, selected_header, select_on_focus, label*/
                 1607461987 | he[1] & /*selected_index, table_height, scrollbar_width*/
                 14 | he[3] & /*$$scope*/
-                16 && (ae.$$scope = {
+                16 && (le.$$scope = {
                     dirty: he,
                     ctx: ce
                 }), !N && he[0] & /*dragging*/
-                536870912 && (N = !0, ae.dragging = /*dragging*/
-                    ce[29], M0(() => N = !1)), M.$set(ae), (!E || he[1] & /*table_height*/
-                    2) && N0(
+                536870912 && (N = !0, le.dragging = /*dragging*/
+                    ce[29], B0(() => N = !1)), M.$set(le), (!E || he[1] & /*table_height*/
+                    2) && z0(
                     r,
                     "height",
                     /*table_height*/
                     ce[32] + "px"
                 ), (!E || he[0] & /*dragging*/
                     536870912) && kt(
                     r,
                     "dragging",
                     /*dragging*/
                     ce[29]
                 ), (!E || he[0] & /*wrap*/
                     128) && kt(r, "no-wrap", ! /*wrap*/
                     ce[7]), /*editable*/
                 ce[6] ? ke ? (ke.p(ce, he), he[0] & /*editable*/
-                    64 && ht(ke, 1)) : (ke = F1(ce), ke.c(), ht(ke, 1), ke.m(e, null)) : ke && (h0(), Bt(ke, 1, 1, () => {
+                    64 && ht(ke, 1)) : (ke = F1(ce), ke.c(), ht(ke, 1), ke.m(e, null)) : ke && (d0(), Bt(ke, 1, 1, () => {
                     ke = null;
-                }), f0()), (!E || he[0] & /*label*/
+                }), h0()), (!E || he[0] & /*label*/
                     2) && kt(
                     e,
                     "label",
                     /*label*/
                     ce[1] && /*label*/
                     ce[1].length !== 0
                 );
@@ -26981,15 +26981,15 @@
         },
         d(ce) {
             ce && At(e), I && I.d(), z && z.d();
             for (let he = 0; he < h.length; he += 1)
                 h[he].d();
             for (let he = 0; he < T.length; he += 1)
                 T[he].d();
-            P(), t[55](null), L0(M), t[71](null), ke && ke.d(), C = !1, Wh(R);
+            P(), t[55](null), H0(M), t[71](null), ke && ke.d(), C = !1, Wh(R);
         }
     };
 }
 
 function B1(t, e) {
     return t ?? e();
 }
@@ -27096,15 +27096,15 @@
         {
             styling: I = null
         } = e,
         z;
     const Y = A7();
     let ne = !1;
     const re = (q, d) => mr([
-        ae,
+        le,
         "optionalAccess",
         (g) => g[q],
         "optionalAccess",
         (g) => g[d],
         "optionalAccess",
         (g) => g.value
     ]);
@@ -27152,21 +27152,21 @@
     }
     let ke = Me(h),
         ce;
 
     function he() {
         n(24, ke = Me(h)), n(50, ce = h.slice()), oe();
     }
-    let ae = [
+    let le = [
             []
         ],
         Be;
     async function oe() {
         Y("change", {
-            data: ae.map((q) => q.map(({
+            data: le.map((q) => q.map(({
                 value: d
             }) => d)),
             headers: ke.map((q) => q.value),
             metadata: T ? null : {
                 display_value: R,
                 styling: I
             }
@@ -27182,39 +27182,39 @@
             if (g === "des")
                 return "descending";
         }
         return "none";
     }
 
     function de(q) {
-        return ae.reduce(
+        return le.reduce(
             (d, g, Z) => {
                 const y = g.reduce((B, ze, fe) => q === ze.id ? fe : B, -1);
                 return y === -1 ? d : [Z, y];
             },
             [-1, -1]
         );
     }
     async function V(q, d) {
-        !T || Fn(ne, [q, d]) || n(22, ne = [q, d]);
+        !T || Cn(ne, [q, d]) || n(22, ne = [q, d]);
     }
 
     function ee(q, d) {
         const g = {
                 ArrowRight: [0, 1],
                 ArrowLeft: [0, -1],
                 ArrowDown: [1, 0],
                 ArrowUp: [-1, 0]
             } [q],
             Z = d[0] + g[0],
             y = d[1] + g[1];
         if (Z < 0 && y <= 0)
             n(28, Ue = y), n(16, C = !1);
         else {
-            const B = mr([ae, "access", (ze) => ze[Z], "optionalAccess", (ze) => ze[y]]);
+            const B = mr([le, "access", (ze) => ze[Z], "optionalAccess", (ze) => ze[y]]);
             n(16, C = B ? [Z, y] : C);
         }
     }
     let we = !1;
     async function ve(q) {
         if (Ue !== !1 && Ie === !1)
             switch (q.key) {
@@ -27250,99 +27250,99 @@
                 if (!T)
                     break;
                 q.preventDefault(), n(22, ne = !1);
                 break;
             case "Enter":
                 if (!T)
                     break;
-                q.preventDefault(), q.shiftKey ? (Re(d), await ni(), n(16, C = [d + 1, g])) : Fn(ne, [d, g]) ? (n(22, ne = !1), await ni(), n(16, C = [d, g])) : n(22, ne = [d, g]);
+                q.preventDefault(), q.shiftKey ? (Re(d), await ni(), n(16, C = [d + 1, g])) : Cn(ne, [d, g]) ? (n(22, ne = !1), await ni(), n(16, C = [d, g])) : n(22, ne = [d, g]);
                 break;
             case "Backspace":
                 if (!T)
                     break;
-                ne || (q.preventDefault(), n(17, ae[d][g].value = "", ae));
+                ne || (q.preventDefault(), n(17, le[d][g].value = "", le));
                 break;
             case "Delete":
                 if (!T)
                     break;
-                ne || (q.preventDefault(), n(17, ae[d][g].value = "", ae));
+                ne || (q.preventDefault(), n(17, le[d][g].value = "", le));
                 break;
             case "Tab":
                 let Z = q.shiftKey ? -1 : 1,
-                    y = ae[d][g + Z],
+                    y = le[d][g + Z],
                     B = mr([
-                        ae,
+                        le,
                         "optionalAccess",
                         (ze) => ze[d + Z],
                         "optionalAccess",
                         (ze) => ze[Z > 0 ? 0 : ke.length - 1]
                     ]);
                 (y || B) && (q.preventDefault(), n(16, C = y ? [d, g + Z] : [d + Z, Z > 0 ? 0 : ke.length - 1])), n(22, ne = !1);
                 break;
             default:
                 if (!T)
                     break;
-                (!ne || ne && Fn(ne, [d, g])) && q.key.length === 1 && (n(25, we = !0), n(22, ne = [d, g]));
+                (!ne || ne && Cn(ne, [d, g])) && q.key.length === 1 && (n(25, we = !0), n(22, ne = [d, g]));
         }
     }
     async function $(q, d) {
-        Fn(ne, [q, d]) || (n(26, Ie = !1), n(28, Ue = !1), n(22, ne = !1), n(16, C = [q, d]), await ni(), Ee.focus());
+        Cn(ne, [q, d]) || (n(26, Ie = !1), n(28, Ue = !1), n(22, ne = !1), n(16, C = [q, d]), await ni(), Ee.focus());
     }
     let xe, Se;
 
     function We(q) {
         typeof Se != "number" || Se !== q ? (n(18, xe = "asc"), n(19, Se = q)) : xe === "asc" ? n(18, xe = "des") : xe === "des" && n(18, xe = "asc");
     }
     let Ie, Xe = !1,
         Ue = !1;
     async function zt(q, d = !1) {
         !T || _[1] !== "dynamic" || Ie === q || (n(16, C = !1), n(28, Ue = q), n(26, Ie = q), n(27, Xe = d));
     }
 
-    function Bn(q) {
+    function Nn(q) {
         if (T)
             switch (q.key) {
                 case "Escape":
                 case "Enter":
                 case "Tab":
                     q.preventDefault(), n(16, C = !1), n(28, Ue = Ie), n(26, Ie = !1), Ee.focus();
                     break;
             }
     }
     async function Re(q) {
         if (Ee.focus(), v[1] === "dynamic") {
-            if (ae.length === 0) {
+            if (le.length === 0) {
                 n(49, p = [Array(h.length).fill("")]);
                 return;
             }
-            ae.splice(q ? q + 1 : ae.length, 0, Array(ae[0].length).fill(0).map((d, g) => {
+            le.splice(q ? q + 1 : le.length, 0, Array(le[0].length).fill(0).map((d, g) => {
                 const Z = Qr();
                 return n(23, pe[Z] = {
                     cell: null,
                     input: null
                 }, pe), {
                     id: Z,
                     value: ""
                 };
-            })), n(17, ae), n(49, p), n(51, Be), n(16, C = [q ? q + 1 : ae.length - 1, 0]);
+            })), n(17, le), n(49, p), n(51, Be), n(16, C = [q ? q + 1 : le.length - 1, 0]);
         }
     }
     async function $t() {
         if (Ee.focus(), _[1] === "dynamic") {
-            for (let q = 0; q < ae.length; q++) {
+            for (let q = 0; q < le.length; q++) {
                 const d = Qr();
                 n(23, pe[d] = {
                     cell: null,
                     input: null
-                }, pe), ae[q].push({
+                }, pe), le[q].push({
                     id: d,
                     value: ""
                 });
             }
-            h.push(`Header ${h.length + 1}`), n(17, ae), n(49, p), n(51, Be), n(48, h), await ni(), requestAnimationFrame(() => {
+            h.push(`Header ${h.length + 1}`), n(17, le), n(49, p), n(51, Be), n(48, h), await ni(), requestAnimationFrame(() => {
                 zt(h.length - 1, !0);
                 const q = Ee.querySelectorAll("tbody")[1].offsetWidth;
                 Ee.querySelectorAll("table")[1].scrollTo({
                     left: q
                 });
             });
         }
@@ -27390,98 +27390,98 @@
                 Ee.style.setProperty(`--cell-width-${d}`, `${q[d] - Ce / q.length}px`);
     }
     let et = M,
         Ce = 0;
 
     function Le(q, d, g, Z, y) {
         let B = null;
-        if (C && C[0] in ae && C[1] in ae[C[0]] && (B = ae[C[0]][C[1]].id), typeof Z != "number" || !y)
+        if (C && C[0] in le && C[1] in le[C[0]] && (B = le[C[0]][C[1]].id), typeof Z != "number" || !y)
             return;
         const ze = [...Array(q.length).keys()];
         if (y === "asc")
             ze.sort((De, ue) => q[De][Z].value < q[ue][Z].value ? -1 : 1);
         else if (y === "des")
             ze.sort((De, ue) => q[De][Z].value > q[ue][Z].value ? -1 : 1);
         else
             return;
         const fe = [...q],
             pt = d ? [...d] : null,
-            kn = g ? [...g] : null;
+            Dn = g ? [...g] : null;
         if (ze.forEach((De, ue) => {
-                q[ue] = fe[De], d && pt && (d[ue] = pt[De]), g && kn && (g[ue] = kn[De]);
-            }), n(17, ae), n(49, p), n(51, Be), B) {
+                q[ue] = fe[De], d && pt && (d[ue] = pt[De]), g && Dn && (g[ue] = Dn[De]);
+            }), n(17, le), n(49, p), n(51, Be), B) {
             const [De, ue] = de(B);
             n(16, C = [De, ue]);
         }
     }
     let tt = !1;
     S7(() => {
         const q = new IntersectionObserver((d, g) => {
             d.forEach((Z) => {
-                Z.isIntersecting && !tt && (Oe(), n(17, ae), n(49, p), n(51, Be)), tt = Z.isIntersecting;
+                Z.isIntersecting && !tt && (Oe(), n(17, le), n(49, p), n(51, Be)), tt = Z.isIntersecting;
             });
         });
         return q.observe(Ee), () => {
             q.disconnect();
         };
     });
     const Rt = () => Oe();
 
     function Jt(q, d) {
         Hn[q ? "unshift" : "push"](() => {
             Fe[d] = q, n(20, Fe);
         });
     }
 
-    function Nn() {
+    function kn() {
         var q;
         z = (q = b7.entries.get(this)) == null ? void 0 : q.contentRect, n(21, z);
     }
 
     function It(q) {
         Hn[q ? "unshift" : "push"](() => {
             me = q, n(31, me);
         });
     }
 
     function Ze(q, d, g) {
-        t.$$.not_equal(ae[d][g].value, q) && (ae[d][g].value = q, n(17, ae), n(49, p), n(51, Be));
+        t.$$.not_equal(le[d][g].value, q) && (le[d][g].value = q, n(17, le), n(49, p), n(51, Be));
     }
 
-    function ie(q, d) {
+    function ae(q, d) {
         t.$$.not_equal(pe[d].input, q) && (pe[d].input = q, n(23, pe));
     }
-    const Gt = () => (n(25, we = !1), Ee.focus()),
-        rr = (q, d) => V(q, d),
+    const Ut = () => (n(25, we = !1), Ee.focus()),
+        s0 = (q, d) => V(q, d),
         Pn = (q, d) => $(q, d),
         sr = (q, d) => V(q, d);
 
-    function s0(q, d) {
+    function i0(q, d) {
         t.$$.not_equal(ke[d].value, q) && (ke[d].value = q, n(24, ke));
     }
 
     function wt(q, d) {
         t.$$.not_equal(pe[d].input, q) && (pe[d].input = q, n(23, pe));
     }
     const qn = (q) => zt(q),
         Ir = (q) => We(q);
 
     function jt(q) {
-        ae = q, n(17, ae), n(49, p), n(51, Be);
+        le = q, n(17, le), n(49, p), n(51, Be);
     }
 
     function en(q) {
         et = q, n(32, et);
     }
 
     function dn(q) {
         Ce = q, n(33, Ce);
     }
 
-    function p0(q) {
+    function g0(q) {
         K = q, n(29, K);
     }
     const ir = (q) => Ct(z7(q.detail.data));
 
     function lr(q) {
         Hn[q ? "unshift" : "push"](() => {
             Ee = q, n(30, Ee);
@@ -27498,20 +27498,20 @@
             const [q, d] = C;
             !isNaN(q) && !isNaN(d) && Y("select", {
                 index: [q, d],
                 value: re(q, d)
             });
         }
         t.$$.dirty[1] & /*headers, old_headers*/
-            655360 && (Fn(h, ce) || he()), t.$$.dirty[1] & /*values, old_val*/
-            1310720 && (Fn(p, Be) || (n(17, ae = Ne(p)), n(51, Be = p))), t.$$.dirty[0] & /*data*/
-            131072 && ae && oe(), t.$$.dirty[0] & /*data*/
-            131072 && n(35, r = ye(ae)), t.$$.dirty[0] & /*cells*/
+            655360 && (Cn(h, ce) || he()), t.$$.dirty[1] & /*values, old_val*/
+            1310720 && (Cn(p, Be) || (n(17, le = Ne(p)), n(51, Be = p))), t.$$.dirty[0] & /*data*/
+            131072 && le && oe(), t.$$.dirty[0] & /*data*/
+            131072 && n(35, r = ye(le)), t.$$.dirty[0] & /*cells*/
             1048576 && Fe[0] && Oe(), t.$$.dirty[0] & /*data, display_value, styling, sort_by, sort_direction*/
-            966656 && Le(ae, R, I, Se, xe), t.$$.dirty[0] & /*selected*/
+            966656 && Le(le, R, I, Se, xe), t.$$.dirty[0] & /*selected*/
             65536 && n(34, l = !!C && C[0]);
     }, [
         o,
         c,
         u,
         _,
         v,
@@ -27523,15 +27523,15 @@
         M,
         N,
         D,
         E,
         R,
         I,
         C,
-        ae,
+        le,
         xe,
         Se,
         Fe,
         z,
         ne,
         pe,
         ke,
@@ -27548,42 +27548,42 @@
         r,
         Q,
         V,
         ve,
         $,
         We,
         zt,
-        Bn,
+        Nn,
         Re,
         $t,
         Ot,
         Ct,
         Oe,
         h,
         p,
         ce,
         Be,
         Rt,
         Jt,
-        Nn,
+        kn,
         It,
         Ze,
-        ie,
-        Gt,
-        rr,
+        ae,
+        Ut,
+        s0,
         Pn,
         sr,
-        s0,
+        i0,
         wt,
         qn,
         Ir,
         jt,
         en,
         dn,
-        p0,
+        g0,
         ir,
         lr,
         ar,
         Lr,
         Qt
     ];
 }
@@ -27906,15 +27906,15 @@
     get_all_dirty_from_scope: _g,
     get_slot_changes: bg,
     init: wg,
     insert: yg,
     null_to_empty: R1,
     safe_not_equal: vg,
     set_style: li,
-    toggle_class: w0,
+    toggle_class: y0,
     transition_in: kg,
     transition_out: Dg,
     update_slot_base: Ag
 } = window.__gradio__svelte__internal;
 
 function Sg(t) {
     let e, n, r = `calc(min(${/*min_width*/
@@ -27937,30 +27937,30 @@
                 e,
                 "id",
                 /*elem_id*/
                 t[3]
             ), ii(e, "class", n = R1(
                 /*elem_classes*/
                 t[4].join(" ")
-            ) + " svelte-1m1obck"), w0(
+            ) + " svelte-1m1obck"), y0(
                 e,
                 "gap",
                 /*gap*/
                 t[1]
-            ), w0(
+            ), y0(
                 e,
                 "compact",
                 /*variant*/
                 t[6] === "compact"
-            ), w0(
+            ), y0(
                 e,
                 "panel",
                 /*variant*/
                 t[6] === "panel"
-            ), w0(e, "hide", ! /*visible*/
+            ), y0(e, "hide", ! /*visible*/
                 t[5]), li(
                 e,
                 "flex-grow",
                 /*scale*/
                 t[0]
             ), li(e, "min-width", r);
         },
@@ -27993,33 +27993,33 @@
                     /*elem_id*/
                     u[3]
                 ), (!l || h & /*elem_classes*/
                     16 && n !== (n = R1(
                         /*elem_classes*/
                         u[4].join(" ")
                     ) + " svelte-1m1obck")) && ii(e, "class", n), (!l || h & /*elem_classes, gap*/
-                    18) && w0(
+                    18) && y0(
                     e,
                     "gap",
                     /*gap*/
                     u[1]
                 ), (!l || h & /*elem_classes, variant*/
-                    80) && w0(
+                    80) && y0(
                     e,
                     "compact",
                     /*variant*/
                     u[6] === "compact"
                 ), (!l || h & /*elem_classes, variant*/
-                    80) && w0(
+                    80) && y0(
                     e,
                     "panel",
                     /*variant*/
                     u[6] === "panel"
                 ), (!l || h & /*elem_classes, visible*/
-                    48) && w0(e, "hide", ! /*visible*/
+                    48) && y0(e, "hide", ! /*visible*/
                     u[5]), h & /*scale*/
                 1 && li(
                     e,
                     "flex-grow",
                     /*scale*/
                     u[0]
                 ), h & /*min_width*/
@@ -28542,15 +28542,15 @@
         });
     }
 }
 const {
     SvelteComponent: Pg,
     append: P1,
     assign: qg,
-    attr: y0,
+    attr: v0,
     binding_callbacks: Ug,
     check_outros: Gg,
     create_component: ao,
     destroy_component: oo,
     detach: Ia,
     element: q1,
     flush: on,
@@ -28683,22 +28683,22 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), {
         c() {
-            v && v.c(), e = j1(), n = q1("label"), ao(r.$$.fragment), l = j1(), o = q1("input"), y0(o, "data-testid", "textbox"), y0(o, "type", "text"), y0(o, "class", "scroll-hide svelte-2jrh70"), y0(
+            v && v.c(), e = j1(), n = q1("label"), ao(r.$$.fragment), l = j1(), o = q1("input"), v0(o, "data-testid", "textbox"), v0(o, "type", "text"), v0(o, "class", "scroll-hide svelte-2jrh70"), v0(
                     o,
                     "placeholder",
                     /*placeholder*/
                     t[6]
                 ), o.disabled = c = ! /*interactive*/
-                t[11], y0(o, "dir", u = /*rtl*/
-                    t[12] ? "rtl" : "ltr"), y0(n, "class", "svelte-2jrh70"), Kg(n, "container", s8);
+                t[11], v0(o, "dir", u = /*rtl*/
+                    t[12] ? "rtl" : "ltr"), v0(n, "class", "svelte-2jrh70"), Kg(n, "container", s8);
         },
         m(k, T) {
             v && v.m(k, T), La(k, e, T), La(k, n, T), uo(r, n, null), P1(n, l), P1(n, o), G1(
                 o,
                 /*value*/
                 t[0]
             ), t[17](o), h = !0, p || (_ = [
@@ -28726,24 +28726,24 @@
             T & /*show_label*/
                 128 && (O.show_label = /*show_label*/
                     k[7]), T & /*$$scope, label*/
                 1048580 && (O.$$scope = {
                     dirty: T,
                     ctx: k
                 }), r.$set(O), (!h || T & /*placeholder*/
-                    64) && y0(
+                    64) && v0(
                     o,
                     "placeholder",
                     /*placeholder*/
                     k[6]
                 ), (!h || T & /*interactive*/
                     2048 && c !== (c = ! /*interactive*/
                         k[11])) && (o.disabled = c), (!h || T & /*rtl*/
                     4096 && u !== (u = /*rtl*/
-                        k[12] ? "rtl" : "ltr")) && y0(o, "dir", u), T & /*value*/
+                        k[12] ? "rtl" : "ltr")) && v0(o, "dir", u), T & /*value*/
                 1 && o.value !== /*value*/
                 k[0] && G1(
                     o,
                     /*value*/
                     k[0]
                 );
         },
@@ -29394,15 +29394,15 @@
     init: c9,
     insert: us,
     listen: Ha,
     prevent_default: f9,
     run_all: h9,
     safe_not_equal: d9,
     set_data: m9,
-    set_style: v0,
+    set_style: k0,
     space: Pa,
     text: p9,
     toggle_class: Zn,
     transition_in: la,
     transition_out: $1
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: g9
@@ -29422,26 +29422,26 @@
     for (let h = 0; h < c.length; h += 1)
         u[h] = nf(ef(t, c, h));
     return {
         c() {
             e = Hi("ul");
             for (let h = 0; h < u.length; h += 1)
                 u[h].c();
-            bn(e, "class", "options svelte-yuohum"), bn(e, "role", "listbox"), v0(
+            bn(e, "class", "options svelte-yuohum"), bn(e, "role", "listbox"), k0(
                 e,
                 "top",
                 /*top*/
                 t[9]
-            ), v0(
+            ), k0(
                 e,
                 "bottom",
                 /*bottom*/
                 t[10]
-            ), v0(e, "max-height", `calc(${/*max_height*/
-      t[11]}px - var(--window-padding))`), v0(
+            ), k0(e, "max-height", `calc(${/*max_height*/
+      t[11]}px - var(--window-padding))`), k0(
                 e,
                 "width",
                 /*input_width*/
                 t[8] + "px"
             );
         },
         m(h, p) {
@@ -29466,29 +29466,29 @@
                     u[_] ? u[_].p(v, p) : (u[_] = nf(v), u[_].c(), u[_].m(e, null));
                 }
                 for (; _ < u.length; _ += 1)
                     u[_].d(1);
                 u.length = c.length;
             }
             p & /*top*/
-                512 && v0(
+                512 && k0(
                     e,
                     "top",
                     /*top*/
                     h[9]
                 ), p & /*bottom*/
-                1024 && v0(
+                1024 && k0(
                     e,
                     "bottom",
                     /*bottom*/
                     h[10]
                 ), p & /*max_height*/
-                2048 && v0(e, "max-height", `calc(${/*max_height*/
+                2048 && k0(e, "max-height", `calc(${/*max_height*/
       h[11]}px - var(--window-padding))`), p & /*input_width*/
-                256 && v0(
+                256 && k0(
                     e,
                     "width",
                     /*input_width*/
                     h[8] + "px"
                 );
         },
         i(h) {
@@ -29843,21 +29843,21 @@
     append: Kn,
     attr: qt,
     binding_callbacks: S9,
     check_outros: Pi,
     create_component: ps,
     destroy_component: gs,
     destroy_each: E9,
-    detach: d0,
+    detach: m0,
     element: $n,
     ensure_array_like: rf,
     group_outros: qi,
     init: x9,
-    insert: m0,
-    listen: u0,
+    insert: p0,
+    listen: c0,
     mount_component: _s,
     prevent_default: sf,
     run_all: co,
     safe_not_equal: T9,
     set_data: fo,
     set_input_value: lf,
     space: Ar,
@@ -29881,26 +29881,26 @@
         c() {
             e = ho(
                 /*label*/
                 t[0]
             );
         },
         m(n, r) {
-            m0(n, e, r);
+            p0(n, e, r);
         },
         p(n, r) {
             r[0] & /*label*/
                 1 && fo(
                     e,
                     /*label*/
                     n[0]
                 );
         },
         d(n) {
-            n && d0(e);
+            n && m0(e);
         }
     };
 }
 
 function B9(t) {
     let e = (
             /*s*/
@@ -29908,23 +29908,23 @@
         ),
         n;
     return {
         c() {
             n = ho(e);
         },
         m(r, l) {
-            m0(r, n, l);
+            p0(r, n, l);
         },
         p(r, l) {
             l[0] & /*selected_indices*/
                 4096 && e !== (e = /*s*/
                     r[40] + "") && fo(n, e);
         },
         d(r) {
-            r && d0(n);
+            r && m0(n);
         }
     };
 }
 
 function N9(t) {
     let e = (
             /*choices_names*/
@@ -29935,26 +29935,26 @@
         ),
         n;
     return {
         c() {
             n = ho(e);
         },
         m(r, l) {
-            m0(r, n, l);
+            p0(r, n, l);
         },
         p(r, l) {
             l[0] & /*choices_names, selected_indices*/
                 36864 && e !== (e = /*choices_names*/
                     r[15][
                         /*s*/
                         r[40]
                     ] + "") && fo(n, e);
         },
         d(r) {
-            r && d0(n);
+            r && m0(n);
         }
     };
 }
 
 function of(t) {
     let e, n, r, l, o, c;
     n = new Zh({});
@@ -29982,17 +29982,17 @@
     return {
         c() {
             e = $n("div"), ps(n.$$.fragment), qt(e, "class", "token-remove svelte-xtjjyg"), qt(e, "role", "button"), qt(e, "tabindex", "0"), qt(e, "title", r = /*i18n*/
                 t[9]("common.remove") + " " + /*s*/
                 t[40]);
         },
         m(p, _) {
-            m0(p, e, _), _s(n, e, null), l = !0, o || (c = [
-                u0(e, "click", sf(u)),
-                u0(e, "keydown", sf(h))
+            p0(p, e, _), _s(n, e, null), l = !0, o || (c = [
+                c0(e, "click", sf(u)),
+                c0(e, "keydown", sf(h))
             ], o = !0);
         },
         p(p, _) {
             t = p, (!l || _[0] & /*i18n, selected_indices*/
                 4608 && r !== (r = /*i18n*/
                     t[9]("common.remove") + " " + /*s*/
                     t[40])) && qt(e, "title", r);
@@ -30000,15 +30000,15 @@
         i(p) {
             l || (Wt(n.$$.fragment, p), l = !0);
         },
         o(p) {
             yn(n.$$.fragment, p), l = !1;
         },
         d(p) {
-            p && d0(e), gs(n), o = !1, co(c);
+            p && m0(e), gs(n), o = !1, co(c);
         }
     };
 }
 
 function uf(t) {
     let e, n, r, l;
 
@@ -30021,15 +30021,15 @@
         h = ! /*disabled*/
         t[4] && of(t);
     return {
         c() {
             e = $n("div"), n = $n("span"), u.c(), r = Ar(), h && h.c(), qt(n, "class", "svelte-xtjjyg"), qt(e, "class", "token svelte-xtjjyg");
         },
         m(p, _) {
-            m0(p, e, _), Kn(e, n), u.m(n, null), Kn(e, r), h && h.m(e, null), l = !0;
+            p0(p, e, _), Kn(e, n), u.m(n, null), Kn(e, r), h && h.m(e, null), l = !0;
         },
         p(p, _) {
             c === (c = o(p)) && u ? u.p(p, _) : (u.d(1), u = c(p), u && (u.c(), u.m(n, null))), /*disabled*/
                 p[4] ? h && (qi(), yn(h, 1, 1, () => {
                     h = null;
                 }), Pi()) : h ? (h.p(p, _), _[0] & /*disabled*/
                     16 && Wt(h, 1)) : (h = of(p), h.c(), Wt(h, 1), h.m(e, null));
@@ -30037,30 +30037,30 @@
         i(p) {
             l || (Wt(h), l = !0);
         },
         o(p) {
             yn(h), l = !1;
         },
         d(p) {
-            p && d0(e), u.d(), h && h.d();
+            p && m0(e), u.d(), h && h.d();
         }
     };
 }
 
 function cf(t) {
     let e, n, r, l, o = (
         /*selected_indices*/
         t[12].length > 0 && ff(t)
     );
     return r = new Q8({}), {
         c() {
             o && o.c(), e = Ar(), n = $n("span"), ps(r.$$.fragment), qt(n, "class", "icon-wrap svelte-xtjjyg");
         },
         m(c, u) {
-            o && o.m(c, u), m0(c, e, u), m0(c, n, u), _s(r, n, null), l = !0;
+            o && o.m(c, u), p0(c, e, u), p0(c, n, u), _s(r, n, null), l = !0;
         },
         p(c, u) {
             /*selected_indices*/
             c[12].length > 0 ? o ? (o.p(c, u), u[0] & /*selected_indices*/
                 4096 && Wt(o, 1)) : (o = ff(c), o.c(), Wt(o, 1), o.m(e.parentNode, e)) : o && (qi(), yn(o, 1, 1, () => {
                 o = null;
             }), Pi());
@@ -30068,35 +30068,35 @@
         i(c) {
             l || (Wt(o), Wt(r.$$.fragment, c), l = !0);
         },
         o(c) {
             yn(o), yn(r.$$.fragment, c), l = !1;
         },
         d(c) {
-            c && (d0(e), d0(n)), o && o.d(c), gs(r);
+            c && (m0(e), m0(n)), o && o.d(c), gs(r);
         }
     };
 }
 
 function ff(t) {
     let e, n, r, l, o, c;
     return n = new Zh({}), {
         c() {
             e = $n("div"), ps(n.$$.fragment), qt(e, "role", "button"), qt(e, "tabindex", "0"), qt(e, "class", "token-remove remove-all svelte-xtjjyg"), qt(e, "title", r = /*i18n*/
                 t[9]("common.clear"));
         },
         m(u, h) {
-            m0(u, e, h), _s(n, e, null), l = !0, o || (c = [
-                u0(
+            p0(u, e, h), _s(n, e, null), l = !0, o || (c = [
+                c0(
                     e,
                     "click",
                     /*remove_all*/
                     t[21]
                 ),
-                u0(
+                c0(
                     e,
                     "keydown",
                     /*keydown_handler_1*/
                     t[36]
                 )
             ], o = !0);
         },
@@ -30108,15 +30108,15 @@
         i(u) {
             l || (Wt(n.$$.fragment, u), l = !0);
         },
         o(u) {
             yn(n.$$.fragment, u), l = !1;
         },
         d(u) {
-            u && d0(e), gs(n), o = !1, co(c);
+            u && m0(e), gs(n), o = !1, co(c);
         }
     };
 }
 
 function z9(t) {
     let e, n, r, l, o, c, u, h, p, _, v, k, T, O, P;
     n = new G8({
@@ -30203,47 +30203,47 @@
                     e,
                     "container",
                     /*container*/
                     t[6]
                 );
         },
         m(E, C) {
-            m0(E, e, C), _s(n, e, null), Kn(e, r), Kn(e, l), Kn(l, o);
+            p0(E, e, C), _s(n, e, null), Kn(e, r), Kn(e, l), Kn(l, o);
             for (let R = 0; R < M.length; R += 1)
                 M[R] && M[R].m(o, null);
             Kn(o, c), Kn(o, u), Kn(u, h), lf(
                 h,
                 /*input_text*/
                 t[10]
             ), t[34](h), Kn(u, _), D && D.m(u, null), Kn(l, v), _s(k, l, null), T = !0, O || (P = [
-                u0(
+                c0(
                     h,
                     "input",
                     /*input_input_handler*/
                     t[33]
                 ),
-                u0(
+                c0(
                     h,
                     "keydown",
                     /*handle_key_down*/
                     t[23]
                 ),
-                u0(
+                c0(
                     h,
                     "keyup",
                     /*keyup_handler*/
                     t[35]
                 ),
-                u0(
+                c0(
                     h,
                     "blur",
                     /*handle_blur*/
                     t[18]
                 ),
-                u0(
+                c0(
                     h,
                     "focus",
                     /*handle_focus*/
                     t[22]
                 )
             ], O = !0);
         },
@@ -30334,15 +30334,15 @@
         o(E) {
             yn(n.$$.fragment, E), M = M.filter(Boolean);
             for (let C = 0; C < M.length; C += 1)
                 yn(M[C]);
             yn(D), yn(k.$$.fragment, E), T = !1;
         },
         d(E) {
-            E && d0(e), gs(n), E9(M, E), t[34](null), D && D.d(), gs(k), O = !1, co(P);
+            E && m0(e), gs(n), E9(M, E), t[34](null), D && D.d(), gs(k), O = !1, co(P);
         }
     };
 }
 
 function R9(t, e, n) {
     let {
         label: r
@@ -30404,15 +30404,15 @@
         Y.includes($) ? Me($) : Ne($), n(10, N = "");
     }
 
     function he($) {
         n(12, Y = []), n(10, N = ""), $.preventDefault();
     }
 
-    function ae($) {
+    function le($) {
         n(11, I = p.map((xe, Se) => Se)), (h === null || Y.length < h) && n(14, E = !0), re("focus");
     }
 
     function Be($) {
         n(14, [E, z] = D9($, z, I), E, (n(16, z), n(3, p), n(27, _), n(10, N), n(28, D), n(7, O), n(11, I))), $.key === "Enter" && (z !== null ? ce(z) : O && (Ne(N), n(10, N = ""))), $.key === "Backspace" && N === "" && n(12, Y = [...Y.slice(0, -1)]), Y.length === h && (n(14, E = !1), n(16, z = null));
     }
 
@@ -30477,15 +30477,15 @@
         C,
         z,
         re,
         pe,
         Me,
         ke,
         he,
-        ae,
+        le,
         Be,
         o,
         u,
         c,
         _,
         D,
         R,
@@ -30530,20 +30530,20 @@
     attr: je,
     create_component: Qh,
     destroy_component: Kh,
     detach: yi,
     element: Jn,
     init: L9,
     insert: vi,
-    listen: k0,
+    listen: D0,
     mount_component: $h,
     run_all: H9,
     safe_not_equal: P9,
     set_data: q9,
-    set_input_value: D0,
+    set_input_value: A0,
     space: br,
     text: U9,
     to_number: Sr,
     transition_in: ed,
     transition_out: td
 } = window.__gradio__svelte__internal, {
     createEventDispatcher: G9
@@ -30642,74 +30642,74 @@
                 D,
                 "max",
                 /*max*/
                 t[6]
             ), je(D, "class", "svelte-1dsqogo"), je(k, "class", "range-slider svelte-1dsqogo");
         },
         m(I, z) {
-            vi(I, e, z), gn(e, n), $h(r, n, null), gn(n, l), gn(n, o), gn(o, c), D0(
+            vi(I, e, z), gn(e, n), $h(r, n, null), gn(n, l), gn(n, o), gn(o, c), A0(
                 c,
                 /*selected_max*/
                 t[1]
-            ), gn(o, h), gn(o, p), D0(
+            ), gn(o, h), gn(o, p), A0(
                 p,
                 /*selected_min*/
                 t[0]
-            ), vi(I, v, z), vi(I, k, z), gn(k, T), gn(k, O), gn(k, P), gn(k, U), gn(k, M), D0(
+            ), vi(I, v, z), vi(I, k, z), gn(k, T), gn(k, O), gn(k, P), gn(k, U), gn(k, M), A0(
                 M,
                 /*selected_min*/
                 t[0]
-            ), gn(k, N), gn(k, D), D0(
+            ), gn(k, N), gn(k, D), A0(
                 D,
                 /*selected_max*/
                 t[1]
             ), E = !0, C || (R = [
-                k0(
+                D0(
                     c,
                     "input",
                     /*input0_input_handler*/
                     t[10]
                 ),
-                k0(
+                D0(
                     p,
                     "input",
                     /*input1_input_handler*/
                     t[11]
                 ),
-                k0(
+                D0(
                     M,
                     "change",
                     /*input2_change_input_handler*/
                     t[12]
                 ),
-                k0(
+                D0(
                     M,
                     "input",
                     /*input2_change_input_handler*/
                     t[12]
                 ),
-                k0(
+                D0(
                     M,
                     "input",
                     /*handle_min_change*/
                     t[8]
                 ),
-                k0(
+                D0(
                     D,
                     "change",
                     /*input3_change_input_handler*/
                     t[13]
                 ),
-                k0(
+                D0(
                     D,
                     "input",
                     /*input3_change_input_handler*/
                     t[13]
                 ),
-                k0(
+                D0(
                     D,
                     "input",
                     /*handle_max_change*/
                     t[9]
                 )
             ], C = !0);
         },
@@ -30735,15 +30735,15 @@
                     64) && je(
                     c,
                     "max",
                     /*max*/
                     I[6]
                 ), z & /*selected_max*/
                 2 && Sr(c.value) !== /*selected_max*/
-                I[1] && D0(
+                I[1] && A0(
                     c,
                     /*selected_max*/
                     I[1]
                 ), (!E || z & /*label*/
                     4 && _ !== (_ = `min input for ${/*label*/
       I[2]}`)) && je(p, "aria-label", _), (!E || z & /*min*/
                     32) && je(
@@ -30755,15 +30755,15 @@
                     64) && je(
                     p,
                     "max",
                     /*max*/
                     I[6]
                 ), z & /*selected_min*/
                 1 && Sr(p.value) !== /*selected_min*/
-                I[0] && D0(
+                I[0] && A0(
                     p,
                     /*selected_min*/
                     I[0]
                 ), (!E || z & /*rangeLine*/
                     128) && je(
                     P,
                     "style",
@@ -30778,15 +30778,15 @@
                 ), (!E || z & /*max*/
                     64) && je(
                     M,
                     "max",
                     /*max*/
                     I[6]
                 ), z & /*selected_min*/
-                1 && D0(
+                1 && A0(
                     M,
                     /*selected_min*/
                     I[0]
                 ), (!E || z & /*min*/
                     32) && je(
                     D,
                     "min",
@@ -30795,15 +30795,15 @@
                 ), (!E || z & /*max*/
                     64) && je(
                     D,
                     "max",
                     /*max*/
                     I[6]
                 ), z & /*selected_max*/
-                2 && D0(
+                2 && A0(
                     D,
                     /*selected_max*/
                     I[1]
                 );
         },
         i(I) {
             E || (ed(r.$$.fragment, I), E = !0);
@@ -30952,23 +30952,23 @@
     assign: Q9,
     bind: K9,
     binding_callbacks: $9,
     check_outros: qa,
     create_component: Xt,
     destroy_component: Yt,
     destroy_each: e_,
-    detach: R0,
+    detach: O0,
     empty: nd,
     ensure_array_like: hf,
     get_spread_object: t_,
     get_spread_update: n_,
     globals: r_,
     group_outros: Ua,
     init: s_,
-    insert: O0,
+    insert: I0,
     mount_component: Zt,
     safe_not_equal: i_,
     space: Nr,
     transition_in: dt,
     transition_out: Dt
 } = window.__gradio__svelte__internal, {
     Boolean: l_
@@ -31203,15 +31203,15 @@
             t[7].allow && pf(t)
         );
     return {
         c() {
             l && l.c(), e = Nr(), o && o.c(), n = nd();
         },
         m(c, u) {
-            l && l.m(c, u), O0(c, e, u), o && o.m(c, u), O0(c, n, u), r = !0;
+            l && l.m(c, u), I0(c, e, u), o && o.m(c, u), I0(c, n, u), r = !0;
         },
         p(c, u) {
             /*search_columns*/
             c[9].primary_column ? l ? (l.p(c, u), u[0] & /*search_columns*/
                     512 && dt(l, 1)) : (l = mf(c), l.c(), dt(l, 1), l.m(e.parentNode, e)) : l && (Ua(), Dt(l, 1, 1, () => {
                     l = null;
                 }), qa()), /*select_columns_config*/
@@ -31223,15 +31223,15 @@
         i(c) {
             r || (dt(l), dt(o), r = !0);
         },
         o(c) {
             Dt(l), Dt(o), r = !1;
         },
         d(c) {
-            c && (R0(e), R0(n)), l && l.d(c), o && o.d(c);
+            c && (O0(e), O0(n)), l && l.d(c), o && o.d(c);
         }
     };
 }
 
 function h_(t) {
     let e, n;
 
@@ -31496,27 +31496,27 @@
         );
     }
     return e = u(t), n = c[e] = o[e](t), {
         c() {
             n.c(), r = nd();
         },
         m(h, p) {
-            c[e].m(h, p), O0(h, r, p), l = !0;
+            c[e].m(h, p), I0(h, r, p), l = !0;
         },
         p(h, p) {
             n.p(h, p);
         },
         i(h) {
             l || (dt(n), l = !0);
         },
         o(h) {
             Dt(n), l = !1;
         },
         d(h) {
-            h && R0(r), c[e].d(h);
+            h && O0(r), c[e].d(h);
         }
     };
 }
 
 function g_(t) {
     let e, n, r, l = hf(
             /*non_checkbox_filter_columns*/
@@ -31561,15 +31561,15 @@
             for (let u = 0; u < o.length; u += 1)
                 o[u].c();
             e = Nr(), Xt(n.$$.fragment);
         },
         m(u, h) {
             for (let p = 0; p < o.length; p += 1)
                 o[p] && o[p].m(u, h);
-            O0(u, e, h), Zt(n, u, h), r = !0;
+            I0(u, e, h), Zt(n, u, h), r = !0;
         },
         p(u, h) {
             if (h[0] & /*non_checkbox_filter_columns, gradio, loading_status, filter_values*/
                 16945152) {
                 l = hf(
                     /*non_checkbox_filter_columns*/
                     u[24]
@@ -31602,15 +31602,15 @@
         o(u) {
             o = o.filter(l_);
             for (let h = 0; h < o.length; h += 1)
                 Dt(o[h]);
             Dt(n.$$.fragment, u), r = !1;
         },
         d(u) {
-            u && R0(e), e_(o, u), Yt(n, u);
+            u && O0(e), e_(o, u), Yt(n, u);
         }
     };
 }
 
 function __(t) {
     let e, n;
     return e = new K7({
@@ -31671,15 +31671,15 @@
             }
         }
     }), {
         c() {
             Xt(e.$$.fragment), n = Nr(), Xt(r.$$.fragment);
         },
         m(o, c) {
-            Zt(e, o, c), O0(o, n, c), Zt(r, o, c), l = !0;
+            Zt(e, o, c), I0(o, n, c), Zt(r, o, c), l = !0;
         },
         p(o, c) {
             const u = {};
             c[0] & /*select_columns_config, gradio, headers, hide_columns, loading_status, default_selection, search_columns, search_value*/
                 824193 | c[1] & /*$$scope*/
                 33554432 && (u.$$scope = {
                     dirty: c,
@@ -31696,15 +31696,15 @@
         i(o) {
             l || (dt(e.$$.fragment, o), dt(r.$$.fragment, o), l = !0);
         },
         o(o) {
             Dt(e.$$.fragment, o), Dt(r.$$.fragment, o), l = !1;
         },
         d(o) {
-            o && R0(n), Yt(e, o), Yt(r, o);
+            o && O0(n), Yt(e, o), Yt(r, o);
         }
     };
 }
 
 function w_(t) {
     let e, n, r, l;
     const o = [{
@@ -31808,15 +31808,15 @@
         /*select_handler*/
         t[43]
     ), {
         c() {
             Xt(e.$$.fragment), n = Nr(), Xt(r.$$.fragment);
         },
         m(u, h) {
-            Zt(e, u, h), O0(u, n, h), Zt(r, u, h), l = !0;
+            Zt(e, u, h), I0(u, n, h), Zt(r, u, h), l = !0;
         },
         p(u, h) {
             const p = h[0] & /*gradio, loading_status*/
                 36864 ? n_(o, [
                     h[0] & /*gradio*/
                     4096 && {
                         autoscroll: (
@@ -31886,15 +31886,15 @@
         i(u) {
             l || (dt(e.$$.fragment, u), dt(r.$$.fragment, u), l = !0);
         },
         o(u) {
             Dt(e.$$.fragment, u), Dt(r.$$.fragment, u), l = !1;
         },
         d(u) {
-            u && R0(n), Yt(e, u), Yt(r, u);
+            u && O0(n), Yt(e, u), Yt(r, u);
         }
     };
 }
 
 function y_(t) {
     let e, n, r, l, o, c;
     return e = new Ii({
@@ -31921,15 +31921,15 @@
             }
         }
     }), {
         c() {
             Xt(e.$$.fragment), n = Nr(), Xt(r.$$.fragment), l = Nr(), Xt(o.$$.fragment);
         },
         m(u, h) {
-            Zt(e, u, h), O0(u, n, h), Zt(r, u, h), O0(u, l, h), Zt(o, u, h), c = !0;
+            Zt(e, u, h), I0(u, n, h), Zt(r, u, h), I0(u, l, h), Zt(o, u, h), c = !0;
         },
         p(u, h) {
             const p = {};
             h[0] & /*bool_checkboxgroup_label, gradio, loading_status, filter_values, select_columns_config, headers, hide_columns, default_selection, search_columns, search_value*/
                 955267 | h[1] & /*$$scope*/
                 33554432 && (p.$$scope = {
                     dirty: h,
@@ -31946,20 +31946,20 @@
         i(u) {
             c || (dt(e.$$.fragment, u), dt(r.$$.fragment, u), dt(o.$$.fragment, u), c = !0);
         },
         o(u) {
             Dt(e.$$.fragment, u), Dt(r.$$.fragment, u), Dt(o.$$.fragment, u), c = !1;
         },
         d(u) {
-            u && (R0(n), R0(l)), Yt(e, u), Yt(r, u), Yt(o, u);
+            u && (O0(n), O0(l)), Yt(e, u), Yt(r, u), Yt(o, u);
         }
     };
 }
 
-function A0(t) {
+function S0(t) {
     let e, n = t[0],
         r = 1;
     for (; r < t.length;) {
         const l = t[r],
             o = t[r + 1];
         if (r += 2, (l === "optionalAccess" || l === "optionalCall") && n == null)
             return;
@@ -32033,42 +32033,42 @@
         latex_delimiters: ne
     } = e, {
         height: re = void 0
     } = e, {
         loading_status: pe
     } = e, {
         interactive: Me
-    } = e, Ne, ke = u.headers.map((K) => K), ce = u.data.map((K) => K), he, ae, Be, oe = [], Q = null, de = E.default_selection.length ? E.default_selection : ke;
+    } = e, Ne, ke = u.headers.map((K) => K), ce = u.data.map((K) => K), he, le, Be, oe = [], Q = null, de = E.default_selection.length ? E.default_selection : ke;
     async function V(K) {
         let ye = K || u;
         n(20, Ne = ke), n(23, Be = ce ? [...ce] : []);
         const Fe = Ne.filter((me) => de.includes(me)),
             Ee = Fe.map((me) => Ne.indexOf(me));
-        n(20, Ne = Fe), n(23, Be = Be.map((me) => Ee.map((Oe) => me[Oe]))), n(21, he = A0([
+        n(20, Ne = Fe), n(23, Be = Be.map((me) => Ee.map((Oe) => me[Oe]))), n(21, he = S0([
             ye,
             "optionalAccess",
             (me) => me.metadata,
             "optionalAccess",
             (me) => me.display_value
         ]) ? [
-            ...A0([
+            ...S0([
                 ye,
                 "optionalAccess",
                 (me) => me.metadata,
                 "optionalAccess",
                 (me) => me.display_value
             ])
-        ] : null), n(22, ae = A0([
+        ] : null), n(22, le = S0([
             ye,
             "optionalAccess",
             (me) => me.metadata,
             "optionalAccess",
             (me) => me.styling
         ]) ? [
-            ...A0([
+            ...S0([
                 ye,
                 "optionalAccess",
                 (me) => me.metadata,
                 "optionalAccess",
                 (me) => me.styling
             ])
         ] : null), await o_(), Y.dispatch("change"), _ || Y.dispatch("input");
@@ -32101,27 +32101,27 @@
             Oe = new Array(K.length).fill(!1);
         let et = !1;
         for (let Ce = 0; Ce < K.length; Ce++) {
             let Le = Array(),
                 tt = Array();
             for (let Rt = 0; Rt < me.length; Rt++) {
                 let Jt = me[Rt],
-                    Nn = ye.indexOf(Fe.primary_column);
+                    kn = ye.indexOf(Fe.primary_column);
                 const It = Jt.indexOf(":");
                 if (It !== -1) {
-                    const ie = Jt.substring(0, It);
-                    if (!Fe.secondary_columns.length || !Fe.secondary_columns.includes(ie)) {
-                        et || Y.dispatch("warning", `Column ${ie} not found in secondary columns of search_columns`), et = !0;
+                    const Ut = Jt.substring(0, It);
+                    if (!Fe.secondary_columns.length || !Fe.secondary_columns.includes(Ut)) {
+                        et || Y.dispatch("warning", `Column ${Ut} not found in secondary columns of search_columns`), et = !0;
                         continue;
                     }
-                    const Gt = ye.indexOf(ie);
-                    Gt !== -1 && (Nn = Gt, Jt = Jt.substring(It + 1).trim());
+                    const s0 = ye.indexOf(Ut);
+                    s0 !== -1 && (kn = s0, Jt = Jt.substring(It + 1).trim());
                 }
                 const Ze = It !== -1 ? tt : Le;
-                K[Ce][Nn].toString().toLowerCase().includes(Jt.toLowerCase()) ? Ze.push(!0) : Ze.push(!1);
+                (K[Ce][kn] === null ? "" : K[Ce][kn].toString()).toLowerCase().includes(Jt.toLowerCase()) ? Ze.push(!0) : Ze.push(!1);
             }
             Le.length && !tt.length ? Oe[Ce] = Le.some((Rt) => Rt) : tt.length && !Le.length ? Oe[Ce] = tt.every((Rt) => !!Rt) : Le.length && tt.length && (Oe[Ce] = Le.some((Rt) => Rt) && tt.every((Rt) => !!Rt));
         }
         return Oe;
     }
 
     function $(K) {
@@ -32136,41 +32136,41 @@
     }
 
     function Se(K, ye, Fe) {
         n(23, Be = ee(ce, K)), n(23, Be = xe(Be, ke, ye, R, Fe)), Be.length === 0 && n(23, Be = [Array(K.length).fill("")]);
     }
     V(), a_(() => {
         n(27, _ = !1);
-    }), (Array.isArray(u) && A0([u, "optionalAccess", (K) => K[0], "optionalAccess", (K) => K.length]) === 0 || A0([
+    }), (Array.isArray(u) && S0([u, "optionalAccess", (K) => K[0], "optionalAccess", (K) => K.length]) === 0 || S0([
         u,
         "access",
         (K) => K.data,
         "optionalAccess",
         (K) => K[0],
         "optionalAccess",
         (K) => K.length
     ]) === 0) && (u = {
         data: [
-            Array(A0([v, "optionalAccess", (K) => K[0]]) || 3).fill("")
+            Array(S0([v, "optionalAccess", (K) => K[0]]) || 3).fill("")
         ],
-        headers: Array(A0([v, "optionalAccess", (K) => K[0]]) || 3).fill("").map((K, ye) => `${ye + 1}`),
+        headers: Array(S0([v, "optionalAccess", (K) => K[0]]) || 3).fill("").map((K, ye) => `${ye + 1}`),
         metadata: null
     });
     const We = D.filter((K) => K.type !== "checkbox"),
         Ie = D.filter((K) => K.type === "checkbox");
     Ie.forEach((K, ye) => {
         K.default && n(17, oe[We.length + ye] = [K.column, K.default], oe);
     });
     const Xe = (K) => n(18, Q = K.detail),
         Ue = (K) => !(C.includes(K) || E.cant_deselect.includes(K));
 
     function zt(K) {
         de = K, n(19, de);
     }
-    const Bn = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
+    const Nn = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
         Re = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
         $t = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
         Ot = (K) => {
             Ie.forEach((ye, Fe) => {
                 n(17, oe[We.length + Fe] = [ye.column, K.detail.includes(ye.column)], oe);
             });
         },
@@ -32201,15 +32201,15 @@
         pe,
         Me,
         oe,
         Q,
         de,
         Ne,
         he,
-        ae,
+        le,
         Be,
         We,
         Ie,
         u,
         _,
         l,
         o,
@@ -32218,15 +32218,15 @@
         U,
         M,
         D,
         p,
         Xe,
         Ue,
         zt,
-        Bn,
+        Nn,
         Re,
         $t,
         Ot,
         Ct
     ];
 }
 class J_ extends Z9 {
```

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/style.css` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/example/index.js` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/backend/gradio_leaderboard/templates/example/style.css` & `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/app.py` & `gradio_leaderboard-0.0.8/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/config.py` & `gradio_leaderboard-0.0.8/demo/config.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/css.css` & `gradio_leaderboard-0.0.8/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/docs.md` & `gradio_leaderboard-0.0.8/demo/docs.md`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/leaderboard_data.json` & `gradio_leaderboard-0.0.8/demo/leaderboard_data.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/demo/space.py` & `gradio_leaderboard-0.0.8/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/Example.svelte` & `gradio_leaderboard-0.0.8/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/Index.svelte` & `gradio_leaderboard-0.0.8/frontend/Index.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,17 @@
 					if (col_index !== -1) {
 						column_index = col_index;
 						query_value = query_value.substring(colon_index + 1).trim();
 					}
 				}
 
 				const push_to = colon_index !== -1 ? secondary_column_matches : primary_column_matches;
+				const val = values[i][column_index] === null ? "" : values[i][column_index].toString();
 
-				if (values[i][column_index].toString().toLowerCase().includes(query_value.toLowerCase())) {
+				if (val.toLowerCase().includes(query_value.toLowerCase())) {
 					push_to.push(true);
 				} else {
 					push_to.push(false);
 				}
 			}
 			if (primary_column_matches.length && !secondary_column_matches.length){
 				mask[i] = primary_column_matches.some(s => s);
```

### Comparing `gradio_leaderboard-0.0.7/frontend/package-lock.json` & `gradio_leaderboard-0.0.8/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/package.json` & `gradio_leaderboard-0.0.8/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/Checkboxgroup.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/Checkboxgroup.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/EditableCell.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/EditableCell.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/RangeSlider.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/RangeSlider.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,14 @@
       <div class="range-bg"></div>
       <div class="range-line" style={rangeLine}></div>
       <input type="range" min={min} max={max} bind:value={selected_min} on:input={handle_min_change} />
       <input type="range" min={min} max={max} bind:value={selected_max} on:input={handle_max_change} />
     </div>
   </Block>
 
-
-  
   <style>
     .wrap {
       display: flex;
       flex-direction: column;
       width: 100%;
 	  }
```

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/SimpleTextbox.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/SimpleTextbox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/Table.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/Table.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/VirtualTable.svelte` & `gradio_leaderboard-0.0.8/frontend/shared/VirtualTable.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/frontend/shared/utils.ts` & `gradio_leaderboard-0.0.8/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/README.md` & `gradio_leaderboard-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.7/pyproject.toml` & `gradio_leaderboard-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_leaderboard"
-version = "0.0.7"
+version = "0.0.8"
 description = "Super fast , batteries included Leaderboard component ⚡️"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Dataframe", "leaderboard", "dataframe", "data", "table"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates"]
+artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_leaderboard"]
```

### Comparing `gradio_leaderboard-0.0.7/PKG-INFO` & `gradio_leaderboard-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_leaderboard
-Version: 0.0.7
+Version: 0.0.8
 Summary: Super fast , batteries included Leaderboard component ⚡️
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: MIT
 Keywords: data,dataframe,gradio-custom-component,gradio-template-Dataframe,leaderboard,table
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```


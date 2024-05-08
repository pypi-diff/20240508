# Comparing `tmp/draggable-charts-1.2.5.tar.gz` & `tmp/draggable-charts-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-charts-1.2.5.tar", last modified: Tue May  7 03:21:34 2024, max compression
+gzip compressed data, was "draggable-charts-1.2.6.tar", last modified: Tue May  7 21:25:44 2024, max compression
```

## Comparing `draggable-charts-1.2.5.tar` & `draggable-charts-1.2.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.190616 draggable-charts-1.2.5/
--rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.5/LICENSE
--rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6106 2024-05-07 03:21:34.186322 draggable-charts-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.981090 draggable-charts-1.2.5/draggable_charts/
--rw-rw-rw-   0        0        0       41 2024-05-07 03:18:24.000000 draggable-charts-1.2.5/draggable_charts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.934858 draggable-charts-1.2.5/draggable_charts/frontend/
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.044910 draggable-charts-1.2.5/draggable_charts/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:33.936756 draggable-charts-1.2.5/draggable_charts/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.079817 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/
--rw-rw-rw-   0        0        0   604810 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js
--rw-rw-rw-   0        0        0     1831 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2584548 2024-05-07 03:21:02.000000 draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.map
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.128206 draggable-charts-1.2.5/draggable_charts/utils/
--rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.5/draggable_charts/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.5/draggable_charts/utils/callback.py
--rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.5/draggable_charts/utils/component_func.py
--rw-rw-rw-   0        0        0     2626 2024-05-06 23:57:39.000000 draggable-charts-1.2.5/draggable_charts/utils/options.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.175081 draggable-charts-1.2.5/draggable_charts/widgets/
--rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.5/draggable_charts/widgets/__init__.py
--rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.5/draggable_charts/widgets/bezierchart.py
--rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.5/draggable_charts/widgets/cubicbezierchart.py
--rw-rw-rw-   0        0        0     4720 2024-05-07 01:53:09.000000 draggable-charts-1.2.5/draggable_charts/widgets/linechart.py
--rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.5/draggable_charts/widgets/scatterchart.py
-drwxrwxrwx   0        0        0        0 2024-05-07 03:21:34.015988 draggable-charts-1.2.5/draggable_charts.egg-info/
--rw-rw-rw-   0        0        0     6106 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      950 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 03:21:33.000000 draggable-charts-1.2.5/draggable_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 03:21:34.192626 draggable-charts-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1115 2024-05-07 03:20:13.000000 draggable-charts-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.917979 draggable-charts-1.2.6/
+-rw-rw-rw-   0        0        0     1057 2024-04-29 05:02:10.000000 draggable-charts-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-04-23 23:20:49.000000 draggable-charts-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6106 2024-05-07 21:25:44.915100 draggable-charts-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5613 2024-04-24 01:12:42.000000 draggable-charts-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.754661 draggable-charts-1.2.6/draggable_charts/
+-rw-rw-rw-   0        0        0       41 2024-05-07 21:22:46.000000 draggable-charts-1.2.6/draggable_charts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.722471 draggable-charts-1.2.6/draggable_charts/frontend/
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.811855 draggable-charts-1.2.6/draggable_charts/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-05-07 21:23:46.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-23 23:20:49.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-05-07 21:23:46.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.725462 draggable-charts-1.2.6/draggable_charts/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.834831 draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   603757 2024-05-07 21:23:46.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js
+-rw-rw-rw-   0        0        0     1831 2024-05-07 21:23:46.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2581145 2024-05-07 21:23:46.000000 draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js.map
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.874827 draggable-charts-1.2.6/draggable_charts/utils/
+-rw-rw-rw-   0        0        0      149 2024-04-25 23:36:44.000000 draggable-charts-1.2.6/draggable_charts/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-04-25 23:34:16.000000 draggable-charts-1.2.6/draggable_charts/utils/callback.py
+-rw-rw-rw-   0        0        0     1220 2024-04-23 23:20:49.000000 draggable-charts-1.2.6/draggable_charts/utils/component_func.py
+-rw-rw-rw-   0        0        0     2838 2024-05-07 21:09:41.000000 draggable-charts-1.2.6/draggable_charts/utils/options.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.907977 draggable-charts-1.2.6/draggable_charts/widgets/
+-rw-rw-rw-   0        0        0      163 2024-04-29 05:02:10.000000 draggable-charts-1.2.6/draggable_charts/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3757 2024-05-02 19:52:35.000000 draggable-charts-1.2.6/draggable_charts/widgets/bezierchart.py
+-rw-rw-rw-   0        0        0     5258 2024-05-02 19:52:32.000000 draggable-charts-1.2.6/draggable_charts/widgets/cubicbezierchart.py
+-rw-rw-rw-   0        0        0     4720 2024-05-07 01:53:09.000000 draggable-charts-1.2.6/draggable_charts/widgets/linechart.py
+-rw-rw-rw-   0        0        0     2324 2024-05-02 19:52:11.000000 draggable-charts-1.2.6/draggable_charts/widgets/scatterchart.py
+drwxrwxrwx   0        0        0        0 2024-05-07 21:25:44.787859 draggable-charts-1.2.6/draggable_charts.egg-info/
+-rw-rw-rw-   0        0        0     6106 2024-05-07 21:25:44.000000 draggable-charts-1.2.6/draggable_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2024-05-07 21:25:44.000000 draggable-charts-1.2.6/draggable_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 21:25:44.000000 draggable-charts-1.2.6/draggable_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-07 21:25:44.000000 draggable-charts-1.2.6/draggable_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 21:25:44.000000 draggable-charts-1.2.6/draggable_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-07 21:25:44.920424 draggable-charts-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2024-05-07 21:25:27.000000 draggable-charts-1.2.6/setup.py
```

### Comparing `draggable-charts-1.2.5/LICENSE` & `draggable-charts-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/PKG-INFO` & `draggable-charts-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.5/README.md` & `draggable-charts-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/frontend/build/bootstrap.min.css` & `draggable-charts-1.2.6/draggable_charts/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js` & `draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.41dd267d.js.LICENSE.txt */
+/*! For license information please see main.8018b5ba.js.LICENSE.txt */
 (() => {
     var e = {
             895: (t, e, n) => {
                 var i;
                 ! function(r, s, o, a) {
                     "use strict";
                     var l, c = ["", "webkit", "Moz", "MS", "ms", "o"],
@@ -146,19 +146,19 @@
                         U = "mouse",
                         V = 25,
                         j = 1,
                         W = 4,
                         H = 8,
                         Y = 1,
                         $ = 2,
-                        X = 4,
-                        K = 8,
-                        q = 16,
-                        Q = $ | X,
-                        G = K | q,
+                        K = 4,
+                        q = 8,
+                        X = 16,
+                        Q = $ | K,
+                        G = q | X,
                         Z = Q | G,
                         J = ["x", "y"],
                         tt = ["clientX", "clientY"];
 
                     function et(t, e) {
                         var n = this;
                         this.manager = t, this.callback = e, this.element = t.element, this.target = t.options.inputTarget, this.domHandler = function(e) {
@@ -250,15 +250,15 @@
                         return {
                             x: e / t || 0,
                             y: n / t || 0
                         }
                     }
 
                     function ot(t, e) {
-                        return t === e ? Y : f(t) >= f(e) ? t < 0 ? $ : X : e < 0 ? K : q
+                        return t === e ? Y : f(t) >= f(e) ? t < 0 ? $ : K : e < 0 ? q : X
                     }
 
                     function at(t, e, n) {
                         n || (n = J);
                         var i = e[n[0]] - t[n[0]],
                             r = e[n[1]] - t[n[1]];
                         return Math.sqrt(i * i + r * r)
@@ -528,35 +528,35 @@
                     }
 
                     function Wt(t) {
                         return 16 & t ? "cancel" : 8 & t ? "end" : 4 & t ? "move" : 2 & t ? "start" : ""
                     }
 
                     function Ht(t) {
-                        return t == q ? "down" : t == K ? "up" : t == $ ? "left" : t == X ? "right" : ""
+                        return t == X ? "down" : t == q ? "up" : t == $ ? "left" : t == K ? "right" : ""
                     }
 
                     function Yt(t, e) {
                         var n = e.manager;
                         return n ? n.get(t) : t
                     }
 
                     function $t() {
                         jt.apply(this, arguments)
                     }
 
-                    function Xt() {
+                    function Kt() {
                         $t.apply(this, arguments), this.pX = null, this.pY = null
                     }
 
-                    function Kt() {
+                    function qt() {
                         $t.apply(this, arguments)
                     }
 
-                    function qt() {
+                    function Xt() {
                         jt.apply(this, arguments), this._timer = null, this._input = null
                     }
 
                     function Qt() {
                         $t.apply(this, arguments)
                     }
 
@@ -640,15 +640,15 @@
                         process: function(t) {
                             var e = this.state,
                                 n = t.eventType,
                                 i = 6 & e,
                                 r = this.attrTest(t);
                             return i && (n & H || !r) ? 16 | e : i || r ? n & W ? 8 | e : 2 & e ? 4 | e : 2 : Vt
                         }
-                    }), _(Xt, $t, {
+                    }), _(Kt, $t, {
                         defaults: {
                             event: "pan",
                             threshold: 10,
                             pointers: 1,
                             direction: Z
                         },
                         getTouchAction: function() {
@@ -659,25 +659,25 @@
                         directionTest: function(t) {
                             var e = this.options,
                                 n = !0,
                                 i = t.distance,
                                 r = t.direction,
                                 s = t.deltaX,
                                 o = t.deltaY;
-                            return r & e.direction || (e.direction & Q ? (r = 0 === s ? Y : s < 0 ? $ : X, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? Y : o < 0 ? K : q, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
+                            return r & e.direction || (e.direction & Q ? (r = 0 === s ? Y : s < 0 ? $ : K, n = s != this.pX, i = Math.abs(t.deltaX)) : (r = 0 === o ? Y : o < 0 ? q : X, n = o != this.pY, i = Math.abs(t.deltaY))), t.direction = r, n && i > e.threshold && r & e.direction
                         },
                         attrTest: function(t) {
                             return $t.prototype.attrTest.call(this, t) && (2 & this.state || !(2 & this.state) && this.directionTest(t))
                         },
                         emit: function(t) {
                             this.pX = t.deltaX, this.pY = t.deltaY;
                             var e = Ht(t.direction);
                             e && (t.additionalEvent = this.options.event + e), this._super.emit.call(this, t)
                         }
-                    }), _(Kt, $t, {
+                    }), _(qt, $t, {
                         defaults: {
                             event: "pinch",
                             threshold: 0,
                             pointers: 2
                         },
                         getTouchAction: function() {
                             return [Lt]
@@ -688,15 +688,15 @@
                         emit: function(t) {
                             if (1 !== t.scale) {
                                 var e = t.scale < 1 ? "in" : "out";
                                 t.additionalEvent = this.options.event + e
                             }
                             this._super.emit.call(this, t)
                         }
-                    }), _(qt, jt, {
+                    }), _(Xt, jt, {
                         defaults: {
                             event: "press",
                             pointers: 1,
                             time: 251,
                             threshold: 9
                         },
                         getTouchAction: function() {
@@ -737,15 +737,15 @@
                             event: "swipe",
                             threshold: 10,
                             velocity: .3,
                             direction: Q | G,
                             pointers: 1
                         },
                         getTouchAction: function() {
-                            return Xt.prototype.getTouchAction.call(this)
+                            return Kt.prototype.getTouchAction.call(this)
                         },
                         attrTest: function(t) {
                             var e, n = this.options.direction;
                             return n & (Q | G) ? e = t.overallVelocity : n & Q ? e = t.overallVelocityX : n & G && (e = t.overallVelocityY), this._super.attrTest.call(this, t) && n & t.offsetDirection && t.distance > this.options.threshold && t.maxPointers == this.options.pointers && f(e) > this.options.velocity && t.eventType & W
                         },
                         emit: function(t) {
                             var e = Ht(t.offsetDirection);
@@ -797,35 +797,35 @@
                         enable: !0,
                         inputTarget: null,
                         inputClass: null,
                         preset: [
                             [Qt, {
                                 enable: !1
                             }],
-                            [Kt, {
+                            [qt, {
                                     enable: !1
                                 },
                                 ["rotate"]
                             ],
                             [Gt, {
                                 direction: Q
                             }],
-                            [Xt, {
+                            [Kt, {
                                     direction: Q
                                 },
                                 ["swipe"]
                             ],
                             [Zt],
                             [Zt, {
                                     event: "doubletap",
                                     taps: 2
                                 },
                                 ["tap"]
                             ],
-                            [qt]
+                            [Xt]
                         ],
                         cssProps: {
                             userSelect: "none",
                             touchSelect: "none",
                             touchCallout: "none",
                             contentZooming: "none",
                             userDrag: "none",
@@ -926,36 +926,36 @@
                         STATE_CHANGED: 4,
                         STATE_ENDED: 8,
                         STATE_RECOGNIZED: 8,
                         STATE_CANCELLED: 16,
                         STATE_FAILED: Vt,
                         DIRECTION_NONE: Y,
                         DIRECTION_LEFT: $,
-                        DIRECTION_RIGHT: X,
-                        DIRECTION_UP: K,
-                        DIRECTION_DOWN: q,
+                        DIRECTION_RIGHT: K,
+                        DIRECTION_UP: q,
+                        DIRECTION_DOWN: X,
                         DIRECTION_HORIZONTAL: Q,
                         DIRECTION_VERTICAL: G,
                         DIRECTION_ALL: Z,
                         Manager: te,
                         Input: et,
                         TouchAction: Rt,
                         TouchInput: St,
                         MouseInput: dt,
                         PointerEventInput: yt,
                         TouchMouseInput: Mt,
                         SingleTouchInput: vt,
                         Recognizer: jt,
                         AttrRecognizer: $t,
                         Tap: Zt,
-                        Pan: Xt,
+                        Pan: Kt,
                         Swipe: Gt,
-                        Pinch: Kt,
+                        Pinch: qt,
                         Rotate: Qt,
-                        Press: qt,
+                        Press: Xt,
                         on: k,
                         off: M,
                         each: y,
                         merge: x,
                         extend: v,
                         assign: l,
                         inherit: _,
@@ -1305,63 +1305,63 @@
                     W = Object.prototype.hasOwnProperty,
                     H = {},
                     Y = {};
 
                 function $(t, e, n, i, r, s) {
                     this.acceptsBooleans = 2 === e || 3 === e || 4 === e, this.attributeName = i, this.attributeNamespace = r, this.mustUseProperty = n, this.propertyName = t, this.type = e, this.sanitizeURL = s
                 }
-                var X = {};
+                var K = {};
                 "children dangerouslySetInnerHTML defaultValue defaultChecked innerHTML suppressContentEditableWarning suppressHydrationWarning style".split(" ").forEach((function(t) {
-                    X[t] = new $(t, 0, !1, t, null, !1)
+                    K[t] = new $(t, 0, !1, t, null, !1)
                 })), [
                     ["acceptCharset", "accept-charset"],
                     ["className", "class"],
                     ["htmlFor", "for"],
                     ["httpEquiv", "http-equiv"]
                 ].forEach((function(t) {
                     var e = t[0];
-                    X[e] = new $(e, 1, !1, t[1], null, !1)
+                    K[e] = new $(e, 1, !1, t[1], null, !1)
                 })), ["contentEditable", "draggable", "spellCheck", "value"].forEach((function(t) {
-                    X[t] = new $(t, 2, !1, t.toLowerCase(), null, !1)
+                    K[t] = new $(t, 2, !1, t.toLowerCase(), null, !1)
                 })), ["autoReverse", "externalResourcesRequired", "focusable", "preserveAlpha"].forEach((function(t) {
-                    X[t] = new $(t, 2, !1, t, null, !1)
+                    K[t] = new $(t, 2, !1, t, null, !1)
                 })), "allowFullScreen async autoFocus autoPlay controls default defer disabled disablePictureInPicture formNoValidate hidden loop noModule noValidate open playsInline readOnly required reversed scoped seamless itemScope".split(" ").forEach((function(t) {
-                    X[t] = new $(t, 3, !1, t.toLowerCase(), null, !1)
+                    K[t] = new $(t, 3, !1, t.toLowerCase(), null, !1)
                 })), ["checked", "multiple", "muted", "selected"].forEach((function(t) {
-                    X[t] = new $(t, 3, !0, t, null, !1)
+                    K[t] = new $(t, 3, !0, t, null, !1)
                 })), ["capture", "download"].forEach((function(t) {
-                    X[t] = new $(t, 4, !1, t, null, !1)
+                    K[t] = new $(t, 4, !1, t, null, !1)
                 })), ["cols", "rows", "size", "span"].forEach((function(t) {
-                    X[t] = new $(t, 6, !1, t, null, !1)
+                    K[t] = new $(t, 6, !1, t, null, !1)
                 })), ["rowSpan", "start"].forEach((function(t) {
-                    X[t] = new $(t, 5, !1, t.toLowerCase(), null, !1)
+                    K[t] = new $(t, 5, !1, t.toLowerCase(), null, !1)
                 }));
-                var K = /[\-:]([a-z])/g;
+                var q = /[\-:]([a-z])/g;
 
-                function q(t) {
+                function X(t) {
                     return t[1].toUpperCase()
                 }
                 "accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height".split(" ").forEach((function(t) {
-                    var e = t.replace(K, q);
-                    X[e] = new $(e, 1, !1, t, null, !1)
+                    var e = t.replace(q, X);
+                    K[e] = new $(e, 1, !1, t, null, !1)
                 })), "xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type".split(" ").forEach((function(t) {
-                    var e = t.replace(K, q);
-                    X[e] = new $(e, 1, !1, t, "http://www.w3.org/1999/xlink", !1)
+                    var e = t.replace(q, X);
+                    K[e] = new $(e, 1, !1, t, "http://www.w3.org/1999/xlink", !1)
                 })), ["xml:base", "xml:lang", "xml:space"].forEach((function(t) {
-                    var e = t.replace(K, q);
-                    X[e] = new $(e, 1, !1, t, "http://www.w3.org/XML/1998/namespace", !1)
+                    var e = t.replace(q, X);
+                    K[e] = new $(e, 1, !1, t, "http://www.w3.org/XML/1998/namespace", !1)
                 })), ["tabIndex", "crossOrigin"].forEach((function(t) {
-                    X[t] = new $(t, 1, !1, t.toLowerCase(), null, !1)
-                })), X.xlinkHref = new $("xlinkHref", 1, !1, "xlink:href", "http://www.w3.org/1999/xlink", !0), ["src", "href", "action", "formAction"].forEach((function(t) {
-                    X[t] = new $(t, 1, !1, t.toLowerCase(), null, !0)
+                    K[t] = new $(t, 1, !1, t.toLowerCase(), null, !1)
+                })), K.xlinkHref = new $("xlinkHref", 1, !1, "xlink:href", "http://www.w3.org/1999/xlink", !0), ["src", "href", "action", "formAction"].forEach((function(t) {
+                    K[t] = new $(t, 1, !1, t.toLowerCase(), null, !0)
                 }));
                 var Q = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED;
 
                 function G(t, e, n, i) {
-                    var r = X.hasOwnProperty(e) ? X[e] : null;
+                    var r = K.hasOwnProperty(e) ? K[e] : null;
                     (null !== r ? 0 === r.type : !i && (2 < e.length && ("o" === e[0] || "O" === e[0]) && ("n" === e[1] || "N" === e[1]))) || (function(t, e, n, i) {
                         if (null === e || "undefined" === typeof e || function(t, e, n, i) {
                                 if (null !== n && 0 === n.type) return !1;
                                 switch (typeof e) {
                                     case "function":
                                     case "symbol":
                                         return !0;
@@ -1697,17 +1697,17 @@
                     if (!Wt[t]) return t;
                     var e, n = Wt[t];
                     for (e in n)
                         if (n.hasOwnProperty(e) && e in Yt) return Ht[t] = n[e];
                     return t
                 }
                 I && (Yt = document.createElement("div").style, "AnimationEvent" in window || (delete Wt.animationend.animation, delete Wt.animationiteration.animation, delete Wt.animationstart.animation), "TransitionEvent" in window || delete Wt.transitionend.transition);
-                var Xt = $t("animationend"),
-                    Kt = $t("animationiteration"),
-                    qt = $t("animationstart"),
+                var Kt = $t("animationend"),
+                    qt = $t("animationiteration"),
+                    Xt = $t("animationstart"),
                     Qt = $t("transitionend"),
                     Gt = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
                     Zt = new("function" === typeof WeakMap ? WeakMap : Map);
 
                 function Jt(t) {
                     var e = Zt.get(t);
                     return void 0 === e && (e = new Map, Zt.set(t, e)), e
@@ -1902,30 +1902,30 @@
                     }
                 }
 
                 function ge(t, e, n) {
                     if (!n.has(t)) {
                         switch (t) {
                             case "scroll":
-                                qe(e, "scroll", !0);
+                                Xe(e, "scroll", !0);
                                 break;
                             case "focus":
                             case "blur":
-                                qe(e, "focus", !0), qe(e, "blur", !0), n.set("blur", null), n.set("focus", null);
+                                Xe(e, "focus", !0), Xe(e, "blur", !0), n.set("blur", null), n.set("focus", null);
                                 break;
                             case "cancel":
                             case "close":
-                                ue(t) && qe(e, t, !0);
+                                ue(t) && Xe(e, t, !0);
                                 break;
                             case "invalid":
                             case "submit":
                             case "reset":
                                 break;
                             default:
-                                -1 === Gt.indexOf(t) && Ke(t, e)
+                                -1 === Gt.indexOf(t) && qe(t, e)
                         }
                         n.set(t, null)
                     }
                 }
                 var me, ye, be, ve = !1,
                     xe = [],
                     _e = null,
@@ -2033,15 +2033,15 @@
                     }
                     for (null !== _e && ze(_e, t), null !== we && ze(we, t), null !== Se && ze(Se, t), Te.forEach(e), ke.forEach(e), n = 0; n < Me.length; n++)(i = Me[n]).blockedOn === t && (i.blockedOn = null);
                     for (; 0 < Me.length && null === (n = Me[0]).blockedOn;) Ae(n), null === n.blockedOn && Me.shift()
                 }
                 var Be = {},
                     Re = new Map,
                     Ue = new Map,
-                    Ve = ["abort", "abort", Xt, "animationEnd", Kt, "animationIteration", qt, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Qt, "transitionEnd", "waiting", "waiting"];
+                    Ve = ["abort", "abort", Kt, "animationEnd", qt, "animationIteration", Xt, "animationStart", "canplay", "canPlay", "canplaythrough", "canPlayThrough", "durationchange", "durationChange", "emptied", "emptied", "encrypted", "encrypted", "ended", "ended", "error", "error", "gotpointercapture", "gotPointerCapture", "load", "load", "loadeddata", "loadedData", "loadedmetadata", "loadedMetadata", "loadstart", "loadStart", "lostpointercapture", "lostPointerCapture", "playing", "playing", "progress", "progress", "seeking", "seeking", "stalled", "stalled", "suspend", "suspend", "timeupdate", "timeUpdate", Qt, "transitionEnd", "waiting", "waiting"];
 
                 function je(t, e) {
                     for (var n = 0; n < t.length; n += 2) {
                         var i = t[n],
                             r = t[n + 1],
                             s = "on" + (r[0].toUpperCase() + r.slice(1));
                         s = {
@@ -2054,21 +2054,21 @@
                         }, Ue.set(i, e), Re.set(i, s), Be[r] = s
                     }
                 }
                 je("blur blur cancel cancel click click close close contextmenu contextMenu copy copy cut cut auxclick auxClick dblclick doubleClick dragend dragEnd dragstart dragStart drop drop focus focus input input invalid invalid keydown keyDown keypress keyPress keyup keyUp mousedown mouseDown mouseup mouseUp paste paste pause pause play play pointercancel pointerCancel pointerdown pointerDown pointerup pointerUp ratechange rateChange reset reset seeked seeked submit submit touchcancel touchCancel touchend touchEnd touchstart touchStart volumechange volumeChange".split(" "), 0), je("drag drag dragenter dragEnter dragexit dragExit dragleave dragLeave dragover dragOver mousemove mouseMove mouseout mouseOut mouseover mouseOver pointermove pointerMove pointerout pointerOut pointerover pointerOver scroll scroll toggle toggle touchmove touchMove wheel wheel".split(" "), 1), je(Ve, 2);
                 for (var We = "change selectionchange textInput compositionstart compositionend compositionupdate".split(" "), He = 0; He < We.length; He++) Ue.set(We[He], 0);
                 var Ye = s.unstable_UserBlockingPriority,
                     $e = s.unstable_runWithPriority,
-                    Xe = !0;
+                    Ke = !0;
 
-                function Ke(t, e) {
-                    qe(e, t, !1)
+                function qe(t, e) {
+                    Xe(e, t, !1)
                 }
 
-                function qe(t, e, n) {
+                function Xe(t, e, n) {
                     var i = Ue.get(e);
                     switch (void 0 === i ? 2 : i) {
                         case 0:
                             i = Qe.bind(null, e, 1, t);
                             break;
                         case 1:
                             i = Ge.bind(null, e, 1, t);
@@ -2092,15 +2092,15 @@
                 }
 
                 function Ge(t, e, n, i) {
                     $e(Ye, Ze.bind(null, t, e, n, i))
                 }
 
                 function Ze(t, e, n, i) {
-                    if (Xe)
+                    if (Ke)
                         if (0 < xe.length && -1 < Ie.indexOf(t)) t = De(null, t, e, n, i), xe.push(t);
                         else {
                             var r = Je(t, e, n, i);
                             if (null === r) Oe(t, i);
                             else if (-1 < Ie.indexOf(t)) t = De(r, t, e, n, i), xe.push(t);
                             else if (! function(t, e, n, i, r) {
                                     switch (e) {
@@ -2469,37 +2469,37 @@
                 function Wn(t) {
                     se(t, Un)
                 }
                 var Hn = null,
                     Yn = null,
                     $n = null;
 
-                function Xn() {
+                function Kn() {
                     if ($n) return $n;
                     var t, e, n = Yn,
                         i = n.length,
                         r = "value" in Hn ? Hn.value : Hn.textContent,
                         s = r.length;
                     for (t = 0; t < i && n[t] === r[t]; t++);
                     var o = i - t;
                     for (e = 1; e <= o && n[i - e] === r[s - e]; e++);
                     return $n = r.slice(t, 1 < e ? 1 - e : void 0)
                 }
 
-                function Kn() {
+                function qn() {
                     return !0
                 }
 
-                function qn() {
+                function Xn() {
                     return !1
                 }
 
                 function Qn(t, e, n, i) {
                     for (var r in this.dispatchConfig = t, this._targetInst = e, this.nativeEvent = n, t = this.constructor.Interface) t.hasOwnProperty(r) && ((e = t[r]) ? this[r] = e(n) : "target" === r ? this.target = i : this[r] = n[r]);
-                    return this.isDefaultPrevented = (null != n.defaultPrevented ? n.defaultPrevented : !1 === n.returnValue) ? Kn : qn, this.isPropagationStopped = qn, this
+                    return this.isDefaultPrevented = (null != n.defaultPrevented ? n.defaultPrevented : !1 === n.returnValue) ? qn : Xn, this.isPropagationStopped = Xn, this
                 }
 
                 function Gn(t, e, n, i) {
                     if (this.eventPool.length) {
                         var r = this.eventPool.pop();
                         return this.call(r, t, e, n, i), r
                     }
@@ -2514,28 +2514,28 @@
                 function Jn(t) {
                     t.eventPool = [], t.getPooled = Gn, t.release = Zn
                 }
                 r(Qn.prototype, {
                     preventDefault: function() {
                         this.defaultPrevented = !0;
                         var t = this.nativeEvent;
-                        t && (t.preventDefault ? t.preventDefault() : "unknown" !== typeof t.returnValue && (t.returnValue = !1), this.isDefaultPrevented = Kn)
+                        t && (t.preventDefault ? t.preventDefault() : "unknown" !== typeof t.returnValue && (t.returnValue = !1), this.isDefaultPrevented = qn)
                     },
                     stopPropagation: function() {
                         var t = this.nativeEvent;
-                        t && (t.stopPropagation ? t.stopPropagation() : "unknown" !== typeof t.cancelBubble && (t.cancelBubble = !0), this.isPropagationStopped = Kn)
+                        t && (t.stopPropagation ? t.stopPropagation() : "unknown" !== typeof t.cancelBubble && (t.cancelBubble = !0), this.isPropagationStopped = qn)
                     },
                     persist: function() {
-                        this.isPersistent = Kn
+                        this.isPersistent = qn
                     },
-                    isPersistent: qn,
+                    isPersistent: Xn,
                     destructor: function() {
                         var t, e = this.constructor.Interface;
                         for (t in e) this[t] = null;
-                        this.nativeEvent = this._targetInst = this.dispatchConfig = null, this.isPropagationStopped = this.isDefaultPrevented = qn, this._dispatchInstances = this._dispatchListeners = null
+                        this.nativeEvent = this._targetInst = this.dispatchConfig = null, this.isPropagationStopped = this.isDefaultPrevented = Xn, this._dispatchInstances = this._dispatchListeners = null
                     }
                 }), Qn.Interface = {
                     type: null,
                     target: null,
                     currentTarget: function() {
                         return null
                     },
@@ -2637,27 +2637,27 @@
                                     case "compositionupdate":
                                         s = li.compositionUpdate;
                                         break t
                                 }
                                 s = void 0
                             }
                             else di ? ui(t, n) && (s = li.compositionEnd) : "keydown" === t && 229 === n.keyCode && (s = li.compositionStart);
-                            return s ? (oi && "ko" !== n.locale && (di || s !== li.compositionStart ? s === li.compositionEnd && di && (r = Xn()) : (Yn = "value" in (Hn = i) ? Hn.value : Hn.textContent, di = !0)), s = ti.getPooled(s, e, n, i), r ? s.data = r : null !== (r = hi(n)) && (s.data = r), Wn(s), r = s) : r = null, (t = si ? function(t, e) {
+                            return s ? (oi && "ko" !== n.locale && (di || s !== li.compositionStart ? s === li.compositionEnd && di && (r = Kn()) : (Yn = "value" in (Hn = i) ? Hn.value : Hn.textContent, di = !0)), s = ti.getPooled(s, e, n, i), r ? s.data = r : null !== (r = hi(n)) && (s.data = r), Wn(s), r = s) : r = null, (t = si ? function(t, e) {
                                 switch (t) {
                                     case "compositionend":
                                         return hi(e);
                                     case "keypress":
                                         return 32 !== e.which ? null : (ci = !0, ai);
                                     case "textInput":
                                         return (t = e.data) === ai && ci ? null : t;
                                     default:
                                         return null
                                 }
                             }(t, n) : function(t, e) {
-                                if (di) return "compositionend" === t || !ii && ui(t, e) ? (t = Xn(), $n = Yn = Hn = null, di = !1, t) : null;
+                                if (di) return "compositionend" === t || !ii && ui(t, e) ? (t = Kn(), $n = Yn = Hn = null, di = !1, t) : null;
                                 switch (t) {
                                     case "paste":
                                     default:
                                         return null;
                                     case "keypress":
                                         if (!(e.ctrlKey || e.altKey || e.metaKey) || e.ctrlKey && e.altKey) {
                                             if (e.char && 1 < e.char.length) return e.char;
@@ -2899,42 +2899,42 @@
                         i = Object.keys(e);
                     if (n.length !== i.length) return !1;
                     for (i = 0; i < n.length; i++)
                         if (!Hi.call(e, n[i]) || !Wi(t[n[i]], e[n[i]])) return !1;
                     return !0
                 }
                 var $i = I && "documentMode" in document && 11 >= document.documentMode,
-                    Xi = {
+                    Ki = {
                         select: {
                             phasedRegistrationNames: {
                                 bubbled: "onSelect",
                                 captured: "onSelectCapture"
                             },
                             dependencies: "blur contextmenu dragend focus keydown keyup mousedown mouseup selectionchange".split(" ")
                         }
                     },
-                    Ki = null,
                     qi = null,
+                    Xi = null,
                     Qi = null,
                     Gi = !1;
 
                 function Zi(t, e) {
                     var n = e.window === e ? e.document : 9 === e.nodeType ? e : e.ownerDocument;
-                    return Gi || null == Ki || Ki !== hn(n) ? null : ("selectionStart" in (n = Ki) && mn(n) ? n = {
+                    return Gi || null == qi || qi !== hn(n) ? null : ("selectionStart" in (n = qi) && mn(n) ? n = {
                         start: n.selectionStart,
                         end: n.selectionEnd
                     } : n = {
                         anchorNode: (n = (n.ownerDocument && n.ownerDocument.defaultView || window).getSelection()).anchorNode,
                         anchorOffset: n.anchorOffset,
                         focusNode: n.focusNode,
                         focusOffset: n.focusOffset
-                    }, Qi && Yi(Qi, n) ? null : (Qi = n, (t = Qn.getPooled(Xi.select, qi, t, e)).type = "select", t.target = Ki, Wn(t), t))
+                    }, Qi && Yi(Qi, n) ? null : (Qi = n, (t = Qn.getPooled(Ki.select, Xi, t, e)).type = "select", t.target = qi, Wn(t), t))
                 }
                 var Ji = {
-                        eventTypes: Xi,
+                        eventTypes: Ki,
                         extractEvents: function(t, e, n, i, r, s) {
                             if (!(s = !(r = s || (i.window === i ? i.document : 9 === i.nodeType ? i : i.ownerDocument)))) {
                                 t: {
                                     r = Jt(r),
                                     s = k.onSelect;
                                     for (var o = 0; o < s.length; o++)
                                         if (!r.has(s[o])) {
@@ -2943,18 +2943,18 @@
                                         } r = !0
                                 }
                                 s = !r
                             }
                             if (s) return null;
                             switch (r = e ? Ln(e) : window, t) {
                                 case "focus":
-                                    (gi(r) || "true" === r.contentEditable) && (Ki = r, qi = e, Qi = null);
+                                    (gi(r) || "true" === r.contentEditable) && (qi = r, Xi = e, Qi = null);
                                     break;
                                 case "blur":
-                                    Qi = qi = Ki = null;
+                                    Qi = Xi = qi = null;
                                     break;
                                 case "mousedown":
                                     Gi = !0;
                                     break;
                                 case "contextmenu":
                                 case "mouseup":
                                 case "dragend":
@@ -3132,17 +3132,17 @@
                                     break;
                                 case "touchcancel":
                                 case "touchend":
                                 case "touchmove":
                                 case "touchstart":
                                     t = lr;
                                     break;
-                                case Xt:
                                 case Kt:
                                 case qt:
+                                case Xt:
                                     t = tr;
                                     break;
                                 case Qt:
                                     t = cr;
                                     break;
                                 case "scroll":
                                     t = Ci;
@@ -3273,15 +3273,15 @@
                         case Nr:
                             return 95;
                         default:
                             throw Error(o(332))
                     }
                 }
 
-                function Xr(t) {
+                function Kr(t) {
                     switch (t) {
                         case 99:
                             return Pr;
                         case 98:
                             return Fr;
                         case 97:
                             return Lr;
@@ -3290,20 +3290,20 @@
                         case 95:
                             return Nr;
                         default:
                             throw Error(o(332))
                     }
                 }
 
-                function Kr(t, e) {
-                    return t = Xr(t), Ir(t, e)
+                function qr(t, e) {
+                    return t = Kr(t), Ir(t, e)
                 }
 
-                function qr(t, e, n) {
-                    return t = Xr(t), Er(t, e, n)
+                function Xr(t, e, n) {
+                    return t = Kr(t), Er(t, e, n)
                 }
 
                 function Qr(t) {
                     return null === Vr ? (Vr = [t], jr = Er(Pr, Zr)) : Vr.push(t), Br
                 }
 
                 function Gr() {
@@ -3316,15 +3316,15 @@
 
                 function Zr() {
                     if (!Wr && null !== Vr) {
                         Wr = !0;
                         var t = 0;
                         try {
                             var e = Vr;
-                            Kr(99, (function() {
+                            qr(99, (function() {
                                 for (; t < e.length; t++) {
                                     var n = e[t];
                                     do {
                                         n = n(!0)
                                     } while (null !== n)
                                 }
                             })), Vr = null
@@ -3634,29 +3634,29 @@
                     }
 
                     function c(t, e, n, i) {
                         return null !== e && e.elementType === n.type ? ((i = r(e, n.props)).ref = Is(t, e, n), i.return = t, i) : ((i = Hl(n.type, n.key, n.props, null, t.mode, i)).ref = Is(t, e, n), i.return = t, i)
                     }
 
                     function u(t, e, n, i) {
-                        return null === e || 4 !== e.tag || e.stateNode.containerInfo !== n.containerInfo || e.stateNode.implementation !== n.implementation ? ((e = Xl(n, t.mode, i)).return = t, e) : ((e = r(e, n.children || [])).return = t, e)
+                        return null === e || 4 !== e.tag || e.stateNode.containerInfo !== n.containerInfo || e.stateNode.implementation !== n.implementation ? ((e = Kl(n, t.mode, i)).return = t, e) : ((e = r(e, n.children || [])).return = t, e)
                     }
 
                     function h(t, e, n, i, s) {
                         return null === e || 7 !== e.tag ? ((e = Yl(n, t.mode, i, s)).return = t, e) : ((e = r(e, n)).return = t, e)
                     }
 
                     function d(t, e, n) {
                         if ("string" === typeof e || "number" === typeof e) return (e = $l("" + e, t.mode, n)).return = t, e;
                         if ("object" === typeof e && null !== e) {
                             switch (e.$$typeof) {
                                 case tt:
                                     return (n = Hl(e.type, e.key, e.props, null, t.mode, n)).ref = Is(t, null, e), n.return = t, n;
                                 case et:
-                                    return (e = Xl(e, t.mode, n)).return = t, e
+                                    return (e = Kl(e, t.mode, n)).return = t, e
                             }
                             if (Ms(e) || gt(e)) return (e = Yl(e, t.mode, n, null)).return = t, e;
                             Es(t, e)
                         }
                         return null
                     }
 
@@ -3769,15 +3769,15 @@
                                                 n(t, i.sibling), (i = r(i, s.children || [])).return = t, t = i;
                                                 break t
                                             }
                                             n(t, i);
                                             break
                                         }
                                         e(t, i), i = i.sibling
-                                    }(i = Xl(s, t.mode, l)).return = t,
+                                    }(i = Kl(s, t.mode, l)).return = t,
                                     t = i
                                 }
                                 return a(t)
                         }
                         if ("string" === typeof s || "number" === typeof s) return s = "" + s, null !== i && 6 === i.tag ? (n(t, i.sibling), (i = r(i, s)).return = t, t = i) : (n(t, i), (i = $l(s, t.mode, l)).return = t, t = i), a(t);
                         if (Ms(s)) return g(t, i, s, l);
                         if (gt(s)) return m(t, i, s, l);
@@ -3863,83 +3863,83 @@
                         responder: t,
                         props: e
                     }
                 }
                 var Hs = Q.ReactCurrentDispatcher,
                     Ys = Q.ReactCurrentBatchConfig,
                     $s = 0,
-                    Xs = null,
                     Ks = null,
                     qs = null,
+                    Xs = null,
                     Qs = !1;
 
                 function Gs() {
                     throw Error(o(321))
                 }
 
                 function Zs(t, e) {
                     if (null === e) return !1;
                     for (var n = 0; n < e.length && n < t.length; n++)
                         if (!Wi(t[n], e[n])) return !1;
                     return !0
                 }
 
                 function Js(t, e, n, i, r, s) {
-                    if ($s = s, Xs = e, e.memoizedState = null, e.updateQueue = null, e.expirationTime = 0, Hs.current = null === t || null === t.memoizedState ? So : To, t = n(i, r), e.expirationTime === $s) {
+                    if ($s = s, Ks = e, e.memoizedState = null, e.updateQueue = null, e.expirationTime = 0, Hs.current = null === t || null === t.memoizedState ? So : To, t = n(i, r), e.expirationTime === $s) {
                         s = 0;
                         do {
                             if (e.expirationTime = 0, !(25 > s)) throw Error(o(301));
-                            s += 1, qs = Ks = null, e.updateQueue = null, Hs.current = ko, t = n(i, r)
+                            s += 1, Xs = qs = null, e.updateQueue = null, Hs.current = ko, t = n(i, r)
                         } while (e.expirationTime === $s)
                     }
-                    if (Hs.current = wo, e = null !== Ks && null !== Ks.next, $s = 0, qs = Ks = Xs = null, Qs = !1, e) throw Error(o(300));
+                    if (Hs.current = wo, e = null !== qs && null !== qs.next, $s = 0, Xs = qs = Ks = null, Qs = !1, e) throw Error(o(300));
                     return t
                 }
 
                 function to() {
                     var t = {
                         memoizedState: null,
                         baseState: null,
                         baseQueue: null,
                         queue: null,
                         next: null
                     };
-                    return null === qs ? Xs.memoizedState = qs = t : qs = qs.next = t, qs
+                    return null === Xs ? Ks.memoizedState = Xs = t : Xs = Xs.next = t, Xs
                 }
 
                 function eo() {
-                    if (null === Ks) {
-                        var t = Xs.alternate;
+                    if (null === qs) {
+                        var t = Ks.alternate;
                         t = null !== t ? t.memoizedState : null
-                    } else t = Ks.next;
-                    var e = null === qs ? Xs.memoizedState : qs.next;
-                    if (null !== e) qs = e, Ks = t;
+                    } else t = qs.next;
+                    var e = null === Xs ? Ks.memoizedState : Xs.next;
+                    if (null !== e) Xs = e, qs = t;
                     else {
                         if (null === t) throw Error(o(310));
                         t = {
-                            memoizedState: (Ks = t).memoizedState,
-                            baseState: Ks.baseState,
-                            baseQueue: Ks.baseQueue,
-                            queue: Ks.queue,
+                            memoizedState: (qs = t).memoizedState,
+                            baseState: qs.baseState,
+                            baseQueue: qs.baseQueue,
+                            queue: qs.queue,
                             next: null
-                        }, null === qs ? Xs.memoizedState = qs = t : qs = qs.next = t
+                        }, null === Xs ? Ks.memoizedState = Xs = t : Xs = Xs.next = t
                     }
-                    return qs
+                    return Xs
                 }
 
                 function no(t, e) {
                     return "function" === typeof e ? e(t) : e
                 }
 
                 function io(t) {
                     var e = eo(),
                         n = e.queue;
                     if (null === n) throw Error(o(311));
                     n.lastRenderedReducer = t;
-                    var i = Ks,
+                    var i = qs,
                         r = i.baseQueue,
                         s = n.pending;
                     if (null !== s) {
                         if (null !== r) {
                             var a = r.next;
                             r.next = s.next, s.next = a
                         }
@@ -3956,15 +3956,15 @@
                                     expirationTime: c.expirationTime,
                                     suspenseConfig: c.suspenseConfig,
                                     action: c.action,
                                     eagerReducer: c.eagerReducer,
                                     eagerState: c.eagerState,
                                     next: null
                                 };
-                                null === l ? (a = l = h, s = i) : l = l.next = h, u > Xs.expirationTime && (Xs.expirationTime = u, Sl(u))
+                                null === l ? (a = l = h, s = i) : l = l.next = h, u > Ks.expirationTime && (Ks.expirationTime = u, Sl(u))
                             } else null !== l && (l = l.next = {
                                 expirationTime: 1073741823,
                                 suspenseConfig: c.suspenseConfig,
                                 action: c.action,
                                 eagerReducer: c.eagerReducer,
                                 eagerState: c.eagerState,
                                 next: null
@@ -3998,47 +3998,47 @@
                 function so(t) {
                     var e = to();
                     return "function" === typeof t && (t = t()), e.memoizedState = e.baseState = t, t = (t = e.queue = {
                         pending: null,
                         dispatch: null,
                         lastRenderedReducer: no,
                         lastRenderedState: t
-                    }).dispatch = _o.bind(null, Xs, t), [e.memoizedState, t]
+                    }).dispatch = _o.bind(null, Ks, t), [e.memoizedState, t]
                 }
 
                 function oo(t, e, n, i) {
                     return t = {
                         tag: t,
                         create: e,
                         destroy: n,
                         deps: i,
                         next: null
-                    }, null === (e = Xs.updateQueue) ? (e = {
+                    }, null === (e = Ks.updateQueue) ? (e = {
                         lastEffect: null
-                    }, Xs.updateQueue = e, e.lastEffect = t.next = t) : null === (n = e.lastEffect) ? e.lastEffect = t.next = t : (i = n.next, n.next = t, t.next = i, e.lastEffect = t), t
+                    }, Ks.updateQueue = e, e.lastEffect = t.next = t) : null === (n = e.lastEffect) ? e.lastEffect = t.next = t : (i = n.next, n.next = t, t.next = i, e.lastEffect = t), t
                 }
 
                 function ao() {
                     return eo().memoizedState
                 }
 
                 function lo(t, e, n, i) {
                     var r = to();
-                    Xs.effectTag |= t, r.memoizedState = oo(1 | e, n, void 0, void 0 === i ? null : i)
+                    Ks.effectTag |= t, r.memoizedState = oo(1 | e, n, void 0, void 0 === i ? null : i)
                 }
 
                 function co(t, e, n, i) {
                     var r = eo();
                     i = void 0 === i ? null : i;
                     var s = void 0;
-                    if (null !== Ks) {
-                        var o = Ks.memoizedState;
+                    if (null !== qs) {
+                        var o = qs.memoizedState;
                         if (s = o.destroy, null !== i && Zs(i, o.deps)) return void oo(e, n, s, i)
                     }
-                    Xs.effectTag |= t, r.memoizedState = oo(1 | e, n, s, i)
+                    Ks.effectTag |= t, r.memoizedState = oo(1 | e, n, s, i)
                 }
 
                 function uo(t, e) {
                     return lo(516, 4, t, e)
                 }
 
                 function ho(t, e) {
@@ -4079,17 +4079,17 @@
                     e = void 0 === e ? null : e;
                     var i = n.memoizedState;
                     return null !== i && null !== e && Zs(e, i[1]) ? i[0] : (t = t(), n.memoizedState = [t, e], t)
                 }
 
                 function xo(t, e, n) {
                     var i = $r();
-                    Kr(98 > i ? 98 : i, (function() {
+                    qr(98 > i ? 98 : i, (function() {
                         t(!0)
-                    })), Kr(97 < i ? 97 : i, (function() {
+                    })), qr(97 < i ? 97 : i, (function() {
                         var i = Ys.suspense;
                         Ys.suspense = void 0 === e ? null : e;
                         try {
                             t(!1), n()
                         } finally {
                             Ys.suspense = i
                         }
@@ -4104,15 +4104,15 @@
                         suspenseConfig: r,
                         action: n,
                         eagerReducer: null,
                         eagerState: null,
                         next: null
                     };
                     var s = e.pending;
-                    if (null === s ? r.next = r : (r.next = s.next, s.next = r), e.pending = r, s = t.alternate, t === Xs || null !== s && s === Xs) Qs = !0, r.expirationTime = $s, Xs.expirationTime = $s;
+                    if (null === s ? r.next = r : (r.next = s.next, s.next = r), e.pending = r, s = t.alternate, t === Ks || null !== s && s === Ks) Qs = !0, r.expirationTime = $s, Ks.expirationTime = $s;
                     else {
                         if (0 === t.expirationTime && (null === s || 0 === s.expirationTime) && null !== (s = e.lastRenderedReducer)) try {
                             var o = e.lastRenderedState,
                                 a = s(o, n);
                             if (r.eagerReducer = s, r.eagerState = a, Wi(a, o)) return
                         } catch (l) {}
                         hl(t, i)
@@ -4152,15 +4152,15 @@
                         useReducer: function(t, e, n) {
                             var i = to();
                             return e = void 0 !== n ? n(e) : e, i.memoizedState = i.baseState = e, t = (t = i.queue = {
                                 pending: null,
                                 dispatch: null,
                                 lastRenderedReducer: t,
                                 lastRenderedState: e
-                            }).dispatch = _o.bind(null, Xs, t), [i.memoizedState, t]
+                            }).dispatch = _o.bind(null, Ks, t), [i.memoizedState, t]
                         },
                         useRef: function(t) {
                             return t = {
                                 current: t
                             }, to().memoizedState = t
                         },
                         useState: so,
@@ -4393,15 +4393,15 @@
                     return e.effectTag |= 1, null !== t && o ? (e.child = Os(e, t.child, null, s), e.child = Os(e, null, a, s)) : No(t, e, a, s), e.memoizedState = i.state, r && Mr(e, n, !0), e.child
                 }
 
                 function Yo(t) {
                     var e = t.stateNode;
                     e.pendingContext ? Sr(0, e.pendingContext, e.pendingContext !== e.context) : e.context && Sr(0, e.context, !1), Ns(t, e.containerInfo)
                 }
-                var $o, Xo, Ko, qo, Qo = {
+                var $o, Ko, qo, Xo, Qo = {
                     dehydrated: null,
                     retryTime: 0
                 };
 
                 function Go(t, e, n) {
                     var i, r = e.mode,
                         s = e.pendingProps,
@@ -4538,61 +4538,61 @@
                         case 9:
                         case 14:
                             return null;
                         case 1:
                         case 17:
                             return _r(e.type) && wr(), null;
                         case 3:
-                            return Bs(), pr(br), pr(yr), (n = e.stateNode).pendingContext && (n.context = n.pendingContext, n.pendingContext = null), null !== t && null !== t.child || !Po(e) || (e.effectTag |= 4), Xo(e), null;
+                            return Bs(), pr(br), pr(yr), (n = e.stateNode).pendingContext && (n.context = n.pendingContext, n.pendingContext = null), null !== t && null !== t.child || !Po(e) || (e.effectTag |= 4), Ko(e), null;
                         case 5:
                             Us(e), n = zs(Ls.current);
                             var s = e.type;
-                            if (null !== t && null != e.stateNode) Ko(t, e, s, i, n), t.ref !== e.ref && (e.effectTag |= 128);
+                            if (null !== t && null != e.stateNode) qo(t, e, s, i, n), t.ref !== e.ref && (e.effectTag |= 128);
                             else {
                                 if (!i) {
                                     if (null === e.stateNode) throw Error(o(166));
                                     return null
                                 }
                                 if (t = zs(Ps.current), Po(e)) {
                                     i = e.stateNode, s = e.type;
                                     var a = e.memoizedProps;
                                     switch (i[On] = e, i[Cn] = a, s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
-                                            Ke("load", i);
+                                            qe("load", i);
                                             break;
                                         case "video":
                                         case "audio":
-                                            for (t = 0; t < Gt.length; t++) Ke(Gt[t], i);
+                                            for (t = 0; t < Gt.length; t++) qe(Gt[t], i);
                                             break;
                                         case "source":
-                                            Ke("error", i);
+                                            qe("error", i);
                                             break;
                                         case "img":
                                         case "image":
                                         case "link":
-                                            Ke("error", i), Ke("load", i);
+                                            qe("error", i), qe("load", i);
                                             break;
                                         case "form":
-                                            Ke("reset", i), Ke("submit", i);
+                                            qe("reset", i), qe("submit", i);
                                             break;
                                         case "details":
-                                            Ke("toggle", i);
+                                            qe("toggle", i);
                                             break;
                                         case "input":
-                                            St(i, a), Ke("invalid", i), cn(n, "onChange");
+                                            St(i, a), qe("invalid", i), cn(n, "onChange");
                                             break;
                                         case "select":
                                             i._wrapperState = {
                                                 wasMultiple: !!a.multiple
-                                            }, Ke("invalid", i), cn(n, "onChange");
+                                            }, qe("invalid", i), cn(n, "onChange");
                                             break;
                                         case "textarea":
-                                            Ct(i, a), Ke("invalid", i), cn(n, "onChange")
+                                            Ct(i, a), qe("invalid", i), cn(n, "onChange")
                                     }
                                     for (var l in on(s, a), t = null, a)
                                         if (a.hasOwnProperty(l)) {
                                             var c = a[l];
                                             "children" === l ? "string" === typeof c ? i.textContent !== c && (t = ["children", c]) : "number" === typeof c && i.textContent !== "" + c && (t = ["children", "" + c]) : T.hasOwnProperty(l) && null != c && cn(n, l)
                                         } switch (s) {
                                         case "input":
@@ -4611,50 +4611,50 @@
                                 } else {
                                     switch (l = 9 === n.nodeType ? n : n.ownerDocument, t === ln && (t = zt(s)), t === ln ? "script" === s ? ((t = l.createElement("div")).innerHTML = "<script><\/script>", t = t.removeChild(t.firstChild)) : "string" === typeof i.is ? t = l.createElement(s, {
                                             is: i.is
                                         }) : (t = l.createElement(s), "select" === s && (l = t, i.multiple ? l.multiple = !0 : i.size && (l.size = i.size))) : t = l.createElementNS(t, s), t[On] = e, t[Cn] = i, $o(t, e, !1, !1), e.stateNode = t, l = an(s, i), s) {
                                         case "iframe":
                                         case "object":
                                         case "embed":
-                                            Ke("load", t), c = i;
+                                            qe("load", t), c = i;
                                             break;
                                         case "video":
                                         case "audio":
-                                            for (c = 0; c < Gt.length; c++) Ke(Gt[c], t);
+                                            for (c = 0; c < Gt.length; c++) qe(Gt[c], t);
                                             c = i;
                                             break;
                                         case "source":
-                                            Ke("error", t), c = i;
+                                            qe("error", t), c = i;
                                             break;
                                         case "img":
                                         case "image":
                                         case "link":
-                                            Ke("error", t), Ke("load", t), c = i;
+                                            qe("error", t), qe("load", t), c = i;
                                             break;
                                         case "form":
-                                            Ke("reset", t), Ke("submit", t), c = i;
+                                            qe("reset", t), qe("submit", t), c = i;
                                             break;
                                         case "details":
-                                            Ke("toggle", t), c = i;
+                                            qe("toggle", t), c = i;
                                             break;
                                         case "input":
-                                            St(t, i), c = wt(t, i), Ke("invalid", t), cn(n, "onChange");
+                                            St(t, i), c = wt(t, i), qe("invalid", t), cn(n, "onChange");
                                             break;
                                         case "option":
                                             c = Et(t, i);
                                             break;
                                         case "select":
                                             t._wrapperState = {
                                                 wasMultiple: !!i.multiple
                                             }, c = r({}, i, {
                                                 value: void 0
-                                            }), Ke("invalid", t), cn(n, "onChange");
+                                            }), qe("invalid", t), cn(n, "onChange");
                                             break;
                                         case "textarea":
-                                            Ct(t, i), c = Ot(t, i), Ke("invalid", t), cn(n, "onChange");
+                                            Ct(t, i), c = Ot(t, i), qe("invalid", t), cn(n, "onChange");
                                             break;
                                         default:
                                             c = i
                                     }
                                     on(s, c);
                                     var u = c;
                                     for (a in u)
@@ -4679,24 +4679,24 @@
                                     }
                                     Sn(s, i) && (e.effectTag |= 4)
                                 }
                                 null !== e.ref && (e.effectTag |= 128)
                             }
                             return null;
                         case 6:
-                            if (t && null != e.stateNode) qo(t, e, t.memoizedProps, i);
+                            if (t && null != e.stateNode) Xo(t, e, t.memoizedProps, i);
                             else {
                                 if ("string" !== typeof i && null === e.stateNode) throw Error(o(166));
                                 n = zs(Ls.current), zs(Ps.current), Po(e) ? (n = e.stateNode, i = e.memoizedProps, n[On] = e, n.nodeValue !== i && (e.effectTag |= 4)) : ((n = (9 === n.nodeType ? n : n.ownerDocument).createTextNode(i))[On] = e, e.stateNode = n)
                             }
                             return null;
                         case 13:
-                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = za) : (Wa !== Pa && Wa !== za || (Wa = Na), 0 !== Ka && null !== Ua && (Ql(Ua, ja), Gl(Ua, Ka)))), (n || i) && (e.effectTag |= 4), null);
+                            return pr(Vs), i = e.memoizedState, 0 !== (64 & e.effectTag) ? (e.expirationTime = n, e) : (n = null !== i, i = !1, null === t ? void 0 !== e.memoizedProps.fallback && Po(e) : (i = null !== (s = t.memoizedState), n || null === s || null !== (s = t.child.sibling) && (null !== (a = e.firstEffect) ? (e.firstEffect = s, s.nextEffect = a) : (e.firstEffect = e.lastEffect = s, s.nextEffect = null), s.effectTag = 8)), n && !i && 0 !== (2 & e.mode) && (null === t && !0 !== e.memoizedProps.unstable_avoidThisFallback || 0 !== (1 & Vs.current) ? Wa === Pa && (Wa = za) : (Wa !== Pa && Wa !== za || (Wa = Na), 0 !== qa && null !== Ua && (Ql(Ua, ja), Gl(Ua, qa)))), (n || i) && (e.effectTag |= 4), null);
                         case 4:
-                            return Bs(), Xo(e), null;
+                            return Bs(), Ko(e), null;
                         case 10:
                             return os(e), null;
                         case 19:
                             if (pr(Vs), null === (i = e.memoizedState)) return null;
                             if (s = 0 !== (64 & e.effectTag), null === (a = i.rendering)) {
                                 if (s) na(i, !1);
                                 else if (Wa !== Pa || null !== t && 0 !== (64 & t.effectTag))
@@ -4764,15 +4764,15 @@
                         if (n === e) break;
                         for (; null === n.sibling;) {
                             if (null === n.return || n.return === e) return;
                             n = n.return
                         }
                         n.sibling.return = n.return, n = n.sibling
                     }
-                }, Xo = function() {}, Ko = function(t, e, n, i, s) {
+                }, Ko = function() {}, qo = function(t, e, n, i, s) {
                     var o = t.memoizedProps;
                     if (o !== i) {
                         var a, l, c = e.stateNode;
                         switch (zs(Ps.current), t = null, n) {
                             case "input":
                                 o = wt(c, o), i = wt(c, i), t = [];
                                 break;
@@ -4805,15 +4805,15 @@
                                         for (l in c) !c.hasOwnProperty(l) || u && u.hasOwnProperty(l) || (n || (n = {}), n[l] = "");
                                         for (l in u) u.hasOwnProperty(l) && c[l] !== u[l] && (n || (n = {}), n[l] = u[l])
                                     } else n || (t || (t = []), t.push(a, n)), n = u;
                             else "dangerouslySetInnerHTML" === a ? (u = u ? u.__html : void 0, c = c ? c.__html : void 0, null != u && c !== u && (t = t || []).push(a, u)) : "children" === a ? c === u || "string" !== typeof u && "number" !== typeof u || (t = t || []).push(a, "" + u) : "suppressContentEditableWarning" !== a && "suppressHydrationWarning" !== a && (T.hasOwnProperty(a) ? (null != u && cn(s, a), t || c === u || (t = [])) : (t = t || []).push(a, u))
                         }
                         n && (t = t || []).push("style", n), s = t, (e.updateQueue = s) && (e.effectTag |= 4)
                     }
-                }, qo = function(t, e, n, i) {
+                }, Xo = function(t, e, n, i) {
                     n !== i && (e.effectTag |= 4)
                 };
                 var oa = "function" === typeof WeakSet ? WeakSet : Set;
 
                 function aa(t, e) {
                     var n = e.source,
                         i = e.stack;
@@ -4931,15 +4931,15 @@
                         case 0:
                         case 11:
                         case 14:
                         case 15:
                         case 22:
                             if (null !== (t = e.updateQueue) && null !== (t = t.lastEffect)) {
                                 var i = t.next;
-                                Kr(97 < n ? 97 : n, (function() {
+                                qr(97 < n ? 97 : n, (function() {
                                     var t = i;
                                     do {
                                         var n = t.destroy;
                                         if (void 0 !== n) {
                                             var r = e;
                                             try {
                                                 n()
@@ -5215,17 +5215,17 @@
                     Ua = null,
                     Va = null,
                     ja = 0,
                     Wa = Pa,
                     Ha = null,
                     Ya = 1073741823,
                     $a = 1073741823,
-                    Xa = null,
-                    Ka = 0,
-                    qa = !1,
+                    Ka = null,
+                    qa = 0,
+                    Xa = !1,
                     Qa = 0,
                     Ga = 500,
                     Za = null,
                     Ja = !1,
                     tl = null,
                     el = null,
                     nl = !1,
@@ -5293,15 +5293,15 @@
                         }
                     return null !== r && (Ua === r && (Sl(e), Wa === Na && Ql(r, ja)), Gl(r, e)), r
                 }
 
                 function fl(t) {
                     var e = t.lastExpiredTime;
                     if (0 !== e) return e;
-                    if (!ql(t, e = t.firstPendingTime)) return e;
+                    if (!Xl(t, e = t.firstPendingTime)) return e;
                     var n = t.lastPingedTime;
                     return 2 >= (t = n > (t = t.nextKnownPendingLevel) ? n : t) && e !== t ? 0 : t
                 }
 
                 function pl(t) {
                     if (0 !== t.lastExpiredTime) t.callbackExpirationTime = 1073741823, t.callbackPriority = 99, t.callbackNode = Qr(ml.bind(null, t));
                     else {
@@ -5311,15 +5311,15 @@
                         else {
                             var i = cl();
                             if (1073741823 === e ? i = 99 : 1 === e || 2 === e ? i = 95 : i = 0 >= (i = 10 * (1073741821 - e) - 10 * (1073741821 - i)) ? 99 : 250 >= i ? 98 : 5250 >= i ? 97 : 95, null !== n) {
                                 var r = t.callbackPriority;
                                 if (t.callbackExpirationTime === e && r >= i) return;
                                 n !== Br && Dr(n)
                             }
-                            t.callbackExpirationTime = e, t.callbackPriority = i, e = 1073741823 === e ? Qr(ml.bind(null, t)) : qr(i, gl.bind(null, t), {
+                            t.callbackExpirationTime = e, t.callbackPriority = i, e = 1073741823 === e ? Qr(ml.bind(null, t)) : Xr(i, gl.bind(null, t), {
                                 timeout: 10 * (1073741821 - e) - Yr()
                             }), t.callbackNode = e
                         }
                     }
                 }
 
                 function gl(t, e) {
@@ -5342,15 +5342,15 @@
                                 case Fa:
                                     throw Error(o(345));
                                 case La:
                                     Zl(t, 2 < n ? 2 : n);
                                     break;
                                 case za:
                                     if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), 1073741823 === Ya && 10 < (r = Qa + Ga - Yr())) {
-                                        if (qa) {
+                                        if (Xa) {
                                             var s = t.lastPingedTime;
                                             if (0 === s || s >= n) {
                                                 t.lastPingedTime = n, vl(t, n);
                                                 break
                                             }
                                         }
                                         if (0 !== (s = fl(t)) && s !== n) break;
@@ -5360,15 +5360,15 @@
                                         }
                                         t.timeoutHandle = kn(Dl.bind(null, t), r);
                                         break
                                     }
                                     Dl(t);
                                     break;
                                 case Na:
-                                    if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), qa && (0 === (r = t.lastPingedTime) || r >= n)) {
+                                    if (Ql(t, n), n === (i = t.lastSuspendedTime) && (t.nextKnownPendingLevel = El(r)), Xa && (0 === (r = t.lastPingedTime) || r >= n)) {
                                         t.lastPingedTime = n, vl(t, n);
                                         break
                                     }
                                     if (0 !== (r = fl(t)) && r !== n) break;
                                     if (0 !== i && i !== n) {
                                         t.lastPingedTime = i;
                                         break
@@ -5376,17 +5376,17 @@
                                     if (1073741823 !== $a ? i = 10 * (1073741821 - $a) - Yr() : 1073741823 === Ya ? i = 0 : (i = 10 * (1073741821 - Ya) - 5e3, 0 > (i = (r = Yr()) - i) && (i = 0), (n = 10 * (1073741821 - n) - r) < (i = (120 > i ? 120 : 480 > i ? 480 : 1080 > i ? 1080 : 1920 > i ? 1920 : 3e3 > i ? 3e3 : 4320 > i ? 4320 : 1960 * Ma(i / 1960)) - i) && (i = n)), 10 < i) {
                                         t.timeoutHandle = kn(Dl.bind(null, t), i);
                                         break
                                     }
                                     Dl(t);
                                     break;
                                 case Ba:
-                                    if (1073741823 !== Ya && null !== Xa) {
+                                    if (1073741823 !== Ya && null !== Ka) {
                                         s = Ya;
-                                        var a = Xa;
+                                        var a = Ka;
                                         if (0 >= (i = 0 | a.busyMinDurationMs) ? i = 0 : (r = 0 | a.busyDelayMs, i = (s = Yr() - (10 * (1073741821 - s) - (0 | a.timeoutMs || 5e3))) <= r ? 0 : r + i - s), 10 < i) {
                                             Ql(t, n), t.timeoutHandle = kn(Dl.bind(null, t), i);
                                             break
                                         }
                                     }
                                     Dl(t);
                                     break;
@@ -5462,26 +5462,26 @@
                                     pr(Vs);
                                     break;
                                 case 10:
                                     os(i)
                             }
                             n = n.return
                         }
-                    Ua = t, Va = Wl(t.current, null), ja = e, Wa = Pa, Ha = null, $a = Ya = 1073741823, Xa = null, Ka = 0, qa = !1
+                    Ua = t, Va = Wl(t.current, null), ja = e, Wa = Pa, Ha = null, $a = Ya = 1073741823, Ka = null, qa = 0, Xa = !1
                 }
 
                 function xl(t, e) {
                     for (;;) {
                         try {
                             if (ss(), Hs.current = wo, Qs)
-                                for (var n = Xs.memoizedState; null !== n;) {
+                                for (var n = Ks.memoizedState; null !== n;) {
                                     var i = n.queue;
                                     null !== i && (i.pending = null), n = n.next
                                 }
-                            if ($s = 0, qs = Ks = Xs = null, Qs = !1, null === Va || null === Va.return) return Wa = Fa, Ha = e, Va = null;
+                            if ($s = 0, Xs = qs = Ks = null, Qs = !1, null === Va || null === Va.return) return Wa = Fa, Ha = e, Va = null;
                             t: {
                                 var r = t,
                                     s = Va.return,
                                     o = Va,
                                     a = e;
                                 if (e = ja, o.effectTag |= 2048, o.firstEffect = o.lastEffect = null, null !== a && "object" === typeof a && "function" === typeof a.then) {
                                     var l = a;
@@ -5560,19 +5560,19 @@
 
                 function _l() {
                     var t = Ia.current;
                     return Ia.current = wo, null === t ? wo : t
                 }
 
                 function wl(t, e) {
-                    t < Ya && 2 < t && (Ya = t), null !== e && t < $a && 2 < t && ($a = t, Xa = e)
+                    t < Ya && 2 < t && (Ya = t), null !== e && t < $a && 2 < t && ($a = t, Ka = e)
                 }
 
                 function Sl(t) {
-                    t > Ka && (Ka = t)
+                    t > qa && (qa = t)
                 }
 
                 function Tl() {
                     for (; null !== Va;) Va = Ml(Va)
                 }
 
                 function kl() {
@@ -5612,15 +5612,15 @@
                 function El(t) {
                     var e = t.expirationTime;
                     return e > (t = t.childExpirationTime) ? e : t
                 }
 
                 function Dl(t) {
                     var e = $r();
-                    return Kr(99, Ol.bind(null, t, e)), null
+                    return qr(99, Ol.bind(null, t, e)), null
                 }
 
                 function Ol(t, e) {
                     do {
                         Al()
                     } while (null !== il);
                     if ((Ra & (Ca | Aa)) !== Da) throw Error(o(327));
@@ -5628,15 +5628,15 @@
                         i = t.finishedExpirationTime;
                     if (null === n) return null;
                     if (t.finishedWork = null, t.finishedExpirationTime = 0, n === t.current) throw Error(o(177));
                     t.callbackNode = null, t.callbackExpirationTime = 0, t.callbackPriority = 90, t.nextKnownPendingLevel = 0;
                     var r = El(n);
                     if (t.firstPendingTime = r, i <= t.lastSuspendedTime ? t.firstSuspendedTime = t.lastSuspendedTime = t.nextKnownPendingLevel = 0 : i <= t.firstSuspendedTime && (t.firstSuspendedTime = i - 1), i <= t.lastPingedTime && (t.lastPingedTime = 0), i <= t.lastExpiredTime && (t.lastExpiredTime = 0), t === Ua && (Va = Ua = null, ja = 0), 1 < n.effectTag ? null !== n.lastEffect ? (n.lastEffect.nextEffect = n, r = n.firstEffect) : r = n : r = n.firstEffect, null !== r) {
                         var s = Ra;
-                        Ra |= Aa, Ea.current = null, _n = Xe;
+                        Ra |= Aa, Ea.current = null, _n = Ke;
                         var a = gn();
                         if (mn(a)) {
                             if ("selectionStart" in a) var l = {
                                 start: a.selectionStart,
                                 end: a.selectionEnd
                             };
                             else t: {
@@ -5679,15 +5679,15 @@
                                 end: 0
                             }
                         } else l = null;
                         wn = {
                             activeElementDetached: null,
                             focusedElem: a,
                             selectionRange: l
-                        }, Xe = !1, Za = r;
+                        }, Ke = !1, Za = r;
                         do {
                             try {
                                 Cl()
                             } catch (M) {
                                 if (null === Za) throw Error(o(330));
                                 Ll(Za, M), Za = Za.nextEffect
                             }
@@ -5735,15 +5735,15 @@
                             for (w = x; w = w.parentNode;) 1 === w.nodeType && _.push({
                                 element: w,
                                 left: w.scrollLeft,
                                 top: w.scrollTop
                             });
                             for ("function" === typeof x.focus && x.focus(), x = 0; x < _.length; x++)(w = _[x]).element.scrollLeft = w.left, w.element.scrollTop = w.top
                         }
-                        Xe = !!_n, wn = _n = null, t.current = n, Za = r;
+                        Ke = !!_n, wn = _n = null, t.current = n, Za = r;
                         do {
                             try {
                                 for (x = t; null !== Za;) {
                                     var S = Za.effectTag;
                                     if (36 & S && da(x, Za.alternate, Za), 128 & S) {
                                         _ = void 0;
                                         var T = Za.ref;
@@ -5767,24 +5767,24 @@
                     if (0 === (e = t.firstPendingTime) && (el = null), 1073741823 === e ? t === al ? ol++ : (ol = 0, al = t) : ol = 0, "function" === typeof Bl && Bl(n.stateNode, i), pl(t), Ja) throw Ja = !1, t = tl, tl = null, t;
                     return (Ra & Oa) !== Da || Gr(), null
                 }
 
                 function Cl() {
                     for (; null !== Za;) {
                         var t = Za.effectTag;
-                        0 !== (256 & t) && ca(Za.alternate, Za), 0 === (512 & t) || nl || (nl = !0, qr(97, (function() {
+                        0 !== (256 & t) && ca(Za.alternate, Za), 0 === (512 & t) || nl || (nl = !0, Xr(97, (function() {
                             return Al(), null
                         }))), Za = Za.nextEffect
                     }
                 }
 
                 function Al() {
                     if (90 !== rl) {
                         var t = 97 < rl ? 97 : rl;
-                        return rl = 90, Kr(t, Pl)
+                        return rl = 90, qr(t, Pl)
                     }
                 }
 
                 function Pl() {
                     if (null === il) return !1;
                     var t = il;
                     if (il = null, (Ra & (Ca | Aa)) !== Da) throw Error(o(331));
@@ -5829,15 +5829,15 @@
                             }
                             n = n.return
                         }
                 }
 
                 function zl(t, e, n) {
                     var i = t.pingCache;
-                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === za && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : qa = !0 : ql(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
+                    null !== i && i.delete(e), Ua === t && ja === n ? Wa === Na || Wa === za && 1073741823 === Ya && Yr() - Qa < Ga ? vl(t, ja) : Xa = !0 : Xl(t, n) && (0 !== (e = t.lastPingedTime) && e < n || (t.lastPingedTime = n, pl(t)))
                 }
 
                 function Nl(t, e) {
                     var n = t.stateNode;
                     null !== n && n.delete(e), 0 === (e = 0) && (e = ul(e = cl(), t, null)), null !== (t = dl(t, e)) && pl(t)
                 }
                 ka = function(t, e, n) {
@@ -6088,27 +6088,27 @@
                     return (t = Vl(7, t, i, e)).expirationTime = n, t
                 }
 
                 function $l(t, e, n) {
                     return (t = Vl(6, t, null, e)).expirationTime = n, t
                 }
 
-                function Xl(t, e, n) {
+                function Kl(t, e, n) {
                     return (e = Vl(4, null !== t.children ? t.children : [], t.key, e)).expirationTime = n, e.stateNode = {
                         containerInfo: t.containerInfo,
                         pendingChildren: null,
                         implementation: t.implementation
                     }, e
                 }
 
-                function Kl(t, e, n) {
+                function ql(t, e, n) {
                     this.tag = e, this.current = null, this.containerInfo = t, this.pingCache = this.pendingChildren = null, this.finishedExpirationTime = 0, this.finishedWork = null, this.timeoutHandle = -1, this.pendingContext = this.context = null, this.hydrate = n, this.callbackNode = null, this.callbackPriority = 90, this.lastExpiredTime = this.lastPingedTime = this.nextKnownPendingLevel = this.lastSuspendedTime = this.firstSuspendedTime = this.firstPendingTime = 0
                 }
 
-                function ql(t, e) {
+                function Xl(t, e) {
                     var n = t.firstSuspendedTime;
                     return t = t.lastSuspendedTime, 0 !== n && n >= e && t <= e
                 }
 
                 function Ql(t, e) {
                     var n = t.firstSuspendedTime,
                         i = t.lastSuspendedTime;
@@ -6173,15 +6173,15 @@
                 }
 
                 function nc(t, e) {
                     ec(t, e), (t = t.alternate) && ec(t, e)
                 }
 
                 function ic(t, e, n) {
-                    var i = new Kl(t, e, n = null != n && !0 === n.hydrate),
+                    var i = new ql(t, e, n = null != n && !0 === n.hydrate),
                         r = Vl(3, null, null, 2 === e ? 7 : 1 === e ? 3 : 0);
                     i.current = r, r.stateNode = i, hs(r), t[An] = i.current, n && 0 !== e && function(t, e) {
                         var n = Jt(e);
                         Ie.forEach((function(t) {
                             ge(t, e, n)
                         })), Ee.forEach((function(t) {
                             ge(t, e, n)
@@ -6281,15 +6281,15 @@
                         case "select":
                             null != (e = n.value) && Dt(t, !!n.multiple, e, !1)
                     }
                 }, F = yl, L = function(t, e, n, i, r) {
                     var s = Ra;
                     Ra |= 4;
                     try {
-                        return Kr(98, t.bind(null, e, n, i, r))
+                        return qr(98, t.bind(null, e, n, i, r))
                     } finally {
                         (Ra = s) === Da && Gr()
                     }
                 }, z = function() {
                     (Ra & (1 | Ca | Aa)) === Da && (function() {
                         if (null !== sl) {
                             var t = sl;
@@ -6365,15 +6365,15 @@
                     }
                     return t = null === (t = ie(e)) ? null : t.stateNode
                 }, e.flushSync = function(t, e) {
                     if ((Ra & (Ca | Aa)) !== Da) throw Error(o(187));
                     var n = Ra;
                     Ra |= 1;
                     try {
-                        return Kr(99, t.bind(null, e))
+                        return qr(99, t.bind(null, e))
                     } finally {
                         Ra = n, Gr()
                     }
                 }, e.hydrate = function(t, e, n) {
                     if (!rc(e)) throw Error(o(200));
                     return sc(null, t, e, !0, n)
                 }, e.render = function(t, e, n) {
@@ -7353,24 +7353,24 @@
         "function" === typeof SuppressedError && SuppressedError;
         const j = new TextDecoder("utf-8"),
             W = t => j.decode(t),
             H = new TextEncoder,
             Y = t => H.encode(t),
             $ = "undefined" !== typeof SharedArrayBuffer ? SharedArrayBuffer : ArrayBuffer;
 
-        function X(t, e) {
+        function K(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0,
                 i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : e.byteLength;
             const r = t.byteLength,
                 s = new Uint8Array(t.buffer, t.byteOffset, r),
                 o = new Uint8Array(e.buffer, e.byteOffset, Math.min(i, r));
             return s.set(o, n), t
         }
 
-        function K(t, e) {
+        function q(t, e) {
             const n = function(t) {
                     const e = t[0] ? [t[0]] : [];
                     let n, i, r, s;
                     for (let o, a, l = 0, c = 0, u = t.length; ++l < u;) o = e[c], a = t[l], !o || !a || o.buffer !== a.buffer || a.byteOffset < o.byteOffset ? a && (e[++c] = a) : (({
                         byteOffset: n,
                         byteLength: r
                     } = o), ({
@@ -7381,39 +7381,39 @@
                 }(t),
                 i = n.reduce(((t, e) => t + e.byteLength), 0);
             let r, s, o, a = 0,
                 l = -1;
             const c = Math.min(e || Number.POSITIVE_INFINITY, i);
             for (const u = n.length; ++l < u;) {
                 if (r = n[l], s = r.subarray(0, Math.min(r.length, c - a)), c <= a + s.length) {
-                    s.length < r.length ? n[l] = r.subarray(s.length) : s.length === r.length && l++, o ? X(o, s, a) : o = s;
+                    s.length < r.length ? n[l] = r.subarray(s.length) : s.length === r.length && l++, o ? K(o, s, a) : o = s;
                     break
                 }
-                X(o || (o = new Uint8Array(c)), s, a), a += s.length
+                K(o || (o = new Uint8Array(c)), s, a), a += s.length
             }
             return [o || new Uint8Array(0), n.slice(l), i - (o ? o.byteLength : 0)]
         }
 
-        function q(t, e) {
+        function X(t, e) {
             let n = E(e) ? e.value : e;
-            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Y(n)), n instanceof ArrayBuffer || n instanceof $ ? new t(n) : F(n) ? q(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
+            return n instanceof t ? t === Uint8Array ? new t(n.buffer, n.byteOffset, n.byteLength) : n : n ? ("string" === typeof n && (n = Y(n)), n instanceof ArrayBuffer || n instanceof $ ? new t(n) : F(n) ? X(t, n.bytes()) : ArrayBuffer.isView(n) ? n.byteLength <= 0 ? new t(0) : new t(n.buffer, n.byteOffset, n.byteLength / t.BYTES_PER_ELEMENT) : t.from(n)) : new t(0)
         }
-        const Q = t => q(Int32Array, t),
-            G = t => q(Uint8Array, t),
+        const Q = t => X(Int32Array, t),
+            G = t => X(Uint8Array, t),
             Z = t => (t.next(), t);
 
         function* J(t, e) {
             const n = function*(t) {
                     yield t
                 },
                 i = "string" === typeof e || ArrayBuffer.isView(e) || e instanceof ArrayBuffer || e instanceof $ ? n(e) : k(e) ? e : n(e);
             return yield* Z(function*(e) {
                 let n = null;
                 do {
-                    n = e.next(yield q(t, n))
+                    n = e.next(yield X(t, n))
                 } while (!n.done)
             }(i[Symbol.iterator]())), new t
         }
 
         function tt(t, e) {
             return R(this, arguments, (function*() {
                 if (T(e)) return yield B(yield B(yield* U(V(tt(t, yield B(e))))));
@@ -7432,15 +7432,15 @@
                             }(t[Symbol.iterator]())))))
                         }))
                     }(e) : M(e) ? e : n(e);
                 return yield B(yield* U(V(Z(function(e) {
                     return R(this, arguments, (function*() {
                         let n = null;
                         do {
-                            n = yield B(e.next(yield yield B(q(t, n))))
+                            n = yield B(e.next(yield yield B(X(t, n))))
                         } while (!n.done)
                     }))
                 }(i[Symbol.asyncIterator]()))))), yield B(new t)
             }))
         }
 
         function et(t, e, n) {
@@ -7450,15 +7450,15 @@
             }
             return n
         }
         const nt = Symbol.for("isArrowBigNum");
 
         function it(t) {
             for (var e = arguments.length, n = new Array(e > 1 ? e - 1 : 0), i = 1; i < e; i++) n[i - 1] = arguments[i];
-            return 0 === n.length ? Object.setPrototypeOf(q(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
+            return 0 === n.length ? Object.setPrototypeOf(X(this.TypedArray, t), this.constructor.prototype) : Object.setPrototypeOf(new this.TypedArray(t, ...n), this.constructor.prototype)
         }
 
         function rt() {
             for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
             return it.apply(this, e)
         }
 
@@ -7917,39 +7917,39 @@
                 return c.Struct
             }
             toString() {
                 return "Struct<{".concat(this.children.map((t => "".concat(t.name, ":").concat(t.type))).join(", "), "}>")
             }
         }
         kt = Symbol.toStringTag, $t[kt] = (t => (t.children = null, t[Symbol.toStringTag] = "Struct"))($t.prototype);
-        class Xt extends At {
+        class Kt extends At {
             constructor(t, e, n) {
                 super(), this.mode = t, this.children = n, this.typeIds = e = Int32Array.from(e), this.typeIdToChildIndex = e.reduce(((t, e, n) => (t[e] = n) && t || t), Object.create(null))
             }
             get typeId() {
                 return c.Union
             }
             toString() {
                 return "".concat(this[Symbol.toStringTag], "<").concat(this.children.map((t => "".concat(t.type))).join(" | "), ">")
             }
         }
-        Mt = Symbol.toStringTag, Xt[Mt] = (t => (t.mode = null, t.typeIds = null, t.children = null, t.typeIdToChildIndex = null, t.ArrayType = Int8Array, t[Symbol.toStringTag] = "Union"))(Xt.prototype);
-        class Kt extends At {
+        Mt = Symbol.toStringTag, Kt[Mt] = (t => (t.mode = null, t.typeIds = null, t.children = null, t.typeIdToChildIndex = null, t.ArrayType = Int8Array, t[Symbol.toStringTag] = "Union"))(Kt.prototype);
+        class qt extends At {
             constructor(t) {
                 super(), this.byteWidth = t
             }
             get typeId() {
                 return c.FixedSizeBinary
             }
             toString() {
                 return "FixedSizeBinary[".concat(this.byteWidth, "]")
             }
         }
-        It = Symbol.toStringTag, Kt[It] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(Kt.prototype);
-        class qt extends At {
+        It = Symbol.toStringTag, qt[It] = (t => (t.byteWidth = null, t.ArrayType = Uint8Array, t[Symbol.toStringTag] = "FixedSizeBinary"))(qt.prototype);
+        class Xt extends At {
             constructor(t, e) {
                 super(), this.listSize = t, this.children = [e]
             }
             get typeId() {
                 return c.FixedSizeList
             }
             get valueType() {
@@ -7961,15 +7961,15 @@
             get ArrayType() {
                 return this.valueType.ArrayType
             }
             toString() {
                 return "FixedSizeList[".concat(this.listSize, "]<").concat(this.valueType, ">")
             }
         }
-        Et = Symbol.toStringTag, qt[Et] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(qt.prototype);
+        Et = Symbol.toStringTag, Xt[Et] = (t => (t.children = null, t.listSize = null, t[Symbol.toStringTag] = "FixedSizeList"))(Xt.prototype);
         class Qt extends At {
             constructor(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                 super(), this.children = [t], this.keysSorted = e
             }
             get typeId() {
                 return c.Map
@@ -8758,27 +8758,27 @@
             },
             $e = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return ((t, e) => t[e + 1] / 1e6 * 4294967296 + (t[e] >>> 0) / 1e6)(n, 2 * e)
             },
-            Xe = (t, e) => {
+            Ke = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            Ke = (t, e) => {
+            qe = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
-            qe = (t, e) => {
+            Xe = (t, e) => {
                 let {
                     values: n
                 } = t;
                 return n[e]
             },
             Qe = (t, e) => {
                 let {
@@ -8863,23 +8863,23 @@
                     return Ye(t, e);
                 case o.NANOSECOND:
                     return $e(t, e)
             }
         })), Fe.prototype.visitTimestampSecond = Le(We), Fe.prototype.visitTimestampMillisecond = Le(He), Fe.prototype.visitTimestampMicrosecond = Le(Ye), Fe.prototype.visitTimestampNanosecond = Le($e), Fe.prototype.visitTime = Le(((t, e) => {
             switch (t.type.unit) {
                 case o.SECOND:
-                    return Xe(t, e);
-                case o.MILLISECOND:
                     return Ke(t, e);
-                case o.MICROSECOND:
+                case o.MILLISECOND:
                     return qe(t, e);
+                case o.MICROSECOND:
+                    return Xe(t, e);
                 case o.NANOSECOND:
                     return Qe(t, e)
             }
-        })), Fe.prototype.visitTimeSecond = Le(Xe), Fe.prototype.visitTimeMillisecond = Le(Ke), Fe.prototype.visitTimeMicrosecond = Le(qe), Fe.prototype.visitTimeNanosecond = Le(Qe), Fe.prototype.visitDecimal = Le(((t, e) => {
+        })), Fe.prototype.visitTimeSecond = Le(Ke), Fe.prototype.visitTimeMillisecond = Le(qe), Fe.prototype.visitTimeMicrosecond = Le(Xe), Fe.prototype.visitTimeNanosecond = Le(Qe), Fe.prototype.visitDecimal = Le(((t, e) => {
             let {
                 values: n,
                 stride: i
             } = t;
             return ht.decimal(n.subarray(i * e, i * (e + 1)))
         })), Fe.prototype.visitList = Le(((t, e) => {
             const {
@@ -9453,15 +9453,15 @@
         var Wn;
         const Hn = {},
             Yn = {};
         class $n {
             constructor(t) {
                 var e, n, i;
                 const r = t[0] instanceof $n ? t.flatMap((t => t.data)) : t;
-                if (0 === r.length || r.some((t => !(t instanceof Kn)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
+                if (0 === r.length || r.some((t => !(t instanceof qn)))) throw new TypeError("Vector constructor expects an Array of Data instances.");
                 const s = null === (e = r[0]) || void 0 === e ? void 0 : e.type;
                 switch (r.length) {
                     case 0:
                         this._offsets = [0];
                         break;
                     case 1: {
                         const {
@@ -9577,22 +9577,22 @@
                 }))) : null
             }
             get isMemoized() {
                 return !!At.isDictionary(this.type) && this.data[0].dictionary.isMemoized
             }
             memoize() {
                 if (At.isDictionary(this.type)) {
-                    const t = new Xn(this.data[0].dictionary),
+                    const t = new Kn(this.data[0].dictionary),
                         e = this.data.map((e => {
                             const n = e.clone();
                             return n.dictionary = t, n
                         }));
                     return new $n(e)
                 }
-                return new Xn(this)
+                return new Kn(this)
             }
             unmemoize() {
                 if (At.isDictionary(this.type) && this.isMemoized) {
                     const t = this.data[0].dictionary.unmemoize(),
                         e = this.data.map((e => {
                             const n = e.clone();
                             return n.dictionary = t, n
@@ -9631,15 +9631,15 @@
                     getByteLength: {
                         value: xn(jn.getVisitFnByTypeId(n))
                     }
                 })
             }
             return "Vector"
         })($n.prototype);
-        class Xn extends $n {
+        class Kn extends $n {
             constructor(t) {
                 super(t.data);
                 const e = this.get,
                     n = this.set,
                     i = this.slice,
                     r = new Array(this.length);
                 Object.defineProperty(this, "get", {
@@ -9650,29 +9650,29 @@
                         return r[t] = i, i
                     }
                 }), Object.defineProperty(this, "set", {
                     value(t, e) {
                         n.call(this, t, e), r[t] = e
                     }
                 }), Object.defineProperty(this, "slice", {
-                    value: (t, e) => new Xn(i.call(this, t, e))
+                    value: (t, e) => new Kn(i.call(this, t, e))
                 }), Object.defineProperty(this, "isMemoized", {
                     value: !0
                 }), Object.defineProperty(this, "unmemoize", {
                     value: () => new $n(this.data)
                 }), Object.defineProperty(this, "memoize", {
                     value: () => this
                 })
             }
         }
-        class Kn {
+        class qn {
             constructor(t, e, n, i, r) {
                 let s, o = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : [],
                     a = arguments.length > 6 ? arguments[6] : void 0;
-                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof Kn ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = te(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
+                this.type = t, this.children = o, this.dictionary = a, this.offset = Math.floor(Math.max(e || 0, 0)), this.length = Math.floor(Math.max(n || 0, 0)), this._nullCount = Math.floor(Math.max(i || 0, -1)), r instanceof qn ? (this.stride = r.stride, this.values = r.values, this.typeIds = r.typeIds, this.nullBitmap = r.nullBitmap, this.valueOffsets = r.valueOffsets) : (this.stride = te(t), r && ((s = r[0]) && (this.valueOffsets = s), (s = r[1]) && (this.values = s), (s = r[2]) && (this.nullBitmap = s), (s = r[3]) && (this.typeIds = s))), this.nullable = 0 !== this._nullCount && this.nullBitmap && this.nullBitmap.byteLength > 0
             }
             get typeId() {
                 return this.type.typeId
             }
             get ArrayType() {
                 return this.type.ArrayType
             }
@@ -9720,15 +9720,15 @@
             clone() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.type,
                     e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.offset,
                     n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.length,
                     i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : this._nullCount,
                     r = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : this,
                     s = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : this.children;
-                return new Kn(t, e, n, i, r, s, this.dictionary)
+                return new qn(t, e, n, i, r, s, this.dictionary)
             }
             slice(t, e) {
                 const {
                     stride: n,
                     typeId: i,
                     children: r
                 } = this, s = +(0 === this._nullCount) - 1, o = 16 === i ? n : 1, a = this._sliceBuffers(t, e, n, i);
@@ -9751,137 +9751,137 @@
                 } = this;
                 return (r = s[u.TYPE]) && (s[u.TYPE] = r.subarray(t, t + e)), (r = s[u.OFFSET]) && (s[u.OFFSET] = r.subarray(t, t + e + 1)) || (r = s[u.DATA]) && (s[u.DATA] = 6 === i ? r : r.subarray(n * t, n * (t + e))), s
             }
             _sliceChildren(t, e, n) {
                 return t.map((t => t.slice(e, n)))
             }
         }
-        Kn.prototype.children = Object.freeze([]);
-        class qn extends ee {
+        qn.prototype.children = Object.freeze([]);
+        class Xn extends ee {
             visit(t) {
                 return this.getVisitFn(t.type).call(this, t)
             }
             visitNull(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     length: i = 0
                 } = t;
-                return new Kn(e, n, i, 0)
+                return new qn(e, n, i, 0)
             }
             visitBool(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length >> 3,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitInt(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitFloat(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length,
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitUtf8(t) {
                 const {
                     type: e,
                     offset: n = 0
                 } = t, i = G(t.data), r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, o, a, [s, i, r])
+                return new qn(e, n, o, a, [s, i, r])
             }
             visitBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
                 } = t, i = G(t.data), r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, o, a, [s, i, r])
+                return new qn(e, n, o, a, [s, i, r])
             }
             visitFixedSizeBinary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitDate(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitTimestamp(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitTime(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitDecimal(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitList(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     child: i
                 } = t, r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, o, a, [s, void 0, r], [i])
+                return new qn(e, n, o, a, [s, void 0, r], [i])
             }
             visitStruct(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
                 } = t, r = G(t.nullBitmap), {
@@ -9889,83 +9889,83 @@
                         let {
                             length: n
                         } = e;
                         return Math.max(t, n)
                     }), 0),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, void 0, r], i)
+                return new qn(e, n, s, o, [void 0, void 0, r], i)
             }
             visitUnion(t) {
                 const {
                     type: e,
                     offset: n = 0,
                     children: i = []
-                } = t, r = G(t.nullBitmap), s = q(e.ArrayType, t.typeIds), {
+                } = t, r = G(t.nullBitmap), s = X(e.ArrayType, t.typeIds), {
                     length: o = s.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                if (At.isSparseUnion(e)) return new Kn(e, n, o, a, [void 0, void 0, r, s], i);
+                if (At.isSparseUnion(e)) return new qn(e, n, o, a, [void 0, void 0, r, s], i);
                 const l = Q(t.valueOffsets);
-                return new Kn(e, n, o, a, [l, void 0, r, s], i)
+                return new qn(e, n, o, a, [l, void 0, r, s], i)
             }
             visitDictionary(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.indices.ArrayType, t.data), {
-                    dictionary: s = new $n([(new qn).visit({
+                } = t, i = G(t.nullBitmap), r = X(e.indices.ArrayType, t.data), {
+                    dictionary: s = new $n([(new Xn).visit({
                         type: e.dictionary
                     })])
                 } = t, {
                     length: o = r.length,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, o, a, [void 0, r, i], [], s)
+                return new qn(e, n, o, a, [void 0, r, i], [], s)
             }
             visitInterval(t) {
                 const {
                     type: e,
                     offset: n = 0
-                } = t, i = G(t.nullBitmap), r = q(e.ArrayType, t.data), {
+                } = t, i = G(t.nullBitmap), r = X(e.ArrayType, t.data), {
                     length: s = r.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, r, i])
+                return new qn(e, n, s, o, [void 0, r, i])
             }
             visitFixedSizeList(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new qn).visit({
+                    child: i = (new Xn).visit({
                         type: e.valueType
                     })
                 } = t, r = G(t.nullBitmap), {
                     length: s = i.length / te(e),
                     nullCount: o = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, s, o, [void 0, void 0, r], [i])
+                return new qn(e, n, s, o, [void 0, void 0, r], [i])
             }
             visitMap(t) {
                 const {
                     type: e,
                     offset: n = 0,
-                    child: i = (new qn).visit({
+                    child: i = (new Xn).visit({
                         type: e.childType
                     })
                 } = t, r = G(t.nullBitmap), s = Q(t.valueOffsets), {
                     length: o = s.length - 1,
                     nullCount: a = (t.nullBitmap ? -1 : 0)
                 } = t;
-                return new Kn(e, n, o, a, [s, void 0, r], [i])
+                return new qn(e, n, o, a, [s, void 0, r], [i])
             }
         }
 
         function Qn(t) {
-            return (new qn).visit(t)
+            return (new Xn).visit(t)
         }
         class Gn {
             constructor() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : [],
                     e = arguments.length > 1 ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0;
                 this.fields = t || [], this.metadata = e || new Map, n || (n = ti(t)), this.dictionaries = n
@@ -10130,15 +10130,15 @@
                         if ([, this.data = Qn({
                                 nullCount: 0,
                                 type: new $t(this.schema.fields),
                                 children: this.schema.fields.map((t => Qn({
                                     type: t.type,
                                     nullCount: 0
                                 })))
-                            })] = e, !(this.data instanceof Kn)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
+                            })] = e, !(this.data instanceof qn)) throw new TypeError("RecordBatch constructor expects a [Schema, Data] pair.");
                         [this.schema, this.data] = mi(this.schema, this.data.children);
                         break;
                     case 1: {
                         const [t] = e, {
                             fields: n,
                             children: i,
                             length: r
@@ -10363,15 +10363,15 @@
                 if (0 === i.length) return this.batches = [], this.schema = new Gn([]), this._offsets = [0], this;
                 let s, o;
                 i[0] instanceof Gn && (s = i.shift()), i[i.length - 1] instanceof Uint32Array && (o = i.pop());
                 const a = t => {
                         if (t) {
                             if (t instanceof gi) return [t];
                             if (t instanceof _i) return t.batches;
-                            if (t instanceof Kn) {
+                            if (t instanceof qn) {
                                 if (t.type instanceof $t) return [new gi(new Gn(t.type.children), t)]
                             } else {
                                 if (Array.isArray(t)) return t.flatMap((t => a(t)));
                                 if ("function" === typeof t[Symbol.iterator]) return [...t].flatMap((t => a(t)));
                                 if ("object" === typeof t) {
                                     const e = Object.keys(t),
                                         n = e.map((e => new $n([t[e]]))),
@@ -11410,22 +11410,22 @@
             static encode(t, e) {
                 const {
                     metaDataLength: n
                 } = e, i = new Vi(e.offset, 0), r = new Vi(e.bodyLength, 0);
                 return wi.createBlock(t, i, n, r)
             }
         }
-        const Xi = {
-                fromIterable: t => Ki(function*(t) {
+        const Ki = {
+                fromIterable: t => qi(function*(t) {
                     let e, n, i, r, s = !1,
                         o = [],
                         a = 0;
 
                     function l() {
-                        return "peek" === i ? K(o, r)[0] : ([n, o, a] = K(o, r), n)
+                        return "peek" === i ? q(o, r)[0] : ([n, o, a] = q(o, r), n)
                     }({
                         cmd: i,
                         size: r
                     } = yield null);
                     const c = (u = t, J(Uint8Array, u))[Symbol.iterator]();
                     var u;
                     try {
@@ -11444,22 +11444,22 @@
                     } catch (h) {
                         (s = !0) && "function" === typeof c.throw && c.throw(h)
                     } finally {
                         !1 === s && "function" === typeof c.return && c.return(null)
                     }
                     return null
                 }(t)),
-                fromAsyncIterable: t => Ki(function(t) {
+                fromAsyncIterable: t => qi(function(t) {
                     return R(this, arguments, (function*() {
                         let e, n, i, r, s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === i ? K(o, r)[0] : ([n, o, a] = K(o, r), n)
+                            return "peek" === i ? q(o, r)[0] : ([n, o, a] = q(o, r), n)
                         }({
                             cmd: i,
                             size: r
                         } = yield yield B(null));
                         const c = (u = t, tt(Uint8Array, u))[Symbol.asyncIterator]();
                         var u;
                         try {
@@ -11479,28 +11479,28 @@
                             (s = !0) && "function" === typeof c.throw && (yield B(c.throw(h)))
                         } finally {
                             !1 === s && "function" === typeof c.return && (yield B(c.return(new Uint8Array(0))))
                         }
                         return yield B(null)
                     }))
                 }(t)),
-                fromDOMStream: t => Ki(function(t) {
+                fromDOMStream: t => qi(function(t) {
                     return R(this, arguments, (function*() {
                         let e, n, i, r = !1,
                             s = !1,
                             o = [],
                             a = 0;
 
                         function l() {
-                            return "peek" === n ? K(o, i)[0] : ([e, o, a] = K(o, i), e)
+                            return "peek" === n ? q(o, i)[0] : ([e, o, a] = q(o, i), e)
                         }({
                             cmd: n,
                             size: i
                         } = yield yield B(null));
-                        const c = new qi(t);
+                        const c = new Xi(t);
                         try {
                             do {
                                 if (({
                                         done: r,
                                         value: e
                                     } = Number.isNaN(i - a) ? yield B(c.read()): yield B(c.read(i - a))), !r && e.byteLength > 0 && (o.push(G(e)), a += e.byteLength), r || i <= a)
                                     do {
@@ -11514,25 +11514,25 @@
                             (s = !0) && (yield B(c.cancel(u)))
                         } finally {
                             !1 === s ? yield B(c.cancel()): t.locked && c.releaseLock()
                         }
                         return yield B(null)
                     }))
                 }(t)),
-                fromNodeStream: t => Ki(function(t) {
+                fromNodeStream: t => qi(function(t) {
                     return R(this, arguments, (function*() {
                         const e = [];
                         let n, i, r, s = "error",
                             o = !1,
                             a = null,
                             l = 0,
                             c = [];
 
                         function u() {
-                            return "peek" === n ? K(c, i)[0] : ([r, c, l] = K(c, i), r)
+                            return "peek" === n ? q(c, i)[0] : ([r, c, l] = q(c, i), r)
                         }
                         if (({
                                 cmd: n,
                                 size: i
                             } = yield yield B(null)), t.isTTY) return yield yield B(new Uint8Array(0)), yield B(null);
                         try {
                             e[0] = Qi(t, "end"), e[1] = Qi(t, "error");
@@ -11569,16 +11569,16 @@
                 toDOMStream(t, e) {
                     throw new Error('"toDOMStream" not available in this environment')
                 },
                 toNodeStream(t, e) {
                     throw new Error('"toNodeStream" not available in this environment')
                 }
             },
-            Ki = t => (t.next(), t);
-        class qi {
+            qi = t => (t.next(), t);
+        class Xi {
             constructor(t) {
                 this.source = t, this.reader = null, this.reader = this.source.getReader(), this.reader.closed.catch((() => {}))
             }
             get closed() {
                 return this.reader ? this.reader.closed.catch((() => {})) : Promise.resolve()
             }
             releaseLock() {
@@ -11681,18 +11681,18 @@
                     for (; t.length > 0;) t.shift().resolve(Gi);
                     this._closedPromiseResolve(), this._closedPromiseResolve = void 0
                 }
             } [Symbol.asyncIterator]() {
                 return this
             }
             toDOMStream(t) {
-                return Xi.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+                return Ki.toDOMStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             toNodeStream(t) {
-                return Xi.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
+                return Ki.toNodeStream(this._closedPromiseResolve || this._error ? this : this._values, t)
             }
             throw (t) {
                 return z(this, void 0, void 0, (function*() {
                     return yield this.abort(t), Gi
                 }))
             }
             return (t) {
@@ -11733,15 +11733,15 @@
             write(t) {
                 if ((t = G(t)).byteLength > 0) return super.write(t)
             }
             toString() {
                 return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? W(this.toUint8Array(!0)) : this.toUint8Array(!1).then(W)
             }
             toUint8Array() {
-                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? K(this._values)[0] : (() => z(this, void 0, void 0, (function*() {
+                return arguments.length > 0 && void 0 !== arguments[0] && arguments[0] ? q(this._values)[0] : (() => z(this, void 0, void 0, (function*() {
                     var t, e;
                     const n = [];
                     let i = 0;
                     try {
                         for (var r, s = V(this); !(r = yield s.next()).done;) {
                             const t = r.value;
                             n.push(t), i += t.byteLength
@@ -11753,21 +11753,21 @@
                     } finally {
                         try {
                             r && !r.done && (e = s.return) && (yield e.call(s))
                         } finally {
                             if (t) throw t.error
                         }
                     }
-                    return K(n, i)[0]
+                    return q(n, i)[0]
                 })))()
             }
         }
         class nr {
             constructor(t) {
-                t && (this.source = new rr(Xi.fromIterable(t)))
+                t && (this.source = new rr(Ki.fromIterable(t)))
             } [Symbol.iterator]() {
                 return this
             }
             next(t) {
                 return this.source.next(t)
             }
             throw (t) {
@@ -11781,15 +11781,15 @@
             }
             read(t) {
                 return this.source.read(t)
             }
         }
         class ir {
             constructor(t) {
-                t instanceof ir ? this.source = t.source : t instanceof er ? this.source = new sr(Xi.fromAsyncIterable(t)) : P(t) ? this.source = new sr(Xi.fromNodeStream(t)) : A(t) ? this.source = new sr(Xi.fromDOMStream(t)) : O(t) ? this.source = new sr(Xi.fromDOMStream(t.body)) : k(t) ? this.source = new sr(Xi.fromIterable(t)) : (T(t) || M(t)) && (this.source = new sr(Xi.fromAsyncIterable(t)))
+                t instanceof ir ? this.source = t.source : t instanceof er ? this.source = new sr(Ki.fromAsyncIterable(t)) : P(t) ? this.source = new sr(Ki.fromNodeStream(t)) : A(t) ? this.source = new sr(Ki.fromDOMStream(t)) : O(t) ? this.source = new sr(Ki.fromDOMStream(t.body)) : k(t) ? this.source = new sr(Ki.fromIterable(t)) : (T(t) || M(t)) && (this.source = new sr(Ki.fromAsyncIterable(t)))
             } [Symbol.asyncIterator]() {
                 return this
             }
             next(t) {
                 return this.source.next(t)
             }
             throw (t) {
@@ -12500,35 +12500,35 @@
                 } = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.nextBufferRange();
                 return e <= 0 ? new Uint8Array(0) : Mn(this.sources[n])
             }
             readOffsets(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return q(Uint8Array, q(Int32Array, this.sources[e]))
+                return X(Uint8Array, X(Int32Array, this.sources[e]))
             }
             readTypeIds(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
-                return q(Uint8Array, q(t.ArrayType, this.sources[e]))
+                return X(Uint8Array, X(t.ArrayType, this.sources[e]))
             }
             readData(t) {
                 let {
                     offset: e
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.nextBufferRange();
                 const {
                     sources: n
                 } = this;
-                return At.isTimestamp(t) || (At.isInt(t) || At.isTime(t)) && 64 === t.bitWidth || At.isDate(t) && t.unit === s.MILLISECOND ? q(Uint8Array, dr.convertArray(n[e])) : At.isDecimal(t) ? q(Uint8Array, fr.convertArray(n[e])) : At.isBinary(t) || At.isFixedSizeBinary(t) ? function(t) {
+                return At.isTimestamp(t) || (At.isInt(t) || At.isTime(t)) && 64 === t.bitWidth || At.isDate(t) && t.unit === s.MILLISECOND ? X(Uint8Array, dr.convertArray(n[e])) : At.isDecimal(t) ? X(Uint8Array, fr.convertArray(n[e])) : At.isBinary(t) || At.isFixedSizeBinary(t) ? function(t) {
                     const e = t.join(""),
                         n = new Uint8Array(e.length / 2);
                     for (let i = 0; i < e.length; i += 2) n[i >> 1] = Number.parseInt(e.slice(i, i + 2), 16);
                     return n
-                }(n[e]) : At.isBool(t) ? Mn(n[e]) : At.isUtf8(t) ? Y(n[e].join("")) : q(Uint8Array, q(t.ArrayType, n[e].map((t => +t))))
+                }(n[e]) : At.isBool(t) ? Mn(n[e]) : At.isUtf8(t) ? Y(n[e].join("")) : X(Uint8Array, X(t.ArrayType, n[e].map((t => +t))))
             }
         }
         var mr, yr, br, vr, xr, _r, wr, Sr;
         ! function(t) {
             t[t.BUFFER = 0] = "BUFFER"
         }(mr || (mr = {})),
         function(t) {
@@ -13288,15 +13288,15 @@
                 return t.endObject()
             }
             static createStruct_(t) {
                 return Yr.startStruct_(t), Yr.endStruct_(t)
             }
         }
         var $r = Ii;
-        const Xr = new class extends ee {
+        const Kr = new class extends ee {
             visit(t, e) {
                 return null == t || null == e ? void 0 : super.visit(t, e)
             }
             visitNull(t, e) {
                 return Ur.startNull(e), Ur.endNull(e)
             }
             visitInt(t, e) {
@@ -13352,19 +13352,19 @@
                 return Nr.startFixedSizeList(e), Nr.addListSize(e, t.listSize), Nr.endFixedSizeList(e)
             }
             visitMap(t, e) {
                 return Br.startMap(e), Br.addKeysSorted(e, t.keysSorted), Br.endMap(e)
             }
         };
 
-        function Kr(t) {
+        function qr(t) {
             return new ss(t.count, Qr(t.columns), Gr(t.columns))
         }
 
-        function qr(t, e) {
+        function Xr(t, e) {
             return (t.children || []).filter(Boolean).map((t => Zn.fromJSON(t, e)))
         }
 
         function Qr(t) {
             return (t || []).reduce(((t, e) => {
                 return [...t, new ls(e.count, (n = e.VALIDITY, (n || []).reduce(((t, e) => t + +(0 === e)), 0))), ...Qr(e.children)];
                 var n
@@ -13433,23 +13433,23 @@
                 }
                 case "interval": {
                     const e = t.type;
                     return new Ht(a[e.unit])
                 }
                 case "union": {
                     const i = t.type;
-                    return new Xt(n[i.mode], i.typeIds || [], e || [])
+                    return new Kt(n[i.mode], i.typeIds || [], e || [])
                 }
                 case "fixedsizebinary": {
                     const e = t.type;
-                    return new Kt(e.byteWidth)
+                    return new qt(e.byteWidth)
                 }
                 case "fixedsizelist": {
                     const n = t.type;
-                    return new qt(n.listSize, (e || [])[0])
+                    return new Xt(n.listSize, (e || [])[0])
                 }
                 case "map": {
                     const n = t.type;
                     return new Qt((e || [])[0], n.keysSorted)
                 }
             }
             throw new Error('Unrecognized type: "'.concat(i, '"'))
@@ -13645,38 +13645,38 @@
                 }
                 case Ai.Interval: {
                     const e = t.type(new Fr);
                     return new Ht(e.unit())
                 }
                 case Ai.Union: {
                     const n = t.type(new Lr);
-                    return new Xt(n.mode(), n.typeIdsArray() || [], e || [])
+                    return new Kt(n.mode(), n.typeIdsArray() || [], e || [])
                 }
                 case Ai.FixedSizeBinary: {
                     const e = t.type(new zr);
-                    return new Kt(e.byteWidth())
+                    return new qt(e.byteWidth())
                 }
                 case Ai.FixedSizeList: {
                     const n = t.type(new Nr);
-                    return new qt(n.listSize(), (e || [])[0])
+                    return new Xt(n.listSize(), (e || [])[0])
                 }
                 case Ai.Map: {
                     const n = t.type(new Br);
                     return new Qt((e || [])[0], n.keysSorted())
                 }
             }
             throw new Error('Unrecognized type: "'.concat(Ai[n], '" (').concat(n, ")"))
         }
         Zn.encode = function(t, e) {
             let n = -1,
                 i = -1,
                 r = -1;
             const s = e.type;
             let o = e.typeId;
-            At.isDictionary(s) ? (o = s.dictionary.typeId, r = Xr.visit(s, t), i = Xr.visit(s.dictionary, t)) : i = Xr.visit(s, t);
+            At.isDictionary(s) ? (o = s.dictionary.typeId, r = Kr.visit(s, t), i = Kr.visit(s.dictionary, t)) : i = Kr.visit(s, t);
             const a = (s.children || []).map((e => Zn.encode(t, e))),
                 l = Bi.createChildrenVector(t, a),
                 c = e.metadata && e.metadata.size > 0 ? Bi.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
                         s = t.createString("".concat(i));
                     return Li.startKeyValue(t), Li.addKey(t, r), Li.addValue(t, s), Li.endKeyValue(t)
@@ -13686,15 +13686,15 @@
             return Bi.endField(t)
         }, Zn.decode = function(t, e) {
             let n, i, r, s, o, a;
             e && (a = t.dictionary()) ? e.has(n = a.id().low) ? (s = (s = a.indexType()) ? hs(s) : new Lt, o = new Jt(e.get(n), s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (s = (s = a.indexType()) ? hs(s) : new Lt, e.set(n, r = ds(t, cs(t, e))), o = new Jt(r, s, n, a.isOrdered()), i = new Zn(t.name(), o, t.nullable(), us(t))) : (r = ds(t, cs(t, e)), i = new Zn(t.name(), r, t.nullable(), us(t)));
             return i || null
         }, Zn.fromJSON = function(t, e) {
             let n, i, r, s, o, a;
-            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new Lt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new Lt, e.set(n, o = ts(t, qr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, qr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
+            return e && (s = t.dictionary) ? e.has(n = s.id) ? (i = (i = s.indexType) ? Jr(i) : new Lt, a = new Jt(e.get(n), i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (i = (i = s.indexType) ? Jr(i) : new Lt, e.set(n, o = ts(t, Xr(t, e))), a = new Jt(o, i, n, s.isOrdered), r = new Zn(t.name, a, t.nullable, Zr(t.customMetadata))) : (o = ts(t, Xr(t, e)), r = new Zn(t.name, o, t.nullable, Zr(t.customMetadata))), r || null
         }, Gn.encode = function(t, e) {
             const n = e.fields.map((e => Zn.encode(t, e)));
             Ri.startFieldsVector(t, n.length);
             const i = Ri.createFieldsVector(t, n),
                 r = e.metadata && e.metadata.size > 0 ? Ri.createCustomMetadataVector(t, [...e.metadata].map((e => {
                     let [n, i] = e;
                     const r = t.createString("".concat(n)),
@@ -13734,22 +13734,22 @@
                 for (let n, i = -1, r = -1, s = t.nodesLength(); ++i < s;)(n = t.nodes(i)) && (e[++r] = ls.decode(n));
                 return e
             }(t), function(t, n) {
                 const i = [];
                 for (let r, s = -1, o = -1, a = t.buffersLength(); ++s < a;)(r = t.buffers(s)) && (n < e.V4 && (r.bb_pos += 8 * (s + 1)), i[++o] = as.decode(r));
                 return i
             }(t, n))
-        }, ss.fromJSON = Kr, os.encode = function(t, e) {
+        }, ss.fromJSON = qr, os.encode = function(t, e) {
             const n = ss.encode(t, e.data);
             return Er.startDictionaryBatch(t), Er.addId(t, new es(e.id, 0)), Er.addIsDelta(t, e.isDelta), Er.addData(t, n), Er.endDictionaryBatch(t)
         }, os.decode = function(t) {
             let n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : e.V4;
             return new os(ss.decode(t.data(), n), t.id(), t.isDelta())
         }, os.fromJSON = function(t) {
-            return new os(Kr(t.data), t.id, t.isDelta)
+            return new os(qr(t.data), t.id, t.isDelta)
         }, ls.encode = function(t, e) {
             return Mr.createFieldNode(t, new es(e.length, 0), new es(e.nullCount, 0))
         }, ls.decode = function(t) {
             return new ls(t.length(), t.nullCount())
         }, as.encode = function(t, e) {
             return kr.createBuffer(t, new es(e.offset, 0), new es(e.length, 0))
         }, as.decode = function(t) {
@@ -14012,22 +14012,22 @@
                 return this._impl.isFile() ? this._impl.readRecordBatch(t) : null
             } [Symbol.iterator]() {
                 return this._impl[Symbol.iterator]()
             } [Symbol.asyncIterator]() {
                 return this._impl[Symbol.asyncIterator]()
             }
             toDOMStream() {
-                return Xi.toDOMStream(this.isSync() ? {
+                return Ki.toDOMStream(this.isSync() ? {
                     [Symbol.iterator]: () => this
                 } : {
                     [Symbol.asyncIterator]: () => this
                 })
             }
             toNodeStream() {
-                return Xi.toNodeStream(this.isSync() ? {
+                return Ki.toNodeStream(this.isSync() ? {
                     [Symbol.iterator]: () => this
                 } : {
                     [Symbol.asyncIterator]: () => this
                 }, {
                     objectMode: !0
                 })
             }
@@ -14568,30 +14568,30 @@
             const {
                 length: e,
                 valueOffsets: n
             } = t;
             return n && Ws.call(this, et(n[0], e, n)), this.visit(t.children[0])
         }
 
-        function Xs(t) {
+        function Ks(t) {
             return this.visitMany(t.type.children.map(((e, n) => t.children[n])).filter(Boolean))[0]
         }
         js.prototype.visitBool = function(t) {
             let e;
             return t.nullCount >= t.length ? Ws.call(this, new Uint8Array(0)) : (e = t.values) instanceof Uint8Array ? Ws.call(this, kn(t.offset, t.length, e)) : Ws.call(this, Mn(t.values))
-        }, js.prototype.visitInt = Hs, js.prototype.visitFloat = Hs, js.prototype.visitUtf8 = Ys, js.prototype.visitBinary = Ys, js.prototype.visitFixedSizeBinary = Hs, js.prototype.visitDate = Hs, js.prototype.visitTimestamp = Hs, js.prototype.visitTime = Hs, js.prototype.visitDecimal = Hs, js.prototype.visitList = $s, js.prototype.visitStruct = Xs, js.prototype.visitUnion = function(t) {
+        }, js.prototype.visitInt = Hs, js.prototype.visitFloat = Hs, js.prototype.visitUtf8 = Ys, js.prototype.visitBinary = Ys, js.prototype.visitFixedSizeBinary = Hs, js.prototype.visitDate = Hs, js.prototype.visitTimestamp = Hs, js.prototype.visitTime = Hs, js.prototype.visitDecimal = Hs, js.prototype.visitList = $s, js.prototype.visitStruct = Ks, js.prototype.visitUnion = function(t) {
             const {
                 type: e,
                 length: i,
                 typeIds: r,
                 valueOffsets: s
             } = t;
-            if (Ws.call(this, r), e.mode === n.Sparse) return Xs.call(this, t);
+            if (Ws.call(this, r), e.mode === n.Sparse) return Ks.call(this, t);
             if (e.mode === n.Dense) {
-                if (t.offset <= 0) return Ws.call(this, s), Xs.call(this, t);
+                if (t.offset <= 0) return Ws.call(this, s), Ks.call(this, t);
                 {
                     const n = r.reduce(((t, e) => Math.max(t, e)), r[0]),
                         o = new Int32Array(n + 1),
                         a = new Int32Array(n + 1).fill(-1),
                         l = new Int32Array(i),
                         c = et(-s[0], i, s);
                     for (let t, e, s = -1; ++s < i;) - 1 === (e = a[t = r[s]]) && (e = a[t] = c[t]), l[s] = c[s] - e, ++o[t];
@@ -14602,15 +14602,15 @@
                                 n = Math.min(i, o[t]);
                             this.visit(r.slice(a[t], n))
                         }
                 }
             }
             return this
         }, js.prototype.visitInterval = Hs, js.prototype.visitFixedSizeList = $s, js.prototype.visitMap = $s;
-        class Ks extends Ji {
+        class qs extends Ji {
             constructor(t) {
                 super(), this._position = 0, this._started = !1, this._sink = new er, this._schema = null, this._dictionaryBlocks = [], this._recordBatchBlocks = [], this._dictionaryDeltaOffsets = new Map, S(t) || (t = {
                     autoDestroy: !0,
                     writeLegacyIpcFormat: !1
                 }), this._autoDestroy = "boolean" !== typeof t.autoDestroy || t.autoDestroy, this._writeLegacyIpcFormat = "boolean" === typeof t.writeLegacyIpcFormat && t.writeLegacyIpcFormat
             }
             static throughNode(t) {
@@ -14730,21 +14730,21 @@
                     let t = this._dictionaryDeltaOffsets.get(e) || 0;
                     if (0 === t || (n = null === n || void 0 === n ? void 0 : n.slice(t)).length > 0)
                         for (const i of n.data) this._writeDictionaryBatch(i, e, t > 0), t += i.length
                 }
                 return this
             }
         }
-        class qs extends Ks {
+        class Xs extends qs {
             static writeAll(t, e) {
-                const n = new qs(e);
+                const n = new Xs(e);
                 return T(t) ? t.then((t => n.writeAll(t))) : M(t) ? Zs(n, t) : Gs(n, t)
             }
         }
-        class Qs extends Ks {
+        class Qs extends qs {
             static writeAll(t) {
                 const e = new Qs;
                 return T(t) ? t.then((t => e.writeAll(t))) : M(t) ? Zs(e, t) : Gs(e, t)
             }
             constructor() {
                 super(), this._autoDestroy = !0
             }
@@ -14789,15 +14789,15 @@
 
         function Js(t) {
             const e = Es.from(t);
             return T(e) ? e.then((t => Js(t))) : e.isAsync() ? e.readAll().then((t => new _i(t))) : new _i(e.readAll())
         }
 
         function to(t) {
-            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? qs : Qs).writeAll(t).toUint8Array(!0)
+            return ("stream" === (arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "stream") ? Xs : Qs).writeAll(t).toUint8Array(!0)
         }
         var eo, no = function() {
                 function t(t, e, n, i) {
                     var r = this;
                     this.getCell = function(t, e) {
                         var n = t < r.headerRows && e < r.headerColumns,
                             i = t >= r.headerRows && e < r.headerColumns,
@@ -15552,24 +15552,24 @@
                     var n = Do(t);
                     n[0] = Ao(n[0] + e), n = Co(n), t.r = n[0], t.g = n[1], t.b = n[2]
                 }(this._rgb, t), this
             }
         }
 
         function $o() {}
-        const Xo = (() => {
+        const Ko = (() => {
             let t = 0;
             return () => t++
         })();
 
-        function Ko(t) {
+        function qo(t) {
             return null === t || "undefined" === typeof t
         }
 
-        function qo(t) {
+        function Xo(t) {
             if (Array.isArray && Array.isArray(t)) return !0;
             const e = Object.prototype.toString.call(t);
             return "[object" === e.slice(0, 7) && "Array]" === e.slice(-6)
         }
 
         function Qo(t) {
             return null !== t && "[object Object]" === Object.prototype.toString.call(t)
@@ -15590,15 +15590,15 @@
 
         function ea(t, e, n) {
             if (t && "function" === typeof t.call) return t.apply(n, e)
         }
 
         function na(t, e, n, i) {
             let r, s, o;
-            if (qo(t))
+            if (Xo(t))
                 if (s = t.length, i)
                     for (r = s - 1; r >= 0; r--) e.call(n, t[r], r);
                 else
                     for (r = 0; r < s; r++) e.call(n, t[r], r);
             else if (Qo(t))
                 for (o = Object.keys(t), s = o.length, r = 0; r < s; r++) e.call(n, t[o[r]], o[r])
         }
@@ -15608,15 +15608,15 @@
             if (!t || !e || t.length !== e.length) return !1;
             for (n = 0, i = t.length; n < i; ++n)
                 if (r = t[n], s = e[n], r.datasetIndex !== s.datasetIndex || r.index !== s.index) return !1;
             return !0
         }
 
         function ra(t) {
-            if (qo(t)) return t.map(ra);
+            if (Xo(t)) return t.map(ra);
             if (Qo(t)) {
                 const e = Object.create(null),
                     n = Object.keys(t),
                     i = n.length;
                 let r = 0;
                 for (; r < i; ++r) e[n[r]] = ra(t[n[r]]);
                 return e
@@ -15632,15 +15632,15 @@
             if (!sa(t)) return;
             const r = e[t],
                 s = n[t];
             Qo(r) && Qo(s) ? aa(r, s, i) : e[t] = ra(s)
         }
 
         function aa(t, e, n) {
-            const i = qo(e) ? e : [e],
+            const i = Xo(e) ? e : [e],
                 r = i.length;
             if (!Qo(t)) return t;
             const s = (n = n || {}).merger || oa;
             let o;
             for (let a = 0; a < r; ++a) {
                 if (o = i[a], !Qo(o)) continue;
                 const e = Object.keys(o);
@@ -15819,26 +15819,26 @@
             const e = new Set(t);
             return e.size === t.length ? t : Array.from(e)
         }
         const $a = "undefined" === typeof window ? function(t) {
             return t()
         } : window.requestAnimationFrame;
 
-        function Xa(t, e) {
+        function Ka(t, e) {
             let n = [],
                 i = !1;
             return function() {
                 for (var r = arguments.length, s = new Array(r), o = 0; o < r; o++) s[o] = arguments[o];
                 n = s, i || (i = !0, $a.call(window, (() => {
                     i = !1, t.apply(e, n)
                 })))
             }
         }
-        const Ka = t => "start" === t ? "left" : "end" === t ? "right" : "center",
-            qa = (t, e, n) => "start" === t ? e : "end" === t ? n : (e + n) / 2;
+        const qa = t => "start" === t ? "left" : "end" === t ? "right" : "center",
+            Xa = (t, e, n) => "start" === t ? e : "end" === t ? n : (e + n) / 2;
 
         function Qa(t, e, n) {
             const i = e.length;
             let r = 0,
                 s = i;
             if (t._sorted) {
                 const {
@@ -15950,15 +15950,15 @@
                 e = e || {};
                 const n = t + JSON.stringify(e);
                 let i = al.get(n);
                 return i || (i = new Intl.NumberFormat(t, e), al.set(n, i)), i
             }(e, n).format(t)
         }
         const cl = {
-            values: t => qo(t) ? t : "" + t,
+            values: t => Xo(t) ? t : "" + t,
             numeric(t, e, n) {
                 if (0 === t) return "0";
                 const i = this.chart.options.locale;
                 let r, s = t;
                 if (n.length > 1) {
                     const e = Math.max(Math.abs(n[0].value), Math.abs(n[n.length - 1].value));
                     (e < 1e-4 || e > 1e15) && (r = "scientific"), s = function(t, e) {
@@ -16207,17 +16207,17 @@
             let r = (i = i || {}).data = i.data || {},
                 s = i.garbageCollect = i.garbageCollect || [];
             i.font !== e && (r = i.data = {}, s = i.garbageCollect = [], i.font = e), t.save(), t.font = e;
             let o = 0;
             const a = n.length;
             let l, c, u, h, d;
             for (l = 0; l < a; l++)
-                if (h = n[l], void 0 === h || null === h || qo(h)) {
-                    if (qo(h))
-                        for (c = 0, u = h.length; c < u; c++) d = h[c], void 0 === d || null === d || qo(d) || (o = yl(t, r, s, o, d))
+                if (h = n[l], void 0 === h || null === h || Xo(h)) {
+                    if (Xo(h))
+                        for (c = 0, u = h.length; c < u; c++) d = h[c], void 0 === d || null === d || Xo(d) || (o = yl(t, r, s, o, d))
                 } else o = yl(t, r, s, o, h);
             t.restore();
             const f = s.length / 2;
             if (f > n.length) {
                 for (l = 0; l < f; l++) delete r[s[l]];
                 s.splice(0, f)
             }
@@ -16327,20 +16327,20 @@
         function Dl(t, e) {
             const n = t.fillStyle;
             t.fillStyle = e.color, t.fillRect(e.left, e.top, e.width, e.height), t.fillStyle = n
         }
 
         function Ol(t, e, n, i, r) {
             let s = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : {};
-            const o = qo(e) ? e : [e],
+            const o = Xo(e) ? e : [e],
                 a = s.strokeWidth > 0 && "" !== s.strokeColor;
             let l, c;
             for (t.save(), t.font = r.string, function(t, e) {
-                    e.translation && t.translate(e.translation[0], e.translation[1]), Ko(e.rotation) || t.rotate(e.rotation), e.color && (t.fillStyle = e.color), e.textAlign && (t.textAlign = e.textAlign), e.textBaseline && (t.textBaseline = e.textBaseline)
-                }(t, s), l = 0; l < o.length; ++l) c = o[l], s.backdrop && Dl(t, s.backdrop), a && (s.strokeColor && (t.strokeStyle = s.strokeColor), Ko(s.strokeWidth) || (t.lineWidth = s.strokeWidth), t.strokeText(c, n, i, s.maxWidth)), t.fillText(c, n, i, s.maxWidth), El(t, n, i, c, s), i += Number(r.lineHeight);
+                    e.translation && t.translate(e.translation[0], e.translation[1]), qo(e.rotation) || t.rotate(e.rotation), e.color && (t.fillStyle = e.color), e.textAlign && (t.textAlign = e.textAlign), e.textBaseline && (t.textBaseline = e.textBaseline)
+                }(t, s), l = 0; l < o.length; ++l) c = o[l], s.backdrop && Dl(t, s.backdrop), a && (s.strokeColor && (t.strokeStyle = s.strokeColor), qo(s.strokeWidth) || (t.lineWidth = s.strokeWidth), t.strokeText(c, n, i, s.maxWidth)), t.fillText(c, n, i, s.maxWidth), El(t, n, i, c, s), i += Number(r.lineHeight);
             t.restore()
         }
 
         function Cl(t, e) {
             const {
                 x: n,
                 y: i,
@@ -16404,22 +16404,22 @@
                 lineHeight: Fl(Jo(t.lineHeight, e.lineHeight), n),
                 size: n,
                 style: i,
                 weight: Jo(t.weight, e.weight),
                 string: ""
             };
             return r.string = function(t) {
-                return !t || Ko(t.size) || Ko(t.family) ? null : (t.style ? t.style + " " : "") + (t.weight ? t.weight + " " : "") + t.size + "px " + t.family
+                return !t || qo(t.size) || qo(t.family) ? null : (t.style ? t.style + " " : "") + (t.weight ? t.weight + " " : "") + t.size + "px " + t.family
             }(r), r
         }
 
         function Vl(t, e, n, i) {
             let r, s, o, a = !0;
             for (r = 0, s = t.length; r < s; ++r)
-                if (o = t[r], void 0 !== o && (void 0 !== e && "function" === typeof o && (o = o(e), a = !1), void 0 !== n && qo(o) && (o = o[n % o.length], a = !1), void 0 !== o)) return i && !a && (i.cacheable = !1), o
+                if (o = t[r], void 0 !== o && (void 0 !== e && "function" === typeof o && (o = o(e), a = !1), void 0 !== n && Xo(o) && (o = o[n % o.length], a = !1), void 0 !== o)) return i && !a && (i.cacheable = !1), o
         }
 
         function jl(t, e) {
             return Object.assign(Object.create(t), e)
         }
 
         function Wl(t) {
@@ -16435,18 +16435,18 @@
                 _rootScopes: r,
                 _fallback: n,
                 _getTarget: i,
                 override: i => Wl([i, ...t], e, r, n)
             };
             return new Proxy(s, {
                 deleteProperty: (e, n) => (delete e[n], delete e._keys, delete t[0][n], !0),
-                get: (n, i) => Kl(n, i, (() => function(t, e, n, i) {
+                get: (n, i) => ql(n, i, (() => function(t, e, n, i) {
                     let r;
                     for (const s of e)
-                        if (r = tc($l(s, t), n), "undefined" !== typeof r) return Xl(t, r) ? Zl(n, i, t, r) : r
+                        if (r = tc($l(s, t), n), "undefined" !== typeof r) return Kl(t, r) ? Zl(n, i, t, r) : r
                 }(i, e, t, n))),
                 getOwnPropertyDescriptor: (t, e) => Reflect.getOwnPropertyDescriptor(t._scopes[0], e),
                 getPrototypeOf: () => Reflect.getPrototypeOf(t[0]),
                 has: (t, e) => ec(t).includes(e),
                 ownKeys: t => ec(t),
                 set(t, e, n) {
                     const r = t._storage || (t._storage = i());
@@ -16464,15 +16464,15 @@
                 _stack: new Set,
                 _descriptors: Yl(t, i),
                 setContext: e => Hl(t, e, n, i),
                 override: r => Hl(t.override(r), e, n, i)
             };
             return new Proxy(r, {
                 deleteProperty: (e, n) => (delete e[n], delete t[n], !0),
-                get: (t, e, n) => Kl(t, e, (() => function(t, e, n) {
+                get: (t, e, n) => ql(t, e, (() => function(t, e, n) {
                     const {
                         _proxy: i,
                         _context: r,
                         _subProxy: s,
                         _descriptors: o
                     } = t;
                     let a = i[e];
@@ -16482,18 +16482,18 @@
                             _context: s,
                             _subProxy: o,
                             _stack: a
                         } = n;
                         if (a.has(t)) throw new Error("Recursion detected: " + Array.from(a).join("->") + "->" + t);
                         a.add(t);
                         let l = e(s, o || i);
-                        a.delete(t), Xl(t, l) && (l = Zl(r._scopes, r, t, l));
+                        a.delete(t), Kl(t, l) && (l = Zl(r._scopes, r, t, l));
                         return l
                     }(e, a, t, n));
-                    qo(a) && a.length && (a = function(t, e, n, i) {
+                    Xo(a) && a.length && (a = function(t, e, n, i) {
                         const {
                             _proxy: r,
                             _context: s,
                             _subProxy: o,
                             _descriptors: a
                         } = n;
                         if ("undefined" !== typeof s.index && i(t)) return e[s.index % e.length];
@@ -16504,15 +16504,15 @@
                             for (const l of n) {
                                 const n = Zl(i, r, t, l);
                                 e.push(Hl(n, s, o && o[t], a))
                             }
                         }
                         return e
                     }(e, a, t, o.isIndexable));
-                    Xl(e, a) && (a = Hl(a, r, s && s[e], o));
+                    Kl(e, a) && (a = Hl(a, r, s && s[e], o));
                     return a
                 }(t, e, n))),
                 getOwnPropertyDescriptor: (e, n) => e._descriptors.allKeys ? Reflect.has(t, n) ? {
                     enumerable: !0,
                     configurable: !0
                 } : void 0 : Reflect.getOwnPropertyDescriptor(t, n),
                 getPrototypeOf: () => Reflect.getPrototypeOf(t),
@@ -16537,51 +16537,51 @@
                 scriptable: n,
                 indexable: i,
                 isScriptable: pa(n) ? n : () => n,
                 isIndexable: pa(i) ? i : () => i
             }
         }
         const $l = (t, e) => t ? t + da(e) : e,
-            Xl = (t, e) => Qo(e) && "adapters" !== t && (null === Object.getPrototypeOf(e) || e.constructor === Object);
+            Kl = (t, e) => Qo(e) && "adapters" !== t && (null === Object.getPrototypeOf(e) || e.constructor === Object);
 
-        function Kl(t, e, n) {
+        function ql(t, e, n) {
             if (Object.prototype.hasOwnProperty.call(t, e)) return t[e];
             const i = n();
             return t[e] = i, i
         }
 
-        function ql(t, e, n) {
+        function Xl(t, e, n) {
             return pa(t) ? t(e, n) : t
         }
         const Ql = (t, e) => !0 === t ? e : "string" === typeof t ? ha(e, t) : void 0;
 
         function Gl(t, e, n, i, r) {
             for (const s of e) {
                 const e = Ql(n, s);
                 if (e) {
                     t.add(e);
-                    const s = ql(e._fallback, n, r);
+                    const s = Xl(e._fallback, n, r);
                     if ("undefined" !== typeof s && s !== n && s !== i) return s
                 } else if (!1 === e && "undefined" !== typeof i && n !== i) return null
             }
             return !1
         }
 
         function Zl(t, e, n, i) {
             const r = e._rootScopes,
-                s = ql(e._fallback, n, i),
+                s = Xl(e._fallback, n, i),
                 o = [...t, ...r],
                 a = new Set;
             a.add(i);
             let l = Jl(a, o, n, s || n, i);
             return null !== l && (("undefined" === typeof s || s === n || (l = Jl(a, o, s, l, i), null !== l)) && Wl(Array.from(a), [""], r, s, (() => function(t, e, n) {
                 const i = t._getTarget();
                 e in i || (i[e] = {});
                 const r = i[e];
-                if (qo(r) && Qo(n)) return n;
+                if (Xo(r) && Qo(n)) return n;
                 return r || {}
             }(e, n, i))))
         }
 
         function Jl(t, e, n, i, r) {
             for (; n;) n = Gl(t, e, n, i, r);
             return n
@@ -17199,15 +17199,15 @@
                 const e = Object.keys(ml.animation),
                     n = this._properties;
                 Object.getOwnPropertyNames(t).forEach((i => {
                     const r = t[i];
                     if (!Qo(r)) return;
                     const s = {};
                     for (const t of e) s[t] = r[t];
-                    (qo(r.properties) && r.properties || [i]).forEach((t => {
+                    (Xo(r.properties) && r.properties || [i]).forEach((t => {
                         t !== i && n.has(t) || n.set(t, s)
                     }))
                 }))
             }
             _animateOptions(t, e) {
                 const n = e.options,
                     i = function(t, e) {
@@ -17311,23 +17311,23 @@
         }
 
         function $c(t, e, n) {
             const i = t[e] || (t[e] = {});
             return i[n] || (i[n] = {})
         }
 
-        function Xc(t, e, n, i) {
+        function Kc(t, e, n, i) {
             for (const r of e.getMatchingVisibleMetas(i).reverse()) {
                 const e = t[r.index];
                 if (n && e > 0 || !n && e < 0) return r.index
             }
             return null
         }
 
-        function Kc(t, e) {
+        function qc(t, e) {
             const {
                 chart: n,
                 _cachedMeta: i
             } = t, r = n._stacks || (n._stacks = {}), {
                 iScale: s,
                 vScale: o,
                 index: a
@@ -17337,20 +17337,20 @@
             let d;
             for (let f = 0; f < h; ++f) {
                 const t = e[f],
                     {
                         [l]: n,
                         [c]: s
                     } = t;
-                d = (t._stacks || (t._stacks = {}))[c] = $c(r, u, n), d[a] = s, d._top = Xc(d, o, !0, i.type), d._bottom = Xc(d, o, !1, i.type);
+                d = (t._stacks || (t._stacks = {}))[c] = $c(r, u, n), d[a] = s, d._top = Kc(d, o, !0, i.type), d._bottom = Kc(d, o, !1, i.type);
                 (d._visualValues || (d._visualValues = {}))[a] = s
             }
         }
 
-        function qc(t, e) {
+        function Xc(t, e) {
             const n = t.scales;
             return Object.keys(n).filter((t => n[t].axis === e)).shift()
         }
 
         function Qc(t, e) {
             const n = t.controller.index,
                 i = t.vScale && t.vScale.axis;
@@ -17377,17 +17377,17 @@
                 this.index !== t && Qc(this._cachedMeta), this.index = t
             }
             linkScales() {
                 const t = this.chart,
                     e = this._cachedMeta,
                     n = this.getDataset(),
                     i = (t, e, n, i) => "x" === t ? e : "r" === t ? i : n,
-                    r = e.xAxisID = Jo(n.xAxisID, qc(t, "x")),
-                    s = e.yAxisID = Jo(n.yAxisID, qc(t, "y")),
-                    o = e.rAxisID = Jo(n.rAxisID, qc(t, "r")),
+                    r = e.xAxisID = Jo(n.xAxisID, Xc(t, "x")),
+                    s = e.yAxisID = Jo(n.yAxisID, Xc(t, "y")),
+                    o = e.rAxisID = Jo(n.rAxisID, Xc(t, "r")),
                     a = e.indexAxis,
                     l = e.iAxisID = i(a, r, s, o),
                     c = e.vAxisID = i(a, s, r, o);
                 e.xScale = this.getScaleForId(r), e.yScale = this.getScaleForId(s), e.rScale = this.getScaleForId(o), e.iScale = this.getScaleForId(l), e.vScale = this.getScaleForId(c)
             }
             getDataset() {
                 return this.chart.data.datasets[this.index]
@@ -17459,15 +17459,15 @@
             }
             buildOrUpdateElements(t) {
                 const e = this._cachedMeta,
                     n = this.getDataset();
                 let i = !1;
                 this._dataCheck();
                 const r = e._stacked;
-                e._stacked = Yc(e.vScale, e), e.stack !== n.stack && (i = !0, Qc(e), e.stack = n.stack), this._resyncElements(t), (i || r !== e._stacked) && Kc(this, e._parsed)
+                e._stacked = Yc(e.vScale, e), e.stack !== n.stack && (i = !0, Qc(e), e.stack = n.stack), this._resyncElements(t), (i || r !== e._stacked) && qc(this, e._parsed)
             }
             configure() {
                 const t = this.chart.config,
                     e = t.datasetScopeKeys(this._type),
                     n = t.getOptionScopes(this.getDataset(), e, !0);
                 this.options = t.createResolver(n, this.getContext()), this._parsing = this.options.parsing, this._cachedDataOpts = {}
             }
@@ -17479,20 +17479,20 @@
                     iScale: r,
                     _stacked: s
                 } = n, o = r.axis;
                 let a, l, c, u = 0 === t && e === i.length || n._sorted,
                     h = t > 0 && n._parsed[t - 1];
                 if (!1 === this._parsing) n._parsed = i, n._sorted = !0, c = i;
                 else {
-                    c = qo(i[t]) ? this.parseArrayData(n, i, t, e) : Qo(i[t]) ? this.parseObjectData(n, i, t, e) : this.parsePrimitiveData(n, i, t, e);
+                    c = Xo(i[t]) ? this.parseArrayData(n, i, t, e) : Qo(i[t]) ? this.parseObjectData(n, i, t, e) : this.parsePrimitiveData(n, i, t, e);
                     const r = () => null === l[o] || h && l[o] < h[o];
                     for (a = 0; a < e; ++a) n._parsed[a + t] = l = c[a], u && (r() && (u = !1), h = l);
                     n._sorted = u
                 }
-                s && Kc(this, c)
+                s && qc(this, c)
             }
             parsePrimitiveData(t, e, n, i) {
                 const {
                     iScale: r,
                     vScale: s
                 } = t, o = r.axis, a = s.axis, l = r.getLabels(), c = r === s, u = new Array(i);
                 let h, d, f;
@@ -17848,15 +17848,15 @@
             };
             for (i = 0, r = n.length; i < r; ++i) s = e.getPixelForValue(n[i]), l();
             for (o = void 0, i = 0, r = e.ticks.length; i < r; ++i) s = e.getPixelForTick(i), l();
             return a
         }
 
         function eu(t, e, n, i) {
-            return qo(t) ? function(t, e, n, i) {
+            return Xo(t) ? function(t, e, n, i) {
                 const r = n.parse(t[0], i),
                     s = n.parse(t[1], i),
                     o = Math.min(r, s),
                     a = Math.max(r, s);
                 let l = o,
                     c = a;
                 Math.abs(o) > Math.abs(a) && (l = a, c = o), e[n.axis] = c, e._custom = {
@@ -17992,15 +17992,15 @@
                     c = this._getRuler(),
                     {
                         sharedOptions: u,
                         includeOptions: h
                     } = this._getSharedOptions(e, i);
                 for (let d = e; d < e + n; d++) {
                     const e = this.getParsed(d),
-                        n = r || Ko(e[o.axis]) ? {
+                        n = r || qo(e[o.axis]) ? {
                             base: a,
                             head: a
                         } : this._calculateBarValuePixels(d),
                         f = this._calculateBarIndexPixels(d, c),
                         p = (e._stacks || {})[o.axis],
                         g = {
                             horizontal: l,
@@ -18018,15 +18018,15 @@
             }
             _getStacks(t, e) {
                 const {
                     iScale: n
                 } = this._cachedMeta, i = n.getMatchingVisibleMetas(this._type).filter((t => t.controller.options.grouped)), r = n.options.stacked, s = [], o = t => {
                     const n = t.controller.getParsed(e),
                         i = n && n[t.vScale.axis];
-                    if (Ko(i) || isNaN(i)) return !0
+                    if (qo(i) || isNaN(i)) return !0
                 };
                 for (const a of i)
                     if ((void 0 === e || !o(a)) && ((!1 === r || -1 === s.indexOf(a.stack) || void 0 === r && void 0 === a.stack) && s.push(a.stack), a.index === t)) break;
                 return s.length || s.push(void 0), s
             }
             _getStackCount(t) {
                 return this._getStacks(void 0, t).length
@@ -18067,15 +18067,15 @@
                         minBarLength: s
                     }
                 } = this, o = r || 0, a = this.getParsed(t), l = a._custom, c = iu(l);
                 let u, h, d = a[e.axis],
                     f = 0,
                     p = n ? this.applyStack(e, a, n) : d;
                 p !== d && (f = p - d, p = d), c && (d = l.barStart, p = l.barEnd - l.barStart, 0 !== d && ka(d) !== ka(l.barEnd) && (f = 0), f += d);
-                const g = Ko(r) || c ? f : r;
+                const g = qo(r) || c ? f : r;
                 let m = e.getPixelForValue(g);
                 if (u = this.chart.getDataVisibility(t) ? e.getPixelForValue(f + p) : m, h = u - m, Math.abs(h) < s) {
                     h = function(t, e, n) {
                         return 0 !== t ? ka(t) : (e.isHorizontal() ? 1 : -1) * (e.min >= n ? 1 : -1)
                     }(h, e, o) * s, d === o && (m -= h / 2);
                     const t = e.getPixelForDecimal(0),
                         r = e.getPixelForDecimal(1),
@@ -18114,15 +18114,15 @@
                                 chunk: Math.abs(a - o) / 2 * l / i,
                                 ratio: n.barPercentage,
                                 start: c
                             }
                         }(t, e, i, n) : function(t, e, n, i) {
                             const r = n.barThickness;
                             let s, o;
-                            return Ko(r) ? (s = e.min * n.categoryPercentage, o = n.barPercentage) : (s = r * i, o = 1), {
+                            return qo(r) ? (s = e.min * n.categoryPercentage, o = n.barPercentage) : (s = r * i, o = 1), {
                                 chunk: s / i,
                                 ratio: o,
                                 start: e.pixels[t] - s / 2
                             }
                         }(t, e, i, n),
                         c = this._getStackIndex(this.index, this._cachedMeta.stack, r ? t : void 0);
                     o = l.start + l.chunk * c + l.chunk / 2, a = Math.min(s, l.chunk * l.ratio)
@@ -18569,15 +18569,15 @@
                     const n = t[x],
                         f = m ? n : {};
                     if (x < e || x >= y) {
                         f.skip = !0;
                         continue
                     }
                     const b = this.getParsed(x),
-                        _ = Ko(b[d]),
+                        _ = qo(b[d]),
                         w = f[h] = s.getPixelForValue(b[h], x),
                         S = f[d] = r || _ ? o.getBasePixel() : o.getPixelForValue(a ? this.applyStack(o, b, a) : b[d], x);
                     f.skip = isNaN(w) || isNaN(S) || _, f.stop = x > 0 && Math.abs(b[h] - v[h]) > g, p && (f.parsed = b, f.raw = l.data[x]), u && (f.options = c || this.resolveDataElementOptions(x, n.active ? "active" : i)), m || this.updateElement(n, x, f, i), v = b
                 }
             }
             getMaxOverflow() {
                 const t = this._cachedMeta,
@@ -18898,15 +18898,15 @@
                     m = Ea(p) ? p : Number.POSITIVE_INFINITY,
                     y = this.chart._animationsDisabled || r || "none" === i;
                 let b = e > 0 && this.getParsed(e - 1);
                 for (let v = e; v < e + n; ++v) {
                     const e = t[v],
                         n = this.getParsed(v),
                         c = y ? e : {},
-                        p = Ko(n[f]),
+                        p = qo(n[f]),
                         x = c[d] = s.getPixelForValue(n[d], v),
                         _ = c[f] = r || p ? o.getBasePixel() : o.getPixelForValue(a ? this.applyStack(o, n, a) : n[f], v);
                     c.skip = isNaN(x) || isNaN(_) || p, c.stop = v > 0 && Math.abs(n[d] - b[d]) > m, g && (c.parsed = n, c.raw = l.data[v]), h && (c.options = u || this.resolveDataElementOptions(v, e.active ? "active" : i)), y || this.updateElement(e, v, c, i), b = n
                 }
                 this.updateSharedOptions(u, i, c)
             }
             getMaxOverflow() {
@@ -19465,37 +19465,37 @@
             passive: !0
         };
 
         function $u(t, e, n) {
             t && t.canvas && t.canvas.removeEventListener(e, n, Yu)
         }
 
-        function Xu(t, e) {
+        function Ku(t, e) {
             for (const n of t)
                 if (n === e || n.contains(e)) return !0
         }
 
-        function Ku(t, e, n) {
+        function qu(t, e, n) {
             const i = t.canvas,
                 r = new MutationObserver((t => {
                     let e = !1;
-                    for (const n of t) e = e || Xu(n.addedNodes, i), e = e && !Xu(n.removedNodes, i);
+                    for (const n of t) e = e || Ku(n.addedNodes, i), e = e && !Ku(n.removedNodes, i);
                     e && n()
                 }));
             return r.observe(document, {
                 childList: !0,
                 subtree: !0
             }), r
         }
 
-        function qu(t, e, n) {
+        function Xu(t, e, n) {
             const i = t.canvas,
                 r = new MutationObserver((t => {
                     let e = !1;
-                    for (const n of t) e = e || Xu(n.removedNodes, i), e = e && !Xu(n.addedNodes, i);
+                    for (const n of t) e = e || Ku(n.removedNodes, i), e = e && !Ku(n.addedNodes, i);
                     e && n()
                 }));
             return r.observe(document, {
                 childList: !0,
                 subtree: !0
             }), r
         }
@@ -19509,15 +19509,15 @@
             })))
         }
 
         function Ju(t, e, n) {
             const i = t.canvas,
                 r = i && hc(i);
             if (!r) return;
-            const s = Xa(((t, e) => {
+            const s = Ka(((t, e) => {
                     const i = r.clientWidth;
                     n(t, e), i < r.clientWidth && n()
                 }), window),
                 o = new ResizeObserver((t => {
                     const e = t[0],
                         n = e.contentRect.width,
                         i = e.contentRect.height;
@@ -19533,15 +19533,15 @@
             n && n.disconnect(), "resize" === e && function(t) {
                 Qu.delete(t), Qu.size || window.removeEventListener("resize", Zu)
             }(t)
         }
 
         function eh(t, e, n) {
             const i = t.canvas,
-                r = Xa((e => {
+                r = Ka((e => {
                     null !== t.ctx && n(function(t, e) {
                         const n = Wu[t.type] || t.type,
                             {
                                 x: i,
                                 y: r
                             } = yc(t, e);
                         return {
@@ -19588,27 +19588,27 @@
             }
             releaseContext(t) {
                 const e = t.canvas;
                 if (!e[ju]) return !1;
                 const n = e[ju].initial;
                 ["height", "width"].forEach((t => {
                     const i = n[t];
-                    Ko(i) ? e.removeAttribute(t) : e.setAttribute(t, i)
+                    qo(i) ? e.removeAttribute(t) : e.setAttribute(t, i)
                 }));
                 const i = n.style || {};
                 return Object.keys(i).forEach((t => {
                     e.style[t] = i[t]
                 })), e.width = e.width, delete e[ju], !0
             }
             addEventListener(t, e, n) {
                 this.removeEventListener(t, e);
                 const i = t.$proxies || (t.$proxies = {}),
                     r = {
-                        attach: Ku,
-                        detach: qu,
+                        attach: qu,
+                        detach: Xu,
                         resize: Ju
                     } [e] || eh;
                 i[e] = r(t, e, n)
             }
             removeEventListener(t, e) {
                 const n = t.$proxies || (t.$proxies = {}),
                     i = n[e];
@@ -19705,16 +19705,16 @@
                     if (t > r) return t
                 }
                 return Math.max(r, 1)
             }(s, e, r);
             if (o > 0) {
                 let t, n;
                 const i = o > 1 ? Math.round((l - a) / (o - 1)) : null;
-                for (sh(e, c, u, Ko(i) ? 0 : a - i, a), t = 0, n = o - 1; t < n; t++) sh(e, c, u, s[t], s[t + 1]);
-                return sh(e, c, u, l, Ko(i) ? e.length : l + i), c
+                for (sh(e, c, u, qo(i) ? 0 : a - i, a), t = 0, n = o - 1; t < n; t++) sh(e, c, u, s[t], s[t + 1]);
+                return sh(e, c, u, l, qo(i) ? e.length : l + i), c
             }
             return sh(e, c, u), c
         }
 
         function sh(t, e, n, i, r) {
             const s = Jo(i, 0),
                 o = Math.min(Jo(r, t.length), t.length);
@@ -19749,19 +19749,19 @@
             return t.drawTicks ? t.tickLength : 0
         }
 
         function hh(t, e) {
             if (!t.display) return 0;
             const n = Ul(t.font, e),
                 i = Rl(t.padding);
-            return (qo(t.text) ? t.text.length : 1) * n.lineHeight + i.height
+            return (Xo(t.text) ? t.text.length : 1) * n.lineHeight + i.height
         }
 
         function dh(t, e, n) {
-            let i = Ka(t);
+            let i = qa(t);
             return (n && "right" !== e || !n && "right" === e) && (i = (t => "left" === t ? "right" : "right" === t ? "left" : t)(i)), i
         }
         class fh extends ih {
             constructor(t) {
                 super(), this.id = t.id, this.type = t.type, this.options = void 0, this.ctx = t.ctx, this.chart = t.chart, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this._margins = {
                     left: 0,
                     right: 0,
@@ -19996,15 +19996,15 @@
                 return "top" === e || "bottom" === e || "x" === t
             }
             isFullSize() {
                 return this.options.fullSize
             }
             _convertTicksToLabels(t) {
                 let e, n;
-                for (this.beforeTickToLabelConversion(), this.generateTickLabels(t), e = 0, n = t.length; e < n; e++) Ko(t[e].label) && (t.splice(e, 1), n--, e--);
+                for (this.beforeTickToLabelConversion(), this.generateTickLabels(t), e = 0, n = t.length; e < n; e++) qo(t[e].label) && (t.splice(e, 1), n--, e--);
                 this.afterTickToLabelConversion()
             }
             _getLabelSizes() {
                 let t = this._labelSizes;
                 if (!t) {
                     const e = this.options.ticks.sampleSize;
                     let n = this.ticks;
@@ -20019,17 +20019,17 @@
                 } = this, s = [], o = [], a = Math.floor(e / ah(e, n));
                 let l, c, u, h, d, f, p, g, m, y, b, v = 0,
                     x = 0;
                 for (l = 0; l < e; l += a) {
                     if (h = t[l].label, d = this._resolveTickFontOptions(l), i.font = f = d.string, p = r[f] = r[f] || {
                             data: {},
                             gc: []
-                        }, g = d.lineHeight, m = y = 0, Ko(h) || qo(h)) {
-                        if (qo(h))
-                            for (c = 0, u = h.length; c < u; ++c) b = h[c], Ko(b) || qo(b) || (m = yl(i, p.data, p.gc, m, b), y += g)
+                        }, g = d.lineHeight, m = y = 0, qo(h) || Xo(h)) {
+                        if (Xo(h))
+                            for (c = 0, u = h.length; c < u; ++c) b = h[c], qo(b) || Xo(b) || (m = yl(i, p.data, p.gc, m, b), y += g)
                     } else m = yl(i, p.data, p.gc, m, h), y = g;
                     s.push(m), o.push(y), v = Math.max(m, v), x = Math.max(y, x)
                 }! function(t, e) {
                     na(t, (t => {
                         const n = t.gc,
                             i = n.length / 2;
                         let r;
@@ -20240,15 +20240,15 @@
                     w = this._getYAxisLabelAlignment(h).textAlign
                 }
                 "y" === e && ("start" === a ? E = "top" : "end" === a && (E = "bottom"));
                 const D = this._getLabelSizes();
                 for (m = 0, y = o.length; m < y; ++m) {
                     b = o[m], v = b.label;
                     const t = r.setContext(this.getContext(m));
-                    S = this.getPixelForTick(m) + r.labelOffset, T = this._resolveTickFontOptions(m), k = T.lineHeight, M = qo(v) ? v.length : 1;
+                    S = this.getPixelForTick(m) + r.labelOffset, T = this._resolveTickFontOptions(m), k = T.lineHeight, M = Xo(v) ? v.length : 1;
                     const e = M / 2,
                         n = t.color,
                         a = t.textStrokeColor,
                         c = t.textStrokeWidth;
                     let h, d = w;
                     if (s ? (x = S, "inner" === w && (d = m === y - 1 ? this.options.reverse ? "left" : "right" : 0 === m ? this.options.reverse ? "right" : "left" : "center"), I = "top" === i ? "near" === l || 0 !== p ? -M * k + k / 2 : "center" === l ? -D.highest.height / 2 - e * k + k : -D.highest.height + k / 2 : "near" === l || 0 !== p ? k / 2 : "center" === l ? D.highest.height / 2 - e * k : D.highest.height - M * k, u && (I *= -1), 0 === p || t.showLabelBackdrop || (x += k / 2 * Math.sin(p))) : (_ = S, I = (1 - M) * k / 2), t.showLabelBackdrop) {
                         const e = Rl(t.backdropPadding),
@@ -20430,15 +20430,15 @@
                     }
                 } = this;
                 if (!n.display) return;
                 const r = Ul(n.font),
                     s = Rl(n.padding),
                     o = n.align;
                 let a = r.lineHeight / 2;
-                "bottom" === e || "center" === e || Qo(e) ? (a += s.bottom, qo(n.text) && (a += r.lineHeight * (n.text.length - 1))) : a += s.top;
+                "bottom" === e || "center" === e || Qo(e) ? (a += s.bottom, Xo(n.text) && (a += r.lineHeight * (n.text.length - 1))) : a += s.top;
                 const {
                     titleX: l,
                     titleY: c,
                     maxWidth: u,
                     rotation: h
                 } = function(t, e, n, i) {
                     const {
@@ -20451,27 +20451,27 @@
                         chartArea: c,
                         scales: u
                     } = l;
                     let h, d, f, p = 0;
                     const g = o - r,
                         m = a - s;
                     if (t.isHorizontal()) {
-                        if (d = qa(i, s, a), Qo(n)) {
+                        if (d = Xa(i, s, a), Qo(n)) {
                             const t = Object.keys(n)[0],
                                 i = n[t];
                             f = u[t].getPixelForValue(i) + g - e
                         } else f = "center" === n ? (c.bottom + c.top) / 2 + g - e : oh(t, n, e);
                         h = a - s
                     } else {
                         if (Qo(n)) {
                             const t = Object.keys(n)[0],
                                 i = n[t];
                             d = u[t].getPixelForValue(i) - m + e
                         } else d = "center" === n ? (c.left + c.right) / 2 - m + e : oh(t, n, e);
-                        f = qa(i, o, r), p = "left" === n ? -_a : _a
+                        f = Xa(i, o, r), p = "left" === n ? -_a : _a
                     }
                     return {
                         titleX: d,
                         titleY: f,
                         maxWidth: h,
                         rotation: p
                     }
@@ -20675,15 +20675,15 @@
                 for (const r of t) {
                     const t = r.plugin;
                     if (!1 === ea(t[n], [e, i, r.options], t) && i.cancelable) return !1
                 }
                 return !0
             }
             invalidate() {
-                Ko(this._cache) || (this._oldCache = this._cache, this._cache = void 0)
+                qo(this._cache) || (this._oldCache = this._cache, this._cache = void 0)
             }
             _descriptors(t) {
                 if (this._cache) return this._cache;
                 const e = this._cache = this._createDescriptors(t);
                 return this._notifyStateChanges(t), e
             }
             _createDescriptors(t, e) {
@@ -20942,15 +20942,15 @@
                             isScriptable: n,
                             isIndexable: i
                         } = Yl(t);
                         for (const r of e) {
                             const e = n(r),
                                 s = i(r),
                                 o = (s || e) && t[r];
-                            if (e && (pa(o) || Ph(o)) || s && qo(o)) return !0
+                            if (e && (pa(o) || Ph(o)) || s && Xo(o)) return !0
                         }
                         return !1
                     }(s, e)) {
                     r.$shared = !1;
                     a = Hl(s, n = pa(n) ? n() : n, this.createResolver(t, n, o))
                 }
                 for (const l of e) r[l] = a[l];
@@ -21043,15 +21043,15 @@
                 this.platform = new(n.platform || function(t) {
                     return !uc() || "undefined" !== typeof OffscreenCanvas && t instanceof OffscreenCanvas ? Vu : nh
                 }(i)), this.platform.updateConfig(n);
                 const o = this.platform.acquireContext(i, s.aspectRatio),
                     a = o && o.canvas,
                     l = a && a.height,
                     c = a && a.width;
-                this.id = Xo(), this.ctx = o, this.canvas = a, this.width = c, this.height = l, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new yh, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = function(t, e) {
+                this.id = Ko(), this.ctx = o, this.canvas = a, this.width = c, this.height = l, this._options = s, this._aspectRatio = this.aspectRatio, this._layers = [], this._metasets = [], this._stacks = void 0, this.boxes = [], this.currentDevicePixelRatio = void 0, this.chartArea = void 0, this._active = [], this._lastEvent = void 0, this._listeners = {}, this._responsiveListeners = void 0, this._sortedMetasets = [], this.scales = {}, this._plugins = new yh, this.$proxies = {}, this._hiddenIndices = {}, this.attached = !1, this._animationsDisabled = void 0, this.$context = void 0, this._doResize = function(t, e) {
                     let n;
                     return function() {
                         for (var i = arguments.length, r = new Array(i), s = 0; s < i; s++) r[s] = arguments[s];
                         return e ? (clearTimeout(n), n = setTimeout(t, e, r)) : t.apply(this, r), e
                     }
                 }((t => this.update(t)), s.resizeDelay || 0), this._dataChanges = [], Uh[this.id] = this, o && a ? (Nc.listen(this, "complete", Nh), Nc.listen(this, "progress", Bh), this._initialize(), this.attached && this.update()) : console.error("Failed to create chart: can't acquire context from the given item")
             }
@@ -21061,15 +21061,15 @@
                         aspectRatio: t,
                         maintainAspectRatio: e
                     },
                     width: n,
                     height: i,
                     _aspectRatio: r
                 } = this;
-                return Ko(t) ? e && r ? r : i ? n / i : null : t
+                return qo(t) ? e && r ? r : i ? n / i : null : t
             }
             get data() {
                 return this.config.data
             }
             set data(t) {
                 this.config.data = t
             }
@@ -21599,22 +21599,22 @@
                 outerStart: a(r.outerStart),
                 outerEnd: a(r.outerEnd),
                 innerStart: Ba(r.innerStart, 0, o),
                 innerEnd: Ba(r.innerEnd, 0, o)
             }
         }
 
-        function Xh(t, e, n, i) {
+        function Kh(t, e, n, i) {
             return {
                 x: n + t * Math.cos(e),
                 y: i + t * Math.sin(e)
             }
         }
 
-        function Kh(t, e, n, i, r, s) {
+        function qh(t, e, n, i, r, s) {
             const {
                 x: o,
                 y: a,
                 startAngle: l,
                 pixelMargin: c,
                 innerRadius: u
             } = e, h = Math.max(e.outerRadius + i + n - c, 0), d = u > 0 ? u + i + n + c : 0;
@@ -21640,45 +21640,45 @@
                 M = d + x,
                 I = d + _,
                 E = m + x / M,
                 D = y - _ / I;
             if (t.beginPath(), s) {
                 const e = (T + k) / 2;
                 if (t.arc(o, a, h, T, e), t.arc(o, a, h, e, k), v > 0) {
-                    const e = Xh(S, k, o, a);
+                    const e = Kh(S, k, o, a);
                     t.arc(e.x, e.y, v, k, y + _a)
                 }
-                const n = Xh(I, y, o, a);
+                const n = Kh(I, y, o, a);
                 if (t.lineTo(n.x, n.y), _ > 0) {
-                    const e = Xh(I, D, o, a);
+                    const e = Kh(I, D, o, a);
                     t.arc(e.x, e.y, _, y + _a, D + Math.PI)
                 }
                 const i = (y - _ / d + (m + x / d)) / 2;
                 if (t.arc(o, a, d, y - _ / d, i, !0), t.arc(o, a, d, i, m + x / d, !0), x > 0) {
-                    const e = Xh(M, E, o, a);
+                    const e = Kh(M, E, o, a);
                     t.arc(e.x, e.y, x, E + Math.PI, m - _a)
                 }
-                const r = Xh(w, m, o, a);
+                const r = Kh(w, m, o, a);
                 if (t.lineTo(r.x, r.y), b > 0) {
-                    const e = Xh(w, T, o, a);
+                    const e = Kh(w, T, o, a);
                     t.arc(e.x, e.y, b, m - _a, T)
                 }
             } else {
                 t.moveTo(o, a);
                 const e = Math.cos(T) * h + o,
                     n = Math.sin(T) * h + a;
                 t.lineTo(e, n);
                 const i = Math.cos(k) * h + o,
                     r = Math.sin(k) * h + a;
                 t.lineTo(i, r)
             }
             t.closePath()
         }
 
-        function qh(t, e, n, i, r) {
+        function Xh(t, e, n, i, r) {
             const {
                 fullCircles: s,
                 startAngle: o,
                 circumference: a,
                 options: l
             } = e, {
                 borderWidth: c,
@@ -21686,30 +21686,30 @@
                 borderDash: h,
                 borderDashOffset: d
             } = l, f = "inner" === l.borderAlign;
             if (!c) return;
             t.setLineDash(h || []), t.lineDashOffset = d, f ? (t.lineWidth = 2 * c, t.lineJoin = u || "round") : (t.lineWidth = c, t.lineJoin = u || "bevel");
             let p = e.endAngle;
             if (s) {
-                Kh(t, e, n, i, p, r);
+                qh(t, e, n, i, p, r);
                 for (let e = 0; e < s; ++e) t.stroke();
                 isNaN(a) || (p = o + (a % ya || ya))
             }
             f && function(t, e, n) {
                 const {
                     startAngle: i,
                     pixelMargin: r,
                     x: s,
                     y: o,
                     outerRadius: a,
                     innerRadius: l
                 } = e;
                 let c = r / a;
                 t.beginPath(), t.arc(s, o, a, i - c, n + c), l > r ? (c = r / l, t.arc(s, o, l, n + c, i - c, !0)) : t.arc(s, o, r, n + _a, i - _a), t.closePath(), t.clip()
-            }(t, e, p), s || (Kh(t, e, n, i, p, r), t.stroke())
+            }(t, e, p), s || (qh(t, e, n, i, p, r), t.stroke())
         }
         ho(Hh, "defaults", ml), ho(Hh, "instances", Uh), ho(Hh, "overrides", hl), ho(Hh, "registry", mh), ho(Hh, "version", "4.4.2"), ho(Hh, "getChart", Vh);
         class Qh extends ih {
             constructor(t) {
                 super(), ho(this, "circumference", void 0), ho(this, "endAngle", void 0), ho(this, "fullCircles", void 0), ho(this, "innerRadius", void 0), ho(this, "outerRadius", void 0), ho(this, "pixelMargin", void 0), ho(this, "startAngle", void 0), this.options = void 0, this.circumference = void 0, this.startAngle = void 0, this.endAngle = void 0, this.innerRadius = void 0, this.outerRadius = void 0, this.pixelMargin = 0, this.fullCircles = 0, t && Object.assign(this, t)
             }
             inRange(t, e, n) {
@@ -21768,20 +21768,20 @@
                         const {
                             fullCircles: s,
                             startAngle: o,
                             circumference: a
                         } = e;
                         let l = e.endAngle;
                         if (s) {
-                            Kh(t, e, n, i, l, r);
+                            qh(t, e, n, i, l, r);
                             for (let e = 0; e < s; ++e) t.fill();
                             isNaN(a) || (l = o + (a % ya || ya))
                         }
-                        Kh(t, e, n, i, l, r), t.fill()
-                    }(t, this, a, r, s), qh(t, this, a, r, s), t.restore()
+                        qh(t, e, n, i, l, r), t.fill()
+                    }(t, this, a, r, s), Xh(t, this, a, r, s), t.restore()
             }
         }
 
         function Gh(t, e) {
             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : e;
             t.lineCap = Jo(n.borderCapStyle, e.borderCapStyle), t.setLineDash(Jo(n.borderDash, e.borderDash)), t.lineDashOffset = Jo(n.borderDashOffset, e.borderDashOffset), t.lineJoin = Jo(n.borderJoinStyle, e.borderJoinStyle), t.lineWidth = Jo(n.borderWidth, e.borderWidth), t.strokeStyle = Jo(n.borderColor, e.borderColor)
         }
@@ -22366,15 +22366,15 @@
                         return l && (r = Ba(Va(e, s.axis, o).lo, 0, n - 1)), i = c ? Ba(Va(e, s.axis, a).hi + 1, r, n) - r : n - r, {
                             start: r,
                             count: i
                         }
                     }(a, l);
                     if (h <= (n.threshold || 4 * i)) return void Sd(e);
                     let d;
-                    switch (Ko(s) && (e._data = l, delete e.data, Object.defineProperty(e, "data", {
+                    switch (qo(s) && (e._data = l, delete e.data, Object.defineProperty(e, "data", {
                             configurable: !0,
                             enumerable: !0,
                             get: function() {
                                 return this._decimated
                             },
                             set: function(t) {
                                 this._data = t
@@ -22419,15 +22419,15 @@
                                     v = t[y].x - b;
                                 for (r = e; r < e + n; ++r) {
                                     s = t[r], o = (s.x - b) / v * i, a = s.y;
                                     const e = 0 | o;
                                     if (e === l) a < d ? (d = a, c = r) : a > f && (f = a, u = r), p = (g * p + s.x) / ++g;
                                     else {
                                         const n = r - 1;
-                                        if (!Ko(c) && !Ko(u)) {
+                                        if (!qo(c) && !qo(u)) {
                                             const e = Math.min(c, u),
                                                 i = Math.max(c, u);
                                             e !== h && e !== n && m.push({
                                                 ...t[e],
                                                 x: p
                                             }), i !== h && i !== n && m.push({
                                                 ...t[i],
@@ -22473,15 +22473,15 @@
         function Ed(t, e, n, i) {
             return t && e ? i(t[n], e[n]) : t ? t[n] : e ? e[n] : 0
         }
 
         function Dd(t, e) {
             let n = [],
                 i = !1;
-            return qo(t) ? (i = !0, n = t) : n = function(t, e) {
+            return Xo(t) ? (i = !0, n = t) : n = function(t, e) {
                 const {
                     x: n = null,
                     y: i = null
                 } = t || {}, r = e.points, s = [];
                 return e.segments.forEach((t => {
                     let {
                         start: e,
@@ -23031,20 +23031,20 @@
                             },
                             rtl: r
                         }
                     } = this,
                     s = Mc(r, this.left, this.width);
                 if (this.isHorizontal()) {
                     let r = 0,
-                        o = qa(n, this.left + i, this.right - this.lineWidths[r]);
-                    for (const a of e) r !== a.row && (r = a.row, o = qa(n, this.left + i, this.right - this.lineWidths[r])), a.top += this.top + t + i, a.left = s.leftForLtr(s.x(o), a.width), o += a.width + i
+                        o = Xa(n, this.left + i, this.right - this.lineWidths[r]);
+                    for (const a of e) r !== a.row && (r = a.row, o = Xa(n, this.left + i, this.right - this.lineWidths[r])), a.top += this.top + t + i, a.left = s.leftForLtr(s.x(o), a.width), o += a.width + i
                 } else {
                     let r = 0,
-                        o = qa(n, this.top + t + i, this.bottom - this.columnSizes[r].height);
-                    for (const a of e) a.col !== r && (r = a.col, o = qa(n, this.top + t + i, this.bottom - this.columnSizes[r].height)), a.top = o, a.left += this.left + i, a.left = s.leftForLtr(s.x(a.left), a.width), o += a.height + i
+                        o = Xa(n, this.top + t + i, this.bottom - this.columnSizes[r].height);
+                    for (const a of e) a.col !== r && (r = a.col, o = Xa(n, this.top + t + i, this.bottom - this.columnSizes[r].height)), a.top = o, a.left += this.left + i, a.left = s.leftForLtr(s.x(a.left), a.width), o += a.height + i
                 }
             }
             isHorizontal() {
                 return "top" === this.options.position || "bottom" === this.options.position
             }
             draw() {
                 if (this.options.display) {
@@ -23068,31 +23068,31 @@
                 this.drawTitle(), i.textAlign = a.textAlign("left"), i.textBaseline = "middle", i.lineWidth = .5, i.font = l.string;
                 const {
                     boxWidth: f,
                     boxHeight: p,
                     itemHeight: g
                 } = Wd(s, u), m = this.isHorizontal(), y = this._computeTitleHeight();
                 d = m ? {
-                    x: qa(r, this.left + c, this.right - n[0]),
+                    x: Xa(r, this.left + c, this.right - n[0]),
                     y: this.top + c + y,
                     line: 0
                 } : {
                     x: this.left + c,
-                    y: qa(r, this.top + y + c, this.bottom - e[0].height),
+                    y: Xa(r, this.top + y + c, this.bottom - e[0].height),
                     line: 0
                 }, Ic(this.ctx, t.textDirection);
                 const b = g + c;
                 this.legendItems.forEach(((v, x) => {
                     i.strokeStyle = v.fontColor, i.fillStyle = v.fontColor;
                     const _ = i.measureText(v.text).width,
                         w = a.textAlign(v.textAlign || (v.textAlign = s.textAlign)),
                         S = f + h + _;
                     let T = d.x,
                         k = d.y;
-                    a.setWidth(this.width), m ? x > 0 && T + S + c > this.right && (k = d.y += b, d.line++, T = d.x = qa(r, this.left + c, this.right - n[d.line])) : x > 0 && k + b > this.bottom && (T = d.x = T + e[d.line].width + c, d.line++, k = d.y = qa(r, this.top + y + c, this.bottom - e[d.line].height));
+                    a.setWidth(this.width), m ? x > 0 && T + S + c > this.right && (k = d.y += b, d.line++, T = d.x = Xa(r, this.left + c, this.right - n[d.line])) : x > 0 && k + b > this.bottom && (T = d.x = T + e[d.line].width + c, d.line++, k = d.y = Xa(r, this.top + y + c, this.bottom - e[d.line].height));
                     if (function(t, e, n) {
                             if (isNaN(f) || f <= 0 || isNaN(p) || p < 0) return;
                             i.save();
                             const r = Jo(n.lineWidth, 1);
                             if (i.fillStyle = Jo(n.fillStyle, o), i.lineCap = Jo(n.lineCap, "butt"), i.lineDashOffset = Jo(n.lineDashOffset, 0), i.lineJoin = Jo(n.lineJoin, "miter"), i.lineWidth = r, i.strokeStyle = Jo(n.strokeStyle, o), i.setLineDash(Jo(n.lineDash, [])), s.usePointStyle) {
                                 const o = {
                                         radius: p * Math.SQRT2 / 2,
@@ -23136,21 +23136,21 @@
                 const r = Mc(t.rtl, this.left, this.width),
                     s = this.ctx,
                     o = e.position,
                     a = n.size / 2,
                     l = i.top + a;
                 let c, u = this.left,
                     h = this.width;
-                if (this.isHorizontal()) h = Math.max(...this.lineWidths), c = this.top + l, u = qa(t.align, u, this.right - h);
+                if (this.isHorizontal()) h = Math.max(...this.lineWidths), c = this.top + l, u = Xa(t.align, u, this.right - h);
                 else {
                     const e = this.columnSizes.reduce(((t, e) => Math.max(t, e.height)), 0);
-                    c = l + qa(t.align, this.top, this.bottom - e - t.labels.padding - this._computeTitleHeight())
+                    c = l + Xa(t.align, this.top, this.bottom - e - t.labels.padding - this._computeTitleHeight())
                 }
-                const d = qa(o, u, u + h);
-                s.textAlign = r.textAlign(Ka(o)), s.textBaseline = "middle", s.strokeStyle = e.color, s.fillStyle = e.color, s.font = n.string, Ol(s, e.text, d, c, n)
+                const d = Xa(o, u, u + h);
+                s.textAlign = r.textAlign(qa(o)), s.textBaseline = "middle", s.strokeStyle = e.color, s.fillStyle = e.color, s.font = n.string, Ol(s, e.text, d, c, n)
             }
             _computeTitleHeight() {
                 const t = this.options.title,
                     e = Ul(t.font),
                     n = Rl(t.padding);
                 return t.display ? e.lineHeight + n.height : 0
             }
@@ -23269,23 +23269,23 @@
             descriptors: {
                 _scriptable: t => !t.startsWith("on"),
                 labels: {
                     _scriptable: t => !["generateLabels", "filter", "sort"].includes(t)
                 }
             }
         };
-        class Xd extends ih {
+        class Kd extends ih {
             constructor(t) {
                 super(), this.chart = t.chart, this.options = t.options, this.ctx = t.ctx, this._padding = void 0, this.top = void 0, this.bottom = void 0, this.left = void 0, this.right = void 0, this.width = void 0, this.height = void 0, this.position = void 0, this.weight = void 0, this.fullSize = void 0
             }
             update(t, e) {
                 const n = this.options;
                 if (this.left = 0, this.top = 0, !n.display) return void(this.width = this.height = this.right = this.bottom = 0);
                 this.width = this.right = t, this.height = this.bottom = e;
-                const i = qo(n.text) ? n.text.length : 1;
+                const i = Xo(n.text) ? n.text.length : 1;
                 this._padding = Rl(n.padding);
                 const r = i * Ul(n.font).lineHeight + this._padding.height;
                 this.isHorizontal() ? this.height = r : this.width = r
             }
             isHorizontal() {
                 const t = this.options.position;
                 return "top" === t || "bottom" === t
@@ -23295,15 +23295,15 @@
                     top: e,
                     left: n,
                     bottom: i,
                     right: r,
                     options: s
                 } = this, o = s.align;
                 let a, l, c, u = 0;
-                return this.isHorizontal() ? (l = qa(o, n, r), c = e + t, a = r - n) : ("left" === s.position ? (l = n + t, c = qa(o, i, e), u = -.5 * ma) : (l = r - t, c = qa(o, e, i), u = .5 * ma), a = i - e), {
+                return this.isHorizontal() ? (l = Xa(o, n, r), c = e + t, a = r - n) : ("left" === s.position ? (l = n + t, c = Xa(o, i, e), u = -.5 * ma) : (l = r - t, c = Xa(o, e, i), u = .5 * ma), a = i - e), {
                     titleX: l,
                     titleY: c,
                     maxWidth: a,
                     rotation: u
                 }
             }
             draw() {
@@ -23318,26 +23318,26 @@
                         maxWidth: o,
                         rotation: a
                     } = this._drawArgs(i);
                 Ol(t, e.text, 0, 0, n, {
                     color: e.color,
                     maxWidth: o,
                     rotation: a,
-                    textAlign: Ka(e.align),
+                    textAlign: qa(e.align),
                     textBaseline: "middle",
                     translation: [r, s]
                 })
             }
         }
-        var Kd = {
+        var qd = {
             id: "title",
-            _element: Xd,
+            _element: Kd,
             start(t, e, n) {
                 ! function(t, e) {
-                    const n = new Xd({
+                    const n = new Kd({
                         ctx: t.ctx,
                         options: e,
                         chart: t
                     });
                     Ru.configure(t, n, e), Ru.addBox(t, n), t.titleBlock = n
                 }(t, n)
             },
@@ -23365,30 +23365,30 @@
                 color: "color"
             },
             descriptors: {
                 _scriptable: !0,
                 _indexable: !1
             }
         };
-        const qd = new WeakMap;
+        const Xd = new WeakMap;
         var Qd = {
             id: "subtitle",
             start(t, e, n) {
-                const i = new Xd({
+                const i = new Kd({
                     ctx: t.ctx,
                     options: n,
                     chart: t
                 });
-                Ru.configure(t, i, n), Ru.addBox(t, i), qd.set(t, i)
+                Ru.configure(t, i, n), Ru.addBox(t, i), Xd.set(t, i)
             },
             stop(t) {
-                Ru.removeBox(t, qd.get(t)), qd.delete(t)
+                Ru.removeBox(t, Xd.get(t)), Xd.delete(t)
             },
             beforeUpdate(t, e, n) {
-                const i = qd.get(t);
+                const i = Xd.get(t);
                 Ru.configure(t, i, n), i.options = n
             },
             defaults: {
                 align: "center",
                 display: !1,
                 font: {
                     weight: "normal"
@@ -23445,15 +23445,15 @@
                     x: s,
                     y: o
                 }
             }
         };
 
         function Zd(t, e) {
-            return e && (qo(e) ? Array.prototype.push.apply(t, e) : t.push(e)), t
+            return e && (Xo(e) ? Array.prototype.push.apply(t, e) : t.push(e)), t
         }
 
         function Jd(t) {
             return ("string" === typeof t || t instanceof String) && t.indexOf("\n") > -1 ? t.split("\n") : t
         }
 
         function tf(t, e) {
@@ -23615,15 +23615,15 @@
             beforeBody: $o,
             beforeLabel: $o,
             label(t) {
                 if (this && this.options && "dataset" === this.options.mode) return t.label + ": " + t.formattedValue || t.formattedValue;
                 let e = t.dataset.label || "";
                 e && (e += ": ");
                 const n = t.formattedValue;
-                return Ko(n) || (e += n), e
+                return qo(n) || (e += n), e
             },
             labelColor(t) {
                 const e = t.chart.getDatasetMeta(t.datasetIndex).controller.getStyle(t.dataIndex);
                 return {
                     borderColor: e.borderColor,
                     backgroundColor: e.backgroundColor,
                     borderWidth: e.borderWidth,
@@ -24088,15 +24088,15 @@
             ff = Object.freeze({
                 __proto__: null,
                 Colors: wd,
                 Decimation: kd,
                 Filler: jd,
                 Legend: $d,
                 SubTitle: Qd,
-                Title: Kd,
+                Title: qd,
                 Tooltip: df
             });
 
         function pf(t, e, n, i) {
             const r = t.indexOf(e);
             if (-1 === r) return ((t, e, n, i) => ("string" === typeof e ? (n = t.push(e) - 1, i.unshift({
                 index: n,
@@ -24123,15 +24123,15 @@
                         }
                         of e) t[n] === i && t.splice(n, 1);
                     this._addedLabels = []
                 }
                 super.init(t)
             }
             parse(t, e) {
-                if (Ko(t)) return null;
+                if (qo(t)) return null;
                 const n = this.getLabels();
                 return ((t, e) => null === t ? null : Ba(Math.round(t), 0, e))(e = isFinite(e) && n[e] === t ? e : pf(n, t, Jo(e, t), this._addedLabels), n.length - 1)
             }
             determineDataLimits() {
                 const {
                     minDefined: t,
                     maxDefined: e
@@ -24190,30 +24190,30 @@
                 } = t,
                 d = r || 1,
                 f = c - 1,
                 {
                     min: p,
                     max: g
                 } = e,
-                m = !Ko(s),
-                y = !Ko(o),
-                b = !Ko(l),
+                m = !qo(s),
+                y = !qo(o),
+                b = !qo(l),
                 v = (g - p) / (u + 1);
             let x, _, w, S, T = Ia((g - p) / f / d) * d;
             if (T < 1e-14 && !m && !y) return [{
                 value: p
             }, {
                 value: g
             }];
-            S = Math.ceil(g / T) - Math.floor(p / T), S > f && (T = Ia(S * T / f / d) * d), Ko(a) || (x = Math.pow(10, a), T = Math.ceil(T * x) / x), "ticks" === i ? (_ = Math.floor(p / T) * T, w = Math.ceil(g / T) * T) : (_ = p, w = g), m && y && r && function(t, e) {
+            S = Math.ceil(g / T) - Math.floor(p / T), S > f && (T = Ia(S * T / f / d) * d), qo(a) || (x = Math.pow(10, a), T = Math.ceil(T * x) / x), "ticks" === i ? (_ = Math.floor(p / T) * T, w = Math.ceil(g / T) * T) : (_ = p, w = g), m && y && r && function(t, e) {
                 const n = Math.round(t);
                 return n - e <= t && n + e >= t
             }((o - s) / r, T / 1e3) ? (S = Math.round(Math.min((o - s) / T, c)), T = (o - s) / S, _ = s, w = o) : b ? (_ = m ? s : _, w = y ? o : w, S = l - 1, T = (w - _) / S) : (S = (w - _) / T, S = Ma(S, Math.round(S), T / 1e3) ? Math.round(S) : Math.ceil(S));
             const k = Math.max(Aa(T), Aa(_));
-            x = Math.pow(10, Ko(a) ? k : a), _ = Math.round(_ * x) / x, w = Math.round(w * x) / x;
+            x = Math.pow(10, qo(a) ? k : a), _ = Math.round(_ * x) / x, w = Math.round(w * x) / x;
             let M = 0;
             for (m && (h && _ !== s ? (n.push({
                     value: s
                 }), _ < s && M++, Ma(Math.round((_ + M * T) * x) / x, s, bf(s, v, t)) && M++) : _ < s && M++); M < S; ++M) {
                 const t = Math.round((_ + M * T) * x) / x;
                 if (y && t > o) break;
                 n.push({
@@ -24243,15 +24243,15 @@
             }
         });
         class vf extends fh {
             constructor(t) {
                 super(t), this.start = void 0, this.end = void 0, this._startValue = void 0, this._endValue = void 0, this._valueRange = 0
             }
             parse(t, e) {
-                return Ko(t) || ("number" === typeof t || t instanceof Number) && !isFinite(+t) ? null : +t
+                return qo(t) || ("number" === typeof t || t instanceof Number) && !isFinite(+t) ? null : +t
             }
             handleTickRangeOptions() {
                 const {
                     beginAtZero: t
                 } = this.options, {
                     minDefined: e,
                     maxDefined: n
@@ -24479,15 +24479,15 @@
                 o = t.options.pointLabels,
                 a = o.centerPointLabels ? ma / s : 0;
             for (let h = 0; h < s; h++) {
                 const s = o.setContext(t.getPointLabelContext(h));
                 r[h] = s.padding;
                 const d = t.getPointPosition(h, t.drawingArea + r[h], a),
                     f = Ul(s.font),
-                    p = (l = t.ctx, c = f, u = qo(u = t._pointLabels[h]) ? u : [u], {
+                    p = (l = t.ctx, c = f, u = Xo(u = t._pointLabels[h]) ? u : [u], {
                         w: bl(l, c.string, u),
                         h: u.length * c.lineHeight
                     });
                 i[h] = p;
                 const g = za(t.getIndexAngle(h) + a),
                     m = Math.round(Ca(g));
                 Of(n, e, g, Ef(m, d.x, p.w, 0, 180), Ef(m, d.y, p.h, 90, 270))
@@ -24586,15 +24586,15 @@
                 left: i,
                 top: r,
                 right: s,
                 bottom: o
             } = n, {
                 backdropColor: a
             } = e;
-            if (!Ko(a)) {
+            if (!qo(a)) {
                 const n = Bl(e.borderRadius),
                     l = Rl(e.backdropPadding);
                 t.fillStyle = a;
                 const c = i - l.left,
                     u = r - l.top,
                     h = s - i + l.width,
                     d = o - r + l.height;
@@ -24660,20 +24660,20 @@
             setCenterPoint(t, e, n, i) {
                 this.xCenter += Math.floor((t - e) / 2), this.yCenter += Math.floor((n - i) / 2), this.drawingArea -= Math.min(this.drawingArea / 2, Math.max(t, e, n, i))
             }
             getIndexAngle(t) {
                 return za(t * (ya / (this._pointLabels.length || 1)) + Oa(this.options.startAngle || 0))
             }
             getDistanceFromCenterForValue(t) {
-                if (Ko(t)) return NaN;
+                if (qo(t)) return NaN;
                 const e = this.drawingArea / (this.max - this.min);
                 return this.options.reverse ? (this.max - t) * e : (t - this.min) * e
             }
             getValueForDistanceFromCenter(t) {
-                if (Ko(t)) return NaN;
+                if (qo(t)) return NaN;
                 const e = t / (this.drawingArea / (this.max - this.min));
                 return this.options.reverse ? this.max - e : this.min + e
             }
             getPointLabelContext(t) {
                 const e = this._pointLabels || [];
                 if (t >= 0 && t < e.length) {
                     const n = e[t];
@@ -24902,15 +24902,15 @@
             Nf = Object.keys(zf);
 
         function Bf(t, e) {
             return t - e
         }
 
         function Rf(t, e) {
-            if (Ko(e)) return null;
+            if (qo(e)) return null;
             const n = t._adapter,
                 {
                     parser: i,
                     round: r,
                     isoWeekday: s
                 } = t._parseOpts;
             let o = e;
@@ -25251,17 +25251,17 @@
             CategoryScale: mf,
             LinearScale: xf,
             LogarithmicScale: Mf,
             RadialLinearScale: Lf,
             TimeScale: Wf,
             TimeSeriesScale: Yf
         })];
-        var Xf = i(895),
-            Kf = i.n(Xf);
-        const qf = t => t && t.enabled && t.modifierKey,
+        var Kf = i(895),
+            qf = i.n(Kf);
+        const Xf = t => t && t.enabled && t.modifierKey,
             Qf = (t, e) => t && e[t + "Key"],
             Gf = (t, e) => t && !e[t + "Key"];
 
         function Zf(t, e, n) {
             return void 0 === t || ("string" === typeof t ? -1 !== t.indexOf(e) : "function" === typeof t && -1 !== t({
                 chart: n
             }).indexOf(e))
@@ -25668,15 +25668,15 @@
 
         function Dp(t, e) {
             const n = np(t),
                 {
                     pan: i,
                     zoom: r = {}
                 } = n.options;
-            if (0 !== e.button || Qf(qf(i), e) || Gf(qf(r.drag), e)) return ea(r.onZoomRejected, [{
+            if (0 !== e.button || Qf(Xf(i), e) || Gf(Xf(r.drag), e)) return ea(r.onZoomRejected, [{
                 chart: t,
                 event: e
             }]);
             !1 !== Ep(t, e, r) && (n.dragStart = e, kp(t, t.canvas, "mousemove", Mp), kp(t, window.document, "keydown", Ip))
         }
 
         function Op(t, e, n, i) {
@@ -25736,15 +25736,15 @@
                     onZoomComplete: n
                 },
                 options: {
                     zoom: i
                 }
             } = np(t);
             if (! function(t, e, n) {
-                    if (Gf(qf(n.wheel), e)) ea(n.onZoomRejected, [{
+                    if (Gf(Xf(n.wheel), e)) ea(n.onZoomRejected, [{
                         chart: t,
                         event: e
                     }]);
                     else if (!1 !== Ep(t, e, n) && (e.cancelable && e.preventDefault(), void 0 !== e.deltaY)) return !0
                 }(t, e, i)) return;
             const r = e.target.getBoundingClientRect(),
                 s = 1 + (e.deltaY >= 0 ? -i.wheel.speed : i.wheel.speed);
@@ -25773,15 +25773,15 @@
             return function(n, i) {
                 const {
                     pan: r,
                     zoom: s = {}
                 } = e.options;
                 if (!r || !r.enabled) return !1;
                 const o = i && i.srcEvent;
-                return !o || (!(!e.panning && "mouse" === i.pointerType && (Gf(qf(r), o) || Qf(qf(s.drag), o))) || (ea(r.onPanRejected, [{
+                return !o || (!(!e.panning && "mouse" === i.pointerType && (Gf(Xf(r), o) || Qf(Xf(s.drag), o))) || (ea(r.onPanRejected, [{
                     chart: t,
                     event: i
                 }]), !1))
             }
         }
 
         function Lp(t, e, n) {
@@ -25825,22 +25825,22 @@
         function Bp(t, e) {
             const n = np(t),
                 i = t.canvas,
                 {
                     pan: r,
                     zoom: s
                 } = e,
-                o = new(Kf().Manager)(i);
-            s && s.pinch.enabled && (o.add(new(Kf().Pinch)), o.on("pinchstart", (() => function(t, e) {
+                o = new(qf().Manager)(i);
+            s && s.pinch.enabled && (o.add(new(qf().Pinch)), o.on("pinchstart", (() => function(t, e) {
                 e.options.zoom.pinch.enabled && (e.scale = 1)
             }(0, n))), o.on("pinch", (e => Lp(t, n, e))), o.on("pinchend", (e => function(t, e, n) {
                 e.scale && (Lp(t, e, n), e.scale = null, ea(e.options.zoom.onZoomComplete, [{
                     chart: t
                 }]))
-            }(t, n, e)))), r && r.enabled && (o.add(new(Kf().Pan)({
+            }(t, n, e)))), r && r.enabled && (o.add(new(qf().Pan)({
                 threshold: r.threshold,
                 enable: Fp(t, n)
             })), o.on("panstart", (e => function(t, e, n) {
                 const {
                     enabled: i,
                     onPanStart: r,
                     onPanRejected: s
@@ -25909,15 +25909,15 @@
                     pinch: {
                         enabled: !1
                     },
                     mode: "xy"
                 }
             },
             start: function(t, e, n) {
-                np(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), Kf() && Bp(t, n), t.pan = (e, n, i) => wp(t, e, n, i), t.zoom = (e, n) => bp(t, e, n), t.zoomRect = (e, n, i) => vp(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
+                np(t).options = n, Object.prototype.hasOwnProperty.call(n.zoom, "enabled") && console.warn("The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`."), (Object.prototype.hasOwnProperty.call(n.zoom, "overScaleMode") || Object.prototype.hasOwnProperty.call(n.pan, "overScaleMode")) && console.warn("The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired)."), qf() && Bp(t, n), t.pan = (e, n, i) => wp(t, e, n, i), t.zoom = (e, n) => bp(t, e, n), t.zoomRect = (e, n, i) => vp(t, e, n, i), t.zoomScale = (e, n, i) => function(t, e, n) {
                     let i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "none";
                     pp(t, np(t)), sp(t.scales[e], n, void 0, !0), t.update(i)
                 }(t, e, n, i), t.resetZoom = e => function(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "default";
                     const n = np(t),
                         i = pp(t, n);
                     na(t.scales, (function(t) {
@@ -25966,15 +25966,15 @@
             },
             afterDraw(t, e, n) {
                 Rp(t, "afterDraw", n)
             },
             stop: function(t) {
                 ! function(t) {
                     Tp(t, "mousedown"), Tp(t, "mousemove"), Tp(t, "mouseup"), Tp(t, "wheel"), Tp(t, "click"), Tp(t, "keydown")
-                }(t), Kf() && function(t) {
+                }(t), qf() && function(t) {
                         const e = Np.get(t);
                         e && (e.remove("pinchstart"), e.remove("pinch"), e.remove("pinchend"), e.remove("panstart"), e.remove("pan"), e.remove("panend"), e.destroy(), Np.delete(t))
                     }(t),
                     function(t) {
                         ep.delete(t)
                     }(t)
             },
@@ -26014,15 +26014,15 @@
 
         function $p(t, e) {
             return t.getElementsAtEventForMode(e.nativeEvent, "nearest", {
                 intersect: !0
             }, !1)
         }
 
-        function Xp(t, e) {
+        function Kp(t, e) {
             const {
                 height: n = 150,
                 width: i = 300,
                 redraw: r = !1,
                 datasetIdKey: s,
                 type: o,
                 data: a,
@@ -26059,24 +26059,24 @@
             }), [o]), (0, f.useEffect)((() => (m(), () => y())), []), f.createElement("canvas", Object.assign({
                 ref: p,
                 role: "img",
                 height: n,
                 width: i
             }, d), u)
         }
-        const Kp = (0, f.forwardRef)(Xp);
+        const qp = (0, f.forwardRef)(Kp);
 
-        function qp(t, e) {
-            return Hh.register(e), (0, f.forwardRef)(((e, n) => f.createElement(Kp, Object.assign({}, e, {
+        function Xp(t, e) {
+            return Hh.register(e), (0, f.forwardRef)(((e, n) => f.createElement(qp, Object.assign({}, e, {
                 ref: n,
                 type: t
             }))))
         }
-        const Qp = qp("line", hu),
-            Gp = qp("scatter", gu);
+        const Qp = Xp("line", hu),
+            Gp = Xp("scatter", gu);
 
         function Zp(t, e) {
             return {
                 labels: Object.keys(t[Object.keys(t)[0]].data),
                 datasets: Object.entries(t).map(((t, n) => {
                     let [i, r] = t;
                     return {
@@ -26172,25 +26172,26 @@
                 },
                 onHover: (t, e, n) => {
                     t.native.target.style.cursor = e ? "pointer" : "default"
                 }
             }
         }
 
-        function rg(t, e, n) {
-            return "linear" === n.x_type ? (0, Jp.Ay)(t) : this.getLabelForValue(t)
+        function rg(t, e) {
+            return e ? (0, Jp.Ay)(t) : this.getLabelForValue(t)
         }
 
         function sg(t, e) {
             const n = {
                 display: !0,
                 type: t.x_type,
                 ticks: {
                     callback: function(e, n) {
-                        return rg.call(this, e, n, t)
+                        const i = "linear" === t.x_type && t.x_format;
+                        return rg.call(this, e, i)
                     }
                 },
                 title: {
                     display: Boolean(t.x_label),
                     text: t.x_label
                 },
                 grid: {
@@ -26200,15 +26201,16 @@
             };
             t.x_labels && (n.min = t.x_labels[0], n.max = t.x_labels[t.x_labels.length - 1]);
             const i = {
                 display: !0,
                 type: t.y_type,
                 ticks: {
                     callback: function(e, n) {
-                        return rg.call(this, e, n, t)
+                        const i = "linear" === t.y_type && t.y_format;
+                        return rg.call(this, e, i)
                     }
                 },
                 title: {
                     display: Boolean(t.y_label),
                     text: t.y_label
                 },
                 grid: {
@@ -26237,49 +26239,68 @@
                         const e = t.parsed.x.toFixed(2),
                             n = t.parsed.y.toFixed(2);
                         return "".concat(e, ", ").concat(n)
                     }
                 }
             }
         }
-        var ag = i(579);
+
+        function ag(t, e, n) {
+            if ("category" === (arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "linear")) {
+                const i = n.getLabels();
+                return i[Math.round(cg(t.y, e.top, e.bottom, 0, i.length - 1))]
+            }
+            return cg(t.y, e.bottom, e.top, n.min, n.max)
+        }
+
+        function lg(t, e, n) {
+            if ("category" === (arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : "linear")) {
+                const i = n.getLabels();
+                return i[Math.round(cg(t.x, e.left, e.right, 0, i.length - 1))]
+            }
+            return cg(t.x, e.left, e.right, n.min, n.max)
+        }
+
+        function cg(t, e, n, i, r) {
+            return i + (t - e) / (n - e) * (r - i)
+        }
+        var ug = i(579);
         Hh.register(...$f, Up);
-        const lg = class extends ao {
+        const hg = class extends ao {
             constructor(t) {
                 super(t), this.downHandler = t => {
                     const e = $p(this.chartRef.current, t);
                     if (e.length > 0) {
                         const t = this.chartRef.current.data.datasets[e[0].datasetIndex].label;
                         if (this.props.args.options.fixed_lines && this.props.args.options.fixed_lines.includes(t)) return;
                         this.setState({
                             activePoint: e[0]
                         }), this.togglePan(!1)
                     }
                 }, this.moveHandler = t => {
                     if (this.state.activePoint) {
                         const e = this.chartRef.current,
-                            n = yc(t, this.chartRef.current),
-                            i = e.chartArea,
-                            r = e.scales.y,
-                            s = this.map(n.y, i.bottom, i.top, r.min, r.max);
-                        e.data.datasets[this.state.activePoint.datasetIndex].data[this.state.activePoint.index] = s, e.update("none")
+                            n = ag(yc(t, this.chartRef.current), e.chartArea, e.scales.y),
+                            i = this.state.activePoint.index,
+                            r = this.state.chartData.labels[i];
+                        e.data.datasets[this.state.activePoint.datasetIndex].data[r] = n, e.update("none")
                     }
                 }, this.upHandler = t => {
                     if (this.state.activePoint) {
                         const t = this.chartRef.current,
                             e = this.state.activePoint.datasetIndex,
                             n = this.state.activePoint.index,
                             i = t.data.datasets[e].label,
                             r = this.state.chartData.labels[n],
-                            s = t.data.datasets[e].data[n];
+                            s = t.data.datasets[e].data[r];
                         this.state.originalData[i].data[r] = s, this.setState({
                             activePoint: null
                         }), this.togglePan(!0), ro.setComponentValue(this.state.originalData)
                     }
-                }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.state = {
+                }, this.chartRef = f.createRef(), this.state = {
                     activePoint: null,
                     originalData: t.args.data,
                     chartData: Zp(t.args.data, t.args.options.colors),
                     options: tg(t.args.options, t.theme)
                 }
             }
             componentDidUpdate(t) {
@@ -26289,26 +26310,26 @@
                     options: tg(this.props.args.options, this.props.theme)
                 })
             }
             togglePan(t) {
                 this.chartRef.current.options.plugins.zoom.pan.enabled = t, this.chartRef.current.update("none")
             }
             render() {
-                return (0, ag.jsx)(Qp, {
+                return (0, ug.jsx)(Qp, {
                     ref: this.chartRef,
                     data: this.state.chartData,
                     options: this.state.options,
                     onPointerDown: this.downHandler,
                     onPointerUp: this.upHandler,
                     onPointerMove: this.moveHandler
                 })
             }
         };
 
-        function cg(t, e) {
+        function dg(t, e) {
             return {
                 labels: e && e.x_labels ? e.x_labels : [],
                 datasets: Object.entries(t).map(((t, n) => {
                     let [i, r] = t;
                     const s = r.x.map(((t, e) => ({
                         x: t,
                         y: r.y[e]
@@ -26325,116 +26346,104 @@
                         pointRadius: r.point_radius,
                         borderDash: r.border_dash
                     }
                 }))
             }
         }
         Hh.register(...$f, Up);
-        const ug = class extends ao {
+        const fg = class extends ao {
                 constructor(t) {
                     super(t), this.downHandler = t => {
                         const e = $p(this.chartRef.current, t);
                         if (e.length > 0) {
                             const t = this.chartRef.current.data.datasets[e[0].datasetIndex].label;
                             if (this.props.args.options.fixed_lines && this.props.args.options.fixed_lines.includes(t)) return;
                             this.setState({
                                 activePoint: e[0]
                             }), this.togglePan(!1)
                         }
-                    }, this.calculateNewYValue = (t, e, n) => {
-                        if ("category" === this.props.args.options.y_type) {
-                            const i = n.getLabels();
-                            return i[Math.round(this.map(t.y, e.top, e.bottom, 0, i.length - 1))]
-                        }
-                        return this.map(t.y, e.bottom, e.top, n.min, n.max)
-                    }, this.calculateNewXValue = (t, e, n) => {
-                        if ("category" === this.props.args.options.x_type) {
-                            const i = n.getLabels();
-                            return i[Math.round(this.map(t.x, e.left, e.right, 0, i.length - 1))]
-                        }
-                        return this.map(t.x, e.left, e.right, n.min, n.max)
                     }, this.moveHandler = t => {
                         if (this.state.activePoint) {
                             const e = this.chartRef.current,
                                 n = yc(t, this.chartRef.current),
                                 i = e.chartArea,
-                                r = this.calculateNewYValue(n, i, e.scales.y),
-                                s = this.calculateNewXValue(n, i, e.scales.x);
+                                r = ag(n, i, e.scales.y, this.props.args.options.y_type),
+                                s = lg(n, i, e.scales.x, this.props.args.options.x_type);
                             e.data.datasets[this.state.activePoint.datasetIndex].data[this.state.activePoint.index].y = r, e.data.datasets[this.state.activePoint.datasetIndex].data[this.state.activePoint.index].x = s, e.update("none")
                         }
                     }, this.upHandler = t => {
                         if (this.state.activePoint) {
                             const t = this.chartRef.current,
                                 e = this.state.activePoint.datasetIndex,
                                 n = this.state.activePoint.index,
                                 i = t.data.datasets[e].label,
                                 r = t.data.datasets[e].data[n].x,
                                 s = t.data.datasets[e].data[n].y;
                             this.state.originalData[i].x[n] = r, this.state.originalData[i].y[n] = s, ro.setComponentValue(this.state.originalData), this.setState({
                                 activePoint: null
                             }), this.togglePan(!0)
                         }
-                    }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.state = {
+                    }, this.chartRef = f.createRef(), this.state = {
                         activePoint: null,
                         originalData: t.args.data,
-                        chartData: cg(t.args.data, t.args.options.colors),
+                        chartData: dg(t.args.data, t.args.options.colors),
                         options: tg(t.args.options, t.theme)
                     }
                 }
                 componentDidUpdate(t) {
                     ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                         originalData: this.props.args.data,
-                        chartData: cg(this.props.args.data, this.props.args.options),
+                        chartData: dg(this.props.args.data, this.props.args.options),
                         options: tg(this.props.args.options, this.props.theme)
                     })
                 }
                 togglePan(t) {
                     this.chartRef.current.options.plugins.zoom.pan.enabled = t, this.chartRef.current.update("none")
                 }
                 render() {
-                    return (0, ag.jsx)(Gp, {
+                    return (0, ug.jsx)(Gp, {
                         ref: this.chartRef,
                         data: this.state.chartData,
                         options: this.state.options,
                         onPointerDown: this.downHandler,
                         onPointerUp: this.upHandler,
                         onPointerMove: this.moveHandler
                     })
                 }
             },
             {
-                abs: hg,
-                cos: dg,
-                sin: fg,
-                acos: pg,
-                atan2: gg,
-                sqrt: mg,
-                pow: yg
+                abs: pg,
+                cos: gg,
+                sin: mg,
+                acos: yg,
+                atan2: bg,
+                sqrt: vg,
+                pow: xg
             } = Math;
 
-        function bg(t) {
-            return t < 0 ? -yg(-t, 1 / 3) : yg(t, 1 / 3)
+        function _g(t) {
+            return t < 0 ? -xg(-t, 1 / 3) : xg(t, 1 / 3)
         }
-        const vg = Math.PI,
-            xg = 2 * vg,
-            _g = vg / 2,
-            wg = Number.MAX_SAFE_INTEGER || 9007199254740991,
-            Sg = Number.MIN_SAFE_INTEGER || -9007199254740991,
-            Tg = {
+        const wg = Math.PI,
+            Sg = 2 * wg,
+            Tg = wg / 2,
+            kg = Number.MAX_SAFE_INTEGER || 9007199254740991,
+            Mg = Number.MIN_SAFE_INTEGER || -9007199254740991,
+            Ig = {
                 x: 0,
                 y: 0,
                 z: 0
             },
-            kg = {
+            Eg = {
                 Tvalues: [-.06405689286260563, .06405689286260563, -.1911188674736163, .1911188674736163, -.3150426796961634, .3150426796961634, -.4337935076260451, .4337935076260451, -.5454214713888396, .5454214713888396, -.6480936519369755, .6480936519369755, -.7401241915785544, .7401241915785544, -.820001985973903, .820001985973903, -.8864155270044011, .8864155270044011, -.9382745520027328, .9382745520027328, -.9747285559713095, .9747285559713095, -.9951872199970213, .9951872199970213],
                 Cvalues: [.12793819534675216, .12793819534675216, .1258374563468283, .1258374563468283, .12167047292780339, .12167047292780339, .1155056680537256, .1155056680537256, .10744427011596563, .10744427011596563, .09761865210411388, .09761865210411388, .08619016153195327, .08619016153195327, .0733464814110803, .0733464814110803, .05929858491543678, .05929858491543678, .04427743881741981, .04427743881741981, .028531388628933663, .028531388628933663, .0123412297999872, .0123412297999872],
                 arcfn: function(t, e) {
                     const n = e(t);
                     let i = n.x * n.x + n.y * n.y;
-                    return "undefined" !== typeof n.z && (i += n.z * n.z), mg(i)
+                    return "undefined" !== typeof n.z && (i += n.z * n.z), vg(i)
                 },
                 compute: function(t, e, n) {
                     if (0 === t) return e[0].t = 0, e[0];
                     const i = e.length - 1;
                     if (1 === t) return e[i].t = 1, e[i];
                     const r = 1 - t;
                     let s = e;
@@ -26447,15 +26456,15 @@
                         };
                         return n && (e.z = r * s[0].z + t * s[1].z), e
                     }
                     if (i < 4) {
                         let e, o, a, l = r * r,
                             c = t * t,
                             u = 0;
-                        2 === i ? (s = [s[0], s[1], s[2], Tg], e = l, o = r * t * 2, a = c) : 3 === i && (e = l * r, o = l * t * 3, a = r * c * 3, u = t * c);
+                        2 === i ? (s = [s[0], s[1], s[2], Ig], e = l, o = r * t * 2, a = c) : 3 === i && (e = l * r, o = l * t * 3, a = r * c * 3, u = t * c);
                         const h = {
                             x: e * s[0].x + o * s[1].x + a * s[2].x + u * s[3].x,
                             y: e * s[0].y + o * s[1].y + a * s[2].y + u * s[3].y,
                             t: t
                         };
                         return n && (h.z = e * s[0].z + o * s[1].z + a * s[2].z + u * s[3].z), h
                     }
@@ -26503,23 +26512,23 @@
                             y: s * (i[r + 1].y - i[r].y)
                         }, e && (n.z = s * (i[r + 1].z - i[r].z)), t.push(n);
                         n.push(t), i = t
                     }
                     return n
                 },
                 between: function(t, e, n) {
-                    return e <= t && t <= n || kg.approximately(t, e) || kg.approximately(t, n)
+                    return e <= t && t <= n || Eg.approximately(t, e) || Eg.approximately(t, n)
                 },
                 approximately: function(t, e, n) {
-                    return hg(t - e) <= (n || 1e-6)
+                    return pg(t - e) <= (n || 1e-6)
                 },
                 length: function(t) {
-                    const e = kg.Tvalues.length;
+                    const e = Eg.Tvalues.length;
                     let n = 0;
-                    for (let i, r = 0; r < e; r++) i = .5 * kg.Tvalues[r] + .5, n += kg.Cvalues[r] * kg.arcfn(i, t);
+                    for (let i, r = 0; r < e; r++) i = .5 * Eg.Tvalues[r] + .5, n += Eg.Cvalues[r] * Eg.arcfn(i, t);
                     return .5 * n
                 },
                 map: function(t, e, n, i, r) {
                     return i + (r - i) * ((t - e) / (n - e))
                 },
                 lerp: function(t, e, n) {
                     const i = {
@@ -26529,58 +26538,58 @@
                     return void 0 !== e.z && void 0 !== n.z && (i.z = e.z + t * (n.z - e.z)), i
                 },
                 pointToString: function(t) {
                     let e = t.x + "/" + t.y;
                     return "undefined" !== typeof t.z && (e += "/" + t.z), e
                 },
                 pointsToString: function(t) {
-                    return "[" + t.map(kg.pointToString).join(", ") + "]"
+                    return "[" + t.map(Eg.pointToString).join(", ") + "]"
                 },
                 copy: function(t) {
                     return JSON.parse(JSON.stringify(t))
                 },
                 angle: function(t, e, n) {
                     const i = e.x - t.x,
                         r = e.y - t.y,
                         s = n.x - t.x,
                         o = n.y - t.y;
-                    return gg(i * o - r * s, i * s + r * o)
+                    return bg(i * o - r * s, i * s + r * o)
                 },
                 round: function(t, e) {
                     const n = "" + t,
                         i = n.indexOf(".");
                     return parseFloat(n.substring(0, i + 1 + e))
                 },
                 dist: function(t, e) {
                     const n = t.x - e.x,
                         i = t.y - e.y;
-                    return mg(n * n + i * i)
+                    return vg(n * n + i * i)
                 },
                 closest: function(t, e) {
-                    let n, i, r = yg(2, 63);
+                    let n, i, r = xg(2, 63);
                     return t.forEach((function(t, s) {
-                        i = kg.dist(e, t), i < r && (r = i, n = s)
+                        i = Eg.dist(e, t), i < r && (r = i, n = s)
                     })), {
                         mdist: r,
                         mpos: n
                     }
                 },
                 abcratio: function(t, e) {
                     if (2 !== e && 3 !== e) return !1;
                     if ("undefined" === typeof t) t = .5;
                     else if (0 === t || 1 === t) return t;
-                    const n = yg(t, e) + yg(1 - t, e);
-                    return hg((n - 1) / n)
+                    const n = xg(t, e) + xg(1 - t, e);
+                    return pg((n - 1) / n)
                 },
                 projectionratio: function(t, e) {
                     if (2 !== e && 3 !== e) return !1;
                     if ("undefined" === typeof t) t = .5;
                     else if (0 === t || 1 === t) return t;
-                    const n = yg(1 - t, e);
-                    return n / (yg(t, e) + n)
+                    const n = xg(1 - t, e);
+                    return n / (xg(t, e) + n)
                 },
                 lli8: function(t, e, n, i, r, s, o, a) {
                     const l = (t - n) * (s - a) - (e - i) * (r - o);
                     return 0 != l && {
                         x: ((t * i - e * n) * (r - o) - (t - n) * (r * a - s * o)) / l,
                         y: ((t * i - e * n) * (s - a) - (e - i) * (r * a - s * o)) / l
                     }
@@ -26590,27 +26599,27 @@
                         s = t.y,
                         o = e.x,
                         a = e.y,
                         l = n.x,
                         c = n.y,
                         u = i.x,
                         h = i.y;
-                    return kg.lli8(r, s, o, a, l, c, u, h)
+                    return Eg.lli8(r, s, o, a, l, c, u, h)
                 },
                 lli: function(t, e) {
-                    return kg.lli4(t, t.c, e, e.c)
+                    return Eg.lli4(t, t.c, e, e.c)
                 },
                 makeline: function(t, e) {
-                    return new Lg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
+                    return new Bg(t.x, t.y, (t.x + e.x) / 2, (t.y + e.y) / 2, e.x, e.y)
                 },
                 findbbox: function(t) {
-                    let e = wg,
-                        n = wg,
-                        i = Sg,
-                        r = Sg;
+                    let e = kg,
+                        n = kg,
+                        i = Mg,
+                        r = Mg;
                     return t.forEach((function(t) {
                         const s = t.bbox();
                         e > s.x.min && (e = s.x.min), n > s.y.min && (n = s.y.min), i < s.x.max && (i = s.x.max), r < s.y.max && (r = s.y.max)
                     })), {
                         x: {
                             min: e,
                             mid: (e + i) / 2,
@@ -26622,66 +26631,66 @@
                             mid: (n + r) / 2,
                             max: r,
                             size: r - n
                         }
                     }
                 },
                 shapeintersections: function(t, e, n, i, r) {
-                    if (!kg.bboxoverlap(e, i)) return [];
+                    if (!Eg.bboxoverlap(e, i)) return [];
                     const s = [],
                         o = [t.startcap, t.forward, t.back, t.endcap],
                         a = [n.startcap, n.forward, n.back, n.endcap];
                     return o.forEach((function(e) {
                         e.virtual || a.forEach((function(i) {
                             if (i.virtual) return;
                             const o = e.intersects(i, r);
                             o.length > 0 && (o.c1 = e, o.c2 = i, o.s1 = t, o.s2 = n, s.push(o))
                         }))
                     })), s
                 },
                 makeshape: function(t, e, n) {
                     const i = e.points.length,
                         r = t.points.length,
-                        s = kg.makeline(e.points[i - 1], t.points[0]),
-                        o = kg.makeline(t.points[r - 1], e.points[0]),
+                        s = Eg.makeline(e.points[i - 1], t.points[0]),
+                        o = Eg.makeline(t.points[r - 1], e.points[0]),
                         a = {
                             startcap: s,
                             forward: t,
                             back: e,
                             endcap: o,
-                            bbox: kg.findbbox([s, t, e, o]),
+                            bbox: Eg.findbbox([s, t, e, o]),
                             intersections: function(t) {
-                                return kg.shapeintersections(a, a.bbox, t, t.bbox, n)
+                                return Eg.shapeintersections(a, a.bbox, t, t.bbox, n)
                             }
                         };
                     return a
                 },
                 getminmax: function(t, e, n) {
                     if (!n) return {
                         min: 0,
                         max: 0
                     };
-                    let i, r, s = wg,
-                        o = Sg; - 1 === n.indexOf(0) && (n = [0].concat(n)), -1 === n.indexOf(1) && n.push(1);
+                    let i, r, s = kg,
+                        o = Mg; - 1 === n.indexOf(0) && (n = [0].concat(n)), -1 === n.indexOf(1) && n.push(1);
                     for (let a = 0, l = n.length; a < l; a++) i = n[a], r = t.get(i), r[e] < s && (s = r[e]), r[e] > o && (o = r[e]);
                     return {
                         min: s,
                         mid: (s + o) / 2,
                         max: o,
                         size: o - s
                     }
                 },
                 align: function(t, e) {
                     const n = e.p1.x,
                         i = e.p1.y,
-                        r = -gg(e.p2.y - i, e.p2.x - n);
+                        r = -bg(e.p2.y - i, e.p2.x - n);
                     return t.map((function(t) {
                         return {
-                            x: (t.x - n) * dg(r) - (t.y - i) * fg(r),
-                            y: (t.x - n) * fg(r) + (t.y - i) * dg(r)
+                            x: (t.x - n) * gg(r) - (t.y - i) * mg(r),
+                            y: (t.x - n) * mg(r) + (t.y - i) * gg(r)
                         }
                     }))
                 },
                 roots: function(t, e) {
                     e = e || {
                         p1: {
                             x: 0,
@@ -26689,72 +26698,72 @@
                         },
                         p2: {
                             x: 1,
                             y: 0
                         }
                     };
                     const n = t.length - 1,
-                        i = kg.align(t, e),
+                        i = Eg.align(t, e),
                         r = function(t) {
                             return 0 <= t && t <= 1
                         };
                     if (2 === n) {
                         const t = i[0].y,
                             e = i[1].y,
                             n = i[2].y,
                             s = t - 2 * e + n;
                         if (0 !== s) {
-                            const i = -mg(e * e - t * n),
+                            const i = -vg(e * e - t * n),
                                 o = -t + e;
                             return [-(i + o) / s, -(-i + o) / s].filter(r)
                         }
                         return e !== n && 0 === s ? [(2 * e - n) / (2 * e - 2 * n)].filter(r) : []
                     }
                     const s = i[0].y,
                         o = i[1].y,
                         a = i[2].y;
                     let l = 3 * o - s - 3 * a + i[3].y,
                         c = 3 * s - 6 * o + 3 * a,
                         u = -3 * s + 3 * o,
                         h = s;
-                    if (kg.approximately(l, 0)) {
-                        if (kg.approximately(c, 0)) return kg.approximately(u, 0) ? [] : [-h / u].filter(r);
-                        const t = mg(u * u - 4 * c * h),
+                    if (Eg.approximately(l, 0)) {
+                        if (Eg.approximately(c, 0)) return Eg.approximately(u, 0) ? [] : [-h / u].filter(r);
+                        const t = vg(u * u - 4 * c * h),
                             e = 2 * c;
                         return [(t - u) / e, (-u - t) / e].filter(r)
                     }
                     c /= l, u /= l, h /= l;
                     const d = (3 * u - c * c) / 3,
                         f = d / 3,
                         p = (2 * c * c * c - 9 * c * u + 27 * h) / 27,
                         g = p / 2,
                         m = g * g + f * f * f;
                     let y, b, v, x, _;
                     if (m < 0) {
                         const t = -d / 3,
-                            e = mg(t * t * t),
+                            e = vg(t * t * t),
                             n = -p / (2 * e),
-                            i = pg(n < -1 ? -1 : n > 1 ? 1 : n),
-                            s = 2 * bg(e);
-                        return v = s * dg(i / 3) - c / 3, x = s * dg((i + xg) / 3) - c / 3, _ = s * dg((i + 2 * xg) / 3) - c / 3, [v, x, _].filter(r)
+                            i = yg(n < -1 ? -1 : n > 1 ? 1 : n),
+                            s = 2 * _g(e);
+                        return v = s * gg(i / 3) - c / 3, x = s * gg((i + Sg) / 3) - c / 3, _ = s * gg((i + 2 * Sg) / 3) - c / 3, [v, x, _].filter(r)
                     }
-                    if (0 === m) return y = g < 0 ? bg(-g) : -bg(g), v = 2 * y - c / 3, x = -y - c / 3, [v, x].filter(r);
+                    if (0 === m) return y = g < 0 ? _g(-g) : -_g(g), v = 2 * y - c / 3, x = -y - c / 3, [v, x].filter(r);
                     {
-                        const t = mg(m);
-                        return y = bg(-g + t), b = bg(g + t), [y - b - c / 3].filter(r)
+                        const t = vg(m);
+                        return y = _g(-g + t), b = _g(g + t), [y - b - c / 3].filter(r)
                     }
                 },
                 droots: function(t) {
                     if (3 === t.length) {
                         const e = t[0],
                             n = t[1],
                             i = t[2],
                             r = e - 2 * n + i;
                         if (0 !== r) {
-                            const t = -mg(n * n - e * i),
+                            const t = -vg(n * n - e * i),
                                 s = -e + n;
                             return [-(t + s) / r, -(-t + s) / r]
                         }
                         return n !== i && 0 === r ? [(2 * n - i) / (2 * (n - i))] : []
                     }
                     if (2 === t.length) {
                         const e = t[0],
@@ -26762,66 +26771,66 @@
                         return e !== n ? [e / (e - n)] : []
                     }
                     return []
                 },
                 curvature: function(t, e, n, i, r) {
                     let s, o, a, l, c = 0,
                         u = 0;
-                    const h = kg.compute(t, e),
-                        d = kg.compute(t, n),
+                    const h = Eg.compute(t, e),
+                        d = Eg.compute(t, n),
                         f = h.x * h.x + h.y * h.y;
-                    if (i ? (s = mg(yg(h.y * d.z - d.y * h.z, 2) + yg(h.z * d.x - d.z * h.x, 2) + yg(h.x * d.y - d.x * h.y, 2)), o = yg(f + h.z * h.z, 1.5)) : (s = h.x * d.y - h.y * d.x, o = yg(f, 1.5)), 0 === s || 0 === o) return {
+                    if (i ? (s = vg(xg(h.y * d.z - d.y * h.z, 2) + xg(h.z * d.x - d.z * h.x, 2) + xg(h.x * d.y - d.x * h.y, 2)), o = xg(f + h.z * h.z, 1.5)) : (s = h.x * d.y - h.y * d.x, o = xg(f, 1.5)), 0 === s || 0 === o) return {
                         k: 0,
                         r: 0
                     };
                     if (c = s / o, u = o / s, !r) {
-                        const r = kg.curvature(t - .001, e, n, i, !0).k,
-                            s = kg.curvature(t + .001, e, n, i, !0).k;
-                        l = (s - c + (c - r)) / 2, a = (hg(s - c) + hg(c - r)) / 2
+                        const r = Eg.curvature(t - .001, e, n, i, !0).k,
+                            s = Eg.curvature(t + .001, e, n, i, !0).k;
+                        l = (s - c + (c - r)) / 2, a = (pg(s - c) + pg(c - r)) / 2
                     }
                     return {
                         k: c,
                         r: u,
                         dk: l,
                         adk: a
                     }
                 },
                 inflections: function(t) {
                     if (t.length < 4) return [];
-                    const e = kg.align(t, {
+                    const e = Eg.align(t, {
                             p1: t[0],
                             p2: t.slice(-1)[0]
                         }),
                         n = e[2].x * e[1].y,
                         i = e[3].x * e[1].y,
                         r = e[1].x * e[2].y,
                         s = 18 * (-3 * n + 2 * i + 3 * r - e[3].x * e[2].y),
                         o = 18 * (3 * n - i - 3 * r),
                         a = 18 * (r - n);
-                    if (kg.approximately(s, 0)) {
-                        if (!kg.approximately(o, 0)) {
+                    if (Eg.approximately(s, 0)) {
+                        if (!Eg.approximately(o, 0)) {
                             let t = -a / o;
                             if (0 <= t && t <= 1) return [t]
                         }
                         return []
                     }
                     const l = 2 * s;
-                    if (kg.approximately(l, 0)) return [];
+                    if (Eg.approximately(l, 0)) return [];
                     const c = o * o - 4 * s * a;
                     if (c < 0) return [];
                     const u = Math.sqrt(c);
                     return [(u - o) / l, -(o + u) / l].filter((function(t) {
                         return 0 <= t && t <= 1
                     }))
                 },
                 bboxoverlap: function(t, e) {
                     const n = ["x", "y"],
                         i = n.length;
                     for (let r, s, o, a, l = 0; l < i; l++)
-                        if (r = n[l], s = t[r].mid, o = e[r].mid, a = (t[r].size + e[r].size) / 2, hg(s - o) >= a) return !1;
+                        if (r = n[l], s = t[r].mid, o = e[r].mid, a = (t[r].size + e[r].size) / 2, pg(s - o) >= a) return !1;
                     return !0
                 },
                 expandbox: function(t, e) {
                     e.x.min < t.x.min && (t.x.min = e.x.min), e.y.min < t.y.min && (t.y.min = e.y.min), e.z && e.z.min < t.z.min && (t.z.min = e.z.min), e.x.max > t.x.max && (t.x.max = e.x.max), e.y.max > t.y.max && (t.y.max = e.y.max), e.z && e.z.max > t.z.max && (t.z.max = e.z.max), t.x.mid = (t.x.min + t.x.max) / 2, t.y.mid = (t.y.min + t.y.max) / 2, t.z && (t.z.mid = (t.z.min + t.z.max) / 2), t.x.size = t.x.max - t.x.min, t.y.size = t.y.max - t.y.min, t.z && (t.z.size = t.z.max - t.z.min)
                 },
                 pairiteration: function(t, e, n) {
                     const i = t.bbox(),
@@ -26841,61 +26850,61 @@
                             left: a.right,
                             right: l.right
                         }, {
                             left: a.right,
                             right: l.left
                         }];
                     c = c.filter((function(t) {
-                        return kg.bboxoverlap(t.left.bbox(), t.right.bbox())
+                        return Eg.bboxoverlap(t.left.bbox(), t.right.bbox())
                     }));
                     let u = [];
                     return 0 === c.length || (c.forEach((function(t) {
-                        u = u.concat(kg.pairiteration(t.left, t.right, o))
+                        u = u.concat(Eg.pairiteration(t.left, t.right, o))
                     })), u = u.filter((function(t, e) {
                         return u.indexOf(t) === e
                     }))), u
                 },
                 getccenter: function(t, e, n) {
                     const i = e.x - t.x,
                         r = e.y - t.y,
                         s = n.x - e.x,
                         o = n.y - e.y,
-                        a = i * dg(_g) - r * fg(_g),
-                        l = i * fg(_g) + r * dg(_g),
-                        c = s * dg(_g) - o * fg(_g),
-                        u = s * fg(_g) + o * dg(_g),
+                        a = i * gg(Tg) - r * mg(Tg),
+                        l = i * mg(Tg) + r * gg(Tg),
+                        c = s * gg(Tg) - o * mg(Tg),
+                        u = s * mg(Tg) + o * gg(Tg),
                         h = (t.x + e.x) / 2,
                         d = (t.y + e.y) / 2,
                         f = (e.x + n.x) / 2,
                         p = (e.y + n.y) / 2,
                         g = h + a,
                         m = d + l,
                         y = f + c,
                         b = p + u,
-                        v = kg.lli8(h, d, g, m, f, p, y, b),
-                        x = kg.dist(v, t);
-                    let _, w = gg(t.y - v.y, t.x - v.x),
-                        S = gg(e.y - v.y, e.x - v.x),
-                        T = gg(n.y - v.y, n.x - v.x);
-                    return w < T ? ((w > S || S > T) && (w += xg), w > T && (_ = T, T = w, w = _)) : T < S && S < w ? (_ = T, T = w, w = _) : T += xg, v.s = w, v.e = T, v.r = x, v
+                        v = Eg.lli8(h, d, g, m, f, p, y, b),
+                        x = Eg.dist(v, t);
+                    let _, w = bg(t.y - v.y, t.x - v.x),
+                        S = bg(e.y - v.y, e.x - v.x),
+                        T = bg(n.y - v.y, n.x - v.x);
+                    return w < T ? ((w > S || S > T) && (w += Sg), w > T && (_ = T, T = w, w = _)) : T < S && S < w ? (_ = T, T = w, w = _) : T += Sg, v.s = w, v.e = T, v.r = x, v
                 },
                 numberSort: function(t, e) {
                     return t - e
                 }
             };
-        class Mg {
+        class Dg {
             constructor(t) {
                 this.curves = [], this._3d = !1, t && (this.curves = t, this._3d = this.curves[0]._3d)
             }
             valueOf() {
                 return this.toString()
             }
             toString() {
                 return "[" + this.curves.map((function(t) {
-                    return kg.pointsToString(t.points)
+                    return Eg.pointsToString(t.points)
                 })).join(", ") + "]"
             }
             addCurve(t) {
                 this.curves.push(t), this._3d = this._3d || t._3d
             }
             length() {
                 return this.curves.map((function(t) {
@@ -26905,34 +26914,34 @@
                 }))
             }
             curve(t) {
                 return this.curves[t]
             }
             bbox() {
                 const t = this.curves;
-                for (var e = t[0].bbox(), n = 1; n < t.length; n++) kg.expandbox(e, t[n].bbox());
+                for (var e = t[0].bbox(), n = 1; n < t.length; n++) Eg.expandbox(e, t[n].bbox());
                 return e
             }
             offset(t) {
                 const e = [];
                 return this.curves.forEach((function(n) {
                     e.push(...n.offset(t))
-                })), new Mg(e)
+                })), new Dg(e)
             }
         }
         const {
-            abs: Ig,
-            min: Eg,
-            max: Dg,
-            cos: Og,
-            sin: Cg,
-            acos: Ag,
-            sqrt: Pg
-        } = Math, Fg = Math.PI;
-        class Lg {
+            abs: Og,
+            min: Cg,
+            max: Ag,
+            cos: Pg,
+            sin: Fg,
+            acos: Lg,
+            sqrt: zg
+        } = Math, Ng = Math.PI;
+        class Bg {
             constructor(t) {
                 let e = t && t.forEach ? t : Array.from(arguments).slice(),
                     n = !1;
                 if ("object" === typeof e[0]) {
                     n = e.length;
                     const t = [];
                     e.forEach((function(e) {
@@ -26957,33 +26966,33 @@
                         y: e[d + 1]
                     };
                     s && (a.z = e[d + 2]), o.push(a)
                 }
                 const l = this.order = o.length - 1,
                     c = this.dims = ["x", "y"];
                 s && c.push("z"), this.dimlen = c.length;
-                const u = kg.align(o, {
+                const u = Eg.align(o, {
                         p1: o[0],
                         p2: o[l]
                     }),
-                    h = kg.dist(o[0], o[l]);
-                this._linear = u.reduce(((t, e) => t + Ig(e.y)), 0) < h / 50, this._lut = [], this._t1 = 0, this._t2 = 1, this.update()
+                    h = Eg.dist(o[0], o[l]);
+                this._linear = u.reduce(((t, e) => t + Og(e.y)), 0) < h / 50, this._lut = [], this._t1 = 0, this._t2 = 1, this.update()
             }
             static quadraticFromPoints(t, e, n, i) {
-                if ("undefined" === typeof i && (i = .5), 0 === i) return new Lg(e, e, n);
-                if (1 === i) return new Lg(t, e, e);
-                const r = Lg.getABC(2, t, e, n, i);
-                return new Lg(t, r.A, n)
+                if ("undefined" === typeof i && (i = .5), 0 === i) return new Bg(e, e, n);
+                if (1 === i) return new Bg(t, e, e);
+                const r = Bg.getABC(2, t, e, n, i);
+                return new Bg(t, r.A, n)
             }
             static cubicFromPoints(t, e, n, i, r) {
                 "undefined" === typeof i && (i = .5);
-                const s = Lg.getABC(3, t, e, n, i);
-                "undefined" === typeof r && (r = kg.dist(e, s.C));
+                const s = Bg.getABC(3, t, e, n, i);
+                "undefined" === typeof r && (r = Eg.dist(e, s.C));
                 const o = r * (1 - i) / i,
-                    a = kg.dist(t, n),
+                    a = Eg.dist(t, n),
                     l = (n.x - t.x) / a,
                     c = (n.y - t.y) / a,
                     u = r * l,
                     h = r * c,
                     d = o * l,
                     f = o * c,
                     p = e.x - u,
@@ -26999,30 +27008,30 @@
                         x: t.x + (v - t.x) / i,
                         y: t.y + (x - t.y) / i
                     },
                     T = {
                         x: n.x + (_ - n.x) / (1 - i),
                         y: n.y + (w - n.y) / (1 - i)
                     };
-                return new Lg(t, S, T, n)
+                return new Bg(t, S, T, n)
             }
             static getUtils() {
-                return kg
+                return Eg
             }
             getUtils() {
-                return Lg.getUtils()
+                return Bg.getUtils()
             }
             static get PolyBezier() {
-                return Mg
+                return Dg
             }
             valueOf() {
                 return this.toString()
             }
             toString() {
-                return kg.pointsToString(this.points)
+                return Eg.pointsToString(this.points)
             }
             toSVG() {
                 if (this._3d) return !1;
                 const t = this.points,
                     e = ["M", t[0].x, t[0].y, 2 === this.order ? "Q" : "C"];
                 for (let n = 1, i = t.length; n < i; n++) e.push(t[n].x), e.push(t[n].y);
                 return e.join(" ")
@@ -27037,37 +27046,37 @@
             }
             coordDigest() {
                 return this.points.map((function(t, e) {
                     return "" + e + t.x + t.y + (t.z ? t.z : 0)
                 })).join("")
             }
             update() {
-                this._lut = [], this.dpoints = kg.derive(this.points, this._3d), this.computedirection()
+                this._lut = [], this.dpoints = Eg.derive(this.points, this._3d), this.computedirection()
             }
             computedirection() {
                 const t = this.points,
-                    e = kg.angle(t[0], t[this.order], t[1]);
+                    e = Eg.angle(t[0], t[this.order], t[1]);
                 this.clockwise = e > 0
             }
             length() {
-                return kg.length(this.derivative.bind(this))
+                return Eg.length(this.derivative.bind(this))
             }
             static getABC() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 2,
                     e = arguments.length > 1 ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0,
                     i = arguments.length > 3 ? arguments[3] : void 0,
                     r = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : .5;
-                const s = kg.projectionratio(r, t),
+                const s = Eg.projectionratio(r, t),
                     o = 1 - s,
                     a = {
                         x: s * e.x + o * i.x,
                         y: s * e.y + o * i.y
                     },
-                    l = kg.abcratio(r, t);
+                    l = Eg.abcratio(r, t);
                 return {
                     A: {
                         x: n.x + (n.x - a.x) / l,
                         y: n.y + (n.y - a.y) / l
                     },
                     B: n,
                     C: a,
@@ -27075,106 +27084,106 @@
                     E: i
                 }
             }
             getABC(t, e) {
                 e = e || this.get(t);
                 let n = this.points[0],
                     i = this.points[this.order];
-                return Lg.getABC(this.order, n, e, i, t)
+                return Bg.getABC(this.order, n, e, i, t)
             }
             getLUT(t) {
                 if (this.verify(), t = t || 100, this._lut.length === t + 1) return this._lut;
                 this._lut = [], t++, this._lut = [];
                 for (let e, n, i = 0; i < t; i++) n = i / (t - 1), e = this.compute(n), e.t = n, this._lut.push(e);
                 return this._lut
             }
             on(e, n) {
                 n = n || 5;
                 const i = this.getLUT(),
                     r = [];
-                for (let t, s = 0, o = 0; s < i.length; s++) t = i[s], kg.dist(t, e) < n && (r.push(t), o += s / i.length);
+                for (let t, s = 0, o = 0; s < i.length; s++) t = i[s], Eg.dist(t, e) < n && (r.push(t), o += s / i.length);
                 return !!r.length && (t /= r.length)
             }
             project(t) {
                 const e = this.getLUT(),
                     n = e.length - 1,
-                    i = kg.closest(e, t),
+                    i = Eg.closest(e, t),
                     r = i.mpos,
                     s = (r - 1) / n,
                     o = (r + 1) / n,
                     a = .1 / n;
                 let l, c = i.mdist,
                     u = s,
                     h = u;
                 c += 1;
-                for (let d; u < o + a; u += a) l = this.compute(u), d = kg.dist(t, l), d < c && (c = d, h = u);
+                for (let d; u < o + a; u += a) l = this.compute(u), d = Eg.dist(t, l), d < c && (c = d, h = u);
                 return h = h < 0 ? 0 : h > 1 ? 1 : h, l = this.compute(h), l.t = h, l.d = c, l
             }
             get(t) {
                 return this.compute(t)
             }
             point(t) {
                 return this.points[t]
             }
             compute(t) {
-                return this.ratios ? kg.computeWithRatios(t, this.points, this.ratios, this._3d) : kg.compute(t, this.points, this._3d, this.ratios)
+                return this.ratios ? Eg.computeWithRatios(t, this.points, this.ratios, this._3d) : Eg.compute(t, this.points, this._3d, this.ratios)
             }
             raise() {
                 const t = this.points,
                     e = [t[0]],
                     n = t.length;
                 for (let i, r, s = 1; s < n; s++) i = t[s], r = t[s - 1], e[s] = {
                     x: (n - s) / n * i.x + s / n * r.x,
                     y: (n - s) / n * i.y + s / n * r.y
                 };
-                return e[n] = t[n - 1], new Lg(e)
+                return e[n] = t[n - 1], new Bg(e)
             }
             derivative(t) {
-                return kg.compute(t, this.dpoints[0], this._3d)
+                return Eg.compute(t, this.dpoints[0], this._3d)
             }
             dderivative(t) {
-                return kg.compute(t, this.dpoints[1], this._3d)
+                return Eg.compute(t, this.dpoints[1], this._3d)
             }
             align() {
                 let t = this.points;
-                return new Lg(kg.align(t, {
+                return new Bg(Eg.align(t, {
                     p1: t[0],
                     p2: t[t.length - 1]
                 }))
             }
             curvature(t) {
-                return kg.curvature(t, this.dpoints[0], this.dpoints[1], this._3d)
+                return Eg.curvature(t, this.dpoints[0], this.dpoints[1], this._3d)
             }
             inflections() {
-                return kg.inflections(this.points)
+                return Eg.inflections(this.points)
             }
             normal(t) {
                 return this._3d ? this.__normal3(t) : this.__normal2(t)
             }
             __normal2(t) {
                 const e = this.derivative(t),
-                    n = Pg(e.x * e.x + e.y * e.y);
+                    n = zg(e.x * e.x + e.y * e.y);
                 return {
                     t: t,
                     x: -e.y / n,
                     y: e.x / n
                 }
             }
             __normal3(t) {
                 const e = this.derivative(t),
                     n = this.derivative(t + .01),
-                    i = Pg(e.x * e.x + e.y * e.y + e.z * e.z),
-                    r = Pg(n.x * n.x + n.y * n.y + n.z * n.z);
+                    i = zg(e.x * e.x + e.y * e.y + e.z * e.z),
+                    r = zg(n.x * n.x + n.y * n.y + n.z * n.z);
                 e.x /= i, e.y /= i, e.z /= i, n.x /= r, n.y /= r, n.z /= r;
                 const s = {
                         x: n.y * e.z - n.z * e.y,
                         y: n.z * e.x - n.x * e.z,
                         z: n.x * e.y - n.y * e.x
                     },
-                    o = Pg(s.x * s.x + s.y * s.y + s.z * s.z);
+                    o = zg(s.x * s.x + s.y * s.y + s.z * s.z);
                 s.x /= o, s.y /= o, s.z /= o;
                 const a = [s.x * s.x, s.x * s.y - s.z, s.x * s.z + s.y, s.x * s.y + s.z, s.y * s.y, s.y * s.z - s.x, s.x * s.z - s.y, s.y * s.z + s.x, s.z * s.z];
                 return {
                     t: t,
                     x: a[0] * e.x + a[1] * e.y + a[2] * e.z,
                     y: a[3] * e.x + a[4] * e.y + a[5] * e.z,
                     z: a[6] * e.x + a[7] * e.y + a[8] * e.z
@@ -27183,56 +27192,56 @@
             hull(t) {
                 let e = this.points,
                     n = [],
                     i = [],
                     r = 0;
                 for (i[r++] = e[0], i[r++] = e[1], i[r++] = e[2], 3 === this.order && (i[r++] = e[3]); e.length > 1;) {
                     n = [];
-                    for (let s, o = 0, a = e.length - 1; o < a; o++) s = kg.lerp(t, e[o], e[o + 1]), i[r++] = s, n.push(s);
+                    for (let s, o = 0, a = e.length - 1; o < a; o++) s = Eg.lerp(t, e[o], e[o + 1]), i[r++] = s, n.push(s);
                     e = n
                 }
                 return i
             }
             split(t, e) {
                 if (0 === t && e) return this.split(e).left;
                 if (1 === e) return this.split(t).right;
                 const n = this.hull(t),
                     i = {
-                        left: 2 === this.order ? new Lg([n[0], n[3], n[5]]) : new Lg([n[0], n[4], n[7], n[9]]),
-                        right: 2 === this.order ? new Lg([n[5], n[4], n[2]]) : new Lg([n[9], n[8], n[6], n[3]]),
+                        left: 2 === this.order ? new Bg([n[0], n[3], n[5]]) : new Bg([n[0], n[4], n[7], n[9]]),
+                        right: 2 === this.order ? new Bg([n[5], n[4], n[2]]) : new Bg([n[9], n[8], n[6], n[3]]),
                         span: n
                     };
-                return i.left._t1 = kg.map(0, 0, 1, this._t1, this._t2), i.left._t2 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t1 = kg.map(t, 0, 1, this._t1, this._t2), i.right._t2 = kg.map(1, 0, 1, this._t1, this._t2), e ? (e = kg.map(e, t, 1, 0, 1), i.right.split(e).left) : i
+                return i.left._t1 = Eg.map(0, 0, 1, this._t1, this._t2), i.left._t2 = Eg.map(t, 0, 1, this._t1, this._t2), i.right._t1 = Eg.map(t, 0, 1, this._t1, this._t2), i.right._t2 = Eg.map(1, 0, 1, this._t1, this._t2), e ? (e = Eg.map(e, t, 1, 0, 1), i.right.split(e).left) : i
             }
             extrema() {
                 const t = {};
                 let e = [];
                 return this.dims.forEach(function(n) {
                     let i = function(t) {
                             return t[n]
                         },
                         r = this.dpoints[0].map(i);
-                    t[n] = kg.droots(r), 3 === this.order && (r = this.dpoints[1].map(i), t[n] = t[n].concat(kg.droots(r))), t[n] = t[n].filter((function(t) {
+                    t[n] = Eg.droots(r), 3 === this.order && (r = this.dpoints[1].map(i), t[n] = t[n].concat(Eg.droots(r))), t[n] = t[n].filter((function(t) {
                         return t >= 0 && t <= 1
-                    })), e = e.concat(t[n].sort(kg.numberSort))
-                }.bind(this)), t.values = e.sort(kg.numberSort).filter((function(t, n) {
+                    })), e = e.concat(t[n].sort(Eg.numberSort))
+                }.bind(this)), t.values = e.sort(Eg.numberSort).filter((function(t, n) {
                     return e.indexOf(t) === n
                 })), t
             }
             bbox() {
                 const t = this.extrema(),
                     e = {};
                 return this.dims.forEach(function(n) {
-                    e[n] = kg.getminmax(this, n, t[n])
+                    e[n] = Eg.getminmax(this, n, t[n])
                 }.bind(this)), e
             }
             overlaps(t) {
                 const e = this.bbox(),
                     n = t.bbox();
-                return kg.bboxoverlap(e, n)
+                return Eg.bboxoverlap(e, n)
             }
             offset(t, e) {
                 if ("undefined" !== typeof e) {
                     const n = this.get(t),
                         i = this.normal(t),
                         r = {
                             c: n,
@@ -27247,54 +27256,54 @@
                         n = this.points.map((function(n) {
                             const i = {
                                 x: n.x + t * e.x,
                                 y: n.y + t * e.y
                             };
                             return n.z && e.z && (i.z = n.z + t * e.z), i
                         }));
-                    return [new Lg(n)]
+                    return [new Bg(n)]
                 }
                 return this.reduce().map((function(e) {
                     return e._linear ? e.offset(t)[0] : e.scale(t)
                 }))
             }
             simple() {
                 if (3 === this.order) {
-                    const t = kg.angle(this.points[0], this.points[3], this.points[1]),
-                        e = kg.angle(this.points[0], this.points[3], this.points[2]);
+                    const t = Eg.angle(this.points[0], this.points[3], this.points[1]),
+                        e = Eg.angle(this.points[0], this.points[3], this.points[2]);
                     if (t > 0 && e < 0 || t < 0 && e > 0) return !1
                 }
                 const t = this.normal(0),
                     e = this.normal(1);
                 let n = t.x * e.x + t.y * e.y;
-                return this._3d && (n += t.z * e.z), Ig(Ag(n)) < Fg / 3
+                return this._3d && (n += t.z * e.z), Og(Lg(n)) < Ng / 3
             }
             reduce() {
                 let t, e, n = 0,
                     i = 0,
                     r = .01,
                     s = [],
                     o = [],
                     a = this.extrema().values;
                 for (-1 === a.indexOf(0) && (a = [0].concat(a)), -1 === a.indexOf(1) && a.push(1), n = a[0], t = 1; t < a.length; t++) i = a[t], e = this.split(n, i), e._t1 = n, e._t2 = i, s.push(e), n = i;
                 return s.forEach((function(t) {
                     for (n = 0, i = 0; i <= 1;)
                         for (i = n + r; i <= 1.01; i += r)
                             if (e = t.split(n, i), !e.simple()) {
-                                if (i -= r, Ig(n - i) < r) return [];
-                                e = t.split(n, i), e._t1 = kg.map(n, 0, 1, t._t1, t._t2), e._t2 = kg.map(i, 0, 1, t._t1, t._t2), o.push(e), n = i;
+                                if (i -= r, Og(n - i) < r) return [];
+                                e = t.split(n, i), e._t1 = Eg.map(n, 0, 1, t._t1, t._t2), e._t2 = Eg.map(i, 0, 1, t._t1, t._t2), o.push(e), n = i;
                                 break
-                            } n < 1 && (e = t.split(n, 1), e._t1 = kg.map(n, 0, 1, t._t1, t._t2), e._t2 = t._t2, o.push(e))
+                            } n < 1 && (e = t.split(n, 1), e._t1 = Eg.map(n, 0, 1, t._t1, t._t2), e._t2 = t._t2, o.push(e))
                 })), o
             }
             translate(t, e, n) {
                 n = "number" === typeof n ? n : e;
                 const i = this.order;
                 let r = this.points.map(((t, r) => (1 - r / i) * e + r / i * n));
-                return new Lg(this.points.map(((e, n) => ({
+                return new Bg(this.points.map(((e, n) => ({
                     x: e.x + t.x * r[n],
                     y: e.y + t.y * r[n]
                 }))))
             }
             scale(t) {
                 const e = this.order;
                 let n = !1;
@@ -27302,44 +27311,44 @@
                 const i = this.clockwise,
                     r = this.points;
                 if (this._linear) return this.translate(this.normal(0), n ? n(0) : t, n ? n(1) : t);
                 const s = n ? n(0) : t,
                     o = n ? n(1) : t,
                     a = [this.offset(0, 10), this.offset(1, 10)],
                     l = [],
-                    c = kg.lli4(a[0], a[0].c, a[1], a[1].c);
+                    c = Eg.lli4(a[0], a[0].c, a[1], a[1].c);
                 if (!c) throw new Error("cannot scale this curve. Try reducing it first.");
                 return [0, 1].forEach((function(t) {
-                    const n = l[t * e] = kg.copy(r[t * e]);
+                    const n = l[t * e] = Eg.copy(r[t * e]);
                     n.x += (t ? o : s) * a[t].n.x, n.y += (t ? o : s) * a[t].n.y
                 })), n ? ([0, 1].forEach((function(s) {
                     if (2 !== e || !s) {
                         var o = r[s + 1],
                             a = {
                                 x: o.x - c.x,
                                 y: o.y - c.y
                             },
                             u = n ? n((s + 1) / e) : t;
                         n && !i && (u = -u);
-                        var h = Pg(a.x * a.x + a.y * a.y);
+                        var h = zg(a.x * a.x + a.y * a.y);
                         a.x /= h, a.y /= h, l[s + 1] = {
                             x: o.x + u * a.x,
                             y: o.y + u * a.y
                         }
                     }
-                })), new Lg(l)) : ([0, 1].forEach((t => {
+                })), new Bg(l)) : ([0, 1].forEach((t => {
                     if (2 === e && t) return;
                     const n = l[t * e],
                         i = this.derivative(t),
                         s = {
                             x: n.x + i.x,
                             y: n.y + i.y
                         };
-                    l[t + 1] = kg.lli4(n, s, c, r[t + 1])
-                })), new Lg(l))
+                    l[t + 1] = Eg.lli4(n, s, c, r[t + 1])
+                })), new Bg(l))
             }
             outline(t, e, n, i) {
                 if (e = void 0 === e ? t : e, this._linear) {
                     const r = this.normal(0),
                         s = this.points[0],
                         o = this.points[this.points.length - 1];
                     let a, l, c;
@@ -27361,71 +27370,71 @@
                         x: o.x - r.x * i,
                         y: o.y - r.y * i
                     }, l = {
                         x: (a.x + c.x) / 2,
                         y: (a.y + c.y) / 2
                     };
                     const h = [c, l, a],
-                        d = kg.makeline(h[2], u[0]),
-                        f = kg.makeline(u[2], h[0]),
-                        p = [d, new Lg(u), f, new Lg(h)];
-                    return new Mg(p)
+                        d = Eg.makeline(h[2], u[0]),
+                        f = Eg.makeline(u[2], h[0]),
+                        p = [d, new Bg(u), f, new Bg(h)];
+                    return new Dg(p)
                 }
                 const r = this.reduce(),
                     s = r.length,
                     o = [];
                 let a, l = [],
                     c = 0,
                     u = this.length();
                 const h = "undefined" !== typeof n && "undefined" !== typeof i;
 
                 function d(t, e, n, i, r) {
                     return function(s) {
                         const o = i / n,
                             a = (i + r) / n,
                             l = e - t;
-                        return kg.map(s, 0, 1, t + o * l, t + a * l)
+                        return Eg.map(s, 0, 1, t + o * l, t + a * l)
                     }
                 }
                 r.forEach((function(r) {
                     const s = r.length();
                     h ? (o.push(r.scale(d(t, n, u, c, s))), l.push(r.scale(d(-e, -i, u, c, s)))) : (o.push(r.scale(t)), l.push(r.scale(-e))), c += s
                 })), l = l.map((function(t) {
                     return a = t.points, a[3] ? t.points = [a[3], a[2], a[1], a[0]] : t.points = [a[2], a[1], a[0]], t
                 })).reverse();
                 const f = o[0].points[0],
                     p = o[s - 1].points[o[s - 1].points.length - 1],
                     g = l[s - 1].points[l[s - 1].points.length - 1],
                     m = l[0].points[0],
-                    y = kg.makeline(g, f),
-                    b = kg.makeline(p, m),
+                    y = Eg.makeline(g, f),
+                    b = Eg.makeline(p, m),
                     v = [y].concat(o).concat([b]).concat(l);
-                return new Mg(v)
+                return new Dg(v)
             }
             outlineshapes(t, e, n) {
                 e = e || t;
                 const i = this.outline(t, e).curves,
                     r = [];
                 for (let s = 1, o = i.length; s < o / 2; s++) {
-                    const t = kg.makeshape(i[s], i[o - s], n);
+                    const t = Eg.makeshape(i[s], i[o - s], n);
                     t.startcap.virtual = s > 1, t.endcap.virtual = s < o / 2 - 1, r.push(t)
                 }
                 return r
             }
             intersects(t, e) {
-                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof Lg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
+                return t ? t.p1 && t.p2 ? this.lineIntersects(t) : (t instanceof Bg && (t = t.reduce()), this.curveintersects(this.reduce(), t, e)) : this.selfintersects(e)
             }
             lineIntersects(t) {
-                const e = Eg(t.p1.x, t.p2.x),
-                    n = Eg(t.p1.y, t.p2.y),
-                    i = Dg(t.p1.x, t.p2.x),
-                    r = Dg(t.p1.y, t.p2.y);
-                return kg.roots(this.points, t).filter((t => {
+                const e = Cg(t.p1.x, t.p2.x),
+                    n = Cg(t.p1.y, t.p2.y),
+                    i = Ag(t.p1.x, t.p2.x),
+                    r = Ag(t.p1.y, t.p2.y);
+                return Eg.roots(this.points, t).filter((t => {
                     var s = this.get(t);
-                    return kg.between(s.x, e, i) && kg.between(s.y, n, r)
+                    return Eg.between(s.x, e, i) && Eg.between(s.y, n, r)
                 }))
             }
             selfintersects(t) {
                 const e = this.reduce(),
                     n = e.length - 2,
                     i = [];
                 for (let r, s, o, a = 0; a < n; a++) s = e.slice(a, a + 1), o = e.slice(a + 2), r = this.curveintersects(s, o, t), i.push(...r);
@@ -27439,53 +27448,53 @@
                             left: t,
                             right: e
                         })
                     }))
                 }));
                 let r = [];
                 return i.forEach((function(t) {
-                    const e = kg.pairiteration(t.left, t.right, n);
+                    const e = Eg.pairiteration(t.left, t.right, n);
                     e.length > 0 && (r = r.concat(e))
                 })), r
             }
             arcs(t) {
                 return t = t || .5, this._iterate(t, [])
             }
             _error(t, e, n, i) {
                 const r = (i - n) / 4,
                     s = this.get(n + r),
                     o = this.get(i - r),
-                    a = kg.dist(t, e),
-                    l = kg.dist(t, s),
-                    c = kg.dist(t, o);
-                return Ig(l - a) + Ig(c - a)
+                    a = Eg.dist(t, e),
+                    l = Eg.dist(t, s),
+                    c = Eg.dist(t, o);
+                return Og(l - a) + Og(c - a)
             }
             _iterate(t, e) {
                 let n, i = 0,
                     r = 1;
                 do {
                     n = 0, r = 1;
                     let s, o, a, l, c, u = this.get(i),
                         h = !1,
                         d = !1,
                         f = r,
                         p = 1,
                         g = 0;
                     do {
-                        if (d = h, l = a, f = (i + r) / 2, g++, s = this.get(f), o = this.get(r), a = kg.getccenter(u, s, o), a.interval = {
+                        if (d = h, l = a, f = (i + r) / 2, g++, s = this.get(f), o = this.get(r), a = Eg.getccenter(u, s, o), a.interval = {
                                 start: i,
                                 end: r
                             }, h = this._error(a, u, i, r) <= t, c = d && !h, c || (p = r), h) {
                             if (r >= 1) {
                                 if (a.interval.end = p = 1, l = a, r > 1) {
                                     let t = {
-                                        x: a.x + a.r * Og(a.e),
-                                        y: a.y + a.r * Cg(a.e)
+                                        x: a.x + a.r * Pg(a.e),
+                                        y: a.y + a.r * Fg(a.e)
                                     };
-                                    a.e += kg.angle({
+                                    a.e += Eg.angle({
                                         x: a.x,
                                         y: a.y
                                     }, t, this.get(1))
                                 }
                                 break
                             }
                             r += (r - i) / 2
@@ -27493,15 +27502,15 @@
                     } while (!c && n++ < 100);
                     if (n >= 100) break;
                     l = l || a, e.push(l), i = p
                 } while (r < 1);
                 return e
             }
         }
-        const zg = {
+        const Rg = {
                 aliceblue: [240, 248, 255],
                 antiquewhite: [250, 235, 215],
                 aqua: [0, 255, 255],
                 aquamarine: [127, 255, 212],
                 azure: [240, 255, 255],
                 beige: [245, 245, 220],
                 bisque: [255, 228, 196],
@@ -27643,40 +27652,40 @@
                 violet: [238, 130, 238],
                 wheat: [245, 222, 179],
                 white: [255, 255, 255],
                 whitesmoke: [245, 245, 245],
                 yellow: [255, 255, 0],
                 yellowgreen: [154, 205, 50]
             },
-            Ng = function(t) {
+            Ug = function(t) {
                 var e, n, i = [],
                     r = 1;
                 if ("number" === typeof t) return {
                     space: "rgb",
                     values: [t >>> 16, (65280 & t) >>> 8, 255 & t],
                     alpha: 1
                 };
                 if ("number" === typeof t) return {
                     space: "rgb",
                     values: [t >>> 16, (65280 & t) >>> 8, 255 & t],
                     alpha: 1
                 };
-                if (t = String(t).toLowerCase(), zg[t]) i = zg[t].slice(), n = "rgb";
+                if (t = String(t).toLowerCase(), Rg[t]) i = Rg[t].slice(), n = "rgb";
                 else if ("transparent" === t) r = 0, n = "rgb", i = [0, 0, 0];
                 else if ("#" === t[0]) {
                     var s = t.slice(1),
                         o = s.length;
                     r = 1, o <= 4 ? (i = [parseInt(s[0] + s[0], 16), parseInt(s[1] + s[1], 16), parseInt(s[2] + s[2], 16)], 4 === o && (r = parseInt(s[3] + s[3], 16) / 255)) : (i = [parseInt(s[0] + s[1], 16), parseInt(s[2] + s[3], 16), parseInt(s[4] + s[5], 16)], 8 === o && (r = parseInt(s[6] + s[7], 16) / 255)), i[0] || (i[0] = 0), i[1] || (i[1] = 0), i[2] || (i[2] = 0), n = "rgb"
                 } else if (e = /^((?:rgba?|hs[lvb]a?|hwba?|cmyk?|xy[zy]|gray|lab|lchu?v?|[ly]uv|lms|oklch|oklab|color))\s*\(([^\)]*)\)/.exec(t)) {
                     var a = e[1],
                         l = "cmyk" === (n = a.replace(/a$/, "")) ? 4 : "gray" === n ? 1 : 3;
                     i = e[2].trim().split(/\s*[,\/]\s*|\s+/), "color" === n && (n = i.shift()), r = (i = i.map((function(t, e) {
                         if ("%" === t[t.length - 1]) return t = parseFloat(t) / 100, 3 === e ? t : "rgb" === n ? 255 * t : "h" === n[0] ? 100 * t : "l" !== n[0] || e ? "lab" === n ? 125 * t : "lch" === n ? e < 2 ? 150 * t : 360 * t : "o" !== n[0] || e ? "oklab" === n ? .4 * t : "oklch" === n ? e < 2 ? .4 * t : 360 * t : t : t : 100 * t;
                         if ("h" === n[e] || 2 === e && "h" === n[n.length - 1]) {
-                            if (void 0 !== Bg[t]) return Bg[t];
+                            if (void 0 !== Vg[t]) return Vg[t];
                             if (t.endsWith("deg")) return parseFloat(t);
                             if (t.endsWith("turn")) return 360 * parseFloat(t);
                             if (t.endsWith("grad")) return 360 * parseFloat(t) / 400;
                             if (t.endsWith("rad")) return 180 * parseFloat(t) / Math.PI
                         }
                         return "none" === t ? 0 : parseFloat(t)
                     }))).length > l ? i.pop() : 1
@@ -27688,30 +27697,30 @@
                 }
                 return {
                     space: n,
                     values: i,
                     alpha: r
                 }
             };
-        var Bg = {
+        var Vg = {
             red: 0,
             orange: 60,
             yellow: 120,
             green: 180,
             blue: 240,
             purple: 300
         };
-        const Rg = {
+        const jg = {
                 name: "rgb",
                 min: [0, 0, 0],
                 max: [255, 255, 255],
                 channel: ["red", "green", "blue"],
                 alias: ["RGB"]
             },
-            Ug = {
+            Wg = {
                 name: "hsl",
                 min: [0, 0, 0],
                 max: [360, 100, 100],
                 channel: ["hue", "saturation", "lightness"],
                 alias: ["HSL"],
                 rgb: function(t) {
                     var e, n, i, r, s, o = t[0] / 360,
@@ -27720,36 +27729,36 @@
                         c = 0;
                     if (0 === a) return [s = 255 * l, s, s];
                     for (e = 2 * l - (n = l < .5 ? l * (1 + a) : l + a - l * a), r = [0, 0, 0]; c < 3;)(i = o + 1 / 3 * -(c - 1)) < 0 ? i++ : i > 1 && i--, s = 6 * i < 1 ? e + 6 * (n - e) * i : 2 * i < 1 ? n : 3 * i < 2 ? e + (n - e) * (2 / 3 - i) * 6 : e, r[c++] = 255 * s;
                     return r
                 }
             };
 
-        function Vg(t) {
+        function Hg(t) {
             var e;
             Array.isArray(t) && t.raw && (t = String.raw(...arguments)), t instanceof Number && (t = +t);
-            var n = Ng(t);
+            var n = Ug(t);
             if (!n.space) return [];
-            const i = "h" === n.space[0] ? Ug.min : Rg.min,
-                r = "h" === n.space[0] ? Ug.max : Rg.max;
-            return (e = Array(3))[0] = Math.min(Math.max(n.values[0], i[0]), r[0]), e[1] = Math.min(Math.max(n.values[1], i[1]), r[1]), e[2] = Math.min(Math.max(n.values[2], i[2]), r[2]), "h" === n.space[0] && (e = Ug.rgb(e)), e.push(Math.min(Math.max(n.alpha, 0), 1)), e
+            const i = "h" === n.space[0] ? Wg.min : jg.min,
+                r = "h" === n.space[0] ? Wg.max : jg.max;
+            return (e = Array(3))[0] = Math.min(Math.max(n.values[0], i[0]), r[0]), e[1] = Math.min(Math.max(n.values[1], i[1]), r[1]), e[2] = Math.min(Math.max(n.values[2], i[2]), r[2]), "h" === n.space[0] && (e = Wg.rgb(e)), e.push(Math.min(Math.max(n.alpha, 0), 1)), e
         }
 
-        function jg(t, e) {
+        function Yg(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, n) => {
                     let [i, r] = t;
                     const s = r.x.map(((t, e) => ({
                             x: t,
                             y: r.y[e]
                         }))),
-                        o = Vg(r.color),
+                        o = Hg(r.color),
                         a = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
                         l = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.5)");
                     return {
                         data: s,
                         isControlPoint: !0,
                         label: i,
                         fill: !1,
@@ -27762,66 +27771,66 @@
                         backgroundColor: l,
                         borderColor: a
                     }
                 }))
             }
         }
 
-        function Wg(t, e) {
+        function $g(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, e) => {
                     let [n, i] = t;
                     const r = i.x.map(((t, e) => ({
                             x: t,
                             y: i.y[e]
                         }))),
                         s = [];
                     for (let a = 0; a < r.length - 2; a += 2) {
                         const t = r.slice(a, a + 3),
-                            e = new Lg(t).getLUT(10);
+                            e = new Bg(t).getLUT(10);
                         s.push(...e)
                     }
-                    const o = Vg(i.color);
+                    const o = Hg(i.color);
                     return {
                         label: n + " (bezier)",
                         data: s,
                         isControlPoint: !1,
                         showLine: !0,
                         tension: .3,
                         pointRadius: 0,
                         backgroundColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
                         borderColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.4)"),
                         borderDash: i.border_dash
                     }
                 }))
             }
         }
-        Rg.hsl = function(t) {
+        jg.hsl = function(t) {
             var e, n, i = t[0] / 255,
                 r = t[1] / 255,
                 s = t[2] / 255,
                 o = Math.min(i, r, s),
                 a = Math.max(i, r, s),
                 l = a - o;
             return a === o ? e = 0 : i === a ? e = (r - s) / l : r === a ? e = 2 + (s - i) / l : s === a && (e = 4 + (i - r) / l), (e = Math.min(60 * e, 360)) < 0 && (e += 360), n = (o + a) / 2, [e, 100 * (a === o ? 0 : n <= .5 ? l / (a + o) : l / (2 - a - o)), 100 * n]
         }, Hh.register(...$f, Up);
-        const Hg = class extends ao {
+        const Kg = class extends ao {
             constructor(t) {
                 var e, n;
                 super(t), this.downHandler = t => {
                     const e = $p(this.chartRef.current, t);
                     if (e.length > 0) {
                         this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
                             activePoint: e[0]
                         }), this.togglePan(!1))
                     }
-                }, this.calculateNewYValue = (t, e, n) => this.map(t.y, e.bottom, e.top, n.min, n.max), this.calculateNewXValue = (t, e, n) => this.map(t.x, e.left, e.right, n.min, n.max), this.updateControlPointPosition = (t, e, n, i) => {
+                }, this.updateControlPointPosition = (t, e, n, i) => {
                     const r = e.datasetIndex,
                         s = e.index;
                     t.data.datasets[r].data[s].x = n, t.data.datasets[r].data[s].y = i
                 }, this.updateOriginalData = (t, e) => {
                     const n = e.datasetIndex,
                         i = e.index,
                         r = t.data.datasets[n].label,
@@ -27830,37 +27839,37 @@
                     this.state.originalData[r].x[i] = s, this.state.originalData[r].y[i] = o
                 }, this.moveHandler = t => {
                     if (this.state.activePoint) {
                         const e = this.chartRef.current,
                             n = this.state.activePoint,
                             i = yc(t, e),
                             r = e.chartArea,
-                            s = this.calculateNewYValue(i, r, e.scales.y),
-                            o = this.calculateNewXValue(i, r, e.scales.x);
+                            s = ag(i, r, e.scales.y),
+                            o = lg(i, r, e.scales.x);
                         this.updateControlPointPosition(e, n, o, s), this.updateOriginalData(e, n);
-                        const a = Wg(this.state.originalData, this.props.args.options);
+                        const a = $g(this.state.originalData, this.props.args.options);
                         this.setState({
                             bezierData: a
                         }), e.update("none")
                     }
                 }, this.upHandler = t => {
                     this.state.activePoint && (this.sendBezierData(), this.setState({
                         activePoint: null
                     }), this.togglePan(!0))
-                }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.fixedData = (e = this.props.args.data, n = this.props.args.options, {
+                }, this.chartRef = f.createRef(), this.fixedData = (e = this.props.args.data, n = this.props.args.options, {
                     datasets: Object.entries(e).filter((t => {
                         let [e] = t;
                         return n.fixed_lines.includes(e)
                     })).map(((t, e) => {
                         let [n, i] = t;
                         const r = i.x.map(((t, e) => ({
                                 x: t,
                                 y: i.y[e]
                             }))),
-                            s = Vg(i.color);
+                            s = Hg(i.color);
                         return {
                             data: r,
                             isControlPoint: !1,
                             label: n,
                             fill: !1,
                             tension: .3,
                             spanGaps: !1,
@@ -27870,24 +27879,24 @@
                             pointRadius: i.point_radius,
                             borderDash: i.border_dash
                         }
                     }))
                 }), this.state = {
                     activePoint: null,
                     originalData: t.args.data,
-                    controlData: jg(this.props.args.data, this.props.args.options),
-                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    controlData: Yg(this.props.args.data, this.props.args.options),
+                    bezierData: $g(this.props.args.data, this.props.args.options),
                     options: tg(t.args.options, t.theme)
                 }
             }
             componentDidUpdate(t) {
                 ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                     originalData: this.props.args.data,
-                    controlData: jg(this.props.args.data, this.props.args.options),
-                    bezierData: Wg(this.props.args.data, this.props.args.options),
+                    controlData: Yg(this.props.args.data, this.props.args.options),
+                    bezierData: $g(this.props.args.data, this.props.args.options),
                     options: tg(this.props.args.options, this.props.theme)
                 })
             }
             sendBezierData() {
                 const t = this.convertBezierData(this.state.bezierData.datasets);
                 ro.setComponentValue(t)
             }
@@ -27906,38 +27915,38 @@
                             x: i,
                             y: r
                         } = t; - 1 === e[n].x.findIndex(((t, s) => t === i && e[n].y[s] === r)) && (e[n].x.push(i), e[n].y.push(r))
                     }))
                 })), e
             }
             render() {
-                return (0, ag.jsx)(Gp, {
+                return (0, ug.jsx)(Gp, {
                     ref: this.chartRef,
                     data: {
                         datasets: [...this.state.controlData.datasets, ...this.state.bezierData.datasets, ...this.fixedData.datasets]
                     },
                     options: this.state.options,
                     onPointerDown: this.downHandler,
                     onPointerUp: this.upHandler,
                     onPointerMove: this.moveHandler
                 })
             }
         };
 
-        function Yg(t, e) {
+        function qg(t, e) {
             const n = Object.entries(t).filter((t => {
                 let [n] = t;
                 return !e.fixed_lines.includes(n)
             })).map(((t, n) => {
                 let [i, r] = t;
                 const s = r.x.map(((t, e) => ({
                         x: t,
                         y: r.y[e]
                     }))),
-                    o = Vg(r.color),
+                    o = Hg(r.color),
                     a = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 1)"),
                     l = "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.8)");
                 return {
                     data: s,
                     isControlPoint: !0,
                     label: i,
                     spanGaps: e.fill_gaps,
@@ -27955,32 +27964,32 @@
                 }
             }));
             return {
                 datasets: n
             }
         }
 
-        function $g(t, e) {
+        function Xg(t, e) {
             return {
                 datasets: Object.entries(t).filter((t => {
                     let [n] = t;
                     return !e.fixed_lines.includes(n)
                 })).map(((t, e) => {
                     let [n, i] = t;
                     const r = i.x.map(((t, e) => ({
                             x: t,
                             y: i.y[e]
                         }))),
                         s = [];
                     for (let a = 0; a < r.length - 3; a += 3) {
                         const t = r.slice(a, a + 4),
-                            e = new Lg(t).getLUT(10);
+                            e = new Bg(t).getLUT(10);
                         s.push(...e)
                     }
-                    const o = Vg(i.color);
+                    const o = Hg(i.color);
                     return {
                         label: n + " (bezier)",
                         data: s,
                         isControlPoint: !1,
                         showLine: !0,
                         tension: .3,
                         backgroundColor: "rgba(".concat(o[0], ", ").concat(o[1], ", ").concat(o[2], ", 0.7)"),
@@ -27988,67 +27997,69 @@
                         pointRadius: 0,
                         borderDash: i.border_dash
                     }
                 }))
             }
         }
         Hh.register(...$f, Up);
-        const Xg = {
-                line_chart: lg,
-                scatter_chart: ug,
-                bezier_chart: Hg,
+        const Qg = {
+                line_chart: hg,
+                scatter_chart: fg,
+                bezier_chart: Kg,
                 cubic_bezier_chart: class extends ao {
                     constructor(t) {
                         var e, n;
                         super(t), this.downHandler = t => {
                             const e = $p(this.chartRef.current, t);
                             if (e.length > 0) {
                                 this.chartRef.current.data.datasets[e[0].datasetIndex].isControlPoint && (this.setState({
                                     activePoint: e[0]
                                 }), this.togglePan(!1))
                             }
-                        }, this.calculateNewYValue = (t, e, n) => this.map(t.y, e.bottom, e.top, n.min, n.max), this.calculateNewXValue = (t, e, n) => this.map(t.x, e.left, e.right, n.min, n.max), this.moveHandler = t => {
+                        }, this.moveHandler = t => {
                             if (this.state.activePoint) {
                                 const e = this.chartRef.current,
                                     n = this.state.activePoint,
                                     i = yc(t, e),
                                     r = e.chartArea,
-                                    s = this.calculateNewYValue(i, r, e.scales.y),
-                                    o = this.calculateNewXValue(i, r, e.scales.x),
+                                    s = ag(i, r, e.scales.y),
+                                    o = lg(i, r, e.scales.x),
                                     a = n.datasetIndex,
-                                    l = n.index,
-                                    c = s - e.data.datasets[a].data[l].y,
-                                    u = o - e.data.datasets[a].data[l].x;
-                                e.data.datasets[a].data[l].x = o, e.data.datasets[a].data[l].y = s;
-                                const h = e.data.datasets[a].label,
-                                    d = e.data.datasets[a].data[l].x,
-                                    f = e.data.datasets[a].data[l].y;
-                                this.state.originalData[h].x[l] = d, this.state.originalData[h].y[l] = f;
-                                const p = e.data.datasets[a].data.length;
-                                0 === l ? (e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : l === p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c) : l % 3 === 0 && 0 !== l && l !== p - 1 ? (e.data.datasets[a].data[l - 1].x += u, e.data.datasets[a].data[l - 1].y += c, e.data.datasets[a].data[l + 1].x += u, e.data.datasets[a].data[l + 1].y += c, this.state.originalData[h].x[l - 1] += u, this.state.originalData[h].y[l - 1] += c, this.state.originalData[h].x[l + 1] += u, this.state.originalData[h].y[l + 1] += c) : (l + 1) % 3 === 0 && l + 1 !== p - 1 ? (e.data.datasets[a].data[l + 2].x -= u, e.data.datasets[a].data[l + 2].y -= c, this.state.originalData[h].x[l + 2] -= u, this.state.originalData[h].y[l + 2] -= c) : (l - 1) % 3 === 0 && l - 1 !== 0 && (e.data.datasets[a].data[l - 2].x -= u, e.data.datasets[a].data[l - 2].y -= c, this.state.originalData[h].x[l - 2] -= u, this.state.originalData[h].y[l - 2] -= c);
-                                const g = $g(this.state.originalData, this.props.args.options);
+                                    l = e.data.datasets[a],
+                                    c = n.index,
+                                    u = s - l.data[c].y,
+                                    h = o - l.data[c].x;
+                                l.data[c].x = o, l.data[c].y = s;
+                                const d = l.label,
+                                    f = this.state.originalData[d],
+                                    p = l.data[c].x,
+                                    g = l.data[c].y;
+                                f.x[c] = p, f.y[c] = g;
+                                const m = l.data.length;
+                                0 === c ? (l.data[c + 1].x += h, l.data[c + 1].y += u, f.x[c + 1] += h, f.y[c + 1] += u) : c === m - 1 ? (l.data[c - 1].x += h, l.data[c - 1].y += u, f.x[c - 1] += h, f.y[c - 1] += u) : c % 3 === 0 && 0 !== c && c !== m - 1 ? (l.data[c - 1].x += h, l.data[c - 1].y += u, l.data[c + 1].x += h, l.data[c + 1].y += u, f.x[c - 1] += h, f.y[c - 1] += u, f.x[c + 1] += h, f.y[c + 1] += u) : (c + 1) % 3 === 0 && c + 1 !== m - 1 ? (l.data[c + 2].x -= h, l.data[c + 2].y -= u, f.x[c + 2] -= h, f.y[c + 2] -= u) : (c - 1) % 3 === 0 && c - 1 !== 0 && (l.data[c - 2].x -= h, l.data[c - 2].y -= u, f.x[c - 2] -= h, f.y[c - 2] -= u);
+                                const y = Xg(this.state.originalData, this.props.args.options);
                                 this.setState({
-                                    bezierData: g
+                                    bezierData: y
                                 }), e.update("none")
                             }
                         }, this.upHandler = t => {
                             this.state.activePoint && (this.sendBezierData(), this.setState({
                                 activePoint: null
                             }), this.togglePan(!0))
-                        }, this.map = (t, e, n, i, r) => i + (t - e) / (n - e) * (r - i), this.chartRef = f.createRef(), this.fixedData = (e = this.props.args.data, n = this.props.args.options, {
+                        }, this.chartRef = f.createRef(), this.fixedData = (e = this.props.args.data, n = this.props.args.options, {
                             datasets: Object.entries(e).filter((t => {
                                 let [e] = t;
                                 return n.fixed_lines.includes(e)
                             })).map(((t, e) => {
                                 let [i, r] = t;
                                 const s = r.x.map(((t, e) => ({
                                         x: t,
                                         y: r.y[e]
                                     }))),
-                                    o = Vg(r.color);
+                                    o = Hg(r.color);
                                 return {
                                     data: s,
                                     isControlPoint: !1,
                                     label: i,
                                     fill: !1,
                                     tension: .3,
                                     showLine: !0,
@@ -28058,24 +28069,24 @@
                                     pointRadius: r.point_radius,
                                     borderDash: r.border_dash
                                 }
                             }))
                         }), this.state = {
                             activePoint: null,
                             originalData: t.args.data,
-                            controlData: Yg(this.props.args.data, this.props.args.options),
-                            bezierData: $g(this.props.args.data, this.props.args.options),
+                            controlData: qg(this.props.args.data, this.props.args.options),
+                            bezierData: Xg(this.props.args.data, this.props.args.options),
                             options: tg(t.args.options, t.theme)
                         }
                     }
                     componentDidUpdate(t) {
                         ro.setFrameHeight(), this.props.args !== t.args && this.setState({
                             originalData: this.props.args.data,
-                            controlData: Yg(this.props.args.data, this.props.args.options),
-                            bezierData: $g(this.props.args.data, this.props.args.options),
+                            controlData: qg(this.props.args.data, this.props.args.options),
+                            bezierData: Xg(this.props.args.data, this.props.args.options),
                             options: tg(this.props.args.options, this.props.theme)
                         })
                     }
                     sendBezierData() {
                         const t = this.convertBezierData(this.state.bezierData.datasets);
                         ro.setComponentValue(t)
                     }
@@ -28094,28 +28105,28 @@
                                     x: i,
                                     y: r
                                 } = t; - 1 === e[n].x.findIndex(((t, s) => t === i && e[n].y[s] === r)) && (e[n].x.push(i), e[n].y.push(r))
                             }))
                         })), e
                     }
                     render() {
-                        return (0, ag.jsx)(Gp, {
+                        return (0, ug.jsx)(Gp, {
                             ref: this.chartRef,
                             data: {
                                 datasets: [...this.state.controlData.datasets, ...this.state.bezierData.datasets, ...this.fixedData.datasets]
                             },
                             options: this.state.options,
                             onPointerDown: this.downHandler,
                             onPointerUp: this.upHandler,
                             onPointerMove: this.moveHandler
                         })
                     }
                 }
             },
-            Kg = function(t) {
+            Gg = function(t) {
                 var e = function(e) {
                     function n(t) {
                         var n = e.call(this, t) || this;
                         return n.componentDidMount = function() {
                             ro.events.addEventListener(ro.RENDER_EVENT, n.onRenderEvent), ro.setComponentReady()
                         }, n.componentDidUpdate = function() {
                             null != n.state.componentError && ro.setFrameHeight()
@@ -28143,22 +28154,22 @@
                         }
                     }, n
                 }(f.PureComponent);
                 return d()(e, t)
             }((t => {
                 const e = t.args.id,
                     n = t.args.kw,
-                    i = Xg[e];
+                    i = Qg[e];
                 if (void 0 === i) throw new Error("Component with id ".concat(e, " is not defined in componentsMap."));
-                return (0, ag.jsx)(i, {
+                return (0, ug.jsx)(i, {
                     args: {
                         ...n
                     },
                     theme: t.theme
                 })
             }));
-        lo.render((0, ag.jsx)(f.StrictMode, {
-            children: (0, ag.jsx)(Kg, {})
+        lo.render((0, ug.jsx)(f.StrictMode, {
+            children: (0, ug.jsx)(Gg, {})
         }), document.getElementById("root"))
     })()
 })();
-//# sourceMappingURL=main.41dd267d.js.map
+//# sourceMappingURL=main.8018b5ba.js.map
```

### Comparing `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt` & `draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/frontend/build/static/js/main.41dd267d.js.map` & `draggable-charts-1.2.6/draggable_charts/frontend/build/static/js/main.8018b5ba.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8529432748758946%*

 * *Differences: {"'file'": "'static/js/main.8018b5ba.js'",*

 * * "'mappings'": "';2BAAA,OAKA,SAAUA,EAAQC,EAAUC,EAAYC,GACtC,aAEF,IA+FIC,EA/FAC,EAAkB,CAAC,GAAI,SAAU,MAAO,KAAM,KAAM,KACpDC,EAAeL,EAASM,cAAc,OAEtCC,EAAgB,WAEhBC,EAAQC,KAAKD,MACbE,EAAMD,KAAKC,IACXC,EAAMC,KAAKD,IASf,SAASE,EAAkBC,EAAIC,EAASC,GACpC,OAAOC,WAAWC,EAAOJ,EAAIE,GAAUD,EAC3C,CAWA,SAASI,EAAeC,EAAKN,EAAIE,GAC7B,QAAIK,MAAMC,QAAQF,KACdG,EAAKH,EAAKJ,EAAQF,GAAKE,IAChB,EAGf,CAQA,SAASO,EAAKC,EAAKC,EAAUT,GACzB,IAAIU,EAEJ,GAAKF,EAIL,GAAIA,EAAIG,QACJH,EAAIG,QAAQF,EAAUT,QACn […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.41dd267d.js",
+    "file": "static/js/main.8018b5ba.js",
     "names": [
         "window",
         "document",
         "exportName",
         "undefined",
         "assign",
         "VENDOR_PREFIXES",
@@ -5699,51 +5699,54 @@
         "chartElement",
         "cursorStyle",
         "fixed_lines",
         "determineCursorStyle",
         "legend_position",
         "legend_align",
         "formatTickValue",
-        "x_type",
         "xScaleOptions",
+        "x_type",
+        "shouldFormat",
+        "x_format",
         "x_label",
         "x_grid",
         "fadedText05",
         "x_labels",
         "yScaleOptions",
         "y_type",
+        "y_format",
         "y_label",
         "y_grid",
         "y_labels",
         "Xvalue",
         "Yvalue",
+        "calculateNewYValue",
+        "yAxis",
+        "categories",
+        "calculateNewXValue",
+        "start1",
+        "stop1",
+        "start2",
+        "stop2",
         "zoomPlugin",
         "downHandler",
         "datasetLabel",
         "activePoint",
         "togglePan",
         "moveHandler",
-        "yAxis",
         "yValue",
-        "upHandler",
         "xLabel",
         "chartData",
+        "upHandler",
         "originalData",
-        "start1",
-        "stop1",
-        "start2",
-        "stop2",
         "prevProps",
         "_jsx",
         "onPointerDown",
         "onPointerUp",
         "onPointerMove",
-        "calculateNewYValue",
-        "categories",
-        "calculateNewXValue",
         "newYValue",
         "newXValue",
         "xValue",
         "acos",
         "crt",
         "tau",
         "quart",
@@ -6137,14 +6140,15 @@
         "line_chart",
         "LineChart",
         "scatter_chart",
         "ScatterChart",
         "bezier_chart",
         "BezierChart",
         "cubic_bezier_chart",
+        "originalDataset",
         "dataLen",
         "StreamlitComponent",
         "WrappedComponent",
         "ComponentWrapper",
         "onRenderEvent",
         "componentError",
         "renderData",
@@ -6348,14 +6352,15 @@
         "../node_modules/chart.js/src/index.ts",
         "../node_modules/chartjs-plugin-zoom/dist/chartjs-plugin-zoom.esm.js",
         "../node_modules/react-chartjs-2/src/utils.ts",
         "../node_modules/react-chartjs-2/src/chart.tsx",
         "../node_modules/react-chartjs-2/src/typedCharts.tsx",
         "LineChart/chartData.jsx",
         "Utils/chartOptions.jsx",
+        "Utils/handlers.jsx",
         "LineChart/LineChart.jsx",
         "ScatterChart/chartData.jsx",
         "ScatterChart/ScatterChart.jsx",
         "../node_modules/bezier-js/src/utils.js",
         "../node_modules/bezier-js/src/poly-bezier.js",
         "../node_modules/bezier-js/src/bezier.js",
         "../node_modules/color-parse/node_modules/color-name/index.js",
@@ -6562,28 +6567,29 @@
         "import TimeScale from './scale.time.js';\nimport {_lookupByKey} from '../helpers/helpers.collection.js';\n\n/**\n * Linearly interpolates the given source `val` using the table. If value is out of bounds, values\n * at edges are used for the interpolation.\n * @param {object} table\n * @param {number} val\n * @param {boolean} [reverse] lookup time based on position instead of vice versa\n * @return {object}\n */\nfunction interpolate(table, val, reverse) {\n  let lo = 0;\n  let hi = table.length - 1;\n  let prevSource, nextSource, prevTarget, nextTarget;\n  if (reverse) {\n    if (val >= table[lo].pos && val <= table[hi].pos) {\n      ({lo, hi} = _lookupByKey(table, 'pos', val));\n    }\n    ({pos: prevSource, time: prevTarget} = table[lo]);\n    ({pos: nextSource, time: nextTarget} = table[hi]);\n  } else {\n    if (val >= table[lo].time && val <= table[hi].time) {\n      ({lo, hi} = _lookupByKey(table, 'time', val));\n    }\n    ({time: prevSource, pos: prevTarget} = table[lo]);\n    ({time: nextSource, pos: nextTarget} = table[hi]);\n  }\n\n  const span = nextSource - prevSource;\n  return span ? prevTarget + (nextTarget - prevTarget) * (val - prevSource) / span : prevTarget;\n}\n\nclass TimeSeriesScale extends TimeScale {\n\n  static id = 'timeseries';\n\n  /**\n   * @type {any}\n   */\n  static defaults = TimeScale.defaults;\n\n  /**\n\t * @param {object} props\n\t */\n  constructor(props) {\n    super(props);\n\n    /** @type {object[]} */\n    this._table = [];\n    /** @type {number} */\n    this._minPos = undefined;\n    /** @type {number} */\n    this._tableRange = undefined;\n  }\n\n  /**\n\t * @protected\n\t */\n  initOffsets() {\n    const timestamps = this._getTimestampsForTable();\n    const table = this._table = this.buildLookupTable(timestamps);\n    this._minPos = interpolate(table, this.min);\n    this._tableRange = interpolate(table, this.max) - this._minPos;\n    super.initOffsets(timestamps);\n  }\n\n  /**\n\t * Returns an array of {time, pos} objects used to interpolate a specific `time` or position\n\t * (`pos`) on the scale, by searching entries before and after the requested value. `pos` is\n\t * a decimal between 0 and 1: 0 being the start of the scale (left or top) and 1 the other\n\t * extremity (left + width or top + height). Note that it would be more optimized to directly\n\t * store pre-computed pixels, but the scale dimensions are not guaranteed at the time we need\n\t * to create the lookup table. The table ALWAYS contains at least two items: min and max.\n\t * @param {number[]} timestamps\n\t * @return {object[]}\n\t * @protected\n\t */\n  buildLookupTable(timestamps) {\n    const {min, max} = this;\n    const items = [];\n    const table = [];\n    let i, ilen, prev, curr, next;\n\n    for (i = 0, ilen = timestamps.length; i < ilen; ++i) {\n      curr = timestamps[i];\n      if (curr >= min && curr <= max) {\n        items.push(curr);\n      }\n    }\n\n    if (items.length < 2) {\n      // In case there is less that 2 timestamps between min and max, the scale is defined by min and max\n      return [\n        {time: min, pos: 0},\n        {time: max, pos: 1}\n      ];\n    }\n\n    for (i = 0, ilen = items.length; i < ilen; ++i) {\n      next = items[i + 1];\n      prev = items[i - 1];\n      curr = items[i];\n\n      // only add points that breaks the scale linearity\n      if (Math.round((next + prev) / 2) !== curr) {\n        table.push({time: curr, pos: i / (ilen - 1)});\n      }\n    }\n    return table;\n  }\n\n  /**\n    * Generates all timestamps defined in the data.\n    * Important: this method can return ticks outside the min and max range, it's the\n    * responsibility of the calling code to clamp values if needed.\n    * @protected\n    */\n  _generate() {\n    const min = this.min;\n    const max = this.max;\n    let timestamps = super.getDataTimestamps();\n    if (!timestamps.includes(min) || !timestamps.length) {\n      timestamps.splice(0, 0, min);\n    }\n    if (!timestamps.includes(max) || timestamps.length === 1) {\n      timestamps.push(max);\n    }\n    return timestamps.sort((a, b) => a - b);\n  }\n\n  /**\n\t * Returns all timestamps\n\t * @return {number[]}\n\t * @private\n\t */\n  _getTimestampsForTable() {\n    let timestamps = this._cache.all || [];\n\n    if (timestamps.length) {\n      return timestamps;\n    }\n\n    const data = this.getDataTimestamps();\n    const label = this.getLabelTimestamps();\n    if (data.length && label.length) {\n      // If combining labels and data (data might not contain all labels),\n      // we need to recheck uniqueness and sort\n      timestamps = this.normalize(data.concat(label));\n    } else {\n      timestamps = data.length ? data : label;\n    }\n    timestamps = this._cache.all = timestamps;\n\n    return timestamps;\n  }\n\n  /**\n\t * @param {number} value - Milliseconds since epoch (1 January 1970 00:00:00 UTC)\n\t * @return {number}\n\t */\n  getDecimalForValue(value) {\n    return (interpolate(this._table, value) - this._minPos) / this._tableRange;\n  }\n\n  /**\n\t * @param {number} pixel\n\t * @return {number}\n\t */\n  getValueForPixel(pixel) {\n    const offsets = this._offsets;\n    const decimal = this.getDecimalForPixel(pixel) / offsets.factor - offsets.end;\n    return interpolate(this._table, decimal * this._tableRange + this._minPos, true);\n  }\n}\n\nexport default TimeSeriesScale;\n",
         "export * from './controllers/index.js';\nexport * from './core/index.js';\nexport * from './elements/index.js';\nexport * from './platform/index.js';\nexport * from './plugins/index.js';\nexport * from './scales/index.js';\n\nimport * as controllers from './controllers/index.js';\nimport * as elements from './elements/index.js';\nimport * as plugins from './plugins/index.js';\nimport * as scales from './scales/index.js';\n\nexport {\n  controllers,\n  elements,\n  plugins,\n  scales,\n};\n\nexport const registerables = [\n  controllers,\n  elements,\n  plugins,\n  scales,\n];\n",
         "/*!\n* chartjs-plugin-zoom v2.0.1\n* undefined\n * (c) 2016-2023 chartjs-plugin-zoom Contributors\n * Released under the MIT License\n */\nimport Hammer from 'hammerjs';\nimport { each, valueOrDefault, callback, sign, getRelativePosition } from 'chart.js/helpers';\n\nconst getModifierKey = opts => opts && opts.enabled && opts.modifierKey;\nconst keyPressed = (key, event) => key && event[key + 'Key'];\nconst keyNotPressed = (key, event) => key && !event[key + 'Key'];\n\n/**\n * @param {string|function} mode can be 'x', 'y' or 'xy'\n * @param {string} dir can be 'x' or 'y'\n * @param {import('chart.js').Chart} chart instance of the chart in question\n * @returns {boolean}\n */\nfunction directionEnabled(mode, dir, chart) {\n  if (mode === undefined) {\n    return true;\n  } else if (typeof mode === 'string') {\n    return mode.indexOf(dir) !== -1;\n  } else if (typeof mode === 'function') {\n    return mode({chart}).indexOf(dir) !== -1;\n  }\n\n  return false;\n}\n\nfunction directionsEnabled(mode, chart) {\n  if (typeof mode === 'function') {\n    mode = mode({chart});\n  }\n  if (typeof mode === 'string') {\n    return {x: mode.indexOf('x') !== -1, y: mode.indexOf('y') !== -1};\n  }\n\n  return {x: false, y: false};\n}\n\n/**\n * Debounces calling `fn` for `delay` ms\n * @param {function} fn - Function to call. No arguments are passed.\n * @param {number} delay - Delay in ms. 0 = immediate invocation.\n * @returns {function}\n */\nfunction debounce(fn, delay) {\n  let timeout;\n  return function() {\n    clearTimeout(timeout);\n    timeout = setTimeout(fn, delay);\n    return delay;\n  };\n}\n\n/**\n * Checks which axis is under the mouse cursor.\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale}\n */\nfunction getScaleUnderPoint({x, y}, chart) {\n  const scales = chart.scales;\n  const scaleIds = Object.keys(scales);\n  for (let i = 0; i < scaleIds.length; i++) {\n    const scale = scales[scaleIds[i]];\n    if (y >= scale.top && y <= scale.bottom && x >= scale.left && x <= scale.right) {\n      return scale;\n    }\n  }\n  return null;\n}\n\n/**\n * Evaluate the chart's mode, scaleMode, and overScaleMode properties to\n * determine which axes are eligible for scaling.\n * options.overScaleMode can be a function if user want zoom only one scale of many for example.\n * @param options - Zoom or pan options\n * @param {{x: number, y: number}} point - the mouse location\n * @param {import('chart.js').Chart} [chart] instance of the chart in question\n * @return {import('chart.js').Scale[]}\n */\nfunction getEnabledScalesByPoint(options, point, chart) {\n  const {mode = 'xy', scaleMode, overScaleMode} = options || {};\n  const scale = getScaleUnderPoint(point, chart);\n\n  const enabled = directionsEnabled(mode, chart);\n  const scaleEnabled = directionsEnabled(scaleMode, chart);\n\n  // Convert deprecated overScaleEnabled to new scaleEnabled.\n  if (overScaleMode) {\n    const overScaleEnabled = directionsEnabled(overScaleMode, chart);\n    for (const axis of ['x', 'y']) {\n      if (overScaleEnabled[axis]) {\n        scaleEnabled[axis] = enabled[axis];\n        enabled[axis] = false;\n      }\n    }\n  }\n\n  if (scale && scaleEnabled[scale.axis]) {\n    return [scale];\n  }\n\n  const enabledScales = [];\n  each(chart.scales, function(scaleItem) {\n    if (enabled[scaleItem.axis]) {\n      enabledScales.push(scaleItem);\n    }\n  });\n  return enabledScales;\n}\n\nconst chartStates = new WeakMap();\n\nfunction getState(chart) {\n  let state = chartStates.get(chart);\n  if (!state) {\n    state = {\n      originalScaleLimits: {},\n      updatedScaleLimits: {},\n      handlers: {},\n      panDelta: {}\n    };\n    chartStates.set(chart, state);\n  }\n  return state;\n}\n\nfunction removeState(chart) {\n  chartStates.delete(chart);\n}\n\nfunction zoomDelta(scale, zoom, center) {\n  const range = scale.max - scale.min;\n  const newRange = range * (zoom - 1);\n\n  const centerPoint = scale.isHorizontal() ? center.x : center.y;\n  // `scale.getValueForPixel()` can return a value less than the `scale.min` or\n  // greater than `scale.max` when `centerPoint` is outside chartArea.\n  const minPercent = Math.max(0, Math.min(1,\n    (scale.getValueForPixel(centerPoint) - scale.min) / range || 0\n  ));\n\n  const maxPercent = 1 - minPercent;\n\n  return {\n    min: newRange * minPercent,\n    max: newRange * maxPercent\n  };\n}\n\nfunction getLimit(state, scale, scaleLimits, prop, fallback) {\n  let limit = scaleLimits[prop];\n  if (limit === 'original') {\n    const original = state.originalScaleLimits[scale.id][prop];\n    limit = valueOrDefault(original.options, original.scale);\n  }\n  return valueOrDefault(limit, fallback);\n}\n\nfunction getRange(scale, pixel0, pixel1) {\n  const v0 = scale.getValueForPixel(pixel0);\n  const v1 = scale.getValueForPixel(pixel1);\n  return {\n    min: Math.min(v0, v1),\n    max: Math.max(v0, v1)\n  };\n}\n\nfunction updateRange(scale, {min, max}, limits, zoom = false) {\n  const state = getState(scale.chart);\n  const {id, axis, options: scaleOpts} = scale;\n\n  const scaleLimits = limits && (limits[id] || limits[axis]) || {};\n  const {minRange = 0} = scaleLimits;\n  const minLimit = getLimit(state, scale, scaleLimits, 'min', -Infinity);\n  const maxLimit = getLimit(state, scale, scaleLimits, 'max', Infinity);\n\n  const range = zoom ? Math.max(max - min, minRange) : scale.max - scale.min;\n  const offset = (range - max + min) / 2;\n  min -= offset;\n  max += offset;\n\n  if (min < minLimit) {\n    min = minLimit;\n    max = Math.min(minLimit + range, maxLimit);\n  } else if (max > maxLimit) {\n    max = maxLimit;\n    min = Math.max(maxLimit - range, minLimit);\n  }\n  scaleOpts.min = min;\n  scaleOpts.max = max;\n\n  state.updatedScaleLimits[scale.id] = {min, max};\n\n  // return true if the scale range is changed\n  return scale.parse(min) !== scale.min || scale.parse(max) !== scale.max;\n}\n\nfunction zoomNumericalScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  const newRange = {min: scale.min + delta.min, max: scale.max - delta.max};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction zoomRectNumericalScale(scale, from, to, limits) {\n  updateRange(scale, getRange(scale, from, to), limits, true);\n}\n\nconst integerChange = (v) => v === 0 || isNaN(v) ? 0 : v < 0 ? Math.min(Math.round(v), -1) : Math.max(Math.round(v), 1);\n\nfunction existCategoryFromMaxZoom(scale) {\n  const labels = scale.getLabels();\n  const maxIndex = labels.length - 1;\n\n  if (scale.min > 0) {\n    scale.min -= 1;\n  }\n  if (scale.max < maxIndex) {\n    scale.max += 1;\n  }\n}\n\nfunction zoomCategoryScale(scale, zoom, center, limits) {\n  const delta = zoomDelta(scale, zoom, center);\n  if (scale.min === scale.max && zoom < 1) {\n    existCategoryFromMaxZoom(scale);\n  }\n  const newRange = {min: scale.min + integerChange(delta.min), max: scale.max - integerChange(delta.max)};\n  return updateRange(scale, newRange, limits, true);\n}\n\nfunction scaleLength(scale) {\n  return scale.isHorizontal() ? scale.width : scale.height;\n}\n\nfunction panCategoryScale(scale, delta, limits) {\n  const labels = scale.getLabels();\n  const lastLabelIndex = labels.length - 1;\n  let {min, max} = scale;\n  // The visible range. Ticks can be skipped, and thus not reliable.\n  const range = Math.max(max - min, 1);\n  // How many pixels of delta is required before making a step. stepSize, but limited to max 1/10 of the scale length.\n  const stepDelta = Math.round(scaleLength(scale) / Math.max(range, 10));\n  const stepSize = Math.round(Math.abs(delta / stepDelta));\n  let applied;\n  if (delta < -stepDelta) {\n    max = Math.min(max + stepSize, lastLabelIndex);\n    min = range === 1 ? max : max - range;\n    applied = max === lastLabelIndex;\n  } else if (delta > stepDelta) {\n    min = Math.max(0, min - stepSize);\n    max = range === 1 ? min : min + range;\n    applied = min === 0;\n  }\n\n  return updateRange(scale, {min, max}, limits) || applied;\n}\n\nconst OFFSETS = {\n  second: 500, // 500 ms\n  minute: 30 * 1000, // 30 s\n  hour: 30 * 60 * 1000, // 30 m\n  day: 12 * 60 * 60 * 1000, // 12 h\n  week: 3.5 * 24 * 60 * 60 * 1000, // 3.5 d\n  month: 15 * 24 * 60 * 60 * 1000, // 15 d\n  quarter: 60 * 24 * 60 * 60 * 1000, // 60 d\n  year: 182 * 24 * 60 * 60 * 1000 // 182 d\n};\n\nfunction panNumericalScale(scale, delta, limits, canZoom = false) {\n  const {min: prevStart, max: prevEnd, options} = scale;\n  const round = options.time && options.time.round;\n  const offset = OFFSETS[round] || 0;\n  const newMin = scale.getValueForPixel(scale.getPixelForValue(prevStart + offset) - delta);\n  const newMax = scale.getValueForPixel(scale.getPixelForValue(prevEnd + offset) - delta);\n  const {min: minLimit = -Infinity, max: maxLimit = Infinity} = canZoom && limits && limits[scale.axis] || {};\n  if (isNaN(newMin) || isNaN(newMax) || newMin < minLimit || newMax > maxLimit) {\n    // At limit: No change but return true to indicate no need to store the delta.\n    // NaN can happen for 0-dimension scales (either because they were configured\n    // with min === max or because the chart has 0 plottable area).\n    return true;\n  }\n  return updateRange(scale, {min: newMin, max: newMax}, limits, canZoom);\n}\n\nfunction panNonLinearScale(scale, delta, limits) {\n  return panNumericalScale(scale, delta, limits, true);\n}\n\nconst zoomFunctions = {\n  category: zoomCategoryScale,\n  default: zoomNumericalScale,\n};\n\nconst zoomRectFunctions = {\n  default: zoomRectNumericalScale,\n};\n\nconst panFunctions = {\n  category: panCategoryScale,\n  default: panNumericalScale,\n  logarithmic: panNonLinearScale,\n  timeseries: panNonLinearScale,\n};\n\nfunction shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits) {\n  const {id, options: {min, max}} = scale;\n  if (!originalScaleLimits[id] || !updatedScaleLimits[id]) {\n    return true;\n  }\n  const previous = updatedScaleLimits[id];\n  return previous.min !== min || previous.max !== max;\n}\n\nfunction removeMissingScales(limits, scales) {\n  each(limits, (opt, key) => {\n    if (!scales[key]) {\n      delete limits[key];\n    }\n  });\n}\n\nfunction storeOriginalScaleLimits(chart, state) {\n  const {scales} = chart;\n  const {originalScaleLimits, updatedScaleLimits} = state;\n\n  each(scales, function(scale) {\n    if (shouldUpdateScaleLimits(scale, originalScaleLimits, updatedScaleLimits)) {\n      originalScaleLimits[scale.id] = {\n        min: {scale: scale.min, options: scale.options.min},\n        max: {scale: scale.max, options: scale.options.max},\n      };\n    }\n  });\n\n  removeMissingScales(originalScaleLimits, scales);\n  removeMissingScales(updatedScaleLimits, scales);\n  return originalScaleLimits;\n}\n\nfunction doZoom(scale, amount, center, limits) {\n  const fn = zoomFunctions[scale.type] || zoomFunctions.default;\n  callback(fn, [scale, amount, center, limits]);\n}\n\nfunction doZoomRect(scale, amount, from, to, limits) {\n  const fn = zoomRectFunctions[scale.type] || zoomRectFunctions.default;\n  callback(fn, [scale, amount, from, to, limits]);\n}\n\nfunction getCenter(chart) {\n  const ca = chart.chartArea;\n  return {\n    x: (ca.left + ca.right) / 2,\n    y: (ca.top + ca.bottom) / 2,\n  };\n}\n\n/**\n * @param chart The chart instance\n * @param {number | {x?: number, y?: number, focalPoint?: {x: number, y: number}}} amount The zoom percentage or percentages and focal point\n * @param {string} [transition] Which transition mode to use. Defaults to 'none'\n */\nfunction zoom(chart, amount, transition = 'none') {\n  const {x = 1, y = 1, focalPoint = getCenter(chart)} = typeof amount === 'number' ? {x: amount, y: amount} : amount;\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 1;\n  const yEnabled = y !== 1;\n  const enabledScales = getEnabledScalesByPoint(zoomOptions, focalPoint, chart);\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoom(scale, x, focalPoint, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoom(scale, y, focalPoint, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomRect(chart, p0, p1, transition = 'none') {\n  const state = getState(chart);\n  const {options: {limits, zoom: zoomOptions}} = state;\n  const {mode = 'xy'} = zoomOptions;\n\n  storeOriginalScaleLimits(chart, state);\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n\n  each(chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      doZoomRect(scale, p0.x, p1.x, limits);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      doZoomRect(scale, p0.y, p1.y, limits);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(zoomOptions.onZoom, [{chart}]);\n}\n\nfunction zoomScale(chart, scaleId, range, transition = 'none') {\n  storeOriginalScaleLimits(chart, getState(chart));\n  const scale = chart.scales[scaleId];\n  updateRange(scale, range, undefined, true);\n  chart.update(transition);\n}\n\nfunction resetZoom(chart, transition = 'default') {\n  const state = getState(chart);\n  const originalScaleLimits = storeOriginalScaleLimits(chart, state);\n\n  each(chart.scales, function(scale) {\n    const scaleOptions = scale.options;\n    if (originalScaleLimits[scale.id]) {\n      scaleOptions.min = originalScaleLimits[scale.id].min.options;\n      scaleOptions.max = originalScaleLimits[scale.id].max.options;\n    } else {\n      delete scaleOptions.min;\n      delete scaleOptions.max;\n    }\n  });\n  chart.update(transition);\n  callback(state.options.zoom.onZoomComplete, [{chart}]);\n}\n\nfunction getOriginalRange(state, scaleId) {\n  const original = state.originalScaleLimits[scaleId];\n  if (!original) {\n    return;\n  }\n  const {min, max} = original;\n  return valueOrDefault(max.options, max.scale) - valueOrDefault(min.options, min.scale);\n}\n\nfunction getZoomLevel(chart) {\n  const state = getState(chart);\n  let min = 1;\n  let max = 1;\n  each(chart.scales, function(scale) {\n    const origRange = getOriginalRange(state, scale.id);\n    if (origRange) {\n      const level = Math.round(origRange / (scale.max - scale.min) * 100) / 100;\n      min = Math.min(min, level);\n      max = Math.max(max, level);\n    }\n  });\n  return min < 1 ? min : max;\n}\n\nfunction panScale(scale, delta, limits, state) {\n  const {panDelta} = state;\n  // Add possible cumulative delta from previous pan attempts where scale did not change\n  const storedDelta = panDelta[scale.id] || 0;\n  if (sign(storedDelta) === sign(delta)) {\n    delta += storedDelta;\n  }\n  const fn = panFunctions[scale.type] || panFunctions.default;\n  if (callback(fn, [scale, delta, limits])) {\n    // The scale changed, reset cumulative delta\n    panDelta[scale.id] = 0;\n  } else {\n    // The scale did not change, store cumulative delta\n    panDelta[scale.id] = delta;\n  }\n}\n\nfunction pan(chart, delta, enabledScales, transition = 'none') {\n  const {x = 0, y = 0} = typeof delta === 'number' ? {x: delta, y: delta} : delta;\n  const state = getState(chart);\n  const {options: {pan: panOptions, limits}} = state;\n  const {onPan} = panOptions || {};\n\n  storeOriginalScaleLimits(chart, state);\n\n  const xEnabled = x !== 0;\n  const yEnabled = y !== 0;\n\n  each(enabledScales || chart.scales, function(scale) {\n    if (scale.isHorizontal() && xEnabled) {\n      panScale(scale, x, limits, state);\n    } else if (!scale.isHorizontal() && yEnabled) {\n      panScale(scale, y, limits, state);\n    }\n  });\n\n  chart.update(transition);\n\n  callback(onPan, [{chart}]);\n}\n\nfunction getInitialScaleBounds(chart) {\n  const state = getState(chart);\n  storeOriginalScaleLimits(chart, state);\n  const scaleBounds = {};\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min, max} = state.originalScaleLimits[scaleId] || {min: {}, max: {}};\n    scaleBounds[scaleId] = {min: min.scale, max: max.scale};\n  }\n\n  return scaleBounds;\n}\n\nfunction isZoomedOrPanned(chart) {\n  const scaleBounds = getInitialScaleBounds(chart);\n  for (const scaleId of Object.keys(chart.scales)) {\n    const {min: originalMin, max: originalMax} = scaleBounds[scaleId];\n\n    if (originalMin !== undefined && chart.scales[scaleId].min !== originalMin) {\n      return true;\n    }\n\n    if (originalMax !== undefined && chart.scales[scaleId].max !== originalMax) {\n      return true;\n    }\n  }\n\n  return false;\n}\n\nfunction removeHandler(chart, type) {\n  const {handlers} = getState(chart);\n  const handler = handlers[type];\n  if (handler && handler.target) {\n    handler.target.removeEventListener(type, handler);\n    delete handlers[type];\n  }\n}\n\nfunction addHandler(chart, target, type, handler) {\n  const {handlers, options} = getState(chart);\n  const oldHandler = handlers[type];\n  if (oldHandler && oldHandler.target === target) {\n    // already attached\n    return;\n  }\n  removeHandler(chart, type);\n  handlers[type] = (event) => handler(chart, event, options);\n  handlers[type].target = target;\n  target.addEventListener(type, handlers[type]);\n}\n\nfunction mouseMove(chart, event) {\n  const state = getState(chart);\n  if (state.dragStart) {\n    state.dragging = true;\n    state.dragEnd = event;\n    chart.update('none');\n  }\n}\n\nfunction keyDown(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart || event.key !== 'Escape') {\n    return;\n  }\n\n  removeHandler(chart, 'keydown');\n  state.dragging = false;\n  state.dragStart = state.dragEnd = null;\n  chart.update('none');\n}\n\nfunction zoomStart(chart, event, zoomOptions) {\n  const {onZoomStart, onZoomRejected} = zoomOptions;\n  if (onZoomStart) {\n    const point = getRelativePosition(event, chart);\n    if (callback(onZoomStart, [{chart, event, point}]) === false) {\n      callback(onZoomRejected, [{chart, event}]);\n      return false;\n    }\n  }\n}\n\nfunction mouseDown(chart, event) {\n  const state = getState(chart);\n  const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n  if (\n    event.button !== 0 ||\n    keyPressed(getModifierKey(panOptions), event) ||\n    keyNotPressed(getModifierKey(zoomOptions.drag), event)\n  ) {\n    return callback(zoomOptions.onZoomRejected, [{chart, event}]);\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n  state.dragStart = event;\n\n  addHandler(chart, chart.canvas, 'mousemove', mouseMove);\n  addHandler(chart, window.document, 'keydown', keyDown);\n}\n\nfunction computeDragRect(chart, mode, beginPointEvent, endPointEvent) {\n  const xEnabled = directionEnabled(mode, 'x', chart);\n  const yEnabled = directionEnabled(mode, 'y', chart);\n  let {top, left, right, bottom, width: chartWidth, height: chartHeight} = chart.chartArea;\n\n  const beginPoint = getRelativePosition(beginPointEvent, chart);\n  const endPoint = getRelativePosition(endPointEvent, chart);\n\n  if (xEnabled) {\n    left = Math.min(beginPoint.x, endPoint.x);\n    right = Math.max(beginPoint.x, endPoint.x);\n  }\n\n  if (yEnabled) {\n    top = Math.min(beginPoint.y, endPoint.y);\n    bottom = Math.max(beginPoint.y, endPoint.y);\n  }\n  const width = right - left;\n  const height = bottom - top;\n\n  return {\n    left,\n    top,\n    right,\n    bottom,\n    width,\n    height,\n    zoomX: xEnabled && width ? 1 + ((chartWidth - width) / chartWidth) : 1,\n    zoomY: yEnabled && height ? 1 + ((chartHeight - height) / chartHeight) : 1\n  };\n}\n\nfunction mouseUp(chart, event) {\n  const state = getState(chart);\n  if (!state.dragStart) {\n    return;\n  }\n\n  removeHandler(chart, 'mousemove');\n  const {mode, onZoomComplete, drag: {threshold = 0}} = state.options.zoom;\n  const rect = computeDragRect(chart, mode, state.dragStart, event);\n  const distanceX = directionEnabled(mode, 'x', chart) ? rect.width : 0;\n  const distanceY = directionEnabled(mode, 'y', chart) ? rect.height : 0;\n  const distance = Math.sqrt(distanceX * distanceX + distanceY * distanceY);\n\n  // Remove drag start and end before chart update to stop drawing selected area\n  state.dragStart = state.dragEnd = null;\n\n  if (distance <= threshold) {\n    state.dragging = false;\n    chart.update('none');\n    return;\n  }\n\n  zoomRect(chart, {x: rect.left, y: rect.top}, {x: rect.right, y: rect.bottom}, 'zoom');\n\n  setTimeout(() => (state.dragging = false), 500);\n  callback(onZoomComplete, [{chart}]);\n}\n\nfunction wheelPreconditions(chart, event, zoomOptions) {\n  // Before preventDefault, check if the modifier key required and pressed\n  if (keyNotPressed(getModifierKey(zoomOptions.wheel), event)) {\n    callback(zoomOptions.onZoomRejected, [{chart, event}]);\n    return;\n  }\n\n  if (zoomStart(chart, event, zoomOptions) === false) {\n    return;\n  }\n\n  // Prevent the event from triggering the default behavior (e.g. content scrolling).\n  if (event.cancelable) {\n    event.preventDefault();\n  }\n\n  // Firefox always fires the wheel event twice:\n  // First without the delta and right after that once with the delta properties.\n  if (event.deltaY === undefined) {\n    return;\n  }\n  return true;\n}\n\nfunction wheel(chart, event) {\n  const {handlers: {onZoomComplete}, options: {zoom: zoomOptions}} = getState(chart);\n\n  if (!wheelPreconditions(chart, event, zoomOptions)) {\n    return;\n  }\n\n  const rect = event.target.getBoundingClientRect();\n  const speed = 1 + (event.deltaY >= 0 ? -zoomOptions.wheel.speed : zoomOptions.wheel.speed);\n  const amount = {\n    x: speed,\n    y: speed,\n    focalPoint: {\n      x: event.clientX - rect.left,\n      y: event.clientY - rect.top\n    }\n  };\n\n  zoom(chart, amount);\n\n  if (onZoomComplete) {\n    onZoomComplete();\n  }\n}\n\nfunction addDebouncedHandler(chart, name, handler, delay) {\n  if (handler) {\n    getState(chart).handlers[name] = debounce(() => callback(handler, [{chart}]), delay);\n  }\n}\n\nfunction addListeners(chart, options) {\n  const canvas = chart.canvas;\n  const {wheel: wheelOptions, drag: dragOptions, onZoomComplete} = options.zoom;\n\n  // Install listeners. Do this dynamically based on options so that we can turn zoom on and off\n  // We also want to make sure listeners aren't always on. E.g. if you're scrolling down a page\n  // and the mouse goes over a chart you don't want it intercepted unless the plugin is enabled\n  if (wheelOptions.enabled) {\n    addHandler(chart, canvas, 'wheel', wheel);\n    addDebouncedHandler(chart, 'onZoomComplete', onZoomComplete, 250);\n  } else {\n    removeHandler(chart, 'wheel');\n  }\n  if (dragOptions.enabled) {\n    addHandler(chart, canvas, 'mousedown', mouseDown);\n    addHandler(chart, canvas.ownerDocument, 'mouseup', mouseUp);\n  } else {\n    removeHandler(chart, 'mousedown');\n    removeHandler(chart, 'mousemove');\n    removeHandler(chart, 'mouseup');\n    removeHandler(chart, 'keydown');\n  }\n}\n\nfunction removeListeners(chart) {\n  removeHandler(chart, 'mousedown');\n  removeHandler(chart, 'mousemove');\n  removeHandler(chart, 'mouseup');\n  removeHandler(chart, 'wheel');\n  removeHandler(chart, 'click');\n  removeHandler(chart, 'keydown');\n}\n\nfunction createEnabler(chart, state) {\n  return function(recognizer, event) {\n    const {pan: panOptions, zoom: zoomOptions = {}} = state.options;\n    if (!panOptions || !panOptions.enabled) {\n      return false;\n    }\n    const srcEvent = event && event.srcEvent;\n    if (!srcEvent) { // Sometimes Hammer queries this with a null event.\n      return true;\n    }\n    if (!state.panning && event.pointerType === 'mouse' && (\n      keyNotPressed(getModifierKey(panOptions), srcEvent) || keyPressed(getModifierKey(zoomOptions.drag), srcEvent))\n    ) {\n      callback(panOptions.onPanRejected, [{chart, event}]);\n      return false;\n    }\n    return true;\n  };\n}\n\nfunction pinchAxes(p0, p1) {\n  // fingers position difference\n  const pinchX = Math.abs(p0.clientX - p1.clientX);\n  const pinchY = Math.abs(p0.clientY - p1.clientY);\n\n  // diagonal fingers will change both (xy) axes\n  const p = pinchX / pinchY;\n  let x, y;\n  if (p > 0.3 && p < 1.7) {\n    x = y = true;\n  } else if (pinchX > pinchY) {\n    x = true;\n  } else {\n    y = true;\n  }\n  return {x, y};\n}\n\nfunction handlePinch(chart, state, e) {\n  if (state.scale) {\n    const {center, pointers} = e;\n    // Hammer reports the total scaling. We need the incremental amount\n    const zoomPercent = 1 / state.scale * e.scale;\n    const rect = e.target.getBoundingClientRect();\n    const pinch = pinchAxes(pointers[0], pointers[1]);\n    const mode = state.options.zoom.mode;\n    const amount = {\n      x: pinch.x && directionEnabled(mode, 'x', chart) ? zoomPercent : 1,\n      y: pinch.y && directionEnabled(mode, 'y', chart) ? zoomPercent : 1,\n      focalPoint: {\n        x: center.x - rect.left,\n        y: center.y - rect.top\n      }\n    };\n\n    zoom(chart, amount);\n\n    // Keep track of overall scale\n    state.scale = e.scale;\n  }\n}\n\nfunction startPinch(chart, state) {\n  if (state.options.zoom.pinch.enabled) {\n    state.scale = 1;\n  }\n}\n\nfunction endPinch(chart, state, e) {\n  if (state.scale) {\n    handlePinch(chart, state, e);\n    state.scale = null; // reset\n    callback(state.options.zoom.onZoomComplete, [{chart}]);\n  }\n}\n\nfunction handlePan(chart, state, e) {\n  const delta = state.delta;\n  if (delta) {\n    state.panning = true;\n    pan(chart, {x: e.deltaX - delta.x, y: e.deltaY - delta.y}, state.panScales);\n    state.delta = {x: e.deltaX, y: e.deltaY};\n  }\n}\n\nfunction startPan(chart, state, event) {\n  const {enabled, onPanStart, onPanRejected} = state.options.pan;\n  if (!enabled) {\n    return;\n  }\n  const rect = event.target.getBoundingClientRect();\n  const point = {\n    x: event.center.x - rect.left,\n    y: event.center.y - rect.top\n  };\n\n  if (callback(onPanStart, [{chart, event, point}]) === false) {\n    return callback(onPanRejected, [{chart, event}]);\n  }\n\n  state.panScales = getEnabledScalesByPoint(state.options.pan, point, chart);\n  state.delta = {x: 0, y: 0};\n  clearTimeout(state.panEndTimeout);\n  handlePan(chart, state, event);\n}\n\nfunction endPan(chart, state) {\n  state.delta = null;\n  if (state.panning) {\n    state.panEndTimeout = setTimeout(() => (state.panning = false), 500);\n    callback(state.options.pan.onPanComplete, [{chart}]);\n  }\n}\n\nconst hammers = new WeakMap();\nfunction startHammer(chart, options) {\n  const state = getState(chart);\n  const canvas = chart.canvas;\n  const {pan: panOptions, zoom: zoomOptions} = options;\n\n  const mc = new Hammer.Manager(canvas);\n  if (zoomOptions && zoomOptions.pinch.enabled) {\n    mc.add(new Hammer.Pinch());\n    mc.on('pinchstart', () => startPinch(chart, state));\n    mc.on('pinch', (e) => handlePinch(chart, state, e));\n    mc.on('pinchend', (e) => endPinch(chart, state, e));\n  }\n\n  if (panOptions && panOptions.enabled) {\n    mc.add(new Hammer.Pan({\n      threshold: panOptions.threshold,\n      enable: createEnabler(chart, state)\n    }));\n    mc.on('panstart', (e) => startPan(chart, state, e));\n    mc.on('panmove', (e) => handlePan(chart, state, e));\n    mc.on('panend', () => endPan(chart, state));\n  }\n\n  hammers.set(chart, mc);\n}\n\nfunction stopHammer(chart) {\n  const mc = hammers.get(chart);\n  if (mc) {\n    mc.remove('pinchstart');\n    mc.remove('pinch');\n    mc.remove('pinchend');\n    mc.remove('panstart');\n    mc.remove('pan');\n    mc.remove('panend');\n    mc.destroy();\n    hammers.delete(chart);\n  }\n}\n\nvar version = \"2.0.1\";\n\nfunction draw(chart, caller, options) {\n  const dragOptions = options.zoom.drag;\n  const {dragStart, dragEnd} = getState(chart);\n\n  if (dragOptions.drawTime !== caller || !dragEnd) {\n    return;\n  }\n  const {left, top, width, height} = computeDragRect(chart, options.zoom.mode, dragStart, dragEnd);\n  const ctx = chart.ctx;\n\n  ctx.save();\n  ctx.beginPath();\n  ctx.fillStyle = dragOptions.backgroundColor || 'rgba(225,225,225,0.3)';\n  ctx.fillRect(left, top, width, height);\n\n  if (dragOptions.borderWidth > 0) {\n    ctx.lineWidth = dragOptions.borderWidth;\n    ctx.strokeStyle = dragOptions.borderColor || 'rgba(225,225,225)';\n    ctx.strokeRect(left, top, width, height);\n  }\n  ctx.restore();\n}\n\nvar plugin = {\n  id: 'zoom',\n\n  version,\n\n  defaults: {\n    pan: {\n      enabled: false,\n      mode: 'xy',\n      threshold: 10,\n      modifierKey: null,\n    },\n    zoom: {\n      wheel: {\n        enabled: false,\n        speed: 0.1,\n        modifierKey: null\n      },\n      drag: {\n        enabled: false,\n        drawTime: 'beforeDatasetsDraw',\n        modifierKey: null\n      },\n      pinch: {\n        enabled: false\n      },\n      mode: 'xy',\n    }\n  },\n\n  start: function(chart, _args, options) {\n    const state = getState(chart);\n    state.options = options;\n\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'enabled')) {\n      console.warn('The option `zoom.enabled` is no longer supported. Please use `zoom.wheel.enabled`, `zoom.drag.enabled`, or `zoom.pinch.enabled`.');\n    }\n    if (Object.prototype.hasOwnProperty.call(options.zoom, 'overScaleMode')\n      || Object.prototype.hasOwnProperty.call(options.pan, 'overScaleMode')) {\n      console.warn('The option `overScaleMode` is deprecated. Please use `scaleMode` instead (and update `mode` as desired).');\n    }\n\n    if (Hammer) {\n      startHammer(chart, options);\n    }\n\n    chart.pan = (delta, panScales, transition) => pan(chart, delta, panScales, transition);\n    chart.zoom = (args, transition) => zoom(chart, args, transition);\n    chart.zoomRect = (p0, p1, transition) => zoomRect(chart, p0, p1, transition);\n    chart.zoomScale = (id, range, transition) => zoomScale(chart, id, range, transition);\n    chart.resetZoom = (transition) => resetZoom(chart, transition);\n    chart.getZoomLevel = () => getZoomLevel(chart);\n    chart.getInitialScaleBounds = () => getInitialScaleBounds(chart);\n    chart.isZoomedOrPanned = () => isZoomedOrPanned(chart);\n  },\n\n  beforeEvent(chart) {\n    const state = getState(chart);\n    if (state.panning || state.dragging) {\n      // cancel any event handling while panning or dragging\n      return false;\n    }\n  },\n\n  beforeUpdate: function(chart, args, options) {\n    const state = getState(chart);\n    state.options = options;\n    addListeners(chart, options);\n  },\n\n  beforeDatasetsDraw(chart, _args, options) {\n    draw(chart, 'beforeDatasetsDraw', options);\n  },\n\n  afterDatasetsDraw(chart, _args, options) {\n    draw(chart, 'afterDatasetsDraw', options);\n  },\n\n  beforeDraw(chart, _args, options) {\n    draw(chart, 'beforeDraw', options);\n  },\n\n  afterDraw(chart, _args, options) {\n    draw(chart, 'afterDraw', options);\n  },\n\n  stop: function(chart) {\n    removeListeners(chart);\n\n    if (Hammer) {\n      stopHammer(chart);\n    }\n    removeState(chart);\n  },\n\n  panFunctions,\n  zoomFunctions,\n  zoomRectFunctions,\n};\n\nexport { plugin as default, pan, resetZoom, zoom, zoomRect, zoomScale };\n",
         "import type { MouseEvent } from 'react';\nimport type {\n  ChartType,\n  ChartData,\n  DefaultDataPoint,\n  ChartDataset,\n  ChartOptions,\n  Chart,\n} from 'chart.js';\n\nimport type { ForwardedRef } from './types.js';\n\nconst defaultDatasetIdKey = 'label';\n\nexport function reforwardRef<T>(ref: ForwardedRef<T>, value: T) {\n  if (typeof ref === 'function') {\n    ref(value);\n  } else if (ref) {\n    ref.current = value;\n  }\n}\n\nexport function setOptions<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(chart: Chart<TType, TData, TLabel>, nextOptions: ChartOptions<TType>) {\n  const options = chart.options;\n\n  if (options && nextOptions) {\n    Object.assign(options, nextOptions);\n  }\n}\n\nexport function setLabels<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextLabels: TLabel[] | undefined\n) {\n  currentData.labels = nextLabels;\n}\n\nexport function setDatasets<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  currentData: ChartData<TType, TData, TLabel>,\n  nextDatasets: ChartDataset<TType, TData>[],\n  datasetIdKey = defaultDatasetIdKey\n) {\n  const addedDatasets: ChartDataset<TType, TData>[] = [];\n\n  currentData.datasets = nextDatasets.map(\n    (nextDataset: Record<string, unknown>) => {\n      // given the new set, find it's current match\n      const currentDataset = currentData.datasets.find(\n        (dataset: Record<string, unknown>) =>\n          dataset[datasetIdKey] === nextDataset[datasetIdKey]\n      );\n\n      // There is no original to update, so simply add new one\n      if (\n        !currentDataset ||\n        !nextDataset.data ||\n        addedDatasets.includes(currentDataset)\n      ) {\n        return { ...nextDataset } as ChartDataset<TType, TData>;\n      }\n\n      addedDatasets.push(currentDataset);\n\n      Object.assign(currentDataset, nextDataset);\n\n      return currentDataset;\n    }\n  );\n}\n\nexport function cloneData<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(data: ChartData<TType, TData, TLabel>, datasetIdKey = defaultDatasetIdKey) {\n  const nextData: ChartData<TType, TData, TLabel> = {\n    labels: [],\n    datasets: [],\n  };\n\n  setLabels(nextData, data.labels);\n  setDatasets(nextData, data.datasets, datasetIdKey);\n\n  return nextData;\n}\n\n/**\n * Get dataset from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getDatasetAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'dataset',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get single dataset element from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'nearest',\n    { intersect: true },\n    false\n  );\n}\n\n/**\n * Get all dataset elements from mouse click event\n * @param chart - Chart.js instance\n * @param event - Mouse click event\n * @returns Dataset\n */\nexport function getElementsAtEvent(\n  chart: Chart,\n  event: MouseEvent<HTMLCanvasElement>\n) {\n  return chart.getElementsAtEventForMode(\n    event.nativeEvent,\n    'index',\n    { intersect: true },\n    false\n  );\n}\n",
         "import React, { useEffect, useRef, forwardRef } from 'react';\nimport { Chart as ChartJS } from 'chart.js';\nimport type { ChartType, DefaultDataPoint } from 'chart.js';\n\nimport type { ForwardedRef, ChartProps, BaseChartComponent } from './types.js';\nimport {\n  reforwardRef,\n  cloneData,\n  setOptions,\n  setLabels,\n  setDatasets,\n} from './utils.js';\n\nfunction ChartComponent<\n  TType extends ChartType = ChartType,\n  TData = DefaultDataPoint<TType>,\n  TLabel = unknown\n>(\n  props: ChartProps<TType, TData, TLabel>,\n  ref: ForwardedRef<ChartJS<TType, TData, TLabel>>\n) {\n  const {\n    height = 150,\n    width = 300,\n    redraw = false,\n    datasetIdKey,\n    type,\n    data,\n    options,\n    plugins = [],\n    fallbackContent,\n    updateMode,\n    ...canvasProps\n  } = props as ChartProps;\n  const canvasRef = useRef<HTMLCanvasElement>(null);\n  const chartRef = useRef<ChartJS | null>();\n\n  const renderChart = () => {\n    if (!canvasRef.current) return;\n\n    chartRef.current = new ChartJS(canvasRef.current, {\n      type,\n      data: cloneData(data, datasetIdKey),\n      options: options && { ...options },\n      plugins,\n    });\n\n    reforwardRef(ref, chartRef.current);\n  };\n\n  const destroyChart = () => {\n    reforwardRef(ref, null);\n\n    if (chartRef.current) {\n      chartRef.current.destroy();\n      chartRef.current = null;\n    }\n  };\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && options) {\n      setOptions(chartRef.current, options);\n    }\n  }, [redraw, options]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current) {\n      setLabels(chartRef.current.config.data, data.labels);\n    }\n  }, [redraw, data.labels]);\n\n  useEffect(() => {\n    if (!redraw && chartRef.current && data.datasets) {\n      setDatasets(chartRef.current.config.data, data.datasets, datasetIdKey);\n    }\n  }, [redraw, data.datasets]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    if (redraw) {\n      destroyChart();\n      setTimeout(renderChart);\n    } else {\n      chartRef.current.update(updateMode);\n    }\n  }, [redraw, options, data.labels, data.datasets, updateMode]);\n\n  useEffect(() => {\n    if (!chartRef.current) return;\n\n    destroyChart();\n    setTimeout(renderChart);\n  }, [type]);\n\n  useEffect(() => {\n    renderChart();\n\n    return () => destroyChart();\n  }, []);\n\n  return (\n    <canvas\n      ref={canvasRef}\n      role='img'\n      height={height}\n      width={width}\n      {...canvasProps}\n    >\n      {fallbackContent}\n    </canvas>\n  );\n}\n\nexport const Chart = forwardRef(ChartComponent) as BaseChartComponent;\n",
         "import React, { forwardRef } from 'react';\nimport {\n  Chart as ChartJS,\n  LineController,\n  BarController,\n  RadarController,\n  DoughnutController,\n  PolarAreaController,\n  BubbleController,\n  PieController,\n  ScatterController,\n} from 'chart.js';\nimport type { ChartType, ChartComponentLike } from 'chart.js';\n\nimport type {\n  ChartProps,\n  ChartJSOrUndefined,\n  TypedChartComponent,\n} from './types.js';\nimport { Chart } from './chart.js';\n\nfunction createTypedChart<T extends ChartType>(\n  type: T,\n  registerables: ChartComponentLike\n) {\n  ChartJS.register(registerables);\n\n  return forwardRef<ChartJSOrUndefined<T>, Omit<ChartProps<T>, 'type'>>(\n    (props, ref) => <Chart {...props} ref={ref} type={type} />\n  ) as TypedChartComponent<T>;\n}\n\nexport const Line = /* #__PURE__ */ createTypedChart('line', LineController);\n\nexport const Bar = /* #__PURE__ */ createTypedChart('bar', BarController);\n\nexport const Radar = /* #__PURE__ */ createTypedChart('radar', RadarController);\n\nexport const Doughnut = /* #__PURE__ */ createTypedChart(\n  'doughnut',\n  DoughnutController\n);\n\nexport const PolarArea = /* #__PURE__ */ createTypedChart(\n  'polarArea',\n  PolarAreaController\n);\n\nexport const Bubble = /* #__PURE__ */ createTypedChart(\n  'bubble',\n  BubbleController\n);\n\nexport const Pie = /* #__PURE__ */ createTypedChart('pie', PieController);\n\nexport const Scatter = /* #__PURE__ */ createTypedChart(\n  'scatter',\n  ScatterController\n);\n",
         "export function createChartData(data, options) {\r\n  const xLabels = Object.keys(data[Object.keys(data)[0]].data)\r\n  const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n    return {\r\n      showLine: options.show_line,\r\n      data: colData.data,\r\n      label: colName,\r\n      lineTension: options.tension,\r\n      cubicInterpolationMode: \"default\",\r\n      spanGaps: options.fill_gaps,\r\n      backgroundColor: colData.color,\r\n      borderColor: colData.color,\r\n      pointRadius: colData.point_radius,\r\n      borderDash: colData.border_dash,\r\n    }\r\n  })\r\n\r\n  return {\r\n    labels: xLabels,\r\n    datasets: datasets,\r\n  }\r\n}\r\n",
-        "import { Chart } from \"chart.js\"\r\nimport millify from \"millify\"\r\n\r\nexport function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    onHover: createHoverOptions(options),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n      tooltip: createTooltipOptions(options, theme),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions(options) {\r\n  return (event, chartElement) => {\r\n    let cursorStyle = \"default\"\r\n    if (chartElement.length > 0) {\r\n      const datasets = event.chart.data.datasets\r\n      const label = datasets[chartElement[0].datasetIndex].label\r\n      cursorStyle = determineCursorStyle(label, options)\r\n    }\r\n    event.native.target.style.cursor = cursorStyle\r\n  }\r\n}\r\n\r\nfunction determineCursorStyle(label, options) {\r\n  if (options.fixed_lines.includes(label)) {\r\n    return \"default\"\r\n  }\r\n  return \"crosshair\"\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"xy\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: Boolean(options.title),\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n      generateLabels: function (chart) {\r\n        const labels =\r\n          Chart.defaults.plugins.legend.labels.generateLabels(chart)\r\n        labels.forEach((label) => {\r\n          if (options.labels.hasOwnProperty(label.text)) {\r\n            label.text = options.labels[label.text]\r\n          }\r\n          if (\r\n            options.labels.hasOwnProperty(label.text.replace(\" (bezier)\", \"\"))\r\n          ) {\r\n            label.text =\r\n              options.labels[label.text.replace(\" (bezier)\", \"\")] + \" (bezier)\"\r\n          }\r\n        })\r\n        return labels\r\n      },\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction formatTickValue(val, index, options) {\r\n  if (options.x_type === \"linear\") {\r\n    return millify(val);\r\n  }\r\n  return this.getLabelForValue(val);\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    ticks: {\r\n      callback: function(val, index) {\r\n        return formatTickValue.call(this, val, index, options);\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.x_label),\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    ticks: {\r\n      callback: function(val, index) {\r\n        return formatTickValue.call(this, val, index, options);\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.y_label),\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n\r\nfunction createTooltipOptions(options, theme) {\r\n  return {\r\n    filter: function (data) {\r\n      const pointRadius = data.dataset.pointRadius\r\n      return pointRadius !== 0\r\n    },\r\n    callbacks: {\r\n      title: function (data) {\r\n        if (data.length === 0) {\r\n          return \"\"\r\n        }\r\n        const label = data[0].dataset.label\r\n        if (options.labels.hasOwnProperty(label)) {\r\n          return `${options.labels[label]}`\r\n        }\r\n        return `${label}`\r\n      },\r\n      label: function (event) {\r\n        const Xvalue = event.parsed.x.toFixed(2)\r\n        const Yvalue = event.parsed.y.toFixed(2)\r\n        return `${Xvalue}, ${Yvalue}`\r\n      },\r\n    },\r\n  }\r\n}\r\n",
-        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\nimport { Line, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass LineChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n      const yAxis = chart.scales.y\r\n      const yValue = this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ] = yValue\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xLabel = this.state.chartData.labels[pointIndex]\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex]\r\n\r\n      this.state.originalData[datasetLabel][\"data\"][xLabel] = yValue\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Line\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default LineChart\r\n",
+        "import { Chart } from \"chart.js\"\r\nimport millify from \"millify\"\r\n\r\nexport function createOptions(options, theme) {\r\n  return {\r\n    responsive: true,\r\n    indexAxis: \"x\",\r\n    animation: {\r\n      duration: 0,\r\n    },\r\n    onHover: createHoverOptions(options),\r\n    plugins: {\r\n      zoom: createZoomOptions(),\r\n      title: createTitleOptions(options),\r\n      legend: createLegendOptions(options),\r\n      tooltip: createTooltipOptions(options, theme),\r\n    },\r\n    scales: createScalesOptions(options, theme),\r\n  }\r\n}\r\n\r\nfunction createHoverOptions(options) {\r\n  return (event, chartElement) => {\r\n    let cursorStyle = \"default\"\r\n    if (chartElement.length > 0) {\r\n      const datasets = event.chart.data.datasets\r\n      const label = datasets[chartElement[0].datasetIndex].label\r\n      cursorStyle = determineCursorStyle(label, options)\r\n    }\r\n    event.native.target.style.cursor = cursorStyle\r\n  }\r\n}\r\n\r\nfunction determineCursorStyle(label, options) {\r\n  if (options.fixed_lines.includes(label)) {\r\n    return \"default\"\r\n  }\r\n  return \"crosshair\"\r\n}\r\n\r\nfunction createZoomOptions() {\r\n  return {\r\n    zoom: {\r\n      wheel: {\r\n        enabled: true,\r\n      },\r\n      mode: \"xy\",\r\n    },\r\n    pan: {\r\n      enabled: true,\r\n    },\r\n    limits: {\r\n      x: { min: \"original\", max: \"original\" },\r\n      y: { min: \"original\", max: \"original\" },\r\n    },\r\n  }\r\n}\r\n\r\nfunction createTitleOptions(options) {\r\n  return {\r\n    display: Boolean(options.title),\r\n    text: options.title,\r\n  }\r\n}\r\n\r\nfunction createLegendOptions(options) {\r\n  return {\r\n    display: options.legend,\r\n    position: options.legend_position,\r\n    align: options.legend_align,\r\n    labels: {\r\n      boxWidth: 16,\r\n      boxHeight: 8,\r\n      padding: 8,\r\n      generateLabels: function (chart) {\r\n        const labels =\r\n          Chart.defaults.plugins.legend.labels.generateLabels(chart)\r\n        labels.forEach((label) => {\r\n          if (options.labels.hasOwnProperty(label.text)) {\r\n            label.text = options.labels[label.text]\r\n          }\r\n          if (\r\n            options.labels.hasOwnProperty(label.text.replace(\" (bezier)\", \"\"))\r\n          ) {\r\n            label.text =\r\n              options.labels[label.text.replace(\" (bezier)\", \"\")] + \" (bezier)\"\r\n          }\r\n        })\r\n        return labels\r\n      },\r\n    },\r\n    onHover: (event, legendItem, legend) => {\r\n      if (legendItem) {\r\n        event.native.target.style.cursor = \"pointer\"\r\n      } else {\r\n        event.native.target.style.cursor = \"default\"\r\n      }\r\n    },\r\n  }\r\n}\r\n\r\nfunction formatTickValue(val, format) {\r\n  if (format) {\r\n    return millify(val)\r\n  }\r\n  return this.getLabelForValue(val)\r\n}\r\n\r\nfunction createScalesOptions(options, theme) {\r\n  const xScaleOptions = {\r\n    display: true,\r\n    type: options.x_type,\r\n    ticks: {\r\n      callback: function (val, index) {\r\n        const shouldFormat = options.x_type === \"linear\" && options.x_format\r\n        return formatTickValue.call(this, val, shouldFormat)\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.x_label),\r\n      text: options.x_label,\r\n    },\r\n    grid: {\r\n      display: options.x_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.x_labels) {\r\n    xScaleOptions.min = options.x_labels[0]\r\n    xScaleOptions.max = options.x_labels[options.x_labels.length - 1]\r\n  }\r\n\r\n  const yScaleOptions = {\r\n    display: true,\r\n    type: options.y_type,\r\n    ticks: {\r\n      callback: function (val, index) {\r\n        const shouldFormat = options.y_type === \"linear\" && options.y_format\r\n        return formatTickValue.call(this, val, shouldFormat)\r\n      },\r\n    },\r\n    title: {\r\n      display: Boolean(options.y_label),\r\n      text: options.y_label,\r\n    },\r\n    grid: {\r\n      display: options.y_grid,\r\n      color: theme.fadedText05,\r\n    },\r\n  }\r\n\r\n  if (options.y_labels) {\r\n    yScaleOptions.labels = options.y_labels\r\n    yScaleOptions.min = options.y_labels[0]\r\n    yScaleOptions.max = options.y_labels[options.y_labels.length - 1]\r\n  }\r\n\r\n  return {\r\n    x: xScaleOptions,\r\n    y: yScaleOptions,\r\n  }\r\n}\r\n\r\nfunction createTooltipOptions(options, theme) {\r\n  return {\r\n    filter: function (data) {\r\n      const pointRadius = data.dataset.pointRadius\r\n      return pointRadius !== 0\r\n    },\r\n    callbacks: {\r\n      title: function (data) {\r\n        if (data.length === 0) {\r\n          return \"\"\r\n        }\r\n        const label = data[0].dataset.label\r\n        if (options.labels.hasOwnProperty(label)) {\r\n          return `${options.labels[label]}`\r\n        }\r\n        return `${label}`\r\n      },\r\n      label: function (event) {\r\n        const Xvalue = event.parsed.x.toFixed(2)\r\n        const Yvalue = event.parsed.y.toFixed(2)\r\n        return `${Xvalue}, ${Yvalue}`\r\n      },\r\n    },\r\n  }\r\n}\r\n",
+        "export function calculateNewYValue(position, chartArea, yAxis, type=\"linear\") {\r\n  if (type === \"category\") {\r\n    const categories = yAxis.getLabels()\r\n    const categoryIndex = Math.round(\r\n      map(position.y, chartArea.top, chartArea.bottom, 0, categories.length - 1)\r\n    )\r\n    return categories[categoryIndex]\r\n  } else {\r\n    return map(\r\n      position.y,\r\n      chartArea.bottom,\r\n      chartArea.top,\r\n      yAxis.min,\r\n      yAxis.max\r\n    )\r\n  }\r\n}\r\n\r\nexport function calculateNewXValue(position, chartArea, xAxis, type=\"linear\") {\r\n  if (type === \"category\") {\r\n    const categories = xAxis.getLabels()\r\n    const categoryIndex = Math.round(\r\n      map(position.x, chartArea.left, chartArea.right, 0, categories.length - 1)\r\n    )\r\n    return categories[categoryIndex]\r\n  } else {\r\n    return map(\r\n      position.x,\r\n      chartArea.left,\r\n      chartArea.right,\r\n      xAxis.min,\r\n      xAxis.max\r\n    )\r\n  }\r\n}\r\n\r\nfunction map(value, start1, stop1, start2, stop2) {\r\n  return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n}\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\nimport { Line, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\nimport { calculateNewYValue } from \"../Utils/handlers\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass LineChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n      const yAxis = chart.scales.y\r\n      const yValue = calculateNewYValue(position, chartArea, yAxis)\r\n      const pointIndex = this.state.activePoint.index\r\n      const xLabel = this.state.chartData.labels[pointIndex]\r\n\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        xLabel\r\n      ] = yValue\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xLabel = this.state.chartData.labels[pointIndex]\r\n      const yValue = chart.data.datasets[datasetIndex].data[xLabel]\r\n\r\n      this.state.originalData[datasetLabel][\"data\"][xLabel] = yValue\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n    }\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Line\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default LineChart\r\n",
         "export function createChartData(data, options) {\r\n  const xLabels = options && options.x_labels ? options.x_labels : []\r\n  const datasets = Object.entries(data).map(([colName, colData], index) => {\r\n    const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n    return {\r\n      showLine: options.show_line,\r\n      data: data,\r\n      label: colName,\r\n      lineTension: options.tension,\r\n      cubicInterpolationMode: \"default\",\r\n      spanGaps: options.fill_gaps,\r\n      backgroundColor: colData.color,\r\n      borderColor: colData.color,\r\n      pointRadius: colData.point_radius,\r\n      borderDash: colData.border_dash,\r\n    }\r\n  })\r\n\r\n  return {\r\n    labels: xLabels,\r\n    datasets: datasets,\r\n  }\r\n}\r\n",
-        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass ScatterChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    if (this.props.args.options.y_type === \"category\") {\r\n      const categories = yAxis.getLabels()\r\n      const categoryIndex = Math.round(\r\n        this.map(\r\n          position.y,\r\n          chartArea.top,\r\n          chartArea.bottom,\r\n          0,\r\n          categories.length - 1\r\n        )\r\n      )\r\n      return categories[categoryIndex]\r\n    } else {\r\n      return this.map(\r\n        position.y,\r\n        chartArea.bottom,\r\n        chartArea.top,\r\n        yAxis.min,\r\n        yAxis.max\r\n      )\r\n    }\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    if (this.props.args.options.x_type === \"category\") {\r\n      const categories = xAxis.getLabels()\r\n      const categoryIndex = Math.round(\r\n        this.map(\r\n          position.x,\r\n          chartArea.left,\r\n          chartArea.right,\r\n          0,\r\n          categories.length - 1\r\n        )\r\n      )\r\n      return categories[categoryIndex]\r\n    } else {\r\n      return this.map(\r\n        position.x,\r\n        chartArea.left,\r\n        chartArea.right,\r\n        xAxis.min,\r\n        xAxis.max\r\n      )\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].y = newYValue\r\n\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].x = newXValue\r\n\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n      this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n      this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default ScatterChart\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport { createChartData } from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\nimport { calculateNewXValue, calculateNewYValue } from \"../Utils/handlers\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass ScatterChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      chartData: createChartData(props.args.data, props.args.options.colors),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        chartData: createChartData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const datasetLabel =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex].label\r\n      if (\r\n        this.props.args.options.fixed_lines &&\r\n        this.props.args.options.fixed_lines.includes(datasetLabel)\r\n      ) {\r\n        // This line is fixed, so don't allow it to be moved\r\n        return\r\n      }\r\n      this.setState({ activePoint: points[0] })\r\n      this.togglePan(false)\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const position = getRelativePosition(event, this.chartRef.current)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y,\r\n        this.props.args.options.y_type\r\n      )\r\n\r\n      const newXValue = calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x,\r\n        this.props.args.options.x_type\r\n      )\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].y = newYValue\r\n\r\n      chart.data.datasets[this.state.activePoint.datasetIndex].data[\r\n        this.state.activePoint.index\r\n      ].x = newXValue\r\n\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const datasetIndex = this.state.activePoint.datasetIndex\r\n      const pointIndex = this.state.activePoint.index\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n      this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n      this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n      Streamlit.setComponentValue(this.state.originalData)\r\n\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={this.state.chartData}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default ScatterChart\r\n",
         "import { Bezier } from \"./bezier.js\";\n\n// math-inlining.\nconst { abs, cos, sin, acos, atan2, sqrt, pow } = Math;\n\n// cube root function yielding real roots\nfunction crt(v) {\n  return v < 0 ? -pow(-v, 1 / 3) : pow(v, 1 / 3);\n}\n\n// trig constants\nconst pi = Math.PI,\n  tau = 2 * pi,\n  quart = pi / 2,\n  // float precision significant decimal\n  epsilon = 0.000001,\n  // extremas used in bbox calculation and similar algorithms\n  nMax = Number.MAX_SAFE_INTEGER || 9007199254740991,\n  nMin = Number.MIN_SAFE_INTEGER || -9007199254740991,\n  // a zero coordinate, which is surprisingly useful\n  ZERO = { x: 0, y: 0, z: 0 };\n\n// Bezier utility functions\nconst utils = {\n  // Legendre-Gauss abscissae with n=24 (x_i values, defined at i=n as the roots of the nth order Legendre polynomial Pn(x))\n  Tvalues: [\n    -0.0640568928626056260850430826247450385909,\n    0.0640568928626056260850430826247450385909,\n    -0.1911188674736163091586398207570696318404,\n    0.1911188674736163091586398207570696318404,\n    -0.3150426796961633743867932913198102407864,\n    0.3150426796961633743867932913198102407864,\n    -0.4337935076260451384870842319133497124524,\n    0.4337935076260451384870842319133497124524,\n    -0.5454214713888395356583756172183723700107,\n    0.5454214713888395356583756172183723700107,\n    -0.6480936519369755692524957869107476266696,\n    0.6480936519369755692524957869107476266696,\n    -0.7401241915785543642438281030999784255232,\n    0.7401241915785543642438281030999784255232,\n    -0.8200019859739029219539498726697452080761,\n    0.8200019859739029219539498726697452080761,\n    -0.8864155270044010342131543419821967550873,\n    0.8864155270044010342131543419821967550873,\n    -0.9382745520027327585236490017087214496548,\n    0.9382745520027327585236490017087214496548,\n    -0.9747285559713094981983919930081690617411,\n    0.9747285559713094981983919930081690617411,\n    -0.9951872199970213601799974097007368118745,\n    0.9951872199970213601799974097007368118745,\n  ],\n\n  // Legendre-Gauss weights with n=24 (w_i values, defined by a function linked to in the Bezier primer article)\n  Cvalues: [\n    0.1279381953467521569740561652246953718517,\n    0.1279381953467521569740561652246953718517,\n    0.1258374563468282961213753825111836887264,\n    0.1258374563468282961213753825111836887264,\n    0.121670472927803391204463153476262425607,\n    0.121670472927803391204463153476262425607,\n    0.1155056680537256013533444839067835598622,\n    0.1155056680537256013533444839067835598622,\n    0.1074442701159656347825773424466062227946,\n    0.1074442701159656347825773424466062227946,\n    0.0976186521041138882698806644642471544279,\n    0.0976186521041138882698806644642471544279,\n    0.086190161531953275917185202983742667185,\n    0.086190161531953275917185202983742667185,\n    0.0733464814110803057340336152531165181193,\n    0.0733464814110803057340336152531165181193,\n    0.0592985849154367807463677585001085845412,\n    0.0592985849154367807463677585001085845412,\n    0.0442774388174198061686027482113382288593,\n    0.0442774388174198061686027482113382288593,\n    0.0285313886289336631813078159518782864491,\n    0.0285313886289336631813078159518782864491,\n    0.0123412297999871995468056670700372915759,\n    0.0123412297999871995468056670700372915759,\n  ],\n\n  arcfn: function (t, derivativeFn) {\n    const d = derivativeFn(t);\n    let l = d.x * d.x + d.y * d.y;\n    if (typeof d.z !== \"undefined\") {\n      l += d.z * d.z;\n    }\n    return sqrt(l);\n  },\n\n  compute: function (t, points, _3d) {\n    // shortcuts\n    if (t === 0) {\n      points[0].t = 0;\n      return points[0];\n    }\n\n    const order = points.length - 1;\n\n    if (t === 1) {\n      points[order].t = 1;\n      return points[order];\n    }\n\n    const mt = 1 - t;\n    let p = points;\n\n    // constant?\n    if (order === 0) {\n      points[0].t = t;\n      return points[0];\n    }\n\n    // linear?\n    if (order === 1) {\n      const ret = {\n        x: mt * p[0].x + t * p[1].x,\n        y: mt * p[0].y + t * p[1].y,\n        t: t,\n      };\n      if (_3d) {\n        ret.z = mt * p[0].z + t * p[1].z;\n      }\n      return ret;\n    }\n\n    // quadratic/cubic curve?\n    if (order < 4) {\n      let mt2 = mt * mt,\n        t2 = t * t,\n        a,\n        b,\n        c,\n        d = 0;\n      if (order === 2) {\n        p = [p[0], p[1], p[2], ZERO];\n        a = mt2;\n        b = mt * t * 2;\n        c = t2;\n      } else if (order === 3) {\n        a = mt2 * mt;\n        b = mt2 * t * 3;\n        c = mt * t2 * 3;\n        d = t * t2;\n      }\n      const ret = {\n        x: a * p[0].x + b * p[1].x + c * p[2].x + d * p[3].x,\n        y: a * p[0].y + b * p[1].y + c * p[2].y + d * p[3].y,\n        t: t,\n      };\n      if (_3d) {\n        ret.z = a * p[0].z + b * p[1].z + c * p[2].z + d * p[3].z;\n      }\n      return ret;\n    }\n\n    // higher order curves: use de Casteljau's computation\n    const dCpts = JSON.parse(JSON.stringify(points));\n    while (dCpts.length > 1) {\n      for (let i = 0; i < dCpts.length - 1; i++) {\n        dCpts[i] = {\n          x: dCpts[i].x + (dCpts[i + 1].x - dCpts[i].x) * t,\n          y: dCpts[i].y + (dCpts[i + 1].y - dCpts[i].y) * t,\n        };\n        if (typeof dCpts[i].z !== \"undefined\") {\n          dCpts[i].z = dCpts[i].z + (dCpts[i + 1].z - dCpts[i].z) * t;\n        }\n      }\n      dCpts.splice(dCpts.length - 1, 1);\n    }\n    dCpts[0].t = t;\n    return dCpts[0];\n  },\n\n  computeWithRatios: function (t, points, ratios, _3d) {\n    const mt = 1 - t,\n      r = ratios,\n      p = points;\n\n    let f1 = r[0],\n      f2 = r[1],\n      f3 = r[2],\n      f4 = r[3],\n      d;\n\n    // spec for linear\n    f1 *= mt;\n    f2 *= t;\n\n    if (p.length === 2) {\n      d = f1 + f2;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y) / d,\n        z: !_3d ? false : (f1 * p[0].z + f2 * p[1].z) / d,\n        t: t,\n      };\n    }\n\n    // upgrade to quadratic\n    f1 *= mt;\n    f2 *= 2 * mt;\n    f3 *= t * t;\n\n    if (p.length === 3) {\n      d = f1 + f2 + f3;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x + f3 * p[2].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y + f3 * p[2].y) / d,\n        z: !_3d ? false : (f1 * p[0].z + f2 * p[1].z + f3 * p[2].z) / d,\n        t: t,\n      };\n    }\n\n    // upgrade to cubic\n    f1 *= mt;\n    f2 *= 1.5 * mt;\n    f3 *= 3 * mt;\n    f4 *= t * t * t;\n\n    if (p.length === 4) {\n      d = f1 + f2 + f3 + f4;\n      return {\n        x: (f1 * p[0].x + f2 * p[1].x + f3 * p[2].x + f4 * p[3].x) / d,\n        y: (f1 * p[0].y + f2 * p[1].y + f3 * p[2].y + f4 * p[3].y) / d,\n        z: !_3d\n          ? false\n          : (f1 * p[0].z + f2 * p[1].z + f3 * p[2].z + f4 * p[3].z) / d,\n        t: t,\n      };\n    }\n  },\n\n  derive: function (points, _3d) {\n    const dpoints = [];\n    for (let p = points, d = p.length, c = d - 1; d > 1; d--, c--) {\n      const list = [];\n      for (let j = 0, dpt; j < c; j++) {\n        dpt = {\n          x: c * (p[j + 1].x - p[j].x),\n          y: c * (p[j + 1].y - p[j].y),\n        };\n        if (_3d) {\n          dpt.z = c * (p[j + 1].z - p[j].z);\n        }\n        list.push(dpt);\n      }\n      dpoints.push(list);\n      p = list;\n    }\n    return dpoints;\n  },\n\n  between: function (v, m, M) {\n    return (\n      (m <= v && v <= M) ||\n      utils.approximately(v, m) ||\n      utils.approximately(v, M)\n    );\n  },\n\n  approximately: function (a, b, precision) {\n    return abs(a - b) <= (precision || epsilon);\n  },\n\n  length: function (derivativeFn) {\n    const z = 0.5,\n      len = utils.Tvalues.length;\n\n    let sum = 0;\n\n    for (let i = 0, t; i < len; i++) {\n      t = z * utils.Tvalues[i] + z;\n      sum += utils.Cvalues[i] * utils.arcfn(t, derivativeFn);\n    }\n    return z * sum;\n  },\n\n  map: function (v, ds, de, ts, te) {\n    const d1 = de - ds,\n      d2 = te - ts,\n      v2 = v - ds,\n      r = v2 / d1;\n    return ts + d2 * r;\n  },\n\n  lerp: function (r, v1, v2) {\n    const ret = {\n      x: v1.x + r * (v2.x - v1.x),\n      y: v1.y + r * (v2.y - v1.y),\n    };\n    if (v1.z !== undefined && v2.z !== undefined) {\n      ret.z = v1.z + r * (v2.z - v1.z);\n    }\n    return ret;\n  },\n\n  pointToString: function (p) {\n    let s = p.x + \"/\" + p.y;\n    if (typeof p.z !== \"undefined\") {\n      s += \"/\" + p.z;\n    }\n    return s;\n  },\n\n  pointsToString: function (points) {\n    return \"[\" + points.map(utils.pointToString).join(\", \") + \"]\";\n  },\n\n  copy: function (obj) {\n    return JSON.parse(JSON.stringify(obj));\n  },\n\n  angle: function (o, v1, v2) {\n    const dx1 = v1.x - o.x,\n      dy1 = v1.y - o.y,\n      dx2 = v2.x - o.x,\n      dy2 = v2.y - o.y,\n      cross = dx1 * dy2 - dy1 * dx2,\n      dot = dx1 * dx2 + dy1 * dy2;\n    return atan2(cross, dot);\n  },\n\n  // round as string, to avoid rounding errors\n  round: function (v, d) {\n    const s = \"\" + v;\n    const pos = s.indexOf(\".\");\n    return parseFloat(s.substring(0, pos + 1 + d));\n  },\n\n  dist: function (p1, p2) {\n    const dx = p1.x - p2.x,\n      dy = p1.y - p2.y;\n    return sqrt(dx * dx + dy * dy);\n  },\n\n  closest: function (LUT, point) {\n    let mdist = pow(2, 63),\n      mpos,\n      d;\n    LUT.forEach(function (p, idx) {\n      d = utils.dist(point, p);\n      if (d < mdist) {\n        mdist = d;\n        mpos = idx;\n      }\n    });\n    return { mdist: mdist, mpos: mpos };\n  },\n\n  abcratio: function (t, n) {\n    // see ratio(t) note on http://pomax.github.io/bezierinfo/#abc\n    if (n !== 2 && n !== 3) {\n      return false;\n    }\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    } else if (t === 0 || t === 1) {\n      return t;\n    }\n    const bottom = pow(t, n) + pow(1 - t, n),\n      top = bottom - 1;\n    return abs(top / bottom);\n  },\n\n  projectionratio: function (t, n) {\n    // see u(t) note on http://pomax.github.io/bezierinfo/#abc\n    if (n !== 2 && n !== 3) {\n      return false;\n    }\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    } else if (t === 0 || t === 1) {\n      return t;\n    }\n    const top = pow(1 - t, n),\n      bottom = pow(t, n) + top;\n    return top / bottom;\n  },\n\n  lli8: function (x1, y1, x2, y2, x3, y3, x4, y4) {\n    const nx =\n        (x1 * y2 - y1 * x2) * (x3 - x4) - (x1 - x2) * (x3 * y4 - y3 * x4),\n      ny = (x1 * y2 - y1 * x2) * (y3 - y4) - (y1 - y2) * (x3 * y4 - y3 * x4),\n      d = (x1 - x2) * (y3 - y4) - (y1 - y2) * (x3 - x4);\n    if (d == 0) {\n      return false;\n    }\n    return { x: nx / d, y: ny / d };\n  },\n\n  lli4: function (p1, p2, p3, p4) {\n    const x1 = p1.x,\n      y1 = p1.y,\n      x2 = p2.x,\n      y2 = p2.y,\n      x3 = p3.x,\n      y3 = p3.y,\n      x4 = p4.x,\n      y4 = p4.y;\n    return utils.lli8(x1, y1, x2, y2, x3, y3, x4, y4);\n  },\n\n  lli: function (v1, v2) {\n    return utils.lli4(v1, v1.c, v2, v2.c);\n  },\n\n  makeline: function (p1, p2) {\n    return new Bezier(\n      p1.x,\n      p1.y,\n      (p1.x + p2.x) / 2,\n      (p1.y + p2.y) / 2,\n      p2.x,\n      p2.y\n    );\n  },\n\n  findbbox: function (sections) {\n    let mx = nMax,\n      my = nMax,\n      MX = nMin,\n      MY = nMin;\n    sections.forEach(function (s) {\n      const bbox = s.bbox();\n      if (mx > bbox.x.min) mx = bbox.x.min;\n      if (my > bbox.y.min) my = bbox.y.min;\n      if (MX < bbox.x.max) MX = bbox.x.max;\n      if (MY < bbox.y.max) MY = bbox.y.max;\n    });\n    return {\n      x: { min: mx, mid: (mx + MX) / 2, max: MX, size: MX - mx },\n      y: { min: my, mid: (my + MY) / 2, max: MY, size: MY - my },\n    };\n  },\n\n  shapeintersections: function (\n    s1,\n    bbox1,\n    s2,\n    bbox2,\n    curveIntersectionThreshold\n  ) {\n    if (!utils.bboxoverlap(bbox1, bbox2)) return [];\n    const intersections = [];\n    const a1 = [s1.startcap, s1.forward, s1.back, s1.endcap];\n    const a2 = [s2.startcap, s2.forward, s2.back, s2.endcap];\n    a1.forEach(function (l1) {\n      if (l1.virtual) return;\n      a2.forEach(function (l2) {\n        if (l2.virtual) return;\n        const iss = l1.intersects(l2, curveIntersectionThreshold);\n        if (iss.length > 0) {\n          iss.c1 = l1;\n          iss.c2 = l2;\n          iss.s1 = s1;\n          iss.s2 = s2;\n          intersections.push(iss);\n        }\n      });\n    });\n    return intersections;\n  },\n\n  makeshape: function (forward, back, curveIntersectionThreshold) {\n    const bpl = back.points.length;\n    const fpl = forward.points.length;\n    const start = utils.makeline(back.points[bpl - 1], forward.points[0]);\n    const end = utils.makeline(forward.points[fpl - 1], back.points[0]);\n    const shape = {\n      startcap: start,\n      forward: forward,\n      back: back,\n      endcap: end,\n      bbox: utils.findbbox([start, forward, back, end]),\n    };\n    shape.intersections = function (s2) {\n      return utils.shapeintersections(\n        shape,\n        shape.bbox,\n        s2,\n        s2.bbox,\n        curveIntersectionThreshold\n      );\n    };\n    return shape;\n  },\n\n  getminmax: function (curve, d, list) {\n    if (!list) return { min: 0, max: 0 };\n    let min = nMax,\n      max = nMin,\n      t,\n      c;\n    if (list.indexOf(0) === -1) {\n      list = [0].concat(list);\n    }\n    if (list.indexOf(1) === -1) {\n      list.push(1);\n    }\n    for (let i = 0, len = list.length; i < len; i++) {\n      t = list[i];\n      c = curve.get(t);\n      if (c[d] < min) {\n        min = c[d];\n      }\n      if (c[d] > max) {\n        max = c[d];\n      }\n    }\n    return { min: min, mid: (min + max) / 2, max: max, size: max - min };\n  },\n\n  align: function (points, line) {\n    const tx = line.p1.x,\n      ty = line.p1.y,\n      a = -atan2(line.p2.y - ty, line.p2.x - tx),\n      d = function (v) {\n        return {\n          x: (v.x - tx) * cos(a) - (v.y - ty) * sin(a),\n          y: (v.x - tx) * sin(a) + (v.y - ty) * cos(a),\n        };\n      };\n    return points.map(d);\n  },\n\n  roots: function (points, line) {\n    line = line || { p1: { x: 0, y: 0 }, p2: { x: 1, y: 0 } };\n\n    const order = points.length - 1;\n    const aligned = utils.align(points, line);\n    const reduce = function (t) {\n      return 0 <= t && t <= 1;\n    };\n\n    if (order === 2) {\n      const a = aligned[0].y,\n        b = aligned[1].y,\n        c = aligned[2].y,\n        d = a - 2 * b + c;\n      if (d !== 0) {\n        const m1 = -sqrt(b * b - a * c),\n          m2 = -a + b,\n          v1 = -(m1 + m2) / d,\n          v2 = -(-m1 + m2) / d;\n        return [v1, v2].filter(reduce);\n      } else if (b !== c && d === 0) {\n        return [(2 * b - c) / (2 * b - 2 * c)].filter(reduce);\n      }\n      return [];\n    }\n\n    // see http://www.trans4mind.com/personal_development/mathematics/polynomials/cubicAlgebra.htm\n    const pa = aligned[0].y,\n      pb = aligned[1].y,\n      pc = aligned[2].y,\n      pd = aligned[3].y;\n\n    let d = -pa + 3 * pb - 3 * pc + pd,\n      a = 3 * pa - 6 * pb + 3 * pc,\n      b = -3 * pa + 3 * pb,\n      c = pa;\n\n    if (utils.approximately(d, 0)) {\n      // this is not a cubic curve.\n      if (utils.approximately(a, 0)) {\n        // in fact, this is not a quadratic curve either.\n        if (utils.approximately(b, 0)) {\n          // in fact in fact, there are no solutions.\n          return [];\n        }\n        // linear solution:\n        return [-c / b].filter(reduce);\n      }\n      // quadratic solution:\n      const q = sqrt(b * b - 4 * a * c),\n        a2 = 2 * a;\n      return [(q - b) / a2, (-b - q) / a2].filter(reduce);\n    }\n\n    // at this point, we know we need a cubic solution:\n\n    a /= d;\n    b /= d;\n    c /= d;\n\n    const p = (3 * b - a * a) / 3,\n      p3 = p / 3,\n      q = (2 * a * a * a - 9 * a * b + 27 * c) / 27,\n      q2 = q / 2,\n      discriminant = q2 * q2 + p3 * p3 * p3;\n\n    let u1, v1, x1, x2, x3;\n    if (discriminant < 0) {\n      const mp3 = -p / 3,\n        mp33 = mp3 * mp3 * mp3,\n        r = sqrt(mp33),\n        t = -q / (2 * r),\n        cosphi = t < -1 ? -1 : t > 1 ? 1 : t,\n        phi = acos(cosphi),\n        crtr = crt(r),\n        t1 = 2 * crtr;\n      x1 = t1 * cos(phi / 3) - a / 3;\n      x2 = t1 * cos((phi + tau) / 3) - a / 3;\n      x3 = t1 * cos((phi + 2 * tau) / 3) - a / 3;\n      return [x1, x2, x3].filter(reduce);\n    } else if (discriminant === 0) {\n      u1 = q2 < 0 ? crt(-q2) : -crt(q2);\n      x1 = 2 * u1 - a / 3;\n      x2 = -u1 - a / 3;\n      return [x1, x2].filter(reduce);\n    } else {\n      const sd = sqrt(discriminant);\n      u1 = crt(-q2 + sd);\n      v1 = crt(q2 + sd);\n      return [u1 - v1 - a / 3].filter(reduce);\n    }\n  },\n\n  droots: function (p) {\n    // quadratic roots are easy\n    if (p.length === 3) {\n      const a = p[0],\n        b = p[1],\n        c = p[2],\n        d = a - 2 * b + c;\n      if (d !== 0) {\n        const m1 = -sqrt(b * b - a * c),\n          m2 = -a + b,\n          v1 = -(m1 + m2) / d,\n          v2 = -(-m1 + m2) / d;\n        return [v1, v2];\n      } else if (b !== c && d === 0) {\n        return [(2 * b - c) / (2 * (b - c))];\n      }\n      return [];\n    }\n\n    // linear roots are even easier\n    if (p.length === 2) {\n      const a = p[0],\n        b = p[1];\n      if (a !== b) {\n        return [a / (a - b)];\n      }\n      return [];\n    }\n\n    return [];\n  },\n\n  curvature: function (t, d1, d2, _3d, kOnly) {\n    let num,\n      dnm,\n      adk,\n      dk,\n      k = 0,\n      r = 0;\n\n    //\n    // We're using the following formula for curvature:\n    //\n    //              x'y\" - y'x\"\n    //   k(t) = ------------------\n    //           (x'\u00b2 + y'\u00b2)^(3/2)\n    //\n    // from https://en.wikipedia.org/wiki/Radius_of_curvature#Definition\n    //\n    // With it corresponding 3D counterpart:\n    //\n    //          sqrt( (y'z\" - y\"z')\u00b2 + (z'x\" - z\"x')\u00b2 + (x'y\" - x\"y')\u00b2)\n    //   k(t) = -------------------------------------------------------\n    //                     (x'\u00b2 + y'\u00b2 + z'\u00b2)^(3/2)\n    //\n\n    const d = utils.compute(t, d1);\n    const dd = utils.compute(t, d2);\n    const qdsum = d.x * d.x + d.y * d.y;\n\n    if (_3d) {\n      num = sqrt(\n        pow(d.y * dd.z - dd.y * d.z, 2) +\n          pow(d.z * dd.x - dd.z * d.x, 2) +\n          pow(d.x * dd.y - dd.x * d.y, 2)\n      );\n      dnm = pow(qdsum + d.z * d.z, 3 / 2);\n    } else {\n      num = d.x * dd.y - d.y * dd.x;\n      dnm = pow(qdsum, 3 / 2);\n    }\n\n    if (num === 0 || dnm === 0) {\n      return { k: 0, r: 0 };\n    }\n\n    k = num / dnm;\n    r = dnm / num;\n\n    // We're also computing the derivative of kappa, because\n    // there is value in knowing the rate of change for the\n    // curvature along the curve. And we're just going to\n    // ballpark it based on an epsilon.\n    if (!kOnly) {\n      // compute k'(t) based on the interval before, and after it,\n      // to at least try to not introduce forward/backward pass bias.\n      const pk = utils.curvature(t - 0.001, d1, d2, _3d, true).k;\n      const nk = utils.curvature(t + 0.001, d1, d2, _3d, true).k;\n      dk = (nk - k + (k - pk)) / 2;\n      adk = (abs(nk - k) + abs(k - pk)) / 2;\n    }\n\n    return { k: k, r: r, dk: dk, adk: adk };\n  },\n\n  inflections: function (points) {\n    if (points.length < 4) return [];\n\n    // FIXME: TODO: add in inflection abstraction for quartic+ curves?\n\n    const p = utils.align(points, { p1: points[0], p2: points.slice(-1)[0] }),\n      a = p[2].x * p[1].y,\n      b = p[3].x * p[1].y,\n      c = p[1].x * p[2].y,\n      d = p[3].x * p[2].y,\n      v1 = 18 * (-3 * a + 2 * b + 3 * c - d),\n      v2 = 18 * (3 * a - b - 3 * c),\n      v3 = 18 * (c - a);\n\n    if (utils.approximately(v1, 0)) {\n      if (!utils.approximately(v2, 0)) {\n        let t = -v3 / v2;\n        if (0 <= t && t <= 1) return [t];\n      }\n      return [];\n    }\n\n    const d2 = 2 * v1;\n\n    if (utils.approximately(d2, 0)) return [];\n\n    const trm = v2 * v2 - 4 * v1 * v3;\n\n    if (trm < 0) return [];\n\n    const sq = Math.sqrt(trm);\n\n    return [(sq - v2) / d2, -(v2 + sq) / d2].filter(function (r) {\n      return 0 <= r && r <= 1;\n    });\n  },\n\n  bboxoverlap: function (b1, b2) {\n    const dims = [\"x\", \"y\"],\n      len = dims.length;\n\n    for (let i = 0, dim, l, t, d; i < len; i++) {\n      dim = dims[i];\n      l = b1[dim].mid;\n      t = b2[dim].mid;\n      d = (b1[dim].size + b2[dim].size) / 2;\n      if (abs(l - t) >= d) return false;\n    }\n    return true;\n  },\n\n  expandbox: function (bbox, _bbox) {\n    if (_bbox.x.min < bbox.x.min) {\n      bbox.x.min = _bbox.x.min;\n    }\n    if (_bbox.y.min < bbox.y.min) {\n      bbox.y.min = _bbox.y.min;\n    }\n    if (_bbox.z && _bbox.z.min < bbox.z.min) {\n      bbox.z.min = _bbox.z.min;\n    }\n    if (_bbox.x.max > bbox.x.max) {\n      bbox.x.max = _bbox.x.max;\n    }\n    if (_bbox.y.max > bbox.y.max) {\n      bbox.y.max = _bbox.y.max;\n    }\n    if (_bbox.z && _bbox.z.max > bbox.z.max) {\n      bbox.z.max = _bbox.z.max;\n    }\n    bbox.x.mid = (bbox.x.min + bbox.x.max) / 2;\n    bbox.y.mid = (bbox.y.min + bbox.y.max) / 2;\n    if (bbox.z) {\n      bbox.z.mid = (bbox.z.min + bbox.z.max) / 2;\n    }\n    bbox.x.size = bbox.x.max - bbox.x.min;\n    bbox.y.size = bbox.y.max - bbox.y.min;\n    if (bbox.z) {\n      bbox.z.size = bbox.z.max - bbox.z.min;\n    }\n  },\n\n  pairiteration: function (c1, c2, curveIntersectionThreshold) {\n    const c1b = c1.bbox(),\n      c2b = c2.bbox(),\n      r = 100000,\n      threshold = curveIntersectionThreshold || 0.5;\n\n    if (\n      c1b.x.size + c1b.y.size < threshold &&\n      c2b.x.size + c2b.y.size < threshold\n    ) {\n      return [\n        (((r * (c1._t1 + c1._t2)) / 2) | 0) / r +\n          \"/\" +\n          (((r * (c2._t1 + c2._t2)) / 2) | 0) / r,\n      ];\n    }\n\n    let cc1 = c1.split(0.5),\n      cc2 = c2.split(0.5),\n      pairs = [\n        { left: cc1.left, right: cc2.left },\n        { left: cc1.left, right: cc2.right },\n        { left: cc1.right, right: cc2.right },\n        { left: cc1.right, right: cc2.left },\n      ];\n\n    pairs = pairs.filter(function (pair) {\n      return utils.bboxoverlap(pair.left.bbox(), pair.right.bbox());\n    });\n\n    let results = [];\n\n    if (pairs.length === 0) return results;\n\n    pairs.forEach(function (pair) {\n      results = results.concat(\n        utils.pairiteration(pair.left, pair.right, threshold)\n      );\n    });\n\n    results = results.filter(function (v, i) {\n      return results.indexOf(v) === i;\n    });\n\n    return results;\n  },\n\n  getccenter: function (p1, p2, p3) {\n    const dx1 = p2.x - p1.x,\n      dy1 = p2.y - p1.y,\n      dx2 = p3.x - p2.x,\n      dy2 = p3.y - p2.y,\n      dx1p = dx1 * cos(quart) - dy1 * sin(quart),\n      dy1p = dx1 * sin(quart) + dy1 * cos(quart),\n      dx2p = dx2 * cos(quart) - dy2 * sin(quart),\n      dy2p = dx2 * sin(quart) + dy2 * cos(quart),\n      // chord midpoints\n      mx1 = (p1.x + p2.x) / 2,\n      my1 = (p1.y + p2.y) / 2,\n      mx2 = (p2.x + p3.x) / 2,\n      my2 = (p2.y + p3.y) / 2,\n      // midpoint offsets\n      mx1n = mx1 + dx1p,\n      my1n = my1 + dy1p,\n      mx2n = mx2 + dx2p,\n      my2n = my2 + dy2p,\n      // intersection of these lines:\n      arc = utils.lli8(mx1, my1, mx1n, my1n, mx2, my2, mx2n, my2n),\n      r = utils.dist(arc, p1);\n\n    // arc start/end values, over mid point:\n    let s = atan2(p1.y - arc.y, p1.x - arc.x),\n      m = atan2(p2.y - arc.y, p2.x - arc.x),\n      e = atan2(p3.y - arc.y, p3.x - arc.x),\n      _;\n\n    // determine arc direction (cw/ccw correction)\n    if (s < e) {\n      // if s<m<e, arc(s, e)\n      // if m<s<e, arc(e, s + tau)\n      // if s<e<m, arc(e, s + tau)\n      if (s > m || m > e) {\n        s += tau;\n      }\n      if (s > e) {\n        _ = e;\n        e = s;\n        s = _;\n      }\n    } else {\n      // if e<m<s, arc(e, s)\n      // if m<e<s, arc(s, e + tau)\n      // if e<s<m, arc(s, e + tau)\n      if (e < m && m < s) {\n        _ = e;\n        e = s;\n        s = _;\n      } else {\n        e += tau;\n      }\n    }\n    // assign and done.\n    arc.s = s;\n    arc.e = e;\n    arc.r = r;\n    return arc;\n  },\n\n  numberSort: function (a, b) {\n    return a - b;\n  },\n};\n\nexport { utils };\n",
         "import { utils } from \"./utils.js\";\n\n/**\n * Poly Bezier\n * @param {[type]} curves [description]\n */\nclass PolyBezier {\n  constructor(curves) {\n    this.curves = [];\n    this._3d = false;\n    if (!!curves) {\n      this.curves = curves;\n      this._3d = this.curves[0]._3d;\n    }\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return (\n      \"[\" +\n      this.curves\n        .map(function (curve) {\n          return utils.pointsToString(curve.points);\n        })\n        .join(\", \") +\n      \"]\"\n    );\n  }\n\n  addCurve(curve) {\n    this.curves.push(curve);\n    this._3d = this._3d || curve._3d;\n  }\n\n  length() {\n    return this.curves\n      .map(function (v) {\n        return v.length();\n      })\n      .reduce(function (a, b) {\n        return a + b;\n      });\n  }\n\n  curve(idx) {\n    return this.curves[idx];\n  }\n\n  bbox() {\n    const c = this.curves;\n    var bbox = c[0].bbox();\n    for (var i = 1; i < c.length; i++) {\n      utils.expandbox(bbox, c[i].bbox());\n    }\n    return bbox;\n  }\n\n  offset(d) {\n    const offset = [];\n    this.curves.forEach(function (v) {\n      offset.push(...v.offset(d));\n    });\n    return new PolyBezier(offset);\n  }\n}\n\nexport { PolyBezier };\n",
         "/**\n  A javascript Bezier curve library by Pomax.\n\n  Based on http://pomax.github.io/bezierinfo\n\n  This code is MIT licensed.\n**/\n\nimport { utils } from \"./utils.js\";\nimport { PolyBezier } from \"./poly-bezier.js\";\n\n// math-inlining.\nconst { abs, min, max, cos, sin, acos, sqrt } = Math;\nconst pi = Math.PI;\n// a zero coordinate, which is surprisingly useful\nconst ZERO = { x: 0, y: 0, z: 0 };\n\n/**\n * Bezier curve constructor.\n *\n * ...docs pending...\n */\nclass Bezier {\n  constructor(coords) {\n    let args =\n      coords && coords.forEach ? coords : Array.from(arguments).slice();\n    let coordlen = false;\n\n    if (typeof args[0] === \"object\") {\n      coordlen = args.length;\n      const newargs = [];\n      args.forEach(function (point) {\n        [\"x\", \"y\", \"z\"].forEach(function (d) {\n          if (typeof point[d] !== \"undefined\") {\n            newargs.push(point[d]);\n          }\n        });\n      });\n      args = newargs;\n    }\n\n    let higher = false;\n    const len = args.length;\n\n    if (coordlen) {\n      if (coordlen > 4) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n        higher = true;\n      }\n    } else {\n      if (len !== 6 && len !== 8 && len !== 9 && len !== 12) {\n        if (arguments.length !== 1) {\n          throw new Error(\n            \"Only new Bezier(point[]) is accepted for 4th and higher order curves\"\n          );\n        }\n      }\n    }\n\n    const _3d = (this._3d =\n      (!higher && (len === 9 || len === 12)) ||\n      (coords && coords[0] && typeof coords[0].z !== \"undefined\"));\n\n    const points = (this.points = []);\n    for (let idx = 0, step = _3d ? 3 : 2; idx < len; idx += step) {\n      var point = {\n        x: args[idx],\n        y: args[idx + 1],\n      };\n      if (_3d) {\n        point.z = args[idx + 2];\n      }\n      points.push(point);\n    }\n    const order = (this.order = points.length - 1);\n\n    const dims = (this.dims = [\"x\", \"y\"]);\n    if (_3d) dims.push(\"z\");\n    this.dimlen = dims.length;\n\n    // is this curve, practically speaking, a straight line?\n    const aligned = utils.align(points, { p1: points[0], p2: points[order] });\n    const baselength = utils.dist(points[0], points[order]);\n    this._linear = aligned.reduce((t, p) => t + abs(p.y), 0) < baselength / 50;\n\n    this._lut = [];\n    this._t1 = 0;\n    this._t2 = 1;\n    this.update();\n  }\n\n  static quadraticFromPoints(p1, p2, p3, t) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    // shortcuts, although they're really dumb\n    if (t === 0) {\n      return new Bezier(p2, p2, p3);\n    }\n    if (t === 1) {\n      return new Bezier(p1, p2, p2);\n    }\n    // real fitting.\n    const abc = Bezier.getABC(2, p1, p2, p3, t);\n    return new Bezier(p1, abc.A, p3);\n  }\n\n  static cubicFromPoints(S, B, E, t, d1) {\n    if (typeof t === \"undefined\") {\n      t = 0.5;\n    }\n    const abc = Bezier.getABC(3, S, B, E, t);\n    if (typeof d1 === \"undefined\") {\n      d1 = utils.dist(B, abc.C);\n    }\n    const d2 = (d1 * (1 - t)) / t;\n\n    const selen = utils.dist(S, E),\n      lx = (E.x - S.x) / selen,\n      ly = (E.y - S.y) / selen,\n      bx1 = d1 * lx,\n      by1 = d1 * ly,\n      bx2 = d2 * lx,\n      by2 = d2 * ly;\n    // derivation of new hull coordinates\n    const e1 = { x: B.x - bx1, y: B.y - by1 },\n      e2 = { x: B.x + bx2, y: B.y + by2 },\n      A = abc.A,\n      v1 = { x: A.x + (e1.x - A.x) / (1 - t), y: A.y + (e1.y - A.y) / (1 - t) },\n      v2 = { x: A.x + (e2.x - A.x) / t, y: A.y + (e2.y - A.y) / t },\n      nc1 = { x: S.x + (v1.x - S.x) / t, y: S.y + (v1.y - S.y) / t },\n      nc2 = {\n        x: E.x + (v2.x - E.x) / (1 - t),\n        y: E.y + (v2.y - E.y) / (1 - t),\n      };\n    // ...done\n    return new Bezier(S, nc1, nc2, E);\n  }\n\n  static getUtils() {\n    return utils;\n  }\n\n  getUtils() {\n    return Bezier.getUtils();\n  }\n\n  static get PolyBezier() {\n    return PolyBezier;\n  }\n\n  valueOf() {\n    return this.toString();\n  }\n\n  toString() {\n    return utils.pointsToString(this.points);\n  }\n\n  toSVG() {\n    if (this._3d) return false;\n    const p = this.points,\n      x = p[0].x,\n      y = p[0].y,\n      s = [\"M\", x, y, this.order === 2 ? \"Q\" : \"C\"];\n    for (let i = 1, last = p.length; i < last; i++) {\n      s.push(p[i].x);\n      s.push(p[i].y);\n    }\n    return s.join(\" \");\n  }\n\n  setRatios(ratios) {\n    if (ratios.length !== this.points.length) {\n      throw new Error(\"incorrect number of ratio values\");\n    }\n    this.ratios = ratios;\n    this._lut = []; //  invalidate any precomputed LUT\n  }\n\n  verify() {\n    const print = this.coordDigest();\n    if (print !== this._print) {\n      this._print = print;\n      this.update();\n    }\n  }\n\n  coordDigest() {\n    return this.points\n      .map(function (c, pos) {\n        return \"\" + pos + c.x + c.y + (c.z ? c.z : 0);\n      })\n      .join(\"\");\n  }\n\n  update() {\n    // invalidate any precomputed LUT\n    this._lut = [];\n    this.dpoints = utils.derive(this.points, this._3d);\n    this.computedirection();\n  }\n\n  computedirection() {\n    const points = this.points;\n    const angle = utils.angle(points[0], points[this.order], points[1]);\n    this.clockwise = angle > 0;\n  }\n\n  length() {\n    return utils.length(this.derivative.bind(this));\n  }\n\n  static getABC(order = 2, S, B, E, t = 0.5) {\n    const u = utils.projectionratio(t, order),\n      um = 1 - u,\n      C = {\n        x: u * S.x + um * E.x,\n        y: u * S.y + um * E.y,\n      },\n      s = utils.abcratio(t, order),\n      A = {\n        x: B.x + (B.x - C.x) / s,\n        y: B.y + (B.y - C.y) / s,\n      };\n    return { A, B, C, S, E };\n  }\n\n  getABC(t, B) {\n    B = B || this.get(t);\n    let S = this.points[0];\n    let E = this.points[this.order];\n    return Bezier.getABC(this.order, S, B, E, t);\n  }\n\n  getLUT(steps) {\n    this.verify();\n    steps = steps || 100;\n    if (this._lut.length === steps + 1) {\n      return this._lut;\n    }\n    this._lut = [];\n    // n steps means n+1 points\n    steps++;\n    this._lut = [];\n    for (let i = 0, p, t; i < steps; i++) {\n      t = i / (steps - 1);\n      p = this.compute(t);\n      p.t = t;\n      this._lut.push(p);\n    }\n    return this._lut;\n  }\n\n  on(point, error) {\n    error = error || 5;\n    const lut = this.getLUT(),\n      hits = [];\n    for (let i = 0, c, t = 0; i < lut.length; i++) {\n      c = lut[i];\n      if (utils.dist(c, point) < error) {\n        hits.push(c);\n        t += i / lut.length;\n      }\n    }\n    if (!hits.length) return false;\n    return (t /= hits.length);\n  }\n\n  project(point) {\n    // step 1: coarse check\n    const LUT = this.getLUT(),\n      l = LUT.length - 1,\n      closest = utils.closest(LUT, point),\n      mpos = closest.mpos,\n      t1 = (mpos - 1) / l,\n      t2 = (mpos + 1) / l,\n      step = 0.1 / l;\n\n    // step 2: fine check\n    let mdist = closest.mdist,\n      t = t1,\n      ft = t,\n      p;\n    mdist += 1;\n    for (let d; t < t2 + step; t += step) {\n      p = this.compute(t);\n      d = utils.dist(point, p);\n      if (d < mdist) {\n        mdist = d;\n        ft = t;\n      }\n    }\n    ft = ft < 0 ? 0 : ft > 1 ? 1 : ft;\n    p = this.compute(ft);\n    p.t = ft;\n    p.d = mdist;\n    return p;\n  }\n\n  get(t) {\n    return this.compute(t);\n  }\n\n  point(idx) {\n    return this.points[idx];\n  }\n\n  compute(t) {\n    if (this.ratios) {\n      return utils.computeWithRatios(t, this.points, this.ratios, this._3d);\n    }\n    return utils.compute(t, this.points, this._3d, this.ratios);\n  }\n\n  raise() {\n    const p = this.points,\n      np = [p[0]],\n      k = p.length;\n    for (let i = 1, pi, pim; i < k; i++) {\n      pi = p[i];\n      pim = p[i - 1];\n      np[i] = {\n        x: ((k - i) / k) * pi.x + (i / k) * pim.x,\n        y: ((k - i) / k) * pi.y + (i / k) * pim.y,\n      };\n    }\n    np[k] = p[k - 1];\n    return new Bezier(np);\n  }\n\n  derivative(t) {\n    return utils.compute(t, this.dpoints[0], this._3d);\n  }\n\n  dderivative(t) {\n    return utils.compute(t, this.dpoints[1], this._3d);\n  }\n\n  align() {\n    let p = this.points;\n    return new Bezier(utils.align(p, { p1: p[0], p2: p[p.length - 1] }));\n  }\n\n  curvature(t) {\n    return utils.curvature(t, this.dpoints[0], this.dpoints[1], this._3d);\n  }\n\n  inflections() {\n    return utils.inflections(this.points);\n  }\n\n  normal(t) {\n    return this._3d ? this.__normal3(t) : this.__normal2(t);\n  }\n\n  __normal2(t) {\n    const d = this.derivative(t);\n    const q = sqrt(d.x * d.x + d.y * d.y);\n    return { t, x: -d.y / q, y: d.x / q };\n  }\n\n  __normal3(t) {\n    // see http://stackoverflow.com/questions/25453159\n    const r1 = this.derivative(t),\n      r2 = this.derivative(t + 0.01),\n      q1 = sqrt(r1.x * r1.x + r1.y * r1.y + r1.z * r1.z),\n      q2 = sqrt(r2.x * r2.x + r2.y * r2.y + r2.z * r2.z);\n    r1.x /= q1;\n    r1.y /= q1;\n    r1.z /= q1;\n    r2.x /= q2;\n    r2.y /= q2;\n    r2.z /= q2;\n    // cross product\n    const c = {\n      x: r2.y * r1.z - r2.z * r1.y,\n      y: r2.z * r1.x - r2.x * r1.z,\n      z: r2.x * r1.y - r2.y * r1.x,\n    };\n    const m = sqrt(c.x * c.x + c.y * c.y + c.z * c.z);\n    c.x /= m;\n    c.y /= m;\n    c.z /= m;\n    // rotation matrix\n    const R = [\n      c.x * c.x,\n      c.x * c.y - c.z,\n      c.x * c.z + c.y,\n      c.x * c.y + c.z,\n      c.y * c.y,\n      c.y * c.z - c.x,\n      c.x * c.z - c.y,\n      c.y * c.z + c.x,\n      c.z * c.z,\n    ];\n    // normal vector:\n    const n = {\n      t,\n      x: R[0] * r1.x + R[1] * r1.y + R[2] * r1.z,\n      y: R[3] * r1.x + R[4] * r1.y + R[5] * r1.z,\n      z: R[6] * r1.x + R[7] * r1.y + R[8] * r1.z,\n    };\n    return n;\n  }\n\n  hull(t) {\n    let p = this.points,\n      _p = [],\n      q = [],\n      idx = 0;\n    q[idx++] = p[0];\n    q[idx++] = p[1];\n    q[idx++] = p[2];\n    if (this.order === 3) {\n      q[idx++] = p[3];\n    }\n    // we lerp between all points at each iteration, until we have 1 point left.\n    while (p.length > 1) {\n      _p = [];\n      for (let i = 0, pt, l = p.length - 1; i < l; i++) {\n        pt = utils.lerp(t, p[i], p[i + 1]);\n        q[idx++] = pt;\n        _p.push(pt);\n      }\n      p = _p;\n    }\n    return q;\n  }\n\n  split(t1, t2) {\n    // shortcuts\n    if (t1 === 0 && !!t2) {\n      return this.split(t2).left;\n    }\n    if (t2 === 1) {\n      return this.split(t1).right;\n    }\n\n    // no shortcut: use \"de Casteljau\" iteration.\n    const q = this.hull(t1);\n    const result = {\n      left:\n        this.order === 2\n          ? new Bezier([q[0], q[3], q[5]])\n          : new Bezier([q[0], q[4], q[7], q[9]]),\n      right:\n        this.order === 2\n          ? new Bezier([q[5], q[4], q[2]])\n          : new Bezier([q[9], q[8], q[6], q[3]]),\n      span: q,\n    };\n\n    // make sure we bind _t1/_t2 information!\n    result.left._t1 = utils.map(0, 0, 1, this._t1, this._t2);\n    result.left._t2 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t1 = utils.map(t1, 0, 1, this._t1, this._t2);\n    result.right._t2 = utils.map(1, 0, 1, this._t1, this._t2);\n\n    // if we have no t2, we're done\n    if (!t2) {\n      return result;\n    }\n\n    // if we have a t2, split again:\n    t2 = utils.map(t2, t1, 1, 0, 1);\n    return result.right.split(t2).left;\n  }\n\n  extrema() {\n    const result = {};\n    let roots = [];\n\n    this.dims.forEach(\n      function (dim) {\n        let mfn = function (v) {\n          return v[dim];\n        };\n        let p = this.dpoints[0].map(mfn);\n        result[dim] = utils.droots(p);\n        if (this.order === 3) {\n          p = this.dpoints[1].map(mfn);\n          result[dim] = result[dim].concat(utils.droots(p));\n        }\n        result[dim] = result[dim].filter(function (t) {\n          return t >= 0 && t <= 1;\n        });\n        roots = roots.concat(result[dim].sort(utils.numberSort));\n      }.bind(this)\n    );\n\n    result.values = roots.sort(utils.numberSort).filter(function (v, idx) {\n      return roots.indexOf(v) === idx;\n    });\n\n    return result;\n  }\n\n  bbox() {\n    const extrema = this.extrema(),\n      result = {};\n    this.dims.forEach(\n      function (d) {\n        result[d] = utils.getminmax(this, d, extrema[d]);\n      }.bind(this)\n    );\n    return result;\n  }\n\n  overlaps(curve) {\n    const lbbox = this.bbox(),\n      tbbox = curve.bbox();\n    return utils.bboxoverlap(lbbox, tbbox);\n  }\n\n  offset(t, d) {\n    if (typeof d !== \"undefined\") {\n      const c = this.get(t),\n        n = this.normal(t);\n      const ret = {\n        c: c,\n        n: n,\n        x: c.x + n.x * d,\n        y: c.y + n.y * d,\n      };\n      if (this._3d) {\n        ret.z = c.z + n.z * d;\n      }\n      return ret;\n    }\n    if (this._linear) {\n      const nv = this.normal(0),\n        coords = this.points.map(function (p) {\n          const ret = {\n            x: p.x + t * nv.x,\n            y: p.y + t * nv.y,\n          };\n          if (p.z && nv.z) {\n            ret.z = p.z + t * nv.z;\n          }\n          return ret;\n        });\n      return [new Bezier(coords)];\n    }\n    return this.reduce().map(function (s) {\n      if (s._linear) {\n        return s.offset(t)[0];\n      }\n      return s.scale(t);\n    });\n  }\n\n  simple() {\n    if (this.order === 3) {\n      const a1 = utils.angle(this.points[0], this.points[3], this.points[1]);\n      const a2 = utils.angle(this.points[0], this.points[3], this.points[2]);\n      if ((a1 > 0 && a2 < 0) || (a1 < 0 && a2 > 0)) return false;\n    }\n    const n1 = this.normal(0);\n    const n2 = this.normal(1);\n    let s = n1.x * n2.x + n1.y * n2.y;\n    if (this._3d) {\n      s += n1.z * n2.z;\n    }\n    return abs(acos(s)) < pi / 3;\n  }\n\n  reduce() {\n    // TODO: examine these var types in more detail...\n    let i,\n      t1 = 0,\n      t2 = 0,\n      step = 0.01,\n      segment,\n      pass1 = [],\n      pass2 = [];\n    // first pass: split on extrema\n    let extrema = this.extrema().values;\n    if (extrema.indexOf(0) === -1) {\n      extrema = [0].concat(extrema);\n    }\n    if (extrema.indexOf(1) === -1) {\n      extrema.push(1);\n    }\n\n    for (t1 = extrema[0], i = 1; i < extrema.length; i++) {\n      t2 = extrema[i];\n      segment = this.split(t1, t2);\n      segment._t1 = t1;\n      segment._t2 = t2;\n      pass1.push(segment);\n      t1 = t2;\n    }\n\n    // second pass: further reduce these segments to simple segments\n    pass1.forEach(function (p1) {\n      t1 = 0;\n      t2 = 0;\n      while (t2 <= 1) {\n        for (t2 = t1 + step; t2 <= 1 + step; t2 += step) {\n          segment = p1.split(t1, t2);\n          if (!segment.simple()) {\n            t2 -= step;\n            if (abs(t1 - t2) < step) {\n              // we can never form a reduction\n              return [];\n            }\n            segment = p1.split(t1, t2);\n            segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n            segment._t2 = utils.map(t2, 0, 1, p1._t1, p1._t2);\n            pass2.push(segment);\n            t1 = t2;\n            break;\n          }\n        }\n      }\n      if (t1 < 1) {\n        segment = p1.split(t1, 1);\n        segment._t1 = utils.map(t1, 0, 1, p1._t1, p1._t2);\n        segment._t2 = p1._t2;\n        pass2.push(segment);\n      }\n    });\n    return pass2;\n  }\n\n  translate(v, d1, d2) {\n    d2 = typeof d2 === \"number\" ? d2 : d1;\n\n    // TODO: make this take curves with control points outside\n    //       of the start-end interval into account\n\n    const o = this.order;\n    let d = this.points.map((_, i) => (1 - i / o) * d1 + (i / o) * d2);\n    return new Bezier(\n      this.points.map((p, i) => ({\n        x: p.x + v.x * d[i],\n        y: p.y + v.y * d[i],\n      }))\n    );\n  }\n\n  scale(d) {\n    const order = this.order;\n    let distanceFn = false;\n    if (typeof d === \"function\") {\n      distanceFn = d;\n    }\n    if (distanceFn && order === 2) {\n      return this.raise().scale(distanceFn);\n    }\n\n    // TODO: add special handling for non-linear degenerate curves.\n\n    const clockwise = this.clockwise;\n    const points = this.points;\n\n    if (this._linear) {\n      return this.translate(\n        this.normal(0),\n        distanceFn ? distanceFn(0) : d,\n        distanceFn ? distanceFn(1) : d\n      );\n    }\n\n    const r1 = distanceFn ? distanceFn(0) : d;\n    const r2 = distanceFn ? distanceFn(1) : d;\n    const v = [this.offset(0, 10), this.offset(1, 10)];\n    const np = [];\n    const o = utils.lli4(v[0], v[0].c, v[1], v[1].c);\n\n    if (!o) {\n      throw new Error(\"cannot scale this curve. Try reducing it first.\");\n    }\n\n    // move all points by distance 'd' wrt the origin 'o',\n    // and move end points by fixed distance along normal.\n    [0, 1].forEach(function (t) {\n      const p = (np[t * order] = utils.copy(points[t * order]));\n      p.x += (t ? r2 : r1) * v[t].n.x;\n      p.y += (t ? r2 : r1) * v[t].n.y;\n    });\n\n    if (!distanceFn) {\n      // move control points to lie on the intersection of the offset\n      // derivative vector, and the origin-through-control vector\n      [0, 1].forEach((t) => {\n        if (order === 2 && !!t) return;\n        const p = np[t * order];\n        const d = this.derivative(t);\n        const p2 = { x: p.x + d.x, y: p.y + d.y };\n        np[t + 1] = utils.lli4(p, p2, o, points[t + 1]);\n      });\n      return new Bezier(np);\n    }\n\n    // move control points by \"however much necessary to\n    // ensure the correct tangent to endpoint\".\n    [0, 1].forEach(function (t) {\n      if (order === 2 && !!t) return;\n      var p = points[t + 1];\n      var ov = {\n        x: p.x - o.x,\n        y: p.y - o.y,\n      };\n      var rc = distanceFn ? distanceFn((t + 1) / order) : d;\n      if (distanceFn && !clockwise) rc = -rc;\n      var m = sqrt(ov.x * ov.x + ov.y * ov.y);\n      ov.x /= m;\n      ov.y /= m;\n      np[t + 1] = {\n        x: p.x + rc * ov.x,\n        y: p.y + rc * ov.y,\n      };\n    });\n    return new Bezier(np);\n  }\n\n  outline(d1, d2, d3, d4) {\n    d2 = d2 === undefined ? d1 : d2;\n\n    if (this._linear) {\n      // TODO: find the actual extrema, because they might\n      //       be before the start, or past the end.\n\n      const n = this.normal(0);\n      const start = this.points[0];\n      const end = this.points[this.points.length - 1];\n      let s, mid, e;\n\n      if (d3 === undefined) {\n        d3 = d1;\n        d4 = d2;\n      }\n\n      s = { x: start.x + n.x * d1, y: start.y + n.y * d1 };\n      e = { x: end.x + n.x * d3, y: end.y + n.y * d3 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const fline = [s, mid, e];\n\n      s = { x: start.x - n.x * d2, y: start.y - n.y * d2 };\n      e = { x: end.x - n.x * d4, y: end.y - n.y * d4 };\n      mid = { x: (s.x + e.x) / 2, y: (s.y + e.y) / 2 };\n      const bline = [e, mid, s];\n\n      const ls = utils.makeline(bline[2], fline[0]);\n      const le = utils.makeline(fline[2], bline[0]);\n      const segments = [ls, new Bezier(fline), le, new Bezier(bline)];\n      return new PolyBezier(segments);\n    }\n\n    const reduced = this.reduce(),\n      len = reduced.length,\n      fcurves = [];\n\n    let bcurves = [],\n      p,\n      alen = 0,\n      tlen = this.length();\n\n    const graduated = typeof d3 !== \"undefined\" && typeof d4 !== \"undefined\";\n\n    function linearDistanceFunction(s, e, tlen, alen, slen) {\n      return function (v) {\n        const f1 = alen / tlen,\n          f2 = (alen + slen) / tlen,\n          d = e - s;\n        return utils.map(v, 0, 1, s + f1 * d, s + f2 * d);\n      };\n    }\n\n    // form curve oulines\n    reduced.forEach(function (segment) {\n      const slen = segment.length();\n      if (graduated) {\n        fcurves.push(\n          segment.scale(linearDistanceFunction(d1, d3, tlen, alen, slen))\n        );\n        bcurves.push(\n          segment.scale(linearDistanceFunction(-d2, -d4, tlen, alen, slen))\n        );\n      } else {\n        fcurves.push(segment.scale(d1));\n        bcurves.push(segment.scale(-d2));\n      }\n      alen += slen;\n    });\n\n    // reverse the \"return\" outline\n    bcurves = bcurves\n      .map(function (s) {\n        p = s.points;\n        if (p[3]) {\n          s.points = [p[3], p[2], p[1], p[0]];\n        } else {\n          s.points = [p[2], p[1], p[0]];\n        }\n        return s;\n      })\n      .reverse();\n\n    // form the endcaps as lines\n    const fs = fcurves[0].points[0],\n      fe = fcurves[len - 1].points[fcurves[len - 1].points.length - 1],\n      bs = bcurves[len - 1].points[bcurves[len - 1].points.length - 1],\n      be = bcurves[0].points[0],\n      ls = utils.makeline(bs, fs),\n      le = utils.makeline(fe, be),\n      segments = [ls].concat(fcurves).concat([le]).concat(bcurves);\n\n    return new PolyBezier(segments);\n  }\n\n  outlineshapes(d1, d2, curveIntersectionThreshold) {\n    d2 = d2 || d1;\n    const outline = this.outline(d1, d2).curves;\n    const shapes = [];\n    for (let i = 1, len = outline.length; i < len / 2; i++) {\n      const shape = utils.makeshape(\n        outline[i],\n        outline[len - i],\n        curveIntersectionThreshold\n      );\n      shape.startcap.virtual = i > 1;\n      shape.endcap.virtual = i < len / 2 - 1;\n      shapes.push(shape);\n    }\n    return shapes;\n  }\n\n  intersects(curve, curveIntersectionThreshold) {\n    if (!curve) return this.selfintersects(curveIntersectionThreshold);\n    if (curve.p1 && curve.p2) {\n      return this.lineIntersects(curve);\n    }\n    if (curve instanceof Bezier) {\n      curve = curve.reduce();\n    }\n    return this.curveintersects(\n      this.reduce(),\n      curve,\n      curveIntersectionThreshold\n    );\n  }\n\n  lineIntersects(line) {\n    const mx = min(line.p1.x, line.p2.x),\n      my = min(line.p1.y, line.p2.y),\n      MX = max(line.p1.x, line.p2.x),\n      MY = max(line.p1.y, line.p2.y);\n    return utils.roots(this.points, line).filter((t) => {\n      var p = this.get(t);\n      return utils.between(p.x, mx, MX) && utils.between(p.y, my, MY);\n    });\n  }\n\n  selfintersects(curveIntersectionThreshold) {\n    // \"simple\" curves cannot intersect with their direct\n    // neighbour, so for each segment X we check whether\n    // it intersects [0:x-2][x+2:last].\n\n    const reduced = this.reduce(),\n      len = reduced.length - 2,\n      results = [];\n\n    for (let i = 0, result, left, right; i < len; i++) {\n      left = reduced.slice(i, i + 1);\n      right = reduced.slice(i + 2);\n      result = this.curveintersects(left, right, curveIntersectionThreshold);\n      results.push(...result);\n    }\n    return results;\n  }\n\n  curveintersects(c1, c2, curveIntersectionThreshold) {\n    const pairs = [];\n    // step 1: pair off any overlapping segments\n    c1.forEach(function (l) {\n      c2.forEach(function (r) {\n        if (l.overlaps(r)) {\n          pairs.push({ left: l, right: r });\n        }\n      });\n    });\n    // step 2: for each pairing, run through the convergence algorithm.\n    let intersections = [];\n    pairs.forEach(function (pair) {\n      const result = utils.pairiteration(\n        pair.left,\n        pair.right,\n        curveIntersectionThreshold\n      );\n      if (result.length > 0) {\n        intersections = intersections.concat(result);\n      }\n    });\n    return intersections;\n  }\n\n  arcs(errorThreshold) {\n    errorThreshold = errorThreshold || 0.5;\n    return this._iterate(errorThreshold, []);\n  }\n\n  _error(pc, np1, s, e) {\n    const q = (e - s) / 4,\n      c1 = this.get(s + q),\n      c2 = this.get(e - q),\n      ref = utils.dist(pc, np1),\n      d1 = utils.dist(pc, c1),\n      d2 = utils.dist(pc, c2);\n    return abs(d1 - ref) + abs(d2 - ref);\n  }\n\n  _iterate(errorThreshold, circles) {\n    let t_s = 0,\n      t_e = 1,\n      safety;\n    // we do a binary search to find the \"good `t` closest to no-longer-good\"\n    do {\n      safety = 0;\n\n      // step 1: start with the maximum possible arc\n      t_e = 1;\n\n      // points:\n      let np1 = this.get(t_s),\n        np2,\n        np3,\n        arc,\n        prev_arc;\n\n      // booleans:\n      let curr_good = false,\n        prev_good = false,\n        done;\n\n      // numbers:\n      let t_m = t_e,\n        prev_e = 1,\n        step = 0;\n\n      // step 2: find the best possible arc\n      do {\n        prev_good = curr_good;\n        prev_arc = arc;\n        t_m = (t_s + t_e) / 2;\n        step++;\n\n        np2 = this.get(t_m);\n        np3 = this.get(t_e);\n\n        arc = utils.getccenter(np1, np2, np3);\n\n        //also save the t values\n        arc.interval = {\n          start: t_s,\n          end: t_e,\n        };\n\n        let error = this._error(arc, np1, t_s, t_e);\n        curr_good = error <= errorThreshold;\n\n        done = prev_good && !curr_good;\n        if (!done) prev_e = t_e;\n\n        // this arc is fine: we can move 'e' up to see if we can find a wider arc\n        if (curr_good) {\n          // if e is already at max, then we're done for this arc.\n          if (t_e >= 1) {\n            // make sure we cap at t=1\n            arc.interval.end = prev_e = 1;\n            prev_arc = arc;\n            // if we capped the arc segment to t=1 we also need to make sure that\n            // the arc's end angle is correct with respect to the bezier end point.\n            if (t_e > 1) {\n              let d = {\n                x: arc.x + arc.r * cos(arc.e),\n                y: arc.y + arc.r * sin(arc.e),\n              };\n              arc.e += utils.angle({ x: arc.x, y: arc.y }, d, this.get(1));\n            }\n            break;\n          }\n          // if not, move it up by half the iteration distance\n          t_e = t_e + (t_e - t_s) / 2;\n        } else {\n          // this is a bad arc: we need to move 'e' down to find a good arc\n          t_e = t_m;\n        }\n      } while (!done && safety++ < 100);\n\n      if (safety >= 100) {\n        break;\n      }\n\n      // console.log(\"L835: [F] arc found\", t_s, prev_e, prev_arc.x, prev_arc.y, prev_arc.s, prev_arc.e);\n\n      prev_arc = prev_arc ? prev_arc : arc;\n      circles.push(prev_arc);\n      t_s = prev_e;\n    } while (t_e < 1);\n    return circles;\n  }\n}\n\nexport { Bezier };\n",
         "export default {\n\taliceblue: [240, 248, 255],\n\tantiquewhite: [250, 235, 215],\n\taqua: [0, 255, 255],\n\taquamarine: [127, 255, 212],\n\tazure: [240, 255, 255],\n\tbeige: [245, 245, 220],\n\tbisque: [255, 228, 196],\n\tblack: [0, 0, 0],\n\tblanchedalmond: [255, 235, 205],\n\tblue: [0, 0, 255],\n\tblueviolet: [138, 43, 226],\n\tbrown: [165, 42, 42],\n\tburlywood: [222, 184, 135],\n\tcadetblue: [95, 158, 160],\n\tchartreuse: [127, 255, 0],\n\tchocolate: [210, 105, 30],\n\tcoral: [255, 127, 80],\n\tcornflowerblue: [100, 149, 237],\n\tcornsilk: [255, 248, 220],\n\tcrimson: [220, 20, 60],\n\tcyan: [0, 255, 255],\n\tdarkblue: [0, 0, 139],\n\tdarkcyan: [0, 139, 139],\n\tdarkgoldenrod: [184, 134, 11],\n\tdarkgray: [169, 169, 169],\n\tdarkgreen: [0, 100, 0],\n\tdarkgrey: [169, 169, 169],\n\tdarkkhaki: [189, 183, 107],\n\tdarkmagenta: [139, 0, 139],\n\tdarkolivegreen: [85, 107, 47],\n\tdarkorange: [255, 140, 0],\n\tdarkorchid: [153, 50, 204],\n\tdarkred: [139, 0, 0],\n\tdarksalmon: [233, 150, 122],\n\tdarkseagreen: [143, 188, 143],\n\tdarkslateblue: [72, 61, 139],\n\tdarkslategray: [47, 79, 79],\n\tdarkslategrey: [47, 79, 79],\n\tdarkturquoise: [0, 206, 209],\n\tdarkviolet: [148, 0, 211],\n\tdeeppink: [255, 20, 147],\n\tdeepskyblue: [0, 191, 255],\n\tdimgray: [105, 105, 105],\n\tdimgrey: [105, 105, 105],\n\tdodgerblue: [30, 144, 255],\n\tfirebrick: [178, 34, 34],\n\tfloralwhite: [255, 250, 240],\n\tforestgreen: [34, 139, 34],\n\tfuchsia: [255, 0, 255],\n\tgainsboro: [220, 220, 220],\n\tghostwhite: [248, 248, 255],\n\tgold: [255, 215, 0],\n\tgoldenrod: [218, 165, 32],\n\tgray: [128, 128, 128],\n\tgreen: [0, 128, 0],\n\tgreenyellow: [173, 255, 47],\n\tgrey: [128, 128, 128],\n\thoneydew: [240, 255, 240],\n\thotpink: [255, 105, 180],\n\tindianred: [205, 92, 92],\n\tindigo: [75, 0, 130],\n\tivory: [255, 255, 240],\n\tkhaki: [240, 230, 140],\n\tlavender: [230, 230, 250],\n\tlavenderblush: [255, 240, 245],\n\tlawngreen: [124, 252, 0],\n\tlemonchiffon: [255, 250, 205],\n\tlightblue: [173, 216, 230],\n\tlightcoral: [240, 128, 128],\n\tlightcyan: [224, 255, 255],\n\tlightgoldenrodyellow: [250, 250, 210],\n\tlightgray: [211, 211, 211],\n\tlightgreen: [144, 238, 144],\n\tlightgrey: [211, 211, 211],\n\tlightpink: [255, 182, 193],\n\tlightsalmon: [255, 160, 122],\n\tlightseagreen: [32, 178, 170],\n\tlightskyblue: [135, 206, 250],\n\tlightslategray: [119, 136, 153],\n\tlightslategrey: [119, 136, 153],\n\tlightsteelblue: [176, 196, 222],\n\tlightyellow: [255, 255, 224],\n\tlime: [0, 255, 0],\n\tlimegreen: [50, 205, 50],\n\tlinen: [250, 240, 230],\n\tmagenta: [255, 0, 255],\n\tmaroon: [128, 0, 0],\n\tmediumaquamarine: [102, 205, 170],\n\tmediumblue: [0, 0, 205],\n\tmediumorchid: [186, 85, 211],\n\tmediumpurple: [147, 112, 219],\n\tmediumseagreen: [60, 179, 113],\n\tmediumslateblue: [123, 104, 238],\n\tmediumspringgreen: [0, 250, 154],\n\tmediumturquoise: [72, 209, 204],\n\tmediumvioletred: [199, 21, 133],\n\tmidnightblue: [25, 25, 112],\n\tmintcream: [245, 255, 250],\n\tmistyrose: [255, 228, 225],\n\tmoccasin: [255, 228, 181],\n\tnavajowhite: [255, 222, 173],\n\tnavy: [0, 0, 128],\n\toldlace: [253, 245, 230],\n\tolive: [128, 128, 0],\n\tolivedrab: [107, 142, 35],\n\torange: [255, 165, 0],\n\torangered: [255, 69, 0],\n\torchid: [218, 112, 214],\n\tpalegoldenrod: [238, 232, 170],\n\tpalegreen: [152, 251, 152],\n\tpaleturquoise: [175, 238, 238],\n\tpalevioletred: [219, 112, 147],\n\tpapayawhip: [255, 239, 213],\n\tpeachpuff: [255, 218, 185],\n\tperu: [205, 133, 63],\n\tpink: [255, 192, 203],\n\tplum: [221, 160, 221],\n\tpowderblue: [176, 224, 230],\n\tpurple: [128, 0, 128],\n\trebeccapurple: [102, 51, 153],\n\tred: [255, 0, 0],\n\trosybrown: [188, 143, 143],\n\troyalblue: [65, 105, 225],\n\tsaddlebrown: [139, 69, 19],\n\tsalmon: [250, 128, 114],\n\tsandybrown: [244, 164, 96],\n\tseagreen: [46, 139, 87],\n\tseashell: [255, 245, 238],\n\tsienna: [160, 82, 45],\n\tsilver: [192, 192, 192],\n\tskyblue: [135, 206, 235],\n\tslateblue: [106, 90, 205],\n\tslategray: [112, 128, 144],\n\tslategrey: [112, 128, 144],\n\tsnow: [255, 250, 250],\n\tspringgreen: [0, 255, 127],\n\tsteelblue: [70, 130, 180],\n\ttan: [210, 180, 140],\n\tteal: [0, 128, 128],\n\tthistle: [216, 191, 216],\n\ttomato: [255, 99, 71],\n\tturquoise: [64, 224, 208],\n\tviolet: [238, 130, 238],\n\twheat: [245, 222, 179],\n\twhite: [255, 255, 255],\n\twhitesmoke: [245, 245, 245],\n\tyellow: [255, 255, 0],\n\tyellowgreen: [154, 205, 50]\n}\n",
         "/**\n * @module color-parse\n */\nimport names from 'color-name'\n\nexport default parse\n\n/**\n * Base hues\n * http://dev.w3.org/csswg/css-color/#typedef-named-hue\n */\n//FIXME: use external hue detector\nvar baseHues = {\n\tred: 0,\n\torange: 60,\n\tyellow: 120,\n\tgreen: 180,\n\tblue: 240,\n\tpurple: 300\n}\n\n/**\n * Parse color from the string passed\n *\n * @return {Object} A space indicator `space`, an array `values` and `alpha`\n */\nfunction parse(cstr) {\n\tvar m, parts = [], alpha = 1, space\n\n\t//numeric case\n\tif (typeof cstr === 'number') {\n\t\treturn { space: 'rgb', values: [cstr >>> 16, (cstr & 0x00ff00) >>> 8, cstr & 0x0000ff], alpha: 1 }\n\t}\n\tif (typeof cstr === 'number') return { space: 'rgb', values: [cstr >>> 16, (cstr & 0x00ff00) >>> 8, cstr & 0x0000ff], alpha: 1 }\n\n\tcstr = String(cstr).toLowerCase();\n\n\t//keyword\n\tif (names[cstr]) {\n\t\tparts = names[cstr].slice()\n\t\tspace = 'rgb'\n\t}\n\n\t//reserved words\n\telse if (cstr === 'transparent') {\n\t\talpha = 0\n\t\tspace = 'rgb'\n\t\tparts = [0, 0, 0]\n\t}\n\n\t//hex\n\telse if (cstr[0] === '#') {\n\t\tvar base = cstr.slice(1)\n\t\tvar size = base.length\n\t\tvar isShort = size <= 4\n\t\talpha = 1\n\n\t\tif (isShort) {\n\t\t\tparts = [\n\t\t\t\tparseInt(base[0] + base[0], 16),\n\t\t\t\tparseInt(base[1] + base[1], 16),\n\t\t\t\tparseInt(base[2] + base[2], 16)\n\t\t\t]\n\t\t\tif (size === 4) {\n\t\t\t\talpha = parseInt(base[3] + base[3], 16) / 255\n\t\t\t}\n\t\t}\n\t\telse {\n\t\t\tparts = [\n\t\t\t\tparseInt(base[0] + base[1], 16),\n\t\t\t\tparseInt(base[2] + base[3], 16),\n\t\t\t\tparseInt(base[4] + base[5], 16)\n\t\t\t]\n\t\t\tif (size === 8) {\n\t\t\t\talpha = parseInt(base[6] + base[7], 16) / 255\n\t\t\t}\n\t\t}\n\n\t\tif (!parts[0]) parts[0] = 0\n\t\tif (!parts[1]) parts[1] = 0\n\t\tif (!parts[2]) parts[2] = 0\n\n\t\tspace = 'rgb'\n\t}\n\n\t// color space\n\telse if (m = /^((?:rgba?|hs[lvb]a?|hwba?|cmyk?|xy[zy]|gray|lab|lchu?v?|[ly]uv|lms|oklch|oklab|color))\\s*\\(([^\\)]*)\\)/.exec(cstr)) {\n\t\tvar name = m[1]\n\t\tspace = name.replace(/a$/, '')\n\t\tvar dims = space === 'cmyk' ? 4 : space === 'gray' ? 1 : 3\n\t\tparts = m[2].trim().split(/\\s*[,\\/]\\s*|\\s+/)\n\n\t\t// color(srgb-linear x x x) -> srgb-linear(x x x)\n\t\tif (space === 'color') space = parts.shift()\n\n\t\tparts = parts.map(function (x, i) {\n\t\t\t//<percentage>\n\t\t\tif (x[x.length - 1] === '%') {\n\t\t\t\tx = parseFloat(x) / 100\n\t\t\t\t// alpha -> 0..1\n\t\t\t\tif (i === 3) return x\n\t\t\t\t// rgb -> 0..255\n\t\t\t\tif (space === 'rgb') return x * 255\n\t\t\t\t// hsl, hwb H -> 0..100\n\t\t\t\tif (space[0] === 'h') return x * 100\n\t\t\t\t// lch, lab L -> 0..100\n\t\t\t\tif (space[0] === 'l' && !i) return x * 100\n\t\t\t\t// lab A B -> -125..125\n\t\t\t\tif (space === 'lab') return x * 125\n\t\t\t\t// lch C -> 0..150, H -> 0..360\n\t\t\t\tif (space === 'lch') return i < 2 ? x * 150 : x * 360\n\t\t\t\t// oklch/oklab L -> 0..1\n\t\t\t\tif (space[0] === 'o' && !i) return x\n\t\t\t\t// oklab A B -> -0.4..0.4\n\t\t\t\tif (space === 'oklab') return x * 0.4\n\t\t\t\t// oklch C -> 0..0.4, H -> 0..360\n\t\t\t\tif (space === 'oklch') return i < 2 ? x * 0.4 : x * 360\n\t\t\t\t// color(xxx) -> 0..1\n\t\t\t\treturn x\n\t\t\t}\n\n\t\t\t//hue\n\t\t\tif (space[i] === 'h' || (i === 2 && space[space.length - 1] === 'h')) {\n\t\t\t\t//<base-hue>\n\t\t\t\tif (baseHues[x] !== undefined) return baseHues[x]\n\t\t\t\t//<deg>\n\t\t\t\tif (x.endsWith('deg')) return parseFloat(x)\n\t\t\t\t//<turn>\n\t\t\t\tif (x.endsWith('turn')) return parseFloat(x) * 360\n\t\t\t\tif (x.endsWith('grad')) return parseFloat(x) * 360 / 400\n\t\t\t\tif (x.endsWith('rad')) return parseFloat(x) * 180 / Math.PI\n\t\t\t}\n\t\t\tif (x === 'none') return 0\n\t\t\treturn parseFloat(x)\n\t\t});\n\n\t\talpha = parts.length > dims ? parts.pop() : 1\n\t}\n\n\t//named channels case\n\telse if (/[0-9](?:\\s|\\/|,)/.test(cstr)) {\n\t\tparts = cstr.match(/([0-9]+)/g).map(function (value) {\n\t\t\treturn parseFloat(value)\n\t\t})\n\n\t\tspace = cstr.match(/([a-z])/ig)?.join('')?.toLowerCase() || 'rgb'\n\t}\n\n\treturn {\n\t\tspace,\n\t\tvalues: parts,\n\t\talpha\n\t}\n}\n",
         "/**\n * RGB space.\n *\n * @module  color-space/rgb\n */\n\nexport default {\n\tname: 'rgb',\n\tmin: [0,0,0],\n\tmax: [255,255,255],\n\tchannel: ['red', 'green', 'blue'],\n\talias: ['RGB']\n};\n",
         "/**\n * @module color-space/hsl\n */\nimport rgb from './rgb.js';\n\nexport default {\n\tname: 'hsl',\n\tmin: [0,0,0],\n\tmax: [360,100,100],\n\tchannel: ['hue', 'saturation', 'lightness'],\n\talias: ['HSL'],\n\n\trgb: function(hsl) {\n\t\tvar h = hsl[0]/360, s = hsl[1]/100, l = hsl[2]/100, t1, t2, t3, rgb, val, i=0;\n\n\t\tif (s === 0) return val = l * 255, [val, val, val];\n\n\t\tt2 = l < 0.5 ? l * (1 + s) : l + s - l * s;\n\t\tt1 = 2 * l - t2;\n\n\t\trgb = [0, 0, 0];\n\t\tfor (;i<3;) {\n\t\t\tt3 = h + 1 / 3 * - (i - 1);\n\t\t\tt3 < 0 ? t3++ : t3 > 1 && t3--;\n\t\t\tval = 6 * t3 < 1 ? t1 + (t2 - t1) * 6 * t3 :\n\t\t\t2 * t3 < 1 ? t2 :\n\t\t\t3 * t3 < 2 ?  t1 + (t2 - t1) * (2 / 3 - t3) * 6 :\n\t\t\tt1;\n\t\t\trgb[i++] = val * 255;\n\t\t}\n\n\t\treturn rgb;\n\t}\n};\n\n\n//extend rgb\nrgb.hsl = function(rgb) {\n\tvar r = rgb[0]/255,\n\t\t\tg = rgb[1]/255,\n\t\t\tb = rgb[2]/255,\n\t\t\tmin = Math.min(r, g, b),\n\t\t\tmax = Math.max(r, g, b),\n\t\t\tdelta = max - min,\n\t\t\th, s, l;\n\n\tif (max === min) {\n\t\th = 0;\n\t}\n\telse if (r === max) {\n\t\th = (g - b) / delta;\n\t}\n\telse if (g === max) {\n\t\th = 2 + (b - r) / delta;\n\t}\n\telse if (b === max) {\n\t\th = 4 + (r - g)/ delta;\n\t}\n\n\th = Math.min(h * 60, 360);\n\n\tif (h < 0) {\n\t\th += 360;\n\t}\n\n\tl = (min + max) / 2;\n\n\tif (max === min) {\n\t\ts = 0;\n\t}\n\telse if (l <= 0.5) {\n\t\ts = delta / (max + min);\n\t}\n\telse {\n\t\ts = delta / (2 - max - min);\n\t}\n\n\treturn [h, s * 100, l * 100];\n};\n",
         "/** @module  color-rgba */\nimport parse from 'color-parse'\nimport rgb from 'color-space/rgb.js'\nimport hsl from 'color-space/hsl.js'\n\nexport default function rgba(color) {\n\t// template literals\n\tif (Array.isArray(color) && color.raw) color = String.raw(...arguments)\n\tif (color instanceof Number) color = +color\n\n\tvar values, i, l\n\n\t//attempt to parse non-array arguments\n\tvar parsed = parse(color)\n\n\tif (!parsed.space) return []\n\n\tconst min = parsed.space[0] === 'h' ? hsl.min : rgb.min\n\tconst max = parsed.space[0] === 'h' ? hsl.max : rgb.max\n\n\tvalues = Array(3)\n\tvalues[0] = Math.min(Math.max(parsed.values[0], min[0]), max[0])\n\tvalues[1] = Math.min(Math.max(parsed.values[1], min[1]), max[1])\n\tvalues[2] = Math.min(Math.max(parsed.values[2], min[2]), max[2])\n\n\tif (parsed.space[0] === 'h') {\n\t\tvalues = hsl.rgb(values)\n\t}\n\n\tvalues.push(Math.min(Math.max(parsed.alpha, 0), 1))\n\n\treturn values\n}\n",
         "import { Bezier } from \"bezier-js\"\r\nimport rgba from \"color-rgba\"\r\n\r\nexport function createFixedData(data, options) {\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => options.fixed_lines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: false,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0.3,\r\n        spanGaps: false,\r\n        showLine: true,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: colData.color,\r\n        pointRadius: colData.point_radius,\r\n        borderDash: colData.border_dash,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createControlData(data, options) {\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => !options.fixed_lines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.5)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: true,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0,\r\n        cubicInterpolationMode: \"default\",\r\n        spanGaps: options.fill_gaps,\r\n        showLine: true,\r\n        borderDash: [5, 5],\r\n        borderWidth: 1,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createBezierData(data, options) {\r\n  const datasets = Object.entries(data)\r\n    .filter(([trace]) => !options.fixed_lines.includes(trace))\r\n    .map(([trace, traceData], i) => {\r\n      const points = traceData.x.map((x, j) => ({\r\n        x: x,\r\n        y: traceData.y[j],\r\n      }))\r\n\r\n      const bezierSegments = []\r\n      for (let i = 0; i < points.length - 2; i += 2) {\r\n        const bezierPoints = points.slice(i, i + 3)\r\n        const bezier = new Bezier(bezierPoints)\r\n        const lut = bezier.getLUT(10)\r\n        bezierSegments.push(...lut)\r\n      }\r\n      const colorRGBA = rgba(traceData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.4)`\r\n      return {\r\n        label: trace + \" (bezier)\",\r\n        data: bezierSegments,\r\n        isControlPoint: false,\r\n        showLine: true,\r\n        tension: 0.3,\r\n        pointRadius: 0,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n        borderDash: traceData.border_dash,\r\n      }\r\n    })\r\n\r\n  return { datasets }\r\n}\r\n",
-        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass BezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    return this.map(\r\n      position.y,\r\n      chartArea.bottom,\r\n      chartArea.top,\r\n      yAxis.min,\r\n      yAxis.max\r\n    )\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    return this.map(\r\n      position.x,\r\n      chartArea.left,\r\n      chartArea.right,\r\n      xAxis.min,\r\n      xAxis.max\r\n    )\r\n  }\r\n\r\n  updateControlPointPosition = (chart, activePoint, newXValue, newYValue) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    chart.data.datasets[datasetIndex].data[pointIndex].x = newXValue\r\n    chart.data.datasets[datasetIndex].data[pointIndex].y = newYValue\r\n  }\r\n\r\n  updateOriginalData = (chart, activePoint) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    const datasetLabel = chart.data.datasets[datasetIndex].label\r\n    const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n    const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n    this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n    this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n\r\n      // Update control point position\r\n      this.updateControlPointPosition(chart, activePoint, newXValue, newYValue)\r\n      // Set new values in originalData\r\n      this.updateOriginalData(chart, activePoint)\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n            ...this.fixedData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default BezierChart\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\nimport { calculateNewXValue, calculateNewYValue } from \"../Utils/handlers\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass BezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  updateControlPointPosition = (chart, activePoint, newXValue, newYValue) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    chart.data.datasets[datasetIndex].data[pointIndex].x = newXValue\r\n    chart.data.datasets[datasetIndex].data[pointIndex].y = newYValue\r\n  }\r\n\r\n  updateOriginalData = (chart, activePoint) => {\r\n    const datasetIndex = activePoint.datasetIndex\r\n    const pointIndex = activePoint.index\r\n    const datasetLabel = chart.data.datasets[datasetIndex].label\r\n    const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n    const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n\r\n    this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n    this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = calculateNewYValue(position, chartArea, chart.scales.y)\r\n      const newXValue = calculateNewXValue(position, chartArea, chart.scales.x)\r\n\r\n      // Update control point position\r\n      this.updateControlPointPosition(chart, activePoint, newXValue, newYValue)\r\n      // Set new values in originalData\r\n      this.updateOriginalData(chart, activePoint)\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n            ...this.fixedData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default BezierChart\r\n",
         "import { Bezier } from \"bezier-js\"\r\nimport rgba from \"color-rgba\"\r\n\r\nexport function createFixedData(data, options) {\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => options.fixed_lines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: false,\r\n        label: colName,\r\n        fill: false,\r\n        tension: 0.3,\r\n        showLine: true,\r\n        backgroundColor: backgroundColorRGBA,\r\n        spanGaps: options.fill_gaps,\r\n        borderColor: colData.color,\r\n        pointRadius: colData.point_radius,\r\n        borderDash: colData.border_dash,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createControlData(data, options) {\r\n  const lineControl = (ctx, value, length) => {\r\n    const index = ctx.p1DataIndex\r\n    if (\r\n      (index % 3 === 0 && index < length - 1) ||\r\n      index % 3 === 1 ||\r\n      index === length - 1\r\n    ) {\r\n      return value\r\n    } else {\r\n      return undefined\r\n    }\r\n  }\r\n  const datasets = Object.entries(data)\r\n    .filter(([colName]) => !options.fixed_lines.includes(colName))\r\n    .map(([colName, colData], index) => {\r\n      const data = colData.x.map((x, i) => ({ x, y: colData.y[i] }))\r\n      const colorRGBA = rgba(colData.color)\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 1)`\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.8)`\r\n      return {\r\n        data: data,\r\n        isControlPoint: true,\r\n        label: colName,\r\n        spanGaps: options.fill_gaps,\r\n        showLine: true,\r\n        borderDash: [8, 5],\r\n        borderWidth: 1.2,\r\n        segment: {\r\n          borderColor: (ctx) => lineControl(ctx, borderColorRGBA, data.length),\r\n        },\r\n        backgroundColor: backgroundColorRGBA,\r\n        pointRadius: colData.point_radius,\r\n      }\r\n    })\r\n\r\n  return {\r\n    datasets: datasets,\r\n  }\r\n}\r\n\r\nexport function createBezierData(data, options) {\r\n  const datasets = Object.entries(data)\r\n    .filter(([trace]) => !options.fixed_lines.includes(trace))\r\n    .map(([trace, traceData], i) => {\r\n      const points = traceData.x.map((x, j) => ({\r\n        x: x,\r\n        y: traceData.y[j],\r\n      }))\r\n\r\n      const bezierSegments = []\r\n      for (let i = 0; i < points.length - 3; i += 3) {\r\n        const bezierPoints = points.slice(i, i + 4)\r\n        const bezier = new Bezier(bezierPoints)\r\n        const lut = bezier.getLUT(10)\r\n        bezierSegments.push(...lut)\r\n      }\r\n      const colorRGBA = rgba(traceData.color)\r\n      const backgroundColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.7)`\r\n      const borderColorRGBA = `rgba(${colorRGBA[0]}, ${colorRGBA[1]}, ${colorRGBA[2]}, 0.6)`\r\n      return {\r\n        label: trace + \" (bezier)\",\r\n        data: bezierSegments,\r\n        isControlPoint: false,\r\n        showLine: true,\r\n        tension: 0.3,\r\n        backgroundColor: backgroundColorRGBA,\r\n        borderColor: borderColorRGBA,\r\n        pointRadius: 0,\r\n        borderDash: traceData.border_dash,\r\n      }\r\n    })\r\n\r\n  return { datasets }\r\n}\r\n",
-        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass CubicBezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  calculateNewYValue = (position, chartArea, yAxis) => {\r\n    return this.map(\r\n      position.y,\r\n      chartArea.bottom,\r\n      chartArea.top,\r\n      yAxis.min,\r\n      yAxis.max\r\n    )\r\n  }\r\n\r\n  calculateNewXValue = (position, chartArea, xAxis) => {\r\n    return this.map(\r\n      position.x,\r\n      chartArea.left,\r\n      chartArea.right,\r\n      xAxis.min,\r\n      xAxis.max\r\n    )\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n\r\n      const newYValue = this.calculateNewYValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.y\r\n      )\r\n\r\n      const newXValue = this.calculateNewXValue(\r\n        position,\r\n        chartArea,\r\n        chart.scales.x\r\n      )\r\n\r\n      // Update control point position\r\n      const datasetIndex = activePoint.datasetIndex\r\n      const pointIndex = activePoint.index\r\n      const deltaY =\r\n        newYValue - chart.data.datasets[datasetIndex].data[pointIndex].y\r\n      const deltaX =\r\n        newXValue - chart.data.datasets[datasetIndex].data[pointIndex].x\r\n\r\n      chart.data.datasets[datasetIndex].data[pointIndex].x = newXValue\r\n      chart.data.datasets[datasetIndex].data[pointIndex].y = newYValue\r\n\r\n      // Set new values in originalData\r\n      const datasetLabel = chart.data.datasets[datasetIndex].label\r\n      const xValue = chart.data.datasets[datasetIndex].data[pointIndex].x\r\n      const yValue = chart.data.datasets[datasetIndex].data[pointIndex].y\r\n      this.state.originalData[datasetLabel][\"x\"][pointIndex] = xValue\r\n      this.state.originalData[datasetLabel][\"y\"][pointIndex] = yValue\r\n\r\n      // If activePoint index is 3, move points 2 and 4 as well\r\n      // If activePoint index is 3, update originalData for points 2 and 4 as well\r\n      const dataLen = chart.data.datasets[datasetIndex].data.length\r\n      if (pointIndex === 0) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 1] += deltaY\r\n      }\r\n      else if (pointIndex === dataLen - 1) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 1] += deltaY\r\n      }\r\n      else if (\r\n        pointIndex % 3 === 0 &&\r\n        pointIndex !== 0 &&\r\n        pointIndex !== dataLen - 1\r\n      ) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 1].y += deltaY\r\n\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].x += deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 1].y += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 1] += deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 1] += deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 1] += deltaY\r\n      } else if ((pointIndex + 1) % 3 === 0 && pointIndex + 1 !== dataLen - 1) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 2].x -= deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex + 2].y -= deltaY\r\n\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex + 2] -= deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex + 2] -= deltaY\r\n      } else if ((pointIndex - 1) % 3 === 0 && pointIndex - 1 !== 0) {\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 2].x -= deltaX\r\n        chart.data.datasets[datasetIndex].data[pointIndex - 2].y -= deltaY\r\n        this.state.originalData[datasetLabel][\"x\"][pointIndex - 2] -= deltaX\r\n        this.state.originalData[datasetLabel][\"y\"][pointIndex - 2] -= deltaY\r\n      }\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  map = (value, start1, stop1, start2, stop2) => {\r\n    return start2 + (stop2 - start2) * ((value - start1) / (stop1 - start1))\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n            ...this.fixedData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default CubicBezierChart\r\n",
+        "import { Chart, registerables } from \"chart.js\"\r\nimport { getRelativePosition } from \"chart.js/helpers\"\r\nimport zoomPlugin from \"chartjs-plugin-zoom\"\r\nimport React from \"react\"\r\n\r\nimport { Scatter, getElementAtEvent } from \"react-chartjs-2\"\r\nimport { Streamlit, StreamlitComponentBase } from \"streamlit-component-lib\"\r\nimport {\r\n  createFixedData,\r\n  createControlData,\r\n  createBezierData,\r\n} from \"./chartData\"\r\nimport { createOptions } from \"../Utils/chartOptions\"\r\nimport { calculateNewXValue, calculateNewYValue } from \"../Utils/handlers\"\r\n\r\nChart.register(...registerables, zoomPlugin)\r\n\r\nclass CubicBezierChart extends StreamlitComponentBase {\r\n  constructor(props) {\r\n    super(props)\r\n    this.chartRef = React.createRef()\r\n    this.fixedData = createFixedData(\r\n      this.props.args.data,\r\n      this.props.args.options\r\n    )\r\n    this.state = {\r\n      activePoint: null,\r\n      originalData: props.args.data,\r\n      controlData: createControlData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      bezierData: createBezierData(\r\n        this.props.args.data,\r\n        this.props.args.options\r\n      ),\r\n      options: createOptions(props.args.options, props.theme),\r\n    }\r\n    // Return the initial Bezier data:\r\n    // this.sendBezierData()\r\n  }\r\n\r\n  componentDidUpdate(prevProps) {\r\n    Streamlit.setFrameHeight()\r\n    if (this.props.args !== prevProps.args) {\r\n      this.setState({\r\n        originalData: this.props.args.data,\r\n        controlData: createControlData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        bezierData: createBezierData(\r\n          this.props.args.data,\r\n          this.props.args.options\r\n        ),\r\n        options: createOptions(this.props.args.options, this.props.theme),\r\n      })\r\n    }\r\n  }\r\n\r\n  sendBezierData() {\r\n    const newBezierData = this.convertBezierData(this.state.bezierData.datasets)\r\n    Streamlit.setComponentValue(newBezierData)\r\n  }\r\n\r\n  togglePan(enabled) {\r\n    this.chartRef.current.options.plugins.zoom.pan.enabled = enabled\r\n    this.chartRef.current.update(\"none\")\r\n  }\r\n\r\n  downHandler = (event) => {\r\n    const points = getElementAtEvent(this.chartRef.current, event, {\r\n      intersect: false,\r\n    })\r\n    if (points.length > 0) {\r\n      const dataset =\r\n        this.chartRef.current.data.datasets[points[0].datasetIndex]\r\n      if (dataset.isControlPoint) {\r\n        this.setState({ activePoint: points[0] })\r\n        this.togglePan(false)\r\n      }\r\n    }\r\n  }\r\n\r\n  moveHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      const chart = this.chartRef.current\r\n      const activePoint = this.state.activePoint\r\n      const position = getRelativePosition(event, chart)\r\n      const chartArea = chart.chartArea\r\n      const newYValue = calculateNewYValue(position, chartArea, chart.scales.y)\r\n      const newXValue = calculateNewXValue(position, chartArea, chart.scales.x)\r\n\r\n      // Update control point position\r\n      const datasetIndex = activePoint.datasetIndex\r\n      const dataset = chart.data.datasets[datasetIndex]\r\n      const pointIndex = activePoint.index\r\n      const deltaY = newYValue - dataset.data[pointIndex].y\r\n      const deltaX = newXValue - dataset.data[pointIndex].x\r\n\r\n      dataset.data[pointIndex].x = newXValue\r\n      dataset.data[pointIndex].y = newYValue\r\n\r\n      // Set new values in originalData\r\n      const datasetLabel = dataset.label\r\n      const originalDataset = this.state.originalData[datasetLabel] \r\n      const xValue = dataset.data[pointIndex].x\r\n      const yValue = dataset.data[pointIndex].y\r\n      originalDataset[\"x\"][pointIndex] = xValue\r\n      originalDataset[\"y\"][pointIndex] = yValue\r\n\r\n      // If activePoint index is 3, move points 2 and 4 as well\r\n      // If activePoint index is 3, update originalData for points 2 and 4 as well\r\n      const dataLen = dataset.data.length\r\n      if (pointIndex === 0) {\r\n        dataset.data[pointIndex + 1].x += deltaX\r\n        dataset.data[pointIndex + 1].y += deltaY\r\n\r\n        originalDataset[\"x\"][pointIndex + 1] += deltaX\r\n        originalDataset[\"y\"][pointIndex + 1] += deltaY\r\n      } else if (pointIndex === dataLen - 1) {\r\n        dataset.data[pointIndex - 1].x += deltaX\r\n        dataset.data[pointIndex - 1].y += deltaY\r\n\r\n        originalDataset[\"x\"][pointIndex - 1] += deltaX\r\n        originalDataset[\"y\"][pointIndex - 1] += deltaY\r\n      } else if (\r\n        pointIndex % 3 === 0 &&\r\n        pointIndex !== 0 &&\r\n        pointIndex !== dataLen - 1\r\n      ) {\r\n        dataset.data[pointIndex - 1].x += deltaX\r\n        dataset.data[pointIndex - 1].y += deltaY\r\n\r\n        dataset.data[pointIndex + 1].x += deltaX\r\n        dataset.data[pointIndex + 1].y += deltaY\r\n\r\n        originalDataset[\"x\"][pointIndex - 1] += deltaX\r\n        originalDataset[\"y\"][pointIndex - 1] += deltaY\r\n\r\n        originalDataset[\"x\"][pointIndex + 1] += deltaX\r\n        originalDataset[\"y\"][pointIndex + 1] += deltaY\r\n      } else if ((pointIndex + 1) % 3 === 0 && pointIndex + 1 !== dataLen - 1) {\r\n        dataset.data[pointIndex + 2].x -= deltaX\r\n        dataset.data[pointIndex + 2].y -= deltaY\r\n\r\n        originalDataset[\"x\"][pointIndex + 2] -= deltaX\r\n        originalDataset[\"y\"][pointIndex + 2] -= deltaY\r\n      } else if ((pointIndex - 1) % 3 === 0 && pointIndex - 1 !== 0) {\r\n        dataset.data[pointIndex - 2].x -= deltaX\r\n        dataset.data[pointIndex - 2].y -= deltaY\r\n        originalDataset[\"x\"][pointIndex - 2] -= deltaX\r\n        originalDataset[\"y\"][pointIndex - 2] -= deltaY\r\n      }\r\n\r\n      // Recalculate Bezier data\r\n      const bezierData = createBezierData(\r\n        this.state.originalData,\r\n        this.props.args.options\r\n      )\r\n      // Update state\r\n      this.setState({ bezierData })\r\n      chart.update(\"none\")\r\n    }\r\n  }\r\n\r\n  upHandler = (event) => {\r\n    if (this.state.activePoint) {\r\n      this.sendBezierData()\r\n      this.setState({ activePoint: null })\r\n      this.togglePan(true)\r\n    }\r\n  }\r\n\r\n  convertBezierData(bezierData) {\r\n    const result = {}\r\n    bezierData.forEach((dataset) => {\r\n      const trace = dataset.label.replace(\" (bezier)\", \"\")\r\n      result[trace] = {\r\n        x: [],\r\n        y: [],\r\n      }\r\n      dataset.data.forEach((point) => {\r\n        const { x, y } = point\r\n        const index = result[trace].x.findIndex(\r\n          (val, i) => val === x && result[trace].y[i] === y\r\n        )\r\n        if (index === -1) {\r\n          result[trace].x.push(x)\r\n          result[trace].y.push(y)\r\n        }\r\n      })\r\n    })\r\n    return result\r\n  }\r\n\r\n  render() {\r\n    return (\r\n      <Scatter\r\n        ref={this.chartRef}\r\n        data={{\r\n          datasets: [\r\n            ...this.state.controlData.datasets,\r\n            ...this.state.bezierData.datasets,\r\n            ...this.fixedData.datasets,\r\n          ],\r\n        }}\r\n        options={this.state.options}\r\n        onPointerDown={this.downHandler}\r\n        onPointerUp={this.upHandler}\r\n        onPointerMove={this.moveHandler}\r\n      />\r\n    )\r\n  }\r\n}\r\n\r\nexport default CubicBezierChart\r\n",
         "import LineChart from \"./LineChart/LineChart\";\r\nimport ScatterChart from \"./ScatterChart/ScatterChart\";\r\nimport BezierChart from \"./BezierChart/BezierChart\";\r\nimport CubicBezierChart from \"./CubicBezierChart/CubicBezierChart\";\r\n\r\nconst componentsMap = {\r\n  line_chart: LineChart,\r\n  scatter_chart: ScatterChart,\r\n  bezier_chart: BezierChart,\r\n  cubic_bezier_chart: CubicBezierChart,\r\n}\r\n\r\nexport default componentsMap\r\n",
         "import { withStreamlitConnection } from \"streamlit-component-lib\"\r\n\r\nimport React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport componentsMap from \"./components\"\r\n\r\nconst SelectComponent = (props) => {\r\n  const id = props.args[\"id\"]\r\n  const kw = props.args[\"kw\"]\r\n  const Component = componentsMap[id]\r\n  if (Component === undefined) {\r\n    throw new Error(`Component with id ${id} is not defined in componentsMap.`)\r\n  } else {\r\n    return <Component args={{ ...kw }} theme={props.theme} />\r\n  }\r\n}\r\n\r\nconst StreamlitComponent = withStreamlitConnection(SelectComponent)\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <StreamlitComponent />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `draggable-charts-1.2.5/draggable_charts/utils/callback.py` & `draggable-charts-1.2.6/draggable_charts/utils/callback.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/utils/component_func.py` & `draggable-charts-1.2.6/draggable_charts/utils/component_func.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/utils/options.py` & `draggable-charts-1.2.6/draggable_charts/utils/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         "#DD4477", "#66AA00", "#B82E2E", "#316395", "#994499", "#22AA99", "#AAAA11",
         "#6633CC", "#E67300", "#8B0707", "#329262", "#5574A6", "#651067"
     ],
     "border_dash": [(0, 0)],
     "point_radius": [3],
     "fill_gaps": False,
     "labels": {},
+    "x_format": True,
+    "y_format": True,
 }
 
 
 def set_options(data: dict, options: dict) -> dict:
     if not options:
         options = DEFAULT_OPTIONS.copy()
     options['x_type'] = _get_scale_type(data, 'x')
@@ -31,14 +33,17 @@
     
     options['colors'] = options.get('colors', DEFAULT_OPTIONS['colors'])
     options['border_dash'] = options.get('border_dash', DEFAULT_OPTIONS['border_dash'])
     options['point_radius'] = options.get('point_radius', DEFAULT_OPTIONS['point_radius'])
     options['fill_gaps'] = options.get('fill_gaps', DEFAULT_OPTIONS['fill_gaps'])
     options['labels'] = options.get('labels', DEFAULT_OPTIONS['labels'])
     
+    options['x_format'] = options.get('x_format', DEFAULT_OPTIONS['x_format'])
+    options['y_format'] = options.get('y_format', DEFAULT_OPTIONS['y_format'])
+    
     data = include_colors(data, options)
     data = include_border_dash(data, options)
     data = include_point_radius(data, options)
     return data, options
 
 
 def include_colors(data: dict, options: dict) -> dict:
```

### Comparing `draggable-charts-1.2.5/draggable_charts/widgets/bezierchart.py` & `draggable-charts-1.2.6/draggable_charts/widgets/bezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/widgets/cubicbezierchart.py` & `draggable-charts-1.2.6/draggable_charts/widgets/cubicbezierchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/widgets/linechart.py` & `draggable-charts-1.2.6/draggable_charts/widgets/linechart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts/widgets/scatterchart.py` & `draggable-charts-1.2.6/draggable_charts/widgets/scatterchart.py`

 * *Files identical despite different names*

### Comparing `draggable-charts-1.2.5/draggable_charts.egg-info/PKG-INFO` & `draggable-charts-1.2.6/draggable_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-charts
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.
 Home-page: https://github.com/balexandermunoz/draggable-charts
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
```

### Comparing `draggable-charts-1.2.5/draggable_charts.egg-info/SOURCES.txt` & `draggable-charts-1.2.6/draggable_charts.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 draggable_charts.egg-info/SOURCES.txt
 draggable_charts.egg-info/dependency_links.txt
 draggable_charts.egg-info/requires.txt
 draggable_charts.egg-info/top_level.txt
 draggable_charts/frontend/build/asset-manifest.json
 draggable_charts/frontend/build/bootstrap.min.css
 draggable_charts/frontend/build/index.html
-draggable_charts/frontend/build/static/js/main.41dd267d.js
-draggable_charts/frontend/build/static/js/main.41dd267d.js.LICENSE.txt
-draggable_charts/frontend/build/static/js/main.41dd267d.js.map
+draggable_charts/frontend/build/static/js/main.8018b5ba.js
+draggable_charts/frontend/build/static/js/main.8018b5ba.js.LICENSE.txt
+draggable_charts/frontend/build/static/js/main.8018b5ba.js.map
 draggable_charts/utils/__init__.py
 draggable_charts/utils/callback.py
 draggable_charts/utils/component_func.py
 draggable_charts/utils/options.py
 draggable_charts/widgets/__init__.py
 draggable_charts/widgets/bezierchart.py
 draggable_charts/widgets/cubicbezierchart.py
```

### Comparing `draggable-charts-1.2.5/setup.py` & `draggable-charts-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-charts",
-    version="1.2.5",
+    version="1.2.6",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component library for interactive charts in chartjs. Draggable line, scatter, and bezier charts. The updated data of the chart is returned after user interaction.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/balexandermunoz/draggable-charts",
     packages=setuptools.find_packages(),
```
